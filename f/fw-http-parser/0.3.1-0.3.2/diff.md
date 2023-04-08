# Comparing `tmp/fw-http-parser-0.3.1.tar.gz` & `tmp/fw-http-parser-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fw-http-parser-0.3.1.tar", last modified: Sat Apr  8 12:10:55 2023, max compression
+gzip compressed data, was "fw-http-parser-0.3.2.tar", last modified: Sat Apr  8 18:19:27 2023, max compression
```

## Comparing `fw-http-parser-0.3.1.tar` & `fw-http-parser-0.3.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:10:55.375641 fw-http-parser-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-08 12:10:43.000000 fw-http-parser-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-08 12:10:55.375641 fw-http-parser-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-08 12:10:43.000000 fw-http-parser-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:10:55.375641 fw-http-parser-0.3.1/fw_http_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-08 12:10:43.000000 fw-http-parser-0.3.1/fw_http_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-08 12:10:43.000000 fw-http-parser-0.3.1/fw_http_parser/fw_http_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:10:55.375641 fw-http-parser-0.3.1/fw_http_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-08 12:10:55.000000 fw-http-parser-0.3.1/fw_http_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-08 12:10:55.000000 fw-http-parser-0.3.1/fw_http_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 12:10:55.000000 fw-http-parser-0.3.1/fw_http_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-08 12:10:55.000000 fw-http-parser-0.3.1/fw_http_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 12:10:55.375641 fw-http-parser-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-08 12:10:43.000000 fw-http-parser-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:19:27.695929 fw-http-parser-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-08 18:19:17.000000 fw-http-parser-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-08 18:19:27.695929 fw-http-parser-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-08 18:19:17.000000 fw-http-parser-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:19:27.695929 fw-http-parser-0.3.2/fw_http_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-08 18:19:17.000000 fw-http-parser-0.3.2/fw_http_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-08 18:19:17.000000 fw-http-parser-0.3.2/fw_http_parser/fw_http_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:19:27.695929 fw-http-parser-0.3.2/fw_http_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-08 18:19:27.000000 fw-http-parser-0.3.2/fw_http_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-08 18:19:27.000000 fw-http-parser-0.3.2/fw_http_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:19:27.000000 fw-http-parser-0.3.2/fw_http_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-08 18:19:27.000000 fw-http-parser-0.3.2/fw_http_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 18:19:27.695929 fw-http-parser-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-08 18:19:17.000000 fw-http-parser-0.3.2/setup.py
```

### Comparing `fw-http-parser-0.3.1/LICENSE` & `fw-http-parser-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fw-http-parser-0.3.1/fw_http_parser/fw_http_parser.py` & `fw-http-parser-0.3.2/fw_http_parser/fw_http_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 	def __init__(self, data):
 		self.data = data
 		self._headers = []
 
 	@property
 	def body(self):
-		body = re.search('({.+?})', self.data)
+		body = re.search(r'({[\s\S]+?})', self.data)
 		return body.group(0) if body is not None else None
 
 	@property
 	def method(self):
 		method = self.data.split(' ')[0]
 		request_methods = ['GET', 'POST', 'HEAD', 'PUT', 'DELETE', 'CONNECT', 'OPTIONS', 'TRACE', 'PATCH']
 		return method if method in request_methods else None
@@ -28,25 +28,29 @@
 
 	@property
 	def content_type(self):
 		return get_field('Content-Type', self.data)
 
 	@property
 	def headers(self):
-		idx = self.data.find('\r\n\r\n')
+		idx = self.data.find("\r\n\r\n")
 		lines = [line for line in self.data[:idx].split("\r\n")]
 
 		while len(lines):
 			curr = lines.pop(0)
 
 			if curr.find(':') < 0:
 				continue
 
 			key, value = curr.split(':', 1)
 			self._headers.append((key, value.strip()))
 
 		return self._headers
 
+	@property
+	def route(self):
+		return self.data.split(' ')[1]
+
 
 def get_field(name, data) -> str | None:
 	value = re.search(rf'{name}:\s(.+?)\s', data)
 	return value.group(1) if value is not None else None
```

### Comparing `fw-http-parser-0.3.1/setup.py` & `fw-http-parser-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as md:
 	long_description = md.read()
 
 setuptools.setup(
 	name="fw-http-parser",
-	version="0.3.1",
+	version="0.3.2",
 	author="fwRelik",
 	author_email="relik.fw@gmail.com",
 	description="Parsing data from a socket connection",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/fwRelik/fw-http-parser",
 	packages=setuptools.find_packages(),
```

