# Comparing `tmp/Pydap-3.2.2.tar.gz` & `tmp/pydap-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Pydap-3.2.2.tar", last modified: Wed May 24 22:40:12 2017, max compression
+gzip compressed data, was "pydap-3.4.0.tar", last modified: Fri Apr  7 23:16:09 2023, max compression
```

## Comparing `Pydap-3.2.2.tar` & `pydap-3.4.0.tar`

### file list

```diff
@@ -1,208 +1,146 @@
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/pydap/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     9129 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/lib.py
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/pydap/wsgi/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     6211 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/wsgi/functions.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)       56 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/wsgi/__init__.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     8255 2017-05-24 22:16:06.000000 Pydap-3.2.2/src/pydap/wsgi/app.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     6788 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/wsgi/ssf.py
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/pydap/wsgi/templates/
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/pydap/wsgi/templates/static/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1572 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/wsgi/templates/static/style.css
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     2292 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/wsgi/templates/index.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     2273 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/wsgi/templates/base.html
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/pydap/parsers/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     5102 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/parsers/__init__.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4162 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/parsers/das.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4574 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/parsers/dds.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4056 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/net.py
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/pydap/cas/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1647 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/cas/esgf.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)        0 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/cas/__init__.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      783 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/cas/urs.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     6195 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/cas/get_cookies.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      103 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/__init__.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1009 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/exceptions.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     6356 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/client.py
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/pydap/server/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)        0 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/server/__init__.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4111 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/server/devel.py
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/pydap/responses/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1560 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/responses/version.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     3126 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/responses/lib.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)       56 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/responses/__init__.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     2304 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/responses/ascii.py
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/pydap/responses/html/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     3392 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/responses/html/__init__.py
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/pydap/responses/html/templates/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     2879 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/responses/html/templates/macros.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1277 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/responses/html/templates/html.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1230 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/responses/error.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     9098 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/responses/dods.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4562 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/responses/das.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     3285 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/responses/dds.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    23419 2017-05-22 19:29:42.000000 Pydap-3.2.2/src/pydap/model.py
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/pydap/handlers/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    17549 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/handlers/lib.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)       56 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/handlers/__init__.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    15213 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/handlers/dap.py
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/pydap/handlers/netcdf/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     6224 2017-05-22 20:32:12.000000 Pydap-3.2.2/src/pydap/handlers/netcdf/__init__.py
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/pydap/tests/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     5308 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/tests/test_cas_esgf.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     7255 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/tests/datasets.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     8464 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/tests/test_lib.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     3892 2017-05-22 20:32:12.000000 Pydap-3.2.2/src/pydap/tests/test_handlers_netcdf.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    20678 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/tests/test_handlers_dap.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     2801 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_D1.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      401 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/tests/test.01.das
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     7028 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_iter_data.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)       56 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/tests/__init__.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     6445 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_wsgi_ssf.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1191 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/tests/rainfall_time_malaysia.cdp.dds
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     3045 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/tests/test_responses_lib.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    14889 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/tests/test_responses_dods.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1273 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_responses_error.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      516 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/tests/test_exceptions.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1831 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_special_chars.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     7798 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/tests/test_client.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      896 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_constrain.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4351 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_dapper.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     3021 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/tests/test_responses_dds.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)  5673697 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/tests/rainfall_time_malaysia.cdp.dods
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    18572 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_handlers_lib.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     3532 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/tests/test_responses_das.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    16695 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_model.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1430 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_responses_version.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     2778 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_responses_ascii.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     2856 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/tests/test_cas_urs.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      248 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/tests/test_pydap.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      263 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/tests/test.01.dods
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     6411 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_parsers.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4117 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/tests/test_parsers_dds.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1466 2017-05-12 16:13:00.000000 Pydap-3.2.2/src/pydap/tests/rainfall_time_malaysia.cdp.das
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      480 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_webtest.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     2063 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_parsers_das.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     3544 2017-05-24 04:46:14.000000 Pydap-3.2.2/src/pydap/tests/test_server_devel.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     3802 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_wsgi_app.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     5413 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_responses_html.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1665 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_net.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    15744 2017-05-22 19:27:13.000000 Pydap-3.2.2/src/pydap/tests/test_wsgi_functions.py
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/Pydap.egg-info/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     6151 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/Pydap.egg-info/SOURCES.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)       49 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/Pydap.egg-info/namespace_packages.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)        1 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/Pydap.egg-info/dependency_links.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)        6 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/Pydap.egg-info/top_level.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      508 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/Pydap.egg-info/requires.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      699 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/Pydap.egg-info/entry_points.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)        1 2016-10-19 21:47:20.000000 Pydap-3.2.2/src/Pydap.egg-info/not-zip-safe
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      577 2017-05-24 22:40:12.000000 Pydap-3.2.2/src/Pydap.egg-info/PKG-INFO
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      402 2017-05-24 22:18:20.000000 Pydap-3.2.2/CONTRIBUTORS.md
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/docs/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1086 2016-06-22 18:05:12.000000 Pydap-3.2.2/docs/license.rst
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    21209 2017-05-24 04:46:14.000000 Pydap-3.2.2/docs/client.rst
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     7661 2017-05-24 04:46:14.000000 Pydap-3.2.2/docs/server.rst
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4179 2017-05-22 19:27:13.000000 Pydap-3.2.2/docs/developer_handlers.rst
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     2991 2016-06-22 18:05:12.000000 Pydap-3.2.2/docs/Makefile
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      623 2017-05-22 19:27:13.000000 Pydap-3.2.2/docs/developer.rst
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     7990 2017-05-24 17:09:02.000000 Pydap-3.2.2/docs/handlers.rst
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    14884 2017-05-22 19:27:13.000000 Pydap-3.2.2/docs/developer_data_model.rst
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/docs/_static/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     9697 2016-06-22 18:05:12.000000 Pydap-3.2.2/docs/_static/default.css
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/docs/_build/
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/docs/_build/doctrees/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    54210 2017-05-23 17:32:54.000000 Pydap-3.2.2/docs/_build/doctrees/developer_data_model.doctree
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    67301 2017-05-24 17:13:16.000000 Pydap-3.2.2/docs/_build/doctrees/client.doctree
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    18624 2017-05-24 17:13:33.000000 Pydap-3.2.2/docs/_build/doctrees/index.doctree
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    31962 2017-05-24 17:13:16.000000 Pydap-3.2.2/docs/_build/doctrees/server.doctree
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     7583 2017-05-23 17:32:54.000000 Pydap-3.2.2/docs/_build/doctrees/developer_templating.doctree
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    19827 2017-05-23 17:32:54.000000 Pydap-3.2.2/docs/_build/doctrees/responses.doctree
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    28652 2017-05-24 17:13:16.000000 Pydap-3.2.2/docs/_build/doctrees/handlers.doctree
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    14465 2017-05-23 17:32:54.000000 Pydap-3.2.2/docs/_build/doctrees/developer_handlers.doctree
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4750 2017-05-23 17:32:54.000000 Pydap-3.2.2/docs/_build/doctrees/license.doctree
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    24455 2017-05-24 17:13:33.000000 Pydap-3.2.2/docs/_build/doctrees/environment.pickle
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    85000 2017-05-23 17:32:54.000000 Pydap-3.2.2/docs/_build/doctrees/developer.doctree
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    12475 2017-05-23 17:32:54.000000 Pydap-3.2.2/docs/_build/doctrees/developer_responses.doctree
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/docs/_build/html/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    14897 2017-05-23 18:11:03.000000 Pydap-3.2.2/docs/_build/html/developer_handlers.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4740 2017-05-24 17:13:34.000000 Pydap-3.2.2/docs/_build/html/genindex.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    19833 2017-05-24 17:13:16.000000 Pydap-3.2.2/docs/_build/html/server.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    13854 2017-05-23 18:11:03.000000 Pydap-3.2.2/docs/_build/html/responses.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      230 2017-05-24 17:13:34.000000 Pydap-3.2.2/docs/_build/html/.buildinfo
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      406 2017-05-24 17:13:34.000000 Pydap-3.2.2/docs/_build/html/objects.inv
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/docs/_build/html/_sources/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      623 2017-05-22 19:27:13.000000 Pydap-3.2.2/docs/_build/html/_sources/developer.rst.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     7661 2017-05-24 04:38:28.000000 Pydap-3.2.2/docs/_build/html/_sources/server.rst.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1606 2017-05-22 19:27:13.000000 Pydap-3.2.2/docs/_build/html/_sources/developer_templating.rst.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     7990 2017-05-24 17:09:02.000000 Pydap-3.2.2/docs/_build/html/_sources/handlers.rst.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     3472 2017-05-24 17:04:34.000000 Pydap-3.2.2/docs/_build/html/_sources/index.rst.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4532 2016-06-22 18:05:12.000000 Pydap-3.2.2/docs/_build/html/_sources/responses.rst.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4179 2017-05-22 19:27:13.000000 Pydap-3.2.2/docs/_build/html/_sources/developer_handlers.rst.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4265 2017-05-22 19:27:13.000000 Pydap-3.2.2/docs/_build/html/_sources/developer_responses.rst.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1086 2016-06-22 18:05:12.000000 Pydap-3.2.2/docs/_build/html/_sources/license.rst.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    14884 2017-05-22 19:27:13.000000 Pydap-3.2.2/docs/_build/html/_sources/developer_data_model.rst.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    21209 2017-05-24 04:46:14.000000 Pydap-3.2.2/docs/_build/html/_sources/client.rst.txt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    14357 2017-05-24 17:13:33.000000 Pydap-3.2.2/docs/_build/html/index.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    78276 2017-05-23 18:11:03.000000 Pydap-3.2.2/docs/_build/html/developer.html
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/docs/_build/html/_static/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      203 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/up.png
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)   263767 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/jquery-3.1.0.js
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      222 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/down-pressed.png
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/docs/_build/html/_static/fonts/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)   391622 2017-05-23 17:32:51.000000 Pydap-3.2.2/docs/_build/html/_static/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)   170616 2017-05-23 17:32:51.000000 Pydap-3.2.2/docs/_build/html/_static/fonts/RobotoSlab-Bold.ttf
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)   109948 2017-05-23 17:32:51.000000 Pydap-3.2.2/docs/_build/html/_static/fonts/Inconsolata-Bold.ttf
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)   656544 2017-05-23 17:32:51.000000 Pydap-3.2.2/docs/_build/html/_static/fonts/Lato-Bold.ttf
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)   656568 2017-05-23 17:32:51.000000 Pydap-3.2.2/docs/_build/html/_static/fonts/Lato-Regular.ttf
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)   169064 2017-05-23 17:32:51.000000 Pydap-3.2.2/docs/_build/html/_static/fonts/RobotoSlab-Regular.ttf
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    90412 2017-05-23 17:32:51.000000 Pydap-3.2.2/docs/_build/html/_static/fonts/fontawesome-webfont.woff
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)   152796 2017-05-23 17:32:51.000000 Pydap-3.2.2/docs/_build/html/_static/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    76518 2017-05-23 17:32:51.000000 Pydap-3.2.2/docs/_build/html/_static/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    96964 2017-05-23 17:32:51.000000 Pydap-3.2.2/docs/_build/html/_static/fonts/Inconsolata-Regular.ttf
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      829 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/comment-close.png
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    25370 2017-05-24 17:13:34.000000 Pydap-3.2.2/docs/_build/html/_static/searchtools.js
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/docs/_build/html/_static/css/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)   112267 2017-05-23 17:32:51.000000 Pydap-3.2.2/docs/_build/html/_static/css/theme.css
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     3376 2017-05-23 17:32:51.000000 Pydap-3.2.2/docs/_build/html/_static/css/badge_only.css
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      202 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/down.png
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    86351 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/jquery.js
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      455 2017-05-24 17:13:34.000000 Pydap-3.2.2/docs/_build/html/_static/opensearch.xml
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     8166 2017-05-24 17:13:34.000000 Pydap-3.2.2/docs/_build/html/_static/doctools.js
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      286 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/file.png
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)       90 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/plus.png
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    25351 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/websupport.js
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     9697 2016-06-22 18:05:12.000000 Pydap-3.2.2/docs/_build/html/_static/default.css
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      756 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/comment-bright.png
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4395 2017-05-24 17:13:34.000000 Pydap-3.2.2/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    10317 2017-05-24 17:13:34.000000 Pydap-3.2.2/docs/_build/html/_static/basic.css
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)       90 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/minus.png
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    35168 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/underscore-1.3.1.js
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      641 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/comment.png
-drwxrwxr-x   0 hiebert   (1000) hiebert   (1000)        0 2017-05-24 22:40:12.000000 Pydap-3.2.2/docs/_build/html/_static/js/
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     6477 2017-05-23 17:32:51.000000 Pydap-3.2.2/docs/_build/html/_static/js/theme.js
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    15414 2017-05-23 17:32:51.000000 Pydap-3.2.2/docs/_build/html/_static/js/modernizr.min.js
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    12140 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/underscore.js
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      214 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/up-pressed.png
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      673 2017-05-23 17:30:48.000000 Pydap-3.2.2/docs/_build/html/_static/ajax-loader.gif
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     5134 2017-05-24 17:13:34.000000 Pydap-3.2.2/docs/_build/html/search.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    14301 2017-05-23 18:11:03.000000 Pydap-3.2.2/docs/_build/html/developer_responses.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     9338 2017-05-23 18:11:03.000000 Pydap-3.2.2/docs/_build/html/developer_templating.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    21053 2017-05-24 17:13:16.000000 Pydap-3.2.2/docs/_build/html/handlers.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    16226 2017-05-24 17:13:34.000000 Pydap-3.2.2/docs/_build/html/searchindex.js
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    51709 2017-05-23 18:11:03.000000 Pydap-3.2.2/docs/_build/html/developer_data_model.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)    59463 2017-05-24 17:13:16.000000 Pydap-3.2.2/docs/_build/html/client.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     6425 2017-05-23 18:11:03.000000 Pydap-3.2.2/docs/_build/html/license.html
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     3472 2017-05-24 17:04:34.000000 Pydap-3.2.2/docs/index.rst
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     1606 2017-05-22 19:27:13.000000 Pydap-3.2.2/docs/developer_templating.rst
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     8435 2016-06-22 18:05:12.000000 Pydap-3.2.2/docs/Special chars.odt
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     2957 2016-06-22 18:05:12.000000 Pydap-3.2.2/docs/make.bat
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4265 2017-05-22 19:27:13.000000 Pydap-3.2.2/docs/developer_responses.rst
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     6585 2017-05-24 04:46:14.000000 Pydap-3.2.2/docs/conf.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     4532 2016-06-22 18:05:12.000000 Pydap-3.2.2/docs/responses.rst
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      236 2017-05-22 19:27:13.000000 Pydap-3.2.2/MANIFEST.in
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     3096 2017-05-24 22:18:20.000000 Pydap-3.2.2/setup.py
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     2990 2017-05-24 22:18:20.000000 Pydap-3.2.2/NEWS.md
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      332 2017-05-24 22:40:12.000000 Pydap-3.2.2/setup.cfg
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)      577 2017-05-24 22:40:12.000000 Pydap-3.2.2/PKG-INFO
--rw-rw-r--   0 hiebert   (1000) hiebert   (1000)     3768 2017-05-24 17:12:07.000000 Pydap-3.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.222408 pydap-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-07 23:15:52.000000 pydap-3.4.0/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-07 23:15:52.000000 pydap-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-07 23:15:52.000000 pydap-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6999 2023-04-07 23:15:52.000000 pydap-3.4.0/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-07 23:16:09.222408 pydap-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-07 23:15:52.000000 pydap-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.202408 pydap-3.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/Special chars.odt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.202408 pydap-3.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/_static/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/client.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/developer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15745 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/developer_data_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/developer_handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/developer_responses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/developer_templating.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/handlers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/responses.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-04-07 23:15:52.000000 pydap-3.4.0/docs/server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-07 23:16:09.222408 pydap-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-04-07 23:15:52.000000 pydap-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.190408 pydap-3.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/apis/netcdf4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/cas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/cas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/cas/esgf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/cas/get_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/cas/urs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/handlers/csv/
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/handlers/csv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23594 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/handlers/dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17787 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/handlers/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/handlers/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/handlers/netcdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23970 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/parsers/das.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/parsers/dds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/parsers/dmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/pycompat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap/responses/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/das.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/dds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/dods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.210408 pydap-3.4.0/src/pydap/responses/html/
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/html/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.210408 pydap-3.4.0/src/pydap/responses/html/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/html/templates/html.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/html/templates/macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/responses/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.210408 pydap-3.4.0/src/pydap/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/server/devel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/server/devel_ssl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.214408 pydap-3.4.0/src/pydap/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.214408 pydap-3.4.0/src/pydap/tests/dap_4_access/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/dap_4_access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/dap_4_access/analyze_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/dap_4_access/dap4_access_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.218408 pydap-3.4.0/src/pydap/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/data/coads_climatology.nc.dods
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/data/rainfall_time_malaysia.cdp.das
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/data/rainfall_time_malaysia.cdp.dds
+-rw-r--r--   0 runner    (1001) docker     (123)  5673697 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/data/rainfall_time_malaysia.cdp.dods
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/data/test.01.das
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/data/test.01.dods
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_D1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_cas_esgf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_cas_urs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_constrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_dapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_handlers_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22380 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_handlers_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18572 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_handlers_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_handlers_netcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_iter_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16851 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_open_dap4_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_parsers_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_parsers_das.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_parsers_dds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_parsers_dmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_pydap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_ascii.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_das.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_dds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_dods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_responses_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_server_devel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_server_devel_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_special_chars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_webtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_wsgi_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15744 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_wsgi_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/tests/test_wsgi_ssf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.222408 pydap-3.4.0/src/pydap/wsgi/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6280 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/ssf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.222408 pydap-3.4.0/src/pydap/wsgi/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/templates/catalog.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.222408 pydap-3.4.0/src/pydap/wsgi/templates/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-04-07 23:15:52.000000 pydap-3.4.0/src/pydap/wsgi/templates/static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:16:09.206408 pydap-3.4.0/src/pydap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-04-07 23:16:09.000000 pydap-3.4.0/src/pydap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-07 23:16:09.000000 pydap-3.4.0/src/pydap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:16:09.000000 pydap-3.4.0/src/pydap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-07 23:16:09.000000 pydap-3.4.0/src/pydap.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 23:16:09.000000 pydap-3.4.0/src/pydap.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:16:08.000000 pydap-3.4.0/src/pydap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-07 23:16:09.000000 pydap-3.4.0/src/pydap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-07 23:16:09.000000 pydap-3.4.0/src/pydap.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Pydap-3.2.2/src/pydap/lib.py` & `pydap-3.4.0/src/pydap/lib.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Basic functions related to the DAP spec."""
 import operator
 
+import numpy as np
 from pkg_resources import get_distribution
 from six.moves.urllib.parse import quote as quote_
 from six.moves import reduce, zip_longest
-from six import binary_type, MAXSIZE
+from six import binary_type, MAXSIZE, string_types
 
 from .exceptions import ConstraintExpressionError
 
-
 __dap__ = '2.15'
-__version__ = get_distribution("Pydap").version
-
+__version__ = get_distribution("pydap").version
 
 START_OF_SEQUENCE = b'\x5a\x00\x00\x00'
 END_OF_SEQUENCE = b'\xa5\x00\x00\x00'
 STRING = '|S128'
 DEFAULT_TIMEOUT = 120  # 120 seconds = 2 minutes
 
 NUMPY_TO_DAP2_TYPEMAP = {
@@ -103,33 +102,60 @@
     'byte': 'B',
     'string': STRING,
     'url': STRING,
     'int': '>i',
     'uint': '>I',
 }
 
+# Typemap from lower case DAP4 types to
+# numpy dtype string with specified endiannes.
+# Here, the endianness is very important:
+DAP4_TO_NUMPY_PARSER_TYPEMAP = {
+    'Float16': '>f2',
+    'Float32': '>f4',
+    'Float64': '>f8',
+    'Int8': '>i1',
+    'UInt8': '>u1',
+    'Int16': '>i2',
+    'UInt16': '>u2',
+    'Int32': '>i4',
+    'UInt32': '>u4',
+    'Int64': '>i8',
+    'UInt64': '>u8',
+    'Byte': 'B',
+    'String': STRING,
+    'Url': STRING,
+}
+
 
 def quote(name):
     """Return quoted name according to the DAP specification.
 
         >>> quote("White space")
         'White%20space'
         >>> quote("Period.")
         'Period%2E'
 
     """
-    safe = '%_!~*\'-"'
+    safe = '%_!~*\'-"/'
     return quote_(name.encode('utf-8'), safe=safe).replace('.', '%2E')
 
 
 def encode(obj):
     """Return an object encoded to its DAP representation."""
+    # fix for Python 3.5, where strings are being encoded as numbers
+    if (
+            isinstance(obj, string_types) or
+            isinstance(obj, np.ndarray) and obj.dtype.char in 'SU'
+    ):
+        return '"{0}"'.format(obj)
+
     try:
         return '%.6g' % obj
-    except:
+    except Exception:
         return '"{0}"'.format(obj)
 
 
 def fix_slice(slice_, shape):
     """Return a normalized slice.
 
     This function returns a slice so that it has the same length of `shape`,
@@ -145,15 +171,15 @@
         slice_ = (slice_,)
 
     # expand Ellipsis and make `slice_` at least as long as `shape`
     expand = len(shape) - len(slice_)
     out = []
     for s in slice_:
         if s is Ellipsis:
-            out.extend((slice(None),) * (expand+1))
+            out.extend((slice(None),) * (expand + 1))
             expand = 0
         else:
             out.append(s)
     slice_ = tuple(out) + (slice(None),) * expand
 
     out = []
     for s, n in zip(slice_, shape):
@@ -168,15 +194,15 @@
             if i is None:
                 i = 0
             elif i < 0:
                 i += n
 
             j = s.stop
             if (j is None or
-               j > n):
+                    j > n):
                 j = n
             elif j < 0:
                 j += n
 
             out.append(slice(i, j, k))
 
     return tuple(out)
@@ -190,17 +216,17 @@
         x[ combine_slices(s1, s2) ] == x[s1][s2]
 
     """
     out = []
     for exp1, exp2 in zip_longest(
             slice1, slice2, fillvalue=slice(None)):
         if isinstance(exp1, int):
-            exp1 = slice(exp1, exp1+1)
+            exp1 = slice(exp1, exp1 + 1)
         if isinstance(exp2, int):
-            exp2 = slice(exp2, exp2+1)
+            exp2 = slice(exp2, exp2 + 1)
 
         start = (exp1.start or 0) + (exp2.start or 0)
         step = (exp1.step or 1) * (exp2.step or 1)
 
         if exp1.stop is None and exp2.stop is None:
             stop = None
         elif exp1.stop is None:
@@ -221,15 +247,15 @@
     else:
         slice_ = list(slice_)
 
     while slice_ and slice_[-1] == slice(None):
         slice_.pop(-1)
 
     return ''.join('[%s:%s:%s]' % (
-        s.start or 0, s.step or 1, (s.stop or MAXSIZE)-1) for s in slice_)
+        s.start or 0, s.step or 1, (s.stop or MAXSIZE) - 1) for s in slice_)
 
 
 def walk(var, type=object):
     """Yield all variables of a given type from a dataset.
 
     The iterator returns also the parent variable.
 
@@ -255,30 +281,30 @@
             token, slice_ = var.pop(0)
             for child in walk(dataset):
                 if token == child.name:
                     if var:
                         raise ConstraintExpressionError(
                             'Ambiguous shorthand notation request: %s' % token)
                     var = [
-                        (parent, ()) for parent in child.id.split('.')[:-1]
-                    ] + [(token, slice_)]
+                              (parent, ()) for parent in child.id.split('.')[:-1]
+                          ] + [(token, slice_)]
         out.append(var)
     return out
 
 
 def get_var(dataset, id_):
     """Given an id, return the corresponding variable from the dataset."""
     tokens = id_.split('.')
     return reduce(operator.getitem, [dataset] + tokens)
 
 
 def decode_np_strings(numpy_var):
     """Given a fixed-width numpy string, decode it to a unicode type"""
-    if isinstance(numpy_var, binary_type) and hasattr(numpy_var, 'tostring'):
-        return numpy_var.tostring().decode('utf-8')
+    if isinstance(numpy_var, binary_type) and hasattr(numpy_var, 'tobytes'):
+        return numpy_var.tobytes().decode('utf-8')
     else:
         return numpy_var
 
 
 def load_from_entry_point_relative(r, package):
     try:
         loaded = getattr(__import__(r.module_name
@@ -288,15 +314,14 @@
         return r.name, loaded
     except ImportError:
         # This is only used in handlers testing:
         return r.name, r.load()
 
 
 class StreamReader(object):
-
     """Class to allow reading a `urllib3.HTTPResponse`."""
 
     def __init__(self, stream):
         self.stream = stream
         self.buf = bytearray()
 
     def read(self, n):
@@ -307,18 +332,21 @@
 
         out = bytes(self.buf[:n])
         self.buf = self.buf[n:]
         return out
 
 
 class BytesReader(object):
-
     """Class to allow reading a `bytes` object."""
 
     def __init__(self, data):
         self.data = data
 
     def read(self, n):
         """Read and return `n` bytes."""
         out = self.data[:n]
         self.data = self.data[n:]
         return out
+
+    def peek(self, n):
+        return self.data[:n]
+
```

### Comparing `Pydap-3.2.2/src/pydap/wsgi/functions.py` & `pydap-3.4.0/src/pydap/wsgi/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,42 @@
-"""Server-side functions for Pydap.
+"""Server-side functions for pydap.
 
-Pydap maps function calls in the request URL to functions defined through entry
-points. For example, Pydap defines an entry point on the group "pydap.function"
+pydap maps function calls in the request URL to functions defined through entry
+points. For example, pydap defines an entry point on the group "pydap.function"
 with the name "density"; from ``setup.py``:
 
     [pydap.function]
     density = pydap.wsgi.functions.density
 
 When a DAP client makes a request to the URL calling this function:
 
     ?cast.oxygen&density(cast.salt,cast.temp,cast.press)>1024
 
-Pydap will call the ``density`` function passing the dataset itself as the
+pydap will call the ``density`` function passing the dataset itself as the
 first argument, followed by the variables from the sequence "cast".
 
 New functions can be defined in third-party modules. Simply create a package
 and declare the entry point in its ``setup.py`` file. The server will
 automatically discover the new functions from the system.
 
 """
 
 from datetime import datetime, timedelta
 import re
 
 import numpy as np
-import coards
-import gsw
 
 from ..model import SequenceType, GridType, BaseType
 from ..lib import walk
 from ..exceptions import ConstraintExpressionError, ServerError
+from ..pycompat import suppress
+
+with suppress(ImportError):
+    import coards
+    import gsw
 
 
 def density(dataset, salinity, temperature, pressure):
     """Calculate in-situ density.
 
     This function calculated in-situ density from absolute salinity and
     conservative temperature, using the `gsw.rho` function. Returns a new
```

### Comparing `Pydap-3.2.2/src/pydap/wsgi/app.py` & `pydap-3.4.0/src/pydap/wsgi/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""A file-based Pydap server running on Gunicorn.
+"""A file-based pydap server running on Gunicorn.
 
 Usage:
   pydap [options]
 
 Options:
   -h --help                     Show this help message and exit
   --version                     Show version
@@ -52,14 +52,15 @@
         if templates is not None:
             loaders.insert(0, FileSystemLoader(templates))
 
         # set the rendering environment; this is also used by pydap responses
         # that need to render templates (like HTML, WMS, KML, etc.)
         self.env = Environment(loader=ChoiceLoader(loaders))
         self.env.filters["datetimeformat"] = datetimeformat
+        self.env.filters["datetimeformat_iso"] = datetimeformat_iso
         self.env.filters["unquote"] = unquote
 
         # cache available handlers, so we don't need to load them every request
         self.handlers = load_handlers()
 
     @wsgify
     def __call__(self, req):
@@ -69,14 +70,16 @@
 
         """
         path = os.path.abspath(
             os.path.join(self.path, *req.path_info.split("/")))
 
         if not path.startswith(self.path):
             return HTTPForbidden()
+        if path.endswith('catalog.xml'):
+            return self.index(os.path.dirname(path), req, catalog=True)
         elif os.path.exists(path):
             if os.path.isdir(path):
                 return self.index(path, req)
             else:
                 return FileApp(path)
 
         # strip DAP extension (``.das``, eg) and see if the file exists
@@ -84,16 +87,19 @@
         if os.path.isfile(base):
             req.environ["pydap.jinja2.environment"] = self.env
             app = ServerSideFunctions(get_handler(base, self.handlers))
             return req.get_response(app)
         else:
             return HTTPNotFound(comment=path)
 
-    def index(self, directory, req):
+    def index(self, directory, req, catalog=False):
         """Return a directory listing."""
+
+        template_name = 'index.html'
+        response_content_type = 'text/html'
         content = [
             os.path.join(directory, name) for name in os.listdir(directory)]
 
         files = [{
             "name": os.path.split(path)[1],
             "size": os.path.getsize(path),
             "last_modified": datetime.fromtimestamp(os.path.getmtime(path)),
@@ -117,29 +123,35 @@
             "root": req.application_url,
             "location": req.path_url,
             "breadcrumbs": breadcrumbs,
             "directories": directories,
             "files": files,
             "version": __version__,
         }
-        template = self.env.get_template("index.html")
+
+        if catalog:
+            context['location'] = req.path.replace('catalog.xml', '')
+            template_name = 'catalog.xml'
+            response_content_type = 'application/xml'
+
+        template = self.env.get_template(template_name)
         return Response(
             body=template.render(context),
-            content_type="text/html",
+            content_type=response_content_type,
             charset="utf-8")
 
 
 def supported(filepath, handlers=None):
     """Test if a file has a corresponding handler.
 
     Returns a boolean.
 
     """
     try:
-        get_handler(filepath, handlers)
+        get_handler(filepath, handlers, instantiate=False)
         return True
     except ExtensionNotSupportedError:
         return False
 
 
 def alphanum_key(s):
     """Parse a string, returning a list of string and number chunks.
@@ -151,24 +163,29 @@
 
     From http://nedbatchelder.com/blog/200712.html#e20071211T054956
 
     """
     def tryint(s):
         try:
             return int(s)
-        except:
+        except Exception:
             return s
     return [tryint(c) for c in re.split('([0-9]+)', s)]
 
 
 def datetimeformat(value, format='%Y-%m-%d %H:%M:%S'):
     """Return a formatted datetime object."""
     return value.strftime(format)
 
 
+def datetimeformat_iso(value):
+    """Return a formatted datetime object as ISO8601 representation."""
+    return value.isoformat()
+
+
 class StaticMiddleware(object):
 
     """WSGI middleware for static assets.
 
     The assets can be either specified as a directory, or retrieved from a
     Python package. Inspired by ``werkezeug.wsgi.SharedDataMiddleware``.
 
@@ -220,15 +237,15 @@
 def main():  # pragma: no cover
     """Run server from the command line."""
     import multiprocessing
 
     from docopt import docopt
     from gunicorn.app.pasterapp import PasterServerApplication
 
-    arguments = docopt(__doc__, version="Pydap %s" % __version__)
+    arguments = docopt(__doc__, version="pydap %s" % __version__)
 
     # init templates?
     if arguments["--init"]:
         init(arguments["--init"])
         return
 
     # create pydap app
```

### Comparing `Pydap-3.2.2/src/pydap/wsgi/ssf.py` & `pydap-3.4.0/src/pydap/wsgi/ssf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """An implementation of server-side functions.
 
-Pydap implements DAP server-side functions throught a custom WSGI middleware.
+pydap implements DAP server-side functions throught a custom WSGI middleware.
 This simplifies writing custom handlers, since they don't need to parse and
 apply the function calls themselves.
 
 """
 
 import re
 import operator
@@ -43,15 +43,15 @@
 
 
 class ServerSideFunctions(object):
 
     """A WebOb based middleware for handling server-side function calls.
 
     The middleware works by removing function calls from the request,
-    forwarding the request to Pydap, and then applying the functions calls to
+    forwarding the request to pydap, and then applying the functions calls to
     the returned dataset.
 
     """
 
     def __init__(self, app, **kwargs):
         self.app = app
 
@@ -179,17 +179,17 @@
     def parse(token):
         if FUNCTION.match(token):
             return eval_function(dataset, token, functions)
         else:
             try:
                 names = re.sub(r'\[.*?\]', '', str(token)).split('.')
                 return reduce(operator.getitem, [dataset] + names)
-            except:
+            except Exception:
                 try:
                     return ast.literal_eval(token)
-                except:
+                except Exception:
                     return token
 
     args = map(parse, tokenize(args))
     func = functions[name]
 
     return func(dataset, *args)
```

### Comparing `Pydap-3.2.2/src/pydap/wsgi/templates/index.html` & `pydap-3.4.0/src/pydap/wsgi/templates/index.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,68 @@
 {% extends "base.html" %}
 
-{% block title %}Index of {{ location }}{% endblock %}
+{% block title %}OPeNDAP pydap: Index of {{ location }}{% endblock %}
 
 {% block breadcrumbs %}
-<ul>
-    {% for crumb in breadcrumbs[:-1] %}
-    <li itemscope itemtype="http://data-vocabulary.org/Breadcrumb">
-    <a itemprop="url" href="{{ crumb.url }}/"><span itemprop="title">{{ crumb.title }}</span></a>
-    </li>
-    <li><i class="icon-angle-right"></i></li>                                             
-    {% endfor %}
-    {% if breadcrumbs %}
-    <li itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="pure-menu-selected">
-    <a itemprop="url" href="{{ breadcrumbs[-1].url }}/"><span itemprop="title">{{ breadcrumbs[-1].title }}</span></a>
-    </li>
-    {% endif %}
-</ul>
+    <p>
+        <span itemscope itemtype="http://data-vocabulary.org/Breadcrumb">
+            <a itemprop="url" href="{{ root }}"><span itemprop="title">Home</span></a>
+        </span>
+        {% for crumb in breadcrumbs %}
+        /<span itemscope itemtype="http://data-vocabulary.org/Breadcrumb">
+            <a itemprop="url" href="{{ crumb.url }}/"><span itemprop="title">{{ crumb.title }}</span></a>
+        </span>
+        {% endfor %}
+    </p>
 {% endblock %}
-
 {% block content %}
-<table class="pure-table pydap-listing">
+<table>
     <thead>
         <tr>
             <th>Name</th>
             <th>Size</th>
             <th>Last modified</th>
+            <th>DAP Response Links</th>
         </tr>
     </thead>
 
     <tbody>
+        {% if breadcrumbs %}
+        <tr>
+            <td><a href="..">..</a></td>
+            <td>&ndash;</td>
+            <td>&ndash;</td>
+            <td>&ndash;</td>
+        </tr>
+        {% endif %}
         {% for directory in directories %}
         <tr>
-            <td><i class="icon-folder-close icon-fixed-width"></i> <a href="{{ directory.name }}/">{{ directory.name }}/</a></td>
+            <td><a href="{{ directory.name }}/">{{ directory.name }}/</a></td>
             <td>&ndash;</td>
             <td>{{ directory.last_modified|datetimeformat }}</td>
+            <td>&ndash;</td>
         </tr>
         {% endfor %}
         {% for file in files %}
         <tr>
             {% if file.supported %}
-            <td><i class="icon-globe icon-fixed-width"></i>
-            <a title="Inspect and filter data" href="{{ file.name }}.html">{{ file.name }}</a>
-            <span class="dap">
-            <a title="View the DDS response" href="{{ file.name }}.dds">dds</a> |
-            <a title="View the DAS response" href="{{ file.name }}.das">das</a>
-            </span>
-            </td>
+            <td><a title="Inspect and filter data" href="{{ file.name }}.html">{{ file.name }}</a></td>
             {% elif file.name.endswith(".html") %}
-            <td><i class="icon-file icon-fixed-width"></i>
-            <a href="{{ file.name }}">{{ file.name }}</a>
+            <td><a href="{{ file.name }}">{{ file.name }}</a>
             </td>
             {% else %}
-            <td><i class="icon-file icon-fixed-width"></i>
-            {{ file.name }}
-            </td>
+            <td>{{ file.name }}</td>
             {% endif %}
             <td><a title="Download file" href="{{ file.name }}">{{ file.size|filesizeformat}}</a></td>
             <td>{{ file.last_modified|datetimeformat }}</td>
+            {% if file.supported %}
+            <td><a title="View the DDS response" href="{{ file.name }}.dds">dds</a> | <a title="View the DAS response" href="{{ file.name }}.das">das</a></td>
+            {% else %}
+            <td>&ndash;</td>
+            {% endif %}
         </tr>
         {% endfor %}
     </tbody>
 </table>
+</p>
+<a href="{{ location }}catalog.xml" title="THREDDS Catalog XML">THREDDS Catalog XML</a>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,18 +1,15 @@
-{% extends "base.html" %} {% block title %}Index of {{ location }}{% endblock
-%} {% block breadcrumbs %}
-    * {% for crumb in breadcrumbs[:-1] %}
-    * {{_crumb.title_}}
-    * {% endfor %} {% if breadcrumbs %}
-    * {{_breadcrumbs[-1].title_}}
-    * {% endif %}
+{% extends "base.html" %} {% block title %}OPeNDAP pydap: Index of {{ location
+}}{% endblock %} {% block breadcrumbs %}
+ Home  {% for crumb in breadcrumbs %} / {{_crumb.title_}}  {% endfor %}
 {% endblock %} {% block content %}
-Name           Size      Last modified
- {                       {
-{              –       {
+Name           Size      Last modified                          DAP Response Links
+..             –       –                                    –
+{                        {
+{              –       {                                      –
 directory.name           directory.last_modified|datetimeformat
 }}/                      }}
-                {                                               {                          {
- {{_file.name  {          {{ file.name }}                       {                          {
-}}  dds | das  file.name                                        file.size|filesizeformat}} file.last_modified|datetimeformat
+               {                                                {                          {                                 dds
+{{_file.name   {         {{ file.name }}                        {                          {                                 |   –
+}}             file.name                                        file.size|filesizeformat}} file.last_modified|datetimeformat das
                }}                                                                          }}
-{% endblock %}
+THREDDS_Catalog_XML {% endblock %}
```

### Comparing `Pydap-3.2.2/src/pydap/parsers/__init__.py` & `pydap-3.4.0/src/pydap/parsers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 
 def parse_selection(expression, dataset):
     """Parse a selection expression into its elements.
 
     This function will parse a selection expression into three tokens: two
     variables or values and a comparison operator. Variables are returned as
-    Pydap objects from a given dataset, while values are parsed using
+    pydap objects from a given dataset, while values are parsed using
     ``ast.literal_eval``.
 
     """
     id1, op, id2 = re.split('(<=|>=|!=|=~|>|<|=)', expression, 1)
 
     op = {
         '<=': operator.le,
@@ -70,20 +70,20 @@
         '=': operator.eq,
         '>': operator.gt,
         '<': operator.lt,
     }[op]
 
     try:
         id1 = get_var(dataset, id1)
-    except:
+    except Exception:
         id1 = ast.literal_eval(id1)
 
     try:
         id2 = get_var(dataset, id2)
-    except:
+    except Exception:
         id2 = ast.literal_eval(id2)
 
     return id1, op, id2
 
 
 def parse_ce(query_string):
     """Extract the projection and selection from the QUERY_STRING.
```

### Comparing `Pydap-3.2.2/src/pydap/parsers/das.py` & `pydap-3.4.0/src/pydap/parsers/das.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,18 @@
                 '''
             )
 
             if type.lower() in ['string', 'url']:
                 value = str(value).strip('"')
             elif value.lower() in ['nan', 'nan.', '-nan']:
                 value = float('nan')
+            elif value.lower() in ['inf', 'inf.']:
+                value = float('inf')
+            elif value.lower() in ['-inf', '-inf.']:
+                value = float('-inf')
             else:
                 value = ast.literal_eval(value)
 
             values.append(value)
             if self.peek(','):
                 self.consume(',')
```

### Comparing `Pydap-3.2.2/src/pydap/parsers/dds.py` & `pydap-3.4.0/src/pydap/parsers/dds.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     the DAP2 specification.
     """
     dtype_str = LOWER_DAP2_TO_NUMPY_PARSER_TYPEMAP[type_string.lower()]
     return np.dtype(dtype_str)
 
 
 class DDSParser(SimpleParser):
-
     """A parser for the DDS."""
 
     def __init__(self, dds):
         super(DDSParser, self).__init__(dds, re.IGNORECASE)
         self.dds = dds
 
     def consume(self, regexp):
@@ -65,21 +64,21 @@
             'structure': self.structure,
         }
         method = map.get(token, self.base)
         return method()
 
     def base(self):
         """Parse a base variable, returning a ``BaseType``."""
-        data_type_string = self.consume('\w+')
+        data_type_string = self.consume(r'\w+')
 
         parser_dtype = DAP2_parser_typemap(data_type_string)
-        name = quote(self.consume('[^;\[]+'))
+        name = quote(self.consume(r'[^;\[]+'))
 
         shape, dimensions = self.dimensions()
-        self.consume(';')
+        self.consume(r';')
 
         data = DummyData(parser_dtype, shape)
         var = BaseType(name, data, dimensions=dimensions)
 
         return var
 
     def dimensions(self):
@@ -148,15 +147,15 @@
 
         grid.name = quote(self.consume('[^;]+'))
         self.consume(';')
 
         return grid
 
 
-def build_dataset(dds):
+def dds_to_dataset(dds):
     """Return a dataset object from a DDS representation."""
     return DDSParser(dds).parse()
 
 
 class DummyData(object):
     def __init__(self, dtype, shape):
         self.dtype = dtype
```

### Comparing `Pydap-3.2.2/src/pydap/cas/esgf.py` & `pydap-3.4.0/src/pydap/cas/esgf.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,19 +19,19 @@
                                         verify=verify)
     # Connections can be kept alive on the ESGF:
     session.headers.update([('Connection', 'keep-alive')])
     return session
 
 
 def _uri(openid):
-    '''
+    """
     Create ESGF authentication url.
     This function might be sensitive to a
     future evolution of the ESGF security.
-    '''
+    """
     def generate_url(dest_url):
         dest_node = _get_node(dest_url)
 
         try:
             url = (dest_node +
                    '/esg-orp/j_spring_openid_security_check.htm?'
                    'openid_identifier=' +
@@ -43,8 +43,8 @@
             return [url, None]
         else:
             return url
     return generate_url
 
 
 def _get_node(url):
-        return '/'.join(url.split('/')[:3]).replace('http:', 'https:')
+    return '/'.join(url.split('/')[:3]).replace('http:', 'https:')
```

### Comparing `Pydap-3.2.2/src/pydap/cas/urs.py` & `pydap-3.4.0/src/pydap/cas/urs.py`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/src/pydap/cas/get_cookies.py` & `pydap-3.4.0/src/pydap/cas/get_cookies.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     A general function to set-up requests session with cookies
     using beautifulsoup and by calling the right url.
     '''
 
     if session is None:
         # Connections must be closed since some CAS
         # will cough when connections are kept alive:
-        headers = [('User-agent', 'Pydap/{}'.format(lib.__version__)),
+        headers = [('User-agent', 'pydap/{}'.format(lib.__version__)),
                    ('Connection', 'close')]
         session = requests.Session()
         session.headers.update(headers)
 
     if uri is None:
         return session
```

### Comparing `Pydap-3.2.2/src/pydap/exceptions.py` & `pydap-3.4.0/src/pydap/exceptions.py`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/src/pydap/server/devel.py` & `pydap-3.4.0/src/pydap/server/devel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from webob.request import Request
 from webob.exc import HTTPError
 import threading
+import multiprocessing
 import time
 import math
 import numpy as np
 import socket
 
 from wsgiref.simple_server import make_server
 
 from ..handlers.lib import BaseHandler
 from ..model import BaseType, DatasetType
-from ..wsgi.ssf import ServerSideFunctions
+from ..net import get_response
 
 DefaultDataset = DatasetType("Default")
 DefaultDataset["byte"] = BaseType("byte", np.arange(5, dtype="B"))
 DefaultDataset["string"] = BaseType("string", np.array(["one", "two"]))
 DefaultDataset["short"] = BaseType("short", np.array(1, dtype="h"))
 
 
@@ -25,21 +26,25 @@
     s.bind(("", 0))
     s.listen(1)
     port = s.getsockname()[1]
     s.close()
     return port
 
 
-def run_simple_server(port, application):
-    application = ServerSideFunctions(application)
+def run_server_in_process(httpd, shutdown, **kwargs):
+    _server = (threading
+               .Thread(target=httpd.serve_forever,
+                       kwargs=kwargs))
+    _server.start()
+    shutdown.wait()
+    httpd.shutdown()
+    _server.join()
 
-    return make_server('0.0.0.0', port, application)
 
-
-class LocalTestServer:
+class LocalTestServer(object):
     """
     Simple server instance that can be used to test pydap.
     Relies on threading and is usually slow (it has to
     start and shutdown which typically takes ~2 sec).
 
     Usage:
     >>> import numpy as np
@@ -74,55 +79,83 @@
     <DatasetType with children 'byte', 'string', 'short'>
     >>> print(dataset['byte'].data[:])
     [0 1 2 3 4]
     >>> server.shutdown()
     """
 
     def __init__(self, application=BaseHandler(DefaultDataset),
-                 port=None, wait=0.5, polling=1e-2):
+                 port=None, wait=0.5, polling=1e-2, as_process=False):
         self._port = port or get_open_port()
         self.application = application
         self._wait = wait
         self._polling = polling
+        self._as_process = as_process
+        self._address = '0.0.0.0'
+
+    @property
+    def url(self):
+        return "http://{0}:{1}/".format(self._address, self.port)
 
     def start(self):
         # Start a simple WSGI server:
-        self.httpd = run_simple_server(self.port, self.application)
-        self.server_process = (threading
-                               .Thread(target=self.httpd.serve_forever,
-                                       kwargs={'poll_interval': 1e-2}))
+        application = self.application
+
+        self._httpd = make_server(self._address, self.port, application)
+        kwargs = {'poll_interval': 0.1}
+
+        if self._as_process:
+            self._shutdown = multiprocessing.Event()
+            self._server = (multiprocessing
+                            .Process(target=run_server_in_process,
+                                     args=(self._httpd, self._shutdown),
+                                     kwargs=kwargs))
+        else:
+            self._server = (threading
+                            .Thread(target=self._httpd.serve_forever,
+                                    kwargs=kwargs))
+
+        self._server.start()
+        self.poll_server()
 
-        self.server_process.start()
+    def poll_server(self):
         # Poll the server
         ok = False
         for trial in range(int(math.ceil(self._wait/self._polling))):
             try:
-                resp = (Request
-                        .blank("http://0.0.0.0:%s/.dds" % self.port)
-                        .get_response())
+                # When checking whether server has started, do
+                # not verify ssl:
+                resp = get_response(
+                        Request
+                        .blank(self.url + '.dds'),
+                        None, verify=False)
                 ok = (resp.status_code == 200)
             except HTTPError:
                 pass
             if ok:
                 break
             time.sleep(self._polling)
 
         if not ok:
+            self.shutdown()
             raise Exception(('LocalTestServer did not start in {0}s. '
                              'Try using LocalTestServer(..., wait={1}')
                             .format(self._wait, 2*self._wait))
 
     @property
     def port(self):
         return self._port
 
     def __enter__(self):
         self.start()
         return self
 
     def shutdown(self):
-        # Shutdown the server:
-        self.httpd.shutdown()
-        self.server_process.join()
+        # Tell the server to shutdown:
+        if self._as_process:
+            self._shutdown.set()
+        else:
+            self._httpd.shutdown()
+        self._server.join()
+        self._httpd.server_close()
 
     def __exit__(self, *_):
         self.shutdown()
```

### Comparing `Pydap-3.2.2/src/pydap/responses/version.py` & `pydap-3.4.0/src/pydap/responses/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Response with information about Pydap version."""
+"""Response with information about pydap version."""
 
 import sys
 from six import text_type
 
 from webob import Response
 from json import dumps
 from pkg_resources import iter_entry_points
```

### Comparing `Pydap-3.2.2/src/pydap/responses/lib.py` & `pydap-3.4.0/src/pydap/responses/lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-"""Fundamental functions for Pydap responses.
+"""Fundamental functions for pydap responses.
 
-Pydap responses are WSGI applications that convert a dataset into different
+pydap responses are WSGI applications that convert a dataset into different
 representations, like the DDS, DAS and DODS responses described in the DAP
 specification.
 
-In addition to the official responses, Pydap also has responses that generate
+In addition to the official responses, pydap also has responses that generate
 KML, WMS, JSON, etc., installed as third-party Python packages that declare the
 "pydap.response" entry point.
 
 """
 
 from pkg_resources import iter_entry_points
 
@@ -29,24 +29,24 @@
                      if not r.module_name.startswith(package))
     base_dict.update(opts_dict)
     return base_dict
 
 
 class BaseResponse(object):
 
-    """A base class for Pydap responses.
+    """A base class for pydap responses.
 
-    A Pydap response is a WSGI application that converts a dataset into any
+    A pydap response is a WSGI application that converts a dataset into any
     other representation. The most know responses are the DDS, DAS and DODS
     responses from the DAP spec, which describe the dataset structure,
     attributes and data, respectively.
 
     According to the WSGI specification, WSGI applications must returned an
     iterable object when called. While this is traditionally a list of strings
-    representing an HTML response, this is not the case for Pydap. Pydap will
+    representing an HTML response, this is not the case for pydap. pydap will
     return an object (the response instance itself), which is an iterable that
     yields the corresponding output (a DDS response, eg).
 
     In practice, this means that the generation of the response is delayed
     until the data is being sent to the client. But since the response object
     also carries the original dataset, this means it's possible to write WSGI
     middleware that modifies the dataset directly. A WSGI middleware can add
```

### Comparing `Pydap-3.2.2/src/pydap/responses/ascii.py` & `pydap-3.4.0/src/pydap/responses/ascii.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """The ASCII response.
 
 The ASCII response is an unnoficial response used to return the data as ASCII.
-Pydap's implementation is reverse engineered from the official server.
+pydap's implementation is reverse engineered from the official server.
 
 """
 
 try:
     from functools import singledispatch
 except ImportError:
     from singledispatch import singledispatch
```

### Comparing `Pydap-3.2.2/src/pydap/responses/html/__init__.py` & `pydap-3.4.0/src/pydap/responses/html/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
         } for i, token in enumerate(tokens) if token]
 
         context = {
             "root": req.application_url,
             "location": req.path_url,
             "breadcrumbs": breadcrumbs,
             "dataset": self.dataset,
+            "dataurl": req.path_url.replace('.html', ''),
             "version": __version__,
         }
 
         return Response(
             body=template.render(context),
             headers=self.headers)
```

### Comparing `Pydap-3.2.2/src/pydap/responses/html/templates/macros.html` & `pydap-3.4.0/src/pydap/responses/html/templates/macros.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 {% macro dispatch(var) %}
-<h2>{{ var.id|unquote }}</h2>
-
 {% if var.__class__.__name__ == "GridType" %}
-<label for="{{ var.id }}" class="pure-checkbox">
-    <input name="{{ var.id }}" id="{{ var.id }}" type="checkbox" value="on">
+<label for="{{ var.id }}">
+    <input name="{{ var.id }}" id="{{ var.id }}" type="checkbox" value="on"/>
     Download this variable
 </label>
 
 {{ attributes(var.attributes) }}
 
 <fieldset>
     {% for name in var.maps %}
-    <div class="pure-control-group">
+    <div>
         <label for="{{ var.id }}[{{ loop.index0 }}]">{{ name }}</label>
+        (start:step:stop):
         <input
             id="{{ var.id }}[{{ loop.index0 }}]"
             type="text"
-            placeholder="0:1:{{ var[name].shape[0]-1 }}">
+            placeholder="0:1:{{ var[name].shape[0]-1 }}"/>
     </div>
     {% endfor %}
 </fieldset>
 
 {% elif var.__class__.__name__ == "BaseType" %}
-<label for="{{ var.id }}" class="pure-checkbox">
-    <input name="{{ var.id }}" id="{{ var.id }}" type="checkbox" value="on">
+<label for="{{ var.id }}">
+    <input name="{{ var.id }}" id="{{ var.id }}" type="checkbox" value="on"/>
     Download this variable
 </label>
 
 {{ attributes(var.attributes) }}
 
 {% if var.shape %}
 <fieldset>
-    <div class="pure-control-group">
+    <div>
         {% for shp in var.shape %}
         <label for="{{ var.id }}[{{ loop.index0 }}]">{{ var.name }}[{{ loop.index0 }}]</label>
         {% if shp > 0 %}
+        (start:step:stop):
         <input
             id="{{ var.id }}[{{ loop.index0 }}]"
             type="text"
             placeholder="0:1:{{ shp - 1 }}">
         {% else %}
-        <input id="{{ var.id }}[{{ loop.index0 }}]" type="text" value="0" readonly>
+        <input id="{{ var.id }}[{{ loop.index0 }}]" type="text" value="0" readonly/>
         {% endif %}
         {% endfor %}
     </div>
 </fieldset>
 {% endif %}
 
 {% elif var.__class__.__name__ == "SequenceType" %}
 {{ attributes(var.attributes) }}
 
 <fieldset>
-    Filter where
+    Filter where:
     <select name="var1_{{ var.id }}" id="var1_{{ var.id }}">
         <option value="--" selected>--</option>
         {% for child in var.children() %}
         <option value="{{ child.id }}">{{ child.name }}</option>
         {% endfor %}
     </select>
     <select name="op_{{ var.id }}" id="op_{{ var.id }}">
@@ -63,16 +63,16 @@
         <option value="%21%3D">≠</option>
         <option value="%3C">&lt;</option>
         <option value="%3C%3D">≤</option>
         <option value="%3E">&gt;</option>
         <option value="%3E%3D">≥</option>
         <option value="%3D%7E">≈</option>
     </select>
-    <input type="text" name="var2_{{ var.id }}" id="var2_{{ var.id }}" value="">
-<fieldset>
+    <input type="text" name="var2_{{ var.id }}" id="var2_{{ var.id }}" value=""/>
+</fieldset>
 
 {% for child in var.children() %}
 {{ dispatch(child) }}
 {% endfor %}
 
 {% else %}
 {{ attributes(var.attributes) }}
@@ -88,19 +88,19 @@
 
 {% macro attributes(d) %}
 <dl>
     {% for k, v in d.items() %}
     <dt>{{ k }}</dt>
     {% if v is mapping %}
     <dd>
-    <div class="nested">
+    <div>
     {{ attributes(v) }}
     </div>
     </dd>
     {% elif v is sequence and not v is string %}
-    <dd class="value">{{ v|join(", ") }}</dd>
+    <dd>{{ v|join(", ") }}</dd>
     {% else %}
-    <dd class="value">{{ v }}</dd>
+    <dd>{{ v }}</dd>
     {% endif %}
     {% endfor %}
 </dl>
 {% endmacro %}
```

### Comparing `Pydap-3.2.2/src/pydap/responses/html/templates/html.html` & `pydap-3.4.0/src/pydap/responses/html/templates/html.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 {% extends "base.html" %}
 {% from "macros.html" import dispatch %}
 
 {% block title %}Dataset {{ location }}{% endblock %}
 
 {% block breadcrumbs %}
-<ul>
-    {% for crumb in breadcrumbs[:-1] %}
-    <li itemscope itemtype="http://data-vocabulary.org/Breadcrumb">
-    <a itemprop="url" href="{{ crumb.url }}/"><span itemprop="title">{{ crumb.title }}</span></a>
-    </li>
-    <li><i class="icon-angle-right"></i></li>                                              
+<p>
+    <span itemscope itemtype="http://data-vocabulary.org/Breadcrumb">
+        <a itemprop="url" href="{{ root }}"><span itemprop="title">Home</span></a>
+    </span>
+    {% for crumb in breadcrumbs %}
+    /<span itemscope itemtype="http://data-vocabulary.org/Breadcrumb">
+        <a itemprop="url" href="{{ crumb.url }}/"><span itemprop="title">{{ crumb.title }}</span></a>
+    </span>
     {% endfor %}
-    {% if breadcrumbs %}
-    <li itemscope itemtype="http://data-vocabulary.org/Breadcrumb" class="pure-menu-selected">
-    <a itemprop="url" href="{{ breadcrumbs[-1].url }}"><span itemprop="title">{{ breadcrumbs[-1].title[:-5] }}</span></a>
-    </li>
-    {% endif %}
-</ul>
+</p>
 {% endblock %}
 
 {% block content %}
-<div class="form">
-    <form class="pure-form pure-form-aligned" action="{{ location }}" method="POST">
-        <button type="submit" class="pure-button pure-button-submit">
-            <i class="icon-download-alt"></i>
-            Download data
-        </button>
+<div>
+    <form action="{{ location }}" method="POST">
+        <button type="submit">Download data</button>
+        <p>
+        <label for="dataset.url">
+            Data URL: <input name="dataset.url" id="dataset.url" type="text" value="{{ dataurl }}" size="50" readonly/>
+        </label>
+        </p>
         {{ dispatch(dataset) }}
-        <button type="submit" class="pure-button pure-button-submit">
-            <i class="icon-download-alt"></i>
-            Download data
-        </button>
+        <button type="submit">Download data</button><button type="reset">Reset</button>
     </form>
 </div>
 {% endblock %}
```

### Comparing `Pydap-3.2.2/src/pydap/responses/error.py` & `pydap-3.4.0/src/pydap/responses/error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-"""Pydap error response.
+"""pydap error response.
 
-Pydap will capture exceptions returned by the system and return them properly
+pydap will capture exceptions returned by the system and return them properly
 formated as a DAP error response.
 
 """
 
 from traceback import print_exception
 
 from webob import Response
```

### Comparing `Pydap-3.2.2/src/pydap/responses/dods.py` & `pydap-3.4.0/src/pydap/responses/dods.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     return np.dtype(dtype_str)
 
 
 def tostring_with_byteorder(x, dtype):
     return (x
             .astype(dtype.str)
             .newbyteorder(dtype.byteorder)
-            .tostring())
+            .tobytes())
 
 
 class DODSResponse(BaseResponse):
 
     """The DODS response."""
 
     __version__ = __version__
@@ -88,24 +88,28 @@
 
 @dods.register(SequenceType)
 def _sequencetype(var):
     # a flat array can be processed one record (or more?) at a time
     if all(isinstance(child, BaseType) for child in var.children()):
         DAP2_types = []
         position = 0
-        for child in var.children():
-            if DAP2_response_dtypemap(child.dtype).char == 'S':
-                (DAP2_types
-                 .append(DAP2_ARRAY_LENGTH_NUMPY_TYPE))  # string length
-                DAP2_types.append('|S{%s}' % position)   # string padded to 4n
-                position += 1
-            else:
-                # Convert any numpy dtypes to numpy dtypes compatible
-                # with the DAP2 standard:
-                DAP2_types.append(DAP2_response_dtypemap(child.dtype).str)
+        try:
+            for child in var.children():
+                if DAP2_response_dtypemap(child.dtype).char == 'S':
+                    (DAP2_types
+                     .append(DAP2_ARRAY_LENGTH_NUMPY_TYPE))  # string length
+                    DAP2_types.append(
+                        '|S{%s}' % position)   # string padded to 4n
+                    position += 1
+                else:
+                    # Convert any numpy dtypes to numpy dtypes compatible
+                    # with the DAP2 standard:
+                    DAP2_types.append(DAP2_response_dtypemap(child.dtype).str)
+        except StopIteration:
+            return
         DAP2_dtype_str = ','.join(DAP2_types)
         strings = position > 0
 
         # array initializations is costy, so we keep a cache here; this will
         # be inneficient if there are many strings of different length only
         cache = {}
 
@@ -132,15 +136,15 @@
                 # the data in var can all be upconverted
                 # in a lossless manner to the dtypes in DAP2_dtype.
                 cache[DAP2_dtype_str] = np.zeros((1,), dtype=DAP2_dtype_str)
             # By assigning record to ``cache`` the upconversion
             # occurs naturally:
             cache[DAP2_dtype_str][:] = tuple(record)
             # byteorder was taken care of during the upconversion:
-            yield cache[DAP2_dtype_str].tostring()
+            yield cache[DAP2_dtype_str].tobytes()
 
         yield END_OF_SEQUENCE
 
     # nested array, need to process individually
     else:
         # create a template structure
         struct = StructureType(var.name)
@@ -164,15 +168,15 @@
 
     # Convert any numpy dtypes to numpy dtypes compatible
     # with the DAP2 standard:
     DAP2_dtype = DAP2_response_dtypemap(data.dtype)
 
     if data.shape:
         # pack length for arrays
-        length = np.prod(data.shape).astype(np.int)
+        length = np.prod(data.shape).astype(int)
 
         # send length twice at the begining of an array...
         factor = 2
         if DAP2_dtype.char == 'S':
             # ... expcept for strings:
             factor = 1
         yield tostring_with_byteorder(
@@ -188,15 +192,15 @@
     #     data = data.reshape(1, -1)
     # Only ensure that 0d arrays are iterable:
     if len(data.shape) == 0:
         data = data[np.newaxis]
 
     # unsigned bytes are padded up to 4n
     if DAP2_dtype == np.ubyte:
-        length = np.prod(data.shape).astype(np.int)
+        length = np.prod(data.shape).astype(int)
         for block in data:
             yield tostring_with_byteorder(block, DAP2_dtype)
         yield (-length % 4) * b'\0'
 
     # regular data
     else:
         # strings are also zero padded and preceeded by their length
@@ -206,16 +210,16 @@
                     length = len(word)
                     yield tostring_with_byteorder(
                                 np.array(length),
                                 np.dtype(DAP2_ARRAY_LENGTH_NUMPY_TYPE))
                     # byteorder is not important for strings:
                     if hasattr(word, 'encode'):
                         yield word.encode('ascii')
-                    elif hasattr(word, 'tostring'):
-                        yield word.tostring()
+                    elif hasattr(word, 'tobytes'):
+                        yield word.tobytes()
                     else:
                         raise TypeError("Could not convert word '{0}' to bytes"
                                         .format(word))
                     yield (-length % 4) * b'\0'
         else:
             for block in data:
                 # Remember that DAP2_dtype is a
@@ -228,15 +232,15 @@
 
 
 def calculate_size(dataset):
     """Calculate the size of the response. Returns the size in bytes."""
     length = 0
 
     for var in walk(dataset):
-        # Pydap can't calculate the size of sequences since the data is
+        # pydap can't calculate the size of sequences since the data is
         # streamed directly from the source. Also, strings are encoded
         # individually, so it's not possible to get their size unless we read
         # everything.
         if (isinstance(var, SequenceType) or
             (isinstance(var, BaseType) and
              DAP2_response_dtypemap(var.dtype).char == 'S')):
             return None
```

### Comparing `Pydap-3.2.2/src/pydap/responses/das.py` & `pydap-3.4.0/src/pydap/responses/das.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,23 @@
 
 """
 
 try:
     from functools import singledispatch
 except ImportError:
     from singledispatch import singledispatch
-from collections import Iterable
-
+try:
+    from collections.abc import Iterable
+except ImportError:
+    from collections import Iterable
 from six import string_types, integer_types
 from six.moves import map
 
+import numpy as np
+
 from ..model import (DatasetType, BaseType,
                      StructureType, SequenceType,
                      GridType)
 from ..lib import encode, quote, __version__, NUMPY_TO_DAP2_TYPEMAP
 from .lib import BaseResponse
 
 
@@ -37,15 +41,18 @@
         self.headers.extend([
             ('Content-description', 'dods_das'),
             ('Content-type', 'text/plain; charset=ascii'),
         ])
 
     def __iter__(self):
         for line in das(self.dataset):
-            yield line.encode('ascii')
+            try:
+                yield line.encode('ascii')
+            except UnicodeDecodeError:
+                yield line.encode('UTF-8')
 
 
 @singledispatch
 def das(var, level=0):
     """Single dispatcher that generates the DAS response."""
     raise StopIteration
 
@@ -84,16 +91,17 @@
 @das.register(BaseType)
 @das.register(GridType)
 def _basetypegridtype(var, level=0):
     yield '{indent}{name} {{\n'.format(indent=level*INDENT, name=var.name)
 
     for attr in sorted(var.attributes.keys()):
         values = var.attributes[attr]
-        for line in build_attributes(attr, values, level+1):
-            yield line
+        if np.asarray(values).size > 0:
+            for line in build_attributes(attr, values, level+1):
+                yield line
     yield '{indent}}}\n'.format(indent=level*INDENT)
 
 
 def build_attributes(attr, values, level=0):
     """Recursive function to build the DAS."""
     # check for metadata
     if isinstance(values, dict):
```

### Comparing `Pydap-3.2.2/src/pydap/responses/dds.py` & `pydap-3.4.0/src/pydap/responses/dds.py`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/src/pydap/model.py` & `pydap-3.4.0/src/pydap/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""This is the Pydap data model, an implementation of the Data Access Protocol
+"""This is the pydap data model, an implementation of the Data Access Protocol
 data model written in Python.
 
 The model is composed of a base object which represents data, the `BaseType`,
 and by objects which can hold other objects, all derived from `StructureType`.
 Here's a simple example of a `BaseType` variable::
 
     >>> import numpy as np
@@ -119,15 +119,15 @@
     >>> cast['salinity'] = BaseType('salinity', units='psu')
     >>> cast['id'] = BaseType('id')
     >>> cast.data = np.array([(10., 17., 35., '1'), (20., 15., 35., '2')],
     ...     dtype=np.dtype([('depth', np.float32), ('temperature', np.float32),
     ...     ('salinity', np.float32), ('id', np.dtype('|S1'))]))
 
 Note that the data in this case is attributed to the `SequenceType`, and is
-composed of a series of values for each of the children.  Pydap `SequenceType`
+composed of a series of values for each of the children.  pydap `SequenceType`
 obects are very flexible. Data can be accessed by iterating over the object::
 
     >>> for record in cast.iterdata():
     ...     print(record)
     (10.0, 17.0, 35.0, '1')
     (20.0, 15.0, 35.0, '2')
 
@@ -168,17 +168,20 @@
 """
 
 import operator
 import copy
 from six.moves import reduce, map
 from six import string_types
 import numpy as np
-from collections import OrderedDict, Mapping
+from collections import OrderedDict
 import warnings
-
+try:
+    from collections.abc import Mapping
+except ImportError:
+    from collections import Mapping
 from .lib import quote, decode_np_strings
 
 
 __all__ = [
     'BaseType', 'StructureType', 'DatasetType', 'SequenceType', 'GridType']
 
 
@@ -205,14 +208,15 @@
 
     # The id.
     def _set_id(self, id):
         self._id = id
 
         # Update children id.
         for child in self.children():
+            #pass
             child.id = '%s.%s' % (id, child.name)
 
     def _get_id(self):
         return self._id
 
     id = property(_get_id, _set_id)
 
@@ -314,14 +318,16 @@
     def __lt__(self, other):
         return self.data < other
 
     # Implement the sequence and iter protocols.
     def __getitem__(self, index):
         out = copy.copy(self)
         out.data = self._get_data_index(index)
+        if type(self.data).__name__ == 'BaseProxyDap4':
+            out.attributes['checksum'] = self.data.checksum
         return out
 
     def __len__(self):
         return len(self.data)
 
     def __iter__(self):
         if self._is_string_dtype:
@@ -339,15 +345,15 @@
         """ This method was added to mimic new SequenceType method."""
         return iter(self)
 
     def __array__(self):
         return self._get_data_index()
 
     def _get_data_index(self, index=Ellipsis):
-        if self._is_string_dtype:
+        if self._is_string_dtype and isinstance(self._data, np.ndarray):
             return np.vectorize(decode_np_strings)(self._data[index])
         else:
             return self._data[index]
 
     def _get_data(self):
         return self._data
 
@@ -376,15 +382,15 @@
         return '<%s with children %s>' % (
             type(self).__name__, ', '.join(map(repr, self._visible_keys)))
 
     def __getattr__(self, attr):
         """Lazy shortcut return children."""
         try:
             return self[attr]
-        except:
+        except Exception:
             return DapType.__getattr__(self, attr)
 
     def __contains__(self, key):
         return (key in self._visible_keys)
 
     # __iter__, __getitem__, __len__ are required for Mapping
     # From these, keys, items, values, get, __eq__,
@@ -403,15 +409,15 @@
         try:
             return self._dict[quote(key)]
         except KeyError:
             splitted = key.split('.')
             if len(splitted) > 1:
                 try:
                     return self[splitted[0]]['.'.join(splitted[1:])]
-                except KeyError:
+                except (KeyError, IndexError):
                     return self['.'.join(splitted[1:])]
             else:
                 raise
 
     def _getitem_string_tuple(self, key):
         """ Assume that key is a tuple of strings """
         out = type(self)(self.name, data=self.data,
@@ -419,17 +425,15 @@
         for name in key:
             out[name] = copy.copy(self._getitem_string(name))
         return out
 
     def __getitem__(self, key):
         if isinstance(key, string_types):
             return self._getitem_string(key)
-        elif (isinstance(key, tuple) and
-              all(isinstance(name, string_types)
-                  for name in key)):
+        elif isinstance(key, tuple) and all(isinstance(name, string_types) for name in key):
             out = copy.copy(self)
             out._visible_keys = list(key)
             return out
         else:
             raise KeyError(key)
 
     def __len__(self):
@@ -468,23 +472,27 @@
         return [var.data for var in self.children()]
 
     def _set_data(self, data):
         for col, var in zip(data, self.children()):
             var.data = col
     data = property(_get_data, _set_data)
 
+    def __shallowcopy__(self):
+        out = type(self)(self.name, self.attributes.copy())
+        out.id = self.id
+        return out
+
     def __copy__(self):
         """Return a lightweight copy of the Structure.
 
         The method will return a new Structure with cloned children, but any
         data object are not copied.
 
         """
-        out = type(self)(self.name, self.attributes.copy())
-        out.id = self.id
+        out = self.__shallowcopy__()
 
         # Clone all children too.
         for child in self._dict.values():
             out[child.name] = copy.copy(child)
         return out
 
 
@@ -500,24 +508,35 @@
         'B'
 
     """
 
     def __setitem__(self, key, item):
         StructureType.__setitem__(self, key, item)
 
-        # The dataset name does not goes into the children ids.
+        # The dataset name does not go into the children ids.
         item.id = item.name
 
     def _set_id(self, id):
         """The dataset name is not included in the children ids."""
         self._id = id
 
         for child in self.children():
             child.id = child.name
 
+    def to_netcdf(self, *args, **kwargs):
+        try:
+            from .apis.netcdf4 import NetCDF
+            return NetCDF(self, *args, **kwargs)
+        except ImportError:
+            raise NotImplementedError('.to_netcdf requires the netCDF4 '
+                                      'package.')
+
+    def change_order(self, order):
+        self._dict = OrderedDict((k, self._dict[k]) for k in order)
+
 
 class SequenceType(StructureType):
 
     """A container that stores data in a Numpy array.
 
     Here's a standard dataset for testing sequential data:
 
@@ -620,50 +639,50 @@
     data = property(_get_data, _set_data)
 
     def iterdata(self):
         for line in self.data:
             yield tuple(map(decode_np_strings, line))
 
     def __iter__(self):
-        # This method should be removed in Pydap 3.4
-        warnings.warn('Starting with Pydap 3.4 '
+        # This method should be removed in pydap 3.4
+        warnings.warn('Starting with pydap 3.4 '
                       '``for val in sequence: ...`` '
                       'will give children names. '
                       'To iterate over data the construct '
                       '``for val in sequence.iterdata(): ...``'
                       'is available now and will be supported in the'
                       'future to iterate over data.',
                       PendingDeprecationWarning)
         return self.iterdata()
 
     def __len__(self):
-        # This method should be removed in Pydap 3.4
-        warnings.warn('Starting with Pydap 3.4, '
+        # This method should be removed in pydap 3.4
+        warnings.warn('Starting with pydap 3.4, '
                       '``len(sequence)`` will give '
                       'the number of children and not the '
                       'length of the data.',
                       PendingDeprecationWarning)
         return len(self.data)
 
     def items(self):
-        # This method should be removed in Pydap 3.4
+        # This method should be removed in pydap 3.4
         for key in self._visible_keys:
             yield (key, self[key])
 
     def values(self):
-        # This method should be removed in Pydap 3.4
+        # This method should be removed in pydap 3.4
         for key in self._visible_keys:
             yield self[key]
 
     def keys(self):
-        # This method should be removed in Pydap 3.4
+        # This method should be removed in pydap 3.4
         return iter(self._visible_keys)
 
     def __contains__(self, key):
-        # This method should be removed in Pydap 3.4
+        # This method should be removed in pydap 3.4
         return (key in self._visible_keys)
 
     def __getitem__(self, key):
         # If key is a string, return child with the corresponding data.
         if isinstance(key, string_types):
             return self._getitem_string(key)
 
@@ -677,32 +696,21 @@
 
         # Else return a new `SequenceType` with the data sliced.
         else:
             out = copy.copy(self)
             out.data = self.data[key]
             return out
 
-    def __copy__(self):
-        """Return a lightweight copy of the Sequence.
-
-        The method will return a new Sequence with cloned children, but any
-        data object are not copied.
-
-        """
+    def __shallowcopy__(self):
         out = type(self)(self.name, self.data, self.attributes.copy())
         out.id = self.id
-
-        # Clone children too.
-        for child in self.children():
-            out[child.name] = copy.copy(child)
         return out
 
 
 class GridType(StructureType):
-
     """A Grid container.
 
     The Grid is a Structure with an array and the corresponding axes.
 
     """
 
     def __init__(self, name='nameless', attributes=None, **kwargs):
@@ -717,30 +725,30 @@
 
     def __getitem__(self, key):
         # Return a child.
         if isinstance(key, string_types):
             return self._getitem_string(key)
 
         # Return a new `GridType` with part of the data.
-        elif (isinstance(key, tuple) and
-              all(isinstance(name, string_types)
-                  for name in key)):
+        elif isinstance(key, tuple) and all(isinstance(name, string_types) for name in key):
             out = self._getitem_string_tuple(key)
             for var in out.children():
                 var.data = self[var.name].data
             return out
         else:
             if not self.output_grid:
                 return self.array[key]
 
             if not isinstance(key, tuple):
                 key = (key,)
 
             out = copy.copy(self)
             for var, slice_ in zip(out.children(), [key] + list(key)):
+                if type(self.data).__name__ == 'BaseProxyDap4':
+                    pass
                 var.data = self[var.name].data[slice_]
             return out
 
     @property
     def dtype(self):
         """Return the first children dtype."""
         return self.array.dtype
@@ -778,7 +786,11 @@
         """Return the axes in an ordered dict."""
         return OrderedDict([(k, self[k]) for k in self.keys()][1:])
 
     @property
     def dimensions(self):
         """Return the name of the axes."""
         return tuple(list(self.keys())[1:])
+
+
+class MapType(StructureType):
+    pass
```

### Comparing `Pydap-3.2.2/src/pydap/handlers/lib.py` & `pydap-3.4.0/src/pydap/handlers/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Basic functions for handlers.
 
-Pydap handlers are responsible for reading data in different formats -- NetCDF,
+pydap handlers are responsible for reading data in different formats -- NetCDF,
 SQL databases, CSV files, etc. -- and convert them into the internal data model
 so that the data may be served using different responses.
 
 """
 
 from __future__ import division
 
@@ -59,42 +59,47 @@
     opts_dict = dict((r.name, r.load())
                      for r in working_set.iter_entry_points(entry_points)
                      if not r.module_name.startswith(package))
     base_dict.update(opts_dict)
     return base_dict.values()
 
 
-def get_handler(filepath, handlers=None):
+def get_handler(filepath, handlers=None, instantiate=True):
     """Given a filepath, return the corresponding instantiated handler."""
     # Check each handler to see which one handles this file.
     for handler in handlers or load_handlers():
         p = re.compile(handler.extensions)
         if p.match(filepath):
+            # only check if extension is supported - don't return instance
+            if not instantiate:
+                return None
             return handler(filepath)
 
     raise ExtensionNotSupportedError(
         'No handler available for file {filepath}.'.format(filepath=filepath))
 
 
 class BaseHandler(object):
 
-    """Base class for Pydap handlers.
+    """Base class for pydap handlers.
 
     Handlers are WSGI applications that parse the client request and build the
     corresponding dataset. The dataset is passed to proper Response (DDS, DAS,
     etc.)
 
     """
 
     # load all available responses
+#    import pdb; pdb.set_trace()
     responses = load_responses()
 
-    def __init__(self, dataset=None):
+    def __init__(self, dataset=None, gzip=False):
         self.dataset = dataset
         self.additional_headers = []
+        self._gzip = gzip
 
     def __call__(self, environ, start_response):
         req = Request(environ)
         path, response = req.path.rsplit('.', 1)
         if response == 'das':
             req.query_string = ''
         projection, selection = parse_ce(req.query_string)
@@ -115,16 +120,18 @@
             # CORS for Javascript requests
             if response in CORS_RESPONSES:
                 res.headers.add('Access-Control-Allow-Origin', '*')
                 res.headers.add(
                     'Access-Control-Allow-Headers',
                     'Origin, X-Requested-With, Content-Type')
 
+            if self._gzip:
+                res.encode_content()
             return res(environ, start_response)
-        except:
+        except Exception:
             # should the exception be catched?
             if environ.get('x-wsgiorg.throw_errors'):
                 raise
             else:
                 res = ErrorResponse(info=sys.exc_info())
                 return res(environ, start_response)
 
@@ -217,19 +224,18 @@
         for i, (name, slice_) in enumerate(p):
             candidate = template[name]
 
             # add variable to target
             if isinstance(candidate, StructureType):
                 if name not in target.keys():
                     if i < len(p) - 1:
-                        # if there are more children to add we need to clear
-                        # the candidate so it has only explicitly added
-                        # children; also, Grids are degenerated into Structures
+                        # A shallow copy of the candidate is created
+                        candidate = candidate.__shallowcopy__()
+                        # Grids are degenerated into Structures
                         candidate = degenerate_grid_to_structure(candidate)
-                        candidate._visible_keys = []
                     target[name] = candidate
                 target, template = target[name], template[name]
             else:
                 target[name] = candidate
 
     # fix sequence data to include only variables that are in the sequence
     for seq in walk(out, SequenceType):
@@ -342,15 +348,15 @@
     def __getitem__(self, key):
         out = copy.copy(self)
 
         # return a child, and adjust the data so that only the corresponding
         # column is returned
         if isinstance(key, string_types):
             try:
-                col = list(self.template.keys()).index(key)
+                col = list(self.template._all_keys()).index(key)
             except ValueError:
                 raise KeyError(key)
             out.level += 1
             out.template = out.template[key]
             out.imap.append(deep_map(operator.itemgetter(col), out.level))
 
         # return a new sequence with the selected children
@@ -453,15 +459,15 @@
         target = template
         for level, token in enumerate(id1.split(".")):
             parent1 = target.id
             keys = list(target._all_keys())
             col = keys.index(token)
             target = target[token]
         a = operator.itemgetter(col)
-    except:
+    except Exception:
         raise ConstraintExpressionError(
             'Invalid constraint expression: "{expression}" '
             '("{id}" is not a valid variable)'.format(
                 expression=expression, id=id1))
 
     # if we're comparing two variables they must be on the same sequence, so
     # ``parent1`` must be equal to ``parent2``
@@ -471,15 +477,15 @@
         b = operator.itemgetter(col)
     else:
         try:
             value = ast.literal_eval(id2)
 
             def b(row):
                 return value
-        except:
+        except Exception:
             raise ConstraintExpressionError(
                 'Invalid constraint expression: "{expression}" '
                 '("{id}" is not valid)'.format(
                     expression=expression, id=id2))
 
     op = {
         '<':  operator.lt,
```

### Comparing `Pydap-3.2.2/src/pydap/handlers/netcdf/__init__.py` & `pydap-3.4.0/src/pydap/handlers/netcdf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-"""Pydap handler for NetCDF3/4 files."""
+"""pydap handler for NetCDF3/4 files."""
 
 import os
 import re
 import time
 from stat import ST_MTIME
 from email.utils import formatdate
 import numpy as np
 
 from pkg_resources import get_distribution
 
-from pydap.model import DatasetType, GridType, BaseType
-from pydap.handlers.lib import BaseHandler
-from pydap.exceptions import OpenFileError
+from ...model import DatasetType, GridType, BaseType
+from ..lib import BaseHandler
+from ...exceptions import OpenFileError
+from ...pycompat import suppress
 
 from collections import OrderedDict
 
 # Check for netCDF4 presence:
-try:
-    from netCDF4 import Dataset as netcdf_file
+with suppress(ImportError):
+    try:
+        from netCDF4 import Dataset as netcdf_file
+
+        def attrs(var):
+            return dict((k, getattr(var, k)) for k in var.ncattrs())
+    except ImportError:
+        from scipy.io.netcdf import netcdf_file
 
-    def attrs(var):
-        return dict((k, getattr(var, k)) for k in var.ncattrs())
-except ImportError:
-    from scipy.io.netcdf import netcdf_file
-
-    def attrs(var):
-        return var._attributes
+        def attrs(var):
+            return var._attributes
 
 
 class NetCDFHandler(BaseHandler):
 
     """A simple handler for NetCDF files.
     Here's a standard dataset for testing sequential data:
     """
@@ -78,22 +80,35 @@
                                                             grid,
                                                             grid,
                                                             self.filepath),
                                                         vars[grid].dimensions,
                                                         attrs(vars[grid]))
                     # add maps
                     for dim in vars[grid].dimensions:
-                        self.dataset[grid][dim] = BaseType(dim, vars[dim][:],
+                        try:
+                            data = vars[dim][:]
+                            attributes = attrs(vars[dim])
+                        except KeyError:
+                            data = np.arange(dims[dim].size, dtype='i')
+                            attributes = None
+                        self.dataset[grid][dim] = BaseType(dim, data,
                                                            None,
-                                                           attrs(vars[dim]))
+                                                           attributes)
 
                 # add dims
                 for dim in dims:
-                    self.dataset[dim] = BaseType(dim, vars[dim][:], None,
-                                                 attrs(vars[dim]))
+                    try:
+                        data = vars[dim][:]
+                        attributes = attrs(vars[dim])
+                    except KeyError:
+                        data = np.arange(dims[dim].size, dtype='i')
+                        attributes = None
+                    self.dataset[dim] = BaseType(dim, data,
+                                                 None,
+                                                 attributes)
         except Exception as exc:
             raise
             message = 'Unable to open file %s: %s' % (filepath, exc)
             raise OpenFileError(message)
 
 
 class LazyVariable:
@@ -151,14 +166,17 @@
         return self[...]
 
     def __array__(self):
         return self[...]
 
     def __getitem__(self, key):
         with netcdf_file(self.filepath, 'r') as source:
+            # Avoid applying scale_factor, see
+            # https://github.com/pydap/pydap/issues/190
+            source.set_auto_scale(False)
             return (np.asarray(source[self.path][key])
                     .astype(self.dtype).reshape(self._reshape))
 
     def reshape(self, *args):
         if len(args) > 1:
             self._reshape = args
         else:
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_cas_esgf.py` & `pydap-3.4.0/src/pydap/tests/test_cas_esgf.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 from pydap.cas import esgf
 import requests
 import numpy as np
 import os
 import pytest
 
 
-url = ('http://aims3.llnl.gov/thredds/dodsC/'
-       'cmip5_css02_data/cmip5/output1/CCCma/CanCM4/'
-       'decadal1995/fx/atmos/fx/r0i0p0/orog/1/'
-       'orog_fx_CanCM4_decadal1995_r0i0p0.nc')
+url = ('http://esgf-data.ucar.edu/thredds/dodsC/cmip5/output1/'
+       'NCAR/CCSM4/historical/fx/atmos/fx/r0i0p0/v20130312/orog/'
+       'orog_fx_CCSM4_historical_r0i0p0.nc')
 test_url = url + '.dods?orog[0:1:4][0:1:4]'
 
 
 @pytest.mark.auth
 @pytest.mark.prod_url
 @pytest.mark.skipif(not (os.environ.get('OPENID_ESGF_NO_REG') and
                          os.environ.get('PASSWORD_ESGF_NO_REG')),
@@ -51,16 +50,15 @@
     open and url if and only if requests is able to
     open the same url.
     """
     session = esgf.setup_session(os.environ.get('OPENID_ESGF'),
                                  os.environ.get('PASSWORD_ESGF'),
                                  check_url=url)
 
-    res = requests.get(test_url, cookies=session.cookies,
-                       verify=False)
+    res = requests.get(test_url, cookies=session.cookies)
     assert(res.status_code == 200)
     res.close()
 
     res = pydap.net.follow_redirect(test_url, session=session)
     assert(res.status_code == 200)
 
 
@@ -77,15 +75,15 @@
 
     # Ensure authentication:
     res = pydap.net.follow_redirect(test_url, session=session)
     assert(res.status_code == 200)
 
     dataset = open_url(url, session=session)
     data = dataset['lon'][:5]
-    expected_data = np.array([0.0, 2.8125, 5.625, 8.4375, 11.25])
+    expected_data = np.array([0., 1.25, 2.5, 3.75, 5.])
     assert(np.isclose(data, expected_data).all())
 
 
 @pytest.mark.auth
 @pytest.mark.prod_url
 @pytest.mark.skipif(not (os.environ.get('OPENID_ESGF') and
                          os.environ.get('PASSWORD_ESGF')),
@@ -96,20 +94,17 @@
                                  os.environ.get('PASSWORD_ESGF'),
                                  check_url=url)
     # Ensure authentication:
     res = pydap.net.follow_redirect(test_url, session=session)
     assert(res.status_code == 200)
 
     dataset = open_url(url, session=session, output_grid=False)
-    data = dataset['orog'][50:55, 50:55]
-    expected_data = [[197.70425, 16.319595, 0.0, 0.0, 0.0],
-                     [0.0, 0.0, 0.0, 0.0, 0.0],
-                     [0.0, 0.0, 0.0, 0.0, 0.0],
-                     [677.014, 628.29675, 551.06, 455.5758, 343.7354],
-                     [1268.3304, 1287.9553, 1161.0402, 978.3153, 809.143]]
+    data = dataset['orog'][103:105, 100:102]
+    expected_data = [[271.36645508, 166.85339355],
+                     [304.22286987, 178.85267639]]
     assert(np.isclose(data, expected_data).all())
 
 
 @pytest.mark.auth
 @pytest.mark.prod_url
 @pytest.mark.skipif(not (os.environ.get('OPENID_ESGF_CEDA') and
                          os.environ.get('USERNAME_ESGF_CEDA') and
@@ -123,14 +118,11 @@
                     check_url=url,
                     username=os.environ.get('USERNAME_ESGF_CEDA'))
     # Ensure authentication:
     res = pydap.net.follow_redirect(test_url, session=session)
     assert(res.status_code == 200)
 
     dataset = open_url(url, session=session, output_grid=False)
-    data = dataset['orog'][50:55, 50:55]
-    expected_data = [[197.70425, 16.319595, 0.0, 0.0, 0.0],
-                     [0.0, 0.0, 0.0, 0.0, 0.0],
-                     [0.0, 0.0, 0.0, 0.0, 0.0],
-                     [677.014, 628.29675, 551.06, 455.5758, 343.7354],
-                     [1268.3304, 1287.9553, 1161.0402, 978.3153, 809.143]]
+    data = dataset['orog'][103:105, 100:102]
+    expected_data = [[271.36645508, 166.85339355],
+                     [304.22286987, 178.85267639]]
     assert(np.isclose(data, expected_data).all())
```

### Comparing `Pydap-3.2.2/src/pydap/tests/datasets.py` & `pydap-3.4.0/src/pydap/tests/datasets.py`

 * *Files 7% similar despite different names*

```diff
@@ -59,17 +59,16 @@
 # encoding for the DODS response.
 SimpleArray = DatasetType("SimpleArray")
 SimpleArray["byte"] = BaseType("byte", np.arange(5, dtype=np.ubyte))
 SimpleArray["string"] = BaseType("string", np.array(["one", "two"]))
 SimpleArray["short"] = BaseType("short", np.array(1, dtype="h"))
 
 
-DODS = os.path.join(
-    os.path.dirname(__file__), 'rainfall_time_malaysia.cdp.dods')
-DAS = os.path.join(os.path.dirname(__file__), 'rainfall_time_malaysia.cdp.das')
+DODS = os.path.join(os.path.dirname(__file__), 'data/rainfall_time_malaysia.cdp.dods')
+DAS = os.path.join(os.path.dirname(__file__), 'data/rainfall_time_malaysia.cdp.das')
 dapper = open_file(DODS, DAS)
 
 
 # dataset from http://test.opendap.org:8080/dods/dts/D1.asc
 D1 = DatasetType('EOSDB.DBO', type='Drifters')
 D1['Drifters'] = SequenceType('Drifters')
 D1['Drifters']['instrument_id'] = BaseType('instrument_id')
@@ -104,15 +103,15 @@
 SimpleStructure['types']['ui16'] = BaseType('ui16', np.array(10, np.uint16))
 SimpleStructure['types']['f32'] = BaseType('f32', np.array(100.0, np.float32))
 SimpleStructure['types']['f64'] = BaseType('f64', np.array(1000., np.float64))
 SimpleStructure['types']['s'] = BaseType(
     's', np.array("This is a data test string (pass 0)."))
 SimpleStructure['types']['u'] = BaseType('u', np.array("http://www.dods.org"))
 SimpleStructure['types']['U'] = BaseType('U', np.array(u"test unicode",
-                                                       np.unicode))
+                                                       str))
 
 
 # test grid
 rain = DatasetType('test')
 rain['rain'] = GridType('rain')
 rain['rain']['rain'] = BaseType(
     'rain', np.arange(6).reshape(2, 3), dimensions=('y', 'x'))
@@ -175,7 +174,19 @@
 SimpleGrid["SimpleGrid"] = GridType("SimpleGrid")
 SimpleGrid["SimpleGrid"]["SimpleGrid"] = BaseType(
     "SimpleGrid", np.arange(6).reshape(2, 3), dimensions=("y", "x"))
 SimpleGrid["x"] = SimpleGrid["SimpleGrid"]["x"] = BaseType(
     "x", np.arange(3), axis="X", units="degrees_east")
 SimpleGrid["y"] = SimpleGrid["SimpleGrid"]["y"] = BaseType(
     "y", np.arange(2), axis="Y", units="degrees_north")
+
+
+# a faulty grid
+FaultyGrid = DatasetType(
+    "FaultyGrid", description="A faulty grid for testing.")
+FaultyGrid["FaultyGrid"] = GridType("FaultyGrid")
+FaultyGrid["FaultyGrid"]["FaultyGrid"] = BaseType(
+    "FaultyGrid", np.arange(6).reshape(2, 3), dimensions=("y", "x"))
+FaultyGrid["x"] = FaultyGrid["FaultyGrid"]["x"] = BaseType(
+    "x", np.arange(3), axis="X", code=1)
+FaultyGrid["y"] = FaultyGrid["FaultyGrid"]["y"] = BaseType(
+    "y", np.arange(2), axis="Y", code=np.int32([]))
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_lib.py` & `pydap-3.4.0/src/pydap/tests/test_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,17 @@
         """Unicode objects are encoded just like strings."""
         self.assertEqual(encode(u"test"), '"test"')
 
     def test_obj(self):
         """Other objects are encoded according to their ``repr``."""
         self.assertEqual(encode({}), '"{}"')
 
+    def test_numpy_string(self):
+        self.assertEqual(encode(np.array('1', dtype='<U1')), '"1"')
+
 
 class TestFixSlice(unittest.TestCase):
 
     """Test the ``fix_slice`` function."""
 
     def test_not_tuple(self):
         """Non tuples should be converted and handled correctly."""
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_handlers_dap.py` & `pydap-3.4.0/src/pydap/tests/test_handlers_dap.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Test the DAP handler, which forms the core of the client."""
 
 import numpy as np
 from pydap.model import StructureType, GridType, DatasetType, BaseType
 from pydap.handlers.lib import BaseHandler, ConstraintExpression
-from pydap.handlers.dap import DAPHandler, BaseProxy, SequenceProxy
+from pydap.handlers.dap import DAPHandler, BaseProxyDap2, SequenceProxy
 from pydap.handlers.dap import find_pattern_in_string_iter
 from pydap.tests.datasets import (
     SimpleSequence, SimpleGrid, SimpleArray, VerySimpleSequence)
 
 import unittest
 try:
     from unittest.mock import patch
@@ -19,35 +19,71 @@
 
     """Test that the handler creates the correct dataset from a URL."""
 
     def setUp(self):
         """Create WSGI apps"""
         self.app1 = BaseHandler(SimpleGrid)
         self.app2 = BaseHandler(SimpleSequence)
+        self.app3 = BaseHandler(SimpleGrid, gzip=True)
 
     def test_grid(self):
         """Test that dataset has the correct data proxies for grids."""
         dataset = DAPHandler("http://localhost:8001/", self.app1).dataset
 
         self.assertEqual(list(dataset.keys()), ["SimpleGrid", "x", "y"])
         self.assertEqual(
             list(dataset.SimpleGrid.keys()), ["SimpleGrid", "x", "y"])
 
         # test one of the axis
-        self.assertIsInstance(dataset.SimpleGrid.x.data, BaseProxy)
+        self.assertIsInstance(dataset.SimpleGrid.x.data, BaseProxyDap2)
         self.assertEqual(
             dataset.SimpleGrid.x.data.baseurl, "http://localhost:8001/")
         self.assertEqual(dataset.SimpleGrid.x.data.id, "SimpleGrid.x")
         self.assertEqual(dataset.SimpleGrid.x.data.dtype, np.dtype('>i4'))
         self.assertEqual(dataset.SimpleGrid.x.data.shape, (3,))
         self.assertEqual(
             dataset.SimpleGrid.x.data.slice, (slice(None),))
 
         # test the grid
-        self.assertIsInstance(dataset.SimpleGrid.SimpleGrid.data, BaseProxy)
+        self.assertIsInstance(dataset.SimpleGrid.SimpleGrid.data, BaseProxyDap2)
+        self.assertEqual(
+            dataset.SimpleGrid.SimpleGrid.data.baseurl,
+            "http://localhost:8001/")
+        self.assertEqual(
+            dataset.SimpleGrid.SimpleGrid.data.id, "SimpleGrid.SimpleGrid")
+        self.assertEqual(
+            dataset.SimpleGrid.SimpleGrid.data.dtype, np.dtype('>i4'))
+        self.assertEqual(dataset.SimpleGrid.SimpleGrid.data.shape, (2, 3))
+        self.assertEqual(
+            dataset.SimpleGrid.SimpleGrid.data.slice,
+            (slice(None), slice(None)))
+        self.assertEqual(
+                repr(dataset.SimpleGrid[:]),
+                "<GridType with array 'SimpleGrid' and maps 'x', 'y'>")
+
+    def test_grid_gzip(self):
+        """Test that dataset has the correct data proxies for grids."""
+        dataset = DAPHandler("http://localhost:8001/", self.app3).dataset
+
+        self.assertEqual(list(dataset.keys()), ["SimpleGrid", "x", "y"])
+        self.assertEqual(
+            list(dataset.SimpleGrid.keys()), ["SimpleGrid", "x", "y"])
+
+        # test one of the axis
+        self.assertIsInstance(dataset.SimpleGrid.x.data, BaseProxyDap2)
+        self.assertEqual(
+            dataset.SimpleGrid.x.data.baseurl, "http://localhost:8001/")
+        self.assertEqual(dataset.SimpleGrid.x.data.id, "SimpleGrid.x")
+        self.assertEqual(dataset.SimpleGrid.x.data.dtype, np.dtype('>i4'))
+        self.assertEqual(dataset.SimpleGrid.x.data.shape, (3,))
+        self.assertEqual(
+            dataset.SimpleGrid.x.data.slice, (slice(None),))
+
+        # test the grid
+        self.assertIsInstance(dataset.SimpleGrid.SimpleGrid.data, BaseProxyDap2)
         self.assertEqual(
             dataset.SimpleGrid.SimpleGrid.data.baseurl,
             "http://localhost:8001/")
         self.assertEqual(
             dataset.SimpleGrid.SimpleGrid.data.id, "SimpleGrid.SimpleGrid")
         self.assertEqual(
             dataset.SimpleGrid.SimpleGrid.data.dtype, np.dtype('>i4'))
@@ -77,25 +113,25 @@
                              output_grid=False).dataset
 
         self.assertEqual(list(dataset.keys()), ["SimpleGrid", "x", "y"])
         self.assertEqual(
             list(dataset.SimpleGrid.keys()), ["SimpleGrid", "x", "y"])
 
         # test one of the axis
-        self.assertIsInstance(dataset.SimpleGrid.x.data, BaseProxy)
+        self.assertIsInstance(dataset.SimpleGrid.x.data, BaseProxyDap2)
         self.assertEqual(
             dataset.SimpleGrid.x.data.baseurl, "http://localhost:8001/")
         self.assertEqual(dataset.SimpleGrid.x.data.id, "SimpleGrid.x")
         self.assertEqual(dataset.SimpleGrid.x.data.dtype, np.dtype('>i4'))
         self.assertEqual(dataset.SimpleGrid.x.data.shape, (3,))
         self.assertEqual(
             dataset.SimpleGrid.x.data.slice, (slice(None),))
 
         # test the grid
-        self.assertIsInstance(dataset.SimpleGrid.SimpleGrid.data, BaseProxy)
+        self.assertIsInstance(dataset.SimpleGrid.SimpleGrid.data, BaseProxyDap2)
         self.assertEqual(
             dataset.SimpleGrid.SimpleGrid.data.baseurl,
             "http://localhost:8001/")
         self.assertEqual(
             dataset.SimpleGrid.SimpleGrid.data.id, "SimpleGrid.SimpleGrid")
         self.assertEqual(
             dataset.SimpleGrid.SimpleGrid.data.dtype, np.dtype('>i4'))
@@ -209,15 +245,15 @@
 
     """Test `BaseProxy` objects."""
 
     def setUp(self):
         """Create a WSGI app"""
         self.app = BaseHandler(SimpleArray)
 
-        self.data = BaseProxy(
+        self.data = BaseProxyDap2(
                               "http://localhost:8001/", "byte",
                               np.dtype("B"), (5,),
                               application=self.app)
 
     def test_repr(self):
         """Test the object representation."""
         self.assertEqual(
@@ -264,15 +300,15 @@
 
     """Test `BaseProxy` objects with short dtype."""
 
     def setUp(self):
         """Create a WSGI app with array data"""
         self.app = BaseHandler(SimpleArray)
 
-        self.data = BaseProxy(
+        self.data = BaseProxyDap2(
                               "http://localhost:8001/", "short",
                               np.dtype(">h"), (),
                               application=self.app)
 
     def test_getitem(self):
         """Test the ``__getitem__`` method."""
         np.testing.assert_array_equal(self.data[:], np.array(1))
@@ -285,15 +321,15 @@
 
     def setUp(self):
         """Create a WSGI app with array data"""
         dataset = DatasetType("test")
         dataset["s"] = BaseType("s", np.array(["one", "two", "three"]))
         self.app = BaseHandler(dataset)
 
-        self.data = BaseProxy(
+        self.data = BaseProxyDap2(
                               "http://localhost:8001/", "s",
                               np.dtype("|S5"), (3,), application=self.app)
 
     def test_getitem(self):
         """Test the ``__getitem__`` method."""
         np.testing.assert_array_equal(
             self.data[:], np.array(["one", "two", "three"], dtype='S'))
@@ -490,15 +526,15 @@
     def setUp(self):
         """Create a WSGI app with array data"""
         dataset = DatasetType("test")
         data = np.array("This is a test", dtype='S')
         dataset["s"] = BaseType("s", data)
         self.app = BaseHandler(dataset)
 
-        self.data = BaseProxy(
+        self.data = BaseProxyDap2(
                               "http://localhost:8001/", "s",
                               np.dtype("|S14"), (), application=self.app)
 
     def test_getitem(self):
         """Test the ``__getitem__`` method."""
         np.testing.assert_array_equal(self.data[:],
                                       "This is a test")
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_D1.py` & `pydap-3.4.0/src/pydap/tests/test_D1.py`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/src/pydap/tests/test_iter_data.py` & `pydap-3.4.0/src/pydap/tests/test_iter_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,52 +115,62 @@
     filtered = simple_object[simple_object["byte"] > 1]
     filtered = filtered[filtered["byte"] < 6]
     filtered = filtered[::2]
     assert ([tuple(row) for row in filtered] ==
             [(2, 3, 30.), (4, 5, 50.)])
 
 
+def test_combined_other(simple_array, simple_object):
+    filtered = simple_array[['int', 'float']][simple_array["byte"] < 2]
+    assert ([tuple(row) for row in filtered] ==
+            [(1, 10.), (2, 20.)])
+
+    filtered = simple_object[['int', 'float']][simple_object["byte"] < 2]
+    assert ([tuple(row) for row in filtered] ==
+            [(1, 10.), (2, 20.)])
+
+
 @pytest.fixture
 def nested_data():
-        shallow_data = [(1, 1, 1), (2, 4, 4),
-                        (3, 6, 9), (4, 8, 16)]
-        deep_data = [[(10, 11, 12), (21, 22, 23)],
-                     [(15, 16, 17)],
-                     [],
-                     [(31, 32, 33), (41, 42, 43),
-                      (51, 52, 53), (61, 62, 63)]]
-        nested = [x + (deep_data[x_id],)
-                  for x_id, x
-                  in enumerate(shallow_data)]
-        return nested
+    shallow_data = [(1, 1, 1), (2, 4, 4),
+                    (3, 6, 9), (4, 8, 16)]
+    deep_data = [[(10, 11, 12), (21, 22, 23)],
+                 [(15, 16, 17)],
+                 [],
+                 [(31, 32, 33), (41, 42, 43),
+                  (51, 52, 53), (61, 62, 63)]]
+    nested = [x + (deep_data[x_id],)
+              for x_id, x
+              in enumerate(shallow_data)]
+    return nested
 
 
 @pytest.fixture
 def nested_dtype():
-        dtype = np.dtype([('a', '<i8'), ('b', '<i8'),
-                          ('c', '<i8'),
-                          ('d', np.dtype([('e', '<i8'),
-                                          ('f', '<i8'),
-                                          ('g', '<i8')]))])
-        return dtype
+    dtype = np.dtype([('a', '<i8'), ('b', '<i8'),
+                      ('c', '<i8'),
+                      ('d', np.dtype([('e', '<i8'),
+                                      ('f', '<i8'),
+                                      ('g', '<i8')]))])
+    return dtype
 
 
 @pytest.fixture
 def nested_object(nested_data):
-        name = 'nameless'
-        dataset = DatasetType(name)
-        seq = dataset['nested'] = SequenceType('nested')
-        for var in ['a', 'b', 'c']:
-            seq[var] = BaseType(var)
-        seq['d'] = SequenceType('d')
-        for var in ['e', 'f', 'g']:
-            seq['d'][var] = BaseType(var)
+    name = 'nameless'
+    dataset = DatasetType(name)
+    seq = dataset['nested'] = SequenceType('nested')
+    for var in ['a', 'b', 'c']:
+        seq[var] = BaseType(var)
+    seq['d'] = SequenceType('d')
+    for var in ['e', 'f', 'g']:
+        seq['d'][var] = BaseType(var)
 
-        nested = IterData(nested_data, seq)
-        return nested
+    nested = IterData(nested_data, seq)
+    return nested
 
 
 def test_nested_iter(nested_data, nested_object):
     assert ([tuple(row) for row in nested_object] ==
             nested_data)
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_wsgi_ssf.py` & `pydap-3.4.0/src/pydap/tests/test_wsgi_ssf.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         # now test a DDS response
         with self.assertRaises(KeyError):
             app.get("/.dds?non_existing_function(sequence)")
 
     def test_no_parsed_response(self):
         """Test that non-parsed responses work or raise error.
 
-        Pydap returns WSGI responses that contain the "parsed" dataset, so it
+        pydap returns WSGI responses that contain the "parsed" dataset, so it
         can be manipulated by middleware.
 
         """
         app = App(
             ServerSideFunctions(Accumulator(BaseHandler(SimpleGrid))))
 
         # a normal request should work, even though server-side functions are
```

### Comparing `Pydap-3.2.2/src/pydap/tests/rainfall_time_malaysia.cdp.dds` & `pydap-3.4.0/src/pydap/tests/data/rainfall_time_malaysia.cdp.dds`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/src/pydap/tests/test_responses_lib.py` & `pydap-3.4.0/src/pydap/tests/test_responses_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     """Test that responses are loaded correctly."""
 
     def setUp(self):
         """Load all available responses.
 
         At least the DDS, DAS, DODS, HTML, ASC and version responses should be
-        loaded, since they are included in Pydap. Other third-party responses
+        loaded, since they are included in pydap. Other third-party responses
         may also be present.
 
         """
         self.responses = load_responses()
 
     def test_responses_das(self):
         """Test that the DAS response is loaded."""
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_responses_dods.py` & `pydap-3.4.0/src/pydap/tests/test_responses_dods.py`

 * *Files 6% similar despite different names*

```diff
@@ -177,36 +177,36 @@
     } types;
 } SimpleStructure;""")
 
         expected = OrderedDict([
             # -10 signed byte upconv. to Int32 for transfer
             ('b', (np.array(-10, dtype=np.byte)
                    .astype('>i')
-                   .tostring())),
+                   .tobytes())),
             # 10 usigned byte padded to multiple of 4 bytes for transfer
             ('ub', (np.array(10, dtype=np.ubyte)
-                    .tostring()) + b'\x00\x00\x00'),
+                    .tobytes()) + b'\x00\x00\x00'),
             ('i32', (np.array(-10, dtype=np.int32)
-                     .astype('>i').tostring())),
+                     .astype('>i').tobytes())),
             ('ui32', (np.array(10, dtype=np.uint32)
-                      .astype('>I').tostring())),
+                      .astype('>I').tobytes())),
             # -10 int16 upconv. to int32 for transfer
             ('i16', (np.array(-10, dtype=np.int16)
                      .astype('>i')
-                     .newbyteorder('>').tostring())),
+                     .newbyteorder('>').tobytes())),
             # 10 uint16 upconv. to uint32 for transfer
             ('ui16', (np.array(10, dtype=np.uint16)
                       .astype('>I')
-                      .tostring())),
+                      .tobytes())),
             ('f32', (np.array(100, dtype=np.float32)
                      .astype('>f')
-                     .tostring())),
+                     .tobytes())),
             ('f64', (np.array(1000, dtype=np.float64)
                      .astype('>d')
-                     .tostring())),
+                     .tobytes())),
             ('s', b'\x00\x00\x00$This is a data test string (pass 0).\x00'),
             ('u', b'\x00\x00\x13http://www.dods.org\x00'),
             ('U', b'\x00\x00\x00\x0ctest unicode')])
 
         for key in expected:
             string = expected[key]
             assert xdrdata.startswith(string)
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_responses_error.py` & `pydap-3.4.0/src/pydap/tests/test_responses_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class TestErrorResponse(unittest.TestCase):
     def setUp(self):
         # create an exception that would happen in runtime
         try:
             1/0
-        except:
+        except Exception:
             error = ErrorResponse(sys.exc_info())
 
         req = Request.blank('/')
         self.res = req.get_response(error)
 
     def test_status(self):
         self.assertEqual(self.res.status, "500 Internal Error")
@@ -30,15 +30,16 @@
         self.assertEqual(self.res.headers['Content-Type'],
                          'text/plain; charset=utf-8')
         self.assertEqual(self.res.headers['Content-description'], 'dods_error')
         self.assertEqual(self.res.headers['XDODS-Server'],
                          'pydap/' + __version__)
 
     def test_body(self):
-        self.assertRegexpMatches(self.res.text, r"""Error {
+        self.assertRegex(self.res.text, r"""Error {
     code = -1;
     message = "Traceback \(most recent call last\):
   File .*
-    1/0
-ZeroDivisionError:( integer)? division( or modulo)? by zero
+    1\/0
+(    \~\^\~
+)?ZeroDivisionError:( integer)? division( or modulo)? by zero
 ";
 }""")
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_exceptions.py` & `pydap-3.4.0/src/pydap/tests/test_exceptions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-"""Test Pydap base exception."""
+"""Test pydap base exception."""
 
 from pydap.exceptions import DapError
 import unittest
 
 
 class TestExceptions(unittest.TestCase):
 
-    """Test Pydap base exception.
+    """Test pydap base exception.
 
     Other exceptions behave exactly like the superclass, differing only by
     name, so no testing is required.
 
     """
 
     def test_dap_error(self):
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_special_chars.py` & `pydap-3.4.0/src/pydap/tests/test_special_chars.py`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/src/pydap/tests/test_constrain.py` & `pydap-3.4.0/src/pydap/tests/test_constrain.py`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/src/pydap/tests/test_dapper.py` & `pydap-3.4.0/src/pydap/tests/test_dapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This is an example of a Dapper-compliant dataset.
 
 """
 import unittest
-from pydap.parsers.dds import build_dataset
+from pydap.parsers.dds import dds_to_dataset
 from pydap.parsers.das import parse_das, add_attributes
 
 
 DDS = """Dataset {
     Sequence {
         Float32 lat;
         Float64 time;
@@ -143,14 +143,14 @@
         Float32 missing_value NaN;
     }
 }"""
 
 
 class TestDapper(unittest.TestCase):
     def setUp(self):
-        dataset = build_dataset(DDS)
+        dataset = dds_to_dataset(DDS)
         attributes = parse_das(DAS)
         self.dataset = add_attributes(dataset, attributes)
 
     def test_parse(self):
         self.assertEqual(list(self.dataset.keys()),
                          ['location', 'constrained_ranges'])
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_responses_dds.py` & `pydap-3.4.0/src/pydap/tests/test_responses_dds.py`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/src/pydap/tests/rainfall_time_malaysia.cdp.dods` & `pydap-3.4.0/src/pydap/tests/data/rainfall_time_malaysia.cdp.dods`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/src/pydap/tests/test_handlers_lib.py` & `pydap-3.4.0/src/pydap/tests/test_handlers_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     """Test handler loading."""
 
     def test_load_handlers(self):
         """Test that handlers can be loaded correctly.
 
         We use a mock working set, since by default no handlers are installed
-        with Pydap.
+        with pydap.
 
         """
         handlers = load_handlers(MockWorkingSet())
         self.assertTrue(MockHandler in handlers)
 
     def test_get_handler(self):
         """Test that we can load a specific handler."""
@@ -87,15 +87,15 @@
         res = self.app.get("/.das?byte")
         self.assertEqual(res.text, das)
 
     def test_exception(self):
         """
         Test exception handling.
 
-        By default Pydap will capture all exceptions and return a formatted
+        By default pydap will capture all exceptions and return a formatted
         error response.
 
         """
         with self.assertRaises(AppError):
             self.app.get("/.foo")
 
     def test_exception_non_captured(self):
@@ -116,15 +116,15 @@
 class TestApplySelection(unittest.TestCase):
 
     """Test function that applies selections to the dataset."""
 
     def setUp(self):
         """Build our own sequence.
 
-        Pydap uses lightweight copies of objects that share data. This breaks
+        pydap uses lightweight copies of objects that share data. This breaks
         unit tests since the same objects are reused for tests.
 
         """
         # make a dataset with its own data
         self.dataset = copy.copy(SimpleSequence)
         self.dataset.cast.data = SimpleSequence.cast.data.copy()
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_responses_das.py` & `pydap-3.4.0/src/pydap/tests/test_responses_das.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Test the DAS response."""
 
 from webtest import TestApp as App
 from webob.headers import ResponseHeaders
 from pydap.lib import __version__
 from pydap.handlers.lib import BaseHandler
-from pydap.tests.datasets import SimpleSequence, SimpleGrid, SimpleStructure
+from pydap.tests.datasets import (
+    SimpleSequence, SimpleGrid, FaultyGrid, SimpleStructure
+)
 from pydap.responses.das import das
 
 import unittest
 
 
 class TestDASResponseSequence(unittest.TestCase):
 
@@ -103,14 +105,37 @@
         String axis "Y";
         String units "degrees_north";
     }
 }
 """)
 
 
+class TestDASResponseFaultyGrid(unittest.TestCase):
+
+    """Test the DAS response from a grid with empty properties."""
+
+    def test_body(self):
+        """Test the generated DAS response."""
+        app = App(BaseHandler(FaultyGrid))
+        res = app.get('/.das')
+        self.assertEqual(res.text, """Attributes {
+    String description "A faulty grid for testing.";
+    FaultyGrid {
+    }
+    x {
+        String axis "X";
+        Int32 code 1;
+    }
+    y {
+        String axis "Y";
+    }
+}
+""")
+
+
 class TestDASResponseStructure(unittest.TestCase):
 
     """The the DAS response from a structure."""
 
     def test_body(self):
         """Test the generated DAS response."""
         app = App(BaseHandler(SimpleStructure))
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_model.py` & `pydap-3.4.0/src/pydap/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
                          GridType, DapType)
 import pytest
 import warnings
 
 warnings.simplefilter('always')
 
 
-# Test the super class for Pydap types.
+# Test the super class for pydap types.
 def test_DapType_quote():
     """Test that names are properly quoted."""
     var = DapType("foo.bar[0]")
     assert (var.name == "foo%2Ebar%5B0%5D")
 
 
 def test_DapType_attributes():
@@ -68,15 +68,15 @@
 
 def test_DapType_children():
     """Test children method."""
     var = DapType("var")
     assert (var.children() == ())
 
 
-# Test the base Pydap type.
+# Test the base pydap type.
 def test_BaseType_no_data():
     """Test empty data and dimensions attributes."""
     var = BaseType("var")
     assert var.data is None
     assert (var.dimensions == ())
 
 
@@ -161,26 +161,29 @@
 def test_BaseType_array():
     """Test array conversion."""
     var = BaseType("var", np.arange(16).reshape(2, 2, 2, 2))
     np.testing.assert_array_equal(np.array(var),
                                   np.arange(16).reshape(2, 2, 2, 2))
 
 
-# Test Pydap structures.
+# Test pydap structures.
 def test_StructureType_init():
     """Test attributes used for dict-like behavior."""
     var = StructureType("var")
     assert (var._visible_keys == [])
     assert (var._dict == {})
 
 
 def test_StructureType_instance():
     """Test that it is a Mapping and DapType."""
     var = StructureType("var")
-    from collections import Mapping
+    try:
+       from collections.abc import Mapping
+    except ImportError:
+       from collections import Mapping
     assert isinstance(var, Mapping)
     assert isinstance(var, DapType)
 
 
 def test_StructureType_repr():
     """Test ``__repr__`` method."""
     var = StructureType("var")
@@ -244,16 +247,18 @@
     assert (list(var.keys()) == ['bar', 'foo%2Ebar'])
 
 
 def test_StructureType_getitem():
     """Test item retrieval."""
     var = StructureType("var")
     child = BaseType("child")
+    child.data = np.array([[[0, 1]]])
     var["child"] = child
     assert var["child"] is child
+    assert var["child.child"] is child
     with pytest.raises(KeyError):
         var["unloved child"]
     with pytest.raises(KeyError):
         var[:]
 
     assert var["parent.child"] is child
     assert var["grandparent.parent.child"] is child
@@ -332,15 +337,15 @@
     assert original["two"].data is clone["two"].data
 
     # test attributes
     assert (original.id == clone.id)
     assert (original.name == clone.name)
 
 
-# Test a Pydap structure.
+# Test a pydap structure.
 def test_DatasetType_setitem():
     """Test item assignment."""
     dataset = DatasetType("dataset")
     dataset["one"] = BaseType("one")
     assert dataset["one"].id == "one"
 
 
@@ -462,15 +467,15 @@
 def test_SequenceType_copy(sequence_example):
     """Test the lightweight ``__copy__`` method."""
     clone = copy.copy(sequence_example)
     assert sequence_example is not clone
     assert (sequence_example.data == clone.data).all()
 
 
-# Test Pydap grids.
+# Test pydap grids.
 @pytest.fixture()
 def gridtype_example():
     """Create a simple grid."""
     example = GridType("example")
     example["a"] = BaseType("a", data=np.arange(30*50).reshape(30, 50))
     example["x"] = BaseType("x", data=np.arange(30))
     example["y"] = BaseType("y", data=np.arange(50))
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_responses_version.py` & `pydap-3.4.0/src/pydap/tests/test_responses_version.py`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/src/pydap/tests/test_responses_ascii.py` & `pydap-3.4.0/src/pydap/tests/test_responses_ascii.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
     def test_charset(self):
         """Test the charset."""
         self.assertEqual(self.res.charset, "ascii")
 
     def test_headers(self):
         """Test headers from the response."""
-        print(self.res.text)
         self.assertEqual(
             self.res.headers,
             ResponseHeaders([
                 ('XDODS-Server', 'pydap/' + __version__),
                 ('Content-description', 'dods_ascii'),
                 ('Content-type', 'text/plain; charset=ascii'),
                 ('Content-Length', '440')]))
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_cas_urs.py` & `pydap-3.4.0/src/pydap/tests/test_cas_urs.py`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/src/pydap/tests/test_parsers.py` & `pydap-3.4.0/src/pydap/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/src/pydap/tests/test_parsers_dds.py` & `pydap-3.4.0/src/pydap/tests/test_parsers_dds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Test DDS parsing functions."""
 
 import numpy as np
-from pydap.parsers.dds import build_dataset
+from pydap.parsers.dds import dds_to_dataset
 from pydap.model import (BaseType,
                          StructureType)
 import unittest
 
 
 DDS = """Dataset {
     Structure {
@@ -39,15 +39,15 @@
 
 class TestBuildDataset(unittest.TestCase):
 
     """Test DDS parser."""
 
     def setUp(self):
         """Parse the whole dataset."""
-        self.dataset = build_dataset(DDS)
+        self.dataset = dds_to_dataset(DDS)
 
     def test_structure(self):
         """Test the structure."""
         self.assertIsInstance(self.dataset.structure, StructureType)
 
     def test_byte(self):
         """Test byte parsing."""
```

### Comparing `Pydap-3.2.2/src/pydap/tests/rainfall_time_malaysia.cdp.das` & `pydap-3.4.0/src/pydap/tests/data/rainfall_time_malaysia.cdp.das`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/src/pydap/tests/test_parsers_das.py` & `pydap-3.4.0/src/pydap/tests/test_parsers_das.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Test DAS parsing functions."""
 
 import numpy as np
 from pydap.parsers.das import add_attributes, parse_das
-from pydap.parsers.dds import build_dataset
+from pydap.parsers.dds import dds_to_dataset
 from pydap.tests.test_parsers_dds import DDS
 import unittest
 
 DAS = """Attributes {
     structure {
         b {
             Int value 1;
@@ -22,28 +22,34 @@
     }
     SPEH {
         Int debug 1;
         Int TIME 0;
         Float32 COADSX 1e20;
         String COADSY "zero";
     }
+    floats {
+        Float64 a nan;
+        Float64 b -inf;
+        Float64 c inf;
+        Float64 d 17;
+    }
 }"""
 
 # It is important to add attributes that have the same
 # name as the dimensions of SPEH. This is an edge
 # case that can break the das parser.
 
 
 class TestParseDAS(unittest.TestCase):
 
     """Test DAS parser."""
 
     def setUp(self):
         """Load a dataset and apply DAS to it."""
-        self.dataset = build_dataset(DDS)
+        self.dataset = dds_to_dataset(DDS)
         attributes = parse_das(DAS)
         add_attributes(self.dataset, attributes)
 
     def test_basic(self):
         """Test a basic attribute."""
         self.assertEqual(self.dataset.structure.b.value, 1)
 
@@ -65,7 +71,14 @@
 
     def test_SPEH_attributes(self):
         """Test attributes not associated with any variables."""
         self.assertEqual(self.dataset.SPEH.debug, 1)
         self.assertEqual(self.dataset.SPEH.attributes['TIME'], 0)
         self.assertEqual(self.dataset.SPEH.attributes['COADSX'], 1e20)
         self.assertEqual(self.dataset.SPEH.attributes['COADSY'], "zero")
+
+    def test_float_attributes(self):
+        """Test various values of float attributes."""
+        self.assertTrue(np.isnan(self.dataset.floats["a"]))
+        self.assertEqual(self.dataset.floats["b"], float("-inf"))
+        self.assertEqual(self.dataset.floats["c"], float("inf"))
+        self.assertEqual(self.dataset.floats["d"], 17.)
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_server_devel.py` & `pydap-3.4.0/src/pydap/tests/test_server_devel.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,20 +9,19 @@
 
 import numpy as np
 import pytest
 import time
 
 from webob.exc import HTTPError
 from pydap.handlers.lib import BaseHandler
-from pydap.handlers.dap import SequenceProxy, BaseProxy
+from pydap.handlers.dap import SequenceProxy, BaseProxyDap2
 from pydap.model import DatasetType, BaseType, SequenceType
-from pydap.client import open_url, open_dods
+from pydap.client import open_url, open_dods_url
 from pydap.server.devel import LocalTestServer
 
-
 server = pytest.mark.server
 
 
 @pytest.fixture
 def sequence_type_data():
     """
     Simple sequence test data
@@ -44,69 +43,83 @@
 
 @server
 def test_open(sequence_type_data):
     """Test that LocalTestServer works properly"""
     TestDataset = DatasetType('Test')
     TestDataset['sequence'] = sequence_type_data
     with LocalTestServer(BaseHandler(TestDataset)) as server:
-        url = ("http://0.0.0.0:%s/" % server.port)
-        dataset = open_url(url)
+        dataset = open_url(server.url)
         seq = dataset['sequence']
         retrieved_data = [line for line in seq]
 
     np.testing.assert_array_equal(np.array(
                                     retrieved_data,
                                     dtype=sequence_type_data.data.dtype),
                                   np.array(
                                     sequence_type_data.data[:],
                                     dtype=sequence_type_data.data.dtype))
 
 
 @server
-def test_timeout(sequence_type_data):
-    """Test that timeout works properly"""
+def test_netcdf(sequence_type_data):
+    """
+    Test that LocalTestServer works properly and that it works well with
+    netcdf4-python.
+    """
     TestDataset = DatasetType('Test')
-    TestDataset['sequence'] = sequence_type_data
-    TestDataset['byte'] = BaseType('byte', 0)
-    application = BaseHandler(TestDataset)
-
-    # Explictly add latency on the devel server
-    # to guarantee that it timeouts
-    def wrap_mocker(func):
-        def mock_add_latency(*args, **kwargs):
-            time.sleep(1e-1)
-            return func(*args, **kwargs)
-        return mock_add_latency
-
-    application = wrap_mocker(application)
-    with LocalTestServer(application) as server:
-        url = ("http://0.0.0.0:%s/" % server.port)
-
-        # test open_url
-        assert open_url(url) == TestDataset
-        with pytest.raises(HTTPError) as e:
-            open_url(url, timeout=1e-5)
-        assert 'Timeout' in str(e)
-
-        # test open_dods
-        with pytest.raises(HTTPError):
-            open_dods(url + '.dods?sequence', timeout=1e-5)
-        assert 'Timeout' in str(e)
+    TestDataset['float'] = BaseType('float', np.array(1, dtype=np.float32))
 
-        # test sequenceproxy
-        dataset = open_url(url)
-        seq = dataset['sequence']
-        assert isinstance(seq.data, SequenceProxy)
-        # Change the timeout of the sequence proxy:
-        seq.data.timeout = 1e-5
-        with pytest.raises(HTTPError) as e:
-            next(seq.iterdata())
-        assert 'Timeout' in str(e)
-
-        # test baseproxy:
-        dat = dataset['byte']
-        assert isinstance(dat.data, BaseProxy)
-        # Change the timeout of the baseprox proxy:
-        dat.data.timeout = 1e-5
-        with pytest.raises(HTTPError) as e:
-            dat[:]
-        assert 'Timeout' in str(e)
+    with TestDataset.to_netcdf() as ds:
+        assert 'float' in ds.variables
+        assert ds['float'].dtype == np.float32
+        assert ds['float'][:] == np.array(1, dtype=np.float32)
+
+
+# @server
+# def test_timeout(sequence_type_data):
+#     """Test that timeout works properly"""
+#     TestDataset = DatasetType('Test')
+#     TestDataset['sequence'] = sequence_type_data
+#     TestDataset['byte'] = BaseType('byte', 0)
+#     application = BaseHandler(TestDataset)
+
+#     # Explictly add latency on the devel server
+#     # to guarantee that it timeouts
+#     def wrap_mocker(func):
+#         def mock_add_latency(*args, **kwargs):
+#             time.sleep(1e-1)
+#             return func(*args, **kwargs)
+#         return mock_add_latency
+
+#     application = wrap_mocker(application)
+#     with LocalTestServer(application) as server:
+#         url = ("http://0.0.0.0:%s/" % server.port)
+
+#         # test open_url
+#         assert open_url(url) == TestDataset
+#         with pytest.raises(HTTPError) as e:
+#             open_url(url, timeout=1e-5)
+#         assert 'Timeout' in str(e)
+
+#         # test open_dods
+#         with pytest.raises(HTTPError):
+#             open_dods(url + '.dods?sequence', timeout=1e-5)
+#         assert 'Timeout' in str(e)
+
+#         # test sequenceproxy
+#         dataset = open_url(url)
+#         seq = dataset['sequence']
+#         assert isinstance(seq.data, SequenceProxy)
+#         # Change the timeout of the sequence proxy:
+#         seq.data.timeout = 1e-5
+#         with pytest.raises(HTTPError) as e:
+#             next(seq.iterdata())
+#         assert 'Timeout' in str(e)
+
+#         # test baseproxy:
+#         dat = dataset['byte']
+#         assert isinstance(dat.data, BaseProxy)
+#         # Change the timeout of the baseprox proxy:
+#         dat.data.timeout = 1e-5
+#         with pytest.raises(HTTPError) as e:
+#             dat[:]
+#         assert 'Timeout' in str(e)
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_wsgi_app.py` & `pydap-3.4.0/src/pydap/tests/test_wsgi_app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-"""Tests for the Pydap server."""
+"""Tests for the pydap server."""
 
 import os
 import tempfile
 import shutil
+from xml.etree import ElementTree as etree
 
 from webtest import AppError
 from webtest import TestApp as App
 from webob import Response
 from webob.dec import wsgify
 
 from pydap.wsgi.app import init, DapServer, StaticMiddleware
 from pydap.exceptions import ExtensionNotSupportedError
 
 import unittest
 
 
 class TestDapServer(unittest.TestCase):
 
-    """Tests for the Pydap server."""
+    """Tests for the pydap server."""
 
     def setUp(self):
         """Create an installation."""
         self.install = tempfile.mkdtemp(suffix="pydap")
 
         # create directory for data with two files
         data = os.path.join(self.install, "data")
@@ -66,14 +67,22 @@
         self.assertEqual(res.text, "Success!")
 
     def test_invalid_dap_request(self):
         """Test invalid DAP requests."""
         with self.assertRaises(ExtensionNotSupportedError):
             self.app.get("/README.txt.dds")
 
+    def test_thredds_catalog_request(self):
+        """Test that THREDDS Catalog requests work."""
+        res = self.app.get("/catalog.xml")
+        self.assertEqual(res.status, "200 OK")
+        self.assertTrue(res.text.startswith('<?xml'))
+        xml = etree.fromstring(res.text)
+        self.assertEqual(xml.tag, '{http://www.unidata.ucar.edu/namespaces/thredds/InvCatalog/v1.0}catalog')  # noqa
+
     def test_not_found(self):
         """Test 404 responses."""
         with self.assertRaises(AppError):
             self.app.get("/README.html")
 
     def test_asset(self):
         """Test that we can load a static asset."""
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_responses_html.py` & `pydap-3.4.0/src/pydap/tests/test_responses_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Test the HTML response from Pydap."""
+"""Test the HTML response from pydap."""
 
 from webtest import TestApp as App
 from webob import Request
 from webob.headers import ResponseHeaders
 from bs4 import BeautifulSoup
 from jinja2 import Environment, DictLoader
 
@@ -40,15 +40,15 @@
         """Test the response headers."""
         res = self.app.get('/.html')
         self.assertEqual(
             res.headers, ResponseHeaders([
                 ('XDODS-Server', 'pydap/' + __version__),
                 ('Content-description', 'dods_form'),
                 ('Content-type', 'text/html; charset=utf-8'),
-                ('Content-Length', '5215')]))
+                ('Content-Length', '5864')]))
 
     def test_body(self):
         """Test the HTML response.
 
         We use BeautifulSoup to parse the response, and check for some
         elements that should be there.
 
@@ -118,15 +118,15 @@
 
 
 class TestHTMLTemplate(unittest.TestCase):
 
     """Test that global environment is used if available.
 
     The HTML response has its own environment and loader, for when used in
-    standalone mode. If used with a Pydap server that defines its own
+    standalone mode. If used with a pydap server that defines its own
     environment, the HTML response will reuse the global environment after
     injecting its loader as a backup. This allows the HTML response to work in
     case the global environment does not have the HTML templates.
 
     """
 
     def test_environ_loader_with_template(self):
```

### Comparing `Pydap-3.2.2/src/pydap/tests/test_net.py` & `pydap-3.4.0/src/pydap/tests/test_net.py`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/src/pydap/tests/test_wsgi_functions.py` & `pydap-3.4.0/src/pydap/tests/test_wsgi_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Test the server-side functions that come with Pydap."""
+"""Test the server-side functions that come with pydap."""
 
 import copy
 
 from webtest import TestApp as App
 
 from pydap.handlers.lib import BaseHandler
 from pydap.tests.datasets import SimpleSequence, SimpleGrid
```

### Comparing `Pydap-3.2.2/docs/license.rst` & `pydap-3.4.0/docs/license.rst`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/docs/client.rst` & `pydap-3.4.0/docs/client.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Using the client
 ================
 
-Pydap can be used as a client to inspect and retrieve data from any of the `hundreds of scientific datasets <http://www.opendap.org/data/datasets.cgi?xmlfilename=datasets.xml&exfunction=none>`_ available on the internet on `OPeNDAP <http://opendap.org/>`_ servers. This way, it's possible to instrospect and manipulate a dataset as if it were stored locally, with data being downloaded on-the-fly as necessary.
+pydap can be used as a client to inspect and retrieve data from any of the `hundreds of scientific datasets <http://www.opendap.org/data/datasets.cgi?xmlfilename=datasets.xml&exfunction=none>`_ available on the internet on `OPeNDAP <http://opendap.org/>`_ servers. This way, it's possible to instrospect and manipulate a dataset as if it were stored locally, with data being downloaded on-the-fly as necessary.
 
 Accessing gridded data
 ----------------------
 
 Let's start accessing gridded data, i.e., data that is stored as a regular multidimensional array. Here's a simple example where we access the `COADS <http://www.ncdc.noaa.gov/oa/climate/coads/>`_ climatology from the official OPeNDAP server:
 
 .. doctest::
@@ -29,15 +29,15 @@
     >>> sst = dataset['SST']  # or dataset.SST
     >>> type(sst)
     <class 'pydap.model.GridType'>
 
 Note that the variable is of type ``GridType``, a multidimensional array with specific axes defining each of its dimensions:
 
 .. doctest::
-    
+
     >>> sst.dimensions
     ('TIME', 'COADSY', 'COADSX')
     >>> sst.maps
     OrderedDict([('TIME', <BaseType with data BaseProxy('http://test.opendap.org/dap/data/nc/coads_climatology.nc', 'SST.TIME', dtype('>f8'), (12,), (slice(None, None, None),))>), ('COADSY', <BaseType with data BaseProxy('http://test.opendap.org/dap/data/nc/coads_climatology.nc', 'SST.COADSY', dtype('>f8'), (90,), (slice(None, None, None),))>), ('COADSX', <BaseType with data BaseProxy('http://test.opendap.org/dap/data/nc/coads_climatology.nc', 'SST.COADSX', dtype('>f8'), (180,), (slice(None, None, None),))>)])
 
 Each map is also, in turn, a variable that can be accessed using the same syntax used for Structures:
 
@@ -113,15 +113,15 @@
     >>> print(sst.array[0,10:14,10:14].data)
     [[[ -1.26285708e+00  -9.99999979e+33  -9.99999979e+33  -9.99999979e+33]
       [ -7.69166648e-01  -7.79999971e-01  -6.75454497e-01  -5.95714271e-01]
       [  1.28333330e-01  -5.00000156e-02  -6.36363626e-02  -1.41666666e-01]
       [  6.38000011e-01   8.95384610e-01   7.21666634e-01   8.10000002e-01]]]
 
 Older Servers
-^^^^^^^^^^^^^
+~~~~~~~~~~~~~
 Some servers using a very old OPeNDAP application might run of of memory when attempting to retrieve both the data and
 the coordinate axes of a variable. The work around is to simply disable the retrieval of coordinate axes by using the
 ``output_grid`` option to open url:
 
 .. doctest::
 
     >>> from pydap.client import open_url
@@ -294,15 +294,14 @@
     ...     print(value[:10])
     [5.0, 10.0, 15.0, 20.0, 25.0, 30.0, 35.0, 40.0, 45.0, 50.0]
     [5.0, 10.0, 15.0, 20.0, 25.0, 30.0, 35.0, 40.0, 45.0, 50.0]
     [5.0, 10.0, 15.0, 20.0, 25.0, 30.0, 35.0, 40.0, 45.0, 50.0]
     [5.0, 10.0, 15.0, 20.0, 25.0, 30.0, 35.0, 40.0, 45.0, 50.0]
     [5.0999999, 9.1000004, 19.4, 29.700001, 39.599998, 49.599998, 59.700001, 69.5, 79.5, 89.699997]
 
-Pydap 3.0 has been rewritten to make it easier to work with Dapper datasets like this one, and it should be intuitive [1]_ to work with these variables. 
 
 Authentication
 --------------
 
 Basic & Digest
 ~~~~~~~~~~~~~~
 
@@ -312,59 +311,59 @@
 
     >>> from pydap.client import open_url
     >>> dataset = open_url('http://username:password@server.example.com/path/to/dataset')
 
 CAS
 ~~~
 
-The `Central Authentication Service <http://en.wikipedia.org/wiki/Central_Authentication_Service>`_ (CAS) is a single sign-on protocol for the web, usually involving a web browser and cookies. Nevertheless it's possible to use Pydap with an OPeNDAP server behind a CAS. The function ``install_cas_client`` below replaces Pydap's default HTTP function with a new version able to submit authentication data to an HTML form and store credentials in cookies. (In this particular case, the server uses Javascript to redirect the browser to a new location, so the client has to parse the location from the Javascript code; other CAS would require a tweaked function.)
+The `Central Authentication Service <http://en.wikipedia.org/wiki/Central_Authentication_Service>`_ (CAS) is a single sign-on protocol for the web, usually involving a web browser and cookies. Nevertheless it's possible to use pydap with an OPeNDAP server behind a CAS. The function ``install_cas_client`` below replaces pydap's default HTTP function with a new version able to submit authentication data to an HTML form and store credentials in cookies. (In this particular case, the server uses Javascript to redirect the browser to a new location, so the client has to parse the location from the Javascript code; other CAS would require a tweaked function.)
 
 To use it, just attach a web browsing ``session`` with authentication cookies:
 
 .. code-block:: python
 
-    >>> from pydap.client import open_url  
-    >>> from pydap.cas.get_cookies import setup_session 
+    >>> from pydap.client import open_url
+    >>> from pydap.cas.get_cookies import setup_session
     >>> session = setup_session(authentication_url, username, password)
     >>> dataset = open_url('http://server.example.com/path/to/dataset', session=session)
 
 This method could work but each CAS is slightly different and might require a specifically designed
 ``setup_session`` instance. Two CAS are however explicitly supported by ``pydap``:
 
 URS NASA EARTHDATA
 ^^^^^^^^^^^^^^^^^^
 Authentication is done through a ``username`` and a ``password``:
 
 .. code-block:: python
 
-    >>> from pydap.client import open_url  
-    >>> from pydap.cas.urs import setup_session 
+    >>> from pydap.client import open_url
+    >>> from pydap.cas.urs import setup_session
     >>> dataset_url = 'http://server.example.com/path/to/dataset'
     >>> session = setup_session(username, password, check_url=dataset_url)
     >>> dataset = open_url(dataset_url, session=session)
 
 Earth System Grid Federation (ESGF)
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 Authentication is done through an ``openid`` and a ``password``:
 
 .. code-block:: python
 
-    >>> from pydap.client import open_url  
-    >>> from pydap.cas.esgf import setup_session 
+    >>> from pydap.client import open_url
+    >>> from pydap.cas.esgf import setup_session
     >>> dataset_url = 'http://server.example.com/path/to/dataset'
     >>> session = setup_session(openid, password, check_url=dataset_url)
     >>> dataset = open_url(dataset_url, session=session)
 
 If your ``openid`` contains contains the
 string ``ceda.ac.uk`` authentication requires an additional ``username`` argument:
 
 .. code-block:: python
 
-    >>> from pydap.client import open_url  
-    >>> from pydap.cas.esgf import setup_session 
+    >>> from pydap.client import open_url
+    >>> from pydap.cas.esgf import setup_session
     >>> session = setup_session(openid, password, check_url=dataset_url, username=username)
     >>> dataset = open_url(dataset_url, session=session)
 
 Advanced features
 -----------------
 
 Calling server-side functions
@@ -411,14 +410,18 @@
 ~~~~~~~~~~~~~~~~~~
 
 The client module has a special function called ``open_dods``, used to access raw data from a DODS response:
 
 .. doctest::
 
     >>> from pydap.client import open_dods
+        >>> dataset = open_dods_url(
+        ...     'http://test.opendap.org/dap/data/nc/coads_climatology.nc.dods?SST[0:3:11][0:1:89][0:1:179]')
+
+    This function allows you to access raw data from any URL, including appending expressions to
     >>> dataset = open_dods(
     ...     'http://test.opendap.org/dap/data/nc/coads_climatology.nc.dods?SST[0:3:11][0:1:89][0:1:179]')
 
 This function allows you to access raw data from any URL, including appending expressions to `F-TDS <http://ferret.pmel.noaa.gov/LAS/documentation/the-ferret-thredds-data-server-f-tds/>`_ and `GDS <http://www.iges.org/grads/gds/>`_ servers or calling server-side functions directly. By default this method downloads the data directly, and skips metadata from the DAS response; if you want to investigate and introspect datasets you should set the ``get_metadata`` parameter to true:
 
 .. doctest::
 
@@ -443,21 +446,21 @@
 ~~~~~~~
 
 To specify a timeout for the client, just set the desired number of seconds using the ``timeout`` option to ``open_url(...)`` or ``open_dods(...)``.
 For example, the following commands would timeout after 30 seconds without receiving a response from the server:
 
 .. code-block:: python
 
-    >>> dataset = open_url('http://test.opendap.org/dap/data/nc/coads_climatology.nc, timeout=30)
-    >>> dataset = open_dods('http://test.opendap.org/dap/data/nc/coads_climatology.nc.dods, timeout=30)
+    >>> dataset = open_url('http://test.opendap.org/dap/data/nc/coads_climatology.nc', timeout=30)
+    >>> dataset = open_dods('http://test.opendap.org/dap/data/nc/coads_climatology.nc.dods', timeout=30)
 
 Configuring a proxy
 ~~~~~~~~~~~~~~~~~~~
 
-It's possible to configure Pydap to access the network through a proxy server. Here's an example for an HTTP proxy running on ``localhost`` listening on port 8000:
+It's possible to configure pydap to access the network through a proxy server. Here's an example for an HTTP proxy running on ``localhost`` listening on port 8000:
 
 .. code-block:: python
 
     >>> import httplib2
     >>> from pydap.util import socks
     >>> import pydap.lib
     >>> pydap.lib.PROXY = httplib2.ProxyInfo(
@@ -483,15 +486,12 @@
             log = logging.getLogger('pydap')
             log.INFO('Opening %s' % url)
 
             f = urllib2.urlopen(url.rstrip('?&'))
             headers = dict(f.info().items())
             body = f.read()
             return headers, body
-                                            
+
         from pydap.util import http
         http.request = new_request
 
 The function ``install_urllib2_client`` should then be called before doing any requests.
-
-.. [1] But please check `this quote <http://www.greenend.org.uk/rjk/2002/08/nipple.html>`_.
-
```

### Comparing `Pydap-3.2.2/docs/server.rst` & `pydap-3.4.0/docs/server.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Running a server
 ================
 
-Pydap comes with a lightweight and scalable OPeNDAP server, implemented as a `WSGI <http://wsgi.org/>`_ application. Being a WSGI `application <http://wsgi.org/wsgi/Applications>`_, Pydap can run on a variety of `servers <http://wsgi.org/wsgi/Servers>`_, and frameworks including Apache, `Nginx <https://www.nginx.com/>`_, IIS, `uWSGI <https://uwsgi-docs.readthedocs.io/en/latest/>`_, `Flask <http://flask.pocoo.org/>`_ or as a standalone Python process. It can also be seamless combined with different `middleware <http://wsgi.org/wsgi/Middleware_and_Utilities>`_ for authentication/authorization, GZip compression, and much more.
+pydap comes with a lightweight and scalable OPeNDAP server, implemented as a `WSGI <http://wsgi.org/>`_ application. Being a WSGI `application <http://wsgi.org/wsgi/Applications>`_, pydap can run on a variety of `servers <http://wsgi.org/wsgi/Servers>`_, and frameworks including Apache, `Nginx <https://www.nginx.com/>`_, IIS, `uWSGI <https://uwsgi-docs.readthedocs.io/en/latest/>`_, `Flask <http://flask.pocoo.org/>`_ or as a standalone Python process. It can also be seamless combined with different `middleware <http://wsgi.org/wsgi/Middleware_and_Utilities>`_ for authentication/authorization, GZip compression, and much more.
 
-There is no one right way to run Pydap server; your application requirements and software stack will inform your deployment decisions. In this chapter we provide a few examples to try and get you on the right track.
+There is no one right way to run pydap server; your application requirements and software stack will inform your deployment decisions. In this chapter we provide a few examples to try and get you on the right track.
 
-In order to distribute your data first you need to install a proper `handler <handlers.html>`_, that will convert the data format to the Pydap data model. 
+In order to distribute your data first you need to install a proper `handler <handlers.html>`_, that will convert the data format to the pydap data model. 
 
 Running standalone
 ------------------
 
-If you just want to quickly test the Pydap server, you can run it as a standalone Python application using the server that comes with `Python Paste <http://pythonpaste.org/>`_ and `gunicorn <http://gunicorn.org/>`_. To run the server, first make sure that you have installed Pydap with the server extras dependencies:
+If you just want to quickly test the pydap server, you can run it as a standalone Python application using the server that comes with `Python Paste <http://pythonpaste.org/>`_ and `gunicorn <http://gunicorn.org/>`_. To run the server, first make sure that you have installed pydap with the server extras dependencies:
 
 .. code-block:: bash
 
-    $ pip install Pydap[server]
+    $ pip install pydap[server]
 
 and then just run the ``pydap`` script that pip installs into your bin directory:
 
 .. code-block:: bash
 
     $ pydap --data /path/to/my/data/files --port 8080
 
@@ -31,15 +31,15 @@
 The HTML form template is fairly complex, since it contain some application logic and some Javascript code, so be careful to not break anything.
 
 .. _wsgi-application-section:
 
 WSGI Application
 ----------------
 
-Pydap follows the `WSGI specification <https://www.fullstackpython.com/wsgi-servers.html>`_, and most web servers gateways simply require a WSGI callable and a small amount of boiler plate code. Pydap provides the ``DapServer`` class which is a WSGI callable located in the ``pydap.wsgi.app`` module. A simple WSGI application script file would be something like this:
+pydap follows the `WSGI specification <https://www.fullstackpython.com/wsgi-servers.html>`_, and most web servers gateways simply require a WSGI callable and a small amount of boiler plate code. pydap provides the ``DapServer`` class which is a WSGI callable located in the ``pydap.wsgi.app`` module. A simple WSGI application script file would be something like this:
 
 .. code-block:: python
 
     from pydap.wsgi.app import DapServer
     application = DapServer('/path/to/my/data/files')
 
 
@@ -57,33 +57,33 @@
     app = Flask(__name__)
     app.wsgi_app = application
     app.run('0.0.0.0', 8000)
 
 Apache
 ------
 
-For a robust deployment you can run Pydap with Apache, using `mod_wsgi <http://modwsgi.org/>`_. After `installing mod_wsgi <http://code.google.com/p/modwsgi/wiki/InstallationInstructions>`_, create a sandbox in a directory *outside* your DocumentRoot, say ``/var/www/pydap/``, using `a virtual environment <https://docs.python.org/3/library/venv.html>`_:
+For a robust deployment you can run pydap with Apache, using `mod_wsgi <http://modwsgi.org/>`_. After `installing mod_wsgi <http://code.google.com/p/modwsgi/wiki/InstallationInstructions>`_, create a sandbox in a directory *outside* your DocumentRoot, say ``/var/www/pydap/``, using `a virtual environment <https://docs.python.org/3/library/venv.html>`_:
 
 .. code-block:: bash
 
     $ mkdir /var/www/pydap
     $ python3 -m venv /var/www/pydap/env
 
 If you want the sandbox to use your system installed packages (like Numpy, e.g.) you can use the ``--system-site-packages`` flag:
 
 .. code-block:: bash
 
     $ python3 -m venv --system-site-packages /var/www/pydap/env
 
-Now let's activate the sandbox and install Pydap -- this way the module and its dependencies can be isolated from the system libraries:
+Now let's activate the sandbox and install pydap -- this way the module and its dependencies can be isolated from the system libraries:
 
 .. code-block:: bash
 
     $ source /var/www/pydap/env/bin/activate.sh
-    (env)$ pip install Pydap
+    (env)$ pip install pydap
 
 Create a `WSGI script file <http://modwsgi.readthedocs.io/en/develop/user-guides/quick-configuration-guide.html#mounting-the-wsgi-application>`_ somewhere convenient (e.g. /var/www/pydap/server/apache/pydap.wsgi) that reads something like this:
 
 .. code-block:: python
 
     import site
     # force mod_wsgi to use the Python modules from the sandbox
@@ -131,37 +131,37 @@
         # alert, emerg.
         LogLevel warn
 
         CustomLog /var/log/apache2/test.pydap.org.access.log combined
         ServerSignature On
     </VirtualHost>
 
-You can find more information on the `mod_wsgi configuration guide <http://code.google.com/p/modwsgi/wiki/QuickConfigurationGuide>`_. Just remember that Pydap is a WSGI application like any other else, so any information on WSGI applications applies to it as well.
+You can find more information on the `mod_wsgi configuration guide <http://code.google.com/p/modwsgi/wiki/QuickConfigurationGuide>`_. Just remember that pydap is a WSGI application like any other else, so any information on WSGI applications applies to it as well.
 
 
 uWSGI
 -----
 
-`uWSGI <http://projects.unbit.it/uwsgi/>`_ is a "fast, self-healing and developer/sysadmin-friendly application container server coded in pure C" that can run Pydap. This is the recommended way to run Pydap if you don't have to integrate it with other web applications. Simply install uWSGI, follow the instructions in the last section in order to create a virtualenv and Pydap installation:
+`uWSGI <http://projects.unbit.it/uwsgi/>`_ is a "fast, self-healing and developer/sysadmin-friendly application container server coded in pure C" that can run pydap. This is the recommended way to run pydap if you don't have to integrate it with other web applications. Simply install uWSGI, follow the instructions in the last section in order to create a virtualenv and pydap installation:
 
 .. code-block:: bash
 
     $ mkdir /var/www/pydap
     $ python virtualenv.py /var/www/pydap/env
     $ source /var/www/pydap/env/bin/activate.sh
-    (env)$ pip install Pydap uWSGI
+    (env)$ pip install pydap uWSGI
     (env)$ cd /var/www/pydap
 
 Create a WSGI application file myapp.wsgi :ref:`as above <wsgi-application-section>`
 
 Now create a file in ``/etc/init/pydap.conf`` with the content:
 
 .. code-block:: bash
 
-    description "uWSGI server for Pydap"
+    description "uWSGI server for pydap"
 
     start on runlevel [2345]
     stop on runlevel [!2345]
 
     respawn
 
     exec /var/www/pydap/env/bin/uwsgi \
@@ -176,8 +176,8 @@
 
     $ sudo initctl reload-configuration
 
 
 Docker
 ------
 
-Users have `reported success <https://github.com/pydap/pydap/issues/46>`_ deploying Pydap with a docker image built with nginx + uWSGI + Flask (based on https://hub.docker.com/r/tiangolo/uwsgi-nginx-flask/. A full configuration is somewhat beyond the scope of this documentation (since it will depend on your requirements and your software stack), but it is certainly possible.
+Users have `reported success <https://github.com/pydap/pydap/issues/46>`_ deploying pydap with a docker image built with nginx + uWSGI + Flask (based on https://hub.docker.com/r/tiangolo/uwsgi-nginx-flask/. A full configuration is somewhat beyond the scope of this documentation (since it will depend on your requirements and your software stack), but it is certainly possible.
```

### Comparing `Pydap-3.2.2/docs/developer_handlers.rst` & `pydap-3.4.0/docs/developer_handlers.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Handlers
 --------
 
-Now that we saw the Pydap data model we can understand handlers: handlers are simply classes that convert data into the Pydap data model. The NetCDF handler, for example, reads a NetCDF file and builds a ``DatasetType`` object. The SQL handler reads a file describing the variables and maps them to a given table on a relational database. Pydap uses `entry points <http://peak.telecommunity.com/DevCenter/setuptools#dynamic-discovery-of-services-and-plugins>`_ in order to find handlers that are installed in the system. This means that handlers can be developed and installed separately from Pydap. Handlers are mapped to files by a regular expression that usually matches the extension of the file.
+Now that we saw the pydap data model we can understand handlers: handlers are simply classes that convert data into the pydap data model. The NetCDF handler, for example, reads a NetCDF file and builds a ``DatasetType`` object. The SQL handler reads a file describing the variables and maps them to a given table on a relational database. pydap uses `entry points <http://peak.telecommunity.com/DevCenter/setuptools#dynamic-discovery-of-services-and-plugins>`_ in order to find handlers that are installed in the system. This means that handlers can be developed and installed separately from pydap. Handlers are mapped to files by a regular expression that usually matches the extension of the file.
 
 Here is the minimal configuration for a handler that serves ``.npz`` files from Numpy:
 
 .. code-block:: python
 
     import os
     import re
@@ -43,15 +43,15 @@
 So let's go over the code. Our handler has a single class called ``Handler`` that should be configured as an entry point in the ``setup.py`` file for the handler:
 
 .. code-block:: ini
 
     [pydap.handler]
     npz = path.to.my.handler:Handler
 
-Here the name of our handler ("npz") can be anything, as long as it points to the correct class. In order for Pydap to be able to find the handler, it must be installed in the system with either a ``python setup.py install`` or, even better, ``python setup.py develop``. 
+Here the name of our handler ("npz") can be anything, as long as it points to the correct class. In order for pydap to be able to find the handler, it must be installed in the system with either a ``python setup.py install`` or, even better, ``python setup.py develop``. 
 
 The class-level attribute ``extensions`` defines a regular expression that matches the files supported by the handler. In this case, the handler will match all files ending with the ``.npz`` extension.
 
 When the handler is instantiated the complete filepath to the data file is passed in ``__init__``. With this information, our handler extracts the filename of the data file and opens it using the ``load()`` function from Numpy. The handler will be initialized for every request, and immediately its ``parse_constraints`` method is called.
 
 The ``parse_constraints`` method is responsible for building a dataset object based on information for the request available on ``environ``. In this simple handler we simply built a ``DatasetType`` object with the entirety of our dataset, i.e., we added *all data from all variables* that were available on the ``.npz`` file. Some requests will ask for only a few variables, and only a subset of their data. The easy way parsing the request is simply passing the complete dataset together with the ``QUERY_STRING`` to the ``contrain()`` function:
```

### Comparing `Pydap-3.2.2/docs/Makefile` & `pydap-3.4.0/docs/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -56,17 +56,17 @@
 	      ".hhp project file in _build/htmlhelp."
 
 qthelp:
 	$(SPHINXBUILD) -b qthelp $(ALLSPHINXOPTS) _build/qthelp
 	@echo
 	@echo "Build finished; now you can run "qcollectiongenerator" with the" \
 	      ".qhcp project file in _build/qthelp, like this:"
-	@echo "# qcollectiongenerator _build/qthelp/Pydap.qhcp"
+	@echo "# qcollectiongenerator _build/qthelp/pydap.qhcp"
 	@echo "To view the help file:"
-	@echo "# assistant -collectionFile _build/qthelp/Pydap.qhc"
+	@echo "# assistant -collectionFile _build/qthelp/pydap.qhc"
 
 latex:
 	$(SPHINXBUILD) -b latex $(ALLSPHINXOPTS) _build/latex
 	@echo
 	@echo "Build finished; the LaTeX files are in _build/latex."
 	@echo "Run \`make all-pdf' or \`make all-ps' in that directory to" \
 	      "run these through (pdf)latex."
```

### Comparing `Pydap-3.2.2/docs/developer.rst` & `pydap-3.4.0/docs/developer.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Developer documentation
 =======================
 
-This documentation is intended for other developers that would like to contribute with the development of Pydap, 
+This documentation is intended for other developers that would like to contribute with the development of pydap, 
 or extend it in new ways. It assumes that you have a basic knowledge of Python and HTTP, and 
 understands how data is stored in different formats. 
 It also assumes some familiarity with the `Data Access Protocol <http://opendap.org/>`_, 
 though a lot of its inner workings will be explained in detail here.
 
 .. include:: developer_data_model.rst
```

### Comparing `Pydap-3.2.2/docs/handlers.rst` & `pydap-3.4.0/docs/handlers.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Handlers
 ========
 
-Handlers are special Python modules that convert between a given data format and the data model used by Pydap (defined in the ``pydap.model`` module). They are necessary in order to Pydap be able to actually serve a dataset. There are handlers for NetCDF, HDF 4 & 5, Matlab, relational databases, Grib 1 & 2, CSV, Seabird CTD files, and a few more. 
+Handlers are special Python modules that convert between a given data format and the data model used by pydap (defined in the ``pydap.model`` module). They are necessary in order to pydap be able to actually serve a dataset. There are handlers for NetCDF, HDF 4 & 5, Matlab, relational databases, Grib 1 & 2, CSV, Seabird CTD files, and a few more. 
 
 Installing data handlers
 ------------------------
 
 NetCDF
 ~~~~~~
 
 `NetCDF <http://www.unidata.ucar.edu/software/netcdf/>`_ is a format commonly used in oceanography, meteorology and climate science to store data in a machine-independent format. You can install the NetCDF handler using `pip <http://pypi.python.org/pypi/pip>`_:
 
 .. code-block:: bash
 
-    $ pip install Pydap[handlers.netcdf]
+    $ pip install pydap[handlers.netcdf]
 
 This will take care of the necessary dependencies. You don't even need to have to NetCDF libraries installed, since the handler will use a pure Python NetCDF library from `scipy.io.netcdf <https://docs.scipy.org/doc/scipy-0.16.1/reference/generated/scipy.io.netcdf.netcdf_file.html/>`_.
 
 The NetCDF handler uses a buffered reader that access the data in contiguous blocks from disk, avoiding reading everything into memory at once. You can configure the size of the buffer by specifying a key in the ``server.ini`` file:
 
 .. code-block:: ini
 
@@ -56,15 +56,15 @@
 
 .. code-block:: ini
 
     [dataset]
     match = /path/to/data*.nc
     axis = TIME  # existing axis
 
-The handler only works with NetCDF files for now, but in the future it should be changed to work with any other Pydap-supported data format. As all handlers, it can be installed using `pip <http://pypi.python.org/pypi/pip>`_:
+The handler only works with NetCDF files for now, but in the future it should be changed to work with any other pydap-supported data format. As all handlers, it can be installed using `pip <http://pypi.python.org/pypi/pip>`_:
 
 .. code-block:: bash
 
     $ pip install pydap.handlers.nca
 
 CDMS
 ~~~~
@@ -88,15 +88,15 @@
     # setting your password on the DSN
     database: 
         dsn: 'sqlite://simple.db'
         table: test
 
     dataset:
         NC_GLOBAL: 
-            history: Created by the Pydap SQL handler
+            history: Created by the pydap SQL handler
             dataType: Station
             Conventions: GrADS
 
         contact: roberto@dealmeida.net
         name: test_dataset
         owner: Roberto De Almeida
         version: 1.0
@@ -165,27 +165,27 @@
     $ pip install "pydap.handlers.sql[postgresql]"
     $ pip install "pydap.handlers.sql[mysql]"
     $ pip install "pydap.handlers.sql[mssql]"
 
 Proxy
 ~~~~~
 
-This is a simple handler intended to serve remote datasets locally. For example, suppose you want to serve `this dataset <http://test.opendap.org:8080/dods/dts/D1.html>`_ on your Pydap server. The URL of the dataset is::
+This is a simple handler intended to serve remote datasets locally. For example, suppose you want to serve `this dataset <http://test.opendap.org:8080/dods/dts/D1.html>`_ on your pydap server. The URL of the dataset is::
 
     http://test.opendap.org:8080/dods/dts/D1
 
 So we create an INI file called, say, ``D1.url``:
 
 .. code-block:: ini
 
     [dataset]
     url = http://test.opendap.org:8080/dods/dts/D1
     pass = dds, das, dods
 
-The file specifies that requests for the DDS, DAS and DODS responses should be passed directly to the server (so that the data is downloaded directly from the remote server). Other requests, like for the HTML form or a WMS image are built by Pydap; in this case Pydap acts as an Opendap client, connecting to the remote server and downloading data to fulfill the request.
+The file specifies that requests for the DDS, DAS and DODS responses should be passed directly to the server (so that the data is downloaded directly from the remote server). Other requests, like for the HTML form or a WMS image are built by pydap; in this case pydap acts as an Opendap client, connecting to the remote server and downloading data to fulfill the request.
 
 CSV
 ~~~
 
 This is a handler for files with comma separated values. The first column should contain the variable names, and subsequent lines the data. Metadata is not supported. The handler is used mostly as a reference for building handlers for sequential data. You can install it with:
 
 .. code-block:: bash
```

### Comparing `Pydap-3.2.2/docs/developer_data_model.rst` & `pydap-3.4.0/docs/developer_data_model.rst`

 * *Files 9% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 In order to transmit data from the server to a client, both must agree on a way to represent data:
 *is it an array of integers?*, *a multi-dimensional grid?*
 In order to do this, the specification defines a *data model* that, in theory, should be able to represent any existing dataset.
 
 Metadata
 ~~~~~~~~
 
-Pydap has a series of classes in the ``pydap.model`` module, representing the DAP data model.
+pydap has a series of classes in the ``pydap.model`` module, representing the DAP data model.
 The most fundamental data type is called ``BaseType``, and it represents a value or an array of values.
 Here an example of creating one of these objects:
 
-.. note:: Prior to Pydap 3.2, the name argument was optional for all date types. Since Pydap 3.2, it is mandatory.
+.. note:: Prior to pydap 3.2, the name argument was optional for all date types. Since pydap 3.2, it is mandatory.
 
 .. doctest::
 
     >>> from pydap.model import *
     >>> import numpy as np
     >>> a = BaseType(
     ...         name='a',
     ...         data=np.array([1]),
     ...         attributes={'long_name': 'variable a'})
 
-All Pydap types have five attributes in common. The first one is the ``name`` of the variable; in this case, our variable is called "a":
+All pydap types have five attributes in common. The first one is the ``name`` of the variable; in this case, our variable is called "a":
 
 .. doctest::
 
     >>> a.name
     'a'
 
 Note that there's a difference between the variable name (the local name ``a``) and its attribute ``name``; in this example they are equal, but we could reference our object using any other name:
@@ -58,15 +58,15 @@
     >>> c.name
     'long%20%26%20complicated'
     >>> c.id
     'long%20%26%20complicated'
 
 This is because the ``id`` is used to show the position of the variable in a given dataset, and in these
 examples the variables do not belong to any datasets. First let's store our variables in a container
-object called ``StructureType``. A ``StructureType`` is a special type of ordered dictionary that holds other Pydap types:
+object called ``StructureType``. A ``StructureType`` is a special type of ordered dictionary that holds other pydap types:
 
 .. doctest::
 
     >>> s = StructureType('s')
     >>> s['a'] = a
     >>> s['c'] = c
     Traceback (most recent call last):
@@ -133,24 +133,24 @@
 
 It's always better to use the correct syntax instead of the lazy one when writing code.
 Use the lazy syntax only when introspecting a dataset on the Python interpreter, to save a few keystrokes.
 
 The fourth attribute is called ``data``, and it holds a representation of the actual data.
 We'll take a detailed look of this attribute in the next subsection.
 
-.. note:: Prior to Pydap 3.2, all variables had also an attribute called ``_nesting_level``.
+.. note:: Prior to pydap 3.2, all variables had also an attribute called ``_nesting_level``.
           This attribute had value 1 if the variable was inside a ``SequenceType`` object,
           0 if it's outside, and >1 if it's inside a nested sequence.
-          Since Pydap 3.2, the ``_nesting_level`` has been deprecated and there is no
+          Since pydap 3.2, the ``_nesting_level`` has been deprecated and there is no
           intrinsic way of finding the where in a deep object a variable is located.
 
 Data
 ~~~~
 
-As we saw on the last subsection, all Pydap objects have a ``data`` attribute that holds a representation of the variable data.
+As we saw on the last subsection, all pydap objects have a ``data`` attribute that holds a representation of the variable data.
 This representation will vary depending on the variable type. 
 
 ``BaseType``
 ************
 
 For the simple ``BaseType`` objects the ``data`` attributes is usually a Numpy array, 
 though we can also use a Numpy scalar or Python number:
@@ -161,15 +161,15 @@
     >>> a.data
     array(1)
 
     >>> b = BaseType(name='b', data=np.arange(4))
     >>> b.data
     array([0, 1, 2, 3])
 
-Note that starting from Pydap 3.2 the datatype is inferred from the input data:
+Note that starting from pydap 3.2 the datatype is inferred from the input data:
 
 .. doctest::
 
     >>> a.dtype
     dtype('int64')
     >>> b.dtype
     dtype('int64')
@@ -192,16 +192,28 @@
 This is how the DAP client works -- instead of assigning an array with data directly to the attribute, 
 we assign a special object which behaves like an array and acts as a *proxy* to a remote dataset. 
 
 Here's an example:
 
 .. doctest::
 
-    >>> from pydap.handlers.dap import BaseProxy
-    >>> pseudo_array = BaseProxy(
+    >>> from pydap.handlers.dap import BaseProxyDap2
+        >>> pseudo_array = BaseProxyDap2(
+        ...         'http://test.opendap.org/dap/data/nc/coads_climatology.nc',
+        ...         'SST.SST',
+        ...         np.float64,
+        ...         (12, 90, 180))
+        >>> print(pseudo_array[0, 10:14, 10:14])  # download the corresponding data #doctest: +SKIP
+        [[[ -1.26285708e+00  -9.99999979e+33  -9.99999979e+33  -9.99999979e+33]
+          [ -7.69166648e-01  -7.79999971e-01  -6.75454497e-01  -5.95714271e-01]
+          [  1.28333330e-01  -5.00000156e-02  -6.36363626e-02  -1.41666666e-01]
+          [  6.38000011e-01   8.95384610e-01   7.21666634e-01   8.10000002e-01]]]
+
+    In the example above, the data is only downloaded in the last line, when the pseudo array is sliced. The object will construct the appropriate DAP URL, request the data, unpack it and return a Numpy array.
+    >>> pseudo_array = BaseProxyDap2(
     ...         'http://test.opendap.org/dap/data/nc/coads_climatology.nc',
     ...         'SST.SST',
     ...         np.float64,
     ...         (12, 90, 180))
     >>> print(pseudo_array[0, 10:14, 10:14])  # download the corresponding data #doctest: +SKIP
     [[[ -1.26285708e+00  -9.99999979e+33  -9.99999979e+33  -9.99999979e+33]
       [ -7.69166648e-01  -7.79999971e-01  -6.75454497e-01  -5.95714271e-01]
@@ -276,25 +288,25 @@
 
     >>> for record in s.iterdata():
     ...     print(record)
     (1, 10)
     (2, 20)
     (3, 30)
 
-Prior to Pydap 3.2.2, this approach was not possible and one had to iterate directly over ``SequenceType``: 
+Prior to pydap 3.2.2, this approach was not possible and one had to iterate directly over ``SequenceType``: 
 
 .. doctest::
 
     >>> for record in s:
     ...     print(record)
     (1, 10)
     (2, 20)
     (3, 30)
 
-This approach will be deprecated in Pydap 3.4.
+This approach will be deprecated in pydap 3.4.
 
 The ``SequenceType`` behaves pretty much like `record arrays <http://docs.scipy.org/doc/numpy/user/basics.rec.html>`_ from 
 Numpy, since we can reference them by column (``s['a']``) or by index:
 
 .. doctest::
 
     >>> s[1].data
@@ -302,26 +314,26 @@
     >>> s[ s.a < 3 ].data
     array([(1, 10), (2, 20)], 
           dtype=[('a', '<i4'), ('long%20%26%20complicated', '<i2')])
 
 Note that these objects are also ``SequenceType`` themselves. The basic rules when working with sequence data are: 
 
 1. When a ``SequenceType`` is sliced with a string the corresponding children is returned. For example: ``s['a']`` will return child ``a``;
-2. When a ``SequenceType`` is iterated over (using ``.iterdata()`` after Pydap 3.2.2) it will return a series of tuples, each one containing the data for a record;
+2. When a ``SequenceType`` is iterated over (using ``.iterdata()`` after pydap 3.2.2) it will return a series of tuples, each one containing the data for a record;
 3. When a ``SequenceType`` is sliced with an integer, a comparison or a ``slice()`` a new ``SequenceType`` will be returned;
 4. When a ``SequenceType`` is sliced with a tuple of strings a new ``SequenceType`` will be returned, containing only the children defined in the tuple in the new order.
    For example, ``s[('c', 'a')]`` will return a sequence ``s`` with the children ``c`` and ``a``, in that order.
 
 Note that except for rule 4 ``SequenceType`` mimics the behavior of Numpy record arrays.
 
 Now imagine that we want to add to a ``SequenceType`` data pulled from a relational database. 
 The easy way would be to fetch the data in the correct column order, and insert it into the sequence. 
 But what if we don't want to store the data in memory, and instead we would like to stream it directly from the database? 
 In this case we can create an object that behaves like a record array, similar to the proxy object that implements the array interface. 
-Pydap defines a "protocol" called ``IterData``, which is simply any object that:
+pydap defines a "protocol" called ``IterData``, which is simply any object that:
 
 1. Returns data when iterated over.
 2. Returns a new ``IterData`` when sliced such that:
 
    a) if the slice is a string the new ``IterData`` contains data only for that children;
    b) if the slice is a tuple of strings the object contains only those children, in that order;
    c) if the slice is an integer, a ``slice()`` or a comparison, the data is filter accordingly.
@@ -347,15 +359,15 @@
 
 .. doctest::
 
     >>> for record in s2:
     ...     print(record)
     (10, 20)
 
-This approach will not be deprecated in Pydap 3.4.
+This approach will not be deprecated in pydap 3.4.
 
 There are many implementations of classes derived from ``IterData``: ``pydap.handlers.dap.SequenceProxy`` is a proxy to 
 sequential data on Opendap servers, ``pydap.handlers.csv.CSVProxy`` wraps a CSV file, 
 and ``pydap.handlers.sql.SQLProxy`` works as a stream to a relational database.
 
 ``GridType``
 ************
```

### Comparing `Pydap-3.2.2/docs/_static/default.css` & `pydap-3.4.0/docs/_static/default.css`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/docs/_build/html/_sources/developer_templating.rst.txt` & `pydap-3.4.0/docs/developer_templating.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Templating
 ----------
 
-Pydap uses an `experimental backend-agnostic templating API <http://svn.pythonpaste.org/Paste/TemplateProposal/>`_ for rendering HTML and XML by responses. Since the API is neutral Pydap can use any templating engine, like `Mako <http://www.makotemplates.org/>`_ or `Genshi <http://genshi.edgewall.org/>`_, and templates can be loaded from disk, memory or a database. The server that comes with Pydap, for example, defines a ``renderer`` object that loads Genshi templates from a directory ``templatedir``:
+pydap uses an `experimental backend-agnostic templating API <http://svn.pythonpaste.org/Paste/TemplateProposal/>`_ for rendering HTML and XML by responses. Since the API is neutral pydap can use any templating engine, like `Mako <http://www.makotemplates.org/>`_ or `Genshi <http://genshi.edgewall.org/>`_, and templates can be loaded from disk, memory or a database. The server that comes with pydap, for example, defines a ``renderer`` object that loads Genshi templates from a directory ``templatedir``:
 
 .. code-block:: python
 
     from pydap.util.template import FileLoader, GenshiRenderer
 
     class FileServer(object):
         def __init__(self, templatedir, ...):
@@ -24,8 +24,8 @@
     def serialize(dataset):
         ...
         renderer = environ['pydap.renderer']
         template = renderer.loader('html.html')
         output = renderer.render(template, context, output_format='text/html')
         return [output]
 
-(This is acutally a simplification; if you look at the code you'll notice that there's also code to fallback to a default renderer if one is not found in the ``environ``.)
+(This is actually a simplification; if you look at the code you'll notice that there's also code to fallback to a default renderer if one is not found in the ``environ``.)
```

### Comparing `Pydap-3.2.2/docs/_build/html/_sources/index.rst.txt` & `pydap-3.4.0/docs/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 .. pydap documentation master file, created by sphinx-quickstart on Tue May  6 23:41:51 2008.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
-Pydap
+pydap
 =====
 
-Pydap is a pure `Python <http://python.org/>`_ library implementing the `Data Access Protocol <http://opendap.org/>`_, also known as **DODS** or **OPeNDAP**. You can use Pydap as a `client <client.html>`_ to access hundreds of scientific datasets in a transparent and efficient way through the internet; or as a server to easily `distribute <server.html>`_ your data from a `variety of formats <handlers.html>`_.
+pydap is a pure `Python <http://python.org/>`_ library implementing the `Data Access Protocol <http://opendap.org/>`_, also known as **DODS** or **OPeNDAP**. You can use pydap as a `client <client.html>`_ to access hundreds of scientific datasets in a transparent and efficient way through the internet; or as a server to easily `distribute <server.html>`_ your data from a `variety of formats <handlers.html>`_.
 
 Quickstart
 ----------
 
-You can install the latest version (|release|) using `pip <http://pypi.python.org/pypi/pip>`_. After `installing pip <http://www.pip-installer.org/en/latest/installing.html>`_ you can install Pydap with this command:
+You can install the latest version (|release|) using `pip <http://pypi.python.org/pypi/pip>`_. After `installing pip <http://www.pip-installer.org/en/latest/installing.html>`_ you can install pydap with this command:
 
 .. code-block:: bash
 
-    $ pip install Pydap
+    $ pip install pydap
 
-This will install Pydap together with all the required dependencies. You can now open any remotely served dataset, and Pydap will download the accessed data on-the-fly as needed:
+This will install pydap together with all the required dependencies. You can now open any remotely served dataset, and pydap will download the accessed data on-the-fly as needed:
 
 .. doctest:: 
 
     >>> from pydap.client import open_url
     >>> dataset = open_url('http://test.opendap.org/dap/data/nc/coads_climatology.nc')
     >>> var = dataset['SST']
     >>> var.shape
@@ -36,45 +36,44 @@
             [ -7.69166648e-01,  -7.79999971e-01,  -6.75454497e-01,
               -5.95714271e-01],
             [  1.28333330e-01,  -5.00000156e-02,  -6.36363626e-02,
               -1.41666666e-01],
             [  6.38000011e-01,   8.95384610e-01,   7.21666634e-01,
                8.10000002e-01]]], dtype=float32), array([ 366.]), array([-69., -67., -65., -63.]), array([ 41.,  43.,  45.,  47.])]
 
-For more information, please check the documentation on `using Pydap as a client <client.html>`_. Pydap also comes with a simple server, implemented as a `WSGI <http://wsgi.org/>`_ application. To use it, you first need to install Pydap with the server extras dependencies. If you want to serve `netCDF <http://www.unidata.ucar.edu/software/netcdf/>`_ files, install Pydap with the ``handlers.netcdf`` extra:
+For more information, please check the documentation on `using pydap as a client <client.html>`_. pydap also comes with a simple server, implemented as a `WSGI <http://wsgi.org/>`_ application. To use it, you first need to install pydap with the server extras dependencies. If you want to serve `netCDF <http://www.unidata.ucar.edu/software/netcdf/>`_ files, install pydap with the ``handlers.netcdf`` extra:
 
 .. code-block:: bash
 
-    $ pip install Pydap[server,handlers.netcdf]
+    $ pip install pydap[server,handlers.netcdf]
 
 More `handlers <handlers.html>`_ for different formats are available, if necessary. To run a simple standalone server just issue the command:
 
 .. code-block:: bash
 
     $ pydap --data ./myserver/data/ --port 8001
 
-This will start a standalone server running on http://localhost:8001/, serving netCDF files from ``./myserver/data/``, similar to the test server at http://test.pydap.org/. Since the server uses the `WSGI <http://wsgi.org/>`_ standard, it can easily be run behind Apache. The `server documentation <server.html>`_ has more information on how to better deploy Pydap.
+This will start a standalone server running on http://localhost:8001/, serving netCDF files from ``./myserver/data/``, similar to the test server at http://test.pydap.org/. Since the server uses the `WSGI <http://wsgi.org/>`_ standard, it can easily be run behind Apache. The `server documentation <server.html>`_ has more information on how to better deploy pydap.
 
 Help
 ----
 
-If you need any help with Pydap, please feel free to send an email to the `mailing list <http://groups.google.com/group/pydap/>`_.
+If you need any help with pydap, please feel free to send an email to the `mailing list <http://groups.google.com/group/pydap/>`_.
 
 Documentation
 -------------
 
 .. toctree::
    :maxdepth: 2
 
    client
    server
    handlers
    responses
    developer
-   Changelog
    license
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `Pydap-3.2.2/docs/_build/html/_sources/responses.rst.txt` & `pydap-3.4.0/docs/responses.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Responses
 =========
 
-Like `handlers <handlers.html>`_, responses are special Python modules that convert between the Pydap data model and an external representation. For instance, to access a given dataset an Opendap client request two diferent representations of the dataset: a *Dataset Attribute Structure* (DAS) response, describing the attributes of the dataset, and a *Dataset Descriptor Structure* (DDS), describing its structure (shape, type, hierarchy). These responses are returned by appending the extension ``.das`` and ``.dds`` to the dataset URL, respectively.
+Like `handlers <handlers.html>`_, responses are special Python modules that convert between the pydap data model and an external representation. For instance, to access a given dataset an Opendap client request two diferent representations of the dataset: a *Dataset Attribute Structure* (DAS) response, describing the attributes of the dataset, and a *Dataset Descriptor Structure* (DDS), describing its structure (shape, type, hierarchy). These responses are returned by appending the extension ``.das`` and ``.dds`` to the dataset URL, respectively.
 
-Other common responses include the ASCII (``.asc`` or ``.ascii``) response, which returns an ASCII representation of the data; and an HTML form for data request using the browser, at the ``.html`` extension. And perhaps the most important response is the ``.dods`` response, which actually carries the data in binary format, and is used when clients request data from the server. All these responses are standard and come with Pydap.
+Other common responses include the ASCII (``.asc`` or ``.ascii``) response, which returns an ASCII representation of the data; and an HTML form for data request using the browser, at the ``.html`` extension. And perhaps the most important response is the ``.dods`` response, which actually carries the data in binary format, and is used when clients request data from the server. All these responses are standard and come with pydap.
 
-There are other extension responses available for Pydap; these are not defined in the DAP specification, but improve the user experience by allowing data to be accessed in different formats.
+There are other extension responses available for pydap; these are not defined in the DAP specification, but improve the user experience by allowing data to be accessed in different formats.
 
 Installing additional responses
 -------------------------------
 
 Web Map Service
 ~~~~~~~~~~~~~~~
 
-This response enables Pydap to act like a `Web Map Service <http://en.wikipedia.org/wiki/Web_Map_Service>`_ 1.1.1 server, returning images (maps) of the available data. These maps can be visualized in any WMS client like Openlayers or Google Earth.
+This response enables pydap to act like a `Web Map Service <http://en.wikipedia.org/wiki/Web_Map_Service>`_ 1.1.1 server, returning images (maps) of the available data. These maps can be visualized in any WMS client like Openlayers or Google Earth.
 
 You can install the WMS response using `pip <http://pypi.python.org/pypi/pip>`_:
 
 .. code-block:: bash
 
     $ pip install pydap.responses.wms
 
-This will take care of the necessary dependencies, which include `Matplotlib <http://matplotlib.sf.net/>`_ and Pydap itself. Once the response is installed you can introspect the available layers at the URL::
+This will take care of the necessary dependencies, which include `Matplotlib <http://matplotlib.sf.net/>`_ and pydap itself. Once the response is installed you can introspect the available layers at the URL::
 
     http://server.example.com/dataset.wms?REQUEST=GetCapabilities
 
 The response will create valid layers from any `COARDS <http://ferret.wrc.noaa.gov/noaa_coop/coop_cdf_profile.html>`_ compliant datasets, ie, grids with properly defined latitude and longitude axes. If the data is not two-dimensional it will be averaged along each axis except for the last two, so the map represents a time and/or level average of the data. Keep in mind that Opendap constraint expressions apply before the map is generated, so it's possible to create a map of a specific level (or time) by constraining the variable on the URL::
 
     http://server.example.com/dataset.wms?var3d[0]&REQUEST=GetCapabilities
 
@@ -40,15 +40,15 @@
     x-wsgiorg.throw_errors = 0
     pydap.responses.wms.dpi = 80
     pydap.responses.wms.cmap = jet
 
 Google Earth
 ~~~~~~~~~~~~
 
-This response converts a Pydap dataset to a `KML <http://code.google.com/apis/kml/documentation/kmlreference.html>`_ representation, allowing the data to be visualized using Google Earth as a client. Simply install it with `pip <http://pypi.python.org/pypi/pip>`_:
+This response converts a pydap dataset to a `KML <http://code.google.com/apis/kml/documentation/kmlreference.html>`_ representation, allowing the data to be visualized using Google Earth as a client. Simply install it with `pip <http://pypi.python.org/pypi/pip>`_:
 
 .. code-block:: bash
 
     $ pip install pydap.responses.kml
 
 And open a URL by appending the ``.kml`` extension to the dataset, say::
```

### Comparing `Pydap-3.2.2/docs/_build/html/_sources/developer_responses.rst.txt` & `pydap-3.4.0/docs/developer_responses.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Responses
 ---------
 
-If handlers are responsible for converting data into the Pydap data model, responses to the opposite: the convert from the data model to different representations. The Opendap specification defines a series of standard responses, that allow clients to introspect a dataset by downloading metadata, and later download data for the subset of interest. These standard responses are the DDS (Dataset Descriptor Structure), the DAS (Dataset Attribute Structure) and the DODS response.
+If handlers are responsible for converting data into the pydap data model, responses to the opposite: the convert from the data model to different representations. The Opendap specification defines a series of standard responses, that allow clients to introspect a dataset by downloading metadata, and later download data for the subset of interest. These standard responses are the DDS (Dataset Descriptor Structure), the DAS (Dataset Attribute Structure) and the DODS response.
 
 Apart from these, there are additional non-standard responses that add functionality to the server. The ASCII response, for example, formats the data as ASCII for quick visualization on the browser; the HTML response builds a form from which the user can select a subset of the data.
 
-Here is an example of a minimal Pydap response that returns the attributes of the dataset as JSON:
+Here is an example of a minimal pydap response that returns the attributes of the dataset as JSON:
 
 .. code-block:: python
 
     from simplejson import dumps
 
     from pydap.responses.lib import BaseResponse
     from pydap.lib import walk
@@ -70,8 +70,8 @@
             dataset.attributes['foo'] = 'bar'
 
             # return original response
             response = BaseHandler.response_map[ environ['pydap.response'] ]
             responder = response(dataset)
             return responder(environ, start_response)
 
-The code should actually do more bookkeeping, like checking if the dataset can be retrieved from the response or updating the ``Content-Length`` header, but I wanted to keep it simple. Pydap comes with a WSGI middleware for handling server-side functions (``pydap.wsgi.ssf``) that makes heavy use of this feature. It works by removing function calls from the request, fetching the dataset from the modified request, applying the function calls and returning a new dataset.
+The code should actually do more bookkeeping, like checking if the dataset can be retrieved from the response or updating the ``Content-Length`` header, but I wanted to keep it simple. pydap comes with a WSGI middleware for handling server-side functions (``pydap.wsgi.ssf``) that makes heavy use of this feature. It works by removing function calls from the request, fetching the dataset from the modified request, applying the function calls and returning a new dataset.
```

### Comparing `Pydap-3.2.2/docs/_build/html/_sources/license.rst.txt` & `pydap-3.4.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-License
-=======
+The MIT License
 
-Copyright (c) 2003--2010 Roberto De Almeida
+Copyright (c) 2003-2010 Roberto De Almeida
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -16,8 +15,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
-
```

### Comparing `Pydap-3.2.2/docs/index.rst` & `pydap-3.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,41 @@
-.. pydap documentation master file, created by sphinx-quickstart on Tue May  6 23:41:51 2008.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
-
-Pydap
+pydap
 =====
 
-Pydap is a pure `Python <http://python.org/>`_ library implementing the `Data Access Protocol <http://opendap.org/>`_, also known as **DODS** or **OPeNDAP**. You can use Pydap as a `client <client.html>`_ to access hundreds of scientific datasets in a transparent and efficient way through the internet; or as a server to easily `distribute <server.html>`_ your data from a `variety of formats <handlers.html>`_.
+[![Build Status](https://travis-ci.org/pydap/pydap.svg)](https://travis-ci.org/pydap/pydap)
+[![Python3](https://img.shields.io/badge/python-3-blue.svg)](https://www.python.org/downloads/)
+[![PyPI](https://img.shields.io/pypi/v/pydap.svg?maxAge=2592000?style=plastic)](https://pypi.python.org/pypi/pydap/)
+[![Join the chat at https://gitter.im/pydap/pydap](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/pydap/pydap) 
+
+[pydap](https://pydap.github.io/pydap/) is an implementation of the
+Opendap/DODS protocol, written from scratch in pure python.  You can
+use pydap to access scientific data on the internet without having to
+download it; instead, you work with special array and iterable objects
+that download data on-the-fly as necessary, saving bandwidth and
+time. The module also comes with a robust-but-lightweight Opendap
+server, implemented as a WSGI application.
+
 
 Quickstart
 ----------
 
-You can install the latest version (|release|) using `pip <http://pypi.python.org/pypi/pip>`_. After `installing pip <http://www.pip-installer.org/en/latest/installing.html>`_ you can install Pydap with this command:
-
-.. code-block:: bash
-
-    $ pip install Pydap
+You can install the latest version using
+[pip](http://pypi.python.org/pypi/pip). After [installing
+pip](http://www.pip-installer.org/en/latest/installing.html) you can
+install pydap with this command:
+
+```bash
+    $ pip install pydap
+```
+
+This will install pydap together with all the required
+dependencies. You can now open any remotely served dataset, and pydap
+will download the accessed data on-the-fly as needed:
 
-This will install Pydap together with all the required dependencies. You can now open any remotely served dataset, and Pydap will download the accessed data on-the-fly as needed:
-
-.. doctest:: 
+```python
 
     >>> from pydap.client import open_url
     >>> dataset = open_url('http://test.opendap.org/dap/data/nc/coads_climatology.nc')
     >>> var = dataset['SST']
     >>> var.shape
     (12, 90, 180)
     >>> var.dtype
@@ -35,48 +48,52 @@
               -9.99999979e+33],
             [ -7.69166648e-01,  -7.79999971e-01,  -6.75454497e-01,
               -5.95714271e-01],
             [  1.28333330e-01,  -5.00000156e-02,  -6.36363626e-02,
               -1.41666666e-01],
             [  6.38000011e-01,   8.95384610e-01,   7.21666634e-01,
                8.10000002e-01]]], dtype=float32), array([ 366.]), array([-69., -67., -65., -63.]), array([ 41.,  43.,  45.,  47.])]
+```
 
-For more information, please check the documentation on `using Pydap as a client <client.html>`_. Pydap also comes with a simple server, implemented as a `WSGI <http://wsgi.org/>`_ application. To use it, you first need to install Pydap with the server extras dependencies. If you want to serve `netCDF <http://www.unidata.ucar.edu/software/netcdf/>`_ files, install Pydap with the ``handlers.netcdf`` extra:
-
-.. code-block:: bash
+For more information, please check the documentation on [using pydap
+as a client](https://pydap.github.io/pydap/client.html). pydap also
+comes with a simple server, implemented as a [WSGI]( http://wsgi.org/)
+application. To use it, you first need to install the server and
+optionally a data handler:
 
-    $ pip install Pydap[server,handlers.netcdf]
+```bash
 
-More `handlers <handlers.html>`_ for different formats are available, if necessary. To run a simple standalone server just issue the command:
+    $ pip install pydap[server,handlers.netcdf]
+```
 
-.. code-block:: bash
+This will install support for
+[netCDF](http://www.unidata.ucar.edu/software/netcdf/) files; more
+[handlers](https://pydap.github.io/pydap/handlers.html) for
+different formats are available, if necessary. Now create a directory
+for your server data.
 
-    $ pydap --data ./myserver/data/ --port 8001
 
-This will start a standalone server running on http://localhost:8001/, serving netCDF files from ``./myserver/data/``, similar to the test server at http://test.pydap.org/. Since the server uses the `WSGI <http://wsgi.org/>`_ standard, it can easily be run behind Apache. The `server documentation <server.html>`_ has more information on how to better deploy Pydap.
+To run the server just issue the command:
 
-Help
-----
+```bash
 
-If you need any help with Pydap, please feel free to send an email to the `mailing list <http://groups.google.com/group/pydap/>`_.
+    $ pydap --data ./myserver/data/ --port 8001
+```
 
-Documentation
--------------
+This will start a standalone server running on http://localhost:8001/,
+serving netCDF files from ``./myserver/data/``, similar to the test
+server at http://test.pydap.org/. Since the server uses the
+[WSGI](http://wsgi.org/) standard, it can easily be run behind
+Apache. The [server
+documentation](https://pydap.github.io/pydap/server.html) has
+more information on how to better deploy pydap.
 
-.. toctree::
-   :maxdepth: 2
+## Documentation
 
-   client
-   server
-   handlers
-   responses
-   developer
-   Changelog
-   license
+For more information, see [the pydap
+documentation](https://pydap.github.io/pydap/).
 
-Indices and tables
-==================
+## Help
 
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
+If you need any help with pydap, please feel free to send an email to
+the [mailing list](http://groups.google.com/group/pydap/)
```

### Comparing `Pydap-3.2.2/docs/Special chars.odt` & `pydap-3.4.0/docs/Special chars.odt`

 * *Files identical despite different names*

### Comparing `Pydap-3.2.2/docs/make.bat` & `pydap-3.4.0/docs/make.bat`

 * *Files 0% similar despite different names*

```diff
@@ -69,17 +69,17 @@
 )
 
 if "%1" == "qthelp" (
 	%SPHINXBUILD% -b qthelp %ALLSPHINXOPTS% _build/qthelp
 	echo.
 	echo.Build finished; now you can run "qcollectiongenerator" with the ^
 .qhcp project file in _build/qthelp, like this:
-	echo.^> qcollectiongenerator _build\qthelp\Pydap.qhcp
+	echo.^> qcollectiongenerator _build\qthelp\pydap.qhcp
 	echo.To view the help file:
-	echo.^> assistant -collectionFile _build\qthelp\Pydap.ghc
+	echo.^> assistant -collectionFile _build\qthelp\pydap.ghc
 	goto end
 )
 
 if "%1" == "latex" (
 	%SPHINXBUILD% -b latex %ALLSPHINXOPTS% _build/latex
 	echo.
 	echo.Build finished; the LaTeX files are in _build/latex.
```

### Comparing `Pydap-3.2.2/docs/conf.py` & `pydap-3.4.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Pydap documentation build configuration file, created by
+# pydap documentation build configuration file, created by
 # sphinx-quickstart on Fri May 22 10:12:59 2009.
 #
 # This file is execfile()d with the current directory set to its containing dir.
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
@@ -35,16 +35,16 @@
 # The encoding of source files.
 #source_encoding = 'utf-8'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'Pydap'
-copyright = u'2003-2017, Pydap contributors'
+project = u'pydap'
+copyright = u'2003-2017, pydap contributors'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 #version = '3.0'
@@ -159,29 +159,29 @@
 # base URL from which the finished HTML is served.
 html_use_opensearch = 'http://pydap.org/'
 
 # If nonempty, this is the file name suffix for HTML files (e.g. ".xhtml").
 #html_file_suffix = ''
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'Pydapdoc'
+htmlhelp_basename = 'pydapdoc'
 
 
 # -- Options for LaTeX output --------------------------------------------------
 
 # The paper size ('letter' or 'a4').
 #latex_paper_size = 'letter'
 
 # The font size ('10pt', '11pt' or '12pt').
 #latex_font_size = '10pt'
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-  ('index', 'Pydap.tex', u'Pydap Documentation',
+  ('index', 'pydap.tex', u'pydap Documentation',
    u'Roberto De Almeida', 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 #latex_logo = None
```

