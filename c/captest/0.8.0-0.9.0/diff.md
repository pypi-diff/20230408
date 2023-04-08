# Comparing `tmp/captest-0.8.0.tar.gz` & `tmp/captest-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/captest-0.8.0.tar", last modified: Mon Apr 13 15:20:59 2020, max compression
+gzip compressed data, was "dist/captest-0.9.0.tar", last modified: Mon Aug 17 02:52:25 2020, max compression
```

## Comparing `captest-0.8.0.tar` & `captest-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-13 15:20:59.000000 captest-0.8.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1067 2020-04-13 15:18:11.000000 captest-0.8.0/LICENSE.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      109 2020-04-13 15:18:11.000000 captest-0.8.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     3651 2020-04-13 15:20:59.000000 captest-0.8.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2354 2020-04-13 15:18:11.000000 captest-0.8.0/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-13 15:20:59.000000 captest-0.8.0/captest/
--rw-rw-r--   0 travis    (2000) travis    (2000)      121 2020-04-13 15:18:11.000000 captest-0.8.0/captest/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2020-04-13 15:20:59.000000 captest-0.8.0/captest/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   117060 2020-04-13 15:18:11.000000 captest-0.8.0/captest/capdata.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-13 15:20:59.000000 captest-0.8.0/captest.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3651 2020-04-13 15:20:59.000000 captest-0.8.0/captest.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      280 2020-04-13 15:20:59.000000 captest-0.8.0/captest.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-13 15:20:59.000000 captest-0.8.0/captest.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      200 2020-04-13 15:20:59.000000 captest-0.8.0/captest.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-04-13 15:20:59.000000 captest-0.8.0/captest.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      269 2020-04-13 15:20:59.000000 captest-0.8.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1889 2020-04-13 15:18:11.000000 captest-0.8.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68611 2020-04-13 15:18:11.000000 captest-0.8.0/versioneer.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-17 02:52:25.000000 captest-0.9.0/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1067 2020-08-17 02:49:04.000000 captest-0.9.0/LICENSE.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      109 2020-08-17 02:49:04.000000 captest-0.9.0/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5378 2020-08-17 02:52:25.000000 captest-0.9.0/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4161 2020-08-17 02:49:04.000000 captest-0.9.0/README.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-17 02:52:25.000000 captest-0.9.0/captest/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      121 2020-08-17 02:49:04.000000 captest-0.9.0/captest/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      497 2020-08-17 02:52:25.000000 captest-0.9.0/captest/_version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   117066 2020-08-17 02:49:04.000000 captest-0.9.0/captest/capdata.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-08-17 02:52:25.000000 captest-0.9.0/captest.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5378 2020-08-17 02:52:25.000000 captest-0.9.0/captest.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      280 2020-08-17 02:52:25.000000 captest-0.9.0/captest.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-08-17 02:52:25.000000 captest-0.9.0/captest.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      197 2020-08-17 02:52:25.000000 captest-0.9.0/captest.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2020-08-17 02:52:25.000000 captest-0.9.0/captest.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      269 2020-08-17 02:52:25.000000 captest-0.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1886 2020-08-17 02:49:04.000000 captest-0.9.0/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    68611 2020-08-17 02:49:04.000000 captest-0.9.0/versioneer.py
```

### Comparing `captest-0.8.0/LICENSE.txt` & `captest-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `captest-0.8.0/captest/capdata.py` & `captest-0.9.0/captest/capdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -771,26 +771,26 @@
     Returns
     -------
     DatetimeIndex with timezone
     """
     if isinstance(time_source, pd.core.indexes.datetimes.DatetimeIndex):
         if time_source.tz is None:
             time_source = time_source.tz_localize(loc['tz'], ambiguous='infer',
-                                                  errors='coerce')
+                                                  nonexistent='NaT')
             return time_source
         else:
             if pytz.timezone(loc['tz']) != time_source.tz:
                 warnings.warn('Passed a DatetimeIndex with a timezone that '
                               'does not match the timezone in the loc dict. '
                               'Using the timezone of the DatetimeIndex.')
             return time_source
     elif isinstance(time_source, pd.core.frame.DataFrame):
         if time_source.index.tz is None:
             return time_source.index.tz_localize(loc['tz'], ambiguous='infer',
-                                                 errors='coerce')
+                                                 nonexistent='NaT')
         else:
             if pytz.timezone(loc['tz']) != time_source.index.tz:
                 warnings.warn('Passed a DataFrame with a timezone that '
                               'does not match the timezone in the loc dict. '
                               'Using the timezone of the DataFrame.')
             return time_source.index
 
@@ -864,15 +864,15 @@
     if output == 'ghi_all':
         csky_df = ghi[['ghi', 'dni', 'dhi']]
     if output == 'all':
         csky_df = pd.concat([mc.total_irrad[cols], ghi[['ghi', 'dni', 'dhi']]],
                             axis=1)
 
     ix_no_tz = csky_df.index.tz_localize(None, ambiguous='infer',
-                                         errors='coerce')
+                                         nonexistent='NaT')
     csky_df.index = ix_no_tz
 
     if concat:
         if isinstance(time_source, pd.core.frame.DataFrame):
             df_with_csky = pd.concat([time_source, csky_df], axis=1)
             return df_with_csky
         else:
```

### Comparing `captest-0.8.0/setup.py` & `captest-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 setup(
     name='captest',
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     url='http://github.com/bt-/pvcaptest',
     license='MIT',
     author='Ben Taylor',
-    python_requires='>=3.5',
-    install_requires=['pandas>=0.24',
+    python_requires='>=3.7',
+    install_requires=['pandas>=1',
                       'numpy>=1.13.0',
                       'python-dateutil>=2.5',
                       'matplotlib>=2',
                       'statsmodels>=0.8',
                       'scikit-learn>=0.19',
                       'bokeh>=1',
                       ],
```

### Comparing `captest-0.8.0/versioneer.py` & `captest-0.9.0/versioneer.py`

 * *Files identical despite different names*

