# Comparing `tmp/agrometeo_geopy-0.1.3.tar.gz` & `tmp/agrometeo_geopy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agrometeo_geopy-0.1.3.tar", max compression
+gzip compressed data, was "agrometeo_geopy-0.2.0.tar", last modified: Sat Apr  8 19:29:48 2023, max compression
```

## Comparing `agrometeo_geopy-0.1.3.tar` & `agrometeo_geopy-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-04-03 12:21:17.182842 agrometeo_geopy-0.1.3/LICENSE
--rw-r--r--   0        0        0     7833 2023-04-03 12:21:17.182842 agrometeo_geopy-0.1.3/README.md
--rw-r--r--   0        0        0      186 2023-04-03 12:21:17.182842 agrometeo_geopy-0.1.3/agrometeo/__init__.py
--rw-r--r--   0        0        0     3918 2023-04-03 12:21:17.182842 agrometeo_geopy-0.1.3/agrometeo/base.py
--rw-r--r--   0        0        0     7617 2023-04-03 12:21:17.182842 agrometeo_geopy-0.1.3/agrometeo/core.py
--rw-r--r--   0        0        0     6068 2023-04-03 12:21:17.182842 agrometeo_geopy-0.1.3/agrometeo/plotting.py
--rw-r--r--   0        0        0      273 2023-04-03 12:21:17.182842 agrometeo_geopy-0.1.3/agrometeo/settings.py
--rw-r--r--   0        0        0     2563 2023-04-03 12:21:17.186842 agrometeo_geopy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       45 2023-04-03 12:21:17.186842 agrometeo_geopy-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     1409 2023-04-03 12:21:17.186842 agrometeo_geopy-0.1.3/tests/test_agrometeo.py
--rw-r--r--   0        0        0    10005 1970-01-01 00:00:00.000000 agrometeo_geopy-0.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:29:48.608429 agrometeo_geopy-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-08 19:29:26.000000 agrometeo_geopy-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-04-08 19:29:48.608429 agrometeo_geopy-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-04-08 19:29:26.000000 agrometeo_geopy-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:29:48.604429 agrometeo_geopy-0.2.0/agrometeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-08 19:29:26.000000 agrometeo_geopy-0.2.0/agrometeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-04-08 19:29:26.000000 agrometeo_geopy-0.2.0/agrometeo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12208 2023-04-08 19:29:26.000000 agrometeo_geopy-0.2.0/agrometeo/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-08 19:29:26.000000 agrometeo_geopy-0.2.0/agrometeo/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-04-08 19:29:26.000000 agrometeo_geopy-0.2.0/agrometeo/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:29:48.608429 agrometeo_geopy-0.2.0/agrometeo_geopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-04-08 19:29:48.000000 agrometeo_geopy-0.2.0/agrometeo_geopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-08 19:29:48.000000 agrometeo_geopy-0.2.0/agrometeo_geopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 19:29:48.000000 agrometeo_geopy-0.2.0/agrometeo_geopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-08 19:29:48.000000 agrometeo_geopy-0.2.0/agrometeo_geopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-08 19:29:48.000000 agrometeo_geopy-0.2.0/agrometeo_geopy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-08 19:29:26.000000 agrometeo_geopy-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 19:29:48.608429 agrometeo_geopy-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 19:29:48.608429 agrometeo_geopy-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-04-08 19:29:26.000000 agrometeo_geopy-0.2.0/tests/test_agrometeo.py
```

### Comparing `agrometeo_geopy-0.1.3/LICENSE` & `agrometeo_geopy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agrometeo_geopy-0.1.3/README.md` & `agrometeo_geopy-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -212,12 +212,12 @@
                     <td>22.0</td>
                 </tr>
             </tbody>
     </table></div>
     <p>576 rows × 10 columns</p>
 </div>
 
-See [the user guide](https://agrometeo-geopy.readthedocs.io/en/latest/usage) for more details.
+See [the user guide](https://agrometeo-geopy.readthedocs.io/en/latest/usage.html) for more details.
 
 ## Acknowledgements
 
 - This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [zillionare/cookiecutter-pypackage](https://github.com/zillionare/cookiecutter-pypackage) project template.
```

#### html2text {}

```diff
@@ -63,12 +63,12 @@
 |23:  |        |      |       |      |       |     |       |      |       |       |
 |40:00|________|______|_______|______|_______|_____|_______|______|_______|_______|
 |2021-|        |      |       |      |       |     |       |      |       |       |
 |08-16|17.1    |17.8  |17.5   |17.1  |17.7   |17.3 |17.1   |17.1  |18.1   |22.0   |
 |23:  |        |      |       |      |       |     |       |      |       |       |
 |50:00|________|______|_______|______|_______|_____|_______|______|_______|_______|
 576 rows Ã 10 columns
-See [the user guide](https://agrometeo-geopy.readthedocs.io/en/latest/usage)
-for more details. ## Acknowledgements - This package was created with
-[Cookiecutter](https://github.com/audreyr/cookiecutter) and the [zillionare/
-cookiecutter-pypackage](https://github.com/zillionare/cookiecutter-pypackage)
-project template.
+See [the user guide](https://agrometeo-geopy.readthedocs.io/en/latest/
+usage.html) for more details. ## Acknowledgements - This package was created
+with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
+[zillionare/cookiecutter-pypackage](https://github.com/zillionare/cookiecutter-
+pypackage) project template.
```

### Comparing `agrometeo_geopy-0.1.3/agrometeo/base.py` & `agrometeo_geopy-0.2.0/agrometeo/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     """Meteo station dataset."""
 
     def __init__(
         self,
         *,
         region=None,
         crs=None,
-        station_id_name=None,
+        stations_id_name=None,
         time_name=None,
         geocode_to_gdf_kws=None,
     ):
         """
         Initialize an meteo station dataset.
 
         Parameters
@@ -81,30 +81,30 @@
             * A geometric object, e.g., shapely geometry
             * A filename or URL, a file-like object opened in binary ('rb') mode, or a
               Path object that will be passed to `geopandas.read_file`.
         """
         self.region = _process_region_arg(
             region=region, geocode_to_gdf_kws=geocode_to_gdf_kws
         ).to_crs(self.CRS)
-        if station_id_name is None:
-            station_id_name = settings.STATION_ID_NAME
-        self.station_id_name = station_id_name
+        if stations_id_name is None:
+            stations_id_name = settings.STATIONS_ID_NAME
+        self.stations_id_name = stations_id_name
         if time_name is None:
             time_name = settings.TIME_NAME
         self.time_name = time_name
 
     @property
     @abc.abstractmethod
     def CRS(self):  # pylint: disable=invalid-name
         """CRS of the data source."""
         pass
 
     @abc.abstractproperty
-    def station_gdf(self):
-        """Station geo-data frame."""
+    def stations_gdf(self):
+        """Geo-data frame with stations data."""
         pass
 
     @abc.abstractmethod
     def get_ts_df(self, *args, **kwargs):
         """
         Get time series data frame.
```

### Comparing `agrometeo_geopy-0.1.3/agrometeo/plotting.py` & `agrometeo_geopy-0.2.0/agrometeo/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,32 +135,32 @@
             set_title_kws = {}
         ax.set_title(title_label, **set_title_kws)
 
     # basemap
     if add_basemap is None:
         add_basemap = settings.PLOT_ADD_BASEMAP
     if add_basemap:
-        if cx is None:
-            logging.warning(
-                """
-The `add_basemap=True` option requires the contextily package. You can install it using
-conda or pip. See https://github.com/geopandas/contextily.
-"""
-            )
-
         # add_basemap arguments
         if add_basemap_kws is None:
             _add_basemap_kws = {}
         else:
             _add_basemap_kws = add_basemap_kws.copy()
         # _add_basemap_kws = {key: add_basemap_kws[key] for key in add_basemap_kws}
         if attribution is None:
             attribution = _add_basemap_kws.pop("attribution", settings.PLOT_ATTRIBUTION)
-        # add basemap
-        cx.add_basemap(
-            ax=ax,
-            crs=ts_gdf.crs,
-            attribution=attribution,
-            **_add_basemap_kws,
-        )
+        if cx is None:
+            logging.warning(
+                """
+The `add_basemap=True` option requires the contextily package. You can install it using
+conda or pip. See https://github.com/geopandas/contextily.
+"""
+            )
+        else:
+            # add basemap
+            cx.add_basemap(
+                ax=ax,
+                crs=ts_gdf.crs,
+                attribution=attribution,
+                **_add_basemap_kws,
+            )
 
     return ax
```

