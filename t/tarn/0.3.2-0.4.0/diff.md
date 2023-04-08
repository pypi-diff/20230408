# Comparing `tmp/tarn-0.3.2.tar.gz` & `tmp/tarn-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tarn-0.3.2.tar", last modified: Tue Feb  7 08:18:25 2023, max compression
+gzip compressed data, was "tarn-0.4.0.tar", last modified: Sat Apr  8 16:41:43 2023, max compression
```

## Comparing `tarn-0.3.2.tar` & `tarn-0.4.0.tar`

### file list

```diff
@@ -1,46 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 08:18:25.245335 tarn-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-02-07 08:18:22.000000 tarn-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-07 08:18:22.000000 tarn-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-02-07 08:18:25.241335 tarn-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-02-07 08:18:22.000000 tarn-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-02-07 08:18:22.000000 tarn-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-07 08:18:22.000000 tarn-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 08:18:25.245335 tarn-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-02-07 08:18:22.000000 tarn-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 08:18:25.241335 tarn-0.3.2/tarn/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 08:18:25.241335 tarn-0.3.2/tarn/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/cache/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/cache/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/cache/pickler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/cache/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/cache/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/digest.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 08:18:25.241335 tarn-0.3.2/tarn/local/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/local/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/local/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/local/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 08:18:25.241335 tarn-0.3.2/tarn/remote/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/remote/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/remote/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 08:18:25.241335 tarn-0.3.2/tarn/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/tools/locker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/tools/size.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/tools/usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-02-07 08:18:22.000000 tarn-0.3.2/tarn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 08:18:25.241335 tarn-0.3.2/tarn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-02-07 08:18:25.000000 tarn-0.3.2/tarn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-02-07 08:18:25.000000 tarn-0.3.2/tarn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 08:18:25.000000 tarn-0.3.2/tarn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-07 08:18:25.000000 tarn-0.3.2/tarn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-07 08:18:25.000000 tarn-0.3.2/tarn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-04-08 16:41:38.000000 tarn-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-08 16:41:38.000000 tarn-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-08 16:41:43.769901 tarn-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-08 16:41:38.000000 tarn-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-08 16:41:38.000000 tarn-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-08 16:41:38.000000 tarn-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 16:41:43.773902 tarn-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-04-08 16:41:38.000000 tarn-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/cache/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/cache/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/cache/pickler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/cache/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/cache/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/local/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/local/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/location/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/location/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/location/disk_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/location/fanout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/location/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/location/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/location/nginx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/location/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/pickler/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/pickler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/pickler/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/pickler/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/pool/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/pool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/pool/hash_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/pool/pickle_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/remote/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/remote/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/tools/locker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/tools/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/tools/usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-08 16:41:38.000000 tarn-0.4.0/tarn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 16:41:43.769901 tarn-0.4.0/tarn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-08 16:41:43.000000 tarn-0.4.0/tarn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-08 16:41:43.000000 tarn-0.4.0/tarn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 16:41:43.000000 tarn-0.4.0/tarn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-08 16:41:43.000000 tarn-0.4.0/tarn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-08 16:41:43.000000 tarn-0.4.0/tarn.egg-info/top_level.txt
```

### Comparing `tarn-0.3.2/LICENSE` & `tarn-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tarn-0.3.2/PKG-INFO` & `tarn-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.3.2
+Version: 0.4.0
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.3.2.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.4.0.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.3.2/README.md` & `tarn-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tarn-0.3.2/pyproject.toml` & `tarn-0.4.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,51 +1,41 @@
-[project]
-name = "tarn"
-dynamic = ["version"]
-description = "A hashmap-based storage on local and remote disks"
-readme = "README.md"
-requires-python = ">=3.6"
-license = { file = "LICENSE" }
-keywords = ["storage", "cache", "invalidation"]
-authors = [
-    { name = "Max", email = "maxs987@gmail.com" }
-]
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Programming Language :: Python :: 3 :: Only",
-]
-dependencies = [
-    "numpy",
-    "cloudpickle>=2.0.0,<2.3.0",
-    "paramiko==2.*",
-    "scp",
-    "tqdm",
-    "redis",
-    "pyyaml",
-    "humanfriendly",
-    "pydantic",
-    "requests",
-]
+import runpy
+from pathlib import Path
 
-[project.urls]
-"Homepage" = "https://github.com/neuro-ml/tarn"
-"Issues" = "https://github.com/neuro-ml/tarn/issues"
-"Source" = "https://github.com/neuro-ml/tarn"
-"Docs" = "https://neuro-ml.github.io/tarn"
+from setuptools import setup, find_packages
 
-[build-system]
-requires = ["setuptools>=43.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
+classifiers = [
+    'Development Status :: 3 - Alpha',
+    'License :: OSI Approved :: Apache Software License',
+    'Programming Language :: Python :: 3',
+    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
+    'Programming Language :: Python :: 3 :: Only',
+]
 
-[tool.setuptools.packages.find]
-include = ["tarn"]
+name = 'tarn'
+root = Path(__file__).resolve().parent
+with open(root / 'requirements.txt', encoding='utf-8') as file:
+    requirements = file.read().splitlines()
+with open(root / 'README.md', encoding='utf-8') as file:
+    long_description = file.read()
+version = runpy.run_path(root / name / '__version__.py')['__version__']
 
-[tool.setuptools.dynamic]
-version = { attr = "tarn.__version__.__version__" }
+setup(
+    name=name,
+    packages=find_packages(include=(name,)),
+    include_package_data=True,
+    version=version,
+    description='A hashmap-based storage on local and remote disks',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/neuro-ml/tarn',
+    download_url='https://github.com/neuro-ml/tarn/archive/v%s.tar.gz' % version,
+    keywords=['storage', 'cache', 'invalidation'],
+    classifiers=classifiers,
+    install_requires=requirements,
+    python_requires='>=3.6',
+)
```

### Comparing `tarn-0.3.2/tarn/cache/compat.py` & `tarn-0.4.0/tarn/pickler/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,23 @@
 LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 import importlib
 import sys
 import warnings
-from weakref import WeakSet
 from collections import ChainMap
 from enum import Enum
 from pickle import _Pickler as Pickler
 from types import ModuleType
-from typing import Union, Set, TypeVar
+from typing import Set, TypeVar, Union
+from weakref import WeakSet
 
 from cloudpickle import CloudPickler
-from cloudpickle.cloudpickle import _whichmodule, _extract_code_globals, _get_cell_contents, _lookup_module_and_qualname
+from cloudpickle.cloudpickle import _extract_code_globals, _get_cell_contents, _lookup_module_and_qualname, _whichmodule
 
 try:
     from gzip import BadGzipFile
 except ImportError:
     BadGzipFile = OSError
 
 
@@ -69,15 +69,15 @@
     module, _ = pair
     module = module.__name__
 
     while True:
         if module in UNSTABLE_MODULES:
             return PickleMode.Deep
 
-        split = module.rsplit(".", 1)
+        split = module.rsplit('.', 1)
         if len(split) == 1:
             break
         module, _ = split
 
     _check_is_under_development(obj, name)
     return PickleMode.Global
```

### Comparing `tarn-0.3.2/tarn/cache/index.py` & `tarn-0.4.0/tarn/location/disk_dict.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,160 @@
-import gzip
 import logging
 import os
 import shutil
-import tempfile
-import warnings
-from itertools import chain
+from contextlib import contextmanager
 from pathlib import Path
-from typing import Any
+from typing import ContextManager, Iterable, Optional, Tuple
 
-from ..compat import rmtree, copy_file
+from ..compat import copy_file, remove_file, rmtree
+from ..config import load_config, root_params
 from ..digest import key_to_relative
-from ..local import Storage, DiskBase
-from ..interface import Key
-from ..utils import create_folders, to_read_only, match_files, adjust_permissions
-from ..exceptions import StorageCorruption, ReadError
-from .serializers import Serializer, SerializerError
-from .compat import BadGzipFile
+from ..exceptions import StorageCorruption
+from ..interface import Key, Keys, MaybeValue, PathOrStr, Value
+from ..tools import Locker, SizeTracker, UsageTracker
+from ..utils import adjust_permissions, create_folders, get_size, match_buffers, match_files
+from .interface import Writable
 
 logger = logging.getLogger(__name__)
+MaybePath = Optional[Path]
 
-DATA_FOLDER = 'data'
-HASH_FILENAME = 'hash.bin'
-GZIP_COMPRESSION = 1
-
-
-class CacheIndex(DiskBase):
-    def __init__(self, root: Path, storage: Storage, serializer: Serializer):
-        super().__init__(root)
-        self.storage = storage
-        self.serializer = serializer
-
-    def _check_value_consistency(self, base: Path, key: Key, value: Any, context):
-        check_consistency(base / HASH_FILENAME, context, check_existence=True)
-
-    def _check_folder_consistency(self, base: Path, key: Key, folder: Path, context):
-        match_files(base / HASH_FILENAME, folder / HASH_FILENAME)
-
-    def _write(self, base: Path, key: Key, value: Any, context: Any):
-        with tempfile.TemporaryDirectory() as temp_folder:
-            data_folder, temp_folder = base / DATA_FOLDER, Path(temp_folder)
-            create_folders(data_folder, self.permissions, self.group)
-
-            self.serializer.save(value, temp_folder)
-            self._mirror_to_storage(temp_folder, data_folder)
-            self._save_meta(base, context)
-
-    def _replicate(self, base: Path, key: Key, source: Path, context):
-        # data
-        destination = base / DATA_FOLDER
-        shutil.copytree(source / DATA_FOLDER, destination)
-        for dst in chain([destination], destination.rglob('*')):
-            adjust_permissions(dst, self.permissions, self.group, read_only=not dst.is_dir())
-
-        # meta
-        copy_file(source / HASH_FILENAME, base / HASH_FILENAME)
-        to_read_only(base / HASH_FILENAME, self.permissions, self.group)
 
-    def _read(self, key, context):
-        def load(base):
+class DiskDict(Writable):
+    def __init__(self, root: PathOrStr):
+        root = Path(root)
+        config = load_config(root)
+        self.levels = config.levels
+        self.hash = config.hash.build()
+        assert self.hash().digest_size == sum(self.levels)
+
+        self.root = root
+        self.permissions, self.group = root_params(self.root)
+        usage_folder = self.root / 'tools/usage'
+        create_folders(usage_folder, self.permissions, self.group)
+
+        self.locker: Locker = config.make_locker()
+        self.size_tracker: SizeTracker = config.make_size()
+        self.usage_tracker: UsageTracker = config.make_usage(usage_folder)
+        self.min_free_size = config.free_disk_size
+        self.max_size = config.max_size
+
+    @property
+    def key_size(self):
+        return sum(self.levels)
+
+    @contextmanager
+    def read(self, key: Key) -> ContextManager[MaybePath]:
+        file = self._key_to_path(key)
+        corrupted = False
+        with self.locker.read(key):
+            if file.exists():
+                # TODO: deprecated
+                if file.is_dir():
+                    file = file / 'data'
+
+                self.usage_tracker.update(key, file)
+                try:
+                    yield file
+                    return
+                except StorageCorruption:
+                    corrupted = True
+
+        if corrupted:
+            self.delete(key)
+            return
+
+        yield None
+
+    def read_batch(self, keys: Keys) -> Iterable[Tuple[Key, MaybeValue]]:
+        for key in keys:
+            with self.read(key) as value:
+                yield key, value
+
+    @contextmanager
+    def write(self, key: Key, value: Value) -> ContextManager[MaybePath]:
+        file = self._key_to_path(key)
+        with self.locker.write(key):
             try:
-                return self.serializer.load(base / DATA_FOLDER, self.storage)
-            except (SerializerError, ReadError):
-                raise
-            except Exception as e:
-                raise RuntimeError(f'An error occurred while loading the cache for "{key}" at {base}') from e
-
-        return self._read_entry(key, context, load)
-
-    def replicate_to(self, key, context, store):
-        self._read_entry(key, context, lambda base: store(key, base))
-
-    def _read_entry(self, key, context, reader):
-        base = self.root / key_to_relative(key, self.levels)
-        with self.locker.read(key, base):
-            if not base.exists():
-                logger.info('Key %s: path not found "%s"', key, base)
-                return None, False
-
-            hash_path = base / HASH_FILENAME
-            # we either have a valid folder
-            if hash_path.exists():
-                check_consistency(hash_path, context)
+                # if already stored
+                if file.exists():
+                    # TODO: legacy
+                    if file.is_dir():
+                        file = file / 'data'
+
+                    if _is_pathlike(value):
+                        match_files(value, file)
+                    else:
+                        with open(file, 'rb') as dst:
+                            match_buffers(value, dst, context=key.hex())
+
+                    yield file
+                    return
+
+                # make sure we can write
+                if not self._writeable():
+                    yield
+                    return
+
                 try:
-                    return reader(base), True
-                except ReadError as e:
-                    # couldn't find the hash - the cache is corrupted
-                    logger.info('Error while reading %s: %s: %s', key, type(e).__name__, e)
-
-        # or it is corrupted, in which case we can remove it
-        with self.locker.write(key, base):
-            self._cleanup_corrupted(base, key)
-            return None, False
-
-    # internal
-
-    def _save_meta(self, base, pickled):
-        hash_path = base / HASH_FILENAME
-        # hash
-        with gzip.GzipFile(hash_path, 'wb', compresslevel=GZIP_COMPRESSION, mtime=0) as file:
-            file.write(pickled)
-        to_read_only(hash_path, self.permissions, self.group)
-
-    def _mirror_to_storage(self, source: Path, destination: Path):
-        for file in source.glob('**/*'):
-            target = destination / file.relative_to(source)
-            if file.is_dir():
-                create_folders(target, self.permissions, self.group)
+                    # create base folders
+                    create_folders(file.parent, self.permissions, self.group)
+                    # populate the folder
+                    if _is_pathlike(value):
+                        copy_file(value, file)
+                    else:
+                        with open(file, 'wb') as dst:
+                            shutil.copyfileobj(value, dst)
+
+                    adjust_permissions(file, self.permissions, self.group, read_only=True)
+
+                except BaseException as e:
+                    if file.exists():
+                        remove_file(file)
+                    raise RuntimeError('An error occurred while copying the file') from e
+
+                # metadata
+                self.size_tracker.inc(get_size(file))
+                self.usage_tracker.update(key, file)
+
+                yield file
+
+            except StorageCorruption:
+                if file.exists():
+                    remove_file(file)
+
+    def delete(self, key: Key) -> bool:
+        file = self._key_to_path(key)
+        with self.locker.write(key):
+            if not file.exists():
+                return False
 
+            # TODO: don't need this if no tracker is used
+            if file.is_dir():
+                # TODO: legacy
+                size = get_size(file / 'data') if file.is_dir() else 0
+                rmtree(file)
             else:
-                with open(target, 'w') as fd:
-                    fd.write(self.storage.write(file))
-                os.remove(file)
-                to_read_only(target, self.permissions, self.group)
-
-    def _cleanup_corrupted(self, folder, digest):
-        message = f'Corrupted storage at {self.root} for key {digest}. Cleaning up.'
-        warnings.warn(message, RuntimeWarning)
-        logger.warning(message)
-        rmtree(folder)
-
-
-def check_consistency(hash_path, pickled, check_existence: bool = False):
-    suggestion = f'You may want to delete the {hash_path.parent} folder.'
-    if check_existence and not hash_path.exists():
-        raise StorageCorruption(f'The pickled graph is missing. {suggestion}')
-    try:
-        with gzip.GzipFile(hash_path, 'rb') as file:
-            dumped = file.read()
-            if dumped != pickled:
-                raise StorageCorruption(
-                    f'The dumped and current pickle do not match at {hash_path}: {dumped} {pickled}. {suggestion}'
-                )
-    except BadGzipFile:
-        raise StorageCorruption(f'The hash is corrupted. {suggestion}') from None
+                size = get_size(file)
+                remove_file(file)
+
+            self.size_tracker.dec(size)
+            self.usage_tracker.delete(key)
+
+            return True
+
+    def _key_to_path(self, key: Key):
+        return self.root / key_to_relative(key, self.levels)
+
+    def _writeable(self):
+        result = True
+
+        if self.min_free_size > 0:
+            result = result and shutil.disk_usage(self.root).free >= self.min_free_size
+
+        if self.max_size is not None and self.max_size < float('inf'):
+            result = result and self.size_tracker.get(self.root) <= self.max_size
+
+        return result
+
+
+def _is_pathlike(x):
+    return isinstance(x, (os.PathLike, str))
```

### Comparing `tarn-0.3.2/tarn/cache/pickler.py` & `tarn-0.4.0/tarn/pickler/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,26 @@
         as long as it helps to achieve (or doesn't impede) 1 and 2
 """
 import abc
 import itertools
 import pickle
 import pickletools
 import types
-from operator import itemgetter
-from typing import NamedTuple, Any
 from contextlib import suppress
 from enum import Enum
 from io import BytesIO
+from operator import itemgetter
+from typing import Any, NamedTuple
 
-from cloudpickle.cloudpickle import is_tornado_coroutine, PYPY, builtin_code_type, \
+from cloudpickle.cloudpickle import (
+    is_tornado_coroutine, PYPY, builtin_code_type,
     _rebuild_tornado_coroutine, _find_imported_submodules, _BUILTIN_TYPE_NAMES, _builtin_type, _extract_class_dict
+)
 
-from .compat import DISPATCH, extract_func_data, Pickler, get_pickle_mode, PickleMode
+from .compat import DISPATCH, PickleMode, Pickler, extract_func_data, get_pickle_mode
 
 
 def sort_dict(d):
     return tuple(sorted(d.items()))
 
 
 VERSION_METHOD = '__getversion__'
@@ -102,15 +104,15 @@
         if consts and isinstance(consts[0], str):
             consts = list(consts)[1:]
             # TODO: this is not enough, None might be referenced in the bytecode under a wrong index
             if None in consts:
                 consts.remove(None)
             consts = (None, *consts)
 
-        if hasattr(obj, "co_posonlyargcount"):
+        if hasattr(obj, 'co_posonlyargcount'):
             posonlyargcount = obj.co_posonlyargcount,
         else:
             posonlyargcount = ()
 
         args = (
             obj.co_argcount, *posonlyargcount,
             obj.co_kwonlyargcount, obj.co_nlocals, obj.co_stacksize,
@@ -173,21 +175,21 @@
     dispatch[types.FunctionType] = save_function
 
     @staticmethod
     def _get_cls_params(obj):
         clsdict = _extract_class_dict(obj)
         clsdict.pop('__weakref__', None)
 
-        if "_abc_impl" in clsdict:
+        if '_abc_impl' in clsdict:
             (registry, _, _, _) = abc._get_dump(obj)
-            clsdict["_abc_impl"] = [subclass_weakref() for subclass_weakref in registry]
+            clsdict['_abc_impl'] = [subclass_weakref() for subclass_weakref in registry]
 
         # originally here was the __doc__
         type_kwargs = {}
-        if hasattr(obj, "__slots__"):
+        if hasattr(obj, '__slots__'):
             type_kwargs['__slots__'] = obj.__slots__
             if isinstance(obj.__slots__, str):
                 clsdict.pop(obj.__slots__)
             else:
                 for k in obj.__slots__:
                     clsdict.pop(k, None)
 
@@ -207,16 +209,16 @@
         state = sort_dict(clsdict)
         return type, args, state
 
     def reduce_dynamic_enum(self, obj):
         clsdict, type_kwargs = self._get_cls_params(obj)
 
         members = {e.name: e.value for e in obj}
-        for attrname in ["_generate_next_value_", "_member_names_", "_member_map_", "_member_type_",
-                         "_value2member_map_"] + list(members):
+        for attrname in ['_generate_next_value_', '_member_names_', '_member_map_', '_member_type_',
+                         '_value2member_map_'] + list(members):
             clsdict.pop(attrname, None)
 
         args = obj.__bases__, obj.__name__, sort_dict(members), obj.__module__
         state = sort_dict(clsdict)
         return type, args, state
 
     def save_dynamic_class(self, obj):
```

### Comparing `tarn-0.3.2/tarn/cache/serializers.py` & `tarn-0.4.0/tarn/serializers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
 import pickle
 from abc import ABC, abstractmethod
 from contextlib import suppress
 from functools import partial
 from gzip import GzipFile
 from pathlib import Path
-from typing import Union, Dict, Callable
+from typing import Callable, Dict, Union
 
 import numpy as np
-from tarn import ReadError
 
-from ..compat import rmtree
-from ..local import Storage
+from .compat import rmtree
+from .exceptions import ReadError
+from .pool import HashKeyStorage
 
 __all__ = (
     'Serializer', 'SerializerError', 'ChainSerializer', 'DictSerializer',
     'NumpySerializer', 'JsonSerializer', 'PickleSerializer',
 )
 
 
@@ -25,19 +25,19 @@
 
 class Serializer(ABC):
     @abstractmethod
     def save(self, value, folder: Path):
         """ Saves the ``value`` to ``folder`` """
 
     @abstractmethod
-    def load(self, folder: Path, storage: Storage):
+    def load(self, folder: Path, storage: HashKeyStorage):
         """ Loads the value from ``folder`` """
 
     @staticmethod
-    def _load_file(storage: Storage, loader: Callable, path: Path, *args, **kwargs):
+    def _load_file(storage: HashKeyStorage, loader: Callable, path: Path, *args, **kwargs):
         """ Useful function for loading files from storage """
         with open(path, 'r') as key:
             return storage.read(loader, key.read(), *args, **kwargs)
 
 
 class ChainSerializer(Serializer):
     def __init__(self, *serializers: Serializer):
@@ -46,15 +46,15 @@
     def save(self, value, folder: Path):
         for serializer in self.serializers:
             with suppress(SerializerError):
                 return serializer.save(value, folder)
 
         raise SerializerError(f'No serializer was able to save to {folder}.')
 
-    def load(self, folder: Path, storage: Storage):
+    def load(self, folder: Path, storage: HashKeyStorage):
         for serializer in self.serializers:
             with suppress(SerializerError):
                 return serializer.load(folder, storage)
 
         raise SerializerError(f'No serializer was able to load from {folder}.')
 
 
@@ -64,15 +64,15 @@
             value = json.dumps(value)
         except TypeError as e:
             raise SerializerError from e
 
         with open(folder / 'value.json', 'w') as file:
             file.write(value)
 
-    def load(self, folder: Path, storage: Storage):
+    def load(self, folder: Path, storage: HashKeyStorage):
         paths = list(folder.iterdir())
         if len(paths) != 1:
             raise SerializerError
 
         path, = paths
         if path.name != 'value.json':
             raise SerializerError
@@ -90,15 +90,15 @@
             value = pickle.dumps(value)
         except TypeError as e:
             raise SerializerError from e
 
         with open(folder / 'value.pkl', 'wb') as file:
             file.write(value)
 
-    def load(self, folder: Path, storage: Storage):
+    def load(self, folder: Path, storage: HashKeyStorage):
         paths = list(folder.iterdir())
         if len(paths) != 1:
             raise SerializerError
 
         path, = paths
         if path.name != 'value.pkl':
             raise SerializerError
@@ -132,15 +132,15 @@
             assert isinstance(compression, int)
             with GzipFile(folder / 'value.npy.gz', 'wb', compresslevel=compression, mtime=0) as file:
                 np.save(file, value, allow_pickle=False)
 
         else:
             np.save(folder / 'value.npy', value, allow_pickle=False)
 
-    def load(self, folder: Path, storage: Storage):
+    def load(self, folder: Path, storage: HashKeyStorage):
         paths = list(folder.iterdir())
         if len(paths) != 1:
             raise SerializerError
 
         path, = paths
         if path.name == 'value.npy':
             loader = partial(np.load, allow_pickle=False)
@@ -162,15 +162,14 @@
         self.keys_filename = 'dict_keys.json'
         self.serializer = serializer
 
     def save(self, data: dict, folder: Path):
         if not isinstance(data, dict):
             raise SerializerError
 
-        # TODO: remove all if at least one iteration fails
         try:
             keys_to_folder = {}
             for index, (key, value) in enumerate(data.items()):
                 keys_to_folder[index] = key
                 sub_folder = folder / str(index)
                 sub_folder.mkdir()
                 self.serializer.save(value, sub_folder)
@@ -181,15 +180,15 @@
                 rmtree(sub_folder)
 
             raise
 
         with open(folder / self.keys_filename, 'w+') as f:
             json.dump(keys_to_folder, f)
 
-    def load(self, folder: Path, storage: Storage):
+    def load(self, folder: Path, storage: HashKeyStorage):
         keys = folder / self.keys_filename
         if not keys.exists():
             raise SerializerError
 
         def loader(x):
             with open(x, 'r') as f:
                 return json.load(f)
```

### Comparing `tarn-0.3.2/tarn/compat.py` & `tarn-0.4.0/tarn/compat.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,46 +2,69 @@
 import os
 import platform
 import shutil
 import stat
 from pathlib import Path
 from typing import Union
 
+try:
+    from typing import Protocol
+except ImportError:
+    Protocol = object
+
+from .interface import PathOrStr
+
 if platform.system() == 'Windows':
     def rmtree(path, ignore_errors=False):
         # source: https://docs.python.org/3.10/library/shutil.html#rmtree-example
         def remove_readonly(func, p, _):
             os.chmod(p, stat.S_IWRITE)
             func(p)
 
         shutil.rmtree(path, ignore_errors=ignore_errors, onerror=remove_readonly)
 
 
-    def get_path_group(path: Union[Path, str]) -> Union[int, None]:
+    def get_path_group(path: PathOrStr) -> Union[int, None]:
         pass
 
+
+    def remove_file(path: PathOrStr):
+        os.chmod(path, stat.S_IWRITE)
+        os.remove(path)
+
 else:
     rmtree = shutil.rmtree
+    remove_file = os.remove
 
 
-    def get_path_group(path: Union[Path, str]) -> Union[int, None]:
+    def get_path_group(path: PathOrStr) -> Union[int, None]:
         return Path(path).stat().st_gid
 
 
 def set_path_attrs(path: Path, permissions: Union[int, None] = None, group: Union[str, int, None] = None):
     if permissions is not None:
         path.chmod(permissions)
     if group is not None:
         shutil.chown(path, group=group)
 
 
-def copy_file(source, destination):
+def copy_file(source: PathOrStr, destination: PathOrStr):
     # in Python>=3.8 the sendfile call is used, which apparently may fail
     try:
         shutil.copyfile(source, destination)
     except OSError as e:
         # BlockingIOError -> fallback to slow copy
         if e.errno != errno.EWOULDBLOCK:
             raise
 
         with open(source, 'rb') as src, open(destination, 'wb') as dst:
             shutil.copyfileobj(src, dst)
+
+
+class HashAlgorithm(Protocol):
+    digest_size: int
+
+    def update(self, chunk: bytes) -> None:
+        pass
+
+    def digest(self) -> bytes:
+        pass
```

### Comparing `tarn-0.3.2/tarn/config.py` & `tarn-0.4.0/tarn/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import hashlib
+import io
 from functools import partial
 from pathlib import Path
-from typing import Union, Dict, Any, Tuple, Sequence
+from typing import Any, Dict, Sequence, Tuple, Union
 
 import humanfriendly
-from pydantic import BaseModel, Extra, validator, root_validator
-from yaml import safe_load, safe_dump
+from pydantic import BaseModel, Extra, root_validator, validator
+from yaml import safe_dump, safe_load
 
-from .tools import Locker, DummyLocker, SizeTracker, DummySize, UsageTracker, DummyUsage
-from .utils import PathLike, mkdir
 from .compat import get_path_group
+from .tools import DummyLocker, DummySize, DummyUsage, Locker, SizeTracker, UsageTracker
+from .utils import PathLike, mkdir
 
 CONFIG_NAME = 'config.yml'
 
 
 class _NoExtra(BaseModel):
     class Config:
         extra = Extra.forbid
@@ -68,28 +69,28 @@
     size: ToolConfig = None
     usage: ToolConfig = None
     free_disk_size: Union[int, str] = 0
     max_size: Union[int, str] = None
     version: str = None
 
     @staticmethod
-    def _make(base, dummy, config):
+    def _make(base, dummy, config, *args):
         if config is None:
-            return dummy()
+            return dummy(*args)
         cls = find_subclass(base, config.name)
-        return cls(*config.args, **config.kwargs)
+        return cls(*args, *config.args, **config.kwargs)
 
     def make_locker(self) -> Locker:
         return self._make(Locker, DummyLocker, self.locker)
 
     def make_size(self) -> SizeTracker:
         return self._make(SizeTracker, DummySize, self.size)
 
-    def make_usage(self) -> UsageTracker:
-        return self._make(UsageTracker, DummyUsage, self.usage)
+    def make_usage(self, root: Path) -> UsageTracker:
+        return self._make(UsageTracker, DummyUsage, self.usage, root)
 
     @validator('free_disk_size', 'max_size')
     def to_size(cls, v):
         return parse_size(v)
 
     @validator('hash', 'locker', 'usage', pre=True)
     def normalize_tools(cls, v):
@@ -106,14 +107,18 @@
 
 
 def root_params(root: Path):
     stat = root.stat()
     return stat.st_mode & 0o777, get_path_group(root)
 
 
+def load_config_buffer(data: str) -> StorageConfig:
+    return StorageConfig.parse_obj(safe_load(io.StringIO(data)))
+
+
 def load_config(root: PathLike) -> StorageConfig:
     with open(Path(root) / CONFIG_NAME) as file:
         return StorageConfig.parse_obj(safe_load(file))
 
 
 def parse_size(x):
     if isinstance(x, int):
```

### Comparing `tarn-0.3.2/tarn/remote/ssh.py` & `tarn-0.4.0/tarn/location/scp.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import contextlib
 import socket
 import tempfile
+from contextlib import contextmanager
 from pathlib import Path
-from typing import Union, Sequence, Callable, Any, Tuple, Iterable
+from typing import ContextManager, Iterable, Sequence, Tuple, Union
 
 import paramiko
-from paramiko import SSHClient, AuthenticationException, SSHException
+from paramiko import AuthenticationException, SSHClient, SSHException
 from paramiko.config import SSH_PORT, SSHConfig
 from paramiko.ssh_exception import NoValidConnectionsError
 from scp import SCPClient, SCPException
 
-from ..compat import rmtree
-from ..config import load_config, HashConfig
+from ..compat import remove_file, rmtree
+from ..config import load_config
 from ..digest import key_to_relative
-from ..interface import RemoteStorage, Key
-from ..utils import PathLike
+from ..interface import Key, Keys, MaybeValue, PathOrStr
+from .interface import Location
 
 
 class UnknownHostException(SSHException):
     pass
 
 
-class SSHLocation(RemoteStorage):
-    def __init__(self, hostname: str, root: PathLike, port: int = SSH_PORT, username: str = None, password: str = None,
-                 key: Union[Path, Sequence[Path]] = (), optional: bool = False):
+class SCP(Location):
+    def __init__(self, hostname: str, root: PathOrStr, port: int = SSH_PORT, username: str = None, password: str = None,
+                 key: Union[Path, Sequence[Path]] = ()):
         ssh = SSHClient()
         ssh.load_system_host_keys()
         # TODO: not safe
         ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
         if isinstance(key, Path):
             key = str(key)
 
@@ -43,94 +43,105 @@
                 username = host.get('user', username)
                 key = host.get('identityfile', key)
 
         self.hostname, self.port, self.username, self.password, self.key = hostname, port, username, password, key
         self.root = Path(root)
         self.ssh = ssh
         self.levels = self.hash = None
-        self.optional = optional
 
-    def fetch(self, keys: Sequence[Key], store: Callable[[Key, Path], Any],
-              config: HashConfig) -> Iterable[Tuple[Any, bool]]:
+    @property
+    def key_size(self):
+        return sum(self.levels) if self.levels is not None else None
+
+    @contextmanager
+    def read(self, key: Key) -> ContextManager[MaybeValue]:
+        with self._connect() as scp:
+            if not scp:
+                yield
+                return
+
+            with tempfile.TemporaryDirectory() as temp_dir:
+                source = Path(temp_dir) / 'source'
+                try:
+                    scp.get(str(self.root / key_to_relative(key, self.levels)), str(source), recursive=True)
+                    if not source.exists():
+                        yield None
+                    else:
+                        # TODO: legacy
+                        if source.is_dir():
+                            yield source / 'data'
+                            rmtree(source)
 
-        with self._connect(config) as scp:
+                        else:
+                            yield source
+                            remove_file(source)
+
+                except (SCPException, socket.timeout, SSHException):
+                    yield None
+
+    def read_batch(self, keys: Keys) -> Iterable[Tuple[Key, MaybeValue]]:
+        with self._connect() as scp:
             if scp is None:
-                yield from [(None, False)] * len(keys)
+                for key in keys:
+                    yield key, None
                 return
 
+            # TODO: add `retry` logic?
             with tempfile.TemporaryDirectory() as temp_dir:
                 source = Path(temp_dir) / 'source'
                 for key in keys:
                     try:
                         scp.get(str(self.root / key_to_relative(key, self.levels)), str(source), recursive=True)
-                        if not source.exists():
-                            yield None, False
+                        if source.exists():
+                            # TODO: legacy
+                            if source.is_dir():
+                                yield key, source / 'data'
+                                rmtree(source)
+
+                            else:
+                                yield key, source
+                                remove_file(source)
 
                         else:
-                            value = store(key, source)
-                            rmtree(source)
-                            yield value, True
+                            yield key, None
 
                     except (SCPException, socket.timeout, SSHException):
-                        yield None, False
-
-                    rmtree(source, ignore_errors=True)
-
-    def push(self, keys: Sequence[Key], resolve: Callable[[Key], Path], config: HashConfig) -> Iterable[bool]:
-        with self._connect(config) as scp:
-            if scp is None:
-                yield from [False] * len(keys)
-                return
+                        yield key, None
 
-            for key in keys:
-                try:
-                    scp.put(resolve(key), str(self.root / key_to_relative(key, self.levels)), recursive=True)
-                    yield True
-
-                except (SCPException, socket.timeout, SSHException):
-                    yield False
-
-    @contextlib.contextmanager
-    def _connect(self, config):
+    @contextmanager
+    def _connect(self) -> SCPClient:
         try:
             self.ssh.connect(
                 self.hostname, self.port, self.username, self.password, key_filename=self.key,
                 auth_timeout=10
             )
         except AuthenticationException:
             raise AuthenticationException(self.hostname) from None
         except socket.gaierror:
             raise UnknownHostException(self.hostname) from None
         except (SSHException, NoValidConnectionsError):
-            if not self.optional:
-                raise
-
             yield None
             return
 
         try:
             with SCPClient(self.ssh.get_transport()) as scp:
-                if not self._get_config(scp, config):
+                if not self._get_config(scp):
                     yield None
                 else:
                     yield scp
 
         finally:
             self.ssh.close()
 
-    def _get_config(self, scp, config):
+    def _get_config(self, scp):
         try:
             if self.levels is None:
                 with tempfile.TemporaryDirectory() as temp_dir:
                     temp = Path(temp_dir) / 'config.yml'
                     scp.get(str(self.root / 'config.yml'), str(temp))
                     remote_config = load_config(temp_dir)
-                    self.hash, self.levels = remote_config.hash, remote_config.levels
+                    self.hash, self.levels = remote_config.hash.build(), remote_config.levels
 
-            assert self.hash == config, (self.hash, config)
             return True
 
         except SCPException:
-            if not self.optional:
-                raise
-
             return False
```

### Comparing `tarn-0.3.2/tarn.egg-info/PKG-INFO` & `tarn-0.4.0/tarn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: tarn
-Version: 0.3.2
+Version: 0.4.0
 Summary: A hashmap-based storage on local and remote disks
 Home-page: https://github.com/neuro-ml/tarn
 License: UNKNOWN
-Download-URL: https://github.com/neuro-ml/tarn/archive/v0.3.2.tar.gz
+Download-URL: https://github.com/neuro-ml/tarn/archive/v0.4.0.tar.gz
 Keywords: storage,cache,invalidation
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `tarn-0.3.2/tarn.egg-info/SOURCES.txt` & `tarn-0.4.0/tarn.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,31 +7,45 @@
 tarn/__init__.py
 tarn/__version__.py
 tarn/compat.py
 tarn/config.py
 tarn/digest.py
 tarn/exceptions.py
 tarn/interface.py
+tarn/legacy.py
+tarn/serializers.py
 tarn/ssh.py
 tarn/utils.py
 tarn.egg-info/PKG-INFO
 tarn.egg-info/SOURCES.txt
 tarn.egg-info/dependency_links.txt
 tarn.egg-info/requires.txt
 tarn.egg-info/top_level.txt
 tarn/cache/__init__.py
 tarn/cache/compat.py
 tarn/cache/index.py
 tarn/cache/pickler.py
 tarn/cache/serializers.py
 tarn/cache/storage.py
 tarn/local/__init__.py
-tarn/local/base.py
 tarn/local/disk.py
 tarn/local/storage.py
+tarn/location/__init__.py
+tarn/location/disk_dict.py
+tarn/location/fanout.py
+tarn/location/interface.py
+tarn/location/levels.py
+tarn/location/nginx.py
+tarn/location/scp.py
+tarn/pickler/__init__.py
+tarn/pickler/compat.py
+tarn/pickler/interface.py
+tarn/pool/__init__.py
+tarn/pool/hash_key.py
+tarn/pool/pickle_key.py
 tarn/remote/__init__.py
 tarn/remote/http.py
 tarn/remote/ssh.py
 tarn/tools/__init__.py
 tarn/tools/locker.py
 tarn/tools/size.py
 tarn/tools/usage.py
```

