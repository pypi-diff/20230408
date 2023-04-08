# Comparing `tmp/django-htmx-viewsets-0.0.2.tar.gz` & `tmp/django-htmx-viewsets-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-htmx-viewsets-0.0.2.tar", last modified: Sat Apr  8 17:21:04 2023, max compression
+gzip compressed data, was "django-htmx-viewsets-0.0.3.tar", last modified: Sat Apr  8 17:26:25 2023, max compression
```

## Comparing `django-htmx-viewsets-0.0.2.tar` & `django-htmx-viewsets-0.0.3.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:21:04.894951 django-htmx-viewsets-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-08 17:21:04.894951 django-htmx-viewsets-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 17:20:56.000000 django-htmx-viewsets-0.0.2/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 17:21:04.894951 django-htmx-viewsets-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:21:04.890951 django-htmx-viewsets-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:21:04.890951 django-htmx-viewsets-0.0.2/src/django_htmx_viewsets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-08 17:21:04.000000 django-htmx-viewsets-0.0.2/src/django_htmx_viewsets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-08 17:21:04.000000 django-htmx-viewsets-0.0.2/src/django_htmx_viewsets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 17:21:04.000000 django-htmx-viewsets-0.0.2/src/django_htmx_viewsets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-08 17:21:04.000000 django-htmx-viewsets-0.0.2/src/django_htmx_viewsets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 17:21:04.000000 django-htmx-viewsets-0.0.2/src/django_htmx_viewsets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:21:04.894951 django-htmx-viewsets-0.0.2/src/htmx_viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:21:04.894951 django-htmx-viewsets-0.0.2/src/htmx_viewsets/table/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/table/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/table/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/table/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/table/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/table/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/table/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:21:04.890951 django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:21:04.894951 django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/chart.html
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/dispatch.html
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/full.html
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:21:04.894951 django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/modal/
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/partial.html
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/table.html
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-04-08 17:20:45.000000 django-htmx-viewsets-0.0.2/src/htmx_viewsets/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:26:25.659715 django-htmx-viewsets-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-08 17:26:25.659715 django-htmx-viewsets-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 17:26:18.000000 django-htmx-viewsets-0.0.3/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 17:26:25.659715 django-htmx-viewsets-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:26:25.655715 django-htmx-viewsets-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:26:25.655715 django-htmx-viewsets-0.0.3/src/django_htmx_viewsets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-08 17:26:25.000000 django-htmx-viewsets-0.0.3/src/django_htmx_viewsets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-08 17:26:25.000000 django-htmx-viewsets-0.0.3/src/django_htmx_viewsets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 17:26:25.000000 django-htmx-viewsets-0.0.3/src/django_htmx_viewsets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-08 17:26:25.000000 django-htmx-viewsets-0.0.3/src/django_htmx_viewsets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 17:26:25.000000 django-htmx-viewsets-0.0.3/src/django_htmx_viewsets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:26:25.655715 django-htmx-viewsets-0.0.3/src/htmx_viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 17:26:18.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:26:25.655715 django-htmx-viewsets-0.0.3/src/htmx_viewsets/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/table/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/table/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/table/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/table/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/table/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/table/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:26:25.655715 django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:26:25.659715 django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/chart.html
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/dispatch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/full.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:26:25.659715 django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/modal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/partial.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-04-08 17:26:07.000000 django-htmx-viewsets-0.0.3/src/htmx_viewsets/viewsets.py
```

### Comparing `django-htmx-viewsets-0.0.2/LICENSE` & `django-htmx-viewsets-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/PKG-INFO` & `django-htmx-viewsets-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-viewsets
-Version: 0.0.2
+Version: 0.0.3
 Summary: Viewsets for Django using HTMX, Chartjs and DataTables
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: GPL3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-htmx-viewsets-0.0.2/setup.py` & `django-htmx-viewsets-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/django_htmx_viewsets.egg-info/PKG-INFO` & `django-htmx-viewsets-0.0.3/src/django_htmx_viewsets.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-htmx-viewsets
-Version: 0.0.2
+Version: 0.0.3
 Summary: Viewsets for Django using HTMX, Chartjs and DataTables
 Author: Snake-Soft
 Author-email: info@snake-soft.com
 License: GPL3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-htmx-viewsets-0.0.2/src/django_htmx_viewsets.egg-info/SOURCES.txt` & `django-htmx-viewsets-0.0.3/src/django_htmx_viewsets.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 VERSION
 setup.py
 src/django_htmx_viewsets.egg-info/PKG-INFO
 src/django_htmx_viewsets.egg-info/SOURCES.txt
 src/django_htmx_viewsets.egg-info/dependency_links.txt
 src/django_htmx_viewsets.egg-info/requires.txt
 src/django_htmx_viewsets.egg-info/top_level.txt
+src/htmx_viewsets/VERSION
 src/htmx_viewsets/__init__.py
 src/htmx_viewsets/apps.py
 src/htmx_viewsets/chart.py
 src/htmx_viewsets/color.py
 src/htmx_viewsets/fields.py
 src/htmx_viewsets/forms.py
 src/htmx_viewsets/views.py
```

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/chart.py` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/chart.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/color.py` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/color.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/fields.py` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/fields.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/forms.py` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/forms.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/table/action.py` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/table/action.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/table/cell.py` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/table/cell.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/table/column.py` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/table/column.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/table/row.py` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/table/row.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/table/table.py` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/table/table.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/delete.html` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/delete.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/form.html` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/form.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/full.html` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/full.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/list.html` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/list.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/modal.html` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/modal.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/partial.html` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/partial.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/templates/htmx_viewsets/table.html` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/templates/htmx_viewsets/table.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/views.py` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/views.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.2/src/htmx_viewsets/viewsets.py` & `django-htmx-viewsets-0.0.3/src/htmx_viewsets/viewsets.py`

 * *Files identical despite different names*

