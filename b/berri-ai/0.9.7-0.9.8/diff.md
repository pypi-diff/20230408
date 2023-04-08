# Comparing `tmp/berri_ai-0.9.7.tar.gz` & `tmp/berri_ai-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "berri_ai-0.9.7.tar", max compression
+gzip compressed data, was "berri_ai-0.9.8.tar", max compression
```

## Comparing `berri_ai-0.9.7.tar` & `berri_ai-0.9.8.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2825 2023-02-01 00:36:52.150618 berri_ai-0.9.7/berri_ai/__init__.py
--rw-r--r--   0        0        0      339 2023-02-01 00:36:54.814612 berri_ai-0.9.7/pyproject.toml
--rw-r--r--   0        0        0      612 2023-02-01 00:36:55.438880 berri_ai-0.9.7/setup.py
--rw-r--r--   0        0        0      425 2023-02-01 00:36:55.439246 berri_ai-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     2824 2023-02-01 00:49:27.252956 berri_ai-0.9.8/berri_ai/__init__.py
+-rw-r--r--   0        0        0      339 2023-02-01 00:49:31.476947 berri_ai-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0      612 2023-02-01 00:49:38.864315 berri_ai-0.9.8/setup.py
+-rw-r--r--   0        0        0      425 2023-02-01 00:49:38.864587 berri_ai-0.9.8/PKG-INFO
```

### Comparing `berri_ai-0.9.7/berri_ai/__init__.py` & `berri_ai-0.9.8/berri_ai/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.9.7'
+__version__ = '0.9.8'
 from google.colab import _message
 import ast 
 import re
 import os 
 import traceback
 import time
 import pipreqs
@@ -18,15 +18,15 @@
     url = f'https://berriserverv2.krrishdholakia.repl.co/berri_orchestrator?user_email={user_email}'
     files_list = []
     
     for file in os.listdir("./berri_files"):
         with open(os.path.join("./berri_files", file), 'rb') as f:
             files_list.append((file, f.read()))
             
-    response = requests.post(url, files=files_list)
+    response = requests.get(url, files=files_list)
     print(response.json())
 
 
 def read_file_copy_files_folders(line):
   # Check if the line contains a path to a file or folder
   path = re.search(r'"([^"]*)"', line)
   if path:
```

### Comparing `berri_ai-0.9.7/setup.py` & `berri_ai-0.9.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pipreqs>=0.4.11,<0.5.0', 'requests>=2.28.2,<3.0.0']
 
 setup_kwargs = {
     'name': 'berri-ai',
-    'version': '0.9.7',
+    'version': '0.9.8',
     'description': '',
     'long_description': None,
     'author': 'Team Berri',
     'author_email': 'clerkieai@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

