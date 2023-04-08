# Comparing `tmp/django_moncash-2.3.3.tar.gz` & `tmp/django_moncash-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_moncash-2.3.3.tar", last modified: Sat Apr  8 20:45:56 2023, max compression
+gzip compressed data, was "django_moncash-2.4.3.tar", last modified: Sat Apr  8 20:56:48 2023, max compression
```

## Comparing `django_moncash-2.3.3.tar` & `django_moncash-2.4.3.tar`

### file list

```diff
@@ -1,32 +1,26 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 20:45:56.397746 django_moncash-2.3.3/
--rw-r--r--   0 macbook    (501) staff       (20)    35149 2023-04-06 01:43:10.000000 django_moncash-2.3.3/LICENSE
--rw-r--r--   0 macbook    (501) staff       (20)    49220 2023-04-08 20:45:56.397966 django_moncash-2.3.3/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     8087 2023-04-07 22:04:44.000000 django_moncash-2.3.3/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 20:45:56.395455 django_moncash-2.3.3/django_moncash/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.3.3/django_moncash/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)      298 2023-04-07 14:53:44.000000 django_moncash-2.3.3/django_moncash/_utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      722 2023-04-07 15:50:36.000000 django_moncash-2.3.3/django_moncash/admin.py
--rw-r--r--   0 macbook    (501) staff       (20)      159 2023-04-06 01:44:10.000000 django_moncash-2.3.3/django_moncash/apps.py
--rw-r--r--   0 macbook    (501) staff       (20)      919 2023-04-07 16:06:02.000000 django_moncash-2.3.3/django_moncash/boot_django.py
--rwxr-xr-x   0 macbook    (501) staff       (20)      258 2023-04-08 20:22:55.000000 django_moncash-2.3.3/django_moncash/djangoshell.py
--rw-r--r--   0 macbook    (501) staff       (20)      667 2023-04-08 13:37:54.000000 django_moncash-2.3.3/django_moncash/load_tests.py
--rw-r--r--   0 macbook    (501) staff       (20)      259 2023-04-08 20:23:34.000000 django_moncash-2.3.3/django_moncash/makemigrations.py
--rw-r--r--   0 macbook    (501) staff       (20)      250 2023-04-08 20:23:12.000000 django_moncash-2.3.3/django_moncash/migrate.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 20:45:56.397588 django_moncash-2.3.3/django_moncash/migrations/
--rw-r--r--   0 macbook    (501) staff       (20)     1466 2023-04-07 15:39:31.000000 django_moncash-2.3.3/django_moncash/migrations/0001_initial.py
--rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.3.3/django_moncash/migrations/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     1088 2023-04-07 15:37:08.000000 django_moncash-2.3.3/django_moncash/models.py
--rw-r--r--   0 macbook    (501) staff       (20)       60 2023-04-06 01:44:10.000000 django_moncash-2.3.3/django_moncash/tests.py
--rw-r--r--   0 macbook    (501) staff       (20)      148 2023-04-06 18:01:13.000000 django_moncash-2.3.3/django_moncash/urls.py
--rw-r--r--   0 macbook    (501) staff       (20)     2526 2023-04-08 04:00:18.000000 django_moncash-2.3.3/django_moncash/utils.py
--rw-r--r--   0 macbook    (501) staff       (20)      564 2023-04-08 03:20:24.000000 django_moncash-2.3.3/django_moncash/views.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 20:45:56.397170 django_moncash-2.3.3/django_moncash.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)    49220 2023-04-08 20:45:56.000000 django_moncash-2.3.3/django_moncash.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      728 2023-04-08 20:45:56.000000 django_moncash-2.3.3/django_moncash.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-08 20:45:56.000000 django_moncash-2.3.3/django_moncash.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)      246 2023-04-08 20:45:56.000000 django_moncash-2.3.3/django_moncash.egg-info/entry_points.txt
--rw-r--r--   0 macbook    (501) staff       (20)       51 2023-04-08 20:45:56.000000 django_moncash-2.3.3/django_moncash.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)       15 2023-04-08 20:45:56.000000 django_moncash-2.3.3/django_moncash.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)     1045 2023-04-08 20:45:30.000000 django_moncash-2.3.3/pyproject.toml
--rw-r--r--   0 macbook    (501) staff       (20)      904 2023-04-08 20:45:56.398393 django_moncash-2.3.3/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)       96 2023-04-08 01:26:12.000000 django_moncash-2.3.3/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 20:56:48.772045 django_moncash-2.4.3/
+-rw-r--r--   0 macbook    (501) staff       (20)    35149 2023-04-06 01:43:10.000000 django_moncash-2.4.3/LICENSE
+-rw-r--r--   0 macbook    (501) staff       (20)    49220 2023-04-08 20:56:48.772284 django_moncash-2.4.3/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     8087 2023-04-07 22:04:44.000000 django_moncash-2.4.3/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 20:56:48.769882 django_moncash-2.4.3/django_moncash/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.4.3/django_moncash/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)      298 2023-04-07 14:53:44.000000 django_moncash-2.4.3/django_moncash/_utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      722 2023-04-07 15:50:36.000000 django_moncash-2.4.3/django_moncash/admin.py
+-rw-r--r--   0 macbook    (501) staff       (20)      159 2023-04-06 01:44:10.000000 django_moncash-2.4.3/django_moncash/apps.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 20:56:48.771894 django_moncash-2.4.3/django_moncash/migrations/
+-rw-r--r--   0 macbook    (501) staff       (20)     1466 2023-04-07 15:39:31.000000 django_moncash-2.4.3/django_moncash/migrations/0001_initial.py
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2023-04-06 01:44:10.000000 django_moncash-2.4.3/django_moncash/migrations/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1088 2023-04-07 15:37:08.000000 django_moncash-2.4.3/django_moncash/models.py
+-rw-r--r--   0 macbook    (501) staff       (20)       60 2023-04-06 01:44:10.000000 django_moncash-2.4.3/django_moncash/tests.py
+-rw-r--r--   0 macbook    (501) staff       (20)      148 2023-04-06 18:01:13.000000 django_moncash-2.4.3/django_moncash/urls.py
+-rw-r--r--   0 macbook    (501) staff       (20)     2526 2023-04-08 04:00:18.000000 django_moncash-2.4.3/django_moncash/utils.py
+-rw-r--r--   0 macbook    (501) staff       (20)      564 2023-04-08 03:20:24.000000 django_moncash-2.4.3/django_moncash/views.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-08 20:56:48.771324 django_moncash-2.4.3/django_moncash.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)    49220 2023-04-08 20:56:48.000000 django_moncash-2.4.3/django_moncash.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      539 2023-04-08 20:56:48.000000 django_moncash-2.4.3/django_moncash.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-08 20:56:48.000000 django_moncash-2.4.3/django_moncash.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       51 2023-04-08 20:56:48.000000 django_moncash-2.4.3/django_moncash.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       15 2023-04-08 20:56:48.000000 django_moncash-2.4.3/django_moncash.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      809 2023-04-08 20:56:39.000000 django_moncash-2.4.3/pyproject.toml
+-rw-r--r--   0 macbook    (501) staff       (20)      904 2023-04-08 20:56:48.772730 django_moncash-2.4.3/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)       96 2023-04-08 01:26:12.000000 django_moncash-2.4.3/setup.py
```

### Comparing `django_moncash-2.3.3/LICENSE` & `django_moncash-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_moncash-2.3.3/PKG-INFO` & `django_moncash-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_moncash
-Version: 2.3.3
+Version: 2.4.3
 Summary: Installable django moncash
 Home-page: https://github.com/undisplay/django_moncash
 Author-email: Freedy Meritus <meritusfreedy@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `django_moncash-2.3.3/README.md` & `django_moncash-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `django_moncash-2.3.3/django_moncash/admin.py` & `django_moncash-2.4.3/django_moncash/admin.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.3.3/django_moncash/migrations/0001_initial.py` & `django_moncash-2.4.3/django_moncash/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.3.3/django_moncash/models.py` & `django_moncash-2.4.3/django_moncash/models.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.3.3/django_moncash/utils.py` & `django_moncash-2.4.3/django_moncash/utils.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.3.3/django_moncash/views.py` & `django_moncash-2.4.3/django_moncash/views.py`

 * *Files identical despite different names*

### Comparing `django_moncash-2.3.3/django_moncash.egg-info/PKG-INFO` & `django_moncash-2.4.3/django_moncash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-moncash
-Version: 2.3.3
+Version: 2.4.3
 Summary: Installable django moncash
 Home-page: https://github.com/undisplay/django_moncash
 Author-email: Freedy Meritus <meritusfreedy@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `django_moncash-2.3.3/django_moncash.egg-info/SOURCES.txt` & `django_moncash-2.4.3/django_moncash.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -3,25 +3,19 @@
 pyproject.toml
 setup.cfg
 setup.py
 django_moncash/__init__.py
 django_moncash/_utils.py
 django_moncash/admin.py
 django_moncash/apps.py
-django_moncash/boot_django.py
-django_moncash/djangoshell.py
-django_moncash/load_tests.py
-django_moncash/makemigrations.py
-django_moncash/migrate.py
 django_moncash/models.py
 django_moncash/tests.py
 django_moncash/urls.py
 django_moncash/utils.py
 django_moncash/views.py
 django_moncash.egg-info/PKG-INFO
 django_moncash.egg-info/SOURCES.txt
 django_moncash.egg-info/dependency_links.txt
-django_moncash.egg-info/entry_points.txt
 django_moncash.egg-info/requires.txt
 django_moncash.egg-info/top_level.txt
 django_moncash/migrations/0001_initial.py
 django_moncash/migrations/__init__.py
```

### Comparing `django_moncash-2.3.3/setup.cfg` & `django_moncash-2.4.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_moncash
-version = 2.3.3
+version = 2.4.3
 description = Installable django moncash
 long_description = file:README.md
 url = https://github.com/undisplay/django_moncash
 license = GNU
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Web Environment
```

