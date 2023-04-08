# Comparing `tmp/init_tikz-0.1.8.tar.gz` & `tmp/init_tikz-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "init_tikz-0.1.8.tar", max compression
+gzip compressed data, was "init_tikz-0.1.9.tar", max compression
```

## Comparing `init_tikz-0.1.8.tar` & `init_tikz-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-04-05 14:55:28.543442 init_tikz-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-04-05 14:55:28.543377 init_tikz-0.1.8/init_tikz/__init__.py
--rw-r--r--   0        0        0       51 2023-04-05 14:56:28.216356 init_tikz-0.1.8/init_tikz/__main__.py
--rw-r--r--   0        0        0     2017 2023-04-05 16:07:00.465294 init_tikz-0.1.8/init_tikz/functions_tex.py
--rw-r--r--   0        0        0     2300 2023-04-07 22:31:26.415823 init_tikz-0.1.8/init_tikz/main.py
--rw-r--r--   0        0        0      408 2023-04-07 22:31:35.767873 init_tikz-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      333 1970-01-01 00:00:00.000000 init_tikz-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-05 14:55:28.543442 init_tikz-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-04-05 14:55:28.543377 init_tikz-0.1.9/init_tikz/__init__.py
+-rw-r--r--   0        0        0       51 2023-04-05 14:56:28.216356 init_tikz-0.1.9/init_tikz/__main__.py
+-rw-r--r--   0        0        0     2017 2023-04-05 16:07:00.465294 init_tikz-0.1.9/init_tikz/functions_tex.py
+-rw-r--r--   0        0        0     2320 2023-04-07 22:34:13.961496 init_tikz-0.1.9/init_tikz/main.py
+-rw-r--r--   0        0        0      408 2023-04-07 22:34:23.541721 init_tikz-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      333 1970-01-01 00:00:00.000000 init_tikz-0.1.9/PKG-INFO
```

### Comparing `init_tikz-0.1.8/init_tikz/functions_tex.py` & `init_tikz-0.1.9/init_tikz/functions_tex.py`

 * *Files identical despite different names*

### Comparing `init_tikz-0.1.8/init_tikz/main.py` & `init_tikz-0.1.9/init_tikz/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,19 +47,19 @@
         help="Environment to be extracted"
         )
 def main(inputfile, outputfile, environment):
     path_tikz = os.path.dirname(os.path.abspath(inputfile))
     os.makedirs(f'{path_tikz}/tikz', exist_ok=True)
     path_main = os.path.join(f'{path_tikz}/tikz', 'main.tex')
     
-    files = []
     try:
         extract_tex_env(inputfile, outputfile, environment)
         try:
-            files = [f for f in os.listdir(f'./tikz') if os.path.isfile(f)]
+            global files
+            files = [f for f in os.listdir(f'{path_tikz}/tikz') if os.path.isfile(f)]
         except:
             click.echo("Faild to list files.")
     except:
         click.echo("Failed to extract_tex_env")
 
     with open(path_main, 'w') as file:
         file.write(f'\\documentclass{{article}}\n')
```

