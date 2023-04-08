# Comparing `tmp/fw-http-parser-0.3.0.tar.gz` & `tmp/fw-http-parser-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fw-http-parser-0.3.0.tar", last modified: Sat Apr  8 11:48:37 2023, max compression
+gzip compressed data, was "fw-http-parser-0.3.1.tar", last modified: Sat Apr  8 12:10:55 2023, max compression
```

## Comparing `fw-http-parser-0.3.0.tar` & `fw-http-parser-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:48:37.994106 fw-http-parser-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-08 11:48:29.000000 fw-http-parser-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-08 11:48:37.994106 fw-http-parser-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-08 11:48:29.000000 fw-http-parser-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:48:37.994106 fw-http-parser-0.3.0/fw_http_parser/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-08 11:48:29.000000 fw-http-parser-0.3.0/fw_http_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-08 11:48:29.000000 fw-http-parser-0.3.0/fw_http_parser/fw_http_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 11:48:37.994106 fw-http-parser-0.3.0/fw_http_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-08 11:48:37.000000 fw-http-parser-0.3.0/fw_http_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-08 11:48:37.000000 fw-http-parser-0.3.0/fw_http_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 11:48:37.000000 fw-http-parser-0.3.0/fw_http_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-08 11:48:37.000000 fw-http-parser-0.3.0/fw_http_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 11:48:37.994106 fw-http-parser-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-08 11:48:29.000000 fw-http-parser-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:10:55.375641 fw-http-parser-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-08 12:10:43.000000 fw-http-parser-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-08 12:10:55.375641 fw-http-parser-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-08 12:10:43.000000 fw-http-parser-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:10:55.375641 fw-http-parser-0.3.1/fw_http_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-08 12:10:43.000000 fw-http-parser-0.3.1/fw_http_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-08 12:10:43.000000 fw-http-parser-0.3.1/fw_http_parser/fw_http_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 12:10:55.375641 fw-http-parser-0.3.1/fw_http_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-08 12:10:55.000000 fw-http-parser-0.3.1/fw_http_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-08 12:10:55.000000 fw-http-parser-0.3.1/fw_http_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 12:10:55.000000 fw-http-parser-0.3.1/fw_http_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-08 12:10:55.000000 fw-http-parser-0.3.1/fw_http_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 12:10:55.375641 fw-http-parser-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-08 12:10:43.000000 fw-http-parser-0.3.1/setup.py
```

### Comparing `fw-http-parser-0.3.0/LICENSE` & `fw-http-parser-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fw-http-parser-0.3.0/fw_http_parser/fw_http_parser.py` & `fw-http-parser-0.3.1/fw_http_parser/fw_http_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 		while len(lines):
 			curr = lines.pop(0)
 
 			if curr.find(':') < 0:
 				continue
 
 			key, value = curr.split(':', 1)
-			self._headers.append((key, value))
+			self._headers.append((key, value.strip()))
 
 		return self._headers
 
 
 def get_field(name, data) -> str | None:
 	value = re.search(rf'{name}:\s(.+?)\s', data)
 	return value.group(1) if value is not None else None
```

### Comparing `fw-http-parser-0.3.0/setup.py` & `fw-http-parser-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as md:
 	long_description = md.read()
 
 setuptools.setup(
 	name="fw-http-parser",
-	version="0.3.0",
+	version="0.3.1",
 	author="fwRelik",
 	author_email="relik.fw@gmail.com",
 	description="Parsing data from a socket connection",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://github.com/fwRelik/fw-http-parser",
 	packages=setuptools.find_packages(),
```

