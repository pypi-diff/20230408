# Comparing `tmp/flask_util_js-0.2.8.tar.gz` & `tmp/flask_util_js-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/flask_util_js-0.2.8.tar", last modified: Tue Jul 16 04:13:18 2013, max compression
+gzip compressed data, was "dist/flask_util_js-0.2.9.tar", last modified: Tue Jul 16 05:42:09 2013, max compression
```

## Comparing `flask_util_js-0.2.8.tar` & `flask_util_js-0.2.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 zny2008    (501) staff       (20)        0 2013-07-16 04:13:18.000000 flask_util_js-0.2.8/
-drwxr-xr-x   0 zny2008    (501) staff       (20)        0 2013-07-16 04:13:18.000000 flask_util_js-0.2.8/flask_util_js.egg-info/
--rw-r--r--   0 zny2008    (501) staff       (20)        1 2013-07-16 04:13:17.000000 flask_util_js-0.2.8/flask_util_js.egg-info/dependency_links.txt
--rw-r--r--   0 zny2008    (501) staff       (20)        1 2012-10-22 14:30:43.000000 flask_util_js-0.2.8/flask_util_js.egg-info/not-zip-safe
--rw-r--r--   0 zny2008    (501) staff       (20)      265 2013-07-16 04:13:17.000000 flask_util_js-0.2.8/flask_util_js.egg-info/PKG-INFO
--rw-r--r--   0 zny2008    (501) staff       (20)      209 2013-07-16 04:13:17.000000 flask_util_js-0.2.8/flask_util_js.egg-info/SOURCES.txt
--rw-r--r--   0 zny2008    (501) staff       (20)       14 2013-07-16 04:13:17.000000 flask_util_js-0.2.8/flask_util_js.egg-info/top_level.txt
--rw-r--r--   0 zny2008    (501) staff       (20)     4657 2013-07-16 04:04:51.000000 flask_util_js-0.2.8/flask_util_js.py
--rw-r--r--   0 zny2008    (501) staff       (20)      265 2013-07-16 04:13:18.000000 flask_util_js-0.2.8/PKG-INFO
--rw-r--r--   0 zny2008    (501) staff       (20)       59 2013-07-16 04:13:18.000000 flask_util_js-0.2.8/setup.cfg
--rw-r--r--   0 zny2008    (501) staff       (20)      366 2013-07-16 04:04:09.000000 flask_util_js-0.2.8/setup.py
+drwxr-xr-x   0 zny2008    (501) staff       (20)        0 2013-07-16 05:42:09.000000 flask_util_js-0.2.9/
+drwxr-xr-x   0 zny2008    (501) staff       (20)        0 2013-07-16 05:42:09.000000 flask_util_js-0.2.9/flask_util_js.egg-info/
+-rw-r--r--   0 zny2008    (501) staff       (20)        1 2013-07-16 05:42:08.000000 flask_util_js-0.2.9/flask_util_js.egg-info/dependency_links.txt
+-rw-r--r--   0 zny2008    (501) staff       (20)        1 2012-10-22 14:30:43.000000 flask_util_js-0.2.9/flask_util_js.egg-info/not-zip-safe
+-rw-r--r--   0 zny2008    (501) staff       (20)      265 2013-07-16 05:42:08.000000 flask_util_js-0.2.9/flask_util_js.egg-info/PKG-INFO
+-rw-r--r--   0 zny2008    (501) staff       (20)      209 2013-07-16 05:42:08.000000 flask_util_js-0.2.9/flask_util_js.egg-info/SOURCES.txt
+-rw-r--r--   0 zny2008    (501) staff       (20)       14 2013-07-16 05:42:08.000000 flask_util_js-0.2.9/flask_util_js.egg-info/top_level.txt
+-rw-r--r--   0 zny2008    (501) staff       (20)     4859 2013-07-16 05:38:35.000000 flask_util_js-0.2.9/flask_util_js.py
+-rw-r--r--   0 zny2008    (501) staff       (20)      265 2013-07-16 05:42:09.000000 flask_util_js-0.2.9/PKG-INFO
+-rw-r--r--   0 zny2008    (501) staff       (20)       59 2013-07-16 05:42:09.000000 flask_util_js-0.2.9/setup.cfg
+-rw-r--r--   0 zny2008    (501) staff       (20)      366 2013-07-16 05:04:17.000000 flask_util_js-0.2.9/setup.py
```

### Comparing `flask_util_js-0.2.8/flask_util_js.py` & `flask_util_js-0.2.9/flask_util_js.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,30 +21,32 @@
 #               0.2.0 | dantezhu | 2012-10-22 21:53:14 | 优化为实例的方式
 #               0.2.3 | dantezhu | 2012-11-20 11:13:22 | 增加no cache
 #               0.2.4 | dantezhu | 2012-11-30 10:58:13 | content-type
 #               0.2.5 | dantezhu | 2012-12-04 11:41:15 | defaults不需要，缺少params报异常
 #               0.2.6 | dantezhu | 2013-07-15 16:44:12 | fix bug，当params中有为0的参数时，不正常
 #               0.2.7 | dantezhu | 2013-07-16 01:28:20 | 增加js直接渲染
 #               0.2.8 | dantezhu | 2013-07-16 12:04:23 | 使用encodeURIComponent，否则中文有问题
+#               0.2.9 | dantezhu | 2013-07-16 12:04:23 | 用tojson，支持直接放到html中
 #
 #=============================================================================
 '''
 
-__version__ = (0, 2, 8)
+__version__ = (0, 2, 9)
 
 from flask import Response, Markup
-from flask import render_template_string, json
+from flask import current_app
+from flask import render_template_string
 
 FLASK_UTIL_JS_PATH = '/flask_util.js'
 
 FLASK_UTIL_JS_TPL_STRING = '''
 {% autoescape false %}
 
 var flask_util = function() {
-    var url_map = {{ json_url_map }};
+    var url_map = {{ url_map|tojson }};
 
     function url_for(endpoint, params) {
         if (!params) {
             params = {};
         }
         if (!url_map[endpoint]) {
             return '';
@@ -119,33 +121,16 @@
         self._app = app
             
         path = app.config.get('FLASK_UTIL_JS_PATH', FLASK_UTIL_JS_PATH)
         endpoint = app.config.get('FLASK_UTIL_JS_ENDPOINT', None)
 
         @app.route(path, endpoint=endpoint)
         def flask_util_js():
-            org_url_map = app.url_map._rules_by_endpoint
-
-            #把重的逻辑还是放到python代码里
-            url_map = dict()
-
-            for k,v in org_url_map.items():
-                url_map[k] = dict(
-                    rule=v[0].rule,
-                    )
-
-            json_url_map = json.dumps(url_map, indent=4, ensure_ascii=False)
-
-            rv = render_template_string(
-                FLASK_UTIL_JS_TPL_STRING, 
-                json_url_map=json_url_map
-                )
-
             return Response(
-                rv,
+                self.content,
                 content_type='text/javascript; charset=UTF-8',
                 headers={
                     'Cache-Control':'no-cache',
                 }
             )
         
         # 最后把数据写到实例里
@@ -157,9 +142,32 @@
         return self._path
 
     @property
     def endpoint(self):
         return self._endpoint
 
     @property
+    def content(self):
+        org_url_map = current_app.url_map._rules_by_endpoint
+
+        #把重的逻辑还是放到python代码里
+        url_map = dict()
+
+        for k,v in org_url_map.items():
+            url_map[k] = dict(
+                rule=v[0].rule,
+                )
+
+        data = render_template_string(
+            FLASK_UTIL_JS_TPL_STRING, 
+            url_map=url_map,
+            )
+
+        return data
+
+    @property
     def js(self):
-        return Markup('<script src="%s" type="text/javascript" charset="utf-8"></script>') % self.path
+        return Markup('<script src="%s" type="text/javascript" charset="utf-8"></script>' % self.path)
+
+    @property
+    def html(self):
+        return Markup('<script type="text/javascript" charset="utf-8">%s</script>' % self.content)
```

