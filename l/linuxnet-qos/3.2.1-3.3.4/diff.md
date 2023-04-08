# Comparing `tmp/linuxnet-qos-3.2.1.tar.gz` & `tmp/linuxnet-qos-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/panos/dvl/gitlab/qos/linuxnet-qos/dist/tmp7ekga3hf/linuxnet-qos-3.2.1.tar", last modified: Fri Feb 24 20:04:49 2023, max compression
+gzip compressed data, was "/home/panos/dvl/gitlab/qos/linuxnet-qos/dist/tmp_egeoisk/linuxnet-qos-3.3.4.tar", last modified: Sat Apr  8 20:38:41 2023, max compression
```

## Comparing `linuxnet-qos-3.2.1.tar` & `linuxnet-qos-3.3.4.tar`

### file list

```diff
@@ -1,73 +1,84 @@
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-02-24 20:04:49.000000 linuxnet-qos-3.2.1/
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-02-24 20:04:49.000000 linuxnet-qos-3.2.1/docs/
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-02-24 20:04:49.000000 linuxnet-qos-3.2.1/docs/extend/
--rw-r--r--   0 panos     (1001) users      (100)     2279 2023-02-22 06:09:41.000000 linuxnet-qos-3.2.1/docs/extend/filter.rst
--rw-r--r--   0 panos     (1001) users      (100)     2623 2023-02-22 06:09:41.000000 linuxnet-qos-3.2.1/docs/extend/parsing.rst
--rw-r--r--   0 panos     (1001) users      (100)     9505 2023-02-22 06:09:42.000000 linuxnet-qos-3.2.1/docs/extend/qdisc.rst
--rw-r--r--   0 panos     (1001) users      (100)     1070 2023-02-22 06:09:42.000000 linuxnet-qos-3.2.1/docs/extend/util.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-02-24 20:04:49.000000 linuxnet-qos-3.2.1/docs/filters/
--rw-r--r--   0 panos     (1001) users      (100)      923 2023-02-22 06:09:42.000000 linuxnet-qos-3.2.1/docs/filters/fwfilter.rst
--rw-r--r--   0 panos     (1001) users      (100)     2582 2023-02-22 06:09:43.000000 linuxnet-qos-3.2.1/docs/filters/u32filter.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-02-24 20:04:49.000000 linuxnet-qos-3.2.1/docs/qdiscs/
--rw-r--r--   0 panos     (1001) users      (100)     1133 2023-02-22 06:09:43.000000 linuxnet-qos-3.2.1/docs/qdiscs/fifo.rst
--rw-r--r--   0 panos     (1001) users      (100)     1371 2023-02-22 06:09:43.000000 linuxnet-qos-3.2.1/docs/qdiscs/fq_codel.rst
--rw-r--r--   0 panos     (1001) users      (100)     1279 2023-02-22 06:09:44.000000 linuxnet-qos-3.2.1/docs/qdiscs/htb.rst
--rw-r--r--   0 panos     (1001) users      (100)     1343 2023-02-22 06:09:44.000000 linuxnet-qos-3.2.1/docs/qdiscs/multiqueue.rst
--rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-22 06:09:44.000000 linuxnet-qos-3.2.1/docs/qdiscs/netem.rst
--rw-r--r--   0 panos     (1001) users      (100)     1311 2023-02-22 06:09:44.000000 linuxnet-qos-3.2.1/docs/qdiscs/prio.rst
--rw-r--r--   0 panos     (1001) users      (100)     1351 2023-02-22 06:09:45.000000 linuxnet-qos-3.2.1/docs/qdiscs/sfq.rst
--rw-r--r--   0 panos     (1001) users      (100)      905 2023-02-20 19:38:13.000000 linuxnet-qos-3.2.1/docs/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     2819 2023-02-20 19:39:24.000000 linuxnet-qos-3.2.1/docs/conf.py
--rw-r--r--   0 panos     (1001) users      (100)     1079 2023-02-22 06:09:41.000000 linuxnet-qos-3.2.1/docs/config.rst
--rw-r--r--   0 panos     (1001) users      (100)     1454 2023-02-22 06:09:41.000000 linuxnet-qos-3.2.1/docs/exceptions.rst
--rw-r--r--   0 panos     (1001) users      (100)     1223 2023-02-22 06:09:42.000000 linuxnet-qos-3.2.1/docs/extensibility.rst
--rw-r--r--   0 panos     (1001) users      (100)     2151 2023-02-22 07:01:57.000000 linuxnet-qos-3.2.1/docs/index.rst
--rw-r--r--   0 panos     (1001) users      (100)      977 2023-02-22 06:09:43.000000 linuxnet-qos-3.2.1/docs/qdisc.rst
--rw-r--r--   0 panos     (1001) users      (100)     1678 2023-02-22 06:09:45.000000 linuxnet-qos-3.2.1/docs/qos_api.rst
--rw-r--r--   0 panos     (1001) users      (100)     1341 2023-02-22 06:09:45.000000 linuxnet-qos-3.2.1/docs/stats.rst
--rw-r--r--   0 panos     (1001) users      (100)     1279 2023-02-22 06:09:45.000000 linuxnet-qos-3.2.1/docs/traffic_filters.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-02-24 20:04:49.000000 linuxnet-qos-3.2.1/linuxnet/
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-02-24 20:04:49.000000 linuxnet-qos-3.2.1/linuxnet/qos/
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-02-24 20:04:49.000000 linuxnet-qos-3.2.1/linuxnet/qos/filters/
--rw-r--r--   0 panos     (1001) users      (100)     1160 2023-02-22 06:09:39.000000 linuxnet-qos-3.2.1/linuxnet/qos/filters/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     7106 2023-02-22 06:09:39.000000 linuxnet-qos-3.2.1/linuxnet/qos/filters/filter.py
--rw-r--r--   0 panos     (1001) users      (100)     5058 2023-02-22 06:09:38.000000 linuxnet-qos-3.2.1/linuxnet/qos/filters/fwfilter.py
--rw-r--r--   0 panos     (1001) users      (100)    28800 2023-02-22 06:09:39.000000 linuxnet-qos-3.2.1/linuxnet/qos/filters/u32filter.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-02-24 20:04:49.000000 linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/
--rw-r--r--   0 panos     (1001) users      (100)     1029 2023-02-22 06:09:36.000000 linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     5488 2023-02-22 06:09:36.000000 linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/fifo.py
--rw-r--r--   0 panos     (1001) users      (100)    13787 2023-02-22 06:09:37.000000 linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/fq_codel.py
--rw-r--r--   0 panos     (1001) users      (100)    20192 2023-02-22 06:09:37.000000 linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/htb.py
--rw-r--r--   0 panos     (1001) users      (100)     3581 2023-02-22 06:09:37.000000 linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/multiqueue.py
--rw-r--r--   0 panos     (1001) users      (100)    11284 2023-02-22 06:09:38.000000 linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/netem.py
--rw-r--r--   0 panos     (1001) users      (100)     7509 2023-02-22 06:09:37.000000 linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/prio.py
--rw-r--r--   0 panos     (1001) users      (100)    24672 2023-02-22 06:09:38.000000 linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/qdisc.py
--rw-r--r--   0 panos     (1001) users      (100)     5769 2023-02-22 06:09:38.000000 linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/sfq.py
--rw-r--r--   0 panos     (1001) users      (100)     1284 2023-02-22 06:09:39.000000 linuxnet-qos-3.2.1/linuxnet/qos/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    24696 2023-02-22 06:09:34.000000 linuxnet-qos-3.2.1/linuxnet/qos/config.py
--rw-r--r--   0 panos     (1001) users      (100)      907 2023-02-22 06:09:40.000000 linuxnet-qos-3.2.1/linuxnet/qos/deps.py
--rw-r--r--   0 panos     (1001) users      (100)     4238 2023-02-22 06:09:39.000000 linuxnet-qos-3.2.1/linuxnet/qos/exceptions.py
--rw-r--r--   0 panos     (1001) users      (100)     1636 2023-02-22 06:09:40.000000 linuxnet-qos-3.2.1/linuxnet/qos/extension.py
--rw-r--r--   0 panos     (1001) users      (100)     5369 2023-02-22 06:09:34.000000 linuxnet-qos-3.2.1/linuxnet/qos/handle.py
--rw-r--r--   0 panos     (1001) users      (100)      893 2023-02-22 06:09:40.000000 linuxnet-qos-3.2.1/linuxnet/qos/metadata.py
--rw-r--r--   0 panos     (1001) users      (100)    28944 2023-02-22 06:09:34.000000 linuxnet-qos-3.2.1/linuxnet/qos/parsers.py
--rw-r--r--   0 panos     (1001) users      (100)     4148 2023-02-22 06:09:36.000000 linuxnet-qos-3.2.1/linuxnet/qos/tcunit.py
--rw-r--r--   0 panos     (1001) users      (100)     2968 2023-02-22 06:09:36.000000 linuxnet-qos-3.2.1/linuxnet/qos/util.py
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-02-20 19:27:55.000000 linuxnet-qos-3.2.1/linuxnet/__init__.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-02-24 20:04:49.000000 linuxnet-qos-3.2.1/linuxnet_qos.egg-info/
--rw-r--r--   0 panos     (1001) users      (100)     2374 2023-02-24 20:04:48.000000 linuxnet-qos-3.2.1/linuxnet_qos.egg-info/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     1378 2023-02-24 20:04:48.000000 linuxnet-qos-3.2.1/linuxnet_qos.egg-info/SOURCES.txt
--rw-r--r--   0 panos     (1001) users      (100)        1 2023-02-24 20:04:48.000000 linuxnet-qos-3.2.1/linuxnet_qos.egg-info/dependency_links.txt
--rw-r--r--   0 panos     (1001) users      (100)        9 2023-02-24 20:04:48.000000 linuxnet-qos-3.2.1/linuxnet_qos.egg-info/top_level.txt
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-02-24 20:04:49.000000 linuxnet-qos-3.2.1/tests/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-02-22 06:58:21.000000 linuxnet-qos-3.2.1/tests/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    19203 2023-02-22 06:09:40.000000 linuxnet-qos-3.2.1/tests/qos_test.py
--rw-r--r--   0 panos     (1001) users      (100)    18811 2023-02-20 19:37:02.000000 linuxnet-qos-3.2.1/.pylintrc
--rw-r--r--   0 panos     (1001) users      (100)       89 2023-02-24 19:59:55.000000 linuxnet-qos-3.2.1/CHANGELOG.md
--rw-r--r--   0 panos     (1001) users      (100)    32387 2023-02-20 19:31:11.000000 linuxnet-qos-3.2.1/LICENSE
--rw-r--r--   0 panos     (1001) users      (100)      271 2023-02-20 19:36:39.000000 linuxnet-qos-3.2.1/MANIFEST.in
--rw-r--r--   0 panos     (1001) users      (100)     5135 2023-02-20 19:36:02.000000 linuxnet-qos-3.2.1/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     1477 2023-02-22 07:01:39.000000 linuxnet-qos-3.2.1/README.md
--rw-r--r--   0 panos     (1001) users      (100)     4993 2023-02-22 06:57:50.000000 linuxnet-qos-3.2.1/setup.py
--rw-r--r--   0 panos     (1001) users      (100)     2374 2023-02-24 20:04:49.000000 linuxnet-qos-3.2.1/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)       38 2023-02-24 20:04:49.000000 linuxnet-qos-3.2.1/setup.cfg
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/docs/
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/docs/actions/
+-rw-r--r--   0 panos     (1001) users      (100)      937 2023-04-08 20:07:35.000000 linuxnet-qos-3.3.4/docs/actions/mirred.rst
+-rw-r--r--   0 panos     (1001) users      (100)      992 2023-04-08 20:07:36.000000 linuxnet-qos-3.3.4/docs/actions/police.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/docs/extend/
+-rw-r--r--   0 panos     (1001) users      (100)     2279 2023-02-22 06:09:41.000000 linuxnet-qos-3.3.4/docs/extend/filter.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2653 2023-04-08 20:07:32.000000 linuxnet-qos-3.3.4/docs/extend/parsing.rst
+-rw-r--r--   0 panos     (1001) users      (100)     9505 2023-02-22 06:09:42.000000 linuxnet-qos-3.3.4/docs/extend/qdisc.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1070 2023-02-22 06:09:42.000000 linuxnet-qos-3.3.4/docs/extend/util.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/docs/filters/
+-rw-r--r--   0 panos     (1001) users      (100)      923 2023-02-22 06:09:42.000000 linuxnet-qos-3.3.4/docs/filters/fwfilter.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2582 2023-02-22 06:09:43.000000 linuxnet-qos-3.3.4/docs/filters/u32filter.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/docs/qdiscs/
+-rw-r--r--   0 panos     (1001) users      (100)     1133 2023-02-22 06:09:43.000000 linuxnet-qos-3.3.4/docs/qdiscs/fifo.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1371 2023-02-22 06:09:43.000000 linuxnet-qos-3.3.4/docs/qdiscs/fq_codel.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1279 2023-02-22 06:09:44.000000 linuxnet-qos-3.3.4/docs/qdiscs/htb.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1282 2023-04-08 20:07:35.000000 linuxnet-qos-3.3.4/docs/qdiscs/ingress.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1343 2023-02-22 06:09:44.000000 linuxnet-qos-3.3.4/docs/qdiscs/multiqueue.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-22 06:09:44.000000 linuxnet-qos-3.3.4/docs/qdiscs/netem.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1311 2023-02-22 06:09:44.000000 linuxnet-qos-3.3.4/docs/qdiscs/prio.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1351 2023-02-22 06:09:45.000000 linuxnet-qos-3.3.4/docs/qdiscs/sfq.rst
+-rw-r--r--   0 panos     (1001) users      (100)      905 2023-02-20 19:38:13.000000 linuxnet-qos-3.3.4/docs/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     2819 2023-02-20 19:39:24.000000 linuxnet-qos-3.3.4/docs/conf.py
+-rw-r--r--   0 panos     (1001) users      (100)     1079 2023-02-22 06:09:41.000000 linuxnet-qos-3.3.4/docs/config.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1454 2023-02-22 06:09:41.000000 linuxnet-qos-3.3.4/docs/exceptions.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1223 2023-02-22 06:09:42.000000 linuxnet-qos-3.3.4/docs/extensibility.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2151 2023-02-22 07:01:57.000000 linuxnet-qos-3.3.4/docs/index.rst
+-rw-r--r--   0 panos     (1001) users      (100)      977 2023-02-22 06:09:43.000000 linuxnet-qos-3.3.4/docs/qdisc.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1789 2023-04-08 20:07:33.000000 linuxnet-qos-3.3.4/docs/qos_api.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1341 2023-02-22 06:09:45.000000 linuxnet-qos-3.3.4/docs/stats.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2065 2023-04-08 20:07:36.000000 linuxnet-qos-3.3.4/docs/traffic_actions.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1279 2023-02-22 06:09:45.000000 linuxnet-qos-3.3.4/docs/traffic_filters.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet/
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet/qos/
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet/qos/actions/
+-rw-r--r--   0 panos     (1001) users      (100)      816 2023-04-08 20:07:34.000000 linuxnet-qos-3.3.4/linuxnet/qos/actions/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     2816 2023-04-08 20:07:34.000000 linuxnet-qos-3.3.4/linuxnet/qos/actions/action.py
+-rw-r--r--   0 panos     (1001) users      (100)     5141 2023-04-08 20:07:35.000000 linuxnet-qos-3.3.4/linuxnet/qos/actions/mirred.py
+-rw-r--r--   0 panos     (1001) users      (100)     5066 2023-04-08 20:07:34.000000 linuxnet-qos-3.3.4/linuxnet/qos/actions/police.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet/qos/filters/
+-rw-r--r--   0 panos     (1001) users      (100)     1160 2023-02-22 06:09:39.000000 linuxnet-qos-3.3.4/linuxnet/qos/filters/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     8006 2023-04-08 20:07:30.000000 linuxnet-qos-3.3.4/linuxnet/qos/filters/filter.py
+-rw-r--r--   0 panos     (1001) users      (100)     5939 2023-04-08 20:07:30.000000 linuxnet-qos-3.3.4/linuxnet/qos/filters/fwfilter.py
+-rw-r--r--   0 panos     (1001) users      (100)    31301 2023-04-08 20:07:30.000000 linuxnet-qos-3.3.4/linuxnet/qos/filters/u32filter.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/
+-rw-r--r--   0 panos     (1001) users      (100)     1029 2023-02-22 06:09:36.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     5501 2023-04-08 20:07:28.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/fifo.py
+-rw-r--r--   0 panos     (1001) users      (100)    13821 2023-04-08 20:07:28.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/fq_codel.py
+-rw-r--r--   0 panos     (1001) users      (100)    20192 2023-02-22 06:09:37.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/htb.py
+-rw-r--r--   0 panos     (1001) users      (100)     2357 2023-04-08 20:07:33.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/ingress.py
+-rw-r--r--   0 panos     (1001) users      (100)     3581 2023-02-22 06:09:37.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/multiqueue.py
+-rw-r--r--   0 panos     (1001) users      (100)    11373 2023-04-08 20:07:29.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/netem.py
+-rw-r--r--   0 panos     (1001) users      (100)     7519 2023-04-08 20:07:28.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/prio.py
+-rw-r--r--   0 panos     (1001) users      (100)    25418 2023-04-08 20:07:29.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/qdisc.py
+-rw-r--r--   0 panos     (1001) users      (100)     5779 2023-04-08 20:07:29.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/sfq.py
+-rw-r--r--   0 panos     (1001) users      (100)     1322 2023-04-08 20:07:31.000000 linuxnet-qos-3.3.4/linuxnet/qos/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    26352 2023-04-08 20:07:31.000000 linuxnet-qos-3.3.4/linuxnet/qos/config.py
+-rw-r--r--   0 panos     (1001) users      (100)      907 2023-02-22 06:09:40.000000 linuxnet-qos-3.3.4/linuxnet/qos/deps.py
+-rw-r--r--   0 panos     (1001) users      (100)     4430 2023-04-08 20:07:31.000000 linuxnet-qos-3.3.4/linuxnet/qos/exceptions.py
+-rw-r--r--   0 panos     (1001) users      (100)     1636 2023-02-22 06:09:40.000000 linuxnet-qos-3.3.4/linuxnet/qos/extension.py
+-rw-r--r--   0 panos     (1001) users      (100)     5369 2023-02-22 06:09:34.000000 linuxnet-qos-3.3.4/linuxnet/qos/handle.py
+-rw-r--r--   0 panos     (1001) users      (100)      893 2023-04-08 20:07:32.000000 linuxnet-qos-3.3.4/linuxnet/qos/metadata.py
+-rw-r--r--   0 panos     (1001) users      (100)    36970 2023-04-08 20:07:30.000000 linuxnet-qos-3.3.4/linuxnet/qos/parsers.py
+-rw-r--r--   0 panos     (1001) users      (100)     4148 2023-02-22 06:09:36.000000 linuxnet-qos-3.3.4/linuxnet/qos/tcunit.py
+-rw-r--r--   0 panos     (1001) users      (100)     2968 2023-02-22 06:09:36.000000 linuxnet-qos-3.3.4/linuxnet/qos/util.py
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-02-20 19:27:55.000000 linuxnet-qos-3.3.4/linuxnet/__init__.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet_qos.egg-info/
+-rw-r--r--   0 panos     (1001) users      (100)     2374 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet_qos.egg-info/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     1632 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet_qos.egg-info/SOURCES.txt
+-rw-r--r--   0 panos     (1001) users      (100)        1 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet_qos.egg-info/dependency_links.txt
+-rw-r--r--   0 panos     (1001) users      (100)        9 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet_qos.egg-info/top_level.txt
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/tests/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-02-22 06:58:21.000000 linuxnet-qos-3.3.4/tests/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    31223 2023-04-08 20:07:32.000000 linuxnet-qos-3.3.4/tests/qos_test.py
+-rw-r--r--   0 panos     (1001) users      (100)    18811 2023-02-20 19:37:02.000000 linuxnet-qos-3.3.4/.pylintrc
+-rw-r--r--   0 panos     (1001) users      (100)      244 2023-04-08 20:11:06.000000 linuxnet-qos-3.3.4/CHANGELOG.md
+-rw-r--r--   0 panos     (1001) users      (100)    32387 2023-02-20 19:31:11.000000 linuxnet-qos-3.3.4/LICENSE
+-rw-r--r--   0 panos     (1001) users      (100)      271 2023-02-20 19:36:39.000000 linuxnet-qos-3.3.4/MANIFEST.in
+-rw-r--r--   0 panos     (1001) users      (100)     5135 2023-02-20 19:36:02.000000 linuxnet-qos-3.3.4/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     1477 2023-02-22 07:01:39.000000 linuxnet-qos-3.3.4/README.md
+-rw-r--r--   0 panos     (1001) users      (100)     4993 2023-02-22 06:57:50.000000 linuxnet-qos-3.3.4/setup.py
+-rw-r--r--   0 panos     (1001) users      (100)     2374 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)       38 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/setup.cfg
```

### Comparing `linuxnet-qos-3.2.1/docs/extend/filter.rst` & `linuxnet-qos-3.3.4/docs/extend/filter.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/extend/parsing.rst` & `linuxnet-qos-3.3.4/docs/extend/parsing.rst`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,18 @@
 The :meth:`TrafficFilterParser.register_filter` method must be invoked
 to register classes traffic filter classes.
 
 .. autoclass:: TrafficFilterParser
    :members:
    :member-order: bysource
 
+-------------
+
 .. autoclass:: FilterOutput
    :members:
    :member-order: bysource
 
+-------------
+
 .. autoclass:: FilterOutputLine
    :members:
    :member-order: bysource
```

### Comparing `linuxnet-qos-3.2.1/docs/extend/qdisc.rst` & `linuxnet-qos-3.3.4/docs/extend/qdisc.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/extend/util.rst` & `linuxnet-qos-3.3.4/docs/extend/util.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/filters/fwfilter.rst` & `linuxnet-qos-3.3.4/docs/filters/fwfilter.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/filters/u32filter.rst` & `linuxnet-qos-3.3.4/docs/filters/u32filter.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/qdiscs/fifo.rst` & `linuxnet-qos-3.3.4/docs/qdiscs/fifo.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/qdiscs/fq_codel.rst` & `linuxnet-qos-3.3.4/docs/qdiscs/fq_codel.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/qdiscs/htb.rst` & `linuxnet-qos-3.3.4/docs/qdiscs/htb.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/qdiscs/multiqueue.rst` & `linuxnet-qos-3.3.4/docs/qdiscs/multiqueue.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/qdiscs/netem.rst` & `linuxnet-qos-3.3.4/docs/qdiscs/netem.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/qdiscs/prio.rst` & `linuxnet-qos-3.3.4/docs/qdiscs/prio.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/qdiscs/sfq.rst` & `linuxnet-qos-3.3.4/docs/qdiscs/sfq.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/Makefile` & `linuxnet-qos-3.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/conf.py` & `linuxnet-qos-3.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/config.rst` & `linuxnet-qos-3.3.4/docs/config.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/exceptions.rst` & `linuxnet-qos-3.3.4/docs/exceptions.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/extensibility.rst` & `linuxnet-qos-3.3.4/docs/extensibility.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/index.rst` & `linuxnet-qos-3.3.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/qdisc.rst` & `linuxnet-qos-3.3.4/docs/qdisc.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/qos_api.rst` & `linuxnet-qos-3.3.4/docs/qos_api.rst`

 * *Files 8% similar despite different names*

```diff
@@ -32,19 +32,22 @@
 - Classes that provide access to queueing discipline
   :ref:`statistics <queuing_statistics>`; at a minimum, the statistics
   are those available
   via the :ref:`QStats <qstats>` class, but some queueing disciplines
   provide their own subclass with additional statistics
 - :ref:`Classes <traffic_filter>` that provide access
   to traffic filters
+- :ref:`Classes <traffic_action>` that provide access
+  to traffic actions (e.g. policing)
 
 
 .. toctree::
     :maxdepth: 2
     :hidden:
 
     config
     qdisc
     traffic_filters
+    traffic_actions
     stats
     exceptions
     extensibility
```

### Comparing `linuxnet-qos-3.2.1/docs/stats.rst` & `linuxnet-qos-3.3.4/docs/stats.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/docs/traffic_filters.rst` & `linuxnet-qos-3.3.4/docs/traffic_filters.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/filters/__init__.py` & `linuxnet-qos-3.3.4/linuxnet/qos/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/filters/filter.py` & `linuxnet-qos-3.3.4/linuxnet/qos/filters/filter.py`

 * *Files 13% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         """
         self.__protocol = protocol
         self.__prio = prio if prio is not None else -1
         self.__filter_type = filter_type
         self.__instantiated = False
         self.__dest_class_handle = dest_class_handle
         self.__filter_name = filter_name
+        self.__action_list = []
 
     def __str__(self):
         prio = 'NOPRIO' if self.__prio < 0 else f'0x{self.__prio:x}'
         return f'Filter({self.__protocol}/{prio}/{self.__filter_type})'
 
     def filter_creation_args(self) -> List[str]:
         """Returns a list of **tc(8)** arguments to create this filter
@@ -134,14 +135,30 @@
             _logger.error(
                 "%s: %s: attempt to change destination of instantiated filter",
                         self.set_dest_handle.__qualname__,
                         self)
             raise TcError(f"attempt to change filter {self} destination")
         self.__dest_class_handle = handle
 
+    def get_actions(self) -> List['TrafficAction']:
+        """Returns the action list for this filter
+        """
+        return self.__action_list
+
+    def add_action(self, action: 'TrafficAction') -> None:
+        """Add a filter action
+        """
+        if self.__instantiated:
+            _logger.error(
+                "%s: %s: attempt to add action to an instantiated filter",
+                        self.add_action.__qualname__,
+                        self)
+            raise TcError(f"attempt to add action to filter {self}")
+        self.__action_list.append(action)
+
     def _instantiate(self, owner) -> None:
         """Instantiate a filter by invoking the **tc(8)** command.
 
         :param owner: :class:`QClass`/:class:`QDisc` that is the parent of
             this filter
         """
         if self.__instantiated:
@@ -158,14 +175,20 @@
             cmd += ['prio', f'{self.__prio:d}']
         else:
             _logger.warning(
                 "instantiating filter %s with no priority -- "
                 "it will not be possible to delete",
                     self)
         cmd += self.filter_creation_args()
+        for action in self.__action_list:
+            cmd += ['action', action.get_kind()]
+            action_index = action.get_action_index()
+            if action_index is not None:
+                cmd += ['index', str(action_index)]
+            cmd += action.action_creation_args()
         config.tc_run(cmd, 'filter creation')
         self.__instantiated = True
 
     def _uninstantiate(self, owner) -> None:
         """Uninstantiate a filter by invoking the **tc(8)** command.
 
         :param owner: :class:`QClass`/:class:`QDisc` that is the parent of
```

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/filters/fwfilter.py` & `linuxnet-qos-3.3.4/linuxnet/qos/filters/fwfilter.py`

 * *Files 14% similar despite different names*

```diff
@@ -94,45 +94,63 @@
         Raises a :class:`TcError` if the filter is already instantiated.
         """
         if self.is_instantiated():
             raise TcError('cannot change fwmark of instantiated filter')
         self.__fwmark = fwmark
 
     @classmethod
-    def parse(cls, filt_output: FilterOutput) -> Optional[TrafficFilter]:
+    def parse(cls, filt_output: FilterOutput) -> TrafficFilter:
         """Parse the filter output in ``filt_output`` into a
         :class:`TrafficFilter` instance.
 
         :meta private:
         """
         #
         # The expected format of the filter output lines (after the
         # 'fw' filter type) is:
         #
         #    handle 0x100 classid 1:200
         #
+        # The classid is optional.
+        #
+        owner = filt_output.get_filter_owner()
         fwmark = None
         class_handle = None
+        action = None
         for filter_line in filt_output.filter_lines_iter():
-            fwmark = None
             field_iter = iter(filter_line)
             for field in field_iter:
                 if field == 'handle':
                     fwmark = int(next(field_iter), 16)
                 elif field == 'classid':
-                    class_handle = Handle.parse(next(field_iter))
+                    class_handle = Handle.parse(next(field_iter),
+                                                    owner.get_handle().major)
+                elif field == 'chain':
+                    _ = next(field_iter)
+                elif field == 'police':
+                    fields = [field] + list(field_iter)
+                    action = TrafficFilterParser.parse_action(fields,
+                                    filt_output.nonfilter_lines_iter())
                 else:
-                    raise TcParsingError(f"unexpected argument: {field}")
+                    reason = f"unexpected argument: {field}"
+                    line = str(filter_line)
+                    _logger.error("%s: %s line='%s' (owner=%s)",
+                        cls.parse.__qualname__, reason, line, owner)
+                    raise TcParsingError(reason, line=line)
             if fwmark is not None and class_handle is not None:
                 break
-        else:
-            return None
-        if filt_output.has_nonfilter_lines():
-            _logger.warning("ignoring non-filter lines in fw filter output")
-        return FwmarkIPFilter(
+        if fwmark is None:
+            reason = 'fw filter with no handle'
+            _logger.error("%s: %s (owner=%s)",
+                        cls.parse.__qualname__, reason, owner)
+            raise TcParsingError(reason)
+        traffic_filter = FwmarkIPFilter(
                         prio=filt_output.get_prio(),
                         dest_class_handle=class_handle,
                         fwmark=fwmark)
+        if action is not None:
+            traffic_filter.add_action(action)
+        return traffic_filter
 
 
 TrafficFilterParser.register_filter(filter_type='fw', protocol='ip',
                                                 klass=FwmarkIPFilter)
```

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/filters/u32filter.py` & `linuxnet-qos-3.3.4/linuxnet/qos/filters/u32filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -677,17 +677,17 @@
         mask = int(mask_str, 16)
         field = next(field_iter)
         if field != 'at':
             raise TcParsingError(f"expected 'at', found {field}")
         offset = int(next(field_iter))
         return cls._parse_u32_selector(value=value, mask=mask, offset=offset)
 
-    # pylint: disable=too-many-branches
+    # pylint: disable=too-many-branches, too-many-locals, too-many-statements
     @classmethod
-    def parse(cls, filt_output: FilterOutput) -> Optional[TrafficFilter]:
+    def parse(cls, filt_output: FilterOutput) -> TrafficFilter:
         """Parse the filter output in ``filt_output`` into a
         :class:`TrafficFilter` instance.
 
         :meta private:
         """
         #
         # When this library is used to create a U32 filter, the output
@@ -701,14 +701,15 @@
         #
         #   fh 801::800 order 2048 key ht 801 bkt 0 link 1:
         #
         # These will be ignored with a log warning.
         #
         class_handle = None
         filter_handle = None
+        is_terminal = False
         for filter_line in filt_output.filter_lines_iter():
             filter_handle = None
             field_iter = iter(filter_line)
             for field in field_iter:
                 try:
                     if field == 'fh':
                         filter_handle = U32FilterHandle.create_from_string(
@@ -737,56 +738,102 @@
                         field = next(field_iter)
                         if field != 'bkt':
                             raise TcParsingError(
                                         f"expecting 'bkt', found '{field}'",
                                         line=str(filter_line))
                         _ = int(next(field_iter))
                     elif field == 'flowid':
-                        class_handle = Handle.create_from_string(
-                                                        next(field_iter))
+                        if not is_terminal:
+                            class_handle = Handle.create_from_string(
+                                                        next(field_iter),
+                                                        default_major=0)
+                    elif field == 'terminal':
+                        is_terminal = True
                     elif field == 'not_in_hw':
                         pass
                     elif field == 'chain':
                         _ = int(next(field_iter))
                     else:
                         raise TcParsingError(f"unexpected argument: {field}",
                                                 line=str(filter_line))
                 except ValueError as valerr:
-                    raise TcParsingError(
-                        f"bad value for field: {field}",
-                        line=str(filter_line)) from valerr
+                    line = str(filter_line)
+                    reason = f"bad value for field: {field}"
+                    _logger.error("%s: %s line='%s' (owner=%s)",
+                            cls.parse.__qualname__, reason, line,
+                            filt_output.get_filter_owner())
+                    raise TcParsingError(reason, line=line) from valerr
                 except StopIteration as stopiter:
-                    raise TcParsingError(
-                        f"missing value for field: {field}",
-                        line=str(filter_line)) from stopiter
+                    line = str(filter_line)
+                    reason = f"missing value for field: {field}"
+                    _logger.error("%s: %s line='%s' (owner=%s)",
+                            cls.parse.__qualname__, reason, line,
+                            filt_output.get_filter_owner())
+                    raise TcParsingError(reason, line=line) from stopiter
             if class_handle is not None and filter_handle is not None:
                 break
-        else:
-            return None
+        if filter_handle is None:
+            reason = 'u32 filter with no handle'
+            _logger.error("%s: %s (owner=%s)",
+                            cls.parse.__qualname__, reason,
+                            filt_output.get_filter_owner())
+            raise TcParsingError('u32 filter with no handle')
         #
-        # If we get here, we have a filter handle and a (destination) class
-        # handle.
+        # If we get here, we have a filter handle and maybe a
+        # (destination) class handle.
         #
         # We now parse the non-filter lines; these lines look like this:
         #
         #       match 00000000/00000000 at 16
         #         hash mask 0000ff00 at 12
         #
         # We only handle 'match' lines here.
         #
         filter_selectors = []
-        for nonfilter_line in filt_output.nonfilter_lines_iter():
+        nfl_iter = filt_output.nonfilter_lines_iter()
+        action_present = False
+        for nonfilter_line in nfl_iter:
+            # lws: leading white-space
+            lws = len(nonfilter_line) - len(nonfilter_line.lstrip())
             fields = nonfilter_line.split()
+            if len(fields) == 0:
+                break
             if fields[0] == 'match':
                 selectors = cls._parse_selector_line(iter(fields[1:]))
                 filter_selectors.extend(selectors)
+            elif lws >= 2:
+                if fields[0] == 'action':
+                    #
+                    # Assume that all remaining lines are action-related
+                    # (I don't know if this is always the case)
+                    #
+                    nfl_iter.rewind()
+                    action_present = True
+                    break
+                _logger.warning("%s: unable to handle line: %s (owner=%s)",
+                                cls.parse.__qualname__,
+                                nonfilter_line, filt_output.get_filter_owner())
+            elif lws == 1:
+                # This is an action line; put the line back, and stop
+                # processing
+                nfl_iter.rewind()
+                action_present = True
+                break
             else:
-                _logger.warning("unable to handle line: %s", nonfilter_line)
+                # This should not happen as all non-filter lines are indented
+                _logger.warning("%s: unexpected line: %s (owner=%s)",
+                                cls.parse.__qualname__,
+                                nonfilter_line, filt_output.get_filter_owner())
+        if not action_present and class_handle is None:
+            _logger.warning(
+                "%s: no action and no dest class for filter %s (owner=%s)",
+                        cls.parse.__qualname__, filter_handle,
+                        filt_output.get_filter_owner())
         return U32IPFilter(
                         prio=filt_output.get_prio(),
                         dest_class_handle=class_handle,
                         filter_handle=filter_handle,
                         selectors=filter_selectors)
-    # pylint: enable=too-many-branches
+    # pylint: enable=too-many-branches, too-many-locals, too-many-statements
 
 TrafficFilterParser.register_filter(filter_type='u32', protocol='ip',
                                         klass=U32IPFilter)
```

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/__init__.py` & `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/fifo.py` & `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/fifo.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,22 +31,22 @@
 
 
 class PFifoFastQDisc(QDisc):
     """This class provides access to the pfifo_fast
     queueing discipline of Linux (see **tc-pfifo_fast(8)**).
     """
 
-    def __init__(self, qdisc_handle: Handle, parent_handle: Handle,
+    def __init__(self, qdisc_handle: Handle, parent_handle: Optional[Handle],
                     *,
                     txqueuelen: Optional[int] =None,
                     bands: Optional[int] =None,
                     priomap: Optional[Sequence[int]] =None):
         """
-        :param class_handle: handle of this :class:`PFifoFastQDisc`
-        :param parent_handle: handle of parent, ``None`` if this is a
+        :param qdisc_handle: handle of this :class:`PFifoFastQDisc`
+        :param parent_handle: handle of parent, or ``None`` if this is a
             root queuing discipline
         :param txqueuelen: as documented in **tc-pfifo_fast(8)**
         :param bands: as documented in **tc-pfifo_fast(8)**
         :param priomap: as documented in **tc-pfifo_fast(8)**
 
         Only ``txqueuelen`` is used when creating a new ``pfifo_fast``
         queuing discipline. If ``bands`` or ``priomap`` are specified,
```

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/fq_codel.py` & `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/fq_codel.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,21 +183,22 @@
 
 
 class FQCoDelQDisc(QDisc):      # pylint: disable=too-many-instance-attributes
     """This class provides access to the Fair Queuing (FQ) with
     Controlled Delay (fq_codel) queueing discipline (see **tc-fq_codel(8)**)
     """
 
-    def __init__(self, qdisc_handle: Handle, parent_handle: Handle, *,
+    def __init__(self, qdisc_handle: Handle, parent_handle: Optional[Handle],
+                        *,
                         limit: Optional[int], flows: Optional[int],
                         quantum: Optional[int], target: Optional[float],
                         interval: Optional[float],
                         memory_limit: Optional[int], ecn: Optional[bool]):
         """
-        :param class_handle: handle of this :class:`FQCoDelQDisc`
+        :param qdisc_handle: handle of this :class:`FQCoDelQDisc`
         :param parent_handle: handle of parent, ``None`` if this is a
             root queuing discipline
         :param limit: as documented in **tc-fq_codel(8)**
         :param flows: as documented in **tc-fq_codel(8)**
         :param quantum: as documented in **tc-fq_codel(8)**
         :param target: as documented in **tc-fq_codel(8)**
         :param interval: as documented in **tc-fq_codel(8)**
```

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/htb.py` & `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/htb.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/multiqueue.py` & `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/multiqueue.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/netem.py` & `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/netem.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,25 +35,26 @@
     """
 
     INT = 1
     TIME = 2
     PERCENT = 3
 
     def __init__(self, *argtypes, **kwargs):
-        self.__param = None
         self.__argtypes = argtypes
         self.__kwargs = kwargs
+        self.__param = None
         self.__values = []
 
-    def parse(self, param: str, field_iter) -> str:
+    def parse(self, param: str, field_iter) -> Optional[str]:
         """Parse the parameter values based on the stored argtypes.
 
         Returns the next field.
         """
         self.__param = param
+        self.__values = []
         try:
             for i, argtype in enumerate(self.__argtypes):
                 field = next(field_iter)
                 if argtype == self.INT:
                     self.__values.append(int(field))
                 elif argtype == self.TIME:
                     self.__values.append(timestr2float(field))
@@ -90,28 +91,28 @@
 
 
 class NetemQDisc(QDisc):
     """This class provides access to the ``netem``
     queueing discipline (see **tc-netem(8)**).
     """
 
-    def __init__(self, qdisc_handle: Handle, parent_handle: Handle,
+    def __init__(self, qdisc_handle: Handle, parent_handle: Optional[Handle],
                     *,
                     delay: Union[float, int, Tuple, None] =None,
                     limit: Optional[int] =None,
                     drop: Union[int, Tuple, None] =None,
                     duplicate: Union[int, Tuple, None] =None,
                     corrupt: Union[int, Tuple, None] =None,
                     reorder: Union[int, Tuple, None] =None,
                     gap: Optional[int] =None,
                     ):
         """
         :param qdisc_handle: :class:`Handle` of this :class:`NetemQDisc`
-        :param parent_handle: :class:`Handle` of the parent of this
-            :class:`QDisc`
+        :param parent_handle: :class:`Handle` of the parent :class:`QDisc`,
+            or ``None`` if this is a root queuing discipline
         :param delay: delay (in ms) added to each outgoing packet;
             ``delay`` can be specified as a :class:`float`, as an :class:`int`,
             or as a tuple of the form ``(delay, [jitter, [correlation]])``
         :param limit: packet limit
         :param drop: drop percentage;
             ``drop`` can be specified as an :class:`int`,
             or as a tuple of the form ``(percent, [correlation])``
```

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/prio.py` & `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/prio.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,19 +80,19 @@
     """This class provides access to the Priority queueing discipline
     of Linux (see **tc-prio(8)**).
     """
 
     DEFAULT_BANDS = 3
     DEFAULT_PRIOMAP = (1, 2, 2, 2, 1, 2, 0, 0 , 1, 1, 1, 1, 1, 1, 1, 1)
 
-    def __init__(self, qdisc_handle: Handle, parent_handle: Handle,
+    def __init__(self, qdisc_handle: Handle, parent_handle: Optional[Handle],
                     bands: Optional[int] =None,
                     priomap: Optional[Sequence[int]] =None):
         """
-        :param class_handle: handle of this :class:`PrioQDisc`
+        :param qdisc_handle: handle of this :class:`PrioQDisc`
         :param parent_handle: handle of parent, ``None`` if this is a
             root queuing discipline
         :param bands: as documented in **tc-prio(8)**
         :param priomap: as documented in **tc-prio(8)**
 
         The ``bands`` and ``priomap`` parameters must be consistent:
             * ``priomap`` must have 16 entries (number of Linux priorities)
```

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/qdisc.py` & `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/qdisc.py`

 * *Files 2% similar despite different names*

```diff
@@ -425,20 +425,15 @@
         traffic_filter._uninstantiate(owner=self)
         self.__filters.remove(traffic_filter)
 
     def get_description(self) -> str:
         """Return a string that *fully* describes this node
         (name + attributes)
         """
-        retval = str(self)
-        if self.__parent_handle is None:
-            retval += ' root'
-        else:
-            retval += f' parent {self.__parent_handle}'
-        return retval
+        raise NotImplementedError
 
     def dump(self, outfile: TextIO, level: int,
                 qclass_map: Mapping[Handle, 'QClass']) -> None:
         """Recursively dump this node and all its child classes to ``outfile``
         """
         prefix = '    ' * level
         print(prefix + self.get_description(), file=outfile)
@@ -487,14 +482,19 @@
         # A leaf class should have a qdisc; may be None if using a
         # default qdisc (pfifo)
         self.__qdisc = None
 
     def __str__(self):
         return f'QClass({self.get_handle()})'
 
+    def get_description(self) -> str:
+        """Return a string that *fully* describes this :class:`QCclass`
+        """
+        return f'{self} parent {self.get_parent_handle()}'
+
     def get_class_name(self) -> str:
         """Returns the class name
         """
         return self.__class_name
 
     def set_class_name(self, class_name: str) -> None:
         """Sets the class name
@@ -611,34 +611,40 @@
     def _instantiate_qdisc(self, config) -> None:
         """Invoke the **tc(8)** command to create the queuing discipline
         described by this object.
 
         :param config: a :class:`QDiscConfig` object
         """
         cmd = ['tc', 'qdisc', 'add', 'dev', config.get_interface()]
-        if self.is_root():
-            cmd.append('root')
+        if self.is_ingress():
+            cmd.append('ingress')
         else:
-            cmd.extend(['parent', str(self.get_parent_handle())])
-        cmd.extend(['handle', str(self.get_handle())])
-        # Derived Python class provides the qdisc-specific arguments
-        cmd.extend(self.qdisc_creation_args())
+            if self.is_root():
+                cmd.append('root')
+            else:
+                cmd.extend(['parent', str(self.get_parent_handle())])
+            cmd.extend(['handle', str(self.get_handle())])
+            # Derived Python class provides the qdisc-specific arguments
+            cmd.extend(self.qdisc_creation_args())
         self._instantiate('qdisc', cmd, config)
 
     def _uninstantiate_qdisc(self, config) -> None:
         """Invoke the **tc(8)** command to delete the queuing discipline
         described by this object.
 
         :param config: a :class:`QDiscConfig` object
         """
         cmd = ['tc', 'qdisc', 'del', 'dev', config.get_interface()]
-        if self.is_root():
-            cmd.append('root')
+        if self.is_ingress():
+            cmd.append('ingress')
         else:
-            cmd.extend(['handle', str(self.get_handle())])
+            if self.is_root():
+                cmd.append('root')
+            else:
+                cmd.extend(['handle', str(self.get_handle())])
         self._uninstantiate('qdisc', cmd, config)
 
     def qdisc_creation_args(self) -> List[str]:
         """Returns the qdisc-specific arguments passed to **tc(8)**
         to create the particular qdisc
 
         It must be implemented by the derived Python class.
@@ -652,14 +658,32 @@
 
     def is_default(self) -> bool:
         """Returns ``True`` if this :class:`QDisc` is the default qdisc used
         by the kernel.
         """
         return self.get_handle().major == 0
 
+    @staticmethod
+    def is_ingress() -> bool:
+        """Returns ``True`` if this :class:`QDisc` is the ingress qdisc
+        """
+        return False
+
+    def get_description(self) -> str:
+        """Return a string that *fully* describes this :class:`QDisc`
+        """
+        retval = str(self)
+        if self.is_root():
+            retval += ' root'
+        elif self.is_ingress():
+            retval += ' ingress'
+        else:
+            retval += f' parent {self.get_parent_handle()}'
+        return retval
+
     def dump(self, outfile: TextIO, level=0,
                 qclass_map: Optional[Mapping[Handle, 'QClass']] =None):
         """Recursively dump this :class:`Qdisc` to ``outfile``.
 
         The ``qclass_map``, if present, is used to determine the
         destination :class:`QClass` objects of traffic filters.
         """
```

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/qdiscs/sfq.py` & `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/sfq.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,18 +65,18 @@
                 file=outfile)
 
 
 class SFQQDisc(QDisc):
     """This class provides access to the Stochastic Fairness Queueing
     queueing discipline of Linux (see **tc-sfq(8)**).
     """
-    def __init__(self, qdisc_handle: Handle, parent_handle: Handle,
+    def __init__(self, qdisc_handle: Handle, parent_handle: Optional[Handle],
                 perturb: Optional[int] =None, quantum: Optional[int] =None):
         """
-        :param class_handle: handle of this :class:`SFQQDisc`
+        :param qdisc_handle: handle of this :class:`SFQQDisc`
         :param parent_handle: handle of parent, ``None`` if this is a
             root queuing discipline
         :param perturb: as documented in **tc-sfq(8)**
         :param quantum: as documented in **tc-sfq(8)**
         """
         super().__init__(qdisc_handle, parent_handle)
         self.__perturb = perturb        # seconds
```

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/__init__.py` & `linuxnet-qos-3.3.4/linuxnet/qos/metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,41 +12,16 @@
 # License for more details.
 #
 # You should have received a copy of the GNU Affero General
 # Public License along with linuxnet-qos. If not, see
 # <https://www.gnu.org/licenses/>.
 
 """
-linuxnet.qos library
-~~~~~~~~~~~~~~~~~~~~
-
-The linuxnet.qos library provides programmatic access to
-the Linux traffic control settings via the **tc(8)** command.
+Metadata information intended to be used by setup.py and the
+Sphinx conf.py
 """
 
+# pylint: disable=invalid-name
 
-#
-# Generic
-#
-from .handle import Handle
-from .config import QDiscConfig
-
-#
-# Queuing disciplines
-#
-from .qdiscs import *
-
-#
-# Filters
-#
-from .filters import *
-
-#
-# Exceptions
-#
-from .exceptions import (
-                        TcError,
-                        TcConfigError,
-                        TcParsingError,
-                        TcExecutionError,
-                        TcBandwidthError,
-                        )
+_version_ = "3.3.4"
+_author_ = "Panagiotis (Panos) Tsirigotis"
+_package_ = "linuxnet.qos"
```

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/config.py` & `linuxnet-qos-3.3.4/linuxnet/qos/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,22 +26,23 @@
 from typing import List, Mapping, Optional, Set
 
 from .deps import get_logger
 from .exceptions import TcConfigError, TcExecutionError, TcError
 
 from .handle import Handle
 from .qdiscs.qdisc import QDisc, QClass, QNode
+from .qdiscs.ingress import IngressQDisc
 from .util import run_command, run_subprocess
 
 from .parsers import TrafficFilterParser, QClassParser, QDiscParser
 
 _logger = get_logger("linuxnet.qos.config")
 
 
-class QDiscConfig:
+class QDiscConfig:      # pylint: disable=too-many-public-methods
     """Objects of this class track and manage the queuing discipline
     configuration of a particular interface. The object internal state can
     reflect the configuration inside the kernel by reading the kernel
     configuration using the **tc(8)** command. This can optionally be
     performed upon object initialization.
 
     :class:`QDiscConfig` also provides the methods for adding/removing
@@ -95,15 +96,15 @@
                                 allow_parsing_errors=False):
         """
         :param interface: network interface name
         :param runner: optional callable used to invoke **tc(8)**
         :param read_interface_config: if ``True``, read and parse
             the existing queuing discipline configuration of the interface
         :param allow_parsing_errors: if ``True``, count the parsing
-            errors instread of raising an exception when processing
+            errors instead of raising an exception when processing
             the existing configuration
 
         Raises a :class:`TcParsingError` if unable to parse the
         existing configuration.
 
         Raises a :class:`TcConfigError` if a logical error is encountered
         when processing the existing configuration.
@@ -114,25 +115,33 @@
         # disciplines/classes of an interface. The goal is to keep
         # them in-sync with the in-kernel state.
         # Key: qdisc/qclass handle
         # Value: qdisc/qclass
         self.__qdisc_map = {}
         self.__qclass_map = {}
         self.__root_qdisc = None
+        self.__ingress_qdisc = None
         self.__allow_parsing_errors = allow_parsing_errors
         self.__parsing_errors = 0
         if read_interface_config:
             self.read_interface_config(allow_parsing_errors)
 
     def get_root_qdisc(self) -> Optional[QDisc]:
         """Returns the root queuing discipline, or ``None`` if the root
         queuing discipline has not been discovered yet.
         """
         return self.__root_qdisc
 
+    def get_ingress_qdisc(self) -> Optional[QDisc]:
+        """Returns the ingress queuing discipline, or ``None`` if there
+        is no ingress queuing discipline (or if the interface configuration
+        has not been read).
+        """
+        return self.__ingress_qdisc
+
     def get_interface(self) -> str:
         """Returns the interface associated with this configuration
         """
         return self.__interface
 
     def _get_existing_node(self, handle: Handle) -> QNode:
         """Returns the node with the specified handle. Thia may be
@@ -270,14 +279,35 @@
         qdisc._uninstantiate_qdisc(config=self)
         # Experimentation shows that the above call will fail.
         # It appears that it is not be possible to delete an existing
         # qdisc. What is possible is to delete the parent class of the
         # qdisc which will result in the deletion of the qdisc
         self.__prune_qdisc(qdisc)
 
+    def create_ingress_qdisc(self) -> QDisc:
+        """Create the ingress queuing discipline.
+
+        :rtype: the ingress queuing discipline
+        """
+        if self.__ingress_qdisc is not None:
+            raise TcError('ingress qdisc exists')
+        qdisc = IngressQDisc()
+        qdisc._instantiate_qdisc(config=self)
+        self.__qdisc_map[qdisc.get_handle()] = qdisc
+        self.__ingress_qdisc = qdisc
+        return qdisc
+
+    def delete_ingress_qdisc(self) -> None:
+        """Delete the ingress queuing discipline.
+        """
+        if self.__ingress_qdisc is None:
+            return
+        self.__ingress_qdisc._uninstantiate_qdisc(config=self)
+        self.__ingress_qdisc = None
+
     def create_qclass(self, qclass: QClass) -> None:
         """Create the queuing class ``qclass`` inside the kernel.
         """
         parent = self._get_existing_node(qclass.get_parent_handle())
         if isinstance(parent, QClass):
             # Experimentation has shown that adding a qclass as a child
             # of a qclass that has a qdisc results in the deletion of
@@ -348,16 +378,21 @@
         # NB: pretty output should be avoided as tc may not show
         #     all selectors (observed with the tc command in iproute2-ss091226)
         # Also, we avoid using pretty output to make filter parsing easier
         cmd = ['tc', 'filter', 'ls', 'dev', self.__interface,
                         'parent', str(qnode.get_handle())]
         proc = self.__runner(cmd, check=True, universal_newlines=True,
                                 stdout=subprocess.PIPE, execute_always=True)
-        parser = TrafficFilterParser()
-        parser.parse_output(proc.stdout.split('\n'))
+        parser = TrafficFilterParser(self.__allow_parsing_errors)
+        if proc.stdout:
+            output_lines = proc.stdout.split('\n')
+        else:
+            output_lines = []
+        parser.parse_output(output_lines, qnode)
+        self.__parsing_errors += parser.get_error_count()
         return parser.get_filter_list()
 
     def __reset_config(self):
         """Set attributes to their initial values
         """
         self.__root_qdisc = None
         self.__qdisc_map.clear()
@@ -444,14 +479,21 @@
             remap_needed = False
             while handle in qdisc_map:
                 handle = self.__remap_handle(handle)
                 remap_needed = True
             if remap_needed:
                 qdisc._replace_handle(handle)
             qdisc_map[qdisc.get_handle()] = qdisc
+            if qdisc.is_ingress():
+                if self.__ingress_qdisc is None:
+                    self.__ingress_qdisc = qdisc
+                else:
+                    _logger.warning(
+                        "found another ingress qdisc; original=%s, new=%s",
+                                self.__ingress_qdisc, qdisc)
         return qdisc_map
 
     def __read_qclass_config(self) -> Mapping[Handle, QClass]:
         """Get the class info via tc(8) and populate __qclass_map
         """
         cmd = ['tc', '-s', 'class', 'ls', 'dev', self.__interface]
         proc = self.__runner(cmd, check=True, universal_newlines=True,
@@ -513,15 +555,15 @@
                     raise TcError(f'Unable to find class {parent_handle}')
                 # pylint: disable=protected-access
                 parent_class._add_child_class(qclass)
                 # pylint: enable=protected-access
         # Find the parents of all qdisc's
         for qdisc in self.__qdisc_map.values():
             parent_handle = qdisc.get_parent_handle()
-            if qdisc.is_root():
+            if qdisc.is_root() or qdisc.is_ingress():
                 continue
             parent_class = self.__qclass_map.get(parent_handle)
             if parent_class is None:
                 _logger.error(
                     "%s: missing class parent of qdisc '%s': "
                     "class-parent-handle='%s'",
                         self.__create_qdisc_tree.__qualname__,
```

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/deps.py` & `linuxnet-qos-3.3.4/linuxnet/qos/deps.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/exceptions.py` & `linuxnet-qos-3.3.4/linuxnet/qos/exceptions.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 
 """Exceptions raised by the QoS classes
 """
 
 import errno
 import os
 
+from typing import Optional
+
 class TcError(Exception):
     """Traffic control error; this is the base exception class
     for all QoS-related exceptions.
     """
 
 
 class TcConfigError(TcError):
@@ -37,22 +39,27 @@
     """Error while parsing the output of the **tc(8)** command.
     """
 
     def __init__(self, *args, **kwargs):
         self.__line = kwargs.pop('line', None)
         super().__init__(*args, **kwargs)
 
-    def set_line(self, line):
+    def set_line(self, line: str) -> None:
         """Identify the line where the parsing error happened.
         Once set, this cannot be changed.
         Note that it may be set via the constructor.
         """
         if self.__line is None:
             self.__line = line
 
+    def get_line(self) -> Optional[str]:
+        """Returns the line where the parsing error was encountered.
+        """
+        return self.__line
+
     def __str__(self):
         if self.__line:
             return super().__str__() + ": " + self.__line
         return super().__str__()
 
 
 class TcExecutionError(TcError):
```

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/extension.py` & `linuxnet-qos-3.3.4/linuxnet/qos/extension.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/handle.py` & `linuxnet-qos-3.3.4/linuxnet/qos/handle.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/metadata.py` & `linuxnet-qos-3.3.4/docs/actions/mirred.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-# Copyright (c) 2022, 2023, Panagiotis Tsirigotis
+..
+    Copyright (c) 2023, Panagiotis Tsirigotis
+    
+    This file is part of linuxnet-qos.
+    
+    linuxnet-qos is free software: you can redistribute it and/or
+    modify it under the terms of version 3 of the GNU Affero General Public
+    License as published by the Free Software Foundation.
+    
+    linuxnet-qos is distributed in the hope that it will be useful, but
+    WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
+    or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public
+    License for more details.
+    
+    You should have received a copy of the GNU Affero General
+    Public License along with linuxnet-qos. If not, see
+    <https://www.gnu.org/licenses/>.
 
-# This file is part of linuxnet-qos.
-#
-# linuxnet-qos is free software: you can redistribute it and/or
-# modify it under the terms of version 3 of the GNU Affero General Public
-# License as published by the Free Software Foundation.
-#
-# linuxnet-qos is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY
-# or FITNESS FOR A PARTICULAR PURPOSE. See the GNU Affero General Public
-# License for more details.
-#
-# You should have received a copy of the GNU Affero General
-# Public License along with linuxnet-qos. If not, see
-# <https://www.gnu.org/licenses/>.
+.. currentmodule:: linuxnet.qos
 
-"""
-Metadata information intended to be used by setup.py and the
-Sphinx conf.py
-"""
+MirredAction
+------------
 
-# pylint: disable=invalid-name
+The :class:`MirredAction` supports packet mirroring and packet rediection.
 
-_version_ = "3.2.1"
-_author_ = "Panagiotis (Panos) Tsirigotis"
-_package_ = "linuxnet.qos"
+
+.. autoclass:: MirredAction
+    :inherited-members:
+    :member-order: bysource
```

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/parsers.py` & `linuxnet-qos-3.3.4/linuxnet/qos/parsers.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,56 +16,104 @@
 # <https://www.gnu.org/licenses/>.
 
 """
 This module contains parsers to create Python objects from the output
 of the **tc(8)** command.
 """
 
-from typing import Any, Iterable, Iterator, List, Optional
+from collections import deque
+from typing import Any, Callable, Iterator, List, Optional
 
 from .deps import get_logger
 from .exceptions import TcError, TcParsingError
 from .handle import Handle
 
 
 _logger = get_logger("linuxnet.qos.parsers")
 
 
-class _PeekingIterator:
-    """An iterator that supports peeking
+class LookaheadIterator:
+    """A LookaheadIterator is an iterator that provides the ability to
+    put back previously returned tokens.
+
+    Conceptual view of the LookaheadIterator::
+
+                               deque
+       +---------------+  +---+---+---+---+---+
+       | back-iterator |  | T | T | T |...| T |
+       +---------------+  +---+---+---+---+---+
+                                ^
+                                |
+                              Cursor
+
+    * Tokens to the right of the cursor have been consumed.
+    * Tokens up to, but not including, the cursor are previously consumed
+      tokens that have been put back.
+    * New tokens are obtained from the back-iterator.
+    * The value of the cursor indicates the number of put-back tokens.
+    * The maximum size of the deque is equal to the lookahead.
     """
-    def __init__(self, iterable) -> Iterable[Any]:
+    def __init__(self, iterable, lookahead: int):
         """
-        :param iterable: an iterable object that does not contain ``None``
+        :param iterable: an iterable object from which we create
+            the back-iterator
+        :param lookahead: number of tokens of look ahead
         """
         self.__iter = iter(iterable)
-        self.__peeked = None
+        if lookahead <= 0:
+            raise ValueError(f'bad lookahead value {lookahead}')
+        self.__tokens = deque(maxlen=lookahead)
+        self.__cursor = 0
 
     def __iter__(self):
         return self
 
-    def __next__(self) -> Any:
-        if self.__peeked is not None:
-            token = self.__peeked
-            self.__peeked = None
-        else:
+    def __next__(self):
+        if self.__cursor == 0:
             token = next(self.__iter)
+            self.__tokens.appendleft(token)
+        else:
+            self.__cursor -= 1
+            token = self.__tokens[self.__cursor]
         return token
 
     def peek(self) -> Optional[Any]:
-        """Returns the next token or ``None`` if there are no more tokens.
+        """Returns the next token, but does not consume it
         """
-        if self.__peeked is not None:
-            return self.__peeked
         try:
-            self.__peeked = next(self.__iter)
-            return self.__peeked
+            token = self.__next__()
+            self.put_back(token)
+            return token
         except StopIteration:
             return None
 
+    def put_back(self, token: str) -> None:
+        """Put back the specified token. This must be a token previously
+        returned by the iterator (identity is checked, not equality)
+        """
+        if self.__cursor == len(self.__tokens):
+            # Either there are no consumed tokens, or this is an attempt to
+            # put back one more tokens than those already consumed.
+            raise ValueError('not a consumed token')
+        if token is not self.__tokens[self.__cursor]:
+            raise ValueError('wrong token')
+        self.__cursor += 1
+
+    def rewind(self, step=1) -> 'LookaheadIterator':
+        """Put back last ``step`` tokens
+
+        A :exc:`ValueError` will be raised if there are not enough
+        tokens to put back.
+        """
+        avail = len(self.__tokens) - self.__cursor
+        if step > avail:
+            raise ValueError(f'unable to rewind {step} token(s)')
+        self.__cursor += step
+        return self
+
 
 class LineGroupIterator:
     """The LineGroupIterator is used to parse the output of
     ``tc filter ls``. It returns lines one-by-one and is capable of
     single-level backtracking. This allows the filter-specific
     parsing code to return a line back to the iterator if it
     does not belong to it.
@@ -98,15 +146,16 @@
 
     def get_field_iter(self) -> Iterator[str]:
         """Returns an iterator over the fields of the current line
         """
         if self.__current_line is None:
             raise TcError("attempt to access next field before line iteration")
         if self.__field_iter is None:
-            self.__field_iter = _PeekingIterator(self.__current_line.split())
+            self.__field_iter = LookaheadIterator(
+                                        self.__current_line.split(), 1)
         return self.__field_iter
 
     def clear_field_iter(self):
         """This method removes the field iterator so that a call
         to :meth:`get_field_iter` will create a new one to scan
         the line from the beginning.
         """
@@ -156,25 +205,30 @@
         return self.__line
 
 
 class FilterOutput:
     """An instance of this class contains the **tc(8)** output for a
     single filter.
     """
-    def __init__(self, proto: str, prio: int, filter_type: str):
+    def __init__(self, proto: str, prio: int, filter_type: str, owner: 'QNode'):
         """
         :param proto: filter protocol
         :param prio: filter priority
         :param filter_type: filter type
+        :param owner: :class:`QDisc`/:class:`QClass` that owns the filter
         """
         self.__proto = proto
         self.__prio = prio
         self.__filter_type = filter_type
+        self.__owner = owner
+        # The __filter_lines are the lines starting with the word 'filter'
+        # The __nonfilter_lines are the rest.
         self.__filter_lines = []
         self.__nonfilter_lines = []
+        self.__nonfilter_lines_iter = None
 
     def matches(self, proto: str, prio: int, filter_type: str) -> bool:
         """Returns ``True`` if the ``proto``, ``prio``, ``filter_type``
         parameters match with the corresponding attributes of this object.
 
         :meta private:
         """
@@ -192,63 +246,123 @@
         return self.__proto
 
     def get_filter_type(self) -> str:
         """Returns the filter type
         """
         return self.__filter_type
 
+    def get_filter_owner(self) -> 'QNode':
+        """Returns the :class:`QDisc`/:class:`QClass` that owns the filter
+        """
+        return self.__owner
+
     def get_first_line(self) -> str:
         """Returns the first line from the **tc(8)** output for this filter
         """
         return str(self.__filter_lines[0])
 
     def has_nonfilter_lines(self) -> bool:
         """Returns ``True`` if the filter output has any lines not
         starting with the word ``filter``
         """
         return bool(self.__nonfilter_lines)
 
+    def has_actions(self) -> bool:
+        """Returns ``True`` if the filter has any actions.
+
+        We assume that any remaining non-filter lines
+        are action lines.
+
+        :meta private:
+        """
+        return (self.has_nonfilter_lines() and
+                        self.nonfilter_lines_iter().peek() is not None)
+
     def add_filter_line(self, line: str, fields: List[str]) -> None:
         """Add a line that starts with ``filter ``
 
         :meta private:
         """
         self.__filter_lines.append(FilterOutputLine(line, fields))
 
     def add_line(self, line: str) -> None:
         """Add a non-filter prefixed line
 
         :meta private:
         """
-        self.__nonfilter_lines.append(line.strip())
+        self.__nonfilter_lines.append(line)
 
     def filter_lines_iter(self) -> Iterator[FilterOutputLine]:
         """Returns an iterator that returns :class:`FilterOutputLine`
         instances.
         """
         return iter(self.__filter_lines)
 
     def nonfilter_lines_iter(self) -> Iterator[str]:
         """Returns an iterator that returns lines (strings)
         """
-        return iter(self.__nonfilter_lines)
+        if self.__nonfilter_lines_iter is None:
+            self.__nonfilter_lines_iter = LookaheadIterator(
+                                                self.__nonfilter_lines, 1)
+        return self.__nonfilter_lines_iter
+
+    def dump(self, path) -> None:
+        """Append the contents of this object to the file at path.
+        This is used for debugging.
+
+        :meta private:
+        """
+        with open(path, "a", encoding='utf-8') as outf:
+            for line in self.__filter_lines:
+                outf.write(str(line) + '\n')
+            for line in self.__nonfilter_lines:
+                outf.write(line + '\n')
+            outf.write("------------------\n")
+
+
+def field_advance(producer: Callable[[], str], expected_field: str,
+                                has_value=True) -> Optional[str]:
+    """We are expecting the next field to be ``expected_field`` optionally
+    followed by its value.
+    We return that value, or ``None``.
+    """
+    next_field = None
+    try:
+        next_field = producer()
+        if next_field != expected_field:
+            _logger.error("%s: expected '%s', found '%s'",
+                field_advance.__qualname__, expected_field, next_field)
+            raise TcParsingError(f"expecting '{expected_field}'")
+        return producer() if has_value else None
+    except StopIteration as stopit:
+        if next_field is None:
+            raise TcParsingError(f'missing {expected_field}') from stopit
+        raise TcParsingError(f'no value for {expected_field}') from stopit
 
 
 class TrafficFilterParser:
     """Helper class that creates :class:`TrafficFilter` objects from the
     output of the **tc(8)** command.
     """
 
     #
     # Key: the tuple (filter_type, protocol) - both strings
     # Value: a TrafficFilter subclass
     #
     _filter_class_map = {}
 
-    def __init__(self):
+    #
+    # Key: the action name (a string)
+    # Value: a TrafficAction subclass
+    #
+    _action_class_map = {}
+
+    def __init__(self, allow_parsing_errors: bool):
+        self.__allow_parsing_errors = allow_parsing_errors
+        self.__parsing_errors = 0
         self.__filter_list = []
         # __iter is a LineGroupIterator
         self.__iter: LineGroupIterator = None
 
     @classmethod
     def register_filter(cls, *, filter_type: str, protocol: str, klass) -> None:
         """Register the given class (which should be a subclass of
@@ -259,128 +373,202 @@
 
         :param filter_type: a **tc(8)** filter type, e.g. ``u32``
         :param protocol: a **tc(8)** protocol name, e.g. ``ip``
         :param klass: the Python class for this ``(filter_type, protocol)``
         """
         cls._filter_class_map[(filter_type, protocol)] = klass
 
-    def __process_filter(self, filt_output: FilterOutput):
+    @classmethod
+    def register_action(cls, *, action_name: str, klass) -> None:
+        """Register the given class (which should be a subclass of
+        the :class:`TrafficAction` class).
+
+        This method is intended to be used for adding support for new
+        traffic actions.
+
+        :param action_name: **tc(8)** action, e.g. ``police``
+        :param klass: the Python class for this action
+        """
+        cls._action_class_map[action_name] = klass
+
+    @classmethod
+    def parse_action(cls, fields: List[str],
+                        nfl_iter: Iterator[str]) -> 'TrafficAction':
+        """Parse the **tc(8)** output for a traffic action.
+
+        :param fields: fields of the output line identifying the action
+            and its arguments; ``fields[0]`` is the action type
+        :param nfl_iter: iterator returning the lines after the lines
+            that start with 'filter'
+        :rtype: a :class:`TrafficAction` instance
+
+        Raises a :exc:`TcParsingError` if unable to parse the action
+        """
+        action_name = fields[0]
+        klass = cls._action_class_map.get(action_name)
+        if klass is None:
+            raise TcParsingError(f"unknown action {action_name}")
+        return klass.parse(fields[1:], nfl_iter)
+
+    def __parse_actions(self, filt_output: FilterOutput,
+                                traffic_filter: 'TrafficFilter') -> None:
+        """Parse the actions in the FilterOutput
+        """
+        nfl_iter = filt_output.nonfilter_lines_iter()
+        for nonfilter_line in nfl_iter:
+            action = None
+            try:
+                line = nonfilter_line.strip()
+                fields = line.split()
+                if fields[0] == 'action':
+                    if fields[1] != 'order' or len(fields) < 4:
+                        raise TcParsingError(
+                                        "unable to parse filter action line",
+                                        line=nonfilter_line)
+                    action = self.parse_action(fields[3:], nfl_iter)
+                elif fields[0] == 'police':
+                    action = self.parse_action(fields, nfl_iter)
+                else:
+                    raise TcParsingError(
+                            f'unknown field in non-filter line: {fields[0]}',
+                            line=nonfilter_line)
+                if action is not None:
+                    traffic_filter.add_action(action)
+            except TcParsingError as parserr:
+                self.__parsing_errors += 1
+                if not self.__allow_parsing_errors:
+                    raise
+                _logger.warning("action parsing error, '%s'", parserr)
+
+    def __process_filter(self, filt_output: FilterOutput) -> None:
         """Try to create a new :class:`TrafficFilter` from ``filt_output``.
         """
         #
         # Currently we only support 'ip' filters
         #
         line = filt_output.get_first_line()
         protocol = filt_output.get_proto()
         if protocol != 'ip':
-            _logger.warning(
-                "we cannot handle protocol '%s' (will skip); "
-                "line=%s", protocol, line)
-            return
+            _logger.error("found protocol '%s', expected 'ip' (owner=%s)",
+                        protocol, filt_output.get_filter_owner())
+            raise TcParsingError(
+                f"unable to handle protocol '{protocol}'", line=line)
         filter_type = filt_output.get_filter_type()
         klass = self._filter_class_map.get((filter_type, protocol))
         if klass is None:
-            _logger.warning(
-                "cannot handle filter type '%s', protocol '%s' (will skip); "
-                "line=%s",
-                    filter_type, protocol, line)
-            return
-        try:
-            traffic_filter = klass.parse(filt_output)
-        except TcParsingError as tcparserr:
-            _logger.warning("failed to parse U32 filter output: %s", tcparserr)
-            return
+            _logger.error("unable to handle filter type '%s' (owner=%s)",
+                        filter_type, filt_output.get_filter_owner())
+            raise TcParsingError(
+                f"unable to handle filter type '{filter_type}'", line=line)
+        traffic_filter = klass.parse(filt_output)
+        if filt_output.has_actions():
+            self.__parse_actions(filt_output, traffic_filter)
         if traffic_filter.get_dest_handle() is None:
-            _logger.warning("filter %s has no dest handle", traffic_filter)
+            _logger.warning("filter %s has no dest handle (owner=%s)",
+                traffic_filter, filt_output.get_filter_owner())
         traffic_filter._mark_as_instantiated()
         self.__filter_list.append(traffic_filter)
 
     def __advance(self, field_name: str, has_value=True) -> Optional[str]:
-        """We are expecting the next 2 fields to be ``field_name``
-        followed by its value.
+        """We are expecting the next field to be ``field_name``
+        optionally followed by its value.
         We return that value.
         """
-        next_field = None
-        try:
-            next_field = self.__iter.next_field()
-            if next_field != field_name:
-                _logger.error("%s: expected '%s', found '%s'",
-                    self.__advance.__qualname__, field_name, next_field)
-                raise TcParsingError(f"expecting '{field_name}'")
-            return self.__iter.next_field() if has_value else None
-        except StopIteration as stopit:
-            if next_field is None:
-                raise TcParsingError(f'missing {field_name}') from stopit
-            raise TcParsingError(f'no value for {field_name}') from stopit
+        # Note that self.__iter.next_field is a callable
+        return field_advance(self.__iter.next_field, field_name, has_value)
 
-    def parse_output(self, tc_output_lines: List[str]) -> None:
+    def parse_output(self, tc_output_lines: List[str],
+                                        owner: 'QNode') -> None:
         """Parse the **tc(8)** output in ``tc_output_lines`` into a list
         of :class:`TrafficFilter` objects; the list can be accessed via
         the :meth:`get_filter_list` method.
 
         :meta private:
         """
         self.__filter_list = []
         self.__iter = LineGroupIterator(tc_output_lines)
         #
         # Process lines into FilterOutput objects.
         # Each FilterOutput object has the lines of one filter.
         # Once all lines of a filter are seen, invoke the
         # filter's parse method to create the TrafficFilter object.
         #
-        filt_out = None
+        filt_output = None
         for line in self.__iter:
-            line = line.strip()
-            if not line:
-                continue
             if not line.startswith('filter '):
-                if filt_out is None:
+                if filt_output is None:
+                    _logger.error("unexpected filter line: '%s' (owner=%s)",
+                                        line, owner)
                     raise TcParsingError('unexpected filter line', line=line)
-                filt_out.add_line(line)
+                filt_output.add_line(line)
                 continue
             #
             # We expect a filter line to look like this:
             #   filter protocol <val> pref <int> <type>
             #
             try:
                 _ = self.__advance('filter', has_value=False)
                 protocol = self.__advance('protocol')
                 priostr = self.__advance('pref')
                 try:
                     prio = int(priostr)
                 except ValueError as valerr:
-                    _logger.error("%s: bad priority: %s",
-                        self.parse_output.__qualname__, priostr)
-                    raise TcParsingError('bad filter priority') from valerr
+                    _logger.error("bad filter priority: %s (owner=%s)",
+                        priostr, owner)
+                    raise TcParsingError(
+                        f'bad filter priority: {priostr}') from valerr
                 try:
                     filter_type = self.__iter.next_field()
                 except StopIteration as stopit:
+                    _logger.error(
+                        "filter line without filter type: '%s' (owner=%s)",
+                            line, owner)
                     raise TcParsingError("missing filter type") from stopit
-                if filt_out is None:
-                    filt_out = FilterOutput(protocol, prio, filter_type)
-                    filt_out.add_filter_line(line,
+                if filt_output is None:
+                    filt_output = FilterOutput(protocol, prio,
+                                                        filter_type, owner)
+                    filt_output.add_filter_line(line,
                                     fields=list(self.__iter.get_field_iter()))
                     continue
-                if filt_out.matches(protocol, prio, filter_type):
-                    filt_out.add_filter_line(line,
+                if filt_output.matches(protocol, prio, filter_type):
+                    filt_output.add_filter_line(line,
                                     fields=list(self.__iter.get_field_iter()))
                     continue
+                #
+                # Beginning of output for a new filter.
+                # Process the one we have.
+                #
+                self.__process_filter(filt_output)
             except TcParsingError as parserr:
+                self.__parsing_errors += 1
                 parserr.set_line(line)
-                raise
-            #
-            # Beginning of output for a new filter.
-            # Process the one we have.
-            #
-            self.__process_filter(filt_out)
-            filt_out = FilterOutput(protocol, prio, filter_type)
-            filt_out.add_filter_line(line,
+                if not self.__allow_parsing_errors:
+                    raise
+                _logger.warning("allowing filter parsing error: %s (owner=%s)",
+                                        parserr, owner)
+            filt_output = FilterOutput(protocol, prio, filter_type, owner)
+            filt_output.add_filter_line(line,
                             fields=list(self.__iter.get_field_iter()))
-        if filt_out is not None:
-            self.__process_filter(filt_out)
+        if filt_output is not None:
+            try:
+                self.__process_filter(filt_output)
+            except TcParsingError as parserr:
+                self.__parsing_errors += 1
+                parserr.set_line(filt_output.get_first_line())
+                if not self.__allow_parsing_errors:
+                    raise
+                _logger.warning("allowing filter parsing error: %s (owner=%s)",
+                                        parserr, owner)
+
+    def get_error_count(self) -> int:
+        """Returns number of parsing errors encountered
+
+        :meta private:
+        """
+        return self.__parsing_errors
 
     def get_filter_list(self) -> List['TrafficFilter']:
         """Returns a list of :class:`TrafficFilter` objects from the
         parsed output
 
         :meta private:
         """
@@ -587,19 +775,19 @@
                     raise TcParsingError(f"unknown qdisc type {qdisc_type}")
                 qclass = klass.parse(qclass_output)
                 qclass._parse_stats(qclass_output.get_linegroup_iter())
                 self.__qclass_list.append(qclass)
             except TcParsingError as parserr:
                 self.__parsing_errors += 1
                 line = qclass_output.get_class_line()
-                _logger.error("%s: parsing error, line='%s'",
-                    self.parse_output.__qualname__, line)
                 if not self.__allow_parsing_errors:
                     parserr.set_line(line)
                     raise
+                _logger.warning("%s: parsing error, line='%s'",
+                    self.parse_output.__qualname__, line)
 
     def get_qclass_list(self) -> List['QClass']:
         """Returns a list of :class:`QClass` objects from the
         parsed output
 
         :meta private:
         """
@@ -776,19 +964,19 @@
                     raise TcParsingError(f"unknown qdisc {qdisc_type}")
                 qdisc = klass.parse(qdisc_output)
                 qdisc._parse_stats(qdisc_output.get_linegroup_iter())
                 self.__qdisc_list.append(qdisc)
             except TcParsingError as parserr:
                 self.__parsing_errors += 1
                 line = qdisc_output.get_qdisc_line()
-                _logger.error("%s: parsing error, line='%s'",
-                    self.parse_output.__qualname__, line)
                 if not self.__allow_parsing_errors:
                     parserr.set_line(line)
                     raise
+                _logger.warning("%s: parsing error, line='%s'",
+                    self.parse_output.__qualname__, line)
 
     def get_qdisc_list(self) -> List['QDisc']:
         """Returns a list of :class:`QDisc` objects from the
         parsed output
 
         :meta private:
         """
```

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/tcunit.py` & `linuxnet-qos-3.3.4/linuxnet/qos/tcunit.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/linuxnet/qos/util.py` & `linuxnet-qos-3.3.4/linuxnet/qos/util.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/linuxnet_qos.egg-info/PKG-INFO` & `linuxnet-qos-3.3.4/linuxnet_qos.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxnet-qos
-Version: 3.2.1
+Version: 3.3.4
 Summary: programmatic access to the Linux queuing disciplines
 Home-page: https://gitlab.com/panos-tools/linuxnet-qos
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-qos
 Project-URL: Documentation, https://linuxnet-qos.readthedocs.io/en/latest/index.html
```

### Comparing `linuxnet-qos-3.2.1/linuxnet_qos.egg-info/SOURCES.txt` & `linuxnet-qos-3.3.4/linuxnet_qos.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,24 +10,28 @@
 docs/config.rst
 docs/exceptions.rst
 docs/extensibility.rst
 docs/index.rst
 docs/qdisc.rst
 docs/qos_api.rst
 docs/stats.rst
+docs/traffic_actions.rst
 docs/traffic_filters.rst
+docs/actions/mirred.rst
+docs/actions/police.rst
 docs/extend/filter.rst
 docs/extend/parsing.rst
 docs/extend/qdisc.rst
 docs/extend/util.rst
 docs/filters/fwfilter.rst
 docs/filters/u32filter.rst
 docs/qdiscs/fifo.rst
 docs/qdiscs/fq_codel.rst
 docs/qdiscs/htb.rst
+docs/qdiscs/ingress.rst
 docs/qdiscs/multiqueue.rst
 docs/qdiscs/netem.rst
 docs/qdiscs/prio.rst
 docs/qdiscs/sfq.rst
 linuxnet/__init__.py
 linuxnet/qos/__init__.py
 linuxnet/qos/config.py
@@ -35,22 +39,27 @@
 linuxnet/qos/exceptions.py
 linuxnet/qos/extension.py
 linuxnet/qos/handle.py
 linuxnet/qos/metadata.py
 linuxnet/qos/parsers.py
 linuxnet/qos/tcunit.py
 linuxnet/qos/util.py
+linuxnet/qos/actions/__init__.py
+linuxnet/qos/actions/action.py
+linuxnet/qos/actions/mirred.py
+linuxnet/qos/actions/police.py
 linuxnet/qos/filters/__init__.py
 linuxnet/qos/filters/filter.py
 linuxnet/qos/filters/fwfilter.py
 linuxnet/qos/filters/u32filter.py
 linuxnet/qos/qdiscs/__init__.py
 linuxnet/qos/qdiscs/fifo.py
 linuxnet/qos/qdiscs/fq_codel.py
 linuxnet/qos/qdiscs/htb.py
+linuxnet/qos/qdiscs/ingress.py
 linuxnet/qos/qdiscs/multiqueue.py
 linuxnet/qos/qdiscs/netem.py
 linuxnet/qos/qdiscs/prio.py
 linuxnet/qos/qdiscs/qdisc.py
 linuxnet/qos/qdiscs/sfq.py
 linuxnet_qos.egg-info/PKG-INFO
 linuxnet_qos.egg-info/SOURCES.txt
```

### Comparing `linuxnet-qos-3.2.1/.pylintrc` & `linuxnet-qos-3.3.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/LICENSE` & `linuxnet-qos-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/Makefile` & `linuxnet-qos-3.3.4/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/README.md` & `linuxnet-qos-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/setup.py` & `linuxnet-qos-3.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.2.1/PKG-INFO` & `linuxnet-qos-3.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linuxnet-qos
-Version: 3.2.1
+Version: 3.3.4
 Summary: programmatic access to the Linux queuing disciplines
 Home-page: https://gitlab.com/panos-tools/linuxnet-qos
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-qos
 Project-URL: Documentation, https://linuxnet-qos.readthedocs.io/en/latest/index.html
```

