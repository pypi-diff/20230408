# Comparing `tmp/graphrole-1.0.3.tar.gz` & `tmp/graphrole-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphrole-1.0.3.tar", last modified: Sat Mar 18 23:42:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

