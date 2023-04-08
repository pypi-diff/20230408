# Comparing `tmp/jaynes-0.9.3-py3-none-any.whl.zip` & `tmp/jaynes-0.9.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,30 @@
-Zip file size: 39933 bytes, number of entries: 28
+Zip file size: 40163 bytes, number of entries: 28
 -rw-r--r--  2.0 unx      138 b- defN 21-Dec-28 04:17 jaynes/__init__.py
 -rw-r--r--  2.0 unx     3197 b- defN 21-Dec-28 04:17 jaynes/client.py
 -rw-r--r--  2.0 unx       40 b- defN 21-Dec-28 04:17 jaynes/constants.py
 -rw-r--r--  2.0 unx      721 b- defN 21-Dec-28 04:17 jaynes/daemon.py
 -rw-r--r--  2.0 unx      376 b- defN 21-Dec-28 04:17 jaynes/entry.py
 -rw-r--r--  2.0 unx     5180 b- defN 22-Sep-10 18:42 jaynes/gce_utils.py
 -rw-r--r--  2.0 unx     2767 b- defN 21-Dec-28 21:38 jaynes/helpers.py
 -rw-r--r--  2.0 unx    10791 b- defN 22-Sep-10 18:42 jaynes/jaynes.py
--rw-r--r--  2.0 unx    24705 b- defN 22-Oct-19 04:14 jaynes/mounts.py
+-rw-r--r--  2.0 unx    24723 b- defN 23-Apr-03 02:01 jaynes/mounts.py
 -rw-r--r--  2.0 unx      664 b- defN 21-Dec-28 04:17 jaynes/param_codec.py
 -rw-r--r--  2.0 unx    20569 b- defN 23-Jan-22 04:50 jaynes/runners.py
 -rw-r--r--  2.0 unx     4290 b- defN 22-Sep-10 18:42 jaynes/server.py
--rw-r--r--  2.0 unx      770 b- defN 21-Dec-28 21:20 jaynes/shell.py
+-rw-r--r--  2.0 unx     1617 b- defN 23-Apr-08 16:31 jaynes/shell.py
 -rw-r--r--  2.0 unx     5387 b- defN 21-Dec-28 04:17 jaynes/templates.py
 -rw-r--r--  2.0 unx      211 b- defN 22-May-10 04:01 jaynes/launchers/__init__.py
 -rw-r--r--  2.0 unx     5203 b- defN 22-Jan-23 06:15 jaynes/launchers/base_launcher.py
 -rw-r--r--  2.0 unx     3735 b- defN 22-Jan-12 15:01 jaynes/launchers/ec2_launch.py
 -rw-r--r--  2.0 unx     6997 b- defN 22-Jan-21 18:58 jaynes/launchers/gcp_launch.py
 -rw-r--r--  2.0 unx     2024 b- defN 22-Jun-17 15:54 jaynes/launchers/kube_launch.py
 -rw-r--r--  2.0 unx     1387 b- defN 21-Dec-28 21:46 jaynes/launchers/local_launcher.py
 -rw-r--r--  2.0 unx     2104 b- defN 22-Jan-12 15:03 jaynes/launchers/manager_launch.py
 -rw-r--r--  2.0 unx     4939 b- defN 21-Dec-28 22:16 jaynes/launchers/ssh_launch.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Dec-28 04:17 jaynes/stale/__init__.py
--rw-r--r--  2.0 unx     1047 b- defN 23-Jan-22 04:52 jaynes-0.9.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     8348 b- defN 23-Jan-22 04:52 jaynes-0.9.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-22 04:52 jaynes-0.9.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Jan-22 04:52 jaynes-0.9.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2197 b- defN 23-Jan-22 04:52 jaynes-0.9.3.dist-info/RECORD
-28 files, 117886 bytes uncompressed, 36447 bytes compressed:  69.1%
+-rw-r--r--  2.0 unx     1047 b- defN 23-Apr-08 16:32 jaynes-0.9.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8348 b- defN 23-Apr-08 16:32 jaynes-0.9.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 16:32 jaynes-0.9.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Apr-08 16:32 jaynes-0.9.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2198 b- defN 23-Apr-08 16:32 jaynes-0.9.5.dist-info/RECORD
+28 files, 118752 bytes uncompressed, 36677 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -63,23 +63,23 @@
 
 Filename: jaynes/launchers/ssh_launch.py
 Comment: 
 
 Filename: jaynes/stale/__init__.py
 Comment: 
 
-Filename: jaynes-0.9.3.dist-info/LICENSE
+Filename: jaynes-0.9.5.dist-info/LICENSE
 Comment: 
 
-Filename: jaynes-0.9.3.dist-info/METADATA
+Filename: jaynes-0.9.5.dist-info/METADATA
 Comment: 
 
-Filename: jaynes-0.9.3.dist-info/WHEEL
+Filename: jaynes-0.9.5.dist-info/WHEEL
 Comment: 
 
-Filename: jaynes-0.9.3.dist-info/top_level.txt
+Filename: jaynes-0.9.5.dist-info/top_level.txt
 Comment: 
 
-Filename: jaynes-0.9.3.dist-info/RECORD
+Filename: jaynes-0.9.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jaynes/mounts.py

```diff
@@ -25,17 +25,17 @@
 
     :param host_path: path on the host
     :param container_path: path inside the container
     :param docker_mount_type: "bind" the mount type, one of "bind," "volume," or "tmpfs."
     :param pypath: boolean flag for whether this mount point should be included in the PYPATH environment variable
     """
 
-    def __init__(self, host_path, container_path, docker_mount_type="bind", pypath=False):
+    def __init__(self, host_path, container_path=None, docker_mount_type="bind", pypath=False):
         self.host_path = host_path
-        self.container_path = container_path
+        self.container_path = container_path or host_path
         self.pypath = pypath
         self.docker_mount = f"--mount type={docker_mount_type},source={host_path},target={container_path}"
 
 
 class S3Code(Mount):
     """
     Tars a local folder, uploads the content to S3, downloads the tar ball on the remote instance and mounts it
```

## jaynes/shell.py

```diff
@@ -4,14 +4,25 @@
 def popen(cmd, *args, verbose=False, **kwargs):
     if verbose:
         print(cmd, *args)
     return subprocess.Popen(cmd, *args, **kwargs)
 
 
 def call(cmd, *args, verbose=False, **kwargs):
+    """Run a command and return the exit code.
+    
+    Pipe the output to stdout and stderr.
+    Args:
+        cmd: The command to run.
+        *args: Additional arguments to pass to subprocess.Popen.
+        verbose: If True, print the command before running it.
+        **kwargs: Additional keyword arguments to pass to subprocess.Popen.
+
+    :return: The exit code of the command.
+    """
     if verbose:
         print(cmd, *args)
     return subprocess.call(cmd, *args, **kwargs)
 
 
 def check_call(cmd, *args, verbose=False, **kwargs) -> object:
     if verbose:
@@ -19,11 +30,25 @@
     try:
         return subprocess.check_call(cmd, *args, **kwargs)
     except subprocess.CalledProcessError as e:
         print(e)
 
 
 def run(cmd, *args, verbose=False, **kwargs) -> [str, str]:
+    """Run a command and return the output and error as strings.
+
+    Example:
+        >>> run(["echo", "hey"])
+        ('hey', '')
+
+    Args:
+        cmd: The command to run.
+        *args: Additional arguments to pass to subprocess.Popen.
+        verbose: If True, print the command before running it.
+        **kwargs: Additional keyword arguments to pass to subprocess.Popen.
+
+    :return: A tuple containing the output and error as strings.
+    """
     if verbose:
         print(cmd, *args)
     process = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, **kwargs)
     return process.communicate()
```

## Comparing `jaynes-0.9.3.dist-info/LICENSE` & `jaynes-0.9.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jaynes-0.9.3.dist-info/METADATA` & `jaynes-0.9.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaynes
-Version: 0.9.3
+Version: 0.9.5
 Summary: A tool for running python code with runner on aws
 Home-page: https://github.com/episodeyang/jaynes
 Author: Ge Yang
 Author-email: yangge1987@gmail.com
 License: Copyright 2022 Ge Yang        
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:        
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

## Comparing `jaynes-0.9.3.dist-info/RECORD` & `jaynes-0.9.5.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 jaynes/client.py,sha256=phuxy9aGNB2UfUpmtafUz_ielK4U0yWPb7K-dEZsU0Q,3197
 jaynes/constants.py,sha256=FI2l_bI8Zs2ftEB6l5BrG6ly3jhInTlkiYhKam0x_BM,40
 jaynes/daemon.py,sha256=57WWnRYqRnjEmg0K5bdUnt1LDIN2gCrgCZ_agzlkeVg,721
 jaynes/entry.py,sha256=GpK811zV6vMeOVpkhkAnPCBhguTJNc0dnuhDegoQwpo,376
 jaynes/gce_utils.py,sha256=dLdZwPKl123TXZm1rMLfWlEHoefwCJ24-TfuJBPT32g,5180
 jaynes/helpers.py,sha256=K6wxDgXBhvMCCrfgap_nmQF1CEyDByfbVmX9kZNMPuw,2767
 jaynes/jaynes.py,sha256=YNoVh-BfqeWZBvQrXYTHw7bFbDS6_MC75IhQ9eBXw-E,10791
-jaynes/mounts.py,sha256=36-Qs4IymFuNLw2bnEfXjma7FNoL9kIDIBieSYl1PO4,24705
+jaynes/mounts.py,sha256=nwptQ8o0Q-oFEAT7kjoVT1dufn4HY15A2gqgxfRY41Y,24723
 jaynes/param_codec.py,sha256=eBG532ixzzcibOx95S98CVy6fZQKUvRXHG45wxsE0vw,664
 jaynes/runners.py,sha256=OJnlV3Nx5587m4wnECnJzhB8DUWjXdWL699Yhr5tDuI,20569
 jaynes/server.py,sha256=k3ZoZcuOpMs6xhR-bA5H2BRv-r-RTNd-uMOWQEGb8co,4290
-jaynes/shell.py,sha256=6VojNKuBq5uSMJc9ym5cTKJ6GLVjqoR6bQYjXh2jTNU,770
+jaynes/shell.py,sha256=bU-8biTC09SH4Fn1NFonwKZnCiZhEX-KhePbCW-gwVE,1617
 jaynes/templates.py,sha256=Tb8b_z3p82nl-fBoF-3qvVsWy7TEpXDTh7Qod3e469U,5387
 jaynes/launchers/__init__.py,sha256=VuDftYyG8ue7f8-L9XmDjkizVpomKMat5bonVPmQaxE,211
 jaynes/launchers/base_launcher.py,sha256=XHaMzLMPQAkCsZIDWIqJnjrwsnWdOWaqxJffSXW4Kak,5203
 jaynes/launchers/ec2_launch.py,sha256=kaoDp6SywgkcJYm0uZJTV3UUePXrWxzY3dLzi6m_D1I,3735
 jaynes/launchers/gcp_launch.py,sha256=2tgIkweroSiC9U4LebWqfAkukMSCJe7FnxY69m6EQ-k,6997
 jaynes/launchers/kube_launch.py,sha256=Bvt_cGblAvxWfkglo-TIsKwH8bIt2fuep4OvYgB9Zes,2024
 jaynes/launchers/local_launcher.py,sha256=xO0IHWF2ivfjT41tra5-6QPKB6bXkkwW5QD81w2ZRow,1387
 jaynes/launchers/manager_launch.py,sha256=krq6adiHee1DI2iWbahZM9tZkhCHUQBxtS3NYy76QkY,2104
 jaynes/launchers/ssh_launch.py,sha256=GzAIotYD3rWZcz-CzSLMTflZJyuygiaQEw88gPa36ac,4939
 jaynes/stale/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-jaynes-0.9.3.dist-info/LICENSE,sha256=7aeBUFBrKApC7DJHqrnGsPuy6pvZegzaTT-iJERVSW0,1047
-jaynes-0.9.3.dist-info/METADATA,sha256=dneX9MwXDkH9SnsYZrhRlt1dbKMyrHIKPg45p6wi1Lk,8348
-jaynes-0.9.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-jaynes-0.9.3.dist-info/top_level.txt,sha256=BqdlhoNVrrByJ8bJYMoZAavY4mca0lxO15ad4EGWqhY,7
-jaynes-0.9.3.dist-info/RECORD,,
+jaynes-0.9.5.dist-info/LICENSE,sha256=7aeBUFBrKApC7DJHqrnGsPuy6pvZegzaTT-iJERVSW0,1047
+jaynes-0.9.5.dist-info/METADATA,sha256=1E0dY1gEzGcWrNxMVkfb4v7KZnYJ8Nl8ZjvbhYCKYy4,8348
+jaynes-0.9.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+jaynes-0.9.5.dist-info/top_level.txt,sha256=BqdlhoNVrrByJ8bJYMoZAavY4mca0lxO15ad4EGWqhY,7
+jaynes-0.9.5.dist-info/RECORD,,
```

