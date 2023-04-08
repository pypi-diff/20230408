# Comparing `tmp/flojoy-0.2.2.dev2.tar.gz` & `tmp/flojoy-0.2.2.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flojoy-0.2.2.dev2.tar", last modified: Tue Apr  4 17:09:52 2023, max compression
+gzip compressed data, was "flojoy-0.2.2.dev3.tar", last modified: Sat Apr  8 18:31:58 2023, max compression
```

## Comparing `flojoy-0.2.2.dev2.tar` & `flojoy-0.2.2.dev3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-04 17:09:52.352512 flojoy-0.2.2.dev2/
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1062 2022-10-05 16:22:32.000000 flojoy-0.2.2.dev2/LICENSE.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-04 17:09:52.352512 flojoy-0.2.2.dev2/PKG-INFO
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       31 2022-10-05 16:21:51.000000 flojoy-0.2.2.dev2/README.md
-drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-04 17:09:52.340512 flojoy-0.2.2.dev2/flojoy/
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      188 2023-04-03 20:53:50.000000 flojoy-0.2.2.dev2/flojoy/__init__.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      209 2023-04-04 16:27:03.000000 flojoy-0.2.2.dev2/flojoy/flojoy_instruction.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)    18898 2023-04-04 16:27:14.000000 flojoy-0.2.2.dev2/flojoy/flojoy_python.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     2629 2023-04-04 17:08:12.000000 flojoy-0.2.2.dev2/flojoy/job_result_builder.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1774 2023-04-04 17:08:40.000000 flojoy-0.2.2.dev2/flojoy/job_result_utils.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     2114 2023-04-04 17:08:55.000000 flojoy-0.2.2.dev2/flojoy/plotly_utils.py
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     6070 2023-02-20 19:12:45.000000 flojoy-0.2.2.dev2/flojoy/utils.py
-drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-04 17:09:52.352512 flojoy-0.2.2.dev2/flojoy.egg-info/
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-04 17:09:52.000000 flojoy-0.2.2.dev2/flojoy.egg-info/PKG-INFO
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      356 2023-04-04 17:09:52.000000 flojoy-0.2.2.dev2/flojoy.egg-info/SOURCES.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        1 2023-04-04 17:09:52.000000 flojoy-0.2.2.dev2/flojoy.egg-info/dependency_links.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       76 2023-04-04 17:09:52.000000 flojoy-0.2.2.dev2/flojoy.egg-info/requires.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        7 2023-04-04 17:09:52.000000 flojoy-0.2.2.dev2/flojoy.egg-info/top_level.txt
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       79 2023-04-04 17:09:52.352512 flojoy-0.2.2.dev2/setup.cfg
--rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      956 2023-04-04 17:09:40.000000 flojoy-0.2.2.dev2/setup.py
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-08 18:31:58.583559 flojoy-0.2.2.dev3/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1062 2022-10-05 16:22:32.000000 flojoy-0.2.2.dev3/LICENSE.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-08 18:31:58.583559 flojoy-0.2.2.dev3/PKG-INFO
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       31 2022-10-05 16:21:51.000000 flojoy-0.2.2.dev3/README.md
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-08 18:31:58.579559 flojoy-0.2.2.dev3/flojoy/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      188 2023-04-03 20:53:50.000000 flojoy-0.2.2.dev3/flojoy/__init__.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      209 2023-04-04 16:27:03.000000 flojoy-0.2.2.dev3/flojoy/flojoy_instruction.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)    18958 2023-04-08 18:30:05.000000 flojoy-0.2.2.dev3/flojoy/flojoy_python.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     2629 2023-04-04 17:08:12.000000 flojoy-0.2.2.dev3/flojoy/job_result_builder.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     1774 2023-04-04 17:08:40.000000 flojoy-0.2.2.dev3/flojoy/job_result_utils.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     2114 2023-04-04 17:08:55.000000 flojoy-0.2.2.dev3/flojoy/plotly_utils.py
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)     6070 2023-02-20 19:12:45.000000 flojoy-0.2.2.dev3/flojoy/utils.py
+drwxrwxr-x   0 smahmed   (1000) smahmed   (1000)        0 2023-04-08 18:31:58.583559 flojoy-0.2.2.dev3/flojoy.egg-info/
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      676 2023-04-08 18:31:58.000000 flojoy-0.2.2.dev3/flojoy.egg-info/PKG-INFO
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      356 2023-04-08 18:31:58.000000 flojoy-0.2.2.dev3/flojoy.egg-info/SOURCES.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        1 2023-04-08 18:31:58.000000 flojoy-0.2.2.dev3/flojoy.egg-info/dependency_links.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       76 2023-04-08 18:31:58.000000 flojoy-0.2.2.dev3/flojoy.egg-info/requires.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)        7 2023-04-08 18:31:58.000000 flojoy-0.2.2.dev3/flojoy.egg-info/top_level.txt
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)       79 2023-04-08 18:31:58.583559 flojoy-0.2.2.dev3/setup.cfg
+-rw-rw-r--   0 smahmed   (1000) smahmed   (1000)      956 2023-04-08 18:31:00.000000 flojoy-0.2.2.dev3/setup.py
```

### Comparing `flojoy-0.2.2.dev2/LICENSE.txt` & `flojoy-0.2.2.dev3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flojoy-0.2.2.dev2/PKG-INFO` & `flojoy-0.2.2.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flojoy
-Version: 0.2.2.dev2
+Version: 0.2.2.dev3
 Summary: Python client library for Flojoy.
 Home-page: https://github.com/flojoy-io/flojoy-python
 Author: flojoy
 Author-email: jack.parmer@proton.me
 License: MIT
 Download-URL: https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip
 Keywords: data-acquisition,lab-automation,low-code,python,scheduler,topic
```

### Comparing `flojoy-0.2.2.dev2/flojoy/flojoy_python.py` & `flojoy-0.2.2.dev3/flojoy/flojoy_python.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,18 +432,19 @@
                     'RUNNING_NODE': '',
                     'jobsetId': jobset_id
                 }))
 
             print('final result:', dump_str(data['output'], limit=100))
 
             return data['output']
-        except:
+        except Exception as e:
             send_to_socket(json.dumps({
-                'SYSTEM_STATUS': 'Failed to run: ' + func.__name__,
+                'SYSTEM_STATUS': f'Failed to run: {func.__name__}',
                 'FAILED_NODES': node_id,
+                'FAILURE_REASON': e.args[0],
                 'jobsetId': jobset_id
             }))
             print('error occured while running the node')
             print(traceback.format_exc())
             raise
 
     wrapper.original = func
```

### Comparing `flojoy-0.2.2.dev2/flojoy/job_result_builder.py` & `flojoy-0.2.2.dev3/flojoy/job_result_builder.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.2.2.dev2/flojoy/job_result_utils.py` & `flojoy-0.2.2.dev3/flojoy/job_result_utils.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.2.2.dev2/flojoy/plotly_utils.py` & `flojoy-0.2.2.dev3/flojoy/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.2.2.dev2/flojoy/utils.py` & `flojoy-0.2.2.dev3/flojoy/utils.py`

 * *Files identical despite different names*

### Comparing `flojoy-0.2.2.dev2/flojoy.egg-info/PKG-INFO` & `flojoy-0.2.2.dev3/flojoy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flojoy
-Version: 0.2.2.dev2
+Version: 0.2.2.dev3
 Summary: Python client library for Flojoy.
 Home-page: https://github.com/flojoy-io/flojoy-python
 Author: flojoy
 Author-email: jack.parmer@proton.me
 License: MIT
 Download-URL: https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip
 Keywords: data-acquisition,lab-automation,low-code,python,scheduler,topic
```

### Comparing `flojoy-0.2.2.dev2/setup.py` & `flojoy-0.2.2.dev3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 setup(
     name='flojoy',
     packages=['flojoy'],
-    version='0.2.2.dev2',
+    version='0.2.2.dev3',
     license='MIT',
     description='Python client library for Flojoy.',
     author='flojoy',
     author_email='jack.parmer@proton.me',
     url='https://github.com/flojoy-io/flojoy-python',
     download_url='https://github.com/flojoy-io/flojoy-python/archive/refs/heads/main.zip',
     keywords=['data-acquisition', 'lab-automation', 'low-code', 'python', 'scheduler', 'topic'],
```

