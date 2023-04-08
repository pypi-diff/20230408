# Comparing `tmp/team_center_api-0.2.7.tar.gz` & `tmp/team_center_api-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\team_center_api-0.2.7.tar", last modified: Sun Apr 28 04:10:53 2019, max compression
+gzip compressed data, was "dist\team_center_api-0.2.9.tar", last modified: Sun Apr 28 04:13:45 2019, max compression
```

## Comparing `team_center_api-0.2.7.tar` & `team_center_api-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2019-04-28 04:10:53.000000 team_center_api-0.2.7/
--rw-rw-rw-   0        0        0      242 2019-04-28 04:10:53.000000 team_center_api-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2019-04-28 04:10:53.000000 team_center_api-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      447 2019-04-28 04:10:32.000000 team_center_api-0.2.7/setup.py
-drwxrwxrwx   0        0        0        0 2019-04-28 04:10:53.000000 team_center_api-0.2.7/team_center_api/
--rw-rw-rw-   0        0        0       45 2019-04-28 04:10:32.000000 team_center_api-0.2.7/team_center_api/__init__.py
--rw-rw-rw-   0        0        0     5509 2019-04-28 04:09:58.000000 team_center_api-0.2.7/team_center_api/api.py
--rw-rw-rw-   0        0        0      476 2019-04-27 11:51:26.000000 team_center_api-0.2.7/team_center_api/constants.py
--rw-rw-rw-   0        0        0      110 2018-12-25 10:10:31.000000 team_center_api-0.2.7/team_center_api/log.py
--rw-rw-rw-   0        0        0      633 2018-12-25 10:10:31.000000 team_center_api-0.2.7/team_center_api/six.py
-drwxrwxrwx   0        0        0        0 2019-04-28 04:10:53.000000 team_center_api-0.2.7/team_center_api.egg-info/
--rw-rw-rw-   0        0        0      242 2019-04-28 04:10:53.000000 team_center_api-0.2.7/team_center_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2019-04-28 04:10:53.000000 team_center_api-0.2.7/team_center_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2019-04-28 04:10:53.000000 team_center_api-0.2.7/team_center_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2019-04-27 12:11:16.000000 team_center_api-0.2.7/team_center_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2019-04-28 04:10:53.000000 team_center_api-0.2.7/team_center_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2019-04-28 04:10:53.000000 team_center_api-0.2.7/team_center_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2019-04-28 04:13:45.000000 team_center_api-0.2.9/
+-rw-rw-rw-   0        0        0      242 2019-04-28 04:13:45.000000 team_center_api-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2019-04-28 04:13:45.000000 team_center_api-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      447 2019-04-28 04:13:32.000000 team_center_api-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2019-04-28 04:13:45.000000 team_center_api-0.2.9/team_center_api/
+-rw-rw-rw-   0        0        0       45 2019-04-28 04:13:33.000000 team_center_api-0.2.9/team_center_api/__init__.py
+-rw-rw-rw-   0        0        0     5541 2019-04-28 04:13:01.000000 team_center_api-0.2.9/team_center_api/api.py
+-rw-rw-rw-   0        0        0      476 2019-04-27 11:51:26.000000 team_center_api-0.2.9/team_center_api/constants.py
+-rw-rw-rw-   0        0        0      110 2018-12-25 10:10:31.000000 team_center_api-0.2.9/team_center_api/log.py
+-rw-rw-rw-   0        0        0      633 2018-12-25 10:10:31.000000 team_center_api-0.2.9/team_center_api/six.py
+drwxrwxrwx   0        0        0        0 2019-04-28 04:13:45.000000 team_center_api-0.2.9/team_center_api.egg-info/
+-rw-rw-rw-   0        0        0      242 2019-04-28 04:13:45.000000 team_center_api-0.2.9/team_center_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2019-04-28 04:13:45.000000 team_center_api-0.2.9/team_center_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2019-04-28 04:13:45.000000 team_center_api-0.2.9/team_center_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2019-04-27 12:11:16.000000 team_center_api-0.2.9/team_center_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2019-04-28 04:13:45.000000 team_center_api-0.2.9/team_center_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2019-04-28 04:13:45.000000 team_center_api-0.2.9/team_center_api.egg-info/top_level.txt
```

### Comparing `team_center_api-0.2.7/team_center_api/api.py` & `team_center_api-0.2.9/team_center_api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,15 @@
 
     def verify_pin(self, username, pin):
         path = constants.URL_PIN_VERIFY
         url = urlunsplit((self.schema, self.host, path, '', ''))
 
         data = dict(
             username=username,
+            source=self.source,
             pin=pin,
         )
 
         try:
             rsp = requests.post(url, data=self._make_signed_params(path, data), timeout=self.timeout)
 
             jdata = rsp.json()
```

### Comparing `team_center_api-0.2.7/team_center_api/six.py` & `team_center_api-0.2.9/team_center_api/six.py`

 * *Files identical despite different names*

