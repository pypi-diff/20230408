# Comparing `tmp/signxml-3.1.0.tar.gz` & `tmp/signxml-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signxml-3.1.0.tar", last modified: Wed Jan  4 08:53:37 2023, max compression
+gzip compressed data, was "signxml-3.1.1.tar", last modified: Sat Apr  8 17:05:58 2023, max compression
```

## Comparing `signxml-3.1.0.tar` & `signxml-3.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-01-04 08:53:37.763598 signxml-3.1.0/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    11324 2021-10-07 21:38:03.000000 signxml-3.1.0/LICENSE
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       66 2022-12-16 21:17:49.000000 signxml-3.1.0/MANIFEST.in
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      589 2022-12-16 21:17:49.000000 signxml-3.1.0/NOTICE
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16126 2023-01-04 08:53:37.763853 signxml-3.1.0/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    15281 2022-12-16 21:17:49.000000 signxml-3.1.0/README.rst
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      162 2022-12-16 21:17:49.000000 signxml-3.1.0/pyproject.toml
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      337 2023-01-04 08:53:37.765122 signxml-3.1.0/setup.cfg
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)     1570 2023-01-04 08:52:19.000000 signxml-3.1.0/setup.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-01-04 08:53:37.747158 signxml-3.1.0/signxml/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      612 2022-12-16 21:17:49.000000 signxml-3.1.0/signxml/__init__.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-01-04 08:53:37.755587 signxml-3.1.0/signxml/__pyinstaller/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      224 2022-08-21 15:15:01.000000 signxml-3.1.0/signxml/__pyinstaller/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      231 2022-11-07 16:31:27.000000 signxml-3.1.0/signxml/__pyinstaller/hook-signxml.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     9475 2022-12-16 21:17:49.000000 signxml-3.1.0/signxml/algorithms.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      614 2022-08-24 04:57:56.000000 signxml-3.1.0/signxml/exceptions.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     6770 2022-12-27 02:53:51.000000 signxml-3.1.0/signxml/processor.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        0 2022-08-24 04:57:56.000000 signxml-3.1.0/signxml/py.typed
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-01-04 08:53:37.757198 signxml-3.1.0/signxml/schemas/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    10293 2021-10-07 21:38:03.000000 signxml-3.1.0/signxml/schemas/xmldsig-core-schema.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      900 2021-10-07 21:38:03.000000 signxml-3.1.0/signxml/schemas/xmldsig1-schema.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     4664 2021-10-07 21:38:03.000000 signxml-3.1.0/signxml/schemas/xmldsig11-schema.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    24308 2022-12-27 03:50:38.000000 signxml-3.1.0/signxml/signer.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-01-04 08:53:37.757714 signxml-3.1.0/signxml/util/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     8963 2022-12-16 21:17:49.000000 signxml-3.1.0/signxml/util/__init__.py
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    31486 2022-12-27 03:30:42.000000 signxml-3.1.0/signxml/verifier.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-01-04 08:53:37.758762 signxml-3.1.0/signxml/xades/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     1938 2022-12-16 21:17:49.000000 signxml-3.1.0/signxml/xades/__init__.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-01-04 08:53:37.762485 signxml-3.1.0/signxml/xades/schemas/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    21737 2022-11-07 16:31:27.000000 signxml-3.1.0/signxml/xades/schemas/XAdES.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    24227 2022-11-07 16:31:27.000000 signxml-3.1.0/signxml/xades/schemas/XAdES01903v132-201506.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    24056 2022-11-07 16:31:27.000000 signxml-3.1.0/signxml/xades/schemas/XAdES01903v132-201601.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     2664 2022-11-07 16:31:27.000000 signxml-3.1.0/signxml/xades/schemas/XAdES01903v141-201506.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)     3184 2022-11-07 16:31:27.000000 signxml-3.1.0/signxml/xades/schemas/XAdES01903v141-201601.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      910 2022-11-07 16:31:27.000000 signxml-3.1.0/signxml/xades/schemas/XAdESv141.xsd
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    19948 2022-12-16 21:17:49.000000 signxml-3.1.0/signxml/xades/xades.py
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-01-04 08:53:37.749857 signxml-3.1.0/signxml.egg-info/
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)    16126 2023-01-04 08:53:37.000000 signxml-3.1.0/signxml.egg-info/PKG-INFO
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)      931 2023-01-04 08:53:37.000000 signxml-3.1.0/signxml.egg-info/SOURCES.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        1 2023-01-04 08:53:37.000000 signxml-3.1.0/signxml.egg-info/dependency_links.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       64 2023-01-04 08:53:37.000000 signxml-3.1.0/signxml.egg-info/entry_points.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)       72 2023-01-04 08:53:37.000000 signxml-3.1.0/signxml.egg-info/requires.txt
--rw-r--r--   0 andrey.kislyuk   (502) staff       (20)        8 2023-01-04 08:53:37.000000 signxml-3.1.0/signxml.egg-info/top_level.txt
-drwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)        0 2023-01-04 08:53:37.763038 signxml-3.1.0/test/
--rwxr-xr-x   0 andrey.kislyuk   (502) staff       (20)    37880 2022-12-27 03:36:42.000000 signxml-3.1.0/test/test.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.903171 signxml-3.1.1/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    11324 2016-06-14 14:22:58.000000 signxml-3.1.1/LICENSE
+-rw-r--r--   0 kislyuk    (501) staff       (20)       66 2022-11-14 00:33:49.000000 signxml-3.1.1/MANIFEST.in
+-rw-r--r--   0 kislyuk    (501) staff       (20)      589 2022-11-13 06:37:55.000000 signxml-3.1.1/NOTICE
+-rw-r--r--   0 kislyuk    (501) staff       (20)    16566 2023-04-08 17:05:58.903255 signxml-3.1.1/PKG-INFO
+-rw-r--r--   0 kislyuk    (501) staff       (20)    15648 2023-04-08 16:53:45.000000 signxml-3.1.1/README.rst
+-rw-r--r--   0 kislyuk    (501) staff       (20)      288 2023-04-08 16:53:45.000000 signxml-3.1.1/pyproject.toml
+-rw-r--r--   0 kislyuk    (501) staff       (20)      177 2023-04-08 17:05:58.903514 signxml-3.1.1/setup.cfg
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)     1809 2023-04-08 17:04:57.000000 signxml-3.1.1/setup.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.897920 signxml-3.1.1/signxml/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      612 2022-11-27 19:29:34.000000 signxml-3.1.1/signxml/__init__.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.899371 signxml-3.1.1/signxml/__pyinstaller/
+-rw-r--r--   0 kislyuk    (501) staff       (20)      224 2022-10-23 23:38:52.000000 signxml-3.1.1/signxml/__pyinstaller/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      231 2022-10-23 23:38:52.000000 signxml-3.1.1/signxml/__pyinstaller/hook-signxml.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     9569 2023-04-08 16:53:45.000000 signxml-3.1.1/signxml/algorithms.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)      614 2022-10-23 23:38:52.000000 signxml-3.1.1/signxml/exceptions.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)     6770 2022-11-30 03:47:11.000000 signxml-3.1.1/signxml/processor.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)        0 2022-10-23 23:38:52.000000 signxml-3.1.1/signxml/py.typed
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.900077 signxml-3.1.1/signxml/schemas/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    10293 2016-06-14 14:23:02.000000 signxml-3.1.1/signxml/schemas/xmldsig-core-schema.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)      900 2016-06-14 14:23:02.000000 signxml-3.1.1/signxml/schemas/xmldsig1-schema.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)     4664 2016-06-14 14:23:02.000000 signxml-3.1.1/signxml/schemas/xmldsig11-schema.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)    24308 2023-01-09 03:45:25.000000 signxml-3.1.1/signxml/signer.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.900311 signxml-3.1.1/signxml/util/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     8963 2023-04-08 16:53:42.000000 signxml-3.1.1/signxml/util/__init__.py
+-rw-r--r--   0 kislyuk    (501) staff       (20)    31486 2023-04-08 16:53:42.000000 signxml-3.1.1/signxml/verifier.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.900676 signxml-3.1.1/signxml/xades/
+-rw-r--r--   0 kislyuk    (501) staff       (20)     1938 2022-11-27 20:16:00.000000 signxml-3.1.1/signxml/xades/__init__.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.902513 signxml-3.1.1/signxml/xades/schemas/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    21737 2022-10-29 20:33:16.000000 signxml-3.1.1/signxml/xades/schemas/XAdES.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)    24227 2022-10-29 20:33:33.000000 signxml-3.1.1/signxml/xades/schemas/XAdES01903v132-201506.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)    24056 2022-10-29 20:34:00.000000 signxml-3.1.1/signxml/xades/schemas/XAdES01903v132-201601.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)     2664 2022-10-29 20:34:18.000000 signxml-3.1.1/signxml/xades/schemas/XAdES01903v141-201506.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)     3184 2022-10-29 20:32:55.000000 signxml-3.1.1/signxml/xades/schemas/XAdES01903v141-201601.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)      910 2022-10-29 20:31:58.000000 signxml-3.1.1/signxml/xades/schemas/XAdESv141.xsd
+-rw-r--r--   0 kislyuk    (501) staff       (20)    20109 2023-04-08 16:53:45.000000 signxml-3.1.1/signxml/xades/xades.py
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.899024 signxml-3.1.1/signxml.egg-info/
+-rw-r--r--   0 kislyuk    (501) staff       (20)    16566 2023-04-08 17:05:58.000000 signxml-3.1.1/signxml.egg-info/PKG-INFO
+-rw-r--r--   0 kislyuk    (501) staff       (20)      931 2023-04-08 17:05:58.000000 signxml-3.1.1/signxml.egg-info/SOURCES.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)        1 2023-04-08 17:05:58.000000 signxml-3.1.1/signxml.egg-info/dependency_links.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)       64 2023-04-08 17:05:58.000000 signxml-3.1.1/signxml.egg-info/entry_points.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)      123 2023-04-08 17:05:58.000000 signxml-3.1.1/signxml.egg-info/requires.txt
+-rw-r--r--   0 kislyuk    (501) staff       (20)        8 2023-04-08 17:05:58.000000 signxml-3.1.1/signxml.egg-info/top_level.txt
+drwxr-xr-x   0 kislyuk    (501) staff       (20)        0 2023-04-08 17:05:58.902760 signxml-3.1.1/test/
+-rwxr-xr-x   0 kislyuk    (501) staff       (20)    38122 2023-04-08 17:03:48.000000 signxml-3.1.1/test/test.py
```

### Comparing `signxml-3.1.0/LICENSE` & `signxml-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/NOTICE` & `signxml-3.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/PKG-INFO` & `signxml-3.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signxml
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python XML Signature and XAdES library
 Home-page: https://github.com/kislyuk/signxml
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Platform: MacOS X
 Platform: Posix
@@ -13,16 +13,18 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
+Provides-Extra: tests
 License-File: LICENSE
 License-File: NOTICE
 
 SignXML: XML Signature and XAdES in Python
 ==========================================
 
 *SignXML* is an implementation of the W3C `XML Signature <http://en.wikipedia.org/wiki/XML_Signature>`_ standard in
@@ -85,15 +87,15 @@
     root = etree.fromstring(data_to_sign)
     signed_root = XMLSigner().sign(root, key=key, cert=cert)
     verified_data = XMLVerifier().verify(signed_root).signed_xml
 
 To make this example self-sufficient for test purposes:
 
 - Generate a test certificate and key using
-  ``openssl req -x509 -nodes -subj "/CN=test" -days 1 -newkey rsa:2048 > cert.pem``
+  ``openssl req -x509 -nodes -subj "/CN=test" -days 1 -newkey rsa -keyout privkey.pem -out cert.pem``
   (run ``yum install openssl`` on Red Hat).
 - Pass the ``x509_cert=cert`` keyword argument to ``XMLVerifier.verify()``. (In production, ensure this is replaced with
   the correct configuration for the trusted CA or certificate - this determines which signatures your application trusts.)
 
 .. _verifying-saml-assertions:
 
 Verifying SAML assertions
@@ -262,17 +264,24 @@
 * `OWASP SAML Security Cheat Sheet <https://www.owasp.org/index.php/SAML_Security_Cheat_Sheet>`_
 * `Okta Developer Docs: SAML <https://developer.okta.com/standards/SAML/>`_
 
 Bugs
 ~~~~
 Please report bugs, issues, feature requests, etc. on `GitHub <https://github.com/XML-Security/signxml/issues>`_.
 
+Versioning
+~~~~~~~~~~
+This package follows the `Semantic Versioning 2.0.0 <http://semver.org/>`_ standard. To control changes, it is
+recommended that application developers pin the package version and manage it using `pip-tools
+<https://github.com/jazzband/pip-tools>`_ or similar. For library developers, pinning the major version is
+recommended.
+
 License
 -------
-Copyright 2014-2022, Andrey Kislyuk and SignXML contributors. Licensed under the terms of the
+Copyright 2014-2023, Andrey Kislyuk and SignXML contributors. Licensed under the terms of the
 `Apache License, Version 2.0 <http://www.apache.org/licenses/LICENSE-2.0>`_. Distribution of the LICENSE and NOTICE
 files with source copies of this package and derivative works is **REQUIRED** as specified by the Apache License.
 
 .. image:: https://github.com/XML-Security/signxml/workflows/Test%20suite/badge.svg
         :target: https://github.com/XML-Security/signxml/actions
 .. image:: https://codecov.io/github/XML-Security/signxml/coverage.svg?branch=master
         :target: https://codecov.io/github/XML-Security/signxml?branch=master
```

### Comparing `signxml-3.1.0/README.rst` & `signxml-3.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     root = etree.fromstring(data_to_sign)
     signed_root = XMLSigner().sign(root, key=key, cert=cert)
     verified_data = XMLVerifier().verify(signed_root).signed_xml
 
 To make this example self-sufficient for test purposes:
 
 - Generate a test certificate and key using
-  ``openssl req -x509 -nodes -subj "/CN=test" -days 1 -newkey rsa:2048 > cert.pem``
+  ``openssl req -x509 -nodes -subj "/CN=test" -days 1 -newkey rsa -keyout privkey.pem -out cert.pem``
   (run ``yum install openssl`` on Red Hat).
 - Pass the ``x509_cert=cert`` keyword argument to ``XMLVerifier.verify()``. (In production, ensure this is replaced with
   the correct configuration for the trusted CA or certificate - this determines which signatures your application trusts.)
 
 .. _verifying-saml-assertions:
 
 Verifying SAML assertions
@@ -238,17 +238,24 @@
 * `OWASP SAML Security Cheat Sheet <https://www.owasp.org/index.php/SAML_Security_Cheat_Sheet>`_
 * `Okta Developer Docs: SAML <https://developer.okta.com/standards/SAML/>`_
 
 Bugs
 ~~~~
 Please report bugs, issues, feature requests, etc. on `GitHub <https://github.com/XML-Security/signxml/issues>`_.
 
+Versioning
+~~~~~~~~~~
+This package follows the `Semantic Versioning 2.0.0 <http://semver.org/>`_ standard. To control changes, it is
+recommended that application developers pin the package version and manage it using `pip-tools
+<https://github.com/jazzband/pip-tools>`_ or similar. For library developers, pinning the major version is
+recommended.
+
 License
 -------
-Copyright 2014-2022, Andrey Kislyuk and SignXML contributors. Licensed under the terms of the
+Copyright 2014-2023, Andrey Kislyuk and SignXML contributors. Licensed under the terms of the
 `Apache License, Version 2.0 <http://www.apache.org/licenses/LICENSE-2.0>`_. Distribution of the LICENSE and NOTICE
 files with source copies of this package and derivative works is **REQUIRED** as specified by the Apache License.
 
 .. image:: https://github.com/XML-Security/signxml/workflows/Test%20suite/badge.svg
         :target: https://github.com/XML-Security/signxml/actions
 .. image:: https://codecov.io/github/XML-Security/signxml/coverage.svg?branch=master
         :target: https://codecov.io/github/XML-Security/signxml?branch=master
```

### Comparing `signxml-3.1.0/setup.py` & `signxml-3.1.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="signxml",
-    version="3.1.0",
+    version="3.1.1",
     url="https://github.com/kislyuk/signxml",
     license="Apache Software License",
     author="Andrey Kislyuk",
     author_email="kislyuk@gmail.com",
     description="Python XML Signature and XAdES library",
     long_description=open("README.rst").read(),
     python_requires=">=3.7",
@@ -16,14 +16,24 @@
         # Dependencies are restricted by major version range according to semver.
         # By default, version minimums are set to be compatible with the oldest supported Ubuntu LTS (currently 18.04).
         "lxml >= 4.2.1, < 5",
         "cryptography >= 3.4.8",  # Set to the version in Ubuntu 22.04 due to features we need from cryptography 3.1
         "pyOpenSSL >= 17.5.0",
         "certifi >= 2018.1.18",
     ],
+    extras_require={
+        "tests": [
+            "ruff",
+            "coverage",
+            "build",
+            "wheel",
+            "mypy",
+            "lxml-stubs",
+        ]
+    },
     packages=find_packages(exclude=["test"]),
     platforms=["MacOS X", "Posix"],
     package_data={"signxml": ["schemas/*.xsd", "py.typed"]},
     include_package_data=True,
     test_suite="test",
     classifiers=[
         "Intended Audience :: Developers",
@@ -31,10 +41,11 @@
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

### Comparing `signxml-3.1.0/signxml/__init__.py` & `signxml-3.1.1/signxml/__init__.py`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/algorithms.py` & `signxml-3.1.1/signxml/algorithms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Callable
+from typing import Callable, Dict, Type, Union
 
 from cryptography.hazmat.primitives import hashes
 
 from .exceptions import InvalidInput
 
 
 class SignatureConstructionMethod(Enum):
@@ -154,15 +154,15 @@
     EXCLUSIVE_XML_CANONICALIZATION_1_0 = "http://www.w3.org/2001/10/xml-exc-c14n#"
     EXCLUSIVE_XML_CANONICALIZATION_1_0_WITH_COMMENTS = "http://www.w3.org/2001/10/xml-exc-c14n#WithComments"
 
     # The identifier for Canonical XML 2.0 is "http://www.w3.org/2010/xml-c14n2", but it is not a W3C standard.
     # While it is supported by lxml, it's not in general use and not supported by SignXML
 
 
-digest_algorithm_implementations = {
+digest_algorithm_implementations: Dict[Union[DigestAlgorithm, SignatureMethod], Type[hashes.HashAlgorithm]] = {
     DigestAlgorithm.SHA1: hashes.SHA1,
     DigestAlgorithm.SHA224: hashes.SHA224,
     DigestAlgorithm.SHA384: hashes.SHA384,
     DigestAlgorithm.SHA256: hashes.SHA256,
     DigestAlgorithm.SHA512: hashes.SHA512,
     DigestAlgorithm.SHA3_224: hashes.SHA3_224,
     DigestAlgorithm.SHA3_256: hashes.SHA3_256,
```

### Comparing `signxml-3.1.0/signxml/exceptions.py` & `signxml-3.1.1/signxml/exceptions.py`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/processor.py` & `signxml-3.1.1/signxml/processor.py`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/schemas/xmldsig-core-schema.xsd` & `signxml-3.1.1/signxml/schemas/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/schemas/xmldsig1-schema.xsd` & `signxml-3.1.1/signxml/schemas/xmldsig1-schema.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/schemas/xmldsig11-schema.xsd` & `signxml-3.1.1/signxml/schemas/xmldsig11-schema.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/signer.py` & `signxml-3.1.1/signxml/signer.py`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/util/__init__.py` & `signxml-3.1.1/signxml/util/__init__.py`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/verifier.py` & `signxml-3.1.1/signxml/verifier.py`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/xades/__init__.py` & `signxml-3.1.1/signxml/xades/__init__.py`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/xades/schemas/XAdES.xsd` & `signxml-3.1.1/signxml/xades/schemas/XAdES.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/xades/schemas/XAdES01903v132-201506.xsd` & `signxml-3.1.1/signxml/xades/schemas/XAdES01903v132-201506.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/xades/schemas/XAdES01903v132-201601.xsd` & `signxml-3.1.1/signxml/xades/schemas/XAdES01903v132-201601.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/xades/schemas/XAdES01903v141-201506.xsd` & `signxml-3.1.1/signxml/xades/schemas/XAdES01903v141-201506.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/xades/schemas/XAdES01903v141-201601.xsd` & `signxml-3.1.1/signxml/xades/schemas/XAdES01903v141-201601.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/xades/schemas/XAdESv141.xsd` & `signxml-3.1.1/signxml/xades/schemas/XAdESv141.xsd`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/signxml/xades/xades.py` & `signxml-3.1.1/signxml/xades/xades.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,21 +162,23 @@
         for ssp_annotator in self.signed_signature_properties_annotators:
             ssp_annotator(signed_signature_properties, sig_root=sig_root, signing_settings=signing_settings)
         signed_data_object_properties = SubElement(
             signed_properties, xades_tag("SignedDataObjectProperties"), nsmap=self.namespaces
         )
         for dop_annotator in self.signed_data_object_properties_annotators:
             dop_annotator(signed_data_object_properties, sig_root=sig_root, signing_settings=signing_settings)
-        self._add_reference_to_signed_info(sig_root, signed_properties)
+        self._add_reference_to_signed_info(sig_root, signed_properties, Type="http://uri.etsi.org/01903#SignedProperties")
         self._add_reference_to_signed_info(sig_root, key_info)
 
-    def _add_reference_to_signed_info(self, sig_root, node_to_reference):
+    def _add_reference_to_signed_info(self, sig_root, node_to_reference, **attrs):
         signed_info = self._find(sig_root, "SignedInfo")
         reference = SubElement(signed_info, ds_tag("Reference"), nsmap=self.namespaces)
         reference.set("URI", f"#{node_to_reference.get('Id')}")
+        for attr_name, attr_value in attrs.items():
+            reference.set(attr_name, attr_value)
         SubElement(reference, ds_tag("DigestMethod"), nsmap=self.namespaces, Algorithm=self.digest_alg.value)
         digest_value_node = SubElement(reference, ds_tag("DigestValue"), nsmap=self.namespaces)
         node_to_reference_c14n = self._c14n(node_to_reference, algorithm=self.c14n_alg)
         digest = self._get_digest(node_to_reference_c14n, algorithm=self.digest_alg)
         digest_value_node.text = b64encode(digest).decode()
 
     def add_signing_time(self, signed_signature_properties, sig_root, signing_settings: SigningSettings):
```

### Comparing `signxml-3.1.0/signxml.egg-info/PKG-INFO` & `signxml-3.1.1/signxml.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signxml
-Version: 3.1.0
+Version: 3.1.1
 Summary: Python XML Signature and XAdES library
 Home-page: https://github.com/kislyuk/signxml
 Author: Andrey Kislyuk
 Author-email: kislyuk@gmail.com
 License: Apache Software License
 Platform: MacOS X
 Platform: Posix
@@ -13,16 +13,18 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
+Provides-Extra: tests
 License-File: LICENSE
 License-File: NOTICE
 
 SignXML: XML Signature and XAdES in Python
 ==========================================
 
 *SignXML* is an implementation of the W3C `XML Signature <http://en.wikipedia.org/wiki/XML_Signature>`_ standard in
@@ -85,15 +87,15 @@
     root = etree.fromstring(data_to_sign)
     signed_root = XMLSigner().sign(root, key=key, cert=cert)
     verified_data = XMLVerifier().verify(signed_root).signed_xml
 
 To make this example self-sufficient for test purposes:
 
 - Generate a test certificate and key using
-  ``openssl req -x509 -nodes -subj "/CN=test" -days 1 -newkey rsa:2048 > cert.pem``
+  ``openssl req -x509 -nodes -subj "/CN=test" -days 1 -newkey rsa -keyout privkey.pem -out cert.pem``
   (run ``yum install openssl`` on Red Hat).
 - Pass the ``x509_cert=cert`` keyword argument to ``XMLVerifier.verify()``. (In production, ensure this is replaced with
   the correct configuration for the trusted CA or certificate - this determines which signatures your application trusts.)
 
 .. _verifying-saml-assertions:
 
 Verifying SAML assertions
@@ -262,17 +264,24 @@
 * `OWASP SAML Security Cheat Sheet <https://www.owasp.org/index.php/SAML_Security_Cheat_Sheet>`_
 * `Okta Developer Docs: SAML <https://developer.okta.com/standards/SAML/>`_
 
 Bugs
 ~~~~
 Please report bugs, issues, feature requests, etc. on `GitHub <https://github.com/XML-Security/signxml/issues>`_.
 
+Versioning
+~~~~~~~~~~
+This package follows the `Semantic Versioning 2.0.0 <http://semver.org/>`_ standard. To control changes, it is
+recommended that application developers pin the package version and manage it using `pip-tools
+<https://github.com/jazzband/pip-tools>`_ or similar. For library developers, pinning the major version is
+recommended.
+
 License
 -------
-Copyright 2014-2022, Andrey Kislyuk and SignXML contributors. Licensed under the terms of the
+Copyright 2014-2023, Andrey Kislyuk and SignXML contributors. Licensed under the terms of the
 `Apache License, Version 2.0 <http://www.apache.org/licenses/LICENSE-2.0>`_. Distribution of the LICENSE and NOTICE
 files with source copies of this package and derivative works is **REQUIRED** as specified by the Apache License.
 
 .. image:: https://github.com/XML-Security/signxml/workflows/Test%20suite/badge.svg
         :target: https://github.com/XML-Security/signxml/actions
 .. image:: https://codecov.io/github/XML-Security/signxml/coverage.svg?branch=master
         :target: https://codecov.io/github/XML-Security/signxml?branch=master
```

### Comparing `signxml-3.1.0/signxml.egg-info/SOURCES.txt` & `signxml-3.1.1/signxml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `signxml-3.1.0/test/test.py` & `signxml-3.1.1/test/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -706,14 +706,19 @@
             doc = etree.parse(fh)
         signer = XAdESSigner(
             signature_policy=self.signature_policy,
             claimed_roles=self.claimed_roles,
             data_object_format=self.data_object_format,
         )
         signed_doc = signer.sign(doc, key=key, cert=cert)
+
+        for ref in signed_doc.findall(".//{http://www.w3.org/2000/09/xmldsig#}Reference"):
+            if "SignedProperties" in ref.get("URI"):
+                self.assertEqual(ref.get("Type"), "http://uri.etsi.org/01903#SignedProperties")
+
         verifier = XAdESVerifier()
         verify_results = verifier.verify(
             signed_doc, x509_cert=cert, expect_references=3, expect_signature_policy=self.signature_policy
         )
         self.assertIsInstance(verify_results[1], XAdESVerifyResult)
         self.assertTrue(hasattr(verify_results[1], "signed_properties"))
```

