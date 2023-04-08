# Comparing `tmp/django_moncash-2.1.1.tar.gz` & `tmp/django_moncash-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_moncash-2.1.1.tar", last modified: Sat Apr  8 04:02:35 2023, max compression
+gzip compressed data, was "django_moncash-2.2.1.tar", last modified: Sat Apr  8 13:41:00 2023, max compression
```

## Comparing `django_moncash-2.1.1.tar` & `django_moncash-2.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 04:02:35.710438 django_moncash-2.1.1/
--rw-r--r--   0 macbook    (501) staff       (20)    35149 2023-04-06 01:43:10.000000 django_moncash-2.1.1/LICENSE
--rw-r--r--   0 macbook    (501) staff       (20)    49220 2023-04-08 04:02:35.710716 django_moncash-2.1.1/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     8087 2023-04-07 22:04:44.000000 django_moncash-2.1.1/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 04:02:35.703800 django_moncash-2.1.1/django_moncash/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.1.1/django_moncash/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      298 2023-04-07 14:53:44.000000 django_moncash-2.1.1/django_moncash/_utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      722 2023-04-07 15:50:36.000000 django_moncash-2.1.1/django_moncash/admin.py
--rw-r--r--   0 macbook    (501) staff       (20)      159 2023-04-06 01:44:10.000000 django_moncash-2.1.1/django_moncash/apps.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 04:02:35.710255 django_moncash-2.1.1/django_moncash/migrations/
--rw-r--r--   0 macbook    (501) staff       (20)     1466 2023-04-07 15:39:31.000000 django_moncash-2.1.1/django_moncash/migrations/0001_initial.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.1.1/django_moncash/migrations/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1088 2023-04-07 15:37:08.000000 django_moncash-2.1.1/django_moncash/models.py
--rw-r--r--   0 macbook    (501) staff       (20)       60 2023-04-06 01:44:10.000000 django_moncash-2.1.1/django_moncash/tests.py
--rw-r--r--   0 macbook    (501) staff       (20)      148 2023-04-06 18:01:13.000000 django_moncash-2.1.1/django_moncash/urls.py
--rw-r--r--   0 macbook    (501) staff       (20)     2526 2023-04-08 04:00:18.000000 django_moncash-2.1.1/django_moncash/utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      564 2023-04-08 03:20:24.000000 django_moncash-2.1.1/django_moncash/views.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 04:02:35.709657 django_moncash-2.1.1/django_moncash.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)    49220 2023-04-08 04:02:35.000000 django_moncash-2.1.1/django_moncash.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      580 2023-04-08 04:02:35.000000 django_moncash-2.1.1/django_moncash.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-08 04:02:35.000000 django_moncash-2.1.1/django_moncash.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)      131 2023-04-08 04:02:35.000000 django_moncash-2.1.1/django_moncash.egg-info/entry_points.txt
--rw-r--r--   0 macbook    (501) staff       (20)       51 2023-04-08 04:02:35.000000 django_moncash-2.1.1/django_moncash.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)       15 2023-04-08 04:02:35.000000 django_moncash-2.1.1/django_moncash.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)      928 2023-04-08 04:01:45.000000 django_moncash-2.1.1/pyproject.toml
--rw-r--r--   0 macbook    (501) staff       (20)      904 2023-04-08 04:02:35.711218 django_moncash-2.1.1/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)       96 2023-04-08 01:26:12.000000 django_moncash-2.1.1/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 13:41:00.684095 django_moncash-2.2.1/
+-rw-r--r--   0 macbook    (501) staff       (20)    35149 2023-04-06 01:43:10.000000 django_moncash-2.2.1/LICENSE
+-rw-r--r--   0 macbook    (501) staff       (20)    49220 2023-04-08 13:41:00.684318 django_moncash-2.2.1/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     8087 2023-04-07 22:04:44.000000 django_moncash-2.2.1/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 13:41:00.681757 django_moncash-2.2.1/django_moncash/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.2.1/django_moncash/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      298 2023-04-07 14:53:44.000000 django_moncash-2.2.1/django_moncash/_utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      722 2023-04-07 15:50:36.000000 django_moncash-2.2.1/django_moncash/admin.py
+-rw-r--r--   0 macbook    (501) staff       (20)      159 2023-04-06 01:44:10.000000 django_moncash-2.2.1/django_moncash/apps.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 13:41:00.683926 django_moncash-2.2.1/django_moncash/migrations/
+-rw-r--r--   0 macbook    (501) staff       (20)     1466 2023-04-07 15:39:31.000000 django_moncash-2.2.1/django_moncash/migrations/0001_initial.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.2.1/django_moncash/migrations/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1088 2023-04-07 15:37:08.000000 django_moncash-2.2.1/django_moncash/models.py
+-rw-r--r--   0 macbook    (501) staff       (20)       60 2023-04-06 01:44:10.000000 django_moncash-2.2.1/django_moncash/tests.py
+-rw-r--r--   0 macbook    (501) staff       (20)      148 2023-04-06 18:01:13.000000 django_moncash-2.2.1/django_moncash/urls.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2526 2023-04-08 04:00:18.000000 django_moncash-2.2.1/django_moncash/utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      564 2023-04-08 03:20:24.000000 django_moncash-2.2.1/django_moncash/views.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 13:41:00.683307 django_moncash-2.2.1/django_moncash.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)    49220 2023-04-08 13:41:00.000000 django_moncash-2.2.1/django_moncash.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      580 2023-04-08 13:41:00.000000 django_moncash-2.2.1/django_moncash.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-08 13:41:00.000000 django_moncash-2.2.1/django_moncash.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      146 2023-04-08 13:41:00.000000 django_moncash-2.2.1/django_moncash.egg-info/entry_points.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       51 2023-04-08 13:41:00.000000 django_moncash-2.2.1/django_moncash.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       15 2023-04-08 13:41:00.000000 django_moncash-2.2.1/django_moncash.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      943 2023-04-08 13:40:35.000000 django_moncash-2.2.1/pyproject.toml
+-rw-r--r--   0 macbook    (501) staff       (20)      904 2023-04-08 13:41:00.684764 django_moncash-2.2.1/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)       96 2023-04-08 01:26:12.000000 django_moncash-2.2.1/setup.py
```

### Comparing `django_moncash-2.1.1/LICENSE` & `django_moncash-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_moncash-2.1.1/PKG-INFO` & `django_moncash-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_moncash
-Version: 2.1.1
+Version: 2.2.1
 Summary: Installable django moncash
 Home-page: https://github.com/undisplay/django_moncash
 Author-email: Freedy Meritus <meritusfreedy@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `django_moncash-2.1.1/README.md` & `django_moncash-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_moncash-2.1.1/django_moncash/admin.py` & `django_moncash-2.2.1/django_moncash/admin.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.1.1/django_moncash/migrations/0001_initial.py` & `django_moncash-2.2.1/django_moncash/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.1.1/django_moncash/models.py` & `django_moncash-2.2.1/django_moncash/models.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.1.1/django_moncash/utils.py` & `django_moncash-2.2.1/django_moncash/utils.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.1.1/django_moncash/views.py` & `django_moncash-2.2.1/django_moncash/views.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.1.1/django_moncash.egg-info/PKG-INFO` & `django_moncash-2.2.1/django_moncash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-moncash
-Version: 2.1.1
+Version: 2.2.1
 Summary: Installable django moncash
 Home-page: https://github.com/undisplay/django_moncash
 Author-email: Freedy Meritus <meritusfreedy@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `django_moncash-2.1.1/django_moncash.egg-info/SOURCES.txt` & `django_moncash-2.2.1/django_moncash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_moncash-2.1.1/pyproject.toml` & `django_moncash-2.2.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django_moncash"
-version = "2.1.1"
+version = "2.2.1"
 description = "Installable django moncash"
 readme = "README.md"
 authors = [{ name = "Freedy Meritus", email = "meritusfreedy@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Programming Language :: Python",
@@ -26,10 +26,10 @@
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/undisplay/django_moncash"
 
 [project.scripts]
-django_moncash_migrate = "migrate"
-django_moncash_makemigrations = "makemigrations"
-django_moncash_test = "load_tests"
+django_moncash_migrate = "migrate:main"
+django_moncash_makemigrations = "makemigrations:main"
+django_moncash_test = "load_tests:main"
```

### Comparing `django_moncash-2.1.1/setup.cfg` & `django_moncash-2.2.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_moncash
-version = 2.1.1
+version = 2.2.1
 description = Installable django moncash
 long_description = file:README.md
 url = https://github.com/undisplay/django_moncash
 license = GNU
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
```

