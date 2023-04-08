# Comparing `tmp/django-vnpay-0.0.7.tar.gz` & `tmp/django-vnpay-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vnpay-0.0.7.tar", last modified: Sat Apr  8 16:08:27 2023, max compression
+gzip compressed data, was "django-vnpay-0.0.9.tar", last modified: Sat Apr  8 16:14:02 2023, max compression
```

## Comparing `django-vnpay-0.0.7.tar` & `django-vnpay-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 macbookpro   (504) staff       (20)        0 2023-04-08 16:08:27.747044 django-vnpay-0.0.7/
--rw-r--r--   0 macbookpro   (504) staff       (20)    11357 2023-04-08 12:29:04.000000 django-vnpay-0.0.7/LICENSE
--rw-r--r--   0 macbookpro   (504) staff       (20)       95 2023-04-08 12:37:08.000000 django-vnpay-0.0.7/MANIFEST.in
--rw-r--r--   0 macbookpro   (504) staff       (20)    14243 2023-04-08 16:08:27.746561 django-vnpay-0.0.7/PKG-INFO
--rw-r--r--   0 macbookpro   (504) staff       (20)      769 2023-04-08 16:07:53.000000 django-vnpay-0.0.7/README.md
-drwxr-xr-x   0 macbookpro   (504) staff       (20)        0 2023-04-08 16:08:27.731632 django-vnpay-0.0.7/django_vnpay.egg-info/
--rw-r--r--   0 macbookpro   (504) staff       (20)    14243 2023-04-08 16:08:27.000000 django-vnpay-0.0.7/django_vnpay.egg-info/PKG-INFO
--rw-r--r--   0 macbookpro   (504) staff       (20)      664 2023-04-08 16:08:27.000000 django-vnpay-0.0.7/django_vnpay.egg-info/SOURCES.txt
--rw-r--r--   0 macbookpro   (504) staff       (20)        1 2023-04-08 16:08:27.000000 django-vnpay-0.0.7/django_vnpay.egg-info/dependency_links.txt
--rw-r--r--   0 macbookpro   (504) staff       (20)      102 2023-04-08 16:08:27.000000 django-vnpay-0.0.7/django_vnpay.egg-info/requires.txt
--rw-r--r--   0 macbookpro   (504) staff       (20)        6 2023-04-08 16:08:27.000000 django-vnpay-0.0.7/django_vnpay.egg-info/top_level.txt
--rw-r--r--   0 macbookpro   (504) staff       (20)     1112 2023-04-08 16:07:53.000000 django-vnpay-0.0.7/pyproject.toml
--rw-r--r--   0 macbookpro   (504) staff       (20)       38 2023-04-08 16:08:27.747185 django-vnpay-0.0.7/setup.cfg
--rw-r--r--   0 macbookpro   (504) staff       (20)       38 2023-04-08 11:34:03.000000 django-vnpay-0.0.7/setup.py
-drwxr-xr-x   0 macbookpro   (504) staff       (20)        0 2023-04-08 16:08:27.737309 django-vnpay-0.0.7/vnpay/
--rw-r--r--   0 macbookpro   (504) staff       (20)        0 2023-04-08 09:36:08.000000 django-vnpay-0.0.7/vnpay/__init__.py
--rw-r--r--   0 macbookpro   (504) staff       (20)      854 2023-04-08 10:48:06.000000 django-vnpay-0.0.7/vnpay/admin.py
-drwxr-xr-x   0 macbookpro   (504) staff       (20)        0 2023-04-08 16:08:27.740868 django-vnpay-0.0.7/vnpay/api/
--rw-r--r--   0 macbookpro   (504) staff       (20)        0 2023-04-02 14:03:20.000000 django-vnpay-0.0.7/vnpay/api/__init__.py
--rw-r--r--   0 macbookpro   (504) staff       (20)     3109 2023-04-08 09:40:32.000000 django-vnpay-0.0.7/vnpay/api/payment_ipn.py
--rw-r--r--   0 macbookpro   (504) staff       (20)     1447 2023-04-08 15:48:58.000000 django-vnpay-0.0.7/vnpay/api/payment_return.py
--rw-r--r--   0 macbookpro   (504) staff       (20)     1033 2023-04-08 09:40:32.000000 django-vnpay-0.0.7/vnpay/api/payment_url.py
--rw-r--r--   0 macbookpro   (504) staff       (20)      451 2023-04-08 10:28:21.000000 django-vnpay-0.0.7/vnpay/api_urls.py
--rw-r--r--   0 macbookpro   (504) staff       (20)      142 2023-04-08 14:35:02.000000 django-vnpay-0.0.7/vnpay/apps.py
-drwxr-xr-x   0 macbookpro   (504) staff       (20)        0 2023-04-08 16:08:27.742983 django-vnpay-0.0.7/vnpay/migrations/
--rw-r--r--   0 macbookpro   (504) staff       (20)     2175 2023-04-08 09:56:20.000000 django-vnpay-0.0.7/vnpay/migrations/0001_initial.py
--rw-r--r--   0 macbookpro   (504) staff       (20)        0 2023-04-08 09:36:08.000000 django-vnpay-0.0.7/vnpay/migrations/__init__.py
--rw-r--r--   0 macbookpro   (504) staff       (20)     2841 2023-04-08 14:36:10.000000 django-vnpay-0.0.7/vnpay/models.py
-drwxr-xr-x   0 macbookpro   (504) staff       (20)        0 2023-04-08 16:08:27.743471 django-vnpay-0.0.7/vnpay/templates/
--rw-r--r--   0 macbookpro   (504) staff       (20)        0 2021-11-09 04:55:44.000000 django-vnpay-0.0.7/vnpay/templates/__init__.py
-drwxr-xr-x   0 macbookpro   (504) staff       (20)        0 2023-04-08 16:08:27.745519 django-vnpay-0.0.7/vnpay/templates/vnpay/
--rw-r--r--   0 macbookpro   (504) staff       (20)     2434 2021-11-09 04:55:44.000000 django-vnpay-0.0.7/vnpay/templates/vnpay/base_layout.html
--rw-r--r--   0 macbookpro   (504) staff       (20)     4110 2021-11-09 04:55:44.000000 django-vnpay-0.0.7/vnpay/templates/vnpay/payment.html
--rw-r--r--   0 macbookpro   (504) staff       (20)     1706 2022-12-22 17:29:02.000000 django-vnpay-0.0.7/vnpay/templates/vnpay/payment_return.html
--rw-r--r--   0 macbookpro   (504) staff       (20)       60 2023-04-08 09:36:08.000000 django-vnpay-0.0.7/vnpay/tests.py
--rw-r--r--   0 macbookpro   (504) staff       (20)     2406 2023-04-05 17:04:09.000000 django-vnpay-0.0.7/vnpay/utils.py
--rw-r--r--   0 macbookpro   (504) staff       (20)       63 2023-04-08 09:36:08.000000 django-vnpay-0.0.7/vnpay/views.py
+drwxr-xr-x   0 macbookpro   (504) staff       (20)        0 2023-04-08 16:14:02.732082 django-vnpay-0.0.9/
+-rw-r--r--   0 macbookpro   (504) staff       (20)    11357 2023-04-08 12:29:04.000000 django-vnpay-0.0.9/LICENSE
+-rw-r--r--   0 macbookpro   (504) staff       (20)       95 2023-04-08 12:37:08.000000 django-vnpay-0.0.9/MANIFEST.in
+-rw-r--r--   0 macbookpro   (504) staff       (20)    14249 2023-04-08 16:14:02.731034 django-vnpay-0.0.9/PKG-INFO
+-rw-r--r--   0 macbookpro   (504) staff       (20)      775 2023-04-08 16:13:13.000000 django-vnpay-0.0.9/README.md
+drwxr-xr-x   0 macbookpro   (504) staff       (20)        0 2023-04-08 16:14:02.715951 django-vnpay-0.0.9/django_vnpay.egg-info/
+-rw-r--r--   0 macbookpro   (504) staff       (20)    14249 2023-04-08 16:14:02.000000 django-vnpay-0.0.9/django_vnpay.egg-info/PKG-INFO
+-rw-r--r--   0 macbookpro   (504) staff       (20)      664 2023-04-08 16:14:02.000000 django-vnpay-0.0.9/django_vnpay.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookpro   (504) staff       (20)        1 2023-04-08 16:14:02.000000 django-vnpay-0.0.9/django_vnpay.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookpro   (504) staff       (20)      102 2023-04-08 16:14:02.000000 django-vnpay-0.0.9/django_vnpay.egg-info/requires.txt
+-rw-r--r--   0 macbookpro   (504) staff       (20)        6 2023-04-08 16:14:02.000000 django-vnpay-0.0.9/django_vnpay.egg-info/top_level.txt
+-rw-r--r--   0 macbookpro   (504) staff       (20)     1120 2023-04-08 16:13:13.000000 django-vnpay-0.0.9/pyproject.toml
+-rw-r--r--   0 macbookpro   (504) staff       (20)       38 2023-04-08 16:14:02.732250 django-vnpay-0.0.9/setup.cfg
+-rw-r--r--   0 macbookpro   (504) staff       (20)       38 2023-04-08 11:34:03.000000 django-vnpay-0.0.9/setup.py
+drwxr-xr-x   0 macbookpro   (504) staff       (20)        0 2023-04-08 16:14:02.721717 django-vnpay-0.0.9/vnpay/
+-rw-r--r--   0 macbookpro   (504) staff       (20)        0 2023-04-08 09:36:08.000000 django-vnpay-0.0.9/vnpay/__init__.py
+-rw-r--r--   0 macbookpro   (504) staff       (20)      854 2023-04-08 10:48:06.000000 django-vnpay-0.0.9/vnpay/admin.py
+drwxr-xr-x   0 macbookpro   (504) staff       (20)        0 2023-04-08 16:14:02.724945 django-vnpay-0.0.9/vnpay/api/
+-rw-r--r--   0 macbookpro   (504) staff       (20)        0 2023-04-02 14:03:20.000000 django-vnpay-0.0.9/vnpay/api/__init__.py
+-rw-r--r--   0 macbookpro   (504) staff       (20)     3109 2023-04-08 09:40:32.000000 django-vnpay-0.0.9/vnpay/api/payment_ipn.py
+-rw-r--r--   0 macbookpro   (504) staff       (20)     1447 2023-04-08 15:48:58.000000 django-vnpay-0.0.9/vnpay/api/payment_return.py
+-rw-r--r--   0 macbookpro   (504) staff       (20)     1033 2023-04-08 09:40:32.000000 django-vnpay-0.0.9/vnpay/api/payment_url.py
+-rw-r--r--   0 macbookpro   (504) staff       (20)      451 2023-04-08 10:28:21.000000 django-vnpay-0.0.9/vnpay/api_urls.py
+-rw-r--r--   0 macbookpro   (504) staff       (20)      142 2023-04-08 14:35:02.000000 django-vnpay-0.0.9/vnpay/apps.py
+drwxr-xr-x   0 macbookpro   (504) staff       (20)        0 2023-04-08 16:14:02.726753 django-vnpay-0.0.9/vnpay/migrations/
+-rw-r--r--   0 macbookpro   (504) staff       (20)     2175 2023-04-08 09:56:20.000000 django-vnpay-0.0.9/vnpay/migrations/0001_initial.py
+-rw-r--r--   0 macbookpro   (504) staff       (20)        0 2023-04-08 09:36:08.000000 django-vnpay-0.0.9/vnpay/migrations/__init__.py
+-rw-r--r--   0 macbookpro   (504) staff       (20)     2841 2023-04-08 14:36:10.000000 django-vnpay-0.0.9/vnpay/models.py
+drwxr-xr-x   0 macbookpro   (504) staff       (20)        0 2023-04-08 16:14:02.727289 django-vnpay-0.0.9/vnpay/templates/
+-rw-r--r--   0 macbookpro   (504) staff       (20)        0 2021-11-09 04:55:44.000000 django-vnpay-0.0.9/vnpay/templates/__init__.py
+drwxr-xr-x   0 macbookpro   (504) staff       (20)        0 2023-04-08 16:14:02.729860 django-vnpay-0.0.9/vnpay/templates/vnpay/
+-rw-r--r--   0 macbookpro   (504) staff       (20)     2434 2021-11-09 04:55:44.000000 django-vnpay-0.0.9/vnpay/templates/vnpay/base_layout.html
+-rw-r--r--   0 macbookpro   (504) staff       (20)     4110 2021-11-09 04:55:44.000000 django-vnpay-0.0.9/vnpay/templates/vnpay/payment.html
+-rw-r--r--   0 macbookpro   (504) staff       (20)     1706 2022-12-22 17:29:02.000000 django-vnpay-0.0.9/vnpay/templates/vnpay/payment_return.html
+-rw-r--r--   0 macbookpro   (504) staff       (20)       60 2023-04-08 09:36:08.000000 django-vnpay-0.0.9/vnpay/tests.py
+-rw-r--r--   0 macbookpro   (504) staff       (20)     2406 2023-04-05 17:04:09.000000 django-vnpay-0.0.9/vnpay/utils.py
+-rw-r--r--   0 macbookpro   (504) staff       (20)       63 2023-04-08 09:36:08.000000 django-vnpay-0.0.9/vnpay/views.py
```

### Comparing `django-vnpay-0.0.7/LICENSE` & `django-vnpay-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-vnpay-0.0.7/PKG-INFO` & `django-vnpay-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vnpay
-Version: 0.0.7
+Version: 0.0.9
 Summary: A quick package for integrating Vnpay payment gateway.
 Author-email: Son Lam <son.lg@eoh.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,15 +214,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 Django-vnpay
 =====
 A quick package for integrating Vnpay payment gateway.
-`Version 0.0.7`
+`Version 0.0.9`
 
 Quick start
 -----------
 
 1. Add "vnpay" to INSTALLED_APPS in `setting.py`
 ```
 INSTALLED_APPS = [
@@ -242,12 +242,12 @@
 
 ```
 path('vnpay/', include('vnpay.api_urls')),
 ```
 
 4. Run ``python manage.py migrate`` to create related models
 
-5. Start the development server and visit http://0.0.7.1:8000/
+5. Start the development server and visit http://127.0.0.1:8000/
 ```
-http://0.0.7.1:8000/admin/ to see the Billing
-http://0.0.7.1:8000/vnpay/ to see the urls
+http://127.0.0.1:8000/admin/ to see the Billing
+http://127.0.0.1:8000/vnpay/ to see the urls
 ```
```

### Comparing `django-vnpay-0.0.7/README.md` & `django-vnpay-0.0.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Django-vnpay
 =====
 A quick package for integrating Vnpay payment gateway.
-`Version 0.0.7`
+`Version 0.0.9`
 
 Quick start
 -----------
 
 1. Add "vnpay" to INSTALLED_APPS in `setting.py`
 ```
 INSTALLED_APPS = [
@@ -25,12 +25,12 @@
 
 ```
 path('vnpay/', include('vnpay.api_urls')),
 ```
 
 4. Run ``python manage.py migrate`` to create related models
 
-5. Start the development server and visit http://0.0.7.1:8000/
+5. Start the development server and visit http://127.0.0.1:8000/
 ```
-http://0.0.7.1:8000/admin/ to see the Billing
-http://0.0.7.1:8000/vnpay/ to see the urls
+http://127.0.0.1:8000/admin/ to see the Billing
+http://127.0.0.1:8000/vnpay/ to see the urls
 ```
```

### Comparing `django-vnpay-0.0.7/django_vnpay.egg-info/PKG-INFO` & `django-vnpay-0.0.9/django_vnpay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-vnpay
-Version: 0.0.7
+Version: 0.0.9
 Summary: A quick package for integrating Vnpay payment gateway.
 Author-email: Son Lam <son.lg@eoh.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,15 +214,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 Django-vnpay
 =====
 A quick package for integrating Vnpay payment gateway.
-`Version 0.0.7`
+`Version 0.0.9`
 
 Quick start
 -----------
 
 1. Add "vnpay" to INSTALLED_APPS in `setting.py`
 ```
 INSTALLED_APPS = [
@@ -242,12 +242,12 @@
 
 ```
 path('vnpay/', include('vnpay.api_urls')),
 ```
 
 4. Run ``python manage.py migrate`` to create related models
 
-5. Start the development server and visit http://0.0.7.1:8000/
+5. Start the development server and visit http://127.0.0.1:8000/
 ```
-http://0.0.7.1:8000/admin/ to see the Billing
-http://0.0.7.1:8000/vnpay/ to see the urls
+http://127.0.0.1:8000/admin/ to see the Billing
+http://127.0.0.1:8000/vnpay/ to see the urls
 ```
```

### Comparing `django-vnpay-0.0.7/django_vnpay.egg-info/SOURCES.txt` & `django-vnpay-0.0.9/django_vnpay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-vnpay-0.0.7/pyproject.toml` & `django-vnpay-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=40.8.0', 'wheel']
 build-backend = 'setuptools.build_meta:__legacy__'
 
 [project]
 name = "django-vnpay"
-version = "0.0.7"
+version = "0.0.9"
 description = "A quick package for integrating Vnpay payment gateway."
 readme = "README.md"
 authors = [{ name = "Son Lam", email = "son.lg@eoh.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -26,22 +26,22 @@
 dev = ["bumpver", "poetry", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/laughlamz/django-vnpay"
 
 
 [tool.bumpver]
-current_version = "0.0.7"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'version = "{version}"',
 ]
 "README.md" = [
-    "{version}",
+    "Version {version}",
 ]
```

### Comparing `django-vnpay-0.0.7/vnpay/admin.py` & `django-vnpay-0.0.9/vnpay/admin.py`

 * *Files identical despite different names*

### Comparing `django-vnpay-0.0.7/vnpay/api/payment_ipn.py` & `django-vnpay-0.0.9/vnpay/api/payment_ipn.py`

 * *Files identical despite different names*

### Comparing `django-vnpay-0.0.7/vnpay/api/payment_return.py` & `django-vnpay-0.0.9/vnpay/api/payment_return.py`

 * *Files identical despite different names*

### Comparing `django-vnpay-0.0.7/vnpay/api/payment_url.py` & `django-vnpay-0.0.9/vnpay/api/payment_url.py`

 * *Files identical despite different names*

### Comparing `django-vnpay-0.0.7/vnpay/migrations/0001_initial.py` & `django-vnpay-0.0.9/vnpay/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-vnpay-0.0.7/vnpay/models.py` & `django-vnpay-0.0.9/vnpay/models.py`

 * *Files identical despite different names*

### Comparing `django-vnpay-0.0.7/vnpay/templates/vnpay/base_layout.html` & `django-vnpay-0.0.9/vnpay/templates/vnpay/base_layout.html`

 * *Files identical despite different names*

### Comparing `django-vnpay-0.0.7/vnpay/templates/vnpay/payment.html` & `django-vnpay-0.0.9/vnpay/templates/vnpay/payment.html`

 * *Files identical despite different names*

### Comparing `django-vnpay-0.0.7/vnpay/templates/vnpay/payment_return.html` & `django-vnpay-0.0.9/vnpay/templates/vnpay/payment_return.html`

 * *Files identical despite different names*

### Comparing `django-vnpay-0.0.7/vnpay/utils.py` & `django-vnpay-0.0.9/vnpay/utils.py`

 * *Files identical despite different names*

