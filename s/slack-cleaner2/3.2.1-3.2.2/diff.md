# Comparing `tmp/slack_cleaner2-3.2.1.tar.gz` & `tmp/slack_cleaner2-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack_cleaner2-3.2.1.tar", last modified: Tue Mar 21 00:31:56 2023, max compression
+gzip compressed data, was "slack_cleaner2-3.2.2.tar", last modified: Sat Apr  8 16:44:12 2023, max compression
```

## Comparing `slack_cleaner2-3.2.1.tar` & `slack_cleaner2-3.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 00:31:56.959945 slack_cleaner2-3.2.1/
--rw-rw-rw-   0        0        0     1094 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.1/LICENSE
--rw-rw-rw-   0        0        0      238 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5658 2023-03-21 00:31:56.959945 slack_cleaner2-3.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     4914 2022-07-21 13:17:11.000000 slack_cleaner2-3.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-03-21 00:31:56.932009 slack_cleaner2-3.2.1/docs/
--rw-rw-rw-   0        0        0      487 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.1/docs/api.rst
--rw-rw-rw-   0        0        0     6156 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.1/docs/conf.py
--rw-rw-rw-   0        0        0      303 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.1/docs/develop-install.rst
--rw-rw-rw-   0        0        0      495 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.1/docs/index.rst
--rw-rw-rw-   0        0        0      146 2023-03-21 00:30:21.000000 slack_cleaner2-3.2.1/docs/installing.rst
--rw-rw-rw-   0        0        0      116 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.1/docs/introduction.rst
--rw-rw-rw-   0        0        0      121 2023-03-21 00:02:41.000000 slack_cleaner2-3.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       78 2022-07-21 13:17:39.000000 slack_cleaner2-3.2.1/requirements.txt
--rw-rw-rw-   0        0        0      447 2023-03-21 00:31:56.961578 slack_cleaner2-3.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1544 2023-03-21 00:31:09.000000 slack_cleaner2-3.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-21 00:31:56.942716 slack_cleaner2-3.2.1/slack_cleaner2/
--rw-rw-rw-   0        0        0      670 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.1/slack_cleaner2/__init__.py
--rw-rw-rw-   0        0        0      128 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.1/slack_cleaner2/__main__.py
--rw-rw-rw-   0        0        0      167 2023-03-21 00:31:09.000000 slack_cleaner2-3.2.1/slack_cleaner2/_info.py
--rw-rw-rw-   0        0        0     7383 2023-03-21 00:30:26.000000 slack_cleaner2-3.2.1/slack_cleaner2/cli.py
--rw-rw-rw-   0        0        0     3277 2023-03-21 00:30:26.000000 slack_cleaner2-3.2.1/slack_cleaner2/logger.py
--rw-rw-rw-   0        0        0    46852 2023-03-21 00:30:26.000000 slack_cleaner2-3.2.1/slack_cleaner2/model.py
--rw-rw-rw-   0        0        0     6023 2022-07-21 13:17:39.000000 slack_cleaner2-3.2.1/slack_cleaner2/predicates.py
--rw-rw-rw-   0        0        0      618 2021-10-27 13:33:40.000000 slack_cleaner2-3.2.1/slack_cleaner2/util.py
-drwxrwxrwx   0        0        0        0 2023-03-21 00:31:56.956996 slack_cleaner2-3.2.1/slack_cleaner2.egg-info/
--rw-rw-rw-   0        0        0     5658 2023-03-21 00:31:56.000000 slack_cleaner2-3.2.1/slack_cleaner2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-03-21 00:31:56.000000 slack_cleaner2-3.2.1/slack_cleaner2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 00:31:56.000000 slack_cleaner2-3.2.1/slack_cleaner2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-03-21 00:31:56.000000 slack_cleaner2-3.2.1/slack_cleaner2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-21 00:31:56.000000 slack_cleaner2-3.2.1/slack_cleaner2.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       74 2023-03-21 00:31:56.000000 slack_cleaner2-3.2.1/slack_cleaner2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-03-21 00:31:56.000000 slack_cleaner2-3.2.1/slack_cleaner2.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-21 00:31:56.958942 slack_cleaner2-3.2.1/tests/
--rw-rw-rw-   0        0        0       18 2019-09-15 21:36:28.000000 slack_cleaner2-3.2.1/tests/__init__.py
--rw-rw-rw-   0        0        0      734 2021-10-27 13:33:40.000000 slack_cleaner2-3.2.1/tests/test_slack_cleaner2.py
+drwxrwxrwx   0        0        0        0 2023-04-08 16:44:12.109470 slack_cleaner2-3.2.2/
+-rw-rw-rw-   0        0        0     1094 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.2/LICENSE
+-rw-rw-rw-   0        0        0      238 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5658 2023-04-08 16:44:12.111470 slack_cleaner2-3.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4914 2022-07-21 13:17:11.000000 slack_cleaner2-3.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-08 16:44:12.004943 slack_cleaner2-3.2.2/docs/
+-rw-rw-rw-   0        0        0      487 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.2/docs/api.rst
+-rw-rw-rw-   0        0        0     6156 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.2/docs/conf.py
+-rw-rw-rw-   0        0        0      303 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.2/docs/develop-install.rst
+-rw-rw-rw-   0        0        0      495 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.2/docs/index.rst
+-rw-rw-rw-   0        0        0      146 2023-03-21 00:30:21.000000 slack_cleaner2-3.2.2/docs/installing.rst
+-rw-rw-rw-   0        0        0      116 2020-05-07 11:49:42.000000 slack_cleaner2-3.2.2/docs/introduction.rst
+-rw-rw-rw-   0        0        0      121 2023-03-21 00:02:41.000000 slack_cleaner2-3.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       78 2022-07-21 13:17:39.000000 slack_cleaner2-3.2.2/requirements.txt
+-rw-rw-rw-   0        0        0      447 2023-04-08 16:44:12.120343 slack_cleaner2-3.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1544 2023-04-08 16:43:31.000000 slack_cleaner2-3.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-08 16:44:12.053344 slack_cleaner2-3.2.2/slack_cleaner2/
+-rw-rw-rw-   0        0        0      670 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.2/slack_cleaner2/__init__.py
+-rw-rw-rw-   0        0        0      128 2020-04-29 15:24:16.000000 slack_cleaner2-3.2.2/slack_cleaner2/__main__.py
+-rw-rw-rw-   0        0        0      167 2023-04-08 16:43:31.000000 slack_cleaner2-3.2.2/slack_cleaner2/_info.py
+-rw-rw-rw-   0        0        0     7383 2023-03-21 00:30:26.000000 slack_cleaner2-3.2.2/slack_cleaner2/cli.py
+-rw-rw-rw-   0        0        0     3277 2023-03-21 00:30:26.000000 slack_cleaner2-3.2.2/slack_cleaner2/logger.py
+-rw-rw-rw-   0        0        0    46774 2023-04-08 16:43:16.000000 slack_cleaner2-3.2.2/slack_cleaner2/model.py
+-rw-rw-rw-   0        0        0     6023 2022-07-21 13:17:39.000000 slack_cleaner2-3.2.2/slack_cleaner2/predicates.py
+-rw-rw-rw-   0        0        0      618 2021-10-27 13:33:40.000000 slack_cleaner2-3.2.2/slack_cleaner2/util.py
+drwxrwxrwx   0        0        0        0 2023-04-08 16:44:12.093558 slack_cleaner2-3.2.2/slack_cleaner2.egg-info/
+-rw-rw-rw-   0        0        0     5658 2023-04-08 16:44:10.000000 slack_cleaner2-3.2.2/slack_cleaner2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-04-08 16:44:10.000000 slack_cleaner2-3.2.2/slack_cleaner2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-08 16:44:10.000000 slack_cleaner2-3.2.2/slack_cleaner2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-04-08 16:44:10.000000 slack_cleaner2-3.2.2/slack_cleaner2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-08 16:44:10.000000 slack_cleaner2-3.2.2/slack_cleaner2.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       74 2023-04-08 16:44:10.000000 slack_cleaner2-3.2.2/slack_cleaner2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-08 16:44:10.000000 slack_cleaner2-3.2.2/slack_cleaner2.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-08 16:44:12.103584 slack_cleaner2-3.2.2/tests/
+-rw-rw-rw-   0        0        0       18 2019-09-15 21:36:28.000000 slack_cleaner2-3.2.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      734 2021-10-27 13:33:40.000000 slack_cleaner2-3.2.2/tests/test_slack_cleaner2.py
```

### Comparing `slack_cleaner2-3.2.1/LICENSE` & `slack_cleaner2-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.1/PKG-INFO` & `slack_cleaner2-3.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack_cleaner2
-Version: 3.2.1
+Version: 3.2.2
 Summary: Slack Cleaner2 is an improved slack cleaner version using a python first approach
 Home-page: https://github.com/sgratzl/slack_cleaner2
 Author: Samuel Gratzl
 Author-email: sam@sgratzl.com
 License: MIT license
 Keywords: slack_cleaner2 slack slack-cleaner
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `slack_cleaner2-3.2.1/README.md` & `slack_cleaner2-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.1/docs/conf.py` & `slack_cleaner2-3.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.1/setup.py` & `slack_cleaner2-3.2.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup_requirements = ["pytest-runner"]
 test_requirements = ["pytest"]
 
 setup(
     name="slack_cleaner2",
     description="Slack Cleaner2 is an improved slack cleaner version using a python first approach",
-    version="3.2.1",
+    version="3.2.2",
     license="MIT license",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords="slack_cleaner2 slack slack-cleaner",
     author="Samuel Gratzl",
     author_email="sam@sgratzl.com",
     url="https://github.com/sgratzl/slack_cleaner2",
```

### Comparing `slack_cleaner2-3.2.1/slack_cleaner2/__init__.py` & `slack_cleaner2-3.2.2/slack_cleaner2/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.1/slack_cleaner2/cli.py` & `slack_cleaner2-3.2.2/slack_cleaner2/cli.py`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.1/slack_cleaner2/logger.py` & `slack_cleaner2-3.2.2/slack_cleaner2/logger.py`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.1/slack_cleaner2/model.py` & `slack_cleaner2-3.2.2/slack_cleaner2/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -722,16 +722,16 @@
         :type channel: str,SlackChannel
         :param types: see slack api, one or multiple of all,spaces,snippets,images,gdocs,zips,pdfs
         :type types: str
         :return: generator of SlackFile objects
         :rtype: SlackFile
         """
 
-        after = _parse_time(after, slack.log, as_int=True)
-        before = _parse_time(before, slack.log, as_int=True)
+        after = _parse_time(after, slack.log)
+        before = _parse_time(before, slack.log)
 
         if isinstance(user, SlackUser):
             user = user.id
         if isinstance(channel, SlackChannel):
             channel = channel.id
 
         slack.log.debug("list all files(user=%s, after=%s, before=%s, types=%s, channel=%s", user, after, before, types, channel)
@@ -883,28 +883,26 @@
     def _context(self) -> str:
         return str(self.file)
 
     def _delete_impl(self):
         return self._slack.call_rate_limited(lambda: self._slack.client.reactions_remove(name=self.name, file=self.file.id))
 
 
-def _parse_time(time_str: TimeIsh, log: SlackLogger, as_int: bool = False) -> Optional[str]:
+def _parse_time(time_str: TimeIsh, log: SlackLogger) -> Optional[str]:
     if time_str is None:
         return None
     if isinstance(time_str, (int, float)):
-        return str(time_str)
+        return str(int(round(time_str)))
     try:
         if len(time_str) == 8:
             time_d = time.strptime(time_str, "%Y%m%d")
         else:
             time_d = time.strptime(time_str, "%Y%m%d%H%M")
         sec = time.mktime(time_d)
-        if as_int:
-            return str(int(sec))
-        return str(sec)
+        return str(int(round(sec)))
     except ValueError:
         log.exception("error parsing date %s", time_str)
         return None
 
 
 ByKey = TypeVar("ByKey")
```

### Comparing `slack_cleaner2-3.2.1/slack_cleaner2/predicates.py` & `slack_cleaner2-3.2.2/slack_cleaner2/predicates.py`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.1/slack_cleaner2/util.py` & `slack_cleaner2-3.2.2/slack_cleaner2/util.py`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.1/slack_cleaner2.egg-info/PKG-INFO` & `slack_cleaner2-3.2.2/slack_cleaner2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-cleaner2
-Version: 3.2.1
+Version: 3.2.2
 Summary: Slack Cleaner2 is an improved slack cleaner version using a python first approach
 Home-page: https://github.com/sgratzl/slack_cleaner2
 Author: Samuel Gratzl
 Author-email: sam@sgratzl.com
 License: MIT license
 Keywords: slack_cleaner2 slack slack-cleaner
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `slack_cleaner2-3.2.1/slack_cleaner2.egg-info/SOURCES.txt` & `slack_cleaner2-3.2.2/slack_cleaner2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slack_cleaner2-3.2.1/tests/test_slack_cleaner2.py` & `slack_cleaner2-3.2.2/tests/test_slack_cleaner2.py`

 * *Files identical despite different names*

