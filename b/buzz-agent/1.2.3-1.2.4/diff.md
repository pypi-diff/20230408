# Comparing `tmp/buzz_agent-1.2.3.tar.gz` & `tmp/buzz_agent-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/buzz_agent-1.2.3.tar", last modified: Mon Jul 16 15:40:17 2018, max compression
+gzip compressed data, was "buzz_agent-1.2.4.tar", last modified: Sat Apr  8 17:26:30 2023, max compression
```

## Comparing `buzz_agent-1.2.3.tar` & `buzz_agent-1.2.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:40:17.000000 buzz_agent-1.2.3/
--rw-r--r--   0 dantezhu   (501) staff       (20)      224 2018-07-16 15:40:17.000000 buzz_agent-1.2.3/PKG-INFO
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:40:17.000000 buzz_agent-1.2.3/buzz_agent/
--rw-r--r--   0 dantezhu   (501) staff       (20)       82 2018-07-16 15:39:49.000000 buzz_agent-1.2.3/buzz_agent/__init__.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:40:17.000000 buzz_agent-1.2.3/buzz_agent/bin/
--rw-r--r--   0 dantezhu   (501) staff       (20)      911 2018-07-16 15:39:40.000000 buzz_agent-1.2.3/buzz_agent/bin/run_buzz_agent.py
--rw-r--r--   0 dantezhu   (501) staff       (20)     7933 2018-05-27 15:57:07.000000 buzz_agent-1.2.3/buzz_agent/buzz_agent.py
--rw-r--r--   0 dantezhu   (501) staff       (20)      681 2018-05-27 15:57:07.000000 buzz_agent-1.2.3/buzz_agent/six.py
-drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2018-07-16 15:40:17.000000 buzz_agent-1.2.3/buzz_agent.egg-info/
--rw-r--r--   0 dantezhu   (501) staff       (20)      224 2018-07-16 15:40:16.000000 buzz_agent-1.2.3/buzz_agent.egg-info/PKG-INFO
--rw-r--r--   0 dantezhu   (501) staff       (20)      309 2018-07-16 15:40:16.000000 buzz_agent-1.2.3/buzz_agent.egg-info/SOURCES.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2018-07-16 15:40:16.000000 buzz_agent-1.2.3/buzz_agent.egg-info/dependency_links.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)        1 2015-01-04 17:13:59.000000 buzz_agent-1.2.3/buzz_agent.egg-info/not-zip-safe
--rw-r--r--   0 dantezhu   (501) staff       (20)       17 2018-07-16 15:40:16.000000 buzz_agent-1.2.3/buzz_agent.egg-info/requires.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       11 2018-07-16 15:40:16.000000 buzz_agent-1.2.3/buzz_agent.egg-info/top_level.txt
--rw-r--r--   0 dantezhu   (501) staff       (20)       38 2018-07-16 15:40:17.000000 buzz_agent-1.2.3/setup.cfg
--rw-r--r--   0 dantezhu   (501) staff       (20)      469 2018-07-16 15:39:49.000000 buzz_agent-1.2.3/setup.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:26:30.055529 buzz_agent-1.2.4/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      270 2023-04-08 17:26:30.055660 buzz_agent-1.2.4/PKG-INFO
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:26:30.050654 buzz_agent-1.2.4/buzz_agent/
+-rw-r--r--   0 dantezhu   (501) staff       (20)       82 2023-04-08 17:26:13.000000 buzz_agent-1.2.4/buzz_agent/__init__.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:26:30.054883 buzz_agent-1.2.4/buzz_agent/bin/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      911 2018-07-16 15:39:40.000000 buzz_agent-1.2.4/buzz_agent/bin/run_buzz_agent.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)     7933 2018-05-27 15:57:07.000000 buzz_agent-1.2.4/buzz_agent/buzz_agent.py
+-rw-r--r--   0 dantezhu   (501) staff       (20)      681 2018-05-27 15:57:07.000000 buzz_agent-1.2.4/buzz_agent/six.py
+drwxr-xr-x   0 dantezhu   (501) staff       (20)        0 2023-04-08 17:26:30.054290 buzz_agent-1.2.4/buzz_agent.egg-info/
+-rw-r--r--   0 dantezhu   (501) staff       (20)      270 2023-04-08 17:26:30.000000 buzz_agent-1.2.4/buzz_agent.egg-info/PKG-INFO
+-rw-r--r--   0 dantezhu   (501) staff       (20)      334 2023-04-08 17:26:30.000000 buzz_agent-1.2.4/buzz_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2023-04-08 17:26:30.000000 buzz_agent-1.2.4/buzz_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)        1 2015-01-04 17:13:59.000000 buzz_agent-1.2.4/buzz_agent.egg-info/not-zip-safe
+-rw-r--r--   0 dantezhu   (501) staff       (20)       17 2023-04-08 17:26:30.000000 buzz_agent-1.2.4/buzz_agent.egg-info/requires.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)       11 2023-04-08 17:26:30.000000 buzz_agent-1.2.4/buzz_agent.egg-info/top_level.txt
+-rw-r--r--   0 dantezhu   (501) staff       (20)      582 2023-04-08 17:26:21.000000 buzz_agent-1.2.4/pyproject.toml
+-rw-r--r--   0 dantezhu   (501) staff       (20)      424 2023-04-08 17:26:30.056323 buzz_agent-1.2.4/setup.cfg
+-rw-r--r--   0 dantezhu   (501) staff       (20)      469 2023-04-08 17:26:06.000000 buzz_agent-1.2.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `buzz_agent-1.2.3/buzz_agent/bin/run_buzz_agent.py` & `buzz_agent-1.2.4/buzz_agent/bin/run_buzz_agent.py`

 * *Files identical despite different names*

### Comparing `buzz_agent-1.2.3/buzz_agent/buzz_agent.py` & `buzz_agent-1.2.4/buzz_agent/buzz_agent.py`

 * *Files identical despite different names*

### Comparing `buzz_agent-1.2.3/buzz_agent/six.py` & `buzz_agent-1.2.4/buzz_agent/six.py`

 * *Files identical despite different names*

