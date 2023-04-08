# Comparing `tmp/idem-7.6.tar.gz` & `tmp/idem-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/idem-7.6.tar", last modified: Sat Oct 24 09:08:21 2020, max compression
+gzip compressed data, was "idem-9.tar", last modified: Thu Jan 28 21:04:52 2021, max compression
```

## Comparing `idem-7.6.tar` & `idem-9.tar`

### file list

```diff
@@ -1,83 +1,85 @@
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.841789 idem-7.6/
--rw-r--r--   0 akmod     (1000) akmod     (1000)       43 2020-01-29 19:58:44.000000 idem-7.6/MANIFEST.in
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4664 2020-10-24 09:08:21.841789 idem-7.6/PKG-INFO
--rw-r--r--   0 akmod     (1000) akmod     (1000)     3484 2020-10-24 08:55:24.000000 idem-7.6/README.rst
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.838456 idem-7.6/idem/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     3003 2020-07-30 20:32:48.000000 idem-7.6/idem/conf.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.838456 idem-7.6/idem/exec/
--rw-r--r--   0 akmod     (1000) akmod     (1000)       67 2020-05-18 19:06:09.000000 idem-7.6/idem/exec/test.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.838456 idem-7.6/idem/idem/
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.838456 idem-7.6/idem/idem/ccomps/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1271 2020-05-18 19:06:09.000000 idem-7.6/idem/idem/ccomps/exclude.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     3529 2020-05-18 19:06:09.000000 idem-7.6/idem/idem/ccomps/extend.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     3649 2020-05-18 19:06:09.000000 idem-7.6/idem/idem/ccomps/low.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     9231 2020-05-18 19:06:09.000000 idem-7.6/idem/idem/ccomps/req_in.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     2274 2020-05-18 19:06:09.000000 idem-7.6/idem/idem/ccomps/treq.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     6998 2020-05-18 19:06:09.000000 idem-7.6/idem/idem/ccomps/verify.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.838456 idem-7.6/idem/idem/compiler/
--rw-r--r--   0 akmod     (1000) akmod     (1000)      257 2020-05-18 19:06:09.000000 idem-7.6/idem/idem/compiler/0010_extend.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      180 2020-05-18 19:06:09.000000 idem-7.6/idem/idem/compiler/0020_verify_high.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      185 2020-05-18 19:06:09.000000 idem-7.6/idem/idem/compiler/0030_req_in.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      175 2020-05-18 19:06:09.000000 idem-7.6/idem/idem/compiler/0040_exclude.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      216 2020-05-18 19:06:09.000000 idem-7.6/idem/idem/compiler/0050_compile.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      212 2020-05-18 19:06:09.000000 idem-7.6/idem/idem/compiler/0060_treq.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1027 2020-10-24 08:55:29.000000 idem-7.6/idem/idem/ex.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      646 2020-07-17 22:43:59.000000 idem-7.6/idem/idem/get.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     3960 2020-10-24 08:30:12.000000 idem-7.6/idem/idem/init.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.838456 idem-7.6/idem/idem/mod/
--rw-r--r--   0 akmod     (1000) akmod     (1000)      976 2020-10-24 08:37:00.000000 idem-7.6/idem/idem/mod/acct.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      416 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/mod/aggregate.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      446 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/mod/init.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.841789 idem-7.6/idem/idem/req/
--rw-r--r--   0 akmod     (1000) akmod     (1000)      319 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/req/init.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      210 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/req/listen.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      151 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/req/onchanges.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      178 2020-05-07 19:03:30.000000 idem-7.6/idem/idem/req/onchanges_any.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      127 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/req/onfail.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      206 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/req/prereq.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      182 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/req/require.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      209 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/req/require_any.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.841789 idem-7.6/idem/idem/req/seq/
--rw-r--r--   0 akmod     (1000) akmod     (1000)      451 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/req/seq/init.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1436 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/req/seq/prereq.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1947 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/req/seq/straight.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      162 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/req/watch.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     9167 2020-07-17 22:32:13.000000 idem-7.6/idem/idem/resolve.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.841789 idem-7.6/idem/idem/resolver/
--rw-r--r--   0 akmod     (1000) akmod     (1000)      245 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/resolver/all.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      399 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/resolver/any.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      480 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/resolver/init.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.841789 idem-7.6/idem/idem/rules/
--rw-r--r--   0 akmod     (1000) akmod     (1000)      529 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/rules/changes.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      309 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/rules/changes_post.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4343 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/rules/init.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      510 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/rules/post_low.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      939 2020-06-25 05:11:20.000000 idem-7.6/idem/idem/rules/prereq.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      458 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/rules/result.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.841789 idem-7.6/idem/idem/run/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1486 2020-07-17 22:46:10.000000 idem-7.6/idem/idem/run/init.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      787 2020-06-25 05:42:45.000000 idem-7.6/idem/idem/run/parallel.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      671 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/run/serial.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.841789 idem-7.6/idem/idem/sls/
--rw-r--r--   0 akmod     (1000) akmod     (1000)      600 2020-05-18 19:06:09.000000 idem-7.6/idem/idem/sls/file_sls.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     2013 2020-10-23 23:10:32.000000 idem-7.6/idem/idem/state.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)     7335 2020-04-23 18:45:14.000000 idem-7.6/idem/idem/tools.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.841789 idem-7.6/idem/output/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1492 2020-05-07 19:53:07.000000 idem-7.6/idem/output/idem.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)      134 2020-04-23 18:45:14.000000 idem-7.6/idem/scripts.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.841789 idem-7.6/idem/states/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     5267 2020-07-30 20:31:20.000000 idem-7.6/idem/states/test.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.841789 idem-7.6/idem/tool/
--rw-r--r--   0 akmod     (1000) akmod     (1000)       48 2020-07-30 20:38:42.000000 idem-7.6/idem/tool/test.py
--rw-r--r--   0 akmod     (1000) akmod     (1000)       40 2020-10-24 09:08:19.000000 idem-7.6/idem/version.py
-drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2020-10-24 09:08:21.838456 idem-7.6/idem.egg-info/
--rw-r--r--   0 akmod     (1000) akmod     (1000)     4664 2020-10-24 09:08:21.000000 idem-7.6/idem.egg-info/PKG-INFO
--rw-r--r--   0 akmod     (1000) akmod     (1000)     1562 2020-10-24 09:08:21.000000 idem-7.6/idem.egg-info/SOURCES.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)        1 2020-10-24 09:08:21.000000 idem-7.6/idem.egg-info/dependency_links.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)       45 2020-10-24 09:08:21.000000 idem-7.6/idem.egg-info/entry_points.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)       71 2020-10-24 09:08:21.000000 idem-7.6/idem.egg-info/requires.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)        5 2020-10-24 09:08:21.000000 idem-7.6/idem.egg-info/top_level.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)       14 2020-07-30 20:58:26.000000 idem-7.6/requirements-test.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)       71 2020-06-24 21:20:44.000000 idem-7.6/requirements.txt
--rw-r--r--   0 akmod     (1000) akmod     (1000)       38 2020-10-24 09:08:21.841789 idem-7.6/setup.cfg
--rw-r--r--   0 akmod     (1000) akmod     (1000)     2135 2020-04-23 18:45:14.000000 idem-7.6/setup.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.756329 idem-9/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       43 2020-11-23 10:02:08.000000 idem-9/MANIFEST.in
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     4662 2021-01-28 21:04:52.756329 idem-9/PKG-INFO
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     3484 2020-11-23 10:02:06.000000 idem-9/README.rst
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       71 2021-01-27 21:40:24.000000 idem-9/__build_requirements.txt
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.749663 idem-9/idem/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     3003 2021-01-13 00:49:35.000000 idem-9/idem/conf.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.749663 idem-9/idem/exec/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      103 2021-01-27 21:43:27.000000 idem-9/idem/exec/test.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.749663 idem-9/idem/idem/
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.749663 idem-9/idem/idem/ccomps/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     1271 2020-11-23 10:02:07.000000 idem-9/idem/idem/ccomps/exclude.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     3529 2020-11-23 10:02:07.000000 idem-9/idem/idem/ccomps/extend.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     3649 2020-11-23 10:02:07.000000 idem-9/idem/idem/ccomps/low.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     9231 2020-11-23 10:02:07.000000 idem-9/idem/idem/ccomps/req_in.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     2274 2020-11-23 10:02:07.000000 idem-9/idem/idem/ccomps/treq.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     6998 2020-11-23 10:02:07.000000 idem-9/idem/idem/ccomps/verify.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.749663 idem-9/idem/idem/compiler/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      257 2020-11-23 10:02:07.000000 idem-9/idem/idem/compiler/0010_extend.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      180 2020-11-23 10:02:07.000000 idem-9/idem/idem/compiler/0020_verify_high.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      185 2020-11-23 10:02:07.000000 idem-9/idem/idem/compiler/0030_req_in.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      175 2020-11-23 10:02:07.000000 idem-9/idem/idem/compiler/0040_exclude.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      216 2020-11-23 10:02:07.000000 idem-9/idem/idem/compiler/0050_compile.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      212 2021-01-13 00:49:35.000000 idem-9/idem/idem/compiler/0060_treq.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     1919 2021-01-27 21:43:27.000000 idem-9/idem/idem/ex.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      608 2021-01-27 21:43:27.000000 idem-9/idem/idem/get.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     3861 2021-01-27 21:43:27.000000 idem-9/idem/idem/init.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.752996 idem-9/idem/idem/mod/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      976 2020-11-23 10:02:08.000000 idem-9/idem/idem/mod/acct.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      416 2020-11-23 10:02:07.000000 idem-9/idem/idem/mod/aggregate.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      446 2020-11-23 10:02:07.000000 idem-9/idem/idem/mod/init.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.752996 idem-9/idem/idem/req/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      319 2020-11-23 10:02:07.000000 idem-9/idem/idem/req/init.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      210 2020-11-23 10:02:07.000000 idem-9/idem/idem/req/listen.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      151 2020-11-23 10:02:07.000000 idem-9/idem/idem/req/onchanges.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      178 2020-11-23 10:02:07.000000 idem-9/idem/idem/req/onchanges_any.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      127 2020-11-23 10:02:07.000000 idem-9/idem/idem/req/onfail.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      206 2020-11-23 10:02:07.000000 idem-9/idem/idem/req/prereq.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      182 2020-11-23 10:02:07.000000 idem-9/idem/idem/req/require.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      209 2020-11-23 10:02:07.000000 idem-9/idem/idem/req/require_any.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.752996 idem-9/idem/idem/req/seq/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      451 2020-11-23 10:02:07.000000 idem-9/idem/idem/req/seq/init.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     1436 2020-11-23 10:02:07.000000 idem-9/idem/idem/req/seq/prereq.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     1947 2020-11-23 10:02:07.000000 idem-9/idem/idem/req/seq/straight.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      162 2020-11-23 10:02:07.000000 idem-9/idem/idem/req/watch.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     9168 2021-01-27 21:43:27.000000 idem-9/idem/idem/resolve.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.752996 idem-9/idem/idem/resolver/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      245 2020-11-23 10:02:07.000000 idem-9/idem/idem/resolver/all.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      399 2020-11-23 10:02:07.000000 idem-9/idem/idem/resolver/any.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      480 2020-11-23 10:02:07.000000 idem-9/idem/idem/resolver/init.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.756329 idem-9/idem/idem/rules/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      529 2020-11-23 10:02:07.000000 idem-9/idem/idem/rules/changes.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      309 2020-11-23 10:02:07.000000 idem-9/idem/idem/rules/changes_post.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     4343 2021-01-13 00:49:35.000000 idem-9/idem/idem/rules/init.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      510 2020-11-23 10:02:07.000000 idem-9/idem/idem/rules/post_low.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      939 2020-11-23 10:02:07.000000 idem-9/idem/idem/rules/prereq.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      458 2020-11-23 10:02:07.000000 idem-9/idem/idem/rules/result.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.756329 idem-9/idem/idem/run/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     1486 2021-01-12 23:00:14.000000 idem-9/idem/idem/run/init.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      787 2021-01-13 00:49:35.000000 idem-9/idem/idem/run/parallel.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      671 2020-11-23 10:02:07.000000 idem-9/idem/idem/run/serial.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.756329 idem-9/idem/idem/sls/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      605 2021-01-27 21:43:27.000000 idem-9/idem/idem/sls/file_sls.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      614 2021-01-27 21:43:27.000000 idem-9/idem/idem/sls/json.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     4103 2021-01-27 21:43:27.000000 idem-9/idem/idem/state.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     7335 2020-11-23 10:02:07.000000 idem-9/idem/idem/tools.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.756329 idem-9/idem/output/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     1492 2020-11-23 10:02:08.000000 idem-9/idem/output/idem.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)      134 2020-11-23 10:02:08.000000 idem-9/idem/scripts.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.756329 idem-9/idem/states/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     5267 2021-01-13 00:49:35.000000 idem-9/idem/states/test.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.756329 idem-9/idem/tool/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       48 2020-11-23 10:02:07.000000 idem-9/idem/tool/test.py
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       38 2021-01-28 21:04:50.000000 idem-9/idem/version.py
+drwxr-xr-x   0 akmod     (1000) akmod     (1000)        0 2021-01-28 21:04:52.749663 idem-9/idem.egg-info/
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     4662 2021-01-28 21:04:52.000000 idem-9/idem.egg-info/PKG-INFO
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     1609 2021-01-28 21:04:52.000000 idem-9/idem.egg-info/SOURCES.txt
+-rw-r--r--   0 akmod     (1000) akmod     (1000)        1 2021-01-28 21:04:52.000000 idem-9/idem.egg-info/dependency_links.txt
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       45 2021-01-28 21:04:52.000000 idem-9/idem.egg-info/entry_points.txt
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       71 2021-01-28 21:04:52.000000 idem-9/idem.egg-info/requires.txt
+-rw-r--r--   0 akmod     (1000) akmod     (1000)        5 2021-01-28 21:04:52.000000 idem-9/idem.egg-info/top_level.txt
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       14 2020-11-23 10:02:07.000000 idem-9/requirements-test.txt
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       71 2020-11-23 10:02:08.000000 idem-9/requirements.txt
+-rw-r--r--   0 akmod     (1000) akmod     (1000)       38 2021-01-28 21:04:52.756329 idem-9/setup.cfg
+-rw-r--r--   0 akmod     (1000) akmod     (1000)     2135 2021-01-13 00:49:35.000000 idem-9/setup.py
```

### Comparing `idem-7.6/PKG-INFO` & `idem-9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem
-Version: 7.6
+Version: 9
 Summary: Transform configuration into idempotent action.
 Home-page: https://idem.readthedocs.io
 Author: Thomas S Hatch
 Author-email: thatch45@gmail.com
 License: UNKNOWN
 Description: ====
         Idem
```

### Comparing `idem-7.6/README.rst` & `idem-9/README.rst`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/conf.py` & `idem-9/idem/conf.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/ccomps/exclude.py` & `idem-9/idem/idem/ccomps/exclude.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/ccomps/extend.py` & `idem-9/idem/idem/ccomps/extend.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/ccomps/low.py` & `idem-9/idem/idem/ccomps/low.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/ccomps/req_in.py` & `idem-9/idem/idem/ccomps/req_in.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/ccomps/treq.py` & `idem-9/idem/idem/ccomps/treq.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/ccomps/verify.py` & `idem-9/idem/idem/ccomps/verify.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/get.py` & `idem-9/idem/idem/get.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,13 +10,12 @@
     Cache the given file from the named reference point
     """
     for source in hub.idem.RUNS[name]["sls_sources"]:
         proto = source[: source.index(":")]
         path = sls.replace(".", "/")
         locs = [f"{path}.sls", f"{path}/init.sls"]
         for loc in locs:
-            full = os.path.join(source, loc)
             cfn = await hub.pop.ref.last(f"idem.sls.{proto}.cache")(
-                hub.idem.RUNS[name]["cache_dir"], full
+                hub.idem.RUNS[name]["cache_dir"], source, loc
             )
             if cfn:
                 return cfn
```

### Comparing `idem-7.6/idem/idem/init.py` & `idem-9/idem/idem/init.py`

 * *Files 15% similar despite different names*

```diff
@@ -72,35 +72,36 @@
 
 
 async def cli_sls(hub):
     """
     Execute the cli routine to run states
     """
     src = hub.idem.init.get_refs()
+    name = "cli"
     await hub.idem.state.apply(
-        "cli",
-        src["sls_sources"],
-        hub.OPT["idem"]["render"],
-        hub.OPT["idem"]["runtime"],
-        ["states"],
-        hub.OPT["idem"]["cache_dir"],
-        src["sls"],
-        hub.OPT["idem"]["test"],
-        hub.OPT["acct"]["acct_file"],
-        hub.OPT["acct"]["acct_key"],
-        hub.OPT["acct"]["acct_profile"],
+        name=name,
+        sls_sources=src["sls_sources"],
+        render=hub.OPT.idem.render,
+        runtime=hub.OPT.idem.runtime,
+        subs=["states"],
+        cache_dir=hub.OPT.idem.cache_dir,
+        sls=src["sls"],
+        test=hub.OPT.idem.test,
+        acct_file=hub.OPT.acct.acct_file,
+        acct_key=hub.OPT.acct.acct_key,
+        acct_profile=hub.OPT.acct.acct_profile,
     )
 
-    errors = hub.idem.RUNS["cli"]["errors"]
+    errors = hub.idem.RUNS[name]["errors"]
     if errors:
         display = getattr(hub, "output.nested.display")(errors)
         print(display)
         return
-    running = hub.idem.RUNS["cli"]["running"]
-    output = hub.OPT["idem"]["output"]
+    running = hub.idem.RUNS[name]["running"]
+    output = hub.OPT.idem.output
     display = getattr(hub, f"output.{output}.display")(running)
     print(display)
 
 
 async def cli_exec(hub):
     exec_path = hub.OPT.idem.exec_func
     exec_args = hub.OPT.idem.exec_args
@@ -109,26 +110,22 @@
     args = []
     kwargs = {}
     for arg in exec_args:
         if isinstance(arg, dict):
             kwargs.update(arg)
         else:
             args.append(arg)
-    try:
-        ret = await hub.idem.ex.run(
-            exec_path,
-            args,
-            kwargs,
-            hub.OPT.acct.acct_file,
-            hub.OPT.acct.acct_key,
-            hub.OPT.acct.acct_profile,
-        )
-    except AttributeError:
-        print(f"The desired execution is not available: {exec_path}")
-        return
+    ret = await hub.idem.ex.run(
+        exec_path,
+        args,
+        kwargs,
+        hub.OPT.acct.acct_file,
+        hub.OPT.acct.acct_key,
+        hub.OPT.acct.acct_profile,
+    )
     output = hub.OPT.idem.output
     # exec can't use the idem outputter
     # TODO in pop-config allow subcommands to have different defaults from their parent
     if output == "idem":
         output = "nested"
     display = getattr(hub, f"output.{output}.display")(ret)
     print(display)
```

### Comparing `idem-7.6/idem/idem/mod/acct.py` & `idem-9/idem/idem/mod/acct.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/req/seq/prereq.py` & `idem-9/idem/idem/req/seq/prereq.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/req/seq/straight.py` & `idem-9/idem/idem/req/seq/straight.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/resolve.py` & `idem-9/idem/idem/resolve.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     """
     rendered = {}
     for sls_ref, blocks in hub.idem.RUNS[name]["blocks"].items():
         cfn = hub.idem.RUNS[name]["sls_refs"][sls_ref]
         for bname, block in blocks.items():
             clear = True
             for key, val in block.get("keys", {}).items():
-                # TODO: This should be an aditional render requisite plugin
+                # TODO: This should be an additional render requisite plugin
                 # subsystem, change it to a subsystem as soon as any new conditionals
                 # are added!!
                 clear = False
                 if key == "require":
                     for tag, data in hub.idem.RUNS[name]["running"].items():
                         if data["name"] == val:
                             clear = True
```

### Comparing `idem-7.6/idem/idem/rules/changes.py` & `idem-9/idem/idem/rules/changes.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/rules/init.py` & `idem-9/idem/idem/rules/init.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/rules/prereq.py` & `idem-9/idem/idem/rules/prereq.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/run/init.py` & `idem-9/idem/idem/run/init.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/run/parallel.py` & `idem-9/idem/idem/run/parallel.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/run/serial.py` & `idem-9/idem/idem/run/serial.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/idem/state.py` & `idem-9/idem/idem/ex.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,98 +1,84 @@
 # Import python libs
 import asyncio
+from dict_tools import data
+from typing import Iterable, Any, Dict, Tuple
 
-__func_alias__ = {"compile_": "compile"}
+__func_alias__ = {"ctx_": "ctx"}
 
 
-def create(
+async def run(
     hub,
-    name,
-    sls_sources,
-    render,
-    runtime,
-    subs,
-    cache_dir,
-    test,
-    acct_file,
-    acct_key,
-    acct_profile,
+    path: str,
+    args: Tuple[Any],
+    kwargs: Dict[str, Any],
+    acct_file: str = None,
+    acct_key: str = None,
+    acct_profile: str = "default",
 ):
-    """
-    Create a new instance to execute against
-    """
-    hub.idem.RUNS[name] = {
-        "sls_sources": sls_sources,
-        "render": render,
-        "runtime": runtime,
-        "subs": subs,
-        "cache_dir": cache_dir,
-        "states": {},
-        "test": test,
-        "resolved": set(),
-        "files": set(),
-        "high": {},
-        "post_low": [],
-        "errors": [],
-        "iorder": 100000,
-        "sls_refs": {},
-        "blocks": {},
-        "running": {},
-        "run_num": 1,
-        "add_low": [],
-        "acct_profile": acct_profile,
-    }
-    if acct_file and acct_key:
-        hub.idem.RUNS[name]["acct"] = hub.acct.init.unlock(acct_file, acct_key)
+    args = [a for a in args]
+
+    if not path.startswith("exec."):
+        path = f"exec.{path}"
+
+    func = getattr(hub, path)
+    params = func.signature.parameters
+
+    if "ctx" in params:
+        ctx = await hub.idem.ex.ctx(path, acct_file, acct_key, acct_profile)
+        args.insert(0, ctx)
+
+    ret = func(*args, **kwargs)
+    if asyncio.iscoroutine(ret):
+        ret = await ret
+    return ret
 
 
-async def apply(
+async def ctx_(
     hub,
-    name,
-    sls_sources,
-    render,
-    runtime,
-    subs,
-    cache_dir,
-    sls,
-    test=False,
-    acct_file=None,
-    acct_key=None,
-    acct_profile="default",
+    path: str,
+    acct_file: str = None,
+    acct_key: str = None,
+    acct_profile: str = "default",
 ):
     """
-    Run idem!
-    """
-    hub.idem.state.create(
-        name,
-        sls_sources,
-        render,
-        runtime,
-        subs,
-        cache_dir,
-        test,
-        acct_file,
-        acct_key,
-        acct_profile,
-    )
-    # Get the sls file
-    # render it
-    # compile high data to "new" low data (bypass keyword issues)
-    # Run the low data using act/idem
-    await hub.idem.resolve.gather(name, *sls)
-    if hub.idem.RUNS[name]["errors"]:
-        return
-    await hub.idem.state.compile(name)
-    if hub.idem.RUNS[name]["errors"]:
-        return
-    ret = await hub.idem.run.init.start(name)
+    :param hub:
+    :param path:
+    :param acct_file:
+    :param acct_key:
+    :param acct_profile:
+    :return:
+    """
+    ctx = data.NamespaceDict()
+
+    first = path[path.index(".") + 1 :]
+    sname = first[: first.index(".")]
+    acct_paths = (f"exec.{sname}.ACCT", f"states.{sname}.ACCT")
 
+    if acct_file and acct_key:
+        ctx.acct = hub.acct.init.unlock(acct_file, acct_key)
 
-async def compile_(hub, name):
-    """
-    Compile the data defined in the given run name
-    """
-    for mod in hub.idem.compiler:
-        if hasattr(mod, "stage"):
-            ret = mod.stage(name)
-            if asyncio.iscoroutine(ret):
-                await ret
+    subs = set()
+    for name in acct_paths:
+        if hasattr(hub, name):
+            sub = getattr(hub, name)
+            if isinstance(sub, Iterable) and sub:
+                subs.update(set(sub))
+
+    ctx.acct = await hub.acct.init.gather(subs, acct_profile)
+
+    return ctx
+
+
+async def single(hub, path: str, *args, **kwargs):
+    acct_file = hub.OPT.acct.acct_file
+    acct_key = hub.OPT.acct.acct_key
+    acct_profile = hub.OPT.acct.get("acct_profile", "default")
+
+    return await hub.idem.ex.run(
+        path,
+        args=args,
+        kwargs=kwargs,
+        acct_file=acct_file,
+        acct_key=acct_key,
+        acct_profile=acct_profile,
+    )
```

### Comparing `idem-7.6/idem/idem/tools.py` & `idem-9/idem/idem/tools.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/output/idem.py` & `idem-9/idem/output/idem.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem/states/test.py` & `idem-9/idem/states/test.py`

 * *Files identical despite different names*

### Comparing `idem-7.6/idem.egg-info/PKG-INFO` & `idem-9/idem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem
-Version: 7.6
+Version: 9
 Summary: Transform configuration into idempotent action.
 Home-page: https://idem.readthedocs.io
 Author: Thomas S Hatch
 Author-email: thatch45@gmail.com
 License: UNKNOWN
 Description: ====
         Idem
```

### Comparing `idem-7.6/idem.egg-info/SOURCES.txt` & `idem-9/idem.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 MANIFEST.in
 README.rst
+__build_requirements.txt
 requirements-test.txt
 requirements.txt
 setup.py
 idem/conf.py
 idem/scripts.py
 idem/version.py
 idem.egg-info/PKG-INFO
@@ -55,10 +56,11 @@
 idem/idem/rules/post_low.py
 idem/idem/rules/prereq.py
 idem/idem/rules/result.py
 idem/idem/run/init.py
 idem/idem/run/parallel.py
 idem/idem/run/serial.py
 idem/idem/sls/file_sls.py
+idem/idem/sls/json.py
 idem/output/idem.py
 idem/states/test.py
 idem/tool/test.py
```

### Comparing `idem-7.6/setup.py` & `idem-9/setup.py`

 * *Files identical despite different names*

