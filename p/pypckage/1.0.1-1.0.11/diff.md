# Comparing `tmp/pypckage-1.0.1.tar.gz` & `tmp/pypckage-1.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypckage-1.0.1.tar", last modified: Fri Apr  7 19:10:40 2023, max compression
+gzip compressed data, was "pypckage-1.0.11.tar", last modified: Sat Apr  8 18:09:07 2023, max compression
```

## Comparing `pypckage-1.0.1.tar` & `pypckage-1.0.11.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 19:10:40.690308 pypckage-1.0.1/
--rw-rw-rw-   0        0        0     1088 2023-04-07 18:52:04.000000 pypckage-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     1396 2023-04-07 19:10:40.689297 pypckage-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      921 2023-04-07 19:04:21.000000 pypckage-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-04-07 19:10:40.690308 pypckage-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      796 2023-04-07 19:10:25.000000 pypckage-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:10:40.653212 pypckage-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-07 19:10:40.669014 pypckage-1.0.1/src/pypckage/
--rw-rw-rw-   0        0        0     5683 2023-04-07 19:10:26.000000 pypckage-1.0.1/src/pypckage/Pypckage.py
--rw-rw-rw-   0        0        0       23 2023-04-07 18:44:16.000000 pypckage-1.0.1/src/pypckage/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-07 19:10:40.687287 pypckage-1.0.1/src/pypckage.egg-info/
--rw-rw-rw-   0        0        0     1396 2023-04-07 19:10:40.000000 pypckage-1.0.1/src/pypckage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-04-07 19:10:40.000000 pypckage-1.0.1/src/pypckage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 19:10:40.000000 pypckage-1.0.1/src/pypckage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-04-07 19:10:40.000000 pypckage-1.0.1/src/pypckage.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-04-07 19:10:40.000000 pypckage-1.0.1/src/pypckage.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-07 19:10:40.000000 pypckage-1.0.1/src/pypckage.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 18:09:07.583467 pypckage-1.0.11/
+-rw-rw-rw-   0        0        0     1088 2023-04-07 19:13:36.000000 pypckage-1.0.11/LICENSE
+-rw-rw-rw-   0        0        0     1688 2023-04-08 18:09:07.582445 pypckage-1.0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     1212 2023-04-08 18:06:46.000000 pypckage-1.0.11/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-08 18:09:07.585152 pypckage-1.0.11/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-04-08 18:08:41.000000 pypckage-1.0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:09:07.523908 pypckage-1.0.11/src/
+drwxrwxrwx   0        0        0        0 2023-04-08 18:09:07.536133 pypckage-1.0.11/src/pypckage/
+-rw-rw-rw-   0        0        0     5684 2023-04-08 18:08:46.000000 pypckage-1.0.11/src/pypckage/Pypckage.py
+-rw-rw-rw-   0        0        0       23 2023-04-07 19:13:39.000000 pypckage-1.0.11/src/pypckage/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-08 18:09:07.578764 pypckage-1.0.11/src/pypckage.egg-info/
+-rw-rw-rw-   0        0        0     1688 2023-04-08 18:09:07.000000 pypckage-1.0.11/src/pypckage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-04-08 18:09:07.000000 pypckage-1.0.11/src/pypckage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 18:09:07.000000 pypckage-1.0.11/src/pypckage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-04-08 18:09:07.000000 pypckage-1.0.11/src/pypckage.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-04-08 18:09:07.000000 pypckage-1.0.11/src/pypckage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-08 18:09:07.000000 pypckage-1.0.11/src/pypckage.egg-info/top_level.txt
```

### Comparing `pypckage-1.0.1/LICENSE` & `pypckage-1.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `pypckage-1.0.1/PKG-INFO` & `pypckage-1.0.11/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: pypckage
-Version: 1.0.1
+Version: 1.0.11
 Summary: Pypckage is a tool to facilitate the configuration of a python package.
 Home-page: https://github.com/LixNew2/Pypckage
 Author: LixNew
 Author-email: lixnew2@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pypckage
 
+[![Downloads](https://static.pepy.tech/badge/pypckage)](https://pepy.tech/project/pypckage)
+[![Version](https://img.shields.io/pypi/v/pypckage)](https://pypi.org/project/pypckage/)
+[![Python Version](https://img.shields.io/pypi/pyversions/pypckage)](https://pypi.org/project/pypckage/)
+
 Pypckage is a tool that facilitates the configuration of a python package. 
 You just need to run a command in the terminal and enter some information and Pypckage takes care of everything. 
 It creates the "setup.py, LICENSE, README.md, etc", all preconfigured. All you have to do is to customize the created files.
 
 ## Set up
 ----
```

### Comparing `pypckage-1.0.1/README.md` & `pypckage-1.0.11/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Pypckage
 
+[![Downloads](https://static.pepy.tech/badge/pypckage)](https://pepy.tech/project/pypckage)
+[![Version](https://img.shields.io/pypi/v/pypckage)](https://pypi.org/project/pypckage/)
+[![Python Version](https://img.shields.io/pypi/pyversions/pypckage)](https://pypi.org/project/pypckage/)
+
 Pypckage is a tool that facilitates the configuration of a python package. 
 You just need to run a command in the terminal and enter some information and Pypckage takes care of everything. 
 It creates the "setup.py, LICENSE, README.md, etc", all preconfigured. All you have to do is to customize the created files.
 
 ## Set up
 ----
```

### Comparing `pypckage-1.0.1/setup.py` & `pypckage-1.0.11/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
                     
 setup(
 name="pypckage",
-version="1.0.1",
+version="1.0.11",
 author="LixNew",
 author_email="lixnew2@gmail.com",
 description="Pypckage is a tool to facilitate the configuration of a python package.",
 long_description=open("README.md", encoding="utf-8").read(),
 long_description_content_type="text/markdown",
 url="https://github.com/LixNew2/Pypckage",
 packages=find_packages("src"),
```

### Comparing `pypckage-1.0.1/src/pypckage/Pypckage.py` & `pypckage-1.0.11/src/pypckage/Pypckage.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-__version__ = '1.0.1'
+__version__ = '1.0.11'
 __title__ = 'Pypckage'
 __description__ = "Pypckage is a tool to facilitate the configuration of a python package."
 __autor__ = 'LixNew'
 __twitter__ = '@LixNew2'
 __url__ = "https://github.com/LixNew2/Pypckage"
```

### Comparing `pypckage-1.0.1/src/pypckage.egg-info/PKG-INFO` & `pypckage-1.0.11/src/pypckage.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 Metadata-Version: 2.1
 Name: pypckage
-Version: 1.0.1
+Version: 1.0.11
 Summary: Pypckage is a tool to facilitate the configuration of a python package.
 Home-page: https://github.com/LixNew2/Pypckage
 Author: LixNew
 Author-email: lixnew2@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Pypckage
 
+[![Downloads](https://static.pepy.tech/badge/pypckage)](https://pepy.tech/project/pypckage)
+[![Version](https://img.shields.io/pypi/v/pypckage)](https://pypi.org/project/pypckage/)
+[![Python Version](https://img.shields.io/pypi/pyversions/pypckage)](https://pypi.org/project/pypckage/)
+
 Pypckage is a tool that facilitates the configuration of a python package. 
 You just need to run a command in the terminal and enter some information and Pypckage takes care of everything. 
 It creates the "setup.py, LICENSE, README.md, etc", all preconfigured. All you have to do is to customize the created files.
 
 ## Set up
 ----
```

