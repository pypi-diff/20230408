# Comparing `tmp/cx_Freeze-6.8b5.tar.gz` & `tmp/cx_Freeze-6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wheelhouse/cx_Freeze-6.8b5.tar", last modified: Fri Sep  3 06:28:16 2021, max compression
+gzip compressed data, was "cx_Freeze-6.9.tar", last modified: Wed Dec  8 02:48:07 2021, max compression
```

## Comparing `cx_Freeze-6.8b5.tar` & `cx_Freeze-6.9.tar`

### file list

```diff
@@ -1,206 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/
--rw-r--r--   0 runner    (1001) docker     (121)     1781 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/test/
--rw-r--r--   0 runner    (1001) docker     (121)      845 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/test/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1843 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/test/test_finder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/test/test_zip_packages.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/
--rw-r--r--   0 runner    (1001) docker     (121)    43276 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/freezer.py
--rw-r--r--   0 runner    (1001) docker     (121)    12803 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2193 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/winmsvcr.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/openpyxl/
--rw-r--r--   0 runner    (1001) docker     (121)      727 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/openpyxl/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      552 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/openpyxl/test_openpyxl.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pyzmq/
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pyzmq/pyzmq_server.py
--rw-r--r--   0 runner    (1001) docker     (121)      584 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pyzmq/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pyzmq/pyzmq_client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/Tkinter/
--rw-r--r--   0 runner    (1001) docker     (121)      764 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/Tkinter/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/Tkinter/SimpleTkApp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/ctypes/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/ctypes/test_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (121)      610 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/ctypes/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/plist_items/
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/plist_items/hello.py
--rw-r--r--   0 runner    (1001) docker     (121)      808 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/plist_items/run.py
--rw-r--r--   0 runner    (1001) docker     (121)      858 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/plist_items/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/plist_items/data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/simple/
--rw-r--r--   0 runner    (1001) docker     (121)      482 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/simple/hello.py
--rw-r--r--   0 runner    (1001) docker     (121)      604 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/simple/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/distutils/
--rw-r--r--   0 runner    (1001) docker     (121)      612 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/distutils/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/distutils/test_dist.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/importlib/
--rw-r--r--   0 runner    (1001) docker     (121)      515 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/importlib/get_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)      489 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/importlib/wsgiserver.py
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/importlib/web_srv.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/importlib/server_simple.py
--rw-r--r--   0 runner    (1001) docker     (121)      898 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/importlib/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/asmodule/
--rw-r--r--   0 runner    (1001) docker     (121)      668 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/asmodule/asmodule.py
--rw-r--r--   0 runner    (1001) docker     (121)      589 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/asmodule/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/icon/
--rw-r--r--   0 runner    (1001) docker     (121)      469 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/icon/test_icon.py
--rw-r--r--   0 runner    (1001) docker     (121)      516 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/icon/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/wx/
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/wx/wxapp.py
--rw-r--r--   0 runner    (1001) docker     (121)      760 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/wx/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pycountry/
--rw-r--r--   0 runner    (1001) docker     (121)      326 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pycountry/test.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pycountry/setup_zip.py
--rw-r--r--   0 runner    (1001) docker     (121)      467 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pycountry/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pyside2/
--rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pyside2/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      526 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pyside2/PySide2app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/service/
--rw-r--r--   0 runner    (1001) docker     (121)     1882 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/service/Config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/service/ServiceHandler.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/service/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/bcrypt/
--rw-r--r--   0 runner    (1001) docker     (121)      647 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/bcrypt/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/bcrypt/test_bcrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/advanced/
--rw-r--r--   0 runner    (1001) docker     (121)      899 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/advanced/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/advanced/modules/
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/advanced/modules/testfreeze_1.py
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/advanced/modules/testfreeze_2.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/advanced/advanced_2.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/advanced/advanced_1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pydantic/
--rw-r--r--   0 runner    (1001) docker     (121)      492 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pydantic/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pydantic/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/sqlite/
--rw-r--r--   0 runner    (1001) docker     (121)      692 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/sqlite/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      598 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/sqlite/test_sqlite3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/build_constants/
--rw-r--r--   0 runner    (1001) docker     (121)      588 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/build_constants/hello.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/build_constants/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/dependencies/
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/dependencies/test_1.py
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/dependencies/getdependentfiles.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/find_spec/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/find_spec/hello.py
--rw-r--r--   0 runner    (1001) docker     (121)      216 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/find_spec/run.py
--rw-r--r--   0 runner    (1001) docker     (121)      631 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/find_spec/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/find_spec/dummypackage/
--rw-r--r--   0 runner    (1001) docker     (121)      117 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/find_spec/dummypackage/dummymodule.py
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/find_spec/dummypackage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pillow/
--rw-r--r--   0 runner    (1001) docker     (121)      555 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pillow/test_pillow.py
--rw-r--r--   0 runner    (1001) docker     (121)      657 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pillow/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/msi_binary_data/
--rw-r--r--   0 runner    (1001) docker     (121)      524 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/msi_binary_data/hello.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/msi_binary_data/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/zope/
--rw-r--r--   0 runner    (1001) docker     (121)      563 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/zope/qotd.py
--rw-r--r--   0 runner    (1001) docker     (121)      720 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/zope/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/relimport/
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/relimport/relimport.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/relimport/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/relimport/pkg1/
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/relimport/pkg1/sub6.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/relimport/pkg1/sub4.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/relimport/pkg1/pkg2/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/relimport/pkg1/pkg2/sub5.py
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/relimport/pkg1/pkg2/sub3.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/relimport/pkg1/pkg2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/relimport/pkg1/sub2.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/relimport/pkg1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/relimport/pkg1/sub1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pandas/
--rw-r--r--   0 runner    (1001) docker     (121)      591 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pandas/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      238 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pandas/test_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/tz/
--rw-r--r--   0 runner    (1001) docker     (121)      628 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/tz/test_tz.py
--rw-r--r--   0 runner    (1001) docker     (121)      870 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/tz/setup_zip.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/tz/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/msi_extensions/
--rw-r--r--   0 runner    (1001) docker     (121)      561 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/msi_extensions/hello.py
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/msi_extensions/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pytz/
--rw-r--r--   0 runner    (1001) docker     (121)      852 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pytz/setup_zip.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pytz/test_pytz.py
--rw-r--r--   0 runner    (1001) docker     (121)      525 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pytz/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/cryptography/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/cryptography/test_crypt.py
--rw-r--r--   0 runner    (1001) docker     (121)      672 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/cryptography/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/matplotlib/
--rw-r--r--   0 runner    (1001) docker     (121)      617 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/matplotlib/matplotlib_afm.py
--rw-r--r--   0 runner    (1001) docker     (121)     1358 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/matplotlib/setup_zip.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/matplotlib/matplotlib_eg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/matplotlib/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pyqt5/
--rwxr-xr-x   0 runner    (1001) docker     (121)      520 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pyqt5/PyQt5app.py
--rw-r--r--   0 runner    (1001) docker     (121)      861 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pyqt5/setup_zip.py
--rw-r--r--   0 runner    (1001) docker     (121)     1684 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pyqt5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pythonnet-demo/
--rw-r--r--   0 runner    (1001) docker     (121)      702 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pythonnet-demo/DynamicGrid.py
--rw-r--r--   0 runner    (1001) docker     (121)     1738 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pythonnet-demo/helloform.py
--rw-r--r--   0 runner    (1001) docker     (121)      576 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pythonnet-demo/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     2984 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pythonnet-demo/splitter.py
--rw-r--r--   0 runner    (1001) docker     (121)    14174 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/pythonnet-demo/wordpad.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/samples/msi_summary_data/
--rw-r--r--   0 runner    (1001) docker     (121)      524 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/msi_summary_data/hello.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/samples/msi_summary_data/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     4444 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/common.py
--rw-r--r--   0 runner    (1001) docker     (121)    15513 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/dist.py
--rw-r--r--   0 runner    (1001) docker     (121)     7658 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/module.py
--rw-r--r--   0 runner    (1001) docker     (121)    23797 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/darwintools.py
--rw-r--r--   0 runner    (1001) docker     (121)    28983 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/finder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3895 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/setupwriter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze/initscripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      971 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/initscripts/ConsoleSetLibPath.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      412 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/initscripts/SharedLib.py
--rw-r--r--   0 runner    (1001) docker     (121)     3760 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/initscripts/__startup__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      799 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/initscripts/SharedLibSource.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      348 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/initscripts/Console.py
--rw-r--r--   0 runner    (1001) docker     (121)      807 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      147 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6069 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/executable.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/winversioninfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4747 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/patchelf.py
--rw-r--r--   0 runner    (1001) docker     (121)    16736 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/macdist.py
--rw-r--r--   0 runner    (1001) docker     (121)    54767 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/exception.py
--rw-r--r--   0 runner    (1001) docker     (121)    32194 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/cx_Freeze/windist.py
--rw-r--r--   0 runner    (1001) docker     (121)     4017 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     9487 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       98 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5278 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       70 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4017 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       10 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/cx_Freeze.egg-info/dependency_links.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/source/bases/
--rw-r--r--   0 runner    (1001) docker     (121)    24700 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/source/bases/Win32Service.c
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/source/bases/dummy.rc
--rwxr-xr-x   0 runner    (1001) docker     (121)      938 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/source/bases/manifest.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6145 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/source/bases/Common.c
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/source/bases/Console.c
--rw-r--r--   0 runner    (1001) docker     (121)     8411 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/source/bases/Win32GUI.c
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/source/bases/manifest.rc
--rw-r--r--   0 runner    (1001) docker     (121)     5138 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/source/bases/cx_Logging.h
--rw-r--r--   0 runner    (1001) docker     (121)    20250 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/source/util.c
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/doc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/doc/src/
--rw-r--r--   0 runner    (1001) docker     (121)     7731 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/doc/src/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     6118 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/doc/src/script.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2866 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/doc/src/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)    59930 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/doc/src/releasenotes.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1206 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/doc/src/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    23511 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/doc/src/setup_script.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4377 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/doc/src/faq.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2836 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/doc/src/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1147 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/doc/src/overview.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-03 06:28:16.000000 cx_Freeze-6.8b5/doc/src/development/
--rw-r--r--   0 runner    (1001) docker     (121)     1499 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/doc/src/development/code_layout.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2833 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/doc/src/development/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      575 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      192 2021-09-03 06:28:07.000000 cx_Freeze-6.8b5/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.563285 cx_Freeze-6.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2021-12-08 02:48:02.000000 cx_Freeze-6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4132 2021-12-08 02:48:07.563285 cx_Freeze-6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2481 2021-12-08 02:48:02.000000 cx_Freeze-6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.551285 cx_Freeze-6.9/cx_Freeze/
+-rw-r--r--   0 runner    (1001) docker     (121)      807 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12803 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4444 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24581 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/darwintools.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15513 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/dist.py
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/exception.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6069 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/executable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29362 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/finder.py
+-rw-r--r--   0 runner    (1001) docker     (121)    44658 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/freezer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    56284 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.551285 cx_Freeze-6.9/cx_Freeze/initscripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      348 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/initscripts/Console.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      971 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/initscripts/ConsoleSetLibPath.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      412 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/initscripts/SharedLib.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      799 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/initscripts/SharedLibSource.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3760 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/initscripts/__startup__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16827 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/macdist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7863 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4747 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/patchelf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.547285 cx_Freeze-6.9/cx_Freeze/samples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.551285 cx_Freeze-6.9/cx_Freeze/samples/Tkinter/
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/Tkinter/SimpleTkApp.py
+-rw-r--r--   0 runner    (1001) docker     (121)      764 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/Tkinter/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.551285 cx_Freeze-6.9/cx_Freeze/samples/advanced/
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/advanced/advanced_1.py
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/advanced/advanced_2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.551285 cx_Freeze-6.9/cx_Freeze/samples/advanced/modules/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/advanced/modules/testfreeze_1.py
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/advanced/modules/testfreeze_2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/advanced/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.551285 cx_Freeze-6.9/cx_Freeze/samples/asmodule/
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/asmodule/asmodule.py
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/asmodule/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.551285 cx_Freeze-6.9/cx_Freeze/samples/bcrypt/
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/bcrypt/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/bcrypt/test_bcrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.551285 cx_Freeze-6.9/cx_Freeze/samples/build_constants/
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/build_constants/hello.py
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/build_constants/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.551285 cx_Freeze-6.9/cx_Freeze/samples/cryptography/
+-rw-r--r--   0 runner    (1001) docker     (121)      672 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/cryptography/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/cryptography/test_crypt.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.551285 cx_Freeze-6.9/cx_Freeze/samples/ctypes/
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/ctypes/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/ctypes/test_ctypes.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.551285 cx_Freeze-6.9/cx_Freeze/samples/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (121)     1534 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/dependencies/getdependentfiles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/dependencies/test_1.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.551285 cx_Freeze-6.9/cx_Freeze/samples/distutils/
+-rw-r--r--   0 runner    (1001) docker     (121)      612 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/distutils/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/distutils/test_dist.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.551285 cx_Freeze-6.9/cx_Freeze/samples/find_spec/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/find_spec/dummypackage/
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/find_spec/dummypackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      117 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/find_spec/dummypackage/dummymodule.py
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/find_spec/hello.py
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/find_spec/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/find_spec/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/icon/
+-rw-r--r--   0 runner    (1001) docker     (121)      516 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/icon/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      469 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/icon/test_icon.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/importlib/
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/importlib/get_examples.py
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/importlib/server_simple.py
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/importlib/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1384 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/importlib/web_srv.py
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/importlib/wsgiserver.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/matplotlib/
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/matplotlib/matplotlib_afm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1646 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/matplotlib/matplotlib_eg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1047 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/matplotlib/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1358 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/matplotlib/setup_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/msi_binary_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/msi_binary_data/hello.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1015 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/msi_binary_data/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/msi_extensions/
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/msi_extensions/hello.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2080 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/msi_extensions/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/msi_summary_data/
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/msi_summary_data/hello.py
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/msi_summary_data/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/openpyxl/
+-rw-r--r--   0 runner    (1001) docker     (121)      727 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/openpyxl/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      552 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/openpyxl/test_openpyxl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/pandas/
+-rw-r--r--   0 runner    (1001) docker     (121)      591 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pandas/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pandas/test_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/pillow/
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pillow/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      555 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pillow/test_pillow.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/plist_items/
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/plist_items/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/plist_items/hello.py
+-rw-r--r--   0 runner    (1001) docker     (121)      808 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/plist_items/run.py
+-rw-r--r--   0 runner    (1001) docker     (121)      858 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/plist_items/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/pycountry/
+-rw-r--r--   0 runner    (1001) docker     (121)      467 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pycountry/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pycountry/setup_zip.py
+-rw-r--r--   0 runner    (1001) docker     (121)      326 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pycountry/test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (121)      546 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pydantic/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      492 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pydantic/test_pydantic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/pyqt5/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      520 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pyqt5/PyQt5app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1684 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pyqt5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1727 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pyqt5/setup_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/pyside2/
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pyside2/PySide2app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1025 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pyside2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/pythonnet-demo/
+-rw-r--r--   0 runner    (1001) docker     (121)      702 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pythonnet-demo/DynamicGrid.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1738 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pythonnet-demo/helloform.py
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pythonnet-demo/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2984 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pythonnet-demo/splitter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14174 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pythonnet-demo/wordpad.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.555285 cx_Freeze-6.9/cx_Freeze/samples/pytz/
+-rw-r--r--   0 runner    (1001) docker     (121)      525 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pytz/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      852 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pytz/setup_zip.py
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pytz/test_pytz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.559285 cx_Freeze-6.9/cx_Freeze/samples/pyzmq/
+-rw-r--r--   0 runner    (1001) docker     (121)     1319 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pyzmq/pyzmq_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1092 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pyzmq/pyzmq_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/pyzmq/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.559285 cx_Freeze-6.9/cx_Freeze/samples/relimport/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.559285 cx_Freeze-6.9/cx_Freeze/samples/relimport/pkg1/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/relimport/pkg1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.559285 cx_Freeze-6.9/cx_Freeze/samples/relimport/pkg1/pkg2/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/relimport/pkg1/pkg2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/relimport/pkg1/pkg2/sub3.py
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/relimport/pkg1/pkg2/sub5.py
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/relimport/pkg1/sub1.py
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/relimport/pkg1/sub2.py
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/relimport/pkg1/sub4.py
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/relimport/pkg1/sub6.py
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/relimport/relimport.py
+-rw-r--r--   0 runner    (1001) docker     (121)      572 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/relimport/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.559285 cx_Freeze-6.9/cx_Freeze/samples/service/
+-rw-r--r--   0 runner    (1001) docker     (121)     1882 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/service/Config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/service/ServiceHandler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      974 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/service/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.559285 cx_Freeze-6.9/cx_Freeze/samples/simple/
+-rw-r--r--   0 runner    (1001) docker     (121)      482 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/simple/hello.py
+-rw-r--r--   0 runner    (1001) docker     (121)      604 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/simple/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.559285 cx_Freeze-6.9/cx_Freeze/samples/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/sqlite/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      598 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/sqlite/test_sqlite3.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.559285 cx_Freeze-6.9/cx_Freeze/samples/tz/
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/tz/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/tz/setup_zip.py
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/tz/test_tz.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.559285 cx_Freeze-6.9/cx_Freeze/samples/wx/
+-rw-r--r--   0 runner    (1001) docker     (121)      760 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/wx/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/wx/wxapp.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.559285 cx_Freeze-6.9/cx_Freeze/samples/zope/
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/zope/qotd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      720 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/samples/zope/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3895 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/setupwriter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32507 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/windist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2193 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/winmsvcr.py
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2021-12-08 02:48:02.000000 cx_Freeze-6.9/cx_Freeze/winversioninfo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.551285 cx_Freeze-6.9/cx_Freeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4132 2021-12-08 02:48:07.000000 cx_Freeze-6.9/cx_Freeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5214 2021-12-08 02:48:07.000000 cx_Freeze-6.9/cx_Freeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-08 02:48:07.000000 cx_Freeze-6.9/cx_Freeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       98 2021-12-08 02:48:07.000000 cx_Freeze-6.9/cx_Freeze.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-08 02:48:07.000000 cx_Freeze-6.9/cx_Freeze.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2021-12-08 02:48:07.000000 cx_Freeze-6.9/cx_Freeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2021-12-08 02:48:07.000000 cx_Freeze-6.9/cx_Freeze.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.559285 cx_Freeze-6.9/doc/
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2021-12-08 02:48:02.000000 cx_Freeze-6.9/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.559285 cx_Freeze-6.9/doc/src/
+-rw-r--r--   0 runner    (1001) docker     (121)     7731 2021-12-08 02:48:02.000000 cx_Freeze-6.9/doc/src/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.559285 cx_Freeze-6.9/doc/src/development/
+-rw-r--r--   0 runner    (1001) docker     (121)     1499 2021-12-08 02:48:02.000000 cx_Freeze-6.9/doc/src/development/code_layout.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2833 2021-12-08 02:48:02.000000 cx_Freeze-6.9/doc/src/development/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5195 2021-12-08 02:48:02.000000 cx_Freeze-6.9/doc/src/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2021-12-08 02:48:02.000000 cx_Freeze-6.9/doc/src/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3131 2021-12-08 02:48:02.000000 cx_Freeze-6.9/doc/src/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2866 2021-12-08 02:48:02.000000 cx_Freeze-6.9/doc/src/license.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2021-12-08 02:48:02.000000 cx_Freeze-6.9/doc/src/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    65741 2021-12-08 02:48:02.000000 cx_Freeze-6.9/doc/src/releasenotes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6118 2021-12-08 02:48:02.000000 cx_Freeze-6.9/doc/src/script.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    23630 2021-12-08 02:48:02.000000 cx_Freeze-6.9/doc/src/setup_script.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1819 2021-12-08 02:48:07.563285 cx_Freeze-6.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9526 2021-12-08 02:48:02.000000 cx_Freeze-6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.559285 cx_Freeze-6.9/source/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-08 02:48:07.563285 cx_Freeze-6.9/source/bases/
+-rw-r--r--   0 runner    (1001) docker     (121)     6091 2021-12-08 02:48:02.000000 cx_Freeze-6.9/source/bases/Common.c
+-rw-r--r--   0 runner    (1001) docker     (121)     3342 2021-12-08 02:48:02.000000 cx_Freeze-6.9/source/bases/Console.c
+-rw-r--r--   0 runner    (1001) docker     (121)     8411 2021-12-08 02:48:02.000000 cx_Freeze-6.9/source/bases/Win32GUI.c
+-rw-r--r--   0 runner    (1001) docker     (121)    24700 2021-12-08 02:48:02.000000 cx_Freeze-6.9/source/bases/Win32Service.c
+-rw-r--r--   0 runner    (1001) docker     (121)     5138 2021-12-08 02:48:02.000000 cx_Freeze-6.9/source/bases/cx_Logging.h
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2021-12-08 02:48:02.000000 cx_Freeze-6.9/source/bases/dummy.rc
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2021-12-08 02:48:02.000000 cx_Freeze-6.9/source/bases/manifest.rc
+-rwxr-xr-x   0 runner    (1001) docker     (121)      938 2021-12-08 02:48:02.000000 cx_Freeze-6.9/source/bases/manifest.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    20250 2021-12-08 02:48:02.000000 cx_Freeze-6.9/source/util.c
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cx_Freeze-6.8b5/setup.cfg` & `cx_Freeze-6.9/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 0
 
 [metadata]
 name = cx_Freeze
-version = 6.8b5
+version = 6.9
 url = https://marcelotduarte.github.io/cx_Freeze
 project_urls = 
 	Bug Tracker = https://github.com/marcelotduarte/cx_Freeze/issues
 	CI: GitHub Workflows = https://github.com/marcelotduarte/cx_Freeze/actions?query=branch:main
 	Source Code = https://github.com/marcelotduarte/cx_Freeze
 description = Create standalone executables from Python scripts
 long_description = file: README.md
@@ -27,14 +27,15 @@
 	Programming Language :: C
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Software Development :: Build Tools
 	Topic :: Software Development :: Libraries :: Python Modules
 	Topic :: System :: Software Distribution
 	Topic :: Utilities
 keywords = 
 	cx-freeze cxfreeze cx_Freeze freeze python
```

### Comparing `cx_Freeze-6.8b5/cx_Freeze/freezer.py` & `cx_Freeze-6.9/cx_Freeze/freezer.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 
         if target in self.files_copied:
             return
         if source == target:
             return
         self._create_directory(target.parent)
         if self.silent < 1:
-            print(f"copying {source!s} -> {target!s}")
+            print(f"copying {source} -> {target}")
         shutil.copyfile(source, target)
         shutil.copystat(source, target)
         if include_mode:
             shutil.copymode(source, target)
         self.files_copied.add(target)
 
         # handle post-copy tasks, including copying dependencies
@@ -194,15 +194,15 @@
         """Post-copy task."""
 
     def _create_directory(self, path: Union[str, Path]):
         if isinstance(path, str):
             path = Path(path)
         if not path.is_dir():
             if self.silent < 1:
-                print(f"creating directory {path!s}")
+                print(f"creating directory {path}")
             path.mkdir(parents=True, exist_ok=True)
 
     def _freeze_executable(self, exe: Executable) -> None:
         finder: ModuleFinder = self.finder
         finder.IncludeFile(exe.main_script, exe.main_module_name)
         finder.IncludeFile(exe.init_script, exe.init_module_name)
         finder.IncludeFile(
@@ -317,23 +317,23 @@
             finder.IncludePackage(name)
         return finder
 
     def _post_freeze_hook(self) -> None:
         """Platform-specific post-Freeze work."""
 
     def _print_report(self, filename: Path, modules: List[Module]) -> None:
-        print(f"writing zip file {filename!s}\n")
+        print(f"writing zip file {filename}\n")
         print("  {:<25} {}".format("Name", "File"))
         print("  {:<25} {}".format("----", "----"))
         for module in modules:
             if module.path:
                 print("P", end="")
             else:
                 print("m", end="")
-            print(f" {module.name:<25} {(module.file or '')!s}")
+            print(f" {module.name:<25} {module.file or ''}")
 
     @staticmethod
     def _remove_version_numbers(filename: str) -> str:
         tweaked = False
         parts = filename.split(".")
         while parts:
             if not parts[-1].isdigit():
@@ -467,27 +467,32 @@
             # a number of packages make the assumption that files that they
             # require will be found in a location relative to where
             # they are located on disk; these packages will fail with strange
             # errors when they are written to a zip file instead
             include_in_file_system = module.in_file_system
 
             # if the module refers to a package, check to see if this package
-            # should be included in the zip file or should be written to the
-            # file system; if the package should be written to the file system,
-            # any non-Python files are copied at this point if the target
-            # directory does not already exist
+            # should be written to the file system
             if (
-                include_in_file_system
+                include_in_file_system >= 1
                 and module.path is not None
                 and module.file is not None
             ):
                 parts = module.name.split(".")
                 target_package_dir = target_lib_dir.joinpath(*parts)
-                source_package_dir = module.file.parent
-                if not target_package_dir.exists():
+                if include_in_file_system == 2:
+                    # a few packages are optimized on the hooks,
+                    # so for now create the directory for this package
+                    self._create_directory(target_package_dir)
+
+                elif not target_package_dir.exists():
+                    # whether the package and its data will be written to the
+                    # file system, any non-Python files are copied at this
+                    # point if the target directory does not already exist
+                    source_package_dir = module.file.parent
                     if self.silent < 1:
                         print(f"copying data from package {module.name}...")
                     shutil.copytree(
                         source_package_dir,
                         target_package_dir,
                         ignore=ignorePatterns,
                     )
@@ -508,15 +513,15 @@
             # if an extension module is found in a package that is to be
             # included in a zip file, copy the actual file to the build
             # directory because shared libraries cannot be loaded from a
             # zip file
             if (
                 module.code is None
                 and module.file is not None
-                and not include_in_file_system
+                and include_in_file_system == 0
             ):
                 parts = module.name.split(".")[:-1]
                 parts.append(module.file.name)
                 target = target_lib_dir / ".".join(parts)
                 files_to_copy.append((module, target))
 
             # starting with Python 3.3 the pyc file format contains the source
@@ -533,15 +538,15 @@
                 if sys.version_info[:2] < (3, 7):
                     header = MAGIC_NUMBER + struct.pack("<ii", mtime, size)
                 else:
                     header = MAGIC_NUMBER + struct.pack("<iii", 0, mtime, size)
                 data = header + marshal.dumps(module.code)
 
             # if the module should be written to the file system, do so
-            if include_in_file_system and module.file is not None:
+            if include_in_file_system >= 1 and module.file is not None:
                 parts = module.name.split(".")
                 if module.code is None:
                     parts.pop()
                     parts.append(module.file.name)
                     target_name = target_lib_dir.joinpath(*parts)
                     self._copy_file(
                         module.file,
@@ -930,15 +935,15 @@
                     self.darwinTracker.getDarwinFile(source, target)
                 )
             return
         if source == target:
             return
         self._create_directory(target.parent)
         if self.silent < 1:
-            print(f"copying {source!s} -> {target!s}")
+            print(f"copying {source} -> {target}")
         shutil.copyfile(source, target)
         shutil.copystat(source, target)
         if include_mode:
             shutil.copymode(source, target)
         self.files_copied.add(target)
 
         # handle post-copy tasks, including copying dependencies
@@ -1007,17 +1012,30 @@
         return dependent_files
 
 
 class LinuxFreezer(Freezer):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.patchelf = Patchelf()
+        self._symlinks: Set[Tuple[Path, str]] = set()
 
     def _pre_copy_hook(self, source: Path, target: Path) -> Tuple[Path, Path]:
-        """Prepare the source and target paths."""
+        """Prepare the source and target paths. Also, ensures that the source
+        of a symlink is copied deferring the link creation."""
+        if source.is_symlink():
+            real_source = source.resolve()
+            symlink = os.readlink(source)
+            real_target = (target.parent / symlink).resolve()
+            try:
+                real_target.relative_to(self.targetdir / "lib")
+            except ValueError:
+                symlink = real_source.name
+                real_target = target.with_name(symlink)
+            self._symlinks.add((target, symlink))
+            return real_source, real_target
         return source, target
 
     def _post_copy_hook(
         self,
         source: Path,
         target: Path,
         copy_dependent_files: bool,
@@ -1044,31 +1062,44 @@
                     if dependent_target not in self.files_copied:
                         for file in self.files_copied:
                             if file.name == dependent_filename:
                                 relative = file.relative_to(library_dir)
                                 dependent_target = library_dir / relative
                                 break
                 else:
-                    if targetdir == library_dir:
-                        parts = relative.parts
+                    dependent_target = targetdir / relative
+                    dependent_target = dependent_target.resolve()
+                    try:
+                        dependent_target.relative_to(library_dir)
+                    except ValueError:
+                        parts = list(relative.parts)
                         while parts[0] == os.pardir:
-                            parts = parts[1:]
+                            parts.pop(0)
                         relative = Path(*parts)
-                    dependent_target = targetdir / relative
+                        dependent_target = library_dir / relative
                 dep_libs = str(relative.parent)
                 fix_rpath.add(dep_libs)
                 self._copy_file(
                     dependent_file, dependent_target, copy_dependent_files
                 )
             if fix_rpath:
                 has_rpath = self.patchelf.get_rpath(target)
                 rpath = ":".join(f"$ORIGIN/{r}" for r in fix_rpath)
                 if has_rpath != rpath:
                     self.patchelf.set_rpath(target, rpath)
 
+    def _post_freeze_hook(self):
+        target: Path
+        symlink: str
+        for target, symlink in self._symlinks:
+            if self.silent < 1:
+                print(f"linking {target} -> {symlink}")
+            if not target.exists():
+                target.symlink_to(symlink)
+
     def _copy_top_dependency(self, source: Path) -> None:
         """Called for copying certain top dependencies in _freeze_executable."""
         target = self.targetdir / "lib" / source.name
         self._copy_file(
             source, target, copy_dependent_files=True, include_mode=True
         )
```

### Comparing `cx_Freeze-6.8b5/cx_Freeze/cli.py` & `cx_Freeze-6.9/cx_Freeze/cli.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/winmsvcr.py` & `cx_Freeze-6.9/cx_Freeze/winmsvcr.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/openpyxl/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/openpyxl/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/openpyxl/test_openpyxl.py` & `cx_Freeze-6.9/cx_Freeze/samples/openpyxl/test_openpyxl.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pyzmq/pyzmq_server.py` & `cx_Freeze-6.9/cx_Freeze/samples/pyzmq/pyzmq_server.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pyzmq/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/pyzmq/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pyzmq/pyzmq_client.py` & `cx_Freeze-6.9/cx_Freeze/samples/pyzmq/pyzmq_client.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/Tkinter/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/Tkinter/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/ctypes/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/ctypes/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/plist_items/run.py` & `cx_Freeze-6.9/cx_Freeze/samples/plist_items/run.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/plist_items/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/plist_items/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/simple/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/simple/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/distutils/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/distutils/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/importlib/get_examples.py` & `cx_Freeze-6.9/cx_Freeze/samples/importlib/get_examples.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/importlib/web_srv.py` & `cx_Freeze-6.9/cx_Freeze/samples/importlib/web_srv.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/importlib/server_simple.py` & `cx_Freeze-6.9/cx_Freeze/samples/importlib/server_simple.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/importlib/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/importlib/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/asmodule/asmodule.py` & `cx_Freeze-6.9/cx_Freeze/samples/asmodule/asmodule.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/asmodule/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/asmodule/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/icon/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/icon/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/wx/wxapp.py` & `cx_Freeze-6.9/cx_Freeze/samples/wx/wxapp.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/wx/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/wx/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pycountry/setup_zip.py` & `cx_Freeze-6.9/cx_Freeze/samples/pycountry/setup_zip.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pyside2/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/pyside2/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pyside2/PySide2app.py` & `cx_Freeze-6.9/cx_Freeze/samples/pyside2/PySide2app.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/service/Config.py` & `cx_Freeze-6.9/cx_Freeze/samples/service/Config.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/service/ServiceHandler.py` & `cx_Freeze-6.9/cx_Freeze/samples/service/ServiceHandler.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/service/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/service/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/bcrypt/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/bcrypt/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/advanced/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/advanced/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pydantic/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/pydantic/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/sqlite/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/sqlite/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/sqlite/test_sqlite3.py` & `cx_Freeze-6.9/cx_Freeze/samples/sqlite/test_sqlite3.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/build_constants/hello.py` & `cx_Freeze-6.9/cx_Freeze/samples/build_constants/hello.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/build_constants/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/build_constants/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/dependencies/test_1.py` & `cx_Freeze-6.9/cx_Freeze/samples/dependencies/test_1.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/dependencies/getdependentfiles.py` & `cx_Freeze-6.9/cx_Freeze/samples/dependencies/getdependentfiles.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/find_spec/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/find_spec/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pillow/test_pillow.py` & `cx_Freeze-6.9/cx_Freeze/samples/pillow/test_pillow.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pillow/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/pillow/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/msi_binary_data/hello.py` & `cx_Freeze-6.9/cx_Freeze/samples/msi_binary_data/hello.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/msi_binary_data/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/msi_binary_data/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/zope/qotd.py` & `cx_Freeze-6.9/cx_Freeze/samples/zope/qotd.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/zope/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/zope/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/relimport/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/relimport/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pandas/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/pandas/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/tz/test_tz.py` & `cx_Freeze-6.9/cx_Freeze/samples/tz/test_tz.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/tz/setup_zip.py` & `cx_Freeze-6.9/cx_Freeze/samples/tz/setup_zip.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/tz/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/tz/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/msi_extensions/hello.py` & `cx_Freeze-6.9/cx_Freeze/samples/msi_extensions/hello.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/msi_extensions/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/msi_extensions/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pytz/setup_zip.py` & `cx_Freeze-6.9/cx_Freeze/samples/pytz/setup_zip.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pytz/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/pytz/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/cryptography/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/cryptography/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/matplotlib/matplotlib_afm.py` & `cx_Freeze-6.9/cx_Freeze/samples/matplotlib/matplotlib_afm.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/matplotlib/setup_zip.py` & `cx_Freeze-6.9/cx_Freeze/samples/matplotlib/setup_zip.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/matplotlib/matplotlib_eg.py` & `cx_Freeze-6.9/cx_Freeze/samples/matplotlib/matplotlib_eg.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/matplotlib/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/matplotlib/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pyqt5/PyQt5app.py` & `cx_Freeze-6.9/cx_Freeze/samples/pyqt5/PyQt5app.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pyqt5/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/pyqt5/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pythonnet-demo/DynamicGrid.py` & `cx_Freeze-6.9/cx_Freeze/samples/pythonnet-demo/DynamicGrid.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pythonnet-demo/helloform.py` & `cx_Freeze-6.9/cx_Freeze/samples/pythonnet-demo/helloform.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pythonnet-demo/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/pythonnet-demo/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pythonnet-demo/splitter.py` & `cx_Freeze-6.9/cx_Freeze/samples/pythonnet-demo/splitter.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/pythonnet-demo/wordpad.py` & `cx_Freeze-6.9/cx_Freeze/samples/pythonnet-demo/wordpad.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/msi_summary_data/hello.py` & `cx_Freeze-6.9/cx_Freeze/samples/msi_summary_data/hello.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/samples/msi_summary_data/setup.py` & `cx_Freeze-6.9/cx_Freeze/samples/msi_summary_data/setup.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/common.py` & `cx_Freeze-6.9/cx_Freeze/common.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/dist.py` & `cx_Freeze-6.9/cx_Freeze/dist.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/module.py` & `cx_Freeze-6.9/cx_Freeze/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,16 +67,14 @@
 
 
 class Module:
     """
     The Module class.
     """
 
-    _file: Optional[Path]
-
     def __init__(
         self,
         name: str,
         path: Optional[List[Union[Path, str]]] = None,
         file_name: Optional[Union[Path, str]] = None,
         parent: Optional["Module"] = None,
     ):
@@ -88,27 +86,28 @@
         self.parent: Optional["Module"] = parent
         self.code: Optional[CodeType] = None
         self.distribution: Optional[DistributionCache] = None
         self.exclude_names: Set[str] = set()
         self.global_names: Set[str] = set()
         self.ignore_names: Set[str] = set()
         self.in_import: bool = True
+        self.source_is_string: bool = False
         self.source_is_zip_file: bool = False
-        self._in_file_system: bool = True
+        self._in_file_system: int = 1
         # cache the dist-info files (metadata)
         self.update_distribution(name)
 
     @property
     def file(self) -> Optional[Path]:
         """Module filename"""
         return self._file
 
     @file.setter
     def file(self, file_name: Optional[Union[Path, str]]):
-        self._file = Path(file_name) if file_name else None
+        self._file: Optional[Path] = Path(file_name) if file_name else None
 
     def update_distribution(self, name: str) -> None:
         """Update the distribution cache based on its name.
         This method may be used to link an distribution's name to a module.
 
         Example: ModuleFinder cannot detects the distribution of _cffi_backend
         but in a hook we can link it to 'cffi'.
@@ -134,25 +133,27 @@
         if self.file is not None:
             parts.append(f"file={self.file!r}")
         if self.path is not None:
             parts.append(f"path={self.path!r}")
         return "<Module {}>".format(", ".join(parts))
 
     @property
-    def in_file_system(self) -> bool:
-        """Returns a boolean indicating if the module will be stored in the
-        file system or not."""
+    def in_file_system(self) -> int:
+        """Returns a value indicating where the module/package will be stored:
+        0. in a zip file (not directly in the file system)
+        1. in the file system, package with modules and data
+        2. in the file system, only detected modules."""
         if self.parent is not None:
             return self.parent.in_file_system
         if self.path is None or self.file is None:
-            return False
+            return 0
         return self._in_file_system
 
     @in_file_system.setter
-    def in_file_system(self, value) -> None:
+    def in_file_system(self, value: int) -> None:
         self._in_file_system = value
 
 
 class ConstantsModule:
     """
     Base ConstantsModule class.
     """
@@ -191,15 +192,15 @@
         """
         Create the module which consists of declaration statements for each
         of the values.
         """
         today = datetime.datetime.today()
         source_timestamp = 0
         for module in modules:
-            if module.file is None:
+            if module.file is None or module.source_is_string:
                 continue
             if module.source_is_zip_file:
                 continue
             if not module.file.exists():
                 raise ConfigError(
                     f"No file named {module.file!s} (for module {module.name})"
                 )
```

### Comparing `cx_Freeze-6.8b5/cx_Freeze/darwintools.py` & `cx_Freeze-6.9/cx_Freeze/darwintools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import os
 from pathlib import Path
+import platform
 import subprocess
+import shutil
 import stat
+import tempfile
 from typing import Dict, Iterable, List, Optional, Set, Union
 
 from .exception import DarwinException
 
 
 # In a MachO file, need to deal specially with links that use @executable_path,
 # @loader_path, @rpath
@@ -462,14 +465,37 @@
     os.chmod(fileName, newMode)
     subprocess.call(
         ("install_name_tool", "-change", oldReference, newReference, fileName)
     )
     os.chmod(fileName, original)
 
 
+def applyAdHocSignature(fileName: str):
+    if platform.machine() != "arm64":
+        return
+
+    args = (
+        "codesign",
+        "--sign",
+        "-",
+        "--force",
+        "--preserve-metadata=entitlements,requirements,flags,runtime",
+        fileName,
+    )
+    if subprocess.call(args):
+        # It may be a bug in Apple's codesign utility
+        # The workaround is to copy the file to another inode, then move it
+        # back erasing the previous file. The sign again.
+        with tempfile.TemporaryDirectory() as dirName:
+            tempName = os.path.join(dirName, os.path.basename(fileName))
+            shutil.copy(fileName, tempName)
+            shutil.move(tempName, fileName)
+        subprocess.call(args)
+
+
 class DarwinFileTracker:
     """Object to track the DarwinFiles that have been added during a freeze."""
 
     def __init__(self):
         # list of DarwinFile objects for files being copied into project
         self._copied_file_list: List[DarwinFile] = []
```

### Comparing `cx_Freeze-6.8b5/cx_Freeze/finder.py` & `cx_Freeze-6.9/cx_Freeze/finder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Base class for finding modules.
 """
 
-import dis
 from importlib.abc import ExecutionLoader
 import importlib.machinery
 import logging
 import os
 from pathlib import Path, PurePath
 import sys
 from types import CodeType
@@ -15,23 +14,26 @@
 
 from .common import code_object_replace, process_path_specs
 from .common import IncludesList, InternalIncludesList
 from .module import ConstantsModule, Module
 
 
 BUILD_LIST = opcode.opmap["BUILD_LIST"]
+EXTENDED_ARG = opcode.opmap["EXTENDED_ARG"]
 INPLACE_ADD = opcode.opmap["INPLACE_ADD"]
 LOAD_CONST = opcode.opmap["LOAD_CONST"]
 IMPORT_NAME = opcode.opmap["IMPORT_NAME"]
 IMPORT_FROM = opcode.opmap["IMPORT_FROM"]
 IMPORT_STAR = opcode.opmap["IMPORT_STAR"]
 STORE_FAST = opcode.opmap["STORE_FAST"]
 STORE_NAME = opcode.opmap["STORE_NAME"]
 STORE_GLOBAL = opcode.opmap["STORE_GLOBAL"]
 STORE_OPS = (STORE_NAME, STORE_GLOBAL)
+HAVE_ARGUMENT = opcode.HAVE_ARGUMENT
+
 
 DeferredList = List[Tuple[Module, Module, List[str]]]
 
 __all__ = ["Module", "ModuleFinder"]
 
 
 class ModuleFinder:
@@ -117,15 +119,15 @@
                 )
                 del self._bad_modules[name]
             if (
                 self.zip_include_all_packages
                 and module.name not in self.zip_exclude_packages
                 or module.name in self.zip_include_packages
             ):
-                module.in_file_system = False
+                module.in_file_system = 0
         if module.path is None and path is not None:
             module.path = [Path(p) for p in path]
         if module.file is None and file_name is not None:
             module.file = file_name
         return module
 
     def _determine_parent(self, caller: Optional[Module]) -> Optional[Module]:
@@ -354,73 +356,74 @@
         self,
         name: str,
         path: Union[str, List[str], List[Path]],
         deferred_imports: DeferredList,
         parent: Optional[Module] = None,
     ) -> Optional[Module]:
         """Load the module, searching the module spec."""
-        spec: Optional[importlib.machinery.ModuleSpec]
-        loader: ExecutionLoader
-        module: Module
+        spec: Optional[importlib.machinery.ModuleSpec] = None
+        loader: Optional[ExecutionLoader] = None
+        module: Optional[Module] = None
 
         if isinstance(path, str):
             # Include file as module
             module = self._add_module(name, file_name=path, parent=parent)
             ext = os.path.splitext(os.path.basename(path))[1]
             if ext in importlib.machinery.SOURCE_SUFFIXES + [""]:
                 loader = importlib.machinery.SourceFileLoader(name, path)
             elif ext in importlib.machinery.BYTECODE_SUFFIXES:
                 loader = importlib.machinery.SourcelessFileLoader(name, path)
             elif ext in importlib.machinery.EXTENSION_SUFFIXES:
                 loader = importlib.machinery.ExtensionFileLoader(name, path)
-            else:
-                loader = None
         else:
             # Find modules to load
             if path:
                 path = [str(p) for p in path]
             try:
                 # It's recommended to clear the caches first.
                 importlib.machinery.PathFinder.invalidate_caches()
                 spec = importlib.machinery.PathFinder.find_spec(name, path)
             except KeyError:
                 if parent:
                     # some packages use a directory with vendored modules
-                    # without an __init__py and are not considered namespace
+                    # without an __init__.py and are not considered namespace
                     # packages, then simulate a subpackage
-                    path = [os.path.join(path[0], name.rpartition(".")[-1])]
-                    origin = os.path.join(path[0], "__init__.py")
-                    module = self._add_module(name, path=path, parent=parent)
+                    module = self._add_module(
+                        name,
+                        path=[os.path.join(path[0], name.rpartition(".")[-1])],
+                        parent=parent,
+                    )
+                    module.source_is_string = True
                     logging.debug("Adding module [%s] [PACKAGE]", name)
-                    module.code = compile("", origin, "exec")
-                    module.in_import = False
-                    return module
-                spec = None
+                    path = os.path.join(path[0], "__init__.py")
             except Exception:
-                spec = None
-            if spec is None:
+                pass
+            if spec is None and module is None:
                 return None
+        if spec:
             # Handle special cases
             loader = spec.loader
             if loader is importlib.machinery.BuiltinImporter:
                 return None
             if loader is importlib.machinery.FrozenImporter:
                 return None
             # Load package or namespace package
             if spec.submodule_search_locations:
-                path_list = list(spec.submodule_search_locations)
-                module = self._add_module(name, path=path_list, parent=parent)
+                module = self._add_module(
+                    name,
+                    path=list(spec.submodule_search_locations),
+                    parent=parent,
+                )
                 if spec.origin in (None, "namespace"):
                     logging.debug("Adding module [%s] [NAMESPACE]", name)
-                    path = os.path.join(path_list[0], "__init__.py")
-                    module.code = compile("", path, "exec")
-                    module.in_import = False
-                    return module
-                logging.debug("Adding module [%s] [PACKAGE]", name)
-                path = spec.origin  # path of __init__
+                    path = str(module.path[0] / "__init__.py")
+                    module.source_is_string = True
+                else:
+                    logging.debug("Adding module [%s] [PACKAGE]", name)
+                    path = spec.origin  # path of __init__.py
                 module.file = path
             else:
                 path = spec.origin
                 module = self._add_module(name, file_name=path, parent=parent)
 
         if isinstance(loader, importlib.machinery.SourceFileLoader):
             logging.debug("Adding module [%s] [SOURCE]", name)
@@ -439,14 +442,16 @@
             logging.debug("Adding module [%s] [BYTECODE]", name)
             # Load Python bytecode
             module.code = loader.get_code(name)
             if module.code is None:
                 raise ImportError(f"Bad magic number in {path}", name=name)
         elif isinstance(loader, importlib.machinery.ExtensionFileLoader):
             logging.debug("Adding module [%s] [EXTENSION]", name)
+        elif module.source_is_string:
+            module.code = compile("", path, "exec")
         else:
             raise ImportError(f"Unknown module loader in {path}", name=name)
 
         # If there's a custom hook for this module, run it.
         self._run_hook("load", module.name, module)
 
         if module.code is not None:
@@ -468,15 +473,15 @@
         when the module is in a package and will be stored in library.zip.
         """
         code = module.code
         # Check if module is in a package and will be stored in library.zip
         # and is not defined in the module, like 'six' do
         if (
             module.parent is None
-            or module.in_file_system
+            or module.in_file_system >= 1
             or "__package__" in module.global_names
             or code is None
         ):
             return code
         # Only if the code references it.
         if "__package__" in code.co_names:
             consts = list(code.co_consts)
@@ -561,15 +566,24 @@
         """
         Scan code, looking for imported modules and keeping track of the
         constants that have been created in order to better tell which
         modules are truly missing.
         """
         arguments = []
         imported_module = None
-        for _index, op, arg in dis._unpack_opargs(code.co_code):
+        co_code = code.co_code
+        extended_arg = 0
+        for i in range(0, len(co_code), 2):
+            op = co_code[i]
+            if op >= HAVE_ARGUMENT:
+                arg = co_code[i + 1] | extended_arg
+                extended_arg = (arg << 8) if op == EXTENDED_ARG else 0
+            else:
+                arg = None
+                extended_arg = 0
 
             # keep track of constants (these are used for importing)
             # immediately restart loop so arguments are retained
             if op == LOAD_CONST:
                 arguments.append(code.co_consts[arg])
                 continue
 
@@ -682,17 +696,16 @@
         # include module
         deferred_imports: DeferredList = []
         module = self._import_module(name, deferred_imports)
         self._import_deferred_imports(deferred_imports, skip_in_import=True)
         return module
 
     def IncludePackage(self, name: str) -> Module:
-        """
-        Include the named package and any submodules in the frozen executable.
-        """
+        """Include the named package and any submodules in the frozen
+        executable."""
         deferred_imports: DeferredList = []
         module = self._import_module(name, deferred_imports)
         if module.path:
             self._import_all_sub_modules(module, deferred_imports)
         self._import_deferred_imports(deferred_imports, skip_in_import=True)
         return module
 
@@ -702,18 +715,16 @@
             print("Missing modules:")
             names = list(self._bad_modules.keys())
             names.sort()
             for name in names:
                 callers = list(self._bad_modules[name].keys())
                 callers.sort()
                 print("? {} imported from {}".format(name, ", ".join(callers)))
-            print(
-                "This is not necessarily a problem - the modules "
-                "may not be needed on this platform.\n"
-            )
+            print("This is not necessarily a problem - the modules ", end="")
+            print("may not be needed on this platform.\n")
 
     def SetOptimizeFlag(self, optimize_flag: int) -> int:
         """Set a new value of optimize flag and returns the previous value."""
         previous = self.optimize_flag
         # The value of optimize_flag is propagated according to the user's
         # choice and checked in dist.py or main,py. This value is unlikely
         # to be wrong, yet we check and ignore any divergent value.
```

### Comparing `cx_Freeze-6.8b5/cx_Freeze/setupwriter.py` & `cx_Freeze-6.9/cx_Freeze/setupwriter.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/initscripts/ConsoleSetLibPath.py` & `cx_Freeze-6.9/cx_Freeze/initscripts/ConsoleSetLibPath.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/initscripts/__startup__.py` & `cx_Freeze-6.9/cx_Freeze/initscripts/__startup__.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/initscripts/SharedLibSource.py` & `cx_Freeze-6.9/cx_Freeze/initscripts/SharedLibSource.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/__init__.py` & `cx_Freeze-6.9/cx_Freeze/__init__.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/executable.py` & `cx_Freeze-6.9/cx_Freeze/executable.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/winversioninfo.py` & `cx_Freeze-6.9/cx_Freeze/winversioninfo.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/cx_Freeze/patchelf.py` & `cx_Freeze-6.9/cx_Freeze/patchelf.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             if dependent_file == path.name:
                 continue
             if dependent_file in ("not found", "(file not found)"):
                 filename = parts[0]
                 if filename not in linker_warnings:
                     linker_warnings[filename] = None
                     if show_warnings:
-                        print(f"WARNING: cannot find {filename!r}")
+                        print(f"WARNING: cannot find '{filename}'")
                 continue
             if dependent_file.startswith("("):
                 continue
             pos = dependent_file.find(" (")
             if pos >= 0:
                 dependent_file = dependent_file[:pos].strip()
             if dependent_file:
```

### Comparing `cx_Freeze-6.8b5/cx_Freeze/macdist.py` & `cx_Freeze-6.9/cx_Freeze/macdist.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import warnings
 
 from typing import List, Tuple
 
 from cx_Freeze.common import normalize_to_list
 
 from cx_Freeze.darwintools import (
+    applyAdHocSignature,
     changeLoadReference,
     DarwinFile,
     DarwinFileTracker,
 )
 
 __all__ = ["bdist_dmg", "bdist_mac"]
 
@@ -82,15 +83,15 @@
         if self.applications_shortcut:
             apps_folder_link = os.path.join(self.dist_dir, "Applications")
             os.symlink(
                 "/Applications", apps_folder_link, target_is_directory=True
             )
 
         # Create the dmg
-        if subprocess.call(("hdiutil", createargs)) != 0:
+        if subprocess.call(createargs) != 0:
             raise OSError("creation of the dmg failed")
 
     def run(self):
         # Create the application bundle
         self.run_command("bdist_mac")
 
         # Find the location of the application bundle and the build dir
@@ -285,14 +286,15 @@
                                 "install_name_tool",
                                 "-change",
                                 lib,
                                 replacement,
                                 filename,
                             )
                         )
+            applyAdHocSignature(filename)
 
     def setRelativeReferencePaths(self, buildDir: str, binDir: str):
         """
         Make all the references from included Mach-O files to other included
         Mach-O files relative.
         """
         darwinFile: DarwinFile
@@ -331,14 +333,16 @@
                 changeLoadReference(
                     filePathInBinDir,
                     oldReference=rawPath,
                     newReference=exePath,
                     VERBOSE=False,
                 )
 
+            applyAdHocSignature(filePathInBinDir)
+
     def find_qt_menu_nib(self):
         """
         Returns a location of a qt_menu.nib folder, or None if this is not
         a Qt application.
         """
         if self.qt_menu_nib:
             return self.qt_menu_nib
@@ -479,9 +483,9 @@
             if self.codesign_resource_rules:
                 signargs.insert(
                     1, "--resource-rules=" + self.codesign_resource_rules
                 )
 
             signargs.append(self.bundleDir)
 
-            if subprocess.call(("codesign", signargs)) != 0:
+            if subprocess.call(signargs) != 0:
                 raise OSError("Code signing of app bundle failed")
```

### Comparing `cx_Freeze-6.8b5/cx_Freeze/hooks.py` & `cx_Freeze-6.9/cx_Freeze/hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
     """The asyncio must be loaded as a package."""
     finder.IncludePackage("asyncio")
 
 
 def load_babel(finder: ModuleFinder, module: Module) -> None:
     """The babel must be loaded as a package, and has pickeable data."""
     finder.IncludePackage("babel")
-    module.in_file_system = True
+    module.in_file_system = 1
 
 
 def load_bcrypt(finder: ModuleFinder, module: Module) -> None:
     """The bcrypt package requires the _cffi_backend module (loaded implicitly)"""
     finder.IncludeModule("_cffi_backend")
 
 
@@ -248,17 +248,17 @@
 
 def load_certifi(finder: ModuleFinder, module: Module) -> None:
     """
     The certifi package, in python 3.7 and up, uses importlib.resources
     to locate the cacert.pem in zip packages.
     In previous versions, it is expected to be stored in the file system.
     """
-    if not module.in_file_system:
+    if module.in_file_system == 0:
         if sys.version_info < (3, 7):
-            module.in_file_system = True
+            module.in_file_system = 1
             return
         cacert = Path(__import__("certifi").where())
         finder.ZipIncludeFiles(cacert, Path("certifi", cacert.name))
 
 
 def load__cffi_backend(finder: ModuleFinder, module: Module) -> None:
     """Add the cffi metadata for _cffi_backend module."""
@@ -301,45 +301,45 @@
 ) -> None:
     """The cryptography module requires the _cffi_backend module."""
     finder.IncludeModule("_cffi_backend")
 
 
 def load_Crypto_Cipher(finder: ModuleFinder, module: Module) -> None:
     """The Crypto.Cipher subpackage of pycryptodome package."""
-    if not module.in_file_system:
+    if module.in_file_system == 0:
         finder.IncludePackage(module.name)
 
 
 def load_Crypto_Hash(finder: ModuleFinder, module: Module) -> None:
     """The Crypto.Hash subpackage of pycryptodome package."""
-    if not module.in_file_system:
+    if module.in_file_system == 0:
         finder.IncludePackage(module.name)
 
 
 def load_Crypto_Math(finder: ModuleFinder, module: Module) -> None:
     """The Crypto.Math subpackage of pycryptodome package."""
-    if not module.in_file_system:
+    if module.in_file_system == 0:
         finder.IncludePackage(module.name)
 
 
 def load_Crypto_Protocol(finder: ModuleFinder, module: Module) -> None:
     """The Crypto.Protocol subpackage of pycryptodome package."""
-    if not module.in_file_system:
+    if module.in_file_system == 0:
         finder.IncludePackage(module.name)
 
 
 def load_Crypto_PublicKey(finder: ModuleFinder, module: Module) -> None:
     """The Crypto.PublicKey subpackage of pycryptodome package."""
-    if not module.in_file_system:
+    if module.in_file_system == 0:
         finder.IncludePackage(module.name)
 
 
 def load_Crypto_Util(finder: ModuleFinder, module: Module) -> None:
     """The Crypto.Util subpackage of pycryptodome package."""
-    if not module.in_file_system:
+    if module.in_file_system == 0:
         finder.IncludePackage(module.name)
 
 
 def load_Crypto_Util__file_system(
     finder: ModuleFinder, module: Module
 ) -> None:
     """The pycryptodome package"""
@@ -351,36 +351,54 @@
     import sys
     if dir_comps[0] != "Crypto":
         raise ValueError("Only available for modules under 'Crypto'")
     dir_comps = list(dir_comps) + [filename]
     root_lib = os.path.join(os.path.dirname(sys.executable), "lib")
     return os.path.join(root_lib, ".".join(dir_comps))
 """
-    if not module.in_file_system and module.code is not None:
+    if module.in_file_system == 0 and module.code is not None:
         new_code = compile(PYCRYPTODOME_CODE_STR, str(module.file), "exec")
         co_func = new_code.co_consts[2]
         name = co_func.co_name
         code = module.code
         consts = list(code.co_consts)
-        for i in enumerate(consts):
-            if isinstance(consts[i], type(code)) and consts[i].co_name == name:
+        for i, c in enumerate(consts):
+            if isinstance(c, type(code)) and c.co_name == name:
                 consts[i] = co_func
                 break
         module.code = code_object_replace(code, co_consts=consts)
 
 
 def load__ctypes(finder: ModuleFinder, module: Module) -> None:
     """
-    In Windows, the _ctypes module in Python 3.8+ requires an additional dll
-    libffi-7.dll to be present in the build directory.
+    In Windows, the _ctypes module in Python 3.8+ requires an additional
+    libffi dll to be present in the build directory.
     """
     if WIN32 and sys.version_info >= (3, 8) and not MINGW:
-        dll_name = "libffi-7.dll"
-        dll_path = Path(sys.base_prefix, "DLLs", dll_name)
-        finder.IncludeFiles(dll_path, Path("lib", dll_name))
+        dll_pattern = "libffi-*.dll"
+        dll_dir = Path(sys.base_prefix, "DLLs")
+        for dll_path in dll_dir.glob(dll_pattern):
+            finder.IncludeFiles(dll_path, Path("lib", dll_path.name))
+
+
+def load_cv2(finder: ModuleFinder, module: Module) -> None:
+    """
+    Versions of cv2 (opencv-python) above 4.5.3 require additional
+    configuration files.
+
+    Additionally, on Linux the opencv_python.libs directory is not
+    copied across for versions above 4.5.3 unless the cv2 package is
+    included.
+    """
+    finder.IncludePackage("cv2")
+
+    dest_dir = Path("lib", "cv2")
+    cv2_dir = module.path[0]
+    for path in cv2_dir.glob("config*.py"):
+        finder.IncludeFiles(path, dest_dir / path.name)
 
 
 def load_cx_Oracle(finder: ModuleFinder, module: Module) -> None:
     """
     The cx_Oracle module implicitly imports datetime; make sure this
     happens.
     """
@@ -405,14 +423,19 @@
     """
     The dummy_threading module plays games with the name of the threading
     module for its own purposes; ignore that here.
     """
     finder.ExcludeModule("_dummy_threading")
 
 
+def load_flask_compress(finder: ModuleFinder, module: Module) -> None:
+    """flask-compress requires its metadata."""
+    module.update_distribution("Flask_Compress")
+
+
 def load_ftplib(finder: ModuleFinder, module: Module) -> None:
     """
     The ftplib module attempts to import the SOCKS module; ignore this
     module if it cannot be found.
     """
     module.ignore_names.add("SOCKS")
 
@@ -514,15 +537,15 @@
 
 def load_googleapiclient_discovery(
     finder: ModuleFinder, module: Module
 ) -> None:
     """The googleapiclient.discovery module needs discovery_cache subpackage
     in file system."""
     discovery_cache = finder.IncludePackage("googleapiclient.discovery_cache")
-    discovery_cache.in_file_system = True
+    discovery_cache.in_file_system = 1
 
 
 def load_google_cloud_storage(finder: ModuleFinder, module: Module) -> None:
     """The google.cloud.storage package always uses the parent module."""
     finder.IncludePackage("google.cloud")
 
 
@@ -588,15 +611,15 @@
     data_path = module.path[0] / "mpl-data"
     target_path = Path("lib", module.name, "mpl-data")
     # After matplotlib 3.4 mpl-data is guaranteed to be a subdirectory.
     if not data_path.is_dir():
         data_path = __import__("matplotlib").get_data_path()
         need_patch = True
     else:
-        need_patch = not module.in_file_system
+        need_patch = module.in_file_system == 0
     finder.IncludeFiles(data_path, target_path, copy_dependent_files=False)
     finder.IncludePackage("matplotlib")
     finder.ExcludeModule("matplotlib.tests")
     finder.ExcludeModule("matplotlib.testing")
     if not need_patch or module.code is None:
         return
     CODE_STR = f"""
@@ -605,16 +628,16 @@
 """
     for code_str in [CODE_STR, CODE_STR.replace("_get_data_", "get_data_")]:
         new_code = compile(code_str, str(module.file), "exec")
         co_func = new_code.co_consts[0]
         name = co_func.co_name
         code = module.code
         consts = list(code.co_consts)
-        for i in enumerate(consts):
-            if isinstance(consts[i], type(code)) and consts[i].co_name == name:
+        for i, c in enumerate(consts):
+            if isinstance(c, type(code)) and c.co_name == name:
                 consts[i] = co_func
                 break
         module.code = code_object_replace(code, co_consts=consts)
 
 
 def load_numpy(finder: ModuleFinder, module: Module) -> None:
     """The numpy must be loaded as a package; support for pypi version and
@@ -640,15 +663,15 @@
 
             # do not check dependencies already handled
             extension = EXTENSION_SUFFIXES[0]
             for path in numpy_dir.rglob(f"*{extension}"):
                 finder.ExcludeDependentFiles(path)
 
         # support for old versions (numpy <= 1.18.2)
-        if not module.in_file_system:
+        if module.in_file_system == 0:
             # copy any file at site-packages/numpy/.libs
             libs_dir = numpy_dir / ".libs"
             if libs_dir.is_dir():
                 finder.IncludeFiles(libs_dir, "lib")
 
     # exclude the tests
     finder.ExcludeModule("numpy.compat.tests")
@@ -800,20 +823,17 @@
 
 def load_ptr(finder: ModuleFinder, module: Module) -> None:
     """pytest-runner requires its metadata"""
     module.update_distribution("pytest-runner")
 
 
 def load_pycountry(finder: ModuleFinder, module: Module) -> None:
-    """
-    The pycountry module has data in subdirectories.
-    """
+    """The pycountry module has data in subdirectories."""
     finder.ExcludeModule("pycountry.tests")
-    if not module.in_file_system:
-        module.in_file_system = True
+    module.in_file_system = 1
 
 
 def load_pycparser(finder: ModuleFinder, module: Module) -> None:
     """
     These files are missing which causes
     permission denied issues on windows when they are regenerated.
     """
@@ -900,15 +920,17 @@
     include_files = []
     for library_dir in _qt_library_paths(name):
         if library_dir.parts[-1] != "plugins":
             continue
         source_path = library_dir / plugins
         if not source_path.exists():
             continue
-        if source_path.parts[-4] == name:
+        if source_path.parts[-3] == name:  # {name}/plugins/{plugins}
+            target_path = Path("lib").joinpath(*source_path.parts[-3:])
+        elif source_path.parts[-4] == name:  # {name}/Qt*/plugins/{plugins}
             target_path = Path("lib").joinpath(*source_path.parts[-4:])
         else:
             # fallback plugins path to be used by load_PyQt5.
             target_path = Path("lib") / name / "Qt" / "plugins" / plugins
         include_files.append((source_path, target_path))
     return include_files
 
@@ -944,14 +966,16 @@
 library_paths = [os.path.normcase(p) for p in QCoreApplication.libraryPaths()]
 if os.path.normcase(plugins_dir) not in library_paths:
     library_paths = QCoreApplication.libraryPaths() + [plugins_dir]
     QCoreApplication.setLibraryPaths(library_paths)
 # cx_Freeze patch end
 """
     module.code = compile(code_string, str(module.file), "exec")
+    if module.in_file_system == 0:
+        module.in_file_system = 2  # use optimized mode
 
 
 def load_PyQt5_phonon(finder: ModuleFinder, module: Module) -> None:
     """In Windows, phonon5.dll requires an additional dll phonon_ds94.dll to
     be present in the build directory inside a folder phonon_backend."""
     if WIN32:
         name = _qt_implementation(module)
@@ -1106,15 +1130,15 @@
             getattr(pytz, "_tzinfo_dir", None)
             or os.getenv("PYTZ_TZDATADIR")
             or "/usr/share/zoneinfo"
         )
         if data_path.is_dir():
             finder.AddConstant("PYTZ_TZDATADIR", str(target_path))
     if data_path.is_dir():
-        if module.in_file_system:
+        if module.in_file_system >= 1:
             finder.IncludeFiles(
                 data_path, target_path, copy_dependent_files=False
             )
         else:
             finder.ZipIncludeFiles(data_path, Path("pytz", "zoneinfo"))
 
 
@@ -1137,14 +1161,28 @@
     """
     The reportlab module loads a submodule rl_settings via exec so force
     its inclusion here.
     """
     finder.IncludeModule("reportlab.rl_settings")
 
 
+def load_sentry(finder: ModuleFinder, module: Module) -> None:
+    """
+    The Sentry.io SDK
+    """
+    finder.IncludeModule("sentry_sdk.integrations.stdlib")
+    finder.IncludeModule("sentry_sdk.integrations.excepthook")
+    finder.IncludeModule("sentry_sdk.integrations.dedupe")
+    finder.IncludeModule("sentry_sdk.integrations.atexit")
+    finder.IncludeModule("sentry_sdk.integrations.modules")
+    finder.IncludeModule("sentry_sdk.integrations.argv")
+    finder.IncludeModule("sentry_sdk.integrations.logging")
+    finder.IncludeModule("sentry_sdk.integrations.threading")
+
+
 def load_scipy(finder: ModuleFinder, module: Module) -> None:
     """
     The scipy module loads items within itself in a way that causes
     problems without the entire package and a number of other subpackages
     being present.
     """
     finder.IncludePackage("scipy._lib")
@@ -1501,15 +1539,15 @@
             finder.IncludeFiles(source, target, copy_dependent_files=False)
             finder.AddConstant("PYTHONTZPATH", str(source))
     if tzdata is None:
         return
     # when the tzdata exists, copy other files in this directory
     source = tzdata.path[0]
     target = Path("lib", "tzdata")
-    if tzdata.in_file_system:
+    if tzdata.in_file_system >= 1:
         finder.IncludeFiles(source, target, copy_dependent_files=False)
     else:
         finder.ZipIncludeFiles(source, "tzdata")
 
 
 load_backports_zoneinfo = load_zoneinfo
```

### Comparing `cx_Freeze-6.8b5/cx_Freeze/windist.py` & `cx_Freeze-6.9/cx_Freeze/windist.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import distutils.command.bdist_msi
-import distutils.errors
+from distutils import log
 import importlib
 import msilib
 import os
 import re
+import shutil
 import sysconfig
 
 __all__ = ["bdist_msi"]
 
 # force the remove existing products action to happen first since Windows
 # installer appears to be braindead and doesn't handle files shared between
 # different "products" very well
@@ -70,39 +71,51 @@
         if self.directories:
             msilib.add_data(self.db, "Directory", self.directories)
         if self.environment_variables:
             msilib.add_data(self.db, "Environment", self.environment_variables)
         # This is needed in case the AlwaysInstallElevated policy is set.
         # Otherwise installation will not end up in TARGETDIR.
         msilib.add_data(
-            self.db, "Property", [("SecureCustomProperties", "TARGETDIR")]
+            self.db,
+            "Property",
+            [("SecureCustomProperties", "TARGETDIR;REINSTALLMODE")],
         )
         msilib.add_data(
             self.db,
             "CustomAction",
             [
                 (
                     "A_SET_TARGET_DIR",
                     256 + 51,
                     "TARGETDIR",
                     self.initial_target_dir,
-                )
+                ),
+                (
+                    "A_SET_REINSTALL_MODE",
+                    256 + 51,
+                    "REINSTALLMODE",
+                    "amus",
+                ),
             ],
         )
         msilib.add_data(
             self.db,
             "InstallExecuteSequence",
-            [("A_SET_TARGET_DIR", 'TARGETDIR=""', 401)],
+            [
+                ("A_SET_TARGET_DIR", 'TARGETDIR=""', 401),
+                ("A_SET_REINSTALL_MODE", 'REINSTALLMODE=""', 402),
+            ],
         )
         msilib.add_data(
             self.db,
             "InstallUISequence",
             [
                 ("PrepareDlg", None, 140),
                 ("A_SET_TARGET_DIR", 'TARGETDIR=""', 401),
+                ("A_SET_REINSTALL_MODE", 'REINSTALLMODE=""', 402),
                 ("SelectDirectoryDlg", "not Installed", 1230),
                 (
                     "MaintenanceTypeDlg",
                     "Installed and not Resume and not Preselected",
                     1250,
                 ),
                 ("ProgressDlg", None, 1280),
@@ -778,26 +791,26 @@
         if line not in rows:
             rows.append(line)
 
     def finalize_options(self):
         distutils.command.bdist_msi.bdist_msi.finalize_options(self)
         name = self.distribution.get_name()
         fullname = self.distribution.get_fullname()
+        platform = sysconfig.get_platform().replace("win-amd64", "win64")
         if self.initial_target_dir is None:
-            if sysconfig.get_platform() == "win-amd64":
+            if platform == "win64" or platform.startswith("mingw_x86_64"):
                 program_files_folder = "ProgramFiles64Folder"
             else:
                 program_files_folder = "ProgramFilesFolder"
             self.initial_target_dir = fr"[{program_files_folder}]\{name}"
         if self.add_to_path is None:
             self.add_to_path = False
         if self.target_name is None:
             self.target_name = fullname
         if not self.target_name.lower().endswith(".msi"):
-            platform = sysconfig.get_platform().replace("win-", "")
             self.target_name = f"{self.target_name}-{platform}.msi"
         if not os.path.isabs(self.target_name):
             self.target_name = os.path.join(self.dist_dir, self.target_name)
         if self.directories is None:
             self.directories = []
         if self.environment_variables is None:
             self.environment_variables = []
@@ -849,36 +862,19 @@
                 None,
                 None,
                 self.distribution.get_description(),
                 None,
                 None,
             )
             self._append_to_data(
-                "Extension",
-                ext,
-                component,
-                progid,
-                mime,
-                "default",
-            )
-            self._append_to_data(
-                "Verb",
-                ext,
-                verb,
-                0,
-                context,
-                argument,
+                "Extension", ext, component, progid, mime, "default"
             )
+            self._append_to_data("Verb", ext, verb, 0, context, argument)
             if mime is not None:
-                self._append_to_data(
-                    "MIME",
-                    mime,
-                    ext,
-                    "None",
-                )
+                self._append_to_data("MIME", mime, ext, "None")
             # Registry entries that allow proper display of the app in menu
             self._append_to_data(
                 "Registry",
                 f"{progid}-name",
                 -1,
                 fr"Software\Classes\{progid}",
                 "FriendlyAppName",
@@ -919,18 +915,19 @@
         self.all_users = False
         self.extensions = None
 
     def run(self):
         if not self.skip_build:
             self.run_command("build")
         install = self.reinitialize_command("install", reinit_subcommands=1)
-        install.prefix = self.bdist_dir
+        bdist_dir = self.bdist_dir
+        install.prefix = bdist_dir
         install.skip_build = self.skip_build
         install.warn_dir = 0
-        distutils.log.info("installing to %s", self.bdist_dir)
+        log.info(f"installing to {bdist_dir}")
         install.ensure_finalized()
         install.run()
         self.mkpath(self.dist_dir)
         fullname = self.distribution.get_fullname()
         if os.path.exists(self.target_name):
             os.unlink(self.target_name)
         metadata = self.distribution.metadata
@@ -967,17 +964,20 @@
         self.add_files()
         self.db.Commit()
         self.distribution.dist_files.append(
             ("bdist_msi", sversion or "any", self.target_name)
         )
 
         if not self.keep_temp:
-            distutils.dir_util.remove_tree(
-                self.bdist_dir, dry_run=self.dry_run
-            )
+            log.info(f"removing '{bdist_dir}' (and everything under it)")
+            if not self.dry_run:
+                try:
+                    shutil.rmtree(bdist_dir)
+                except OSError as exc:
+                    log.warn(f"error removing {bdist_dir}: {exc}")
 
         # Cause the MSI file to be released. Without this, then if bdist_msi
         # is run programmatically from within a larger script, subsequent
         # editting of the MSI is blocked.
         self.db = None
```

### Comparing `cx_Freeze-6.8b5/PKG-INFO` & `cx_Freeze-6.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cx_Freeze
-Version: 6.8b5
+Version: 6.9
 Summary: Create standalone executables from Python scripts
 Home-page: https://marcelotduarte.github.io/cx_Freeze
 Author: Anthony Tuininga
 Author-email: anthony.tuininga@gmail.com
 Maintainer: Marcelo Duarte @marcelotduarte
 License: Python Software Foundation License
 Project-URL: Bug Tracker, https://github.com/marcelotduarte/cx_Freeze/issues
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -43,24 +44,24 @@
 [![LGTM](https://img.shields.io/lgtm/grade/python/g/marcelotduarte/cx_Freeze.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/marcelotduarte/cx_Freeze)
 
 
 **cx\_Freeze** creates standalone executables from Python scripts, with the same
 performance, is cross-platform and should work on any platform that Python
 itself works on.
 
-# Highlights of Version 6.2 up to 6.7:
+# Highlights of Version 6.2 up to 6.9:
+- Support for pathlib.Path
+- New or improved hooks, with emphasis on matplotlib, numpy, PyQt5 and PySide2
 - New ModuleFinder engine uses importlib.machinery
 - Refactored Freezer
 - New support for package metadata improving Module and new DitributionCache
-- Enhanced support for Python 3.8 and good support for Python 3.9
-- Inclusive support for MSYS2 and Anaconda
+- Enhanced support for Python 3.8 and Python 3.9, including MSYS2 and Anaconda distributions
 - Improvements for multiprocessing
 - Optimizations in detection and distribution of libraries
 - Integrated to setuptools and importlib-metadata
-- New or improved hooks
 - Code modernization
 - Various bug fixes.
 
 # Installation
 
 In a virtual environment, install by issuing the command:
```

### Comparing `cx_Freeze-6.8b5/setup.py` & `cx_Freeze-6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,16 @@
                 extra_args.extend(get_config_var("BASEMODLIBS").split())
             if get_config_var("LOCALMODLIBS"):
                 extra_args.extend(get_config_var("LOCALMODLIBS").split())
             if DARWIN:
                 # macOS on Github Actions
                 extra_args.append("-Wl,-export_dynamic")
             else:
-                extra_args.append("-s")
+                if not self.debug:
+                    extra_args.append("-s")
                 extra_args.append("-Wl,-rpath,$ORIGIN/lib")
                 extra_args.append("-Wl,-rpath,$ORIGIN/../lib")
         self.compiler.link_executable(
             objects,
             fullname,
             libraries=libraries,
             library_dirs=library_dirs,
```

### Comparing `cx_Freeze-6.8b5/cx_Freeze.egg-info/SOURCES.txt` & `cx_Freeze-6.9/cx_Freeze.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -146,11 +146,8 @@
 source/bases/Common.c
 source/bases/Console.c
 source/bases/Win32GUI.c
 source/bases/Win32Service.c
 source/bases/cx_Logging.h
 source/bases/dummy.rc
 source/bases/manifest.rc
-source/bases/manifest.txt
-test/test_finder.py
-test/test_misc.py
-test/test_zip_packages.py
+source/bases/manifest.txt
```

### Comparing `cx_Freeze-6.8b5/cx_Freeze.egg-info/PKG-INFO` & `cx_Freeze-6.9/cx_Freeze.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cx-Freeze
-Version: 6.8b5
+Version: 6.9
 Summary: Create standalone executables from Python scripts
 Home-page: https://marcelotduarte.github.io/cx_Freeze
 Author: Anthony Tuininga
 Author-email: anthony.tuininga@gmail.com
 Maintainer: Marcelo Duarte @marcelotduarte
 License: Python Software Foundation License
 Project-URL: Bug Tracker, https://github.com/marcelotduarte/cx_Freeze/issues
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Software Distribution
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -43,24 +44,24 @@
 [![LGTM](https://img.shields.io/lgtm/grade/python/g/marcelotduarte/cx_Freeze.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/marcelotduarte/cx_Freeze)
 
 
 **cx\_Freeze** creates standalone executables from Python scripts, with the same
 performance, is cross-platform and should work on any platform that Python
 itself works on.
 
-# Highlights of Version 6.2 up to 6.7:
+# Highlights of Version 6.2 up to 6.9:
+- Support for pathlib.Path
+- New or improved hooks, with emphasis on matplotlib, numpy, PyQt5 and PySide2
 - New ModuleFinder engine uses importlib.machinery
 - Refactored Freezer
 - New support for package metadata improving Module and new DitributionCache
-- Enhanced support for Python 3.8 and good support for Python 3.9
-- Inclusive support for MSYS2 and Anaconda
+- Enhanced support for Python 3.8 and Python 3.9, including MSYS2 and Anaconda distributions
 - Improvements for multiprocessing
 - Optimizations in detection and distribution of libraries
 - Integrated to setuptools and importlib-metadata
-- New or improved hooks
 - Code modernization
 - Various bug fixes.
 
 # Installation
 
 In a virtual environment, install by issuing the command:
```

### Comparing `cx_Freeze-6.8b5/source/bases/Win32Service.c` & `cx_Freeze-6.9/source/bases/Win32Service.c`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/source/bases/manifest.txt` & `cx_Freeze-6.9/source/bases/manifest.txt`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/source/bases/Common.c` & `cx_Freeze-6.9/source/bases/Common.c`

 * *Files 7% similar despite different names*

```diff
@@ -155,37 +155,40 @@
 
 //-----------------------------------------------------------------------------
 // ExecuteScript()
 //   Execute the script found within the file.
 //-----------------------------------------------------------------------------
 static int ExecuteScript(void)
 {
-    PyObject *module, *function_init, *result_init, *function_run, *result_run;
+    PyObject *module, *func = NULL, *result = NULL;
 
     module = PyImport_ImportModule("__startup__");
     if (!module)
         return FatalScriptError();
 
-    function_init = PyObject_GetAttrString(module, "init");
-    if (!function_init)
+    func = PyObject_GetAttrString(module, "init");
+    if (!func) {
+        Py_DECREF(module);
         return FatalScriptError();
+    }
 
-    result_init = PyObject_CallObject(function_init, NULL);
-    if (!result_init)
+    result = PyObject_CallObject(func, NULL);
+    Py_DECREF(func);
+    if (!result) {
+        Py_DECREF(module);
         return FatalScriptError();
+    }
+    Py_DECREF(result);
 
-    function_run = PyObject_GetAttrString(module, "run");
-    if (!function_run)
+    func = PyObject_GetAttrString(module, "run");
+    Py_DECREF(module);
+    if (!func)
         return FatalScriptError();
 
-    result_run = PyObject_CallObject(function_run, NULL);
-    if (!result_run)
+    result = PyObject_CallObject(func, NULL);
+    Py_DECREF(func);
+    if (!result)
         return FatalScriptError();
-
-    Py_DECREF(result_run);
-    Py_DECREF(function_run);
-    Py_DECREF(result_init);
-    Py_DECREF(function_init);
-    Py_DECREF(module);
+    Py_DECREF(result);
 
     return 0;
 }
```

### Comparing `cx_Freeze-6.8b5/source/bases/Console.c` & `cx_Freeze-6.9/source/bases/Console.c`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/source/bases/Win32GUI.c` & `cx_Freeze-6.9/source/bases/Win32GUI.c`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/source/bases/cx_Logging.h` & `cx_Freeze-6.9/source/bases/cx_Logging.h`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/source/util.c` & `cx_Freeze-6.9/source/util.c`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/README.md` & `cx_Freeze-6.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 [![LGTM](https://img.shields.io/lgtm/grade/python/g/marcelotduarte/cx_Freeze.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/marcelotduarte/cx_Freeze)
 
 
 **cx\_Freeze** creates standalone executables from Python scripts, with the same
 performance, is cross-platform and should work on any platform that Python
 itself works on.
 
-# Highlights of Version 6.2 up to 6.7:
+# Highlights of Version 6.2 up to 6.9:
+- Support for pathlib.Path
+- New or improved hooks, with emphasis on matplotlib, numpy, PyQt5 and PySide2
 - New ModuleFinder engine uses importlib.machinery
 - Refactored Freezer
 - New support for package metadata improving Module and new DitributionCache
-- Enhanced support for Python 3.8 and good support for Python 3.9
-- Inclusive support for MSYS2 and Anaconda
+- Enhanced support for Python 3.8 and Python 3.9, including MSYS2 and Anaconda distributions
 - Improvements for multiprocessing
 - Optimizations in detection and distribution of libraries
 - Integrated to setuptools and importlib-metadata
-- New or improved hooks
 - Code modernization
 - Various bug fixes.
 
 # Installation
 
 In a virtual environment, install by issuing the command:
```

### Comparing `cx_Freeze-6.8b5/doc/src/conf.py` & `cx_Freeze-6.9/doc/src/conf.py`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/doc/src/script.rst` & `cx_Freeze-6.9/doc/src/script.rst`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/doc/src/license.rst` & `cx_Freeze-6.9/doc/src/license.rst`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/doc/src/releasenotes.rst` & `cx_Freeze-6.9/doc/src/releasenotes.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,157 @@
 Release notes
 =============
 
 6.x releases
 ############
 
+Version 6.9 (December 2021)
+---------------------------
+
+#)  Improvements:
+	- Extend Module.in_file_system to support an optimized mode (:pull:`1301`)
+
+#)  Refactor and bugfix for all systems:
+	- Fix Implicit Namespace Packages (:pull:`1290`, :issue:`1276`)
+	- Extend the support for vendored subpackages (:pull:`1294`)
+	- Common: Prevent memory leaks on fail (:pull:`1245`)
+	- Merge dis._unpack_opargs into scan_code to be able to fix a bug in py310
+	  (:pull:`1306`)
+	- Fix some print and f-string (:pull:`1246`)
+	- fixing enumerations (:pull:`1263`)
+	- Fixes for the existing nose tests (:pull:`1234`)
+	- Generate `dev-requirements.txt` + improve readme for contributors wanting
+	  to run tests (:pull:`1224`)
+	- Convert existing tests to pytest + increase coverage (:pull:`1255`)
+
+#)  Linux:
+	- Fix relative path in dependencies, detected in miniconda linux
+	  (:pull:`1258`)
+	- Create symlinks in the target (:pull:`1292`, :issue:`750`)
+
+#)  macOS:
+	- fix bugs in certain subprocess calls (:pull:`1260`)
+	- Apply ad-hoc signature to modified libraries (:pull:`1251`)
+
+#)  Windows:
+	- Set REINSTALLMODE to force installing same-version executables
+	  (:pull:`1252`, :issue:`1250`)
+
+#)  New or improved hooks for:
+	- ctypes/libffi (:pull:`1279`)
+	- flask-compress (:pull:`1295`, :issue:`1273`)
+	- opencv-python (:pull:`1278`, :issue:`1275`)
+	- PyQt5 hooks (:pull:`1302`, :issue:`1261`)
+	- PySide2 - Linux only (:pull:`1302`)
+	- sentry-sdk modules (:pull:`1282`)
+
+#)  Samples:
+	- Update PyQt5 sample (:pull:`1307`)
+
+#)  Documentation:
+	- Update the FAQ (:pull:`1247`)
+	- Update msi doc (:pull:`1248`)
+	- fade to black (:pull:`1291`)
+	- docs: new item in faq (:pull:`1298`)
+	- docs: open external links in a tab (:pull:`1299`)
+	- prepare to release with python 3.10 support (:pull:`1308`)
+
+
+Version 6.8 (September 2021)
+----------------------------
+
+#)  Improvements:
+	- Support pathlib in ModuleFinder (:pull:`1153`)
+	- Use Path in Module.file (:pull:`1158`)
+	- Use Path in _replace_paths_in_code (:pull:`1159`)
+	- Use Path in Module.path (:pull:`1160`)
+	- Convert code in hooks to use Path (:pull:`1161`)
+	- Use path.iterdir to simplify a code block (:pull:`1162`)
+	- Use Path in executable module (:pull:`1163`)
+	- Use Path in ModuleFinder.zip_includes (:pull:`1164`)
+	- Use Path in process_path_specs (:pull:`1167`)
+	- Use Path in Freezer include_files and zip_includes (:pull:`1168`)
+	- Use Path in Freezer.targetdir and some related code (:pull:`1169`)
+	- Use Path in Freezer._copy_file and almost remaining related code
+	  (:pull:`1172`)
+	- Use Path in Executable icon and shortcut_dir (:pull:`1173`)
+	- Use Set[Path] in dependent_files (:pull:`1215`)
+	- Use subprocess (:pull:`1214`)
+	- Add more options to cxfreeze script and tweak the docs (:pull:`1174`)
+
+#)  Refactor and bugfix for all systems:
+	- Remove unused and unnecessary code (:pull:`1142`)
+	- Add some old modules to exclude list (:pull:`1149`)
+	- Fix a last minute change and tweak docstrings (:pull:`1154`)
+	- Include files (from a directory) is ignoring the exclude dependencies
+	  option (:pull:`1216`)
+	- Add more typing to freeze (:pull:`1218`)
+	- Create permanent cx_Freeze/bases (:pull:`1227`)
+	- Make Freezer.targetdir a property to improve a bit (:pull:`1170`)
+	- Code analysis, pep8, f-string (:pull:`1177`)
+	- Complementary fixes (:pull:`1179`)
+	- Use setuptools instead distutils a bit more (:pull:`1195`)
+
+#)  Linux:
+	- Fix py39 in ArchLinux using lto (in a different way than mac)
+	  (:pull:`1146`, :issue:`1132`)
+	- Patchelf calls supports Path type (:pull:`1178`)
+	- Use Path (relative_to and parts) to rewrite the fix rpaths (:pull:`1181`)
+	- Complementary patch to #1181 (:pull:`1201`)
+	- Fix for Miniconda python in linux (:pull:`1219`)
+	- Implement Patchelf.get_needed (still based on ldd) (:pull:`1220`)
+	- Implement Patchelf.is_elf to optimize get_needed (:pull:`1221`)
+	- Fix dependency target and rpath settings (:pull:`1223`)
+	- Patchelf needs permission to write
+	  (:pull:`1232`, :issue:`1171`, :issue:`1197`)
+	- Disable strip with build --debug [linux] (:pull:`1235`, :issue:`1194`)
+
+#)  macOS:
+	- Use Path in darwintools and some pep8 (:pull:`1222`)
+	- Fix MachORef in macdist and add-on tweaks to #1222 (:pull:`1229`)
+
+#)  Windows:
+	- Fix compatibility with msys2 python 3.9.6 (:pull:`1182`)
+	- LLVM dlltool only supports generating an import library (:pull:`1187`)
+	- Normalize paths at startup for MSYS2 python (:pull:`1193`)
+	- Disable delay load to avoid 'Segmentation fault' in mingw 32 bits
+	  (:pull:`1217`)
+	- Support Path as parameter for some functions in C (:pull:`1225`)
+	- Add a stub interface for util module (:pull:`1226`)
+	- Recursing into directories to search for load order files (:pull:`1200`)
+	- Fix program files folder for msi using mingw and some tweaks
+	  (:pull:`1236`)
+
+#)  New or improved hooks for:
+	- _cffi_backend (cffi) (:pull:`1150`)
+	- googleapiclient (:pull:`1151`, :issue:`1147`)
+	- PyQt5 hooks (:pull:`1148`, :pull:`1155`, :pull:`1156`, :issue:`631`,
+	  :issue:`846`, :issue:`972`, :issue:`1119`)
+	- PySide2 (:pull:`1183`)
+	- tzdata, zoneinfo and backports.zoneinfo
+	  (:pull:`1198`, :pull:`1204`, :pull:`1208`)
+	- pyzmq (:pull:`1199`)
+	- numpy+mkl in conda (:pull:`1205`)
+
+#)  Samples:
+	- Fix code of some samples (:pull:`1145`)
+	- Remove outdated sample (:pull:`1157`)
+	- Improve sample to support pyzmq < 20 and timeout (:pull:`1190`)
+	- Tweak pyqt5 and pyside2 samples (:pull:`1180`)
+	- Improve PyQt5 and PySide2 samples (:pull:`1192`)
+
+#)  Documentation:
+	- Make distutils help and documentation more in line with cxfreeze script
+	  (:pull:`1175`)
+	- Update distutils build_exe help in docs (:pull:`1176`)
+	- Remove distutils references in main docs (:pull:`1196`)
+	- Better explain the miniconda installation (:pull:`1209`)
+	- Minor updates to docs (:pull:`1230`)
+
+
 Version 6.7 (July 2021)
 -----------------------
 
 #)  Improvements, refactor and bugfix for all systems:
 	- Implemented multi levels for build_exe silent option (:pull:`883`)
 	- Corrected silent_level to default to 0 (to agree with documentation) (:pull:`1046`)
 	- Split up Freezer object (:pull:`1035`)
```

### Comparing `cx_Freeze-6.8b5/doc/src/index.rst` & `cx_Freeze-6.9/doc/src/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,18 @@
 .. list-table::
    :header-rows: 1
    :widths: 300 300 200
 
    * - cx_Freeze version
      - Python version
      - Status
-   * - cx_Freeze 6.4 to 6.7
+   * - cx_Freeze 6.9
+     - Python 3.6 to 3.10
+     - supported
+   * - cx_Freeze 6.4 to 6.8
      - Python 3.6 to 3.9
      - supported
    * - cx_Freeze 6.2, 6.3
      - Python 3.5.2 to 3.8
      - unsupported
    * - cx_Freeze 6.1
      - Python 3.5.0 to 3.8
```

### Comparing `cx_Freeze-6.8b5/doc/src/setup_script.rst` & `cx_Freeze-6.9/doc/src/setup_script.rst`

 * *Files 1% similar despite different names*

```diff
@@ -366,14 +366,20 @@
    * - .. option:: extensions
      - list of dictionaries specifying the extensions that the installed program
        handles. Each extension needs to specify at least the extension, a verb,
        and an executable. Additional allowed keys are `argument` to specify
        the invocation of the executable, `mime` for the extension’s mime type,
        and `context` for the context menu text.
 
+.. versionadded:: 6.7
+    ``extensions`` options.
+    
+.. note:: ``extensions`` is supported in python 3.7.4 and up.
+
+
 This is the equivalent help to specify the same options on the command line:
 
   .. code-block:: console
 
     python setup.py bdist_msi --help
 
 For example:
```

### Comparing `cx_Freeze-6.8b5/doc/src/installation.rst` & `cx_Freeze-6.9/doc/src/installation.rst`

 * *Files 7% similar despite different names*

```diff
@@ -50,129 +50,147 @@
 00000310: 7463 6865 6c66 0a0a 546f 2069 6e73 7461  tchelf..To insta
 00000320: 6c6c 2070 6174 6368 656c 6620 696e 2066  ll patchelf in f
 00000330: 6564 6f72 613a 0a0a 2020 2e2e 2063 6f64  edora:..  .. cod
 00000340: 652d 626c 6f63 6b3a 3a20 636f 6e73 6f6c  e-block:: consol
 00000350: 650a 0a20 2020 2064 6e66 2069 6e73 7461  e..    dnf insta
 00000360: 6c6c 2070 6174 6368 656c 660a 0a4f 7220  ll patchelf..Or 
 00000370: 696e 7374 616c 6c20 7061 7463 6865 6c66  install patchelf
-00000380: 2066 726f 6d0a 6073 6f75 7263 6573 203c   from.`sources <
-00000390: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000003a0: 6f6d 2f4e 6978 4f53 2f70 6174 6368 656c  om/NixOS/patchel
-000003b0: 6623 636f 6d70 696c 696e 672d 616e 642d  f#compiling-and-
-000003c0: 7465 7374 696e 673e 605f 3a0a 0a20 202e  testing>`_:..  .
-000003d0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2063  . code-block:: c
-000003e0: 6f6e 736f 6c65 0a0a 2020 2020 6769 7420  onsole..    git 
-000003f0: 636c 6f6e 6520 2d62 2030 2e31 3320 2d2d  clone -b 0.13 --
-00000400: 7369 6e67 6c65 2d62 7261 6e63 6820 6874  single-branch ht
-00000410: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000420: 2f4e 6978 4f53 2f70 6174 6368 656c 662e  /NixOS/patchelf.
-00000430: 6769 740a 2020 2020 6364 2070 6174 6368  git.    cd patch
-00000440: 656c 660a 2020 2020 2e2f 626f 6f74 7374  elf.    ./bootst
-00000450: 7261 702e 7368 0a20 2020 202e 2f63 6f6e  rap.sh.    ./con
-00000460: 6669 6775 7265 0a20 2020 206d 616b 650a  figure.    make.
-00000470: 2020 2020 6d61 6b65 2063 6865 636b 0a20      make check. 
-00000480: 2020 2073 7564 6f20 6d61 6b65 2069 6e73     sudo make ins
-00000490: 7461 6c6c 0a0a 0a50 6970 656e 760a 2d2d  tall...Pipenv.--
-000004a0: 2d2d 2d2d 0a0a 5573 696e 6720 7069 7065  ----..Using pipe
-000004b0: 6e76 2c20 696e 7374 616c 6c20 6f72 2075  nv, install or u
-000004c0: 7064 6174 6520 6279 2069 7373 7569 6e67  pdate by issuing
-000004d0: 206f 6e65 206f 6620 7468 6520 666f 6c6f   one of the folo
-000004e0: 7769 6e67 2063 6f6d 6d61 6e64 613a 0a0a  wing commanda:..
-000004f0: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-00000500: 3a20 636f 6e73 6f6c 650a 0a20 2020 2070  : console..    p
-00000510: 6970 656e 7620 696e 7374 616c 6c20 6378  ipenv install cx
-00000520: 5f46 7265 657a 650a 2020 2020 7069 7065  _Freeze.    pipe
-00000530: 6e76 2075 7064 6174 6520 6378 5f46 7265  nv update cx_Fre
-00000540: 657a 650a 0a4d 696e 6963 6f6e 6461 330a  eze..Miniconda3.
-00000550: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 4469 7265  ----------..Dire
-00000560: 6374 6c79 2066 726f 6d20 7468 6520 636f  ctly from the co
-00000570: 6e64 612d 666f 7267 6520 6368 616e 6e65  nda-forge channe
-00000580: 6c3a 0a0a 2020 2e2e 2063 6f64 652d 626c  l:..  .. code-bl
-00000590: 6f63 6b3a 3a20 636f 6e73 6f6c 650a 0a20  ock:: console.. 
-000005a0: 2020 2063 6f6e 6461 2069 6e73 7461 6c6c     conda install
-000005b0: 202d 6320 636f 6e64 612d 666f 7267 6520   -c conda-forge 
-000005c0: 6378 5f66 7265 657a 650a 0a49 6620 796f  cx_freeze..If yo
-000005d0: 7520 6172 6520 696e 7374 616c 6c69 6e67  u are installing
-000005e0: 2061 2070 7265 2d72 656c 6561 7365 206f   a pre-release o
-000005f0: 7220 6672 6f6d 2073 6f75 7263 6573 2c20  r from sources, 
-00000600: 696e 7374 616c 6c20 7468 6520 7265 7175  install the requ
-00000610: 6972 656d 656e 7473 0a75 7369 6e67 2074  irements.using t
-00000620: 6865 2073 616d 6520 6368 616e 6e65 6c3a  he same channel:
-00000630: 0a0a 2d20 7079 7468 6f6e 0a2d 2063 2d63  ..- python.- c-c
-00000640: 6f6d 7069 6c65 720a 2d20 6c69 6270 7974  ompiler.- libpyt
-00000650: 686f 6e2d 7374 6174 6963 2028 666f 7220  hon-static (for 
-00000660: 7079 7468 6f6e 203e 3d33 2e38 2069 6e20  python >=3.8 in 
-00000670: 6c69 6e75 7820 616e 6420 6d61 634f 5329  linux and macOS)
-00000680: 0a2d 2069 6d70 6f72 746c 6962 2d6d 6574  .- importlib-met
-00000690: 6164 6174 610a 2d20 7061 7463 6865 6c66  adata.- patchelf
-000006a0: 2028 6f70 7469 6f6e 616c 2069 6620 616c   (optional if al
-000006b0: 7265 6164 7920 696e 7374 616c 6c65 6420  ready installed 
-000006c0: 696e 2074 6865 204c 696e 7578 2073 7973  in the Linux sys
-000006d0: 7465 6d29 0a2d 2064 6563 6c61 7265 2053  tem).- declare S
-000006e0: 444b 524f 4f54 206f 7220 434f 4e44 415f  DKROOT or CONDA_
-000006f0: 4255 494c 445f 5359 5352 4f4f 5420 2866  BUILD_SYSROOT (f
-00000700: 6f72 2070 7974 686f 6e20 332e 3920 696e  or python 3.9 in
-00000710: 206d 6163 4f53 290a 0a41 2065 7861 6d70   macOS)..A examp
-00000720: 6c65 2075 7369 6e67 204d 696e 6963 6f6e  le using Minicon
-00000730: 6461 333a 0a0a 2020 2e2e 2063 6f64 652d  da3:..  .. code-
-00000740: 626c 6f63 6b3a 3a20 636f 6e73 6f6c 650a  block:: console.
-00000750: 0a20 2020 2023 2049 6620 7573 696e 6720  .    # If using 
-00000760: 7079 7468 6f6e 2033 2e39 206f 7220 6869  python 3.9 or hi
-00000770: 6765 7220 696e 2047 6974 6875 6220 4163  ger in Github Ac
-00000780: 7469 6f6e 7320 4349 2c20 6d61 634f 532c  tions CI, macOS,
-00000790: 2075 7365 2074 6869 733a 0a20 2020 2065   use this:.    e
-000007a0: 7870 6f72 7420 5344 4b52 4f4f 543d 2f4c  xport SDKROOT=/L
-000007b0: 6962 7261 7279 2f44 6576 656c 6f70 6572  ibrary/Developer
-000007c0: 2f43 6f6d 6d61 6e64 4c69 6e65 546f 6f6c  /CommandLineTool
-000007d0: 732f 5344 4b73 2f4d 6163 4f53 5831 312e  s/SDKs/MacOSX11.
-000007e0: 312e 7364 6b0a 0a20 2020 2023 2046 6f72  1.sdk..    # For
-000007f0: 206d 6163 4f53 2061 6e64 204c 696e 7578   macOS and Linux
-00000800: 0a20 2020 2063 6f6e 6461 2063 7265 6174  .    conda creat
-00000810: 6520 2d6e 2063 7833 3963 6f6e 6461 202d  e -n cx39conda -
-00000820: 6320 636f 6e64 612d 666f 7267 6520 7079  c conda-forge py
-00000830: 7468 6f6e 3d33 2e39 206c 6962 7079 7468  thon=3.9 libpyth
-00000840: 6f6e 2d73 7461 7469 6320 2d79 0a20 2020  on-static -y.   
-00000850: 2063 6f6e 6461 2061 6374 6976 6174 6520   conda activate 
-00000860: 6378 3339 636f 6e64 610a 2020 2020 636f  cx39conda.    co
-00000870: 6e64 6120 696e 7374 616c 6c20 2d63 2063  nda install -c c
-00000880: 6f6e 6461 2d66 6f72 6765 2063 2d63 6f6d  onda-forge c-com
-00000890: 7069 6c65 7220 696d 706f 7274 6c69 622d  piler importlib-
-000008a0: 6d65 7461 6461 7461 202d 790a 2020 2020  metadata -y.    
-000008b0: 7069 7020 696e 7374 616c 6c20 2d2d 6e6f  pip install --no
-000008c0: 2d62 696e 6172 7920 3a61 6c6c 3a20 2d2d  -binary :all: --
-000008d0: 7072 6520 6378 5f46 7265 657a 6520 2d76  pre cx_Freeze -v
-000008e0: 0a0a 446f 776e 6c6f 6164 2074 6172 6261  ..Download tarba
-000008f0: 6c6c 206f 7220 7768 6565 6c73 0a2d 2d2d  ll or wheels.---
-00000900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000910: 2d2d 2d2d 2d2d 2d0a 0a44 6f77 6e6c 6f61  -------..Downloa
-00000920: 6420 6469 7265 6374 6c79 2066 726f 6d20  d directly from 
-00000930: 6050 7950 4920 3c68 7474 7073 3a2f 2f70  `PyPI <https://p
-00000940: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000950: 6378 5f46 7265 657a 653e 605f 2e0a 0a0a  cx_Freeze>`_....
-00000960: 446f 776e 6c6f 6164 2074 6865 2073 6f75  Download the sou
-00000970: 7263 6520 636f 6465 0a2d 2d2d 2d2d 2d2d  rce code.-------
-00000980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000990: 2d0a 0a59 6f75 2063 616e 2064 6f77 6e6c  -..You can downl
-000009a0: 6f61 6420 616e 6420 6578 7472 6163 7420  oad and extract 
-000009b0: 7468 6520 736f 7572 6365 2063 6f64 6520  the source code 
-000009c0: 666f 756e 6420 6f6e 0a60 4769 7468 7562  found on.`Github
-000009d0: 203c 6874 7470 733a 2f2f 6769 7468 7562   <https://github
-000009e0: 2e63 6f6d 2f6d 6172 6365 6c6f 7464 7561  .com/marcelotdua
-000009f0: 7274 652f 6378 5f46 7265 657a 653e 605f  rte/cx_Freeze>`_
-00000a00: 5f0a 746f 2064 6f20 6120 6120 6d61 6e75  _.to do a a manu
-00000a10: 616c 2069 6e73 7461 6c6c 6174 696f 6e2e  al installation.
-00000a20: 0a0a 496e 2074 6865 2073 6f75 7263 6520  ..In the source 
-00000a30: 6469 7265 6374 6f72 792c 2075 7365 206f  directory, use o
-00000a40: 6e65 206f 6620 7468 6520 636f 6d6d 616e  ne of the comman
-00000a50: 643a 0a0a 2020 2e2e 2063 6f64 652d 626c  d:..  .. code-bl
-00000a60: 6f63 6b3a 3a20 636f 6e73 6f6c 650a 0a20  ock:: console.. 
-00000a70: 2020 2070 6970 2069 6e73 7461 6c6c 202d     pip install -
-00000a80: 6520 2e0a 0a6f 720a 0a20 202e 2e20 636f  e ...or..  .. co
-00000a90: 6465 2d62 6c6f 636b 3a3a 2063 6f6e 736f  de-block:: conso
-00000aa0: 6c65 0a0a 2020 2020 7079 7468 6f6e 2073  le..    python s
-00000ab0: 6574 7570 2e70 7920 6465 7665 6c6f 700a  etup.py develop.
-00000ac0: 0a0a 4973 7375 6520 7472 6163 6b69 6e67  ..Issue tracking
-00000ad0: 206f 6e20 6047 6974 6875 6220 3c68 7474   on `Github <htt
-00000ae0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000af0: 6d61 7263 656c 6f74 6475 6172 7465 2f63  marcelotduarte/c
-00000b00: 785f 4672 6565 7a65 2f69 7373 7565 733e  x_Freeze/issues>
-00000b10: 605f 2e0a                                `_..
+00000380: 2066 726f 6d20 7c70 6174 6368 656c 665f   from |patchelf_
+00000390: 736f 7572 6365 737c 3a0a 0a2e 2e20 7c70  sources|:.... |p
+000003a0: 6174 6368 656c 665f 736f 7572 6365 737c  atchelf_sources|
+000003b0: 2072 6177 3a3a 2068 746d 6c0a 0a20 2020   raw:: html..   
+000003c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000003d0: 2f67 6974 6875 622e 636f 6d2f 4e69 784f  /github.com/NixO
+000003e0: 532f 7061 7463 6865 6c66 2363 6f6d 7069  S/patchelf#compi
+000003f0: 6c69 6e67 2d61 6e64 2d74 6573 7469 6e67  ling-and-testing
+00000400: 2220 7461 7267 6574 3d22 5f62 6c61 6e6b  " target="_blank
+00000410: 223e 736f 7572 6365 733c 2f61 3e0a 0a20  ">sources</a>.. 
+00000420: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+00000430: 2063 6f6e 736f 6c65 0a0a 2020 2020 6769   console..    gi
+00000440: 7420 636c 6f6e 6520 2d62 2030 2e31 3320  t clone -b 0.13 
+00000450: 2d2d 7369 6e67 6c65 2d62 7261 6e63 6820  --single-branch 
+00000460: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000470: 6f6d 2f4e 6978 4f53 2f70 6174 6368 656c  om/NixOS/patchel
+00000480: 662e 6769 740a 2020 2020 6364 2070 6174  f.git.    cd pat
+00000490: 6368 656c 660a 2020 2020 2e2f 626f 6f74  chelf.    ./boot
+000004a0: 7374 7261 702e 7368 0a20 2020 202e 2f63  strap.sh.    ./c
+000004b0: 6f6e 6669 6775 7265 0a20 2020 206d 616b  onfigure.    mak
+000004c0: 650a 2020 2020 6d61 6b65 2063 6865 636b  e.    make check
+000004d0: 0a20 2020 2073 7564 6f20 6d61 6b65 2069  .    sudo make i
+000004e0: 6e73 7461 6c6c 0a0a 0a50 6970 656e 760a  nstall...Pipenv.
+000004f0: 2d2d 2d2d 2d2d 0a0a 5573 696e 6720 7069  ------..Using pi
+00000500: 7065 6e76 2c20 696e 7374 616c 6c20 6f72  penv, install or
+00000510: 2075 7064 6174 6520 6279 2069 7373 7569   update by issui
+00000520: 6e67 206f 6e65 206f 6620 7468 6520 666f  ng one of the fo
+00000530: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 613a  lowing commanda:
+00000540: 0a0a 2020 2e2e 2063 6f64 652d 626c 6f63  ..  .. code-bloc
+00000550: 6b3a 3a20 636f 6e73 6f6c 650a 0a20 2020  k:: console..   
+00000560: 2070 6970 656e 7620 696e 7374 616c 6c20   pipenv install 
+00000570: 6378 5f46 7265 657a 650a 2020 2020 7069  cx_Freeze.    pi
+00000580: 7065 6e76 2075 7064 6174 6520 6378 5f46  penv update cx_F
+00000590: 7265 657a 650a 0a4d 696e 6963 6f6e 6461  reeze..Miniconda
+000005a0: 330a 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 4469  3.----------..Di
+000005b0: 7265 6374 6c79 2066 726f 6d20 7468 6520  rectly from the 
+000005c0: 636f 6e64 612d 666f 7267 6520 6368 616e  conda-forge chan
+000005d0: 6e65 6c3a 0a0a 2020 2e2e 2063 6f64 652d  nel:..  .. code-
+000005e0: 626c 6f63 6b3a 3a20 636f 6e73 6f6c 650a  block:: console.
+000005f0: 0a20 2020 2063 6f6e 6461 2069 6e73 7461  .    conda insta
+00000600: 6c6c 202d 6320 636f 6e64 612d 666f 7267  ll -c conda-forg
+00000610: 6520 6378 5f66 7265 657a 650a 0a49 6620  e cx_freeze..If 
+00000620: 796f 7520 6172 6520 696e 7374 616c 6c69  you are installi
+00000630: 6e67 2061 2070 7265 2d72 656c 6561 7365  ng a pre-release
+00000640: 206f 7220 6672 6f6d 2073 6f75 7263 6573   or from sources
+00000650: 2c20 696e 7374 616c 6c20 7468 6520 7265  , install the re
+00000660: 7175 6972 656d 656e 7473 0a75 7369 6e67  quirements.using
+00000670: 2074 6865 2073 616d 6520 6368 616e 6e65   the same channe
+00000680: 6c3a 0a0a 2d20 7079 7468 6f6e 0a2d 2063  l:..- python.- c
+00000690: 2d63 6f6d 7069 6c65 720a 2d20 6c69 6270  -compiler.- libp
+000006a0: 7974 686f 6e2d 7374 6174 6963 2028 666f  ython-static (fo
+000006b0: 7220 7079 7468 6f6e 203e 3d33 2e38 2069  r python >=3.8 i
+000006c0: 6e20 6c69 6e75 7820 616e 6420 6d61 634f  n linux and macO
+000006d0: 5329 0a2d 2069 6d70 6f72 746c 6962 2d6d  S).- importlib-m
+000006e0: 6574 6164 6174 610a 2d20 7061 7463 6865  etadata.- patche
+000006f0: 6c66 2028 6f70 7469 6f6e 616c 2069 6620  lf (optional if 
+00000700: 616c 7265 6164 7920 696e 7374 616c 6c65  already installe
+00000710: 6420 696e 2074 6865 204c 696e 7578 2073  d in the Linux s
+00000720: 7973 7465 6d29 0a2d 2064 6563 6c61 7265  ystem).- declare
+00000730: 2053 444b 524f 4f54 206f 7220 434f 4e44   SDKROOT or COND
+00000740: 415f 4255 494c 445f 5359 5352 4f4f 5420  A_BUILD_SYSROOT 
+00000750: 2866 6f72 2070 7974 686f 6e20 332e 3920  (for python 3.9 
+00000760: 696e 206d 6163 4f53 290a 0a41 6e20 6578  in macOS)..An ex
+00000770: 616d 706c 6520 7573 696e 6720 4d69 6e69  ample using Mini
+00000780: 636f 6e64 6133 3a0a 0a20 202e 2e20 636f  conda3:..  .. co
+00000790: 6465 2d62 6c6f 636b 3a3a 2063 6f6e 736f  de-block:: conso
+000007a0: 6c65 0a0a 2020 2020 2320 4966 2075 7369  le..    # If usi
+000007b0: 6e67 2070 7974 686f 6e20 332e 3920 6f72  ng python 3.9 or
+000007c0: 2068 6967 6572 2069 6e20 4769 7468 7562   higer in Github
+000007d0: 2041 6374 696f 6e73 2043 492c 206d 6163   Actions CI, mac
+000007e0: 4f53 2c20 7573 6520 7468 6973 3a0a 2020  OS, use this:.  
+000007f0: 2020 6578 706f 7274 2053 444b 524f 4f54    export SDKROOT
+00000800: 3d2f 4c69 6272 6172 792f 4465 7665 6c6f  =/Library/Develo
+00000810: 7065 722f 436f 6d6d 616e 644c 696e 6554  per/CommandLineT
+00000820: 6f6f 6c73 2f53 444b 732f 4d61 634f 5358  ools/SDKs/MacOSX
+00000830: 3131 2e31 2e73 646b 0a0a 2020 2020 2320  11.1.sdk..    # 
+00000840: 466f 7220 6d61 634f 5320 616e 6420 4c69  For macOS and Li
+00000850: 6e75 780a 2020 2020 636f 6e64 6120 6372  nux.    conda cr
+00000860: 6561 7465 202d 6e20 6378 3339 636f 6e64  eate -n cx39cond
+00000870: 6120 2d63 2063 6f6e 6461 2d66 6f72 6765  a -c conda-forge
+00000880: 2070 7974 686f 6e3d 332e 3920 6c69 6270   python=3.9 libp
+00000890: 7974 686f 6e2d 7374 6174 6963 202d 790a  ython-static -y.
+000008a0: 2020 2020 636f 6e64 6120 6163 7469 7661      conda activa
+000008b0: 7465 2063 7833 3963 6f6e 6461 0a20 2020  te cx39conda.   
+000008c0: 2063 6f6e 6461 2069 6e73 7461 6c6c 202d   conda install -
+000008d0: 6320 636f 6e64 612d 666f 7267 6520 632d  c conda-forge c-
+000008e0: 636f 6d70 696c 6572 2069 6d70 6f72 746c  compiler importl
+000008f0: 6962 2d6d 6574 6164 6174 6120 2d79 0a20  ib-metadata -y. 
+00000900: 2020 2070 6970 2069 6e73 7461 6c6c 202d     pip install -
+00000910: 2d6e 6f2d 6269 6e61 7279 203a 616c 6c3a  -no-binary :all:
+00000920: 202d 2d70 7265 2063 785f 4672 6565 7a65   --pre cx_Freeze
+00000930: 202d 760a 0a44 6f77 6e6c 6f61 6420 7461   -v..Download ta
+00000940: 7262 616c 6c20 6f72 2077 6865 656c 730a  rball or wheels.
+00000950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000960: 2d2d 2d2d 2d2d 2d2d 2d2d 0a0a 446f 776e  ----------..Down
+00000970: 6c6f 6164 2064 6972 6563 746c 7920 6672  load directly fr
+00000980: 6f6d 207c 5079 5049 5f6c 696e 6b7c 2e0a  om |PyPI_link|..
+00000990: 0a2e 2e20 7c50 7950 495f 6c69 6e6b 7c20  ... |PyPI_link| 
+000009a0: 7261 773a 3a20 6874 6d6c 0a0a 2020 203c  raw:: html..   <
+000009b0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000009c0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000009d0: 2f63 785f 4672 6565 7a65 2220 7461 7267  /cx_Freeze" targ
+000009e0: 6574 3d22 5f62 6c61 6e6b 223e 5079 5049  et="_blank">PyPI
+000009f0: 3c2f 613e 0a0a 446f 776e 6c6f 6164 2074  </a>..Download t
+00000a00: 6865 2073 6f75 7263 6520 636f 6465 0a2d  he source code.-
+00000a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000a20: 2d2d 2d2d 2d2d 2d0a 0a59 6f75 2063 616e  -------..You can
+00000a30: 2064 6f77 6e6c 6f61 6420 616e 6420 6578   download and ex
+00000a40: 7472 6163 7420 7468 6520 736f 7572 6365  tract the source
+00000a50: 2063 6f64 6520 666f 756e 6420 6f6e 207c   code found on |
+00000a60: 4769 7468 7562 5f6d 6169 6e7c 2074 6f20  Github_main| to 
+00000a70: 646f 2061 0a6d 616e 7561 6c20 696e 7374  do a.manual inst
+00000a80: 616c 6c61 7469 6f6e 2e0a 0a2e 2e20 7c47  allation..... |G
+00000a90: 6974 6875 625f 6d61 696e 7c20 7261 773a  ithub_main| raw:
+00000aa0: 3a20 6874 6d6c 0a0a 2020 203c 6120 6872  : html..   <a hr
+00000ab0: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000ac0: 7562 2e63 6f6d 2f6d 6172 6365 6c6f 7464  ub.com/marcelotd
+00000ad0: 7561 7274 652f 6378 5f46 7265 657a 6522  uarte/cx_Freeze"
+00000ae0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000af0: 3e47 6974 6875 623c 2f61 3e0a 0a49 6e20  >Github</a>..In 
+00000b00: 7468 6520 736f 7572 6365 2064 6972 6563  the source direc
+00000b10: 746f 7279 2c20 7573 6520 6f6e 6520 6f66  tory, use one of
+00000b20: 2074 6865 2063 6f6d 6d61 6e64 3a0a 0a20   the command:.. 
+00000b30: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+00000b40: 2063 6f6e 736f 6c65 0a0a 2020 2020 7069   console..    pi
+00000b50: 7020 696e 7374 616c 6c20 2d65 202e 0a0a  p install -e ...
+00000b60: 6f72 0a0a 2020 2e2e 2063 6f64 652d 626c  or..  .. code-bl
+00000b70: 6f63 6b3a 3a20 636f 6e73 6f6c 650a 0a20  ock:: console.. 
+00000b80: 2020 2070 7974 686f 6e20 7365 7475 702e     python setup.
+00000b90: 7079 2064 6576 656c 6f70 0a0a 0a49 7373  py develop...Iss
+00000ba0: 7565 2074 7261 636b 696e 6720 6f6e 207c  ue tracking on |
+00000bb0: 4769 7468 7562 5f69 7373 7565 737c 2e0a  Github_issues|..
+00000bc0: 0a2e 2e20 7c47 6974 6875 625f 6973 7375  ... |Github_issu
+00000bd0: 6573 7c20 7261 773a 3a20 6874 6d6c 0a0a  es| raw:: html..
+00000be0: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+00000bf0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
+00000c00: 6172 6365 6c6f 7464 7561 7274 652f 6378  arcelotduarte/cx
+00000c10: 5f46 7265 657a 652f 6973 7375 6573 2220  _Freeze/issues" 
+00000c20: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00000c30: 4769 7468 7562 3c2f 613e 0a              Github</a>.
```

### Comparing `cx_Freeze-6.8b5/doc/src/overview.rst` & `cx_Freeze-6.9/doc/src/overview.rst`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 3. Work directly with the classes and modules used internally by cx_Freeze.
    This should be reserved for complicated scripts or extending or embedding.
 
 cx_Freeze normally produces a folder containing an executable file for your
 program, along with the shared libraries (DLLs or .so files) needed to run it.
 You can make a simple Windows installer using a :ref:`setup script <setup_script>`
 with the ``bdist_msi`` option, or a Mac disk image with ``bdist_dmg``. For a
-more advanced Windows installer, use a separate tool like `Inno Setup
-<https://www.jrsoftware.org/isinfo.php>`_ to package the files cx_Freeze
-collects.
+more advanced Windows installer, use a separate tool like |Inno_Setup| to
+package the files cx_Freeze collects.
 
 Python modules for your executables are stored in a zip file. Packages are
 stored in the file system by default but can also be included in the zip file.
 
+.. |Inno_Setup| raw:: html
+
+   <a href="https://www.jrsoftware.org/isinfo.php" target="_blank">Inno Setup</a>
```

### Comparing `cx_Freeze-6.8b5/doc/src/development/code_layout.rst` & `cx_Freeze-6.9/doc/src/development/code_layout.rst`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/doc/src/development/index.rst` & `cx_Freeze-6.9/doc/src/development/index.rst`

 * *Files identical despite different names*

### Comparing `cx_Freeze-6.8b5/doc/Makefile` & `cx_Freeze-6.9/doc/Makefile`

 * *Files identical despite different names*

