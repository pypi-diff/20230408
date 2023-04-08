# Comparing `tmp/dockyard_cli-0.1.8.tar.gz` & `tmp/dockyard_cli-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dockyard_cli-0.1.8.tar", max compression
+gzip compressed data, was "dockyard_cli-0.1.9.tar", max compression
```

## Comparing `dockyard_cli-0.1.8.tar` & `dockyard_cli-0.1.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      904 2023-01-23 21:31:52.389272 dockyard_cli-0.1.8/README.md
--rw-r--r--   0        0        0       22 2023-01-11 15:37:26.393803 dockyard_cli-0.1.8/dockyard_cli/__init__.py
--rw-r--r--   0        0        0     1116 2023-01-11 15:37:26.393866 dockyard_cli-0.1.8/dockyard_cli/login.py
--rw-r--r--   0        0        0     9941 2023-01-23 21:30:07.061575 dockyard_cli-0.1.8/dockyard_cli/main.py
--rw-r--r--   0        0        0      307 2023-01-11 15:37:26.394029 dockyard_cli-0.1.8/dockyard_cli/utils.py
--rw-r--r--   0        0        0     1732 2023-01-11 15:37:26.394096 dockyard_cli-0.1.8/dockyard_cli/workspace.py
--rw-r--r--   0        0        0      496 2023-01-23 21:31:26.762122 dockyard_cli-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 dockyard_cli-0.1.8/setup.py
--rw-r--r--   0        0        0     1567 1970-01-01 00:00:00.000000 dockyard_cli-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      904 2023-01-23 21:31:52.389272 dockyard_cli-0.1.9/README.md
+-rw-r--r--   0        0        0       22 2023-01-11 15:37:26.393803 dockyard_cli-0.1.9/dockyard_cli/__init__.py
+-rw-r--r--   0        0        0     1116 2023-01-11 15:37:26.393866 dockyard_cli-0.1.9/dockyard_cli/login.py
+-rw-r--r--   0        0        0     9957 2023-01-23 21:45:46.745148 dockyard_cli-0.1.9/dockyard_cli/main.py
+-rw-r--r--   0        0        0      307 2023-01-11 15:37:26.394029 dockyard_cli-0.1.9/dockyard_cli/utils.py
+-rw-r--r--   0        0        0     1732 2023-01-11 15:37:26.394096 dockyard_cli-0.1.9/dockyard_cli/workspace.py
+-rw-r--r--   0        0        0      496 2023-01-23 21:46:15.776502 dockyard_cli-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 dockyard_cli-0.1.9/setup.py
+-rw-r--r--   0        0        0     1567 1970-01-01 00:00:00.000000 dockyard_cli-0.1.9/PKG-INFO
```

### Comparing `dockyard_cli-0.1.8/README.md` & `dockyard_cli-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dockyard_cli-0.1.8/dockyard_cli/login.py` & `dockyard_cli-0.1.9/dockyard_cli/login.py`

 * *Files identical despite different names*

### Comparing `dockyard_cli-0.1.8/dockyard_cli/main.py` & `dockyard_cli-0.1.9/dockyard_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,17 @@
         click.echo(r.text)
         raise click.Abort()
 
     resp = r.json()
     host = resp["ip"]
     port = resp["ports"]["ssh"]
     print(f"running ssh {user}@{host} -p {port} {' '.join(command)}")
-    os.execlp("ssh","ssh", f"{user}@{host}", "-p", str(port), ' '.join(command))
+    a = ["ssh", f"{user}@{host}", "-p", str(port)]
+    a.extend(command)
+    os.execvp("ssh", a)
 
 
 @main.command()
 @click.argument("workspace_name", envvar="DOCKYARD_WORKSPACE", shell_complete=get_workspaces)
 @catch_os_exec
 def code(workspace_name):
     """Start local VSCode and connect to dockyard workspace"""
```

### Comparing `dockyard_cli-0.1.8/dockyard_cli/workspace.py` & `dockyard_cli-0.1.9/dockyard_cli/workspace.py`

 * *Files identical despite different names*

### Comparing `dockyard_cli-0.1.8/setup.py` & `dockyard_cli-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'webdriver-setup>=1.1.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['dcli = dockyard_cli.main:main']}
 
 setup_kwargs = {
     'name': 'dockyard-cli',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'CLI for dockyard',
     'long_description': 'Usage\n======\n\n1. `dcli configure` - Configure dockyard CLI \n2. `dcli login` - Login to dockyard  \n3. `dcli list` - List dockyard workspaces\n4. `dcli activate` - Set active workspace. Subsequent commands use this workspace if no workspace name is specified.\n5. `dcli ssh [workspace name] [command]` - SSH to dockyard workspace\n6. `dcli scp <source> <target>` - Transfer files/directories to/from workspace.\n\n    a) source/target could be a local path (including .)\n\n    b) source/target could be a remote relative path inside workspace directory `<workspace_name>:<path>`\n\n    c) source/target could be a remote full path inside workspace `<workspace_name>:/<path>` or `<workspace_name>:~/<path>`\n\n7. `dcli code` - Start local VSCode and connect to dockyard workspace\n\n8. `dcli vnc` -  VNC connection to dockyard workspace\n\n9. `dcli start` - Start given workspace\n\n10. `dcli stop` - Stop given workspace\n\n',
     'author': 'rsingh',
     'author_email': 'rsingh@altoslabs.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `dockyard_cli-0.1.8/PKG-INFO` & `dockyard_cli-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dockyard-cli
-Version: 0.1.8
+Version: 0.1.9
 Summary: CLI for dockyard
 Author: rsingh
 Author-email: rsingh@altoslabs.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

