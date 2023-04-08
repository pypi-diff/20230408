# Comparing `tmp/s3fs-2023.3.0.tar.gz` & `tmp/s3fs-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3fs-2023.3.0.tar", last modified: Sat Mar  4 19:39:29 2023, max compression
+gzip compressed data, was "s3fs-2023.4.0.tar", last modified: Sat Apr  8 18:01:05 2023, max compression
```

## Comparing `s3fs-2023.3.0.tar` & `s3fs-2023.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 19:39:29.987751 s3fs-2023.3.0/
--rw-r--r--   0 mdurant    (502) staff       (20)     1505 2022-09-18 01:28:11.000000 s3fs-2023.3.0/LICENSE.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      225 2022-09-18 01:28:11.000000 s3fs-2023.3.0/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     1341 2023-03-04 19:39:29.987837 s3fs-2023.3.0/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      620 2022-09-18 01:28:11.000000 s3fs-2023.3.0/README.rst
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 19:39:29.981011 s3fs-2023.3.0/docs/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 19:39:29.983796 s3fs-2023.3.0/docs/source/
--rw-r--r--   0 mdurant    (502) staff       (20)      906 2023-02-23 19:42:13.000000 s3fs-2023.3.0/docs/source/api.rst
--rw-r--r--   0 mdurant    (502) staff       (20)     3921 2023-03-04 19:38:56.000000 s3fs-2023.3.0/docs/source/changelog.rst
--rw-r--r--   0 mdurant    (502) staff       (20)      151 2022-09-18 01:28:11.000000 s3fs-2023.3.0/docs/source/development.rst
--rw-r--r--   0 mdurant    (502) staff       (20)    11488 2023-02-23 19:42:13.000000 s3fs-2023.3.0/docs/source/index.rst
--rw-r--r--   0 mdurant    (502) staff       (20)      530 2022-09-18 01:28:11.000000 s3fs-2023.3.0/docs/source/install.rst
--rw-r--r--   0 mdurant    (502) staff       (20)       64 2023-03-04 19:38:56.000000 s3fs-2023.3.0/requirements.txt
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 19:39:29.988601 s3fs-2023.3.0/s3fs/
--rw-r--r--   0 mdurant    (502) staff       (20)      160 2022-09-18 01:28:11.000000 s3fs-2023.3.0/s3fs/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-03-04 19:39:29.988661 s3fs-2023.3.0/s3fs/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)    82069 2023-02-23 19:42:13.000000 s3fs-2023.3.0/s3fs/core.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7779 2022-09-18 01:28:11.000000 s3fs-2023.3.0/s3fs/errors.py
--rw-r--r--   0 mdurant    (502) staff       (20)      237 2022-09-18 01:28:11.000000 s3fs-2023.3.0/s3fs/mapping.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 19:39:29.987587 s3fs-2023.3.0/s3fs/tests/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:11.000000 s3fs-2023.3.0/s3fs/tests/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2859 2022-09-18 01:28:11.000000 s3fs-2023.3.0/s3fs/tests/test_mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)    78292 2023-02-23 22:09:58.000000 s3fs-2023.3.0/s3fs/tests/test_s3fs.py
--rw-r--r--   0 mdurant    (502) staff       (20)      370 2022-09-18 01:28:11.000000 s3fs-2023.3.0/s3fs/tests/test_utils.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5246 2023-01-02 15:39:19.000000 s3fs-2023.3.0/s3fs/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-03-04 19:39:29.986471 s3fs-2023.3.0/s3fs.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     1341 2023-03-04 19:39:29.000000 s3fs-2023.3.0/s3fs.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      561 2023-03-04 19:39:29.000000 s3fs-2023.3.0/s3fs.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-03-04 19:39:29.000000 s3fs-2023.3.0/s3fs.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-10-19 15:15:30.000000 s3fs-2023.3.0/s3fs.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      135 2023-03-04 19:39:29.000000 s3fs-2023.3.0/s3fs.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        5 2023-03-04 19:39:29.000000 s3fs-2023.3.0/s3fs.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      438 2023-03-04 19:39:29.988166 s3fs-2023.3.0/setup.cfg
--rwxr-xr-x   0 mdurant    (502) staff       (20)     1365 2023-02-23 19:42:13.000000 s3fs-2023.3.0/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    78281 2022-09-18 01:28:11.000000 s3fs-2023.3.0/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 18:01:05.942296 s3fs-2023.4.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1505 2022-09-18 01:28:11.000000 s3fs-2023.4.0/LICENSE.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      225 2022-09-18 01:28:11.000000 s3fs-2023.4.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     1341 2023-04-08 18:01:05.942373 s3fs-2023.4.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      620 2022-09-18 01:28:11.000000 s3fs-2023.4.0/README.rst
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 18:01:05.935002 s3fs-2023.4.0/docs/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 18:01:05.938276 s3fs-2023.4.0/docs/source/
+-rw-r--r--   0 mdurant    (502) staff       (20)      906 2023-02-23 19:42:13.000000 s3fs-2023.4.0/docs/source/api.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)     4029 2023-04-08 17:52:10.000000 s3fs-2023.4.0/docs/source/changelog.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)      151 2022-09-18 01:28:11.000000 s3fs-2023.4.0/docs/source/development.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)    11489 2023-04-08 17:17:48.000000 s3fs-2023.4.0/docs/source/index.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)      530 2022-09-18 01:28:11.000000 s3fs-2023.4.0/docs/source/install.rst
+-rw-r--r--   0 mdurant    (502) staff       (20)       64 2023-04-08 17:51:12.000000 s3fs-2023.4.0/requirements.txt
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 18:01:05.942981 s3fs-2023.4.0/s3fs/
+-rw-r--r--   0 mdurant    (502) staff       (20)      160 2022-09-18 01:28:11.000000 s3fs-2023.4.0/s3fs/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-04-08 18:01:05.943035 s3fs-2023.4.0/s3fs/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    83227 2023-04-08 17:48:33.000000 s3fs-2023.4.0/s3fs/core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7779 2022-09-18 01:28:11.000000 s3fs-2023.4.0/s3fs/errors.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      237 2022-09-18 01:28:11.000000 s3fs-2023.4.0/s3fs/mapping.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 18:01:05.942162 s3fs-2023.4.0/s3fs/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-18 01:28:11.000000 s3fs-2023.4.0/s3fs/tests/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2859 2022-09-18 01:28:11.000000 s3fs-2023.4.0/s3fs/tests/test_mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    78932 2023-04-08 17:48:28.000000 s3fs-2023.4.0/s3fs/tests/test_s3fs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      370 2022-09-18 01:28:11.000000 s3fs-2023.4.0/s3fs/tests/test_utils.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5246 2023-01-02 15:39:19.000000 s3fs-2023.4.0/s3fs/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-04-08 18:01:05.941203 s3fs-2023.4.0/s3fs.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1341 2023-04-08 18:01:05.000000 s3fs-2023.4.0/s3fs.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      561 2023-04-08 18:01:05.000000 s3fs-2023.4.0/s3fs.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-04-08 18:01:05.000000 s3fs-2023.4.0/s3fs.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-10-19 15:15:30.000000 s3fs-2023.4.0/s3fs.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      135 2023-04-08 18:01:05.000000 s3fs-2023.4.0/s3fs.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        5 2023-04-08 18:01:05.000000 s3fs-2023.4.0/s3fs.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      438 2023-04-08 18:01:05.942749 s3fs-2023.4.0/setup.cfg
+-rwxr-xr-x   0 mdurant    (502) staff       (20)     1365 2023-02-23 19:42:13.000000 s3fs-2023.4.0/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    78281 2022-09-18 01:28:11.000000 s3fs-2023.4.0/versioneer.py
```

### Comparing `s3fs-2023.3.0/LICENSE.txt` & `s3fs-2023.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `s3fs-2023.3.0/PKG-INFO` & `s3fs-2023.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3fs
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: Convenient Filesystem interface over S3
 Home-page: http://github.com/fsspec/s3fs/
 Maintainer: Martin Durant
 Maintainer-email: mdurant@continuum.io
 License: BSD
 Keywords: s3,boto
 Classifier: Development Status :: 4 - Beta
```

### Comparing `s3fs-2023.3.0/README.rst` & `s3fs-2023.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `s3fs-2023.3.0/docs/source/api.rst` & `s3fs-2023.4.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `s3fs-2023.3.0/docs/source/changelog.rst` & `s3fs-2023.4.0/docs/source/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+2023.4.0
+--------
+
+- Add streaming async read file (#722)
+- Doc fixes (#721)
+- aiobotocore to 2.5.0 (#710)
+
 2023.3.0
 --------
 
 - Allow setting endpoint_url as top-level kwarg (#704)
 - minimum python version 3.8 (#702)
 - Update docs config (#697)
 - get/put/cp recursive extra tests (#691)
```

### Comparing `s3fs-2023.3.0/docs/source/index.rst` & `s3fs-2023.4.0/docs/source/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -206,14 +206,15 @@
          secret='asecretkey...',
          endpoint_url='https://...'
       )
 
 It is also possible to set credentials through envrironment variables:
 
 .. code-block:: python
+
    # export FSSPEC_S3_ENDPOINT_URL=https://...
    # export FSSPEC_S3_KEY='miniokey...'
    # export FSSPEC_S3_SECRET='asecretkey...'
    >>> s3 = s3fs.S3FileSystem()
    # or ...
    >>> f = fsspec.open("s3://minio-bucket/...")
```

### Comparing `s3fs-2023.3.0/docs/source/install.rst` & `s3fs-2023.4.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `s3fs-2023.3.0/s3fs/core.py` & `s3fs-2023.4.0/s3fs/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from urllib3.exceptions import IncompleteRead
 
 import fsspec  # noqa: F401
 from fsspec.spec import AbstractBufferedFile
 from fsspec.utils import infer_storage_options, tokenize, setup_logging as setup_logger
 from fsspec.asyn import (
     AsyncFileSystem,
+    AbstractAsyncStreamedFile,
     sync,
     sync_wrapper,
     FSTimeoutError,
     _run_coros_in_chunks,
 )
 from fsspec.callbacks import _DEFAULT_CALLBACK
 
@@ -1934,14 +1935,19 @@
         # do nothing.
         cache = getattr(self, "_s3creator", None)
         if cache is not None:
             await cache.clear()
 
     invalidate_region_cache = sync_wrapper(_invalidate_region_cache)
 
+    async def open_async(self, path, mode="rb", **kwargs):
+        if "b" not in mode or kwargs.get("compression"):
+            raise ValueError
+        return S3AsyncStreamedFile(self, path, mode)
+
 
 class S3File(AbstractBufferedFile):
     """
     Open S3 key as a file. Data is only loaded and cached on demand.
 
     Parameters
     ----------
@@ -2273,14 +2279,44 @@
                 Bucket=self.bucket,
                 Key=self.key,
                 UploadId=self.mpu["UploadId"],
             )
             self.mpu = None
 
 
+class S3AsyncStreamedFile(AbstractAsyncStreamedFile):
+    def __init__(self, fs, path, mode):
+        self.fs = fs
+        self.path = path
+        self.mode = mode
+        self.r = None
+
+    async def read(self, length=-1):
+        if self.r is None:
+            bucket, key, gen = self.fs.split_path(self.path)
+            r = await self.fs._call_s3("get_object", Bucket=bucket, Key=key)
+            self.r = r["Body"]
+        return await self.r.read(length)
+
+
+class S3AsyncStreamedFile(AbstractAsyncStreamedFile):
+    def __init__(self, fs, path, mode):
+        self.fs = fs
+        self.path = path
+        self.mode = mode
+        self.r = None
+
+    async def read(self, length=-1):
+        if self.r is None:
+            bucket, key, gen = self.fs.split_path(self.path)
+            r = await self.fs._call_s3("get_object", Bucket=bucket, Key=key)
+            self.r = r["Body"]
+        return await self.r.read(length)
+
+
 def _fetch_range(fs, bucket, key, version_id, start, end, req_kw=None):
     if req_kw is None:
         req_kw = {}
     if start == end:
         logger.debug(
             "skip fetch for negative range - bucket=%s,key=%s,start=%d,end=%d",
             bucket,
```

### Comparing `s3fs-2023.3.0/s3fs/errors.py` & `s3fs-2023.4.0/s3fs/errors.py`

 * *Files identical despite different names*

### Comparing `s3fs-2023.3.0/s3fs/tests/test_mapping.py` & `s3fs-2023.4.0/s3fs/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `s3fs-2023.3.0/s3fs/tests/test_s3fs.py` & `s3fs-2023.4.0/s3fs/tests/test_s3fs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2570,7 +2570,31 @@
     s3.cp([file0, file1], target)
 
     assert s3.isdir(target)
     assert sorted(s3.find(target)) == [
         target + "/file0",
         target + "/file1",
     ]
+
+
+def test_async_stream(s3_base):
+    fn = test_bucket_name + "/target"
+    data = b"hello world" * 1000
+    out = []
+
+    async def read_stream():
+        fs = S3FileSystem(
+            anon=False,
+            client_kwargs={"endpoint_url": endpoint_uri},
+            skip_instance_cache=True,
+        )
+        await fs._mkdir(test_bucket_name)
+        await fs._pipe(fn, data)
+        f = await fs.open_async(fn, mode="rb", block_seze=1000)
+        while True:
+            got = await f.read(1000)
+            if not got:
+                break
+            out.append(got)
+
+    asyncio.run(read_stream())
+    assert b"".join(out) == data
```

### Comparing `s3fs-2023.3.0/s3fs/utils.py` & `s3fs-2023.4.0/s3fs/utils.py`

 * *Files identical despite different names*

### Comparing `s3fs-2023.3.0/s3fs.egg-info/PKG-INFO` & `s3fs-2023.4.0/s3fs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3fs
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: Convenient Filesystem interface over S3
 Home-page: http://github.com/fsspec/s3fs/
 Maintainer: Martin Durant
 Maintainer-email: mdurant@continuum.io
 License: BSD
 Keywords: s3,boto
 Classifier: Development Status :: 4 - Beta
```

### Comparing `s3fs-2023.3.0/s3fs.egg-info/SOURCES.txt` & `s3fs-2023.4.0/s3fs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `s3fs-2023.3.0/setup.py` & `s3fs-2023.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `s3fs-2023.3.0/versioneer.py` & `s3fs-2023.4.0/versioneer.py`

 * *Files identical despite different names*

