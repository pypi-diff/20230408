# Comparing `tmp/RP-DataBase-1.0.1.tar.gz` & `tmp/RP-DataBase-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RP-DataBase-1.0.1.tar", last modified: Wed Jan 25 08:44:24 2023, max compression
+gzip compressed data, was "RP-DataBase-1.1.0.tar", last modified: Sat Apr  8 16:33:57 2023, max compression
```

## Comparing `RP-DataBase-1.0.1.tar` & `RP-DataBase-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-01-25 08:44:24.000000 RP-DataBase-1.0.1/
--rw-rw-rw-   0        0        0     2301 2022-10-16 00:27:24.000000 RP-DataBase-1.0.1/containers.py
--rw-rw-rw-   0        0        0     1085 2023-01-25 07:39:48.000000 RP-DataBase-1.0.1/license
--rw-rw-rw-   0        0        0      253 2023-01-25 08:44:24.000000 RP-DataBase-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-25 08:44:24.000000 RP-DataBase-1.0.1/RPDB/
--rw-rw-rw-   0        0        0     6224 2023-01-25 08:14:10.000000 RP-DataBase-1.0.1/RPDB/database.py
--rw-rw-rw-   0        0        0        0 2023-01-25 08:13:50.000000 RP-DataBase-1.0.1/RPDB/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-25 08:44:24.000000 RP-DataBase-1.0.1/RP_DataBase.egg-info/
--rw-rw-rw-   0        0        0        1 2023-01-25 08:44:24.000000 RP-DataBase-1.0.1/RP_DataBase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      253 2023-01-25 08:44:24.000000 RP-DataBase-1.0.1/RP_DataBase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-01-25 08:44:24.000000 RP-DataBase-1.0.1/RP_DataBase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        5 2023-01-25 08:44:24.000000 RP-DataBase-1.0.1/RP_DataBase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-25 08:44:24.000000 RP-DataBase-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      281 2023-01-25 08:37:42.000000 RP-DataBase-1.0.1/setup.py
+drwxr-xr-x   0 hsn       (1000) hsn       (1000)        0 2023-04-08 16:33:57.770037 RP-DataBase-1.1.0/
+-rw-r--r--   0 hsn       (1000) hsn       (1000)      190 2023-04-08 16:33:57.770037 RP-DataBase-1.1.0/PKG-INFO
+drwxr-xr-x   0 hsn       (1000) hsn       (1000)        0 2023-04-08 16:33:57.770037 RP-DataBase-1.1.0/RPDB/
+-rw-r--r--   0 hsn       (1000) hsn       (1000)        0 2023-04-08 15:24:42.000000 RP-DataBase-1.1.0/RPDB/__init__.py
+-rw-r--r--   0 hsn       (1000) hsn       (1000)     9750 2023-04-08 16:26:05.000000 RP-DataBase-1.1.0/RPDB/database.py
+drwxr-xr-x   0 hsn       (1000) hsn       (1000)        0 2023-04-08 16:33:57.770037 RP-DataBase-1.1.0/RP_DataBase.egg-info/
+-rw-r--r--   0 hsn       (1000) hsn       (1000)      190 2023-04-08 16:33:57.000000 RP-DataBase-1.1.0/RP_DataBase.egg-info/PKG-INFO
+-rw-r--r--   0 hsn       (1000) hsn       (1000)      182 2023-04-08 16:33:57.000000 RP-DataBase-1.1.0/RP_DataBase.egg-info/SOURCES.txt
+-rw-r--r--   0 hsn       (1000) hsn       (1000)        1 2023-04-08 16:33:57.000000 RP-DataBase-1.1.0/RP_DataBase.egg-info/dependency_links.txt
+-rw-r--r--   0 hsn       (1000) hsn       (1000)        5 2023-04-08 16:33:57.000000 RP-DataBase-1.1.0/RP_DataBase.egg-info/top_level.txt
+-rw-r--r--   0 hsn       (1000) hsn       (1000)       38 2023-04-08 16:33:57.770037 RP-DataBase-1.1.0/setup.cfg
+-rw-r--r--   0 hsn       (1000) hsn       (1000)      269 2023-04-08 16:33:31.000000 RP-DataBase-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

