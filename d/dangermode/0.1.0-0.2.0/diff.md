# Comparing `tmp/dangermode-0.1.0.tar.gz` & `tmp/dangermode-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dangermode-0.1.0.tar", max compression
+gzip compressed data, was "dangermode-0.2.0.tar", max compression
```

## Comparing `dangermode-0.1.0.tar` & `dangermode-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1498 2023-04-08 17:49:45.486300 dangermode-0.1.0/LICENSE
--rw-r--r--   0        0        0     2205 2023-04-08 18:47:15.087793 dangermode-0.1.0/README.md
--rw-r--r--   0        0        0      688 2023-04-08 18:30:04.836882 dangermode-0.1.0/dangermode/__init__.py
--rw-r--r--   0        0        0      738 2023-04-08 18:30:04.837227 dangermode-0.1.0/dangermode/__main__.py
--rw-r--r--   0        0        0      797 2023-04-08 17:49:45.480818 dangermode-0.1.0/dangermode/app.py
--rw-r--r--   0        0        0     2669 2023-04-08 17:49:45.481016 dangermode-0.1.0/dangermode/models.py
--rw-r--r--   0        0        0     2365 2023-04-08 17:49:45.481243 dangermode-0.1.0/dangermode/routes.py
--rw-r--r--   0        0        0    38480 2023-04-08 17:49:45.481925 dangermode-0.1.0/dangermode/static/images/logo.png
--rw-r--r--   0        0        0     1668 2023-04-08 18:30:43.991309 dangermode-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3173 1970-01-01 00:00:00.000000 dangermode-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-04-08 17:49:45.486300 dangermode-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2205 2023-04-08 18:47:15.087793 dangermode-0.2.0/README.md
+-rw-r--r--   0        0        0      688 2023-04-08 19:53:49.280201 dangermode-0.2.0/dangermode/__init__.py
+-rw-r--r--   0        0        0      738 2023-04-08 19:53:22.824382 dangermode-0.2.0/dangermode/__main__.py
+-rw-r--r--   0        0        0      957 2023-04-08 19:53:20.688768 dangermode-0.2.0/dangermode/app.py
+-rw-r--r--   0        0        0     2669 2023-04-08 17:49:45.481016 dangermode-0.2.0/dangermode/models.py
+-rw-r--r--   0        0        0     2365 2023-04-08 17:49:45.481243 dangermode-0.2.0/dangermode/routes.py
+-rw-r--r--   0        0        0    38480 2023-04-08 17:49:45.481925 dangermode-0.2.0/dangermode/static/images/logo.png
+-rw-r--r--   0        0        0     1668 2023-04-08 19:53:49.279987 dangermode-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3173 1970-01-01 00:00:00.000000 dangermode-0.2.0/PKG-INFO
```

### Comparing `dangermode-0.1.0/LICENSE` & `dangermode-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dangermode-0.1.0/README.md` & `dangermode-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dangermode-0.1.0/dangermode/__init__.py` & `dangermode-0.2.0/dangermode/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for Dangermode."""
 
 __author__ = """Kyle Kelley"""
 __email__ = "rgbkrk@gmail.com"
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 
 def activate_dangermode(host="127.0.0.1"):
     """Activate the dangermode plugin for ChatGPT. 🚨
 
     Intended for use in a Jupyter console or IPython kernel, like in the
     Jupyter Notebook or JupyterLab.
```

### Comparing `dangermode-0.1.0/dangermode/__main__.py` & `dangermode-0.2.0/dangermode/__main__.py`

 * *Files identical despite different names*

### Comparing `dangermode-0.1.0/dangermode/app.py` & `dangermode-0.2.0/dangermode/app.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+import importlib.resources
 from fastapi import FastAPI
 from fastapi.staticfiles import StaticFiles
 from fastapi.middleware.cors import CORSMiddleware
 
 from dangermode.routes import router
 
 # We have to set the servers to show an HTTP localhost so that ChatGPT doesn't try HTTPS in development
 app = FastAPI(servers=[{"url": "http://localhost:8000", "description": "Local server"}])
 
 app.include_router(router)
 
-app.mount("/static", StaticFiles(directory="dangermode/static"), name="static")
+# Allow for serving the image asset from the package itself
+static_directory = importlib.resources.files("dangermode") / "static"
+
+app.mount("/static", StaticFiles(directory=str(static_directory)), name="static")
 
 
 # Defined outside of the router so we can call app.openapi()
 @app.get("/openapi.json", include_in_schema=False)
 async def get_openapi():
     return app.openapi()
```

### Comparing `dangermode-0.1.0/dangermode/models.py` & `dangermode-0.2.0/dangermode/models.py`

 * *Files identical despite different names*

### Comparing `dangermode-0.1.0/dangermode/routes.py` & `dangermode-0.2.0/dangermode/routes.py`

 * *Files identical despite different names*

### Comparing `dangermode-0.1.0/dangermode/static/images/logo.png` & `dangermode-0.2.0/dangermode/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `dangermode-0.1.0/pyproject.toml` & `dangermode-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dangermode"
-version = "0.1.0"
+version = "0.2.0"
 homepage = "https://github.com/rgbkrk/dangermode"
 description = "ChatGPT Danger Mode for Jupyter"
 authors = ["Kyle Kelley <rgbkrk@gmail.com>", "Kafonek <matt.kafonek@noteable.io>"]
 readme = "README.md"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
```

### Comparing `dangermode-0.1.0/PKG-INFO` & `dangermode-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dangermode
-Version: 0.1.0
+Version: 0.2.0
 Summary: ChatGPT Danger Mode for Jupyter
 Home-page: https://github.com/rgbkrk/dangermode
 Author: Kyle Kelley
 Author-email: rgbkrk@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

