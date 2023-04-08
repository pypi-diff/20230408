# Comparing `tmp/django_util_js-0.0.8.tar.gz` & `tmp/django_util_js-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django_util_js-0.0.8.tar", last modified: Mon Dec  9 13:25:27 2013, max compression
+gzip compressed data, was "dist/django_util_js-0.0.9.tar", last modified: Mon Dec  9 14:08:16 2013, max compression
```

## Comparing `django_util_js-0.0.8.tar` & `django_util_js-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 zny2008    (501) staff       (20)        0 2013-12-09 13:25:27.000000 django_util_js-0.0.8/
-drwxr-xr-x   0 zny2008    (501) staff       (20)        0 2013-12-09 13:25:27.000000 django_util_js-0.0.8/django_util_js/
--rw-r--r--   0 zny2008    (501) staff       (20)       23 2013-12-09 13:22:15.000000 django_util_js-0.0.8/django_util_js/__init__.py
--rw-r--r--   0 zny2008    (501) staff       (20)     5274 2013-12-09 13:23:45.000000 django_util_js-0.0.8/django_util_js/views.py
-drwxr-xr-x   0 zny2008    (501) staff       (20)        0 2013-12-09 13:25:27.000000 django_util_js-0.0.8/django_util_js.egg-info/
--rw-r--r--   0 zny2008    (501) staff       (20)        1 2013-12-09 13:25:27.000000 django_util_js-0.0.8/django_util_js.egg-info/dependency_links.txt
--rw-r--r--   0 zny2008    (501) staff       (20)        1 2013-12-08 05:49:05.000000 django_util_js-0.0.8/django_util_js.egg-info/not-zip-safe
--rw-r--r--   0 zny2008    (501) staff       (20)      268 2013-12-09 13:25:27.000000 django_util_js-0.0.8/django_util_js.egg-info/PKG-INFO
--rw-r--r--   0 zny2008    (501) staff       (20)      248 2013-12-09 13:25:27.000000 django_util_js-0.0.8/django_util_js.egg-info/SOURCES.txt
--rw-r--r--   0 zny2008    (501) staff       (20)       15 2013-12-09 13:25:27.000000 django_util_js-0.0.8/django_util_js.egg-info/top_level.txt
--rw-r--r--   0 zny2008    (501) staff       (20)      268 2013-12-09 13:25:27.000000 django_util_js-0.0.8/PKG-INFO
--rw-r--r--   0 zny2008    (501) staff       (20)       59 2013-12-09 13:25:27.000000 django_util_js-0.0.8/setup.cfg
--rw-r--r--   0 zny2008    (501) staff       (20)      424 2013-12-08 05:48:22.000000 django_util_js-0.0.8/setup.py
+drwxr-xr-x   0 zny2008    (501) staff       (20)        0 2013-12-09 14:08:16.000000 django_util_js-0.0.9/
+drwxr-xr-x   0 zny2008    (501) staff       (20)        0 2013-12-09 14:08:16.000000 django_util_js-0.0.9/django_util_js/
+-rw-r--r--   0 zny2008    (501) staff       (20)       23 2013-12-09 14:07:18.000000 django_util_js-0.0.9/django_util_js/__init__.py
+-rw-r--r--   0 zny2008    (501) staff       (20)     5274 2013-12-09 14:07:10.000000 django_util_js-0.0.9/django_util_js/views.py
+drwxr-xr-x   0 zny2008    (501) staff       (20)        0 2013-12-09 14:08:16.000000 django_util_js-0.0.9/django_util_js.egg-info/
+-rw-r--r--   0 zny2008    (501) staff       (20)        1 2013-12-09 14:08:16.000000 django_util_js-0.0.9/django_util_js.egg-info/dependency_links.txt
+-rw-r--r--   0 zny2008    (501) staff       (20)        1 2013-12-08 05:49:05.000000 django_util_js-0.0.9/django_util_js.egg-info/not-zip-safe
+-rw-r--r--   0 zny2008    (501) staff       (20)      268 2013-12-09 14:08:16.000000 django_util_js-0.0.9/django_util_js.egg-info/PKG-INFO
+-rw-r--r--   0 zny2008    (501) staff       (20)      248 2013-12-09 14:08:16.000000 django_util_js-0.0.9/django_util_js.egg-info/SOURCES.txt
+-rw-r--r--   0 zny2008    (501) staff       (20)       15 2013-12-09 14:08:16.000000 django_util_js-0.0.9/django_util_js.egg-info/top_level.txt
+-rw-r--r--   0 zny2008    (501) staff       (20)      268 2013-12-09 14:08:16.000000 django_util_js-0.0.9/PKG-INFO
+-rw-r--r--   0 zny2008    (501) staff       (20)       59 2013-12-09 14:08:16.000000 django_util_js-0.0.9/setup.cfg
+-rw-r--r--   0 zny2008    (501) staff       (20)      424 2013-12-08 05:48:22.000000 django_util_js-0.0.9/setup.py
```

### Comparing `django_util_js-0.0.8/django_util_js/views.py` & `django_util_js-0.0.9/django_util_js/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 """
 
 def django_util_js(request):
 
     RE_KWARG = re.compile(r"(\(\?P\<(.*?)\>.*?\))") #Pattern for recongnizing named parameters in urls
     RE_ARG = re.compile(r"(\(.*?\))") #Pattern for recognizing unnamed url parameters
 
-    def force_src(src):
+    def force_str(src):
         if src is None:
             src = ''
         return src.encode('utf8') if isinstance(src, unicode) else src
 
     def handle_url_module(js_patterns, module_name, prefix=""):
         """
         Load the module and output all of the patterns
@@ -130,18 +130,18 @@
                             #prepare the output for JS resolver
                             full_url = full_url.replace(el[0], "<%s>" % el[1])
                     #after processing all kwargs try args
                     args_matches = RE_ARG.findall(full_url)
                     if args_matches:
                         for el in args_matches:
                             full_url = full_url.replace(el, "<>")#replace by a empty parameter name
-                    js_patterns[force_src(pattern.name)] = force_src("/" + full_url)
+                    js_patterns[force_str(pattern.name)] = force_str("/" + full_url)
                     # add by dantezhu
                     if hasattr(pattern, '_callback_str'):
-                        js_patterns[force_src(pattern._callback_str)] = force_src("/" + full_url)
+                        js_patterns[force_str(pattern._callback_str)] = force_str("/" + full_url)
 
             elif issubclass(pattern.__class__, RegexURLResolver):
                 if pattern.urlconf_name:
                     # modified by dantezhu
                     handle_url_module(js_patterns, pattern.urlconf_name, prefix=prefix+pattern.regex.pattern)
 
     js_patterns = SortedDict()
```

