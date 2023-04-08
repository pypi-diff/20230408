# Comparing `tmp/tradingbutler-0.1.8.tar.gz` & `tmp/tradingbutler-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradingbutler-0.1.8.tar", max compression
+gzip compressed data, was "tradingbutler-0.1.9.tar", max compression
```

## Comparing `tradingbutler-0.1.8.tar` & `tradingbutler-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1058 2022-11-07 16:40:32.960098 tradingbutler-0.1.8/LICENSE
--rw-r--r--   0        0        0      478 2023-03-04 22:08:12.609599 tradingbutler-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       70 2022-12-12 16:51:47.633372 tradingbutler-0.1.8/README.md
--rw-r--r--   0        0        0        0 2022-12-12 16:37:17.567396 tradingbutler-0.1.8/tradingbutler/__init__.py
--rw-r--r--   0        0        0     8527 2023-03-04 21:12:31.081751 tradingbutler-0.1.8/tradingbutler/summary.py
--rw-r--r--   0        0        0      551 2022-10-19 16:35:57.111425 tradingbutler-0.1.8/tradingbutler/templates/template.html
--rw-r--r--   0        0        0        0 2022-12-12 16:38:51.593784 tradingbutler-0.1.8/tradingbutler/tests/__init__.py
--rw-r--r--   0        0        0      153 2022-12-21 18:41:49.328115 tradingbutler-0.1.8/tradingbutler/tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    15847 2022-12-21 20:14:11.065156 tradingbutler-0.1.8/tradingbutler/tests/__pycache__/tests.cpython-310-pytest-7.1.3.pyc
--rw-r--r--   0        0        0    18806 2022-12-21 20:14:10.735933 tradingbutler-0.1.8/tradingbutler/tests/tests.py
--rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 tradingbutler-0.1.8/setup.py
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 tradingbutler-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1058 2022-11-07 16:40:32.960098 tradingbutler-0.1.9/LICENSE
+-rw-r--r--   0        0        0      478 2023-04-07 22:05:41.168918 tradingbutler-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       70 2022-12-12 16:51:47.633372 tradingbutler-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2022-12-12 16:37:17.567396 tradingbutler-0.1.9/tradingbutler/__init__.py
+-rw-r--r--   0        0        0     8715 2023-04-07 22:04:00.084284 tradingbutler-0.1.9/tradingbutler/summary.py
+-rw-r--r--   0        0        0      551 2022-10-19 16:35:57.111425 tradingbutler-0.1.9/tradingbutler/templates/template.html
+-rw-r--r--   0        0        0        0 2022-12-12 16:38:51.593784 tradingbutler-0.1.9/tradingbutler/tests/__init__.py
+-rw-r--r--   0        0        0      153 2022-12-21 18:41:49.328115 tradingbutler-0.1.9/tradingbutler/tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    15847 2022-12-21 20:14:11.065156 tradingbutler-0.1.9/tradingbutler/tests/__pycache__/tests.cpython-310-pytest-7.1.3.pyc
+-rw-r--r--   0        0        0    18806 2022-12-21 20:14:10.735933 tradingbutler-0.1.9/tradingbutler/tests/tests.py
+-rw-r--r--   0        0        0      779 1970-01-01 00:00:00.000000 tradingbutler-0.1.9/setup.py
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 tradingbutler-0.1.9/PKG-INFO
```

### Comparing `tradingbutler-0.1.8/LICENSE` & `tradingbutler-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tradingbutler-0.1.8/tradingbutler/summary.py` & `tradingbutler-0.1.9/tradingbutler/summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,21 @@
     loader=PackageLoader(__package__),
     autoescape=select_autoescape()
 )
 
 
 class BaseTradeImporter:
     def __init__(self, json_string):
-        self.trades = json.loads(json_string, parse_float=Decimal)
+        parsed = json.loads(json_string, parse_float=Decimal)
+        if isinstance(parsed, list):
+            self.trades = parsed
+        elif isinstance(parsed, dict):
+            self.trades = [parsed]
+        else:
+            raise ValueError
         self.legs = self.get_legs(self.trades)
 
     @classmethod
     def from_path(cls, path):
         json_string = cls.read_file(cls, path)
         return cls(json_string)
```

### Comparing `tradingbutler-0.1.8/tradingbutler/templates/template.html` & `tradingbutler-0.1.9/tradingbutler/templates/template.html`

 * *Files identical despite different names*

### Comparing `tradingbutler-0.1.8/tradingbutler/tests/__pycache__/tests.cpython-310-pytest-7.1.3.pyc` & `tradingbutler-0.1.9/tradingbutler/tests/__pycache__/tests.cpython-310-pytest-7.1.3.pyc`

 * *Files identical despite different names*

### Comparing `tradingbutler-0.1.8/tradingbutler/tests/tests.py` & `tradingbutler-0.1.9/tradingbutler/tests/tests.py`

 * *Files identical despite different names*

### Comparing `tradingbutler-0.1.8/setup.py` & `tradingbutler-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*'], 'tradingbutler': ['templates/*']}
 
 install_requires = \
 ['Jinja2>=3.1.2,<4.0.0', 'python-dateutil>=2.8.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'tradingbutler',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': '',
     'long_description': '# tradingbutler\n\norganizes data from trades and turn into statistics',
     'author': 'Robin Huo',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Robinhuo1/tradingbutler',
```

### Comparing `tradingbutler-0.1.8/PKG-INFO` & `tradingbutler-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradingbutler
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Home-page: https://github.com/Robinhuo1/tradingbutler
 License: MIT
 Author: Robin Huo
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

