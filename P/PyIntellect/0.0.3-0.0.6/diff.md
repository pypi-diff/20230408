# Comparing `tmp/PyIntellect-0.0.3.tar.gz` & `tmp/PyIntellect-0.0.6.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyIntellect-0.0.3.tar", last modified: Sat Apr  8 17:00:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

