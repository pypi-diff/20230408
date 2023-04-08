# Comparing `tmp/d3blocks-1.2.8.tar.gz` & `tmp/d3blocks-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d3blocks-1.2.8.tar", last modified: Fri Jan 20 16:29:25 2023, max compression
+gzip compressed data, was "d3blocks-1.2.9.tar", last modified: Fri Mar 10 13:13:17 2023, max compression
```

## Comparing `d3blocks-1.2.8.tar` & `d3blocks-1.2.9.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.288818 d3blocks-1.2.8/
--rw-rw-rw-   0        0        0    35837 2022-09-16 10:26:19.000000 d3blocks-1.2.8/LICENSE
--rw-rw-rw-   0        0        0      340 2023-01-18 18:48:46.000000 d3blocks-1.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     7585 2023-01-20 16:29:25.288818 d3blocks-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     7036 2023-01-16 08:10:19.000000 d3blocks-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.205067 d3blocks-1.2.8/d3blocks/
--rw-rw-rw-   0        0        0     1155 2023-01-19 20:26:57.000000 d3blocks-1.2.8/d3blocks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.216036 d3blocks-1.2.8/d3blocks/chord/
--rw-rw-rw-   0        0        0    12585 2023-01-19 15:36:50.000000 d3blocks-1.2.8/d3blocks/chord/Chord.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/chord/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.219152 d3blocks-1.2.8/d3blocks/chord/d3js/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/chord/d3js/__init__.py
--rw-rw-rw-   0        0        0     1000 2022-10-16 08:41:27.000000 d3blocks-1.2.8/d3blocks/chord/d3js/chord.html.j2
--rw-rw-rw-   0        0        0    59483 2022-10-16 11:19:33.000000 d3blocks-1.2.8/d3blocks/chord/d3js/chord.js
--rw-rw-rw-   0        0        0   107053 2023-01-20 16:28:07.000000 d3blocks-1.2.8/d3blocks/d3blocks.py
--rw-rw-rw-   0        0        0    64914 2023-01-20 16:16:26.000000 d3blocks-1.2.8/d3blocks/examples.py
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.220145 d3blocks-1.2.8/d3blocks/heatmap/
--rw-rw-rw-   0        0        0     9680 2023-01-19 15:38:07.000000 d3blocks-1.2.8/d3blocks/heatmap/Heatmap.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/heatmap/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.233133 d3blocks-1.2.8/d3blocks/heatmap/d3js/
--rw-rw-rw-   0        0        0        0 2020-11-17 20:33:44.000000 d3blocks-1.2.8/d3blocks/heatmap/d3js/__init__.py
--rw-rw-rw-   0        0        0    19831 2023-01-18 19:37:38.000000 d3blocks-1.2.8/d3blocks/heatmap/d3js/d3.scale.chromatic.v1.min.js
--rw-rw-rw-   0        0        0   978290 2020-11-17 20:33:44.000000 d3blocks-1.2.8/d3blocks/heatmap/d3js/d3.v4.js
--rw-rw-rw-   0        0        0   124409 2023-01-17 11:55:33.000000 d3blocks-1.2.8/d3blocks/heatmap/d3js/heatmap.html.j2
--rw-rw-rw-   0        0        0     4212 2023-01-18 11:20:35.000000 d3blocks-1.2.8/d3blocks/heatmap/d3js/matrix.html.j2
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.234130 d3blocks-1.2.8/d3blocks/imageslider/
--rw-rw-rw-   0        0        0     8308 2023-01-19 15:40:30.000000 d3blocks-1.2.8/d3blocks/imageslider/Imageslider.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/imageslider/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.240509 d3blocks-1.2.8/d3blocks/imageslider/d3js/
--rw-rw-rw-   0        0        0        0 2022-09-22 13:52:17.000000 d3blocks-1.2.8/d3blocks/imageslider/d3js/.keep
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/imageslider/d3js/__init__.py
--rw-rw-rw-   0        0        0     1666 2022-09-18 11:05:56.000000 d3blocks-1.2.8/d3blocks/imageslider/d3js/imageslider.html.j2
--rw-rw-rw-   0        0        0   247351 2022-07-13 19:24:39.000000 d3blocks-1.2.8/d3blocks/imageslider/d3js/jquery-2.1.1.js
--rw-rw-rw-   0        0        0     5426 2022-07-13 19:24:39.000000 d3blocks-1.2.8/d3blocks/imageslider/d3js/main.js
--rw-rw-rw-   0        0        0    51351 2022-07-13 19:24:39.000000 d3blocks-1.2.8/d3blocks/imageslider/d3js/modernizr.js
--rw-rw-rw-   0        0        0      947 2022-07-13 21:41:56.000000 d3blocks-1.2.8/d3blocks/imageslider/d3js/reset.css
--rw-rw-rw-   0        0        0     4116 2022-07-13 21:41:49.000000 d3blocks-1.2.8/d3blocks/imageslider/d3js/style.css
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.241510 d3blocks-1.2.8/d3blocks/matrix/
--rw-rw-rw-   0        0        0     9064 2023-01-19 15:39:23.000000 d3blocks-1.2.8/d3blocks/matrix/Matrix.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/matrix/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.245184 d3blocks-1.2.8/d3blocks/matrix/d3js/
--rw-rw-rw-   0        0        0        0 2020-11-17 20:33:44.000000 d3blocks-1.2.8/d3blocks/matrix/d3js/__init__.py
--rw-rw-rw-   0        0        0    19831 2020-11-17 20:33:44.000000 d3blocks-1.2.8/d3blocks/matrix/d3js/d3.scale.chromatic.v1.min.js
--rw-rw-rw-   0        0        0   978290 2020-11-17 20:33:44.000000 d3blocks-1.2.8/d3blocks/matrix/d3js/d3.v4.js
--rw-rw-rw-   0        0        0     4122 2023-01-18 19:44:22.000000 d3blocks-1.2.8/d3blocks/matrix/d3js/matrix.html.j2
--rw-rw-rw-   0        0        0     3982 2023-01-18 19:36:40.000000 d3blocks-1.2.8/d3blocks/matrix/d3js/matrix.html.j2.new
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.247178 d3blocks-1.2.8/d3blocks/movingbubbles/
--rw-rw-rw-   0        0        0    24189 2023-01-20 16:14:32.000000 d3blocks-1.2.8/d3blocks/movingbubbles/Movingbubbles.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/movingbubbles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.250169 d3blocks-1.2.8/d3blocks/movingbubbles/d3js/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/movingbubbles/d3js/__init__.py
--rw-rw-rw-   0        0        0   151125 2022-04-02 10:57:29.000000 d3blocks-1.2.8/d3blocks/movingbubbles/d3js/d3-3-5-5.min.js
--rw-rw-rw-   0        0        0    10470 2023-01-20 12:57:52.000000 d3blocks-1.2.8/d3blocks/movingbubbles/d3js/movingbubbles.html.j2
--rw-rw-rw-   0        0        0     1901 2022-04-24 13:58:40.000000 d3blocks-1.2.8/d3blocks/movingbubbles/d3js/style.css
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.250978 d3blocks-1.2.8/d3blocks/particles/
--rw-rw-rw-   0        0        0     2998 2023-01-19 15:40:03.000000 d3blocks-1.2.8/d3blocks/particles/Particles.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/particles/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.254166 d3blocks-1.2.8/d3blocks/particles/d3js/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/particles/d3js/__init__.py
--rw-rw-rw-   0        0        0    19831 2022-09-07 21:21:56.000000 d3blocks-1.2.8/d3blocks/particles/d3js/d3-scale-chromatic.v1.min.js
--rw-rw-rw-   0        0        0   221957 2022-05-09 15:15:54.000000 d3blocks-1.2.8/d3blocks/particles/d3js/d3.v4.min.js
--rw-rw-rw-   0        0        0     6558 2022-10-19 19:55:00.000000 d3blocks-1.2.8/d3blocks/particles/d3js/particles.html.j2
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.263142 d3blocks-1.2.8/d3blocks/sankey/
--rw-rw-rw-   0        0        0     9014 2023-01-19 15:40:47.000000 d3blocks-1.2.8/d3blocks/sankey/Sankey.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/sankey/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.265137 d3blocks-1.2.8/d3blocks/sankey/d3js/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/sankey/d3js/__init__.py
--rw-rw-rw-   0        0        0     3634 2023-01-19 20:24:54.000000 d3blocks-1.2.8/d3blocks/sankey/d3js/sankey.html.j2
--rw-rw-rw-   0        0        0    73109 2022-08-27 15:02:46.000000 d3blocks-1.2.8/d3blocks/sankey/d3js/sankey.js
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.266134 d3blocks-1.2.8/d3blocks/scatter/
--rw-rw-rw-   0        0        0    14847 2023-01-19 15:44:33.000000 d3blocks-1.2.8/d3blocks/scatter/Scatter.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/scatter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.269126 d3blocks-1.2.8/d3blocks/scatter/d3js/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/scatter/d3js/__init__.py
--rw-rw-rw-   0        0        0   221957 2022-05-09 15:15:54.000000 d3blocks-1.2.8/d3blocks/scatter/d3js/d3.v4.min.js
--rw-rw-rw-   0        0        0     6774 2022-10-19 19:55:06.000000 d3blocks-1.2.8/d3blocks/scatter/d3js/scatter.html.j2
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.272118 d3blocks-1.2.8/d3blocks/tests/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/tests/__init__.py
--rw-rw-rw-   0        0        0    17320 2023-01-19 15:53:44.000000 d3blocks-1.2.8/d3blocks/tests/test_d3blocks.py
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.274578 d3blocks-1.2.8/d3blocks/timeseries/
--rw-rw-rw-   0        0        0     9363 2023-01-19 15:41:31.000000 d3blocks-1.2.8/d3blocks/timeseries/Timeseries.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/timeseries/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.279843 d3blocks-1.2.8/d3blocks/timeseries/d3js/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/timeseries/d3js/__init__.py
--rw-rw-rw-   0        0        0   337945 2022-04-21 07:39:27.000000 d3blocks-1.2.8/d3blocks/timeseries/d3js/d3.v3.js
--rw-rw-rw-   0        0        0    15492 2022-09-13 20:40:47.000000 d3blocks-1.2.8/d3blocks/timeseries/d3js/script.js
--rw-rw-rw-   0        0        0      735 2022-04-24 13:58:40.000000 d3blocks-1.2.8/d3blocks/timeseries/d3js/style.css
--rw-rw-rw-   0        0        0      864 2022-09-18 11:17:26.000000 d3blocks-1.2.8/d3blocks/timeseries/d3js/timeseries.html.j2
--rw-rw-rw-   0        0        0    11203 2023-01-20 12:56:28.000000 d3blocks-1.2.8/d3blocks/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.281837 d3blocks-1.2.8/d3blocks/violin/
--rw-rw-rw-   0        0        0    10389 2023-01-19 15:41:41.000000 d3blocks-1.2.8/d3blocks/violin/Violin.py
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/violin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.287821 d3blocks-1.2.8/d3blocks/violin/d3js/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.8/d3blocks/violin/d3js/__init__.py
--rw-rw-rw-   0        0        0    19831 2022-09-01 20:28:35.000000 d3blocks-1.2.8/d3blocks/violin/d3js/d3-scale-chromatic.v1.min.js
--rw-rw-rw-   0        0        0   221957 2022-05-09 15:15:54.000000 d3blocks-1.2.8/d3blocks/violin/d3js/d3.v4.min.js
--rw-rw-rw-   0        0        0     6233 2022-09-18 11:03:45.000000 d3blocks-1.2.8/d3blocks/violin/d3js/violin.html.j2
-drwxrwxrwx   0        0        0        0 2023-01-20 16:29:25.215040 d3blocks-1.2.8/d3blocks.egg-info/
--rw-rw-rw-   0        0        0     7585 2023-01-20 16:29:24.000000 d3blocks-1.2.8/d3blocks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2600 2023-01-20 16:29:25.000000 d3blocks-1.2.8/d3blocks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-20 16:29:24.000000 d3blocks-1.2.8/d3blocks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2023-01-20 16:29:24.000000 d3blocks-1.2.8/d3blocks.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-20 16:29:24.000000 d3blocks-1.2.8/d3blocks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-20 16:29:25.288818 d3blocks-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1733 2023-01-18 11:09:58.000000 d3blocks-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.576271 d3blocks-1.2.9/
+-rw-rw-rw-   0        0        0    35837 2022-09-16 10:26:19.000000 d3blocks-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0      340 2023-01-18 18:48:46.000000 d3blocks-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     7585 2023-03-10 13:13:17.574932 d3blocks-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     7036 2023-03-10 13:03:50.000000 d3blocks-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.071745 d3blocks-1.2.9/d3blocks/
+-rw-rw-rw-   0        0        0     1155 2023-03-10 13:05:39.000000 d3blocks-1.2.9/d3blocks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.116256 d3blocks-1.2.9/d3blocks/chord/
+-rw-rw-rw-   0        0        0    12585 2023-01-19 15:36:50.000000 d3blocks-1.2.9/d3blocks/chord/Chord.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/chord/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.136169 d3blocks-1.2.9/d3blocks/chord/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/chord/d3js/__init__.py
+-rw-rw-rw-   0        0        0     1000 2022-10-16 08:41:27.000000 d3blocks-1.2.9/d3blocks/chord/d3js/chord.html.j2
+-rw-rw-rw-   0        0        0    59483 2022-10-16 11:19:33.000000 d3blocks-1.2.9/d3blocks/chord/d3js/chord.js
+-rw-rw-rw-   0        0        0   107446 2023-03-10 13:02:54.000000 d3blocks-1.2.9/d3blocks/d3blocks.py
+-rw-rw-rw-   0        0        0    66693 2023-03-10 12:57:47.000000 d3blocks-1.2.9/d3blocks/examples.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.153285 d3blocks-1.2.9/d3blocks/heatmap/
+-rw-rw-rw-   0        0        0     9977 2023-01-28 20:43:48.000000 d3blocks-1.2.9/d3blocks/heatmap/Heatmap.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/heatmap/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.179088 d3blocks-1.2.9/d3blocks/heatmap/d3js/
+-rw-rw-rw-   0        0        0        0 2020-11-17 20:33:44.000000 d3blocks-1.2.9/d3blocks/heatmap/d3js/__init__.py
+-rw-rw-rw-   0        0        0    19831 2023-01-18 19:37:38.000000 d3blocks-1.2.9/d3blocks/heatmap/d3js/d3.scale.chromatic.v1.min.js
+-rw-rw-rw-   0        0        0   978290 2020-11-17 20:33:44.000000 d3blocks-1.2.9/d3blocks/heatmap/d3js/d3.v4.js
+-rw-rw-rw-   0        0        0   124409 2023-01-17 11:55:33.000000 d3blocks-1.2.9/d3blocks/heatmap/d3js/heatmap.html.j2
+-rw-rw-rw-   0        0        0     4212 2023-01-18 11:20:35.000000 d3blocks-1.2.9/d3blocks/heatmap/d3js/matrix.html.j2
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.188025 d3blocks-1.2.9/d3blocks/imageslider/
+-rw-rw-rw-   0        0        0     8308 2023-01-19 15:40:30.000000 d3blocks-1.2.9/d3blocks/imageslider/Imageslider.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/imageslider/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.267060 d3blocks-1.2.9/d3blocks/imageslider/d3js/
+-rw-rw-rw-   0        0        0        0 2022-09-22 13:52:17.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/.keep
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/__init__.py
+-rw-rw-rw-   0        0        0     1666 2022-09-18 11:05:56.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/imageslider.html.j2
+-rw-rw-rw-   0        0        0   247351 2022-07-13 19:24:39.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/jquery-2.1.1.js
+-rw-rw-rw-   0        0        0     5426 2022-07-13 19:24:39.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/main.js
+-rw-rw-rw-   0        0        0    51351 2022-07-13 19:24:39.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/modernizr.js
+-rw-rw-rw-   0        0        0      947 2022-07-13 21:41:56.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/reset.css
+-rw-rw-rw-   0        0        0     4116 2022-07-13 21:41:49.000000 d3blocks-1.2.9/d3blocks/imageslider/d3js/style.css
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.270843 d3blocks-1.2.9/d3blocks/matrix/
+-rw-rw-rw-   0        0        0     9064 2023-01-19 15:39:23.000000 d3blocks-1.2.9/d3blocks/matrix/Matrix.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/matrix/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.299247 d3blocks-1.2.9/d3blocks/matrix/d3js/
+-rw-rw-rw-   0        0        0        0 2020-11-17 20:33:44.000000 d3blocks-1.2.9/d3blocks/matrix/d3js/__init__.py
+-rw-rw-rw-   0        0        0    19831 2020-11-17 20:33:44.000000 d3blocks-1.2.9/d3blocks/matrix/d3js/d3.scale.chromatic.v1.min.js
+-rw-rw-rw-   0        0        0   978290 2020-11-17 20:33:44.000000 d3blocks-1.2.9/d3blocks/matrix/d3js/d3.v4.js
+-rw-rw-rw-   0        0        0     4122 2023-01-18 19:44:22.000000 d3blocks-1.2.9/d3blocks/matrix/d3js/matrix.html.j2
+-rw-rw-rw-   0        0        0     3982 2023-01-18 19:36:40.000000 d3blocks-1.2.9/d3blocks/matrix/d3js/matrix.html.j2.new
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.316017 d3blocks-1.2.9/d3blocks/movingbubbles/
+-rw-rw-rw-   0        0        0    24345 2023-01-20 17:00:37.000000 d3blocks-1.2.9/d3blocks/movingbubbles/Movingbubbles.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/movingbubbles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.353660 d3blocks-1.2.9/d3blocks/movingbubbles/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/movingbubbles/d3js/__init__.py
+-rw-rw-rw-   0        0        0   151125 2022-04-02 10:57:29.000000 d3blocks-1.2.9/d3blocks/movingbubbles/d3js/d3-3-5-5.min.js
+-rw-rw-rw-   0        0        0    10475 2023-01-20 16:57:23.000000 d3blocks-1.2.9/d3blocks/movingbubbles/d3js/movingbubbles.html.j2
+-rw-rw-rw-   0        0        0     1901 2022-04-24 13:58:40.000000 d3blocks-1.2.9/d3blocks/movingbubbles/d3js/style.css
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.361636 d3blocks-1.2.9/d3blocks/particles/
+-rw-rw-rw-   0        0        0     2998 2023-01-19 15:40:03.000000 d3blocks-1.2.9/d3blocks/particles/Particles.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/particles/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.386583 d3blocks-1.2.9/d3blocks/particles/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/particles/d3js/__init__.py
+-rw-rw-rw-   0        0        0    19831 2022-09-07 21:21:56.000000 d3blocks-1.2.9/d3blocks/particles/d3js/d3-scale-chromatic.v1.min.js
+-rw-rw-rw-   0        0        0   221957 2022-05-09 15:15:54.000000 d3blocks-1.2.9/d3blocks/particles/d3js/d3.v4.min.js
+-rw-rw-rw-   0        0        0     6558 2022-10-19 19:55:00.000000 d3blocks-1.2.9/d3blocks/particles/d3js/particles.html.j2
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.411167 d3blocks-1.2.9/d3blocks/sankey/
+-rw-rw-rw-   0        0        0     9014 2023-01-19 15:40:47.000000 d3blocks-1.2.9/d3blocks/sankey/Sankey.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/sankey/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.433484 d3blocks-1.2.9/d3blocks/sankey/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/sankey/d3js/__init__.py
+-rw-rw-rw-   0        0        0     3634 2023-01-19 20:24:54.000000 d3blocks-1.2.9/d3blocks/sankey/d3js/sankey.html.j2
+-rw-rw-rw-   0        0        0    73109 2022-08-27 15:02:46.000000 d3blocks-1.2.9/d3blocks/sankey/d3js/sankey.js
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.449662 d3blocks-1.2.9/d3blocks/scatter/
+-rw-rw-rw-   0        0        0    14847 2023-01-19 15:44:33.000000 d3blocks-1.2.9/d3blocks/scatter/Scatter.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/scatter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.470646 d3blocks-1.2.9/d3blocks/scatter/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/scatter/d3js/__init__.py
+-rw-rw-rw-   0        0        0   221957 2022-05-09 15:15:54.000000 d3blocks-1.2.9/d3blocks/scatter/d3js/d3.v4.min.js
+-rw-rw-rw-   0        0        0     6774 2022-10-19 19:55:06.000000 d3blocks-1.2.9/d3blocks/scatter/d3js/scatter.html.j2
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.478839 d3blocks-1.2.9/d3blocks/tests/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/tests/__init__.py
+-rw-rw-rw-   0        0        0    17320 2023-01-19 15:53:44.000000 d3blocks-1.2.9/d3blocks/tests/test_d3blocks.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.494693 d3blocks-1.2.9/d3blocks/timeseries/
+-rw-rw-rw-   0        0        0     9363 2023-01-19 15:41:31.000000 d3blocks-1.2.9/d3blocks/timeseries/Timeseries.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/timeseries/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.543168 d3blocks-1.2.9/d3blocks/timeseries/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/timeseries/d3js/__init__.py
+-rw-rw-rw-   0        0        0   337945 2022-04-21 07:39:27.000000 d3blocks-1.2.9/d3blocks/timeseries/d3js/d3.v3.js
+-rw-rw-rw-   0        0        0    15492 2022-09-13 20:40:47.000000 d3blocks-1.2.9/d3blocks/timeseries/d3js/script.js
+-rw-rw-rw-   0        0        0      735 2022-04-24 13:58:40.000000 d3blocks-1.2.9/d3blocks/timeseries/d3js/style.css
+-rw-rw-rw-   0        0        0      864 2022-09-18 11:17:26.000000 d3blocks-1.2.9/d3blocks/timeseries/d3js/timeseries.html.j2
+-rw-rw-rw-   0        0        0    11203 2023-01-20 12:56:28.000000 d3blocks-1.2.9/d3blocks/utils.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.547089 d3blocks-1.2.9/d3blocks/violin/
+-rw-rw-rw-   0        0        0    11196 2023-03-10 12:54:49.000000 d3blocks-1.2.9/d3blocks/violin/Violin.py
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/violin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.571939 d3blocks-1.2.9/d3blocks/violin/d3js/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 d3blocks-1.2.9/d3blocks/violin/d3js/__init__.py
+-rw-rw-rw-   0        0        0    19831 2022-09-01 20:28:35.000000 d3blocks-1.2.9/d3blocks/violin/d3js/d3-scale-chromatic.v1.min.js
+-rw-rw-rw-   0        0        0   221957 2022-05-09 15:15:54.000000 d3blocks-1.2.9/d3blocks/violin/d3js/d3.v4.min.js
+-rw-rw-rw-   0        0        0     6317 2023-03-10 12:45:47.000000 d3blocks-1.2.9/d3blocks/violin/d3js/violin.html.j2
+drwxrwxrwx   0        0        0        0 2023-03-10 13:13:17.104457 d3blocks-1.2.9/d3blocks.egg-info/
+-rw-rw-rw-   0        0        0     7585 2023-03-10 13:13:15.000000 d3blocks-1.2.9/d3blocks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2600 2023-03-10 13:13:16.000000 d3blocks-1.2.9/d3blocks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-10 13:13:15.000000 d3blocks-1.2.9/d3blocks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-03-10 13:13:16.000000 d3blocks-1.2.9/d3blocks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-03-10 13:13:16.000000 d3blocks-1.2.9/d3blocks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-10 13:13:17.576271 d3blocks-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1696 2023-01-28 20:41:18.000000 d3blocks-1.2.9/setup.py
```

### Comparing `d3blocks-1.2.8/LICENSE` & `d3blocks-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/PKG-INFO` & `d3blocks-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: d3blocks
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python package d3blocks
 Home-page: https://github.com/d3blocks/d3blocks
-Download-URL: https://github.com/d3blocks/d3blocks/archive/1.2.8.tar.gz
+Download-URL: https://github.com/d3blocks/d3blocks/archive/1.2.9.tar.gz
 Author: Erdogan Taskesen, Oliver Verver
 Author-email: erdogant@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 [![LOC](https://sloc.xyz/github/d3blocks/d3blocks/?category=code)](https://github.com/d3blocks/d3blocks/)
 [![Downloads](https://static.pepy.tech/personalized-badge/d3blocks?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/month)](https://pepy.tech/project/d3blocks)
 [![Downloads](https://static.pepy.tech/personalized-badge/d3blocks?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/d3blocks)
 [![License](https://img.shields.io/badge/license-GPL3-green.svg)](https://github.com/d3blocks/d3blocks/blob/master/LICENSE)
 [![Forks](https://img.shields.io/github/forks/d3blocks/d3blocks.svg)](https://github.com/d3blocks/d3blocks/network)
 [![Open Issues](https://img.shields.io/github/issues/d3blocks/d3blocks.svg)](https://github.com/d3blocks/d3blocks/issues)
 [![Project Status](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
-[![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#medium-blog)
+[![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#medium-blog)
 ![GitHub Repo stars](https://img.shields.io/github/stars/d3blocks/d3blocks)
 ![GitHub repo size](https://img.shields.io/github/repo-size/d3blocks/d3blocks)
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#colab-notebook)
 [![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#)
 
 -------------------------------------------------------------------------
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: d3blocks Version: 1.2.8 Summary: Python package
+Metadata-Version: 2.1 Name: d3blocks Version: 1.2.9 Summary: Python package
 d3blocks Home-page: https://github.com/d3blocks/d3blocks Download-URL: https://
-github.com/d3blocks/d3blocks/archive/1.2.8.tar.gz Author: Erdogan Taskesen,
+github.com/d3blocks/d3blocks/archive/1.2.9.tar.gz Author: Erdogan Taskesen,
 Oliver Verver Author-email: erdogant@gmail.com License: UNKNOWN Platform:
 UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved Classifier: Operating System :: OS Independent Requires-Python:
 >=3 Description-Content-Type: text/markdown License-File: LICENSE
            [https://github.com/d3blocks/d3blocks/blob/main/logo.png]
 [![Python](https://img.shields.io/pypi/pyversions/d3blocks)](https://
 img.shields.io/pypi/pyversions/d3blocks) [![Pypi](https://img.shields.io/pypi/
@@ -20,15 +20,15 @@
 (https://pepy.tech/project/d3blocks) [![License](https://img.shields.io/badge/
 license-GPL3-green.svg)](https://github.com/d3blocks/d3blocks/blob/master/
 LICENSE) [![Forks](https://img.shields.io/github/forks/d3blocks/d3blocks.svg)]
 (https://github.com/d3blocks/d3blocks/network) [![Open Issues](https://
 img.shields.io/github/issues/d3blocks/d3blocks.svg)](https://github.com/
 d3blocks/d3blocks/issues) [![Project Status](http://www.repostatus.org/badges/
 latest/active.svg)](http://www.repostatus.org/#active) [![Medium](https://
-img.shields.io/badge/Medium-Blog-green)](https://d3blocks.github.io/d3blocks/
+img.shields.io/badge/Medium-Blog-black)](https://d3blocks.github.io/d3blocks/
 pages/html/Documentation.html#medium-blog) ![GitHub Repo stars](https://
 img.shields.io/github/stars/d3blocks/d3blocks) ![GitHub repo size](https://
 img.shields.io/github/repo-size/d3blocks/d3blocks) [![Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://d3blocks.github.io/
 d3blocks/pages/html/Documentation.html#colab-notebook) [![Donate](https://
 img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)]
 (https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#) ----------
```

### Comparing `d3blocks-1.2.8/README.md` & `d3blocks-1.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [![LOC](https://sloc.xyz/github/d3blocks/d3blocks/?category=code)](https://github.com/d3blocks/d3blocks/)
 [![Downloads](https://static.pepy.tech/personalized-badge/d3blocks?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/month)](https://pepy.tech/project/d3blocks)
 [![Downloads](https://static.pepy.tech/personalized-badge/d3blocks?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/d3blocks)
 [![License](https://img.shields.io/badge/license-GPL3-green.svg)](https://github.com/d3blocks/d3blocks/blob/master/LICENSE)
 [![Forks](https://img.shields.io/github/forks/d3blocks/d3blocks.svg)](https://github.com/d3blocks/d3blocks/network)
 [![Open Issues](https://img.shields.io/github/issues/d3blocks/d3blocks.svg)](https://github.com/d3blocks/d3blocks/issues)
 [![Project Status](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
-[![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#medium-blog)
+[![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#medium-blog)
 ![GitHub Repo stars](https://img.shields.io/github/stars/d3blocks/d3blocks)
 ![GitHub repo size](https://img.shields.io/github/repo-size/d3blocks/d3blocks)
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#colab-notebook)
 [![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#)
 
 -------------------------------------------------------------------------
```

#### html2text {}

```diff
@@ -13,15 +13,15 @@
 (https://pepy.tech/project/d3blocks) [![License](https://img.shields.io/badge/
 license-GPL3-green.svg)](https://github.com/d3blocks/d3blocks/blob/master/
 LICENSE) [![Forks](https://img.shields.io/github/forks/d3blocks/d3blocks.svg)]
 (https://github.com/d3blocks/d3blocks/network) [![Open Issues](https://
 img.shields.io/github/issues/d3blocks/d3blocks.svg)](https://github.com/
 d3blocks/d3blocks/issues) [![Project Status](http://www.repostatus.org/badges/
 latest/active.svg)](http://www.repostatus.org/#active) [![Medium](https://
-img.shields.io/badge/Medium-Blog-green)](https://d3blocks.github.io/d3blocks/
+img.shields.io/badge/Medium-Blog-black)](https://d3blocks.github.io/d3blocks/
 pages/html/Documentation.html#medium-blog) ![GitHub Repo stars](https://
 img.shields.io/github/stars/d3blocks/d3blocks) ![GitHub repo size](https://
 img.shields.io/github/repo-size/d3blocks/d3blocks) [![Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://d3blocks.github.io/
 d3blocks/pages/html/Documentation.html#colab-notebook) [![Donate](https://
 img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)]
 (https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#) ----------
```

### Comparing `d3blocks-1.2.8/d3blocks/__init__.py` & `d3blocks-1.2.9/d3blocks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from d3blocks.d3blocks import D3Blocks
 
 __author__ = 'Erdogan Taskesen, Oliver Verver'
 __email__ = 'erdogant@gmail.com, mail@oliver3.nl'
-__version__ = '1.2.8'
+__version__ = '1.2.9'
 
 # module level doc-string
 __doc__ = """
 d3blocks
 =====================================================================
 
 Description
```

### Comparing `d3blocks-1.2.8/d3blocks/chord/Chord.py` & `d3blocks-1.2.9/d3blocks/chord/Chord.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/chord/d3js/chord.html.j2` & `d3blocks-1.2.9/d3blocks/chord/d3js/chord.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/chord/d3js/chord.js` & `d3blocks-1.2.9/d3blocks/chord/d3js/chord.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/d3blocks.py` & `d3blocks-1.2.9/d3blocks/d3blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 logger = logging.getLogger('')
 for handler in logger.handlers[:]:  # get rid of existing old handlers
     logger.removeHandler(handler)
 console = logging.StreamHandler()
 formatter = logging.Formatter('[d3blocks] >%(levelname)s> %(message)s')
 console.setFormatter(formatter)
 logger.addHandler(console)
-logger = logging.getLogger()
+logger = logging.getLogger(__name__)
 
 
 class D3Blocks():
     """D3Blocks.
 
     Parameters
     ----------
@@ -217,14 +217,15 @@
                size=5,
                color=None,
                x_order=None,
                opacity=0.6,
                stroke='#000000',
                tooltip=None,
                cmap='inferno',
+               fontsize=12,
                bins=50,
                ylim=[None, None],
                title='Violin - D3blocks',
                filepath='violin.html',
                figsize=[None, None],
                showfig=True,
                overwrite=True,
@@ -260,14 +261,16 @@
             Edgecolor of dot in hex colors.
                 * '#000000' : Edge colors are all black.
         tooltip: list of labels with same size as (x,y)
             labels of the samples.
         cmap : String, (default: 'inferno')
             All colors can be reversed with '_r', e.g. 'binary' to 'binary_r'
                 * 'Set1', 'Set2', 'rainbow', 'bwr', 'binary', 'seismic', 'Blues', 'Reds', 'Pastel1', 'Paired', 'twilight', 'hsv'
+        fontsize : int, optional (default: 12)
+            Text fontsize.
         bins : Int (default: 50)
             The bin size is the 'resolution' of the violin plot.
         ylim : tuple, (default: [None, None])
             Limit the width of the y-axis [min, max].
                 *  [None, None] : The width is determined based on the min-max value range.
         title : String, (default: None)
             Title of the figure.
@@ -311,19 +314,22 @@
         >>> from d3blocks import D3Blocks
         >>> #
         >>> # Initialize
         >>> d3 = D3Blocks()
         >>> #
         >>> # Import example dataset
         >>> df = d3.import_example('cancer')
+        >>> #
         >>> # Set some input variables.
         >>> tooltip = df['labels'].values + ' <br /> Survival: ' + df['survival_months'].astype(str).values
+        >>> fontsize = df['age'].values
+        >>> # fontsize = 16  # Set one fontsize for all nodes
         >>> #
         >>> # Create the chart
-        >>> d3.violin(x=df['labels'].values, y=df['age'].values, tooltip=tooltip, bins=50, size=df['survival_months'].values/10, x_order=['acc','kich', 'brca','lgg','blca','coad','ov'], filepath='violine.html', figsize=[900, None])
+        >>> d3.violin(x=df['labels'].values, y=df['age'].values, fontsize=fontsize, tooltip=tooltip, bins=50, size=df['survival_months'].values/10, x_order=['acc','kich', 'brca','lgg','blca','coad','ov'], filepath='violine.html', figsize=[900, None])
         >>> #
 
         Examples
         --------
         >>> # Load d3blocks
         >>> from d3blocks import D3Blocks
         >>> #
@@ -336,14 +342,15 @@
         >>> # Set the properties by providing the labels
         >>> d3.set_edge_properties(x=df['labels'].values, y=df['age'].values, size=df['survival_months'].values/10, x_order=['acc','kich', 'brca','lgg','blca','coad','ov'])
         >>> #
         >>> # Set specific node properties.
         >>> d3.edge_properties.loc[0,'size']=50
         >>> d3.edge_properties.loc[0,'color']='#000000'
         >>> d3.edge_properties.loc[0,'tooltip']='I am adjusted!'
+        >>> d3.edge_properties.loc[0,'fontsize']=30
         >>> #
         >>> # Configuration can be changed too.
         >>> print(d3.config)
         >>> #
         >>> # Show the chart
         >>> d3.show()
 
@@ -353,17 +360,17 @@
 
         """
         # Cleaning
         self._clean(clean_config=reset_properties, logger=logger)
         # Store chart
         self.chart = set_chart_func('Violin', logger)
         # Store properties
-        self.config = self.chart.set_config(config=self.config, filepath=filepath, title=title, showfig=showfig, overwrite=overwrite, figsize=figsize, cmap=cmap, bins=bins, ylim=ylim, x_order=x_order, reset_properties=reset_properties, notebook=notebook, logger=logger)
+        self.config = self.chart.set_config(config=self.config, filepath=filepath, title=title, showfig=showfig, overwrite=overwrite, figsize=figsize, cmap=cmap, bins=bins, ylim=ylim, x_order=x_order, reset_properties=reset_properties, notebook=notebook, fontsize=fontsize, logger=logger)
         # Remvove quotes from source-target node_properties
-        self.edge_properties = self.chart.set_edge_properties(x, y, config=self.config, color=color, size=size, stroke=stroke, opacity=opacity, tooltip=tooltip, cmap=self.config['cmap'], x_order=self.config['x_order'], logger=logger)
+        self.edge_properties = self.chart.set_edge_properties(x, y, config=self.config, color=color, size=size, stroke=stroke, opacity=opacity, tooltip=tooltip, cmap=self.config['cmap'], x_order=self.config['x_order'], fontsize=self.config['fontsize'], logger=logger)
         # Set default label properties
         if self.config['reset_properties'] or (not hasattr(self, 'node_properties')):
             self.set_node_properties(np.unique(self.edge_properties['x'].values), cmap=self.config['cmap'])
         # Create the plot
         return self.show()
 
     def scatter(self,
@@ -1007,15 +1014,15 @@
     def movingbubbles(self,
                       df,
                       datetime: str = 'datetime',
                       sample_id: str = 'sample_id',
                       state: str = 'state',
                       center: str = None,
                       size=5,
-                      color='#808080',
+                      color=None,
                       cmap: str = 'Set1',
                       color_method: str = 'state',
                       dt_format: str = '%d-%m-%Y %H:%M:%S',
                       damper: float = 1,
                       fontsize: int = 14,
                       timedelta: str = 'minutes',
                       standardize: str = 'samplewise',
@@ -1057,14 +1064,15 @@
             Size the nodes by specifying per sample_id the size.
                 * 5: set all nodes this this size
                 * {'0': 4, '1': 10, '2': 5, ..}: Specify size for each sample_id
         color: int or dictionary. (default: '#808080') or {sample_id i: hex-color}
             Color the nodes by specifying per sample_id the color.
                 * '#000FFF': set all nodes to this color.
                 * {'0': '#808080', '1': '#FFF000', '3': '#000000', ..}: Specify color for each sample_id
+                * None: Colors are based on sample_id using the cmap.
         color_method : str
             Coloring of the nodes.
                 * 'state': Use the colors defined per state as (d3.node_properties).
                 * 'node': Use the colors defined in the dataframe (d3.edge_properties).
         dt_format : str
             Date time format.
                 * '%d-%m-%Y %H:%M:%S'.
@@ -1440,19 +1448,17 @@
         >>> # Load example data
         >>> df = d3.import_example('stormofswords')  # 'energy'
         >>> df = d3.vec2adjmat(df['source'], df['target'], weight=df['weight'], symmetric=True)
         >>> #
         >>> # Plot
         >>> d3.heatmap(df)
         >>> #
-        >>> #
 
         Examples
         --------
-        >>> #
         >>> # Initialize
         >>> d3 = D3Blocks()
         >>> #
         >>> # Load example data
         >>> df = d3.import_example('bigbang')
         >>> df = d3.vec2adjmat(df['source'], df['target'], weight=df['weight'])
         >>> #
```

### Comparing `d3blocks-1.2.8/d3blocks/examples.py` & `d3blocks-1.2.9/d3blocks/examples.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,75 @@
 # %%
 # import d3blocks
 # print(dir(d3blocks))
 # print(d3blocks.__version__)
 import pandas as pd
 import numpy as np
 
+# %% VIOLIN - EXAMPLE
+from d3blocks import D3Blocks
+
+# Initialize
+d3 = D3Blocks()
+
+# Import example dataset
+df = d3.import_example('cancer')
+
+# Set some input variables.
+tooltip = df['labels'].values + ' <br /> Survival: ' + df['survival_months'].astype(str).values
+fontsize = df['survival_months'].values/10
+
+# Create the chart
+d3.violin(x=df['labels'].values,
+          y=df['age'].values,
+          fontsize=fontsize,
+          tooltip=tooltip,
+          bins=50,
+          size=df['survival_months'].values/10,
+          x_order=['acc','kich', 'brca','lgg','blca','coad','ov'],
+          filepath=r'c:\temp\violine.html', figsize=[900, None])
+
+
+from d3blocks import D3Blocks
+# Initialize
+d3 = D3Blocks(chart='Violin', frame=True)
+# Import example
+df = d3.import_example('cancer')
+# Edge properties
+tooltip = df['labels'].values + ' <br /> Survival: ' + df['survival_months'].astype(str).values
+d3.set_edge_properties(x=df['labels'].values,
+                        y=df['age'].values,
+                        fontsize=16,
+                        tooltip=tooltip,
+                        size=df['survival_months'].values/10,
+                        x_order=['acc','kich', 'brca','lgg','blca','coad','ov'],
+                        filepath='violine_demo.html')
+# d3.edge_properties
+d3.show(filepath='c://temp//violin1.html')
+
+
+
+
+# %%
+from d3blocks import D3Blocks
+
+# Initialize
+d3 = D3Blocks(verbose=10)
+# Import example
+df = d3.import_example('energy')
+html = d3.chord(df, filepath=None, notebook=True)
+
+# Link settings
+# d3.chord(df, filepath=None, color='target', showfig=False)
+# html = d3.chord(df, filepath=None, showfig=True)
+
+
+d3.chord(df, filepath=r'c:\temp\chord\chord.html', color='target', notebook=False)
+
+
 # %% Movingbubbles - Make manual dataset to test the working
 
 # This is an example to demonstrate standardize='samplewise'.
 # 
 
 import pandas as pd
 from d3blocks import D3Blocks
@@ -98,17 +159,17 @@
                  color=color,
                  color_method='node',
                  timedelta='minutes',
                  speed={"slow": 1000, "medium": 200, "fast": 10},
                  time_notes=time_notes,
                  filepath=r'c:\temp\movingbubbles.html',
                  cmap='Set2',
-                  # standardize='minimum',
-                   # standardize='samplewise',
-                   standardize='relative',
+                 # standardize='minimum',
+                  standardize='samplewise',
+                 # standardize='relative',
                  )
 
 df1=d3.edge_properties
 
 
 # %% Moving bubbles
 from d3blocks import D3Blocks
```

### Comparing `d3blocks-1.2.8/d3blocks/heatmap/Heatmap.py` & `d3blocks-1.2.9/d3blocks/heatmap/Heatmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 License     : GPL3
 """
 from ismember import ismember
 import colourmap
 import numpy as np
 import os
 from shutil import copyfile
-from clusteval import clusteval
 
 try:
     from .. utils import set_path, set_labels, write_html_file
 except:
     from utils import set_path, set_labels, write_html_file
 
 
@@ -104,19 +103,32 @@
     # Create the html file
     html = write_html(json_data, config, logger)
     # Return html
     return html
 
 
 def color_on_clusterlabel(adjmat, df, node_properties, config, logger):
+    """Color in clusterlabel.
+
+    Returns
+    -------
+    node_properties : array-like
+        Node properties.
+
+    """
     # Default is all cluster labels are the same
     node_properties['classlabel'] = np.zeros(node_properties.shape[0]).astype(int)
 
     if config['classlabel']=='cluster':
         # Cluster the nodes
+        try:
+            from clusteval import clusteval
+        except:
+            raise Exception('clusteval needs to be pip installed first. Tip: pip install clusteval')
+        # Initialize
         ce = clusteval(**config['cluster_params'])
         results = ce.fit(adjmat.values)
         Iloc, idx = ismember(node_properties['label'].values, adjmat.index.values)
         if np.any(~Iloc):
             logger.error('Feature name(s): %s can not be used. Hint: Remove special characters. <return>' %(df.index.values[~np.isin(np.arange(0, df.shape[0]), idx)]))
             return None
         node_properties['classlabel'] = np.zeros(node_properties.shape[0]).astype(int)
```

### Comparing `d3blocks-1.2.8/d3blocks/heatmap/d3js/d3.scale.chromatic.v1.min.js` & `d3blocks-1.2.9/d3blocks/heatmap/d3js/d3.scale.chromatic.v1.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/heatmap/d3js/d3.v4.js` & `d3blocks-1.2.9/d3blocks/heatmap/d3js/d3.v4.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/heatmap/d3js/heatmap.html.j2` & `d3blocks-1.2.9/d3blocks/heatmap/d3js/heatmap.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/heatmap/d3js/matrix.html.j2` & `d3blocks-1.2.9/d3blocks/heatmap/d3js/matrix.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/imageslider/Imageslider.py` & `d3blocks-1.2.9/d3blocks/imageslider/Imageslider.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/imageslider/d3js/imageslider.html.j2` & `d3blocks-1.2.9/d3blocks/imageslider/d3js/imageslider.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/imageslider/d3js/jquery-2.1.1.js` & `d3blocks-1.2.9/d3blocks/imageslider/d3js/jquery-2.1.1.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/imageslider/d3js/main.js` & `d3blocks-1.2.9/d3blocks/imageslider/d3js/main.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/imageslider/d3js/modernizr.js` & `d3blocks-1.2.9/d3blocks/imageslider/d3js/modernizr.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/imageslider/d3js/reset.css` & `d3blocks-1.2.9/d3blocks/imageslider/d3js/reset.css`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/imageslider/d3js/style.css` & `d3blocks-1.2.9/d3blocks/imageslider/d3js/style.css`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/matrix/Matrix.py` & `d3blocks-1.2.9/d3blocks/matrix/Matrix.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/matrix/d3js/d3.scale.chromatic.v1.min.js` & `d3blocks-1.2.9/d3blocks/matrix/d3js/d3.scale.chromatic.v1.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/matrix/d3js/d3.v4.js` & `d3blocks-1.2.9/d3blocks/matrix/d3js/d3.v4.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/matrix/d3js/matrix.html.j2` & `d3blocks-1.2.9/d3blocks/matrix/d3js/matrix.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/matrix/d3js/matrix.html.j2.new` & `d3blocks-1.2.9/d3blocks/matrix/d3js/matrix.html.j2.new`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/movingbubbles/Movingbubbles.py` & `d3blocks-1.2.9/d3blocks/movingbubbles/Movingbubbles.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,16 @@
     """
     datetime = kwargs.get('datetime', 'datetime')
     sample_id = kwargs.get('sample_id', 'sample_id')
     state = kwargs.get('state', 'state')
     method = kwargs.get('standardize', None)
     timedelta = kwargs.get('timedelta', None)
     size = kwargs.get('size', 4)
-    color = kwargs.get('color', '#808080')
+    color = kwargs.get('color', None)
+    cmap = kwargs.get('cmap', 'Set1')
     dt_format = kwargs.get('dt_format', '%d-%m-%Y %H:%M:%S')
     logger = kwargs.get('logger', None)
     df = df.copy()
 
     # Compute delta
     if ~np.any(df.columns=='delta') and isinstance(df, pd.DataFrame) and np.any(df.columns==state) and np.any(df.columns==datetime) and np.any(df.columns==sample_id):
         if logger is not None: logger.info('Standardizing input dataframe using method: [%s].' %(method))
@@ -169,33 +170,37 @@
         df = standardize(df, method=method, sample_id=sample_id, datetime=datetime, dt_format=dt_format, minimum_time=timedelta, logger=logger)
     else:
         raise Exception(print('Can not find the specified columns: "state", "datetime", or "sample_id" columns in the input dataframe: %s' %(df.columns.values)))
 
     # Set size per node. Note that sizes are still constant per node!
     df = _set_nodesize(df, sample_id, size, logger)
     # Colol per node
-    df = _set_nodecolor(df, sample_id, color, logger)
+    df = _set_nodecolor(df, sample_id, color, cmap, logger)
     return df
 
-def _set_nodecolor(df, sample_id, color, logger):
+def _set_nodecolor(df, sample_id, color, cmap, logger):
     # Node color is set to default.
     if isinstance(color, dict):
         # add new column to df with node color for the specified sample_id
         if logger is not None: logger.info('Processing the specified in node colors in dictionary..')
         df['color'] = '#808080'
         for key in color.keys():
             df.loc[df[sample_id]==key, 'color'] = color.get(key)
 
+    if color is None:
+        df['color'] = colourmap.fromlist(df['sample_id'], cmap=cmap, scheme='hex')[0]
+
     # If the color column not exists, create one with default color
     if not np.any(np.isin(df.columns, 'color')):
         df['color'] = color
         if logger is not None: logger.info('Set all nodes to color: %s' %(color))
 
     return df
 
+
 def _set_nodesize(df, sample_id, size, logger):
     # Node size is set to default.
     if isinstance(size, dict):
         # add new column to df with node size for the specified sample_id
         if logger is not None: logger.info('Processing the specified in node sizes in dictionary..')
         df['size'] = 4
         for key in size.keys():
@@ -204,15 +209,15 @@
     # If the size column not exists, create one with default size
     if not np.any(np.isin(df.columns, 'size')):
         df['size'] = size
         if logger is not None: logger.info('Set all nodes to size: %d' %(size))
 
     return df
 
-    
+
 def show(df, **kwargs):
     """Build and show the graph.
 
     df : pd.DataFrame()
         Input dataframe.
     config : dict
         Dictionary containing configuration keys.
```

### Comparing `d3blocks-1.2.8/d3blocks/movingbubbles/d3js/d3-3-5-5.min.js` & `d3blocks-1.2.9/d3blocks/movingbubbles/d3js/d3-3-5-5.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/movingbubbles/d3js/movingbubbles.html.j2` & `d3blocks-1.2.9/d3blocks/movingbubbles/d3js/movingbubbles.html.j2`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     </div>
 
     <div id="chart"></div>
 
     <b>Color method:</b>
     	<select id="ColorOptions" onchange="link_color_changed(this.value)">
     	  <option value="STATE" {{ COLOR_STATE_SELECTED }}>State</option>
-    	  <option value="NODE" {{ COLOR_NODE_SELECTED }}>Node</option>
+    	  <option value="NODE" {{ COLOR_NODE_SELECTED }}>Sample id</option>
     </select>
     
     <div class="clr"></div>
     </div>
```

### Comparing `d3blocks-1.2.8/d3blocks/movingbubbles/d3js/style.css` & `d3blocks-1.2.9/d3blocks/movingbubbles/d3js/style.css`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/particles/Particles.py` & `d3blocks-1.2.9/d3blocks/particles/Particles.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/particles/d3js/d3-scale-chromatic.v1.min.js` & `d3blocks-1.2.9/d3blocks/particles/d3js/d3-scale-chromatic.v1.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/particles/d3js/d3.v4.min.js` & `d3blocks-1.2.9/d3blocks/particles/d3js/d3.v4.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/particles/d3js/particles.html.j2` & `d3blocks-1.2.9/d3blocks/particles/d3js/particles.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/sankey/Sankey.py` & `d3blocks-1.2.9/d3blocks/sankey/Sankey.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/sankey/d3js/sankey.html.j2` & `d3blocks-1.2.9/d3blocks/sankey/d3js/sankey.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/sankey/d3js/sankey.js` & `d3blocks-1.2.9/d3blocks/sankey/d3js/sankey.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/scatter/Scatter.py` & `d3blocks-1.2.9/d3blocks/scatter/Scatter.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/scatter/d3js/d3.v4.min.js` & `d3blocks-1.2.9/d3blocks/scatter/d3js/d3.v4.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/scatter/d3js/scatter.html.j2` & `d3blocks-1.2.9/d3blocks/scatter/d3js/scatter.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/tests/test_d3blocks.py` & `d3blocks-1.2.9/d3blocks/tests/test_d3blocks.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/timeseries/Timeseries.py` & `d3blocks-1.2.9/d3blocks/timeseries/Timeseries.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/timeseries/d3js/d3.v3.js` & `d3blocks-1.2.9/d3blocks/timeseries/d3js/d3.v3.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/timeseries/d3js/script.js` & `d3blocks-1.2.9/d3blocks/timeseries/d3js/script.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/timeseries/d3js/style.css` & `d3blocks-1.2.9/d3blocks/timeseries/d3js/style.css`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/timeseries/d3js/timeseries.html.j2` & `d3blocks-1.2.9/d3blocks/timeseries/d3js/timeseries.html.j2`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/utils.py` & `d3blocks-1.2.9/d3blocks/utils.py`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/violin/Violin.py` & `d3blocks-1.2.9/d3blocks/violin/Violin.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     logger = kwargs.get('logger', None)
     config['chart'] ='violin'
     config['title'] = kwargs.get('title', 'Violin - D3blocks')
     config['filepath'] = set_path(kwargs.get('filepath', 'violin.html'), logger)
     config['figsize'] = kwargs.get('figsize', [None, None])
     config['showfig'] = kwargs.get('showfig', True)
     config['overwrite'] = kwargs.get('overwrite', True)
+    config['fontsize'] = kwargs.get('fontsize', 12)
     config['bins'] = kwargs.get('bins', 20)
     config['cmap'] = kwargs.get('cmap', 'inferno')
     config['ylim'] = kwargs.get('ylim', [None, None])
     config['x_order'] = kwargs.get('x_order', None)
     config['reset_properties'] = kwargs.get('reset_properties', True)
     config['notebook'] = kwargs.get('notebook', False)
     # Return
@@ -87,14 +88,16 @@
         Edgecolor of dot in hex colors.
         '#000000' : Edge colors are all black.
     tooltip: list of labels with same size as (x,y)
         labels of the samples.
     cmap : String, (default: 'inferno')
         All colors can be reversed with '_r', e.g. 'binary' to 'binary_r'
         'Set1','Set2','rainbow','bwr','binary','seismic','Blues','Reds','Pastel1','Paired','twilight','hsv'
+    fontsize : int, optional (default: 12)
+        Text fontsize.
 
     Returns
     -------
     d3.edge_properties: DataFrame of dictionary
          Contains properties of the unique input edges/links.
     """
     # Collect arguments
@@ -106,28 +109,43 @@
     # Collect key-word arguments
     color = kwargs.get('color', None)
     size = kwargs.get('size', 5)
     stroke = kwargs.get('stroke', '#ffffff')
     opacity = kwargs.get('opacity', 0.8)
     tooltip = kwargs.get('tooltip', '')
     cmap = kwargs.get('cmap', 'inferno')
+    fontsize = kwargs.get('fontsize', 12)
     x_order = kwargs.get('x_order', None)
     logger = kwargs.get('logger', None)
 
     # Make checks
     if len(x)!=len(y): raise Exception(logger.error('input parameter "x" should be of size of "y".'))
     if size is None: raise Exception(logger.error('input parameter "size" should have value >0.'))
-    if isinstance(size, (list, np.ndarray)) and (len(size)!=len(x)): raise Exception(logger.error('input parameter "s" should be of same size of (x, y).'))
     if stroke is None: raise Exception(logger.error('input parameter "stroke" should have hex value.'))
-    if isinstance(stroke, (list, np.ndarray)) and (len(stroke)!=len(x)): raise Exception(logger.error('input parameter "stroke" should be of same size of (x, y).'))
     if opacity is None: raise Exception(logger.error('input parameter "opacity" should have value in range [0..1].'))
+
+    if isinstance(stroke, (list, np.ndarray)) and (len(stroke)!=len(x)): raise Exception(logger.error('input parameter "stroke" should be of same size of (x, y).'))
+    if isinstance(size, (list, np.ndarray)) and (len(size)!=len(x)): raise Exception(logger.error('input parameter "s" should be of same size of (x, y).'))
     if isinstance(opacity, (list, np.ndarray)) and (len(opacity)!=len(x)): raise Exception(logger.error('input parameter "opacity" should be of same size of (x, y).'))
+    if isinstance(fontsize, (list, np.ndarray)) and (len(fontsize)!=len(x)): raise Exception(logger.error('input parameter "fontsize" should be of same size of (x, y).'))
+
+    # Set fontsize to a minimum of 0
+    if isinstance(fontsize, (list, np.ndarray)):
+        fontsize=np.array(fontsize)
+        fontsize[np.isnan(fontsize)] = 0
+        fontsize = np.maximum(fontsize, 0)
+        fontsize = fontsize.astype(int)
+    # Set size to a minimum of 1
+    if isinstance(size, (list, np.ndarray)):
+        size = np.array(size)
+        size[np.isnan(size)] = 0
+        size = np.maximum(size, 0)
 
     # Convert to dataframe
-    df = pd.DataFrame({'x': x, 'y': y, 'color': color, 'size': size, 'stroke': stroke, 'opacity': opacity, 'tooltip': tooltip})
+    df = pd.DataFrame({'x': x, 'y': y, 'color': color, 'size': size, 'stroke': stroke, 'opacity': opacity, 'tooltip': tooltip, 'fontsize': fontsize})
 
     # Remove NaN values
     Irem = df['y'].isna()
     if np.any(Irem):
         if logger is not None: logger.info('Removing [%.0d] NaN values.' %(sum(Irem)))
         df = df.loc[~Irem, :]
 
@@ -272,10 +290,10 @@
     -------
     X : str.
         Converted data into a string that is d3 compatible.
 
     """
     df['y']=df['y'].astype(str)
     # Set x, y
-    X = df[['x', 'y', 'color', 'size', 'stroke', 'opacity', 'tooltip']].to_json(orient='records')
+    X = df[['x', 'y', 'color', 'size', 'stroke', 'opacity', 'tooltip', 'fontsize']].to_json(orient='records')
     # Return
     return X
```

### Comparing `d3blocks-1.2.8/d3blocks/violin/d3js/d3-scale-chromatic.v1.min.js` & `d3blocks-1.2.9/d3blocks/violin/d3js/d3-scale-chromatic.v1.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/violin/d3js/d3.v4.min.js` & `d3blocks-1.2.9/d3blocks/violin/d3js/d3.v4.min.js`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/d3blocks/violin/d3js/violin.html.j2` & `d3blocks-1.2.9/d3blocks/violin/d3js/violin.html.j2`

 * *Files 2% similar despite different names*

```diff
@@ -127,20 +127,22 @@
       .style("border-radius", "5px")
       .style("padding", "5px")
       .style("position", "absolute")
     
     // Three function that change the tooltip when user hover / move / leave a cell
     var mouseover = function(d) {
     Tooltip
-      .style("opacity", 1);
+      .style("opacity", 1)
+      .style("font-size", d.fontsize+"px"); // Set font size of the tooltip
     
     // Increases size of the dot with 0.5
     d3.select(this)
       .style("r",  d.size + (0.5*d.size))
-      .style("opacity", 0.8);
+      .style("opacity", 0.8)
+      ;
     }
     
     var mousemove = function(d) {
     Tooltip
       .html(d.tooltip)
     //  .html("Exact value: " + d[6])
       .style("left", (d3.mouse(this)[0]+70) + "px")
```

### Comparing `d3blocks-1.2.8/d3blocks.egg-info/PKG-INFO` & `d3blocks-1.2.9/d3blocks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: d3blocks
-Version: 1.2.8
+Version: 1.2.9
 Summary: Python package d3blocks
 Home-page: https://github.com/d3blocks/d3blocks
-Download-URL: https://github.com/d3blocks/d3blocks/archive/1.2.8.tar.gz
+Download-URL: https://github.com/d3blocks/d3blocks/archive/1.2.9.tar.gz
 Author: Erdogan Taskesen, Oliver Verver
 Author-email: erdogant@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 [![LOC](https://sloc.xyz/github/d3blocks/d3blocks/?category=code)](https://github.com/d3blocks/d3blocks/)
 [![Downloads](https://static.pepy.tech/personalized-badge/d3blocks?period=month&units=international_system&left_color=grey&right_color=brightgreen&left_text=PyPI%20downloads/month)](https://pepy.tech/project/d3blocks)
 [![Downloads](https://static.pepy.tech/personalized-badge/d3blocks?period=total&units=international_system&left_color=grey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/d3blocks)
 [![License](https://img.shields.io/badge/license-GPL3-green.svg)](https://github.com/d3blocks/d3blocks/blob/master/LICENSE)
 [![Forks](https://img.shields.io/github/forks/d3blocks/d3blocks.svg)](https://github.com/d3blocks/d3blocks/network)
 [![Open Issues](https://img.shields.io/github/issues/d3blocks/d3blocks.svg)](https://github.com/d3blocks/d3blocks/issues)
 [![Project Status](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
-[![Medium](https://img.shields.io/badge/Medium-Blog-green)](https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#medium-blog)
+[![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#medium-blog)
 ![GitHub Repo stars](https://img.shields.io/github/stars/d3blocks/d3blocks)
 ![GitHub repo size](https://img.shields.io/github/repo-size/d3blocks/d3blocks)
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#colab-notebook)
 [![Donate](https://img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)](https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#)
 
 -------------------------------------------------------------------------
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: d3blocks Version: 1.2.8 Summary: Python package
+Metadata-Version: 2.1 Name: d3blocks Version: 1.2.9 Summary: Python package
 d3blocks Home-page: https://github.com/d3blocks/d3blocks Download-URL: https://
-github.com/d3blocks/d3blocks/archive/1.2.8.tar.gz Author: Erdogan Taskesen,
+github.com/d3blocks/d3blocks/archive/1.2.9.tar.gz Author: Erdogan Taskesen,
 Oliver Verver Author-email: erdogant@gmail.com License: UNKNOWN Platform:
 UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier: License ::
 OSI Approved Classifier: Operating System :: OS Independent Requires-Python:
 >=3 Description-Content-Type: text/markdown License-File: LICENSE
            [https://github.com/d3blocks/d3blocks/blob/main/logo.png]
 [![Python](https://img.shields.io/pypi/pyversions/d3blocks)](https://
 img.shields.io/pypi/pyversions/d3blocks) [![Pypi](https://img.shields.io/pypi/
@@ -20,15 +20,15 @@
 (https://pepy.tech/project/d3blocks) [![License](https://img.shields.io/badge/
 license-GPL3-green.svg)](https://github.com/d3blocks/d3blocks/blob/master/
 LICENSE) [![Forks](https://img.shields.io/github/forks/d3blocks/d3blocks.svg)]
 (https://github.com/d3blocks/d3blocks/network) [![Open Issues](https://
 img.shields.io/github/issues/d3blocks/d3blocks.svg)](https://github.com/
 d3blocks/d3blocks/issues) [![Project Status](http://www.repostatus.org/badges/
 latest/active.svg)](http://www.repostatus.org/#active) [![Medium](https://
-img.shields.io/badge/Medium-Blog-green)](https://d3blocks.github.io/d3blocks/
+img.shields.io/badge/Medium-Blog-black)](https://d3blocks.github.io/d3blocks/
 pages/html/Documentation.html#medium-blog) ![GitHub Repo stars](https://
 img.shields.io/github/stars/d3blocks/d3blocks) ![GitHub repo size](https://
 img.shields.io/github/repo-size/d3blocks/d3blocks) [![Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://d3blocks.github.io/
 d3blocks/pages/html/Documentation.html#colab-notebook) [![Donate](https://
 img.shields.io/badge/Support%20this%20project-grey.svg?logo=github%20sponsors)]
 (https://d3blocks.github.io/d3blocks/pages/html/Documentation.html#) ----------
```

### Comparing `d3blocks-1.2.8/d3blocks.egg-info/SOURCES.txt` & `d3blocks-1.2.9/d3blocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `d3blocks-1.2.8/setup.py` & `d3blocks-1.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,14 @@
                        'colourmap>=1.1.10',
                        'jinja2',
                        'd3graph>=2.3.6',
                        'requests',
                        'ismember>=1.0.1',
                        'scikit-learn',
                        'elasticgraph>=0.1.2',
-                       'clusteval',
                        ],
      python_requires='>=3',
      name='d3blocks',
      version=new_version,
      author="Erdogan Taskesen, Oliver Verver",
      author_email="erdogant@gmail.com",
      description="Python package d3blocks",
```

