# Comparing `tmp/django-htmx-viewsets-0.0.4.tar.gz` & `tmp/django-htmx-viewsets-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-htmx-viewsets-0.0.4.tar", last modified: Sat Apr  8 21:30:08 2023, max compression
+gzip compressed data, was "django-htmx-viewsets-0.0.5.tar", last modified: Sat Apr  8 21:38:57 2023, max compression
```

## Comparing `django-htmx-viewsets-0.0.4.tar` & `django-htmx-viewsets-0.0.5.tar`

### file list

```diff
@@ -1,50 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:30:08.327897 django-htmx-viewsets-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-08 21:30:08.327897 django-htmx-viewsets-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 21:30:01.000000 django-htmx-viewsets-0.0.4/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 21:30:08.327897 django-htmx-viewsets-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:30:08.319897 django-htmx-viewsets-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:30:08.319897 django-htmx-viewsets-0.0.4/src/django_htmx_viewsets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-08 21:30:08.000000 django-htmx-viewsets-0.0.4/src/django_htmx_viewsets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-08 21:30:08.000000 django-htmx-viewsets-0.0.4/src/django_htmx_viewsets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:30:08.000000 django-htmx-viewsets-0.0.4/src/django_htmx_viewsets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-08 21:30:08.000000 django-htmx-viewsets-0.0.4/src/django_htmx_viewsets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 21:30:08.000000 django-htmx-viewsets-0.0.4/src/django_htmx_viewsets.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:30:08.323897 django-htmx-viewsets-0.0.4/src/htmx_viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 21:30:01.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:30:08.323897 django-htmx-viewsets-0.0.4/src/htmx_viewsets/table/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/table/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/table/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/table/column.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/table/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/table/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/table/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:30:08.319897 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:30:08.323897 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/chart.html
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/delete.html
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/detail.html
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/dispatch.html
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/full.html
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:30:08.323897 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/modal/
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/partial.html
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:30:08.323897 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/templatetags/htmx_viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/views.py
--rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-08 21:29:53.000000 django-htmx-viewsets-0.0.4/src/htmx_viewsets/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 21:38:51.000000 django-htmx-viewsets-0.0.5/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/django_htmx_viewsets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-08 21:38:57.000000 django-htmx-viewsets-0.0.5/src/django_htmx_viewsets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-04-08 21:38:57.000000 django-htmx-viewsets-0.0.5/src/django_htmx_viewsets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 21:38:57.000000 django-htmx-viewsets-0.0.5/src/django_htmx_viewsets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-08 21:38:57.000000 django-htmx-viewsets-0.0.5/src/django_htmx_viewsets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-08 21:38:57.000000 django-htmx-viewsets-0.0.5/src/django_htmx_viewsets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.949133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-08 21:38:51.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4655 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20012 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/bootstrap/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.949133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/bootstrap/5.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)   194901 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    60404 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/bootstrap/5.2.3/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/datatables/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.949133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/datatables/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    18721 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    87108 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/datatables/1.13.1/datatables.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.949133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   102025 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/css/all.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   187208 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   108020 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    63952 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    24948 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   394628 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   150124 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/font-awesome/6.4.0/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/htmx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/htmx/1.8.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    41024 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/htmx/1.8.6/htmx.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/jquery/3.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    89795 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/jquery/3.6.4/jquery-3.6.4.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/select2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/select2/4.1.0-rc.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/static/select2/4.1.0-rc.0/select2.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.945133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/chart.html
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/delete.html
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/dispatch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/full.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/modal/
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/partial.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:57.953133 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/templatetags/htmx_viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7054 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11075 2023-04-08 21:38:44.000000 django-htmx-viewsets-0.0.5/src/htmx_viewsets/viewsets.py
```

### Comparing `django-htmx-viewsets-0.0.4/LICENSE` & `django-htmx-viewsets-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/setup.py` & `django-htmx-viewsets-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 setup(
     name='django-htmx-viewsets',
     version=version,
     author="Snake-Soft",
     author_email="info@snake-soft.com",
     description="Viewsets for Django using HTMX, Chartjs and DataTables",
     long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
     license='GPL3',
     package_dir={'': 'src'},
     packages=find_packages('src'),
     include_package_data=True,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Web Environment',
```

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/chart.py` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/chart.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/color.py` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/color.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/fields.py` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/fields.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/forms.py` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/forms.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/table/action.py` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/action.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/table/cell.py` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/cell.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/table/column.py` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/column.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/table/row.py` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/row.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/table/table.py` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/table/table.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/delete.html` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/delete.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/form.html` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/form.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/list.html` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/list.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/modal/formset.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/modal.html` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/modal.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/partial.html` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/partial.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/templates/htmx_viewsets/table.html` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templates/htmx_viewsets/table.html`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/templatetags/htmx_viewsets.py` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/templatetags/htmx_viewsets.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/views.py` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/views.py`

 * *Files identical despite different names*

### Comparing `django-htmx-viewsets-0.0.4/src/htmx_viewsets/viewsets.py` & `django-htmx-viewsets-0.0.5/src/htmx_viewsets/viewsets.py`

 * *Files identical despite different names*

