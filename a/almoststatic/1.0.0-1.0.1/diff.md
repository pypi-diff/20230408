# Comparing `tmp/almoststatic-1.0.0.tar.gz` & `tmp/almoststatic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almoststatic-1.0.0.tar", last modified: Tue Mar 21 18:34:10 2023, max compression
+gzip compressed data, was "almoststatic-1.0.1.tar", last modified: Sat Apr  8 18:13:43 2023, max compression
```

## Comparing `almoststatic-1.0.0.tar` & `almoststatic-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-03-21 18:34:10.523902 almoststatic-1.0.0/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     7652 2021-07-11 08:32:04.000000 almoststatic-1.0.0/LICENSE
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     6254 2023-03-21 18:34:10.527902 almoststatic-1.0.0/PKG-INFO
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     5326 2023-03-21 17:43:21.000000 almoststatic-1.0.0/README.md
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-03-21 18:34:10.523902 almoststatic-1.0.0/almoststatic/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)    28142 2023-03-21 18:30:31.000000 almoststatic-1.0.0/almoststatic/__init__.py
-drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-03-21 18:34:10.523902 almoststatic-1.0.0/almoststatic.egg-info/
--rw-rw-r--   0 claudio   (1000) claudio   (1000)     6254 2023-03-21 18:34:10.000000 almoststatic-1.0.0/almoststatic.egg-info/PKG-INFO
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      246 2023-03-21 18:34:10.000000 almoststatic-1.0.0/almoststatic.egg-info/SOURCES.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2023-03-21 18:34:10.000000 almoststatic-1.0.0/almoststatic.egg-info/dependency_links.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       22 2023-03-21 18:34:10.000000 almoststatic-1.0.0/almoststatic.egg-info/requires.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       13 2023-03-21 18:34:10.000000 almoststatic-1.0.0/almoststatic.egg-info/top_level.txt
--rw-rw-r--   0 claudio   (1000) claudio   (1000)       90 2021-07-11 07:09:18.000000 almoststatic-1.0.0/pyproject.toml
--rw-rw-r--   0 claudio   (1000) claudio   (1000)      972 2023-03-21 18:34:10.527902 almoststatic-1.0.0/setup.cfg
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-04-08 18:13:43.442071 almoststatic-1.0.1/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     7652 2021-07-11 08:32:04.000000 almoststatic-1.0.1/LICENSE
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     6254 2023-04-08 18:13:43.442071 almoststatic-1.0.1/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     5326 2023-03-21 17:43:21.000000 almoststatic-1.0.1/README.md
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-04-08 18:13:43.438071 almoststatic-1.0.1/almoststatic/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)    28214 2023-04-08 09:46:31.000000 almoststatic-1.0.1/almoststatic/__init__.py
+drwxrwxr-x   0 claudio   (1000) claudio   (1000)        0 2023-04-08 18:13:43.442071 almoststatic-1.0.1/almoststatic.egg-info/
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)     6254 2023-04-08 18:13:43.000000 almoststatic-1.0.1/almoststatic.egg-info/PKG-INFO
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      246 2023-04-08 18:13:43.000000 almoststatic-1.0.1/almoststatic.egg-info/SOURCES.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)        1 2023-04-08 18:13:43.000000 almoststatic-1.0.1/almoststatic.egg-info/dependency_links.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       22 2023-04-08 18:13:43.000000 almoststatic-1.0.1/almoststatic.egg-info/requires.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       13 2023-04-08 18:13:43.000000 almoststatic-1.0.1/almoststatic.egg-info/top_level.txt
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)       90 2021-07-11 07:09:18.000000 almoststatic-1.0.1/pyproject.toml
+-rw-rw-r--   0 claudio   (1000) claudio   (1000)      972 2023-04-08 18:13:43.442071 almoststatic-1.0.1/setup.cfg
```

### Comparing `almoststatic-1.0.0/LICENSE` & `almoststatic-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `almoststatic-1.0.0/PKG-INFO` & `almoststatic-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almoststatic
-Version: 1.0.0
+Version: 1.0.1
 Summary: Use Jinja2 template system to build static pages with Flask integration
 Home-page: https://gitlab.com/claudio.driussi/almoststatic
 Author: Claudio driussi
 Author-email: claudio.driussi@gmail.com
 License: LGPL
 Keywords: Flask,static,web,"static pages","static sites",html
 Platform: any
```

### Comparing `almoststatic-1.0.0/README.md` & `almoststatic-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `almoststatic-1.0.0/almoststatic/__init__.py` & `almoststatic-1.0.1/almoststatic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,16 @@
         # set globals shortcut
         self.vars = self.env.globals
 
         # load global vars from config.yaml
         self.vars['meta'] = {}
         for k, v in config.items():
             self.env.globals[k] = v
+        # and add config as a dict
+        self.vars['config'] = config
 
         # global configuration
         self.vars['is_static'] = False
         """bool: method write_static set this to True and this let to know to
                  templates when we are writing static pages."""
 
         self.vars['url_prefix'] = ""
```

### Comparing `almoststatic-1.0.0/almoststatic.egg-info/PKG-INFO` & `almoststatic-1.0.1/almoststatic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almoststatic
-Version: 1.0.0
+Version: 1.0.1
 Summary: Use Jinja2 template system to build static pages with Flask integration
 Home-page: https://gitlab.com/claudio.driussi/almoststatic
 Author: Claudio driussi
 Author-email: claudio.driussi@gmail.com
 License: LGPL
 Keywords: Flask,static,web,"static pages","static sites",html
 Platform: any
```

### Comparing `almoststatic-1.0.0/setup.cfg` & `almoststatic-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = almoststatic
-version = 1.0.0
+version = 1.0.1
 author = Claudio driussi
 author_email = claudio.driussi@gmail.com
 description = Use Jinja2 template system to build static pages with Flask integration
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/claudio.driussi/almoststatic
 license = LGPL
```

