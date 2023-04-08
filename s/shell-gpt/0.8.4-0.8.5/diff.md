# Comparing `tmp/shell_gpt-0.8.4.tar.gz` & `tmp/shell_gpt-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shell_gpt-0.8.4.tar", last modified: Fri Apr  7 18:29:43 2023, max compression
+gzip compressed data, was "shell_gpt-0.8.5.tar", last modified: Fri Apr  7 21:58:59 2023, max compression
```

## Comparing `shell_gpt-0.8.4.tar` & `shell_gpt-0.8.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 18:29:43.974816 shell_gpt-0.8.4/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1072 2023-03-14 23:56:44.000000 shell_gpt-0.8.4/LICENSE
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14754 2023-04-07 18:29:43.974589 shell_gpt-0.8.4/PKG-INFO
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14406 2023-04-07 18:29:19.000000 shell_gpt-0.8.4/README.md
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       38 2023-04-07 18:29:43.974855 shell_gpt-0.8.4/setup.cfg
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      829 2023-04-07 18:29:19.000000 shell_gpt-0.8.4/setup.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 18:29:43.972838 shell_gpt-0.8.4/sgpt/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      445 2023-04-04 16:16:05.000000 shell_gpt-0.8.4/sgpt/__init__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       44 2023-03-14 23:56:44.000000 shell_gpt-0.8.4/sgpt/__main__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     4130 2023-04-07 18:29:19.000000 shell_gpt-0.8.4/sgpt/app.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2175 2023-04-02 15:59:57.000000 shell_gpt-0.8.4/sgpt/cache.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     3134 2023-04-02 15:59:57.000000 shell_gpt-0.8.4/sgpt/client.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2380 2023-04-04 16:16:05.000000 shell_gpt-0.8.4/sgpt/config.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 18:29:43.973666 shell_gpt-0.8.4/sgpt/handlers/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-02 15:59:57.000000 shell_gpt-0.8.4/sgpt/handlers/__init__.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     7115 2023-04-04 16:16:05.000000 shell_gpt-0.8.4/sgpt/handlers/chat_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      845 2023-04-02 15:59:57.000000 shell_gpt-0.8.4/sgpt/handlers/default_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1121 2023-04-06 23:34:58.000000 shell_gpt-0.8.4/sgpt/handlers/handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1839 2023-04-07 18:29:19.000000 shell_gpt-0.8.4/sgpt/handlers/repl_handler.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2092 2023-04-07 18:29:19.000000 shell_gpt-0.8.4/sgpt/make_prompt.py
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2276 2023-04-07 18:29:19.000000 shell_gpt-0.8.4/sgpt/utils.py
-drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 18:29:43.974394 shell_gpt-0.8.4/shell_gpt.egg-info/
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14754 2023-04-07 18:29:43.000000 shell_gpt-0.8.4/shell_gpt.egg-info/PKG-INFO
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      494 2023-04-07 18:29:43.000000 shell_gpt-0.8.4/shell_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        1 2023-04-07 18:29:43.000000 shell_gpt-0.8.4/shell_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       34 2023-04-07 18:29:43.000000 shell_gpt-0.8.4/shell_gpt.egg-info/entry_points.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       97 2023-04-07 18:29:43.000000 shell_gpt-0.8.4/shell_gpt.egg-info/requires.txt
--rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        5 2023-04-07 18:29:43.000000 shell_gpt-0.8.4/shell_gpt.egg-info/top_level.txt
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 21:58:59.474375 shell_gpt-0.8.5/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1072 2023-03-14 23:56:44.000000 shell_gpt-0.8.5/LICENSE
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14754 2023-04-07 21:58:59.474136 shell_gpt-0.8.5/PKG-INFO
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14406 2023-04-07 21:51:34.000000 shell_gpt-0.8.5/README.md
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       38 2023-04-07 21:58:59.474411 shell_gpt-0.8.5/setup.cfg
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      829 2023-04-07 21:51:34.000000 shell_gpt-0.8.5/setup.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 21:58:59.471910 shell_gpt-0.8.5/sgpt/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      445 2023-04-04 16:16:05.000000 shell_gpt-0.8.5/sgpt/__init__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       44 2023-03-14 23:56:44.000000 shell_gpt-0.8.5/sgpt/__main__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     4130 2023-04-07 18:29:19.000000 shell_gpt-0.8.5/sgpt/app.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2175 2023-04-02 15:59:57.000000 shell_gpt-0.8.5/sgpt/cache.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     3134 2023-04-02 15:59:57.000000 shell_gpt-0.8.5/sgpt/client.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2380 2023-04-04 16:16:05.000000 shell_gpt-0.8.5/sgpt/config.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 21:58:59.473046 shell_gpt-0.8.5/sgpt/handlers/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-02 15:59:57.000000 shell_gpt-0.8.5/sgpt/handlers/__init__.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     7115 2023-04-04 16:16:05.000000 shell_gpt-0.8.5/sgpt/handlers/chat_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      845 2023-04-02 15:59:57.000000 shell_gpt-0.8.5/sgpt/handlers/default_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1121 2023-04-06 23:34:58.000000 shell_gpt-0.8.5/sgpt/handlers/handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1839 2023-04-07 18:29:19.000000 shell_gpt-0.8.5/sgpt/handlers/repl_handler.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     2092 2023-04-07 18:29:19.000000 shell_gpt-0.8.5/sgpt/make_prompt.py
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)     1771 2023-04-07 21:44:34.000000 shell_gpt-0.8.5/sgpt/utils.py
+drwxr-xr-x   0 farkhod.sadykov   (501) staff       (20)        0 2023-04-07 21:58:59.473919 shell_gpt-0.8.5/shell_gpt.egg-info/
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)    14754 2023-04-07 21:58:59.000000 shell_gpt-0.8.5/shell_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)      494 2023-04-07 21:58:59.000000 shell_gpt-0.8.5/shell_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        1 2023-04-07 21:58:59.000000 shell_gpt-0.8.5/shell_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       34 2023-04-07 21:58:59.000000 shell_gpt-0.8.5/shell_gpt.egg-info/entry_points.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)       97 2023-04-07 21:58:59.000000 shell_gpt-0.8.5/shell_gpt.egg-info/requires.txt
+-rw-r--r--   0 farkhod.sadykov   (501) staff       (20)        5 2023-04-07 21:58:59.000000 shell_gpt-0.8.5/shell_gpt.egg-info/top_level.txt
```

### Comparing `shell_gpt-0.8.4/LICENSE` & `shell_gpt-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.4/PKG-INFO` & `shell_gpt-0.8.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell_gpt
-Version: 0.8.4
+Version: 0.8.5
 Summary: A command-line productivity tool powered by ChatGPT, will help you accomplish your tasks faster and more efficiently.
 Home-page: https://github.com/ther1d/shell_gpt
 Author: Farkhod Sadykov
 Author-email: farkhod@sadykov.dev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -13,15 +13,15 @@
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.4
+pip install shell-gpt==0.8.5
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
```

### Comparing `shell_gpt-0.8.4/README.md` & `shell_gpt-0.8.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.4
+pip install shell-gpt==0.8.5
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
```

### Comparing `shell_gpt-0.8.4/setup.py` & `shell_gpt-0.8.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 # pylint: disable=consider-using-with
 setup(
     name="shell_gpt",
-    version="0.8.4",
+    version="0.8.5",
     packages=find_packages(),
     install_requires=[
         "typer~=0.7.0",
         "requests~=2.28.2",
         "rich==13.3.1",
         "distro~=1.8.0",
     ],
```

### Comparing `shell_gpt-0.8.4/sgpt/app.py` & `shell_gpt-0.8.5/sgpt/app.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.4/sgpt/cache.py` & `shell_gpt-0.8.5/sgpt/cache.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.4/sgpt/client.py` & `shell_gpt-0.8.5/sgpt/client.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.4/sgpt/config.py` & `shell_gpt-0.8.5/sgpt/config.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.4/sgpt/handlers/chat_handler.py` & `shell_gpt-0.8.5/sgpt/handlers/chat_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.4/sgpt/handlers/default_handler.py` & `shell_gpt-0.8.5/sgpt/handlers/default_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.4/sgpt/handlers/handler.py` & `shell_gpt-0.8.5/sgpt/handlers/handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.4/sgpt/handlers/repl_handler.py` & `shell_gpt-0.8.5/sgpt/handlers/repl_handler.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.4/sgpt/make_prompt.py` & `shell_gpt-0.8.5/sgpt/make_prompt.py`

 * *Files identical despite different names*

### Comparing `shell_gpt-0.8.4/sgpt/utils.py` & `shell_gpt-0.8.5/sgpt/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import os
 import shlex
-import subprocess
 
 from enum import Enum
 from tempfile import NamedTemporaryFile
 
 import platform
-import typer
 
 from click import BadParameter
 
 
 class CompletionModes(Enum):
     NORMAL = "normal"
     SHELL = "shell"
@@ -52,32 +50,16 @@
     Runs a command in the user's shell.
     It is aware of the current user's $SHELL.
     :param command: A shell command to run.
     """
     if platform.system() == "Windows":
         is_powershell = len(os.getenv("PSModulePath", "").split(os.pathsep)) >= 3
         full_command = (
-            ["powershell.exe", "-Command", command]
+            f'powershell.exe -Command "{command}"'
             if is_powershell
-            else ["cmd.exe", "/c", command]
-        )
-        result = subprocess.run(
-            full_command,
-            shell=True,
-            text=True,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            check=False,
+            else f'cmd.exe /c "{command}"'
         )
     else:
         shell = os.environ.get("SHELL", "/bin/sh")
         full_command = f"{shell} -c {shlex.quote(command)}"
-        result = subprocess.run(
-            full_command,
-            shell=True,
-            text=True,
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            check=False,
-        )
-    output = result.stdout or result.stderr
-    typer.echo(output.strip())
+
+    os.system(full_command)
```

### Comparing `shell_gpt-0.8.4/shell_gpt.egg-info/PKG-INFO` & `shell_gpt-0.8.5/shell_gpt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shell-gpt
-Version: 0.8.4
+Version: 0.8.5
 Summary: A command-line productivity tool powered by ChatGPT, will help you accomplish your tasks faster and more efficiently.
 Home-page: https://github.com/ther1d/shell_gpt
 Author: Farkhod Sadykov
 Author-email: farkhod@sadykov.dev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -13,15 +13,15 @@
 
 <div align="center">
     <img src="https://i.ibb.co/nzPqnVd/sgpt-v0-8.gif" width="800"/>
 </div>
 
 ## Installation
 ```shell
-pip install shell-gpt==0.8.4
+pip install shell-gpt==0.8.5
 ```
 You'll need an OpenAI API key, you can generate one [here](https://beta.openai.com/account/api-keys).
 
 If the`$OPENAI_API_KEY` environment variable is set it will be used, otherwise, you will be prompted for your key which will then be stored in `~/.config/shell_gpt/.sgptrc`.
 
 ## Usage
 `sgpt` has a variety of use cases, including simple queries, shell queries, and code queries.
```

