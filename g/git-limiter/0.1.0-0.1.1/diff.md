# Comparing `tmp/git_limiter-0.1.0.tar.gz` & `tmp/git_limiter-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_limiter-0.1.0.tar", max compression
+gzip compressed data, was "git_limiter-0.1.1.tar", max compression
```

## Comparing `git_limiter-0.1.0.tar` & `git_limiter-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1069 2023-04-06 18:06:38.105491 git_limiter-0.1.0/LICENSE.md
--rw-r--r--   0        0        0        0 2023-04-06 18:47:57.888805 git_limiter-0.1.0/git_limiter/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 16:04:08.705803 git_limiter-0.1.0/git_limiter/backend/__init__.py
--rw-r--r--   0        0        0      168 2023-04-06 20:05:12.888698 git_limiter-0.1.0/git_limiter/backend/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      999 2023-04-08 07:10:03.676719 git_limiter-0.1.0/git_limiter/backend/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     1998 2023-04-08 07:55:09.934424 git_limiter-0.1.0/git_limiter/backend/__pycache__/git_subprocess_backend.cpython-39.pyc
--rw-r--r--   0        0        0      516 2023-04-08 07:10:02.918273 git_limiter-0.1.0/git_limiter/backend/base.py
--rw-r--r--   0        0        0     1906 2023-04-08 07:59:41.247720 git_limiter-0.1.0/git_limiter/backend/git_subprocess_backend.py
--rw-r--r--   0        0        0        0 2023-04-06 17:08:13.652946 git_limiter-0.1.0/git_limiter/checks/__init__.py
--rw-r--r--   0        0        0      167 2023-04-06 18:13:33.838984 git_limiter-0.1.0/git_limiter/checks/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1028 2023-04-08 07:10:08.573492 git_limiter-0.1.0/git_limiter/checks/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     1843 2023-04-06 19:20:53.714336 git_limiter-0.1.0/git_limiter/checks/__pycache__/max_diff.cpython-39.pyc
--rw-r--r--   0        0        0      557 2023-04-08 07:10:07.775150 git_limiter-0.1.0/git_limiter/checks/base.py
--rw-r--r--   0        0        0     1499 2023-04-06 19:17:07.272209 git_limiter-0.1.0/git_limiter/checks/max_diff.py
--rw-r--r--   0        0        0     3172 2023-04-08 07:59:41.230272 git_limiter-0.1.0/git_limiter/cli.py
--rw-r--r--   0        0        0        0 2023-04-08 07:06:15.975203 git_limiter-0.1.0/git_limiter/config/__init__.py
--rw-r--r--   0        0        0      167 2023-04-08 07:09:57.600715 git_limiter-0.1.0/git_limiter/config/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2266 2023-04-08 07:09:57.601752 git_limiter-0.1.0/git_limiter/config/__pycache__/settings.cpython-39.pyc
--rw-r--r--   0        0        0     1753 2023-04-08 08:01:18.085530 git_limiter-0.1.0/git_limiter/config/settings.py
--rw-r--r--   0        0        0      211 2023-04-08 07:59:40.988664 git_limiter-0.1.0/git_limiter/constants.py
--rw-r--r--   0        0        0        0 2023-04-06 17:08:02.232981 git_limiter-0.1.0/git_limiter/errors.py
--rw-r--r--   0        0        0        0 2023-04-07 18:11:42.780855 git_limiter-0.1.0/git_limiter/parsers/__init__.py
--rw-r--r--   0        0        0      166 2023-04-07 19:13:02.707477 git_limiter-0.1.0/git_limiter/parsers/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1000 2023-04-08 07:17:36.436796 git_limiter-0.1.0/git_limiter/parsers/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0     1106 2023-04-08 06:40:55.378432 git_limiter-0.1.0/git_limiter/parsers/__pycache__/max_diff.cpython-39.pyc
--rw-r--r--   0        0        0      593 2023-04-08 07:15:53.684031 git_limiter-0.1.0/git_limiter/parsers/base.py
--rw-r--r--   0        0        0      785 2023-04-07 20:13:48.317698 git_limiter-0.1.0/git_limiter/parsers/max_diff.py
--rw-r--r--   0        0        0      568 2023-04-06 19:17:54.710272 git_limiter-0.1.0/git_limiter/stats.py
--rw-r--r--   0        0        0        0 2023-04-06 17:33:21.955230 git_limiter-0.1.0/git_limiter/terminal/__init__.py
--rw-r--r--   0        0        0      169 2023-04-06 18:13:33.839884 git_limiter-0.1.0/git_limiter/terminal/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      674 2023-04-06 19:20:53.713696 git_limiter-0.1.0/git_limiter/terminal/__pycache__/base.cpython-39.pyc
--rw-r--r--   0        0        0      698 2023-04-08 06:40:55.381233 git_limiter-0.1.0/git_limiter/terminal/__pycache__/rich_terminal.cpython-39.pyc
--rw-r--r--   0        0        0      254 2023-04-06 19:17:07.276564 git_limiter-0.1.0/git_limiter/terminal/base.py
--rw-r--r--   0        0        0      272 2023-04-08 04:56:43.714398 git_limiter-0.1.0/git_limiter/terminal/rich_terminal.py
--rw-r--r--   0        0        0     1088 2023-04-08 08:36:35.513121 git_limiter-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 git_limiter-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-06 18:06:38.105491 git_limiter-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-04-06 18:47:57.888805 git_limiter-0.1.1/git_limiter/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 16:04:08.705803 git_limiter-0.1.1/git_limiter/backend/__init__.py
+-rw-r--r--   0        0        0      168 2023-04-06 20:05:12.888698 git_limiter-0.1.1/git_limiter/backend/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      999 2023-04-08 07:10:03.676719 git_limiter-0.1.1/git_limiter/backend/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     1998 2023-04-08 10:31:57.634967 git_limiter-0.1.1/git_limiter/backend/__pycache__/git_subprocess_backend.cpython-39.pyc
+-rw-r--r--   0        0        0      516 2023-04-08 07:10:02.918273 git_limiter-0.1.1/git_limiter/backend/base.py
+-rw-r--r--   0        0        0     1888 2023-04-08 11:06:52.171814 git_limiter-0.1.1/git_limiter/backend/git_subprocess_backend.py
+-rw-r--r--   0        0        0        0 2023-04-06 17:08:13.652946 git_limiter-0.1.1/git_limiter/checks/__init__.py
+-rw-r--r--   0        0        0      167 2023-04-06 18:13:33.838984 git_limiter-0.1.1/git_limiter/checks/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1028 2023-04-08 07:10:08.573492 git_limiter-0.1.1/git_limiter/checks/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     2000 2023-04-08 10:31:57.639147 git_limiter-0.1.1/git_limiter/checks/__pycache__/max_diff.cpython-39.pyc
+-rw-r--r--   0        0        0      557 2023-04-08 07:10:07.775150 git_limiter-0.1.1/git_limiter/checks/base.py
+-rw-r--r--   0        0        0     2122 2023-04-08 10:22:57.199030 git_limiter-0.1.1/git_limiter/checks/max_diff.py
+-rw-r--r--   0        0        0     3172 2023-04-08 14:56:35.462380 git_limiter-0.1.1/git_limiter/cli.py
+-rw-r--r--   0        0        0        0 2023-04-08 07:06:15.975203 git_limiter-0.1.1/git_limiter/config/__init__.py
+-rw-r--r--   0        0        0      167 2023-04-08 07:09:57.600715 git_limiter-0.1.1/git_limiter/config/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2251 2023-04-08 10:31:57.631955 git_limiter-0.1.1/git_limiter/config/__pycache__/settings.cpython-39.pyc
+-rw-r--r--   0        0        0     1753 2023-04-08 08:01:18.085530 git_limiter-0.1.1/git_limiter/config/settings.py
+-rw-r--r--   0        0        0      993 2023-04-08 14:56:35.462567 git_limiter-0.1.1/git_limiter/constants.py
+-rw-r--r--   0        0        0        0 2023-04-06 17:08:02.232981 git_limiter-0.1.1/git_limiter/errors.py
+-rw-r--r--   0        0        0        0 2023-04-07 18:11:42.780855 git_limiter-0.1.1/git_limiter/parsers/__init__.py
+-rw-r--r--   0        0        0      166 2023-04-07 19:13:02.707477 git_limiter-0.1.1/git_limiter/parsers/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1000 2023-04-08 07:17:36.436796 git_limiter-0.1.1/git_limiter/parsers/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0     1106 2023-04-08 06:40:55.378432 git_limiter-0.1.1/git_limiter/parsers/__pycache__/max_diff.cpython-39.pyc
+-rw-r--r--   0        0        0      593 2023-04-08 07:15:53.684031 git_limiter-0.1.1/git_limiter/parsers/base.py
+-rw-r--r--   0        0        0      785 2023-04-07 20:13:48.317698 git_limiter-0.1.1/git_limiter/parsers/max_diff.py
+-rw-r--r--   0        0        0      568 2023-04-06 19:17:54.710272 git_limiter-0.1.1/git_limiter/stats.py
+-rw-r--r--   0        0        0        0 2023-04-06 17:33:21.955230 git_limiter-0.1.1/git_limiter/terminal/__init__.py
+-rw-r--r--   0        0        0      169 2023-04-06 18:13:33.839884 git_limiter-0.1.1/git_limiter/terminal/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      674 2023-04-06 19:20:53.713696 git_limiter-0.1.1/git_limiter/terminal/__pycache__/base.cpython-39.pyc
+-rw-r--r--   0        0        0      698 2023-04-08 10:31:57.641039 git_limiter-0.1.1/git_limiter/terminal/__pycache__/rich_terminal.cpython-39.pyc
+-rw-r--r--   0        0        0      254 2023-04-06 19:17:07.276564 git_limiter-0.1.1/git_limiter/terminal/base.py
+-rw-r--r--   0        0        0      272 2023-04-08 10:30:56.496627 git_limiter-0.1.1/git_limiter/terminal/rich_terminal.py
+-rw-r--r--   0        0        0     1088 2023-04-08 16:27:05.565658 git_limiter-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      560 1970-01-01 00:00:00.000000 git_limiter-0.1.1/PKG-INFO
```

### Comparing `git_limiter-0.1.0/LICENSE.md` & `git_limiter-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `git_limiter-0.1.0/git_limiter/backend/__pycache__/base.cpython-39.pyc` & `git_limiter-0.1.1/git_limiter/backend/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `git_limiter-0.1.0/git_limiter/backend/__pycache__/git_subprocess_backend.cpython-39.pyc` & `git_limiter-0.1.1/git_limiter/backend/__pycache__/git_subprocess_backend.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Apr  8 07:55:08 2023 UTC, .py size: 1904 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 dc1d 3164 7007 0000  a.........1dp...
+00000000: 610d 0d0a 0000 0000 ed1e 3164 7207 0000  a.........1dr...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6400 6405 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 0100 6400  m.Z.m.Z.m.Z...d.
 00000070: 6406 6c0b 6d0c 5a0c 0100 6502 6500 6a0d  d.l.m.Z...e.e.j.
@@ -42,15 +42,15 @@
 00000290: 7365 7273 2f73 6572 6765 796b 6f6e 696b  sers/sergeykonik
 000002a0: 2f50 7963 6861 726d 5072 6f6a 6563 7473  /PycharmProjects
 000002b0: 2f64 6966 665f 6c69 6d69 742f 6769 745f  /diff_limit/git_
 000002c0: 6c69 6d69 7465 722f 6261 636b 656e 642f  limiter/backend/
 000002d0: 6769 745f 7375 6270 726f 6365 7373 5f62  git_subprocess_b
 000002e0: 6163 6b65 6e64 2e70 79da 1c5f 7275 6e5f  ackend.py.._run_
 000002f0: 6769 745f 6469 6666 5f76 6961 5f73 7562  git_diff_via_sub
-00000300: 7072 6f63 6573 7312 0000 0073 1200 0000  process....s....
+00000300: 7072 6f63 6573 7314 0000 0073 1200 0000  process....s....
 00000310: 0001 0402 0201 0201 0201 0601 02fb 0207  ................
 00000320: 02f8 7a31 4769 7453 7562 7072 6f63 6573  ..z1GitSubproces
 00000330: 7342 6163 6b65 6e64 2e5f 7275 6e5f 6769  sBackend._run_gi
 00000340: 745f 6469 6666 5f76 6961 5f73 7562 7072  t_diff_via_subpr
 00000350: 6f63 6573 7329 02da 1570 726f 6365 7373  ocess)...process
 00000360: 5f69 6e76 6f6b 655f 7265 7375 6c74 720a  _invoke_resultr.
 00000370: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
@@ -77,39 +77,39 @@
 000004c0: 00da 0570 6172 7365 7207 0000 0072 0600  ...parser....r..
 000004d0: 0000 7208 0000 0029 0772 1200 0000 7216  ..r....).r....r.
 000004e0: 0000 005a 0f67 6974 5f64 6966 665f 6f75  ...Z.git_diff_ou
 000004f0: 7470 7574 7218 0000 0072 1900 0000 721a  tputr....r....r.
 00000500: 0000 00da 0a64 6966 665f 7374 6174 7372  .....diff_statsr
 00000510: 1300 0000 7213 0000 0072 1400 0000 da11  ....r....r......
 00000520: 5f70 6172 7365 5f64 6966 665f 7374 6174  _parse_diff_stat
-00000530: 731e 0000 0073 1800 0000 0002 0c01 0a02  s....s..........
+00000530: 7320 0000 0073 1800 0000 0002 0c01 0a02  s ...s..........
 00000540: 0c02 0c01 0c01 0c02 0201 0201 0201 02fd  ................
 00000550: 0606 7a26 4769 7453 7562 7072 6f63 6573  ..z&GitSubproces
 00000560: 7342 6163 6b65 6e64 2e5f 7061 7273 655f  sBackend._parse_
 00000570: 6469 6666 5f73 7461 7473 6301 0000 0000  diff_statsc.....
 00000580: 0000 0000 0000 0003 0000 0003 0000 0043  ...............C
 00000590: 0000 0073 1800 0000 7c00 a000 a100 7d01  ...s....|.....}.
 000005a0: 7c00 6a01 7c01 6401 8d01 7d02 7c02 5300  |.j.|.d...}.|.S.
 000005b0: 2902 7a2b 496e 766f 6b65 2067 6974 2069  ).z+Invoke git i
 000005c0: 6e20 7375 6270 726f 6365 7373 2061 6e64  n subprocess and
 000005d0: 2063 6f6c 6c65 6374 2073 7461 7473 2e29   collect stats.)
 000005e0: 0172 1600 0000 2902 7215 0000 0072 2300  .r....).r....r#.
 000005f0: 0000 2903 7212 0000 0072 1600 0000 7222  ..).r....r....r"
 00000600: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-00000610: 0000 7222 0000 0031 0000 0073 0600 0000  ..r"...1...s....
+00000610: 0000 7222 0000 0033 0000 0073 0600 0000  ..r"...3...s....
 00000620: 0002 0801 0c02 7a1f 4769 7453 7562 7072  ......z.GitSubpr
 00000630: 6f63 6573 7342 6163 6b65 6e64 2e64 6966  ocessBackend.dif
 00000640: 665f 7374 6174 734e 2909 da08 5f5f 6e61  f_statsN)...__na
 00000650: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
 00000660: da0c 5f5f 7175 616c 6e61 6d65 5f5f da07  ..__qualname__..
 00000670: 5f5f 646f 635f 5fda 1350 726f 6365 7373  __doc__..Process
 00000680: 496e 766f 6b65 5265 7375 6c74 7215 0000  InvokeResultr...
 00000690: 0072 0800 0000 7223 0000 0072 2200 0000  .r....r#...r"...
 000006a0: 7213 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
-000006b0: 1400 0000 7209 0000 000f 0000 0073 0800  ....r........s..
+000006b0: 1400 0000 7209 0000 0011 0000 0073 0800  ....r........s..
 000006c0: 0000 0801 0402 0e0c 1013 7209 0000 0029  ..........r....)
 000006d0: 1272 0e00 0000 da06 7479 7069 6e67 7202  .r......typingr.
 000006e0: 0000 00da 0b67 6974 5f6c 696d 6974 6572  .....git_limiter
 000006f0: 7203 0000 00da 1867 6974 5f6c 696d 6974  r......git_limit
 00000700: 6572 2e62 6163 6b65 6e64 2e62 6173 6572  er.backend.baser
 00000710: 0400 0000 5a1c 6769 745f 6c69 6d69 7465  ....Z.git_limite
 00000720: 722e 7061 7273 6572 732e 6d61 785f 6469  r.parsers.max_di
@@ -118,8 +118,8 @@
 00000750: 7461 7473 7208 0000 00da 1043 6f6d 706c  tatsr......Compl
 00000760: 6574 6564 5072 6f63 6573 73da 1243 616c  etedProcess..Cal
 00000770: 6c65 6450 726f 6365 7373 4572 726f 7272  ledProcessErrorr
 00000780: 2800 0000 5a0c 5a45 524f 5f43 4841 4e47  (...Z.ZERO_CHANG
 00000790: 4553 7209 0000 0072 1300 0000 7213 0000  ESr....r....r...
 000007a0: 0072 1300 0000 7214 0000 00da 083c 6d6f  .r....r......<mo
 000007b0: 6475 6c65 3e01 0000 0073 1000 0000 0801  dule>....s......
-000007c0: 0c02 0c01 0c02 1401 0c02 1002 0403       ..............
+000007c0: 0c02 0c01 0c03 1401 0c03 1002 0403       ..............
```

### Comparing `git_limiter-0.1.0/git_limiter/backend/base.py` & `git_limiter-0.1.1/git_limiter/backend/base.py`

 * *Files identical despite different names*

### Comparing `git_limiter-0.1.0/git_limiter/backend/git_subprocess_backend.py` & `git_limiter-0.1.1/git_limiter/backend/git_subprocess_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import subprocess
 from typing import Union
 
 from git_limiter import constants
 from git_limiter.backend.base import GitBackend
-
-# Typing Aliases
 from git_limiter.parsers.max_diff import changed_files_parser, deletions_parser, insertions_parser
 from git_limiter.stats import DiffStats
 
 
 ProcessInvokeResult = Union[subprocess.CompletedProcess, subprocess.CalledProcessError]
 
 ZERO_CHANGES = 0
```

### Comparing `git_limiter-0.1.0/git_limiter/checks/__pycache__/base.cpython-39.pyc` & `git_limiter-0.1.1/git_limiter/checks/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `git_limiter-0.1.0/git_limiter/checks/base.py` & `git_limiter-0.1.1/git_limiter/checks/base.py`

 * *Files identical despite different names*

### Comparing `git_limiter-0.1.0/git_limiter/cli.py` & `git_limiter-0.1.1/git_limiter/cli.py`

 * *Files identical despite different names*

### Comparing `git_limiter-0.1.0/git_limiter/config/__pycache__/settings.cpython-39.pyc` & `git_limiter-0.1.1/git_limiter/config/__pycache__/settings.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Apr  8 07:08:14 2023 UTC, .py size: 1758 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,142 +1,141 @@
-00000000: 610d 0d0a 0000 0000 de12 3164 de06 0000  a.........1d....
+00000000: 610d 0d0a 0000 0000 4e1f 3164 d906 0000  a.......N.1d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 7200 0000 6400  .....@...sr...d.
+00000020: 0004 0000 0040 0000 0073 6e00 0000 6400  .....@...sn...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6401 6c08 5a08 6500 6a09 4700 6405 6406  d.l.Z.e.j.G.d.d.
-00000070: 8400 6406 8302 8301 5a0a 4700 6407 6408  ..d.....Z.G.d.d.
-00000080: 8400 6408 8302 5a0b 6500 6a09 4700 6409  ..d...Z.e.j.G.d.
-00000090: 640a 8400 640a 8302 8301 5a0c 6401 5300  d...d.....Z.d.S.
-000000a0: 290b e900 0000 004e 2901 da04 5061 7468  )......N)...Path
-000000b0: 2902 da04 4469 6374 da08 4f70 7469 6f6e  )...Dict..Option
-000000c0: 616c 2901 da09 636f 6e73 7461 6e74 7363  al)...constantsc
-000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000000e0: 0300 0000 4000 0000 734e 0000 0065 005a  ....@...sN...e.Z
-000000f0: 0164 005a 0255 0064 015a 0365 0465 0519  .d.Z.U.d.Z.e.e..
-00000100: 0065 0664 023c 0064 015a 0765 0465 0819  .e.d.<.d.Z.e.e..
-00000110: 0065 0664 033c 0064 015a 0965 0465 0819  .e.d.<.d.Z.e.e..
-00000120: 0065 0664 043c 0064 015a 0a65 0465 0819  .e.d.<.d.Z.e.e..
-00000130: 0065 0664 053c 0064 0153 0029 06da 1550  .e.d.<.d.S.)...P
-00000140: 7950 726f 6a65 6374 546f 6f6c 5365 7474  yProjectToolSett
-00000150: 696e 6773 4eda 0f63 6f6d 7061 7265 645f  ingsN..compared_
-00000160: 6272 616e 6368 da11 6d61 785f 6368 616e  branch..max_chan
-00000170: 6765 645f 6669 6c65 73da 0e6d 6178 5f69  ged_files..max_i
-00000180: 6e73 6572 7469 6f6e 73da 0d6d 6178 5f64  nsertions..max_d
-00000190: 656c 6574 696f 6e73 290b da08 5f5f 6e61  eletions)...__na
-000001a0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000001b0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7207  ..__qualname__r.
-000001c0: 0000 0072 0400 0000 da03 7374 72da 0f5f  ...r......str.._
-000001d0: 5f61 6e6e 6f74 6174 696f 6e73 5f5f 7208  _annotations__r.
-000001e0: 0000 00da 0369 6e74 7209 0000 0072 0a00  .....intr....r..
-000001f0: 0000 a900 7211 0000 0072 1100 0000 fa4c  ....r....r.....L
-00000200: 2f55 7365 7273 2f73 6572 6765 796b 6f6e  /Users/sergeykon
-00000210: 696b 2f50 7963 6861 726d 5072 6f6a 6563  ik/PycharmProjec
-00000220: 7473 2f64 6966 665f 6c69 6d69 742f 6769  ts/diff_limit/gi
-00000230: 745f 6c69 6d69 7465 722f 636f 6e66 6967  t_limiter/config
-00000240: 2f73 6574 7469 6e67 732e 7079 7206 0000  /settings.pyr...
-00000250: 0009 0000 0073 0800 0000 0a02 1001 1001  .....s..........
-00000260: 1001 7206 0000 0063 0000 0000 0000 0000  ..r....c........
-00000270: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000280: 732e 0000 0065 005a 0164 005a 0264 015a  s....e.Z.d.Z.d.Z
-00000290: 0365 0464 0264 039c 0264 0464 0584 045a  .e.d.d...d.d...Z
-000002a0: 0565 0664 069c 0164 0764 0884 045a 0764  .e.d...d.d...Z.d
-000002b0: 0253 0029 09da 0f50 7950 726f 6a65 6374  .S.)...PyProject
-000002c0: 5265 6164 6572 7a0b 6769 742d 6c69 6d69  Readerz.git-limi
-000002d0: 7465 724e 2902 da07 636f 6e74 656e 74da  terN)...content.
-000002e0: 0672 6574 7572 6e63 0200 0000 0000 0000  .returnc........
-000002f0: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-00000300: 730a 0000 007c 017c 005f 0064 0053 0029  s....|.|._.d.S.)
-00000310: 014e a901 7214 0000 0029 02da 0473 656c  .N..r....)...sel
-00000320: 6672 1400 0000 7211 0000 0072 1100 0000  fr....r....r....
-00000330: 7212 0000 00da 085f 5f69 6e69 745f 5f14  r......__init__.
-00000340: 0000 0073 0200 0000 0001 7a18 5079 5072  ...s......z.PyPr
-00000350: 6f6a 6563 7452 6561 6465 722e 5f5f 696e  ojectReader.__in
-00000360: 6974 5f5f 2901 7215 0000 0063 0100 0000  it__).r....c....
-00000370: 0000 0000 0000 0000 0800 0000 0500 0000  ................
-00000380: 4300 0000 735c 0000 0074 00a0 017c 006a  C...s\...t...|.j
-00000390: 02a1 017d 017c 01a0 0364 01a1 017d 027c  ...}.|...d...}.|
-000003a0: 02a0 037c 006a 0469 00a1 027d 0369 007d  ...|.j.i...}.i.}
-000003b0: 047c 03a0 05a1 0044 005d 1c5c 027d 057d  .|.....D.].\.}.}
-000003c0: 067c 05a0 0664 0264 03a1 027d 077c 067c  .|...d.d...}.|.|
-000003d0: 047c 073c 0071 3074 0766 0069 007c 04a4  .|.<.q0t.f.i.|..
-000003e0: 018e 0153 0029 044e da04 746f 6f6c da01  ...S.).N..tool..
-000003f0: 2dda 015f 2908 da05 746f 6d6c 69da 056c  -.._)...tomli..l
-00000400: 6f61 6473 7214 0000 00da 0367 6574 da09  oadsr......get..
-00000410: 4e41 4d45 5350 4143 45da 0569 7465 6d73  NAMESPACE..items
-00000420: da07 7265 706c 6163 6572 0600 0000 2908  ..replacer....).
-00000430: 7217 0000 005a 0974 6f6d 6c5f 6469 6374  r....Z.toml_dict
-00000440: 5a05 746f 6f6c 735a 1467 6974 5f6c 696d  Z.toolsZ.git_lim
-00000450: 6974 6572 5f73 6574 7469 6e67 735a 1c67  iter_settingsZ.g
-00000460: 6974 5f6c 696d 6974 6572 5f73 6574 7469  it_limiter_setti
-00000470: 6e67 735f 636c 6561 6e65 64da 036b 6579  ngs_cleaned..key
-00000480: da05 7661 6c75 655a 0e73 6e61 6b65 5f63  ..valueZ.snake_c
-00000490: 6173 655f 6b65 7972 1100 0000 7211 0000  ase_keyr....r...
-000004a0: 0072 1200 0000 da04 7265 6164 1700 0000  .r......read....
-000004b0: 7310 0000 0000 010c 010a 010e 0204 0110  s...............
-000004c0: 010c 010a 027a 1450 7950 726f 6a65 6374  .....z.PyProject
-000004d0: 5265 6164 6572 2e72 6561 6429 0872 0b00  Reader.read).r..
-000004e0: 0000 720c 0000 0072 0d00 0000 721f 0000  ..r....r....r...
-000004f0: 0072 0e00 0000 7218 0000 0072 0600 0000  .r....r....r....
-00000500: 7224 0000 0072 1100 0000 7211 0000 0072  r$...r....r....r
-00000510: 1100 0000 7212 0000 0072 1300 0000 1100  ....r....r......
-00000520: 0000 7306 0000 0008 0104 0210 0372 1300  ..s..........r..
-00000530: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
-00000540: 0000 0003 0000 0040 0000 0073 5800 0000  .......@...sX...
-00000550: 6500 5a01 6400 5a02 5500 6503 6a04 5a05  e.Z.d.Z.U.e.j.Z.
-00000560: 6506 6507 6401 3c00 6503 6a08 5a09 650a  e.e.d.<.e.j.Z.e.
-00000570: 6507 6402 3c00 6503 6a0b 5a0c 650a 6507  e.d.<.e.j.Z.e.e.
-00000580: 6403 3c00 6503 6a0d 5a0e 650a 6507 6404  d.<.e.j.Z.e.e.d.
-00000590: 3c00 650f 6506 1900 6405 9c01 6406 6407  <.e.e...d...d.d.
-000005a0: 8404 5a10 6408 5300 2909 da08 5365 7474  ..Z.d.S.)...Sett
-000005b0: 696e 6773 7207 0000 0072 0800 0000 7209  ingsr....r....r.
-000005c0: 0000 0072 0a00 0000 2901 da0b 636f 6e66  ...r....)...conf
-000005d0: 6967 5f70 6174 6863 0200 0000 0000 0000  ig_pathc........
-000005e0: 0000 0000 0800 0000 0500 0000 4300 0000  ............C...
-000005f0: 7364 0000 007c 0164 0075 0072 0c64 0053  sd...|.d.u.r.d.S
-00000600: 0074 007c 0183 017d 027c 02a0 01a1 007d  .t.|...}.|.....}
-00000610: 0374 027c 0364 018d 017d 047c 04a0 03a1  .t.|.d...}.|....
-00000620: 007d 057c 056a 04a0 05a1 0044 005d 265c  .}.|.j.....D.]&\
-00000630: 027d 067d 077c 0764 0075 0172 3874 067c  .}.}.|.d.u.r8t.|
-00000640: 007c 0683 0272 3874 077c 007c 067c 0783  .|...r8t.|.|.|..
-00000650: 0301 0071 3864 0053 0029 024e 7216 0000  ...q8d.S.).Nr...
-00000660: 0029 0872 0200 0000 da09 7265 6164 5f74  .).r......read_t
-00000670: 6578 7472 1300 0000 7224 0000 00da 085f  extr....r$....._
-00000680: 5f64 6963 745f 5f72 2000 0000 da07 6861  _dict__r .....ha
-00000690: 7361 7474 72da 0773 6574 6174 7472 2908  sattr..setattr).
-000006a0: 7217 0000 0072 2600 0000 da0b 636f 6e66  r....r&.....conf
-000006b0: 6967 5f66 696c 655a 1170 7970 726f 6a65  ig_fileZ.pyproje
-000006c0: 6374 5f63 6f6e 7465 6e74 da10 7079 7072  ct_content..pypr
-000006d0: 6f6a 6563 745f 7265 6164 6572 5a12 7079  oject_readerZ.py
-000006e0: 7072 6f6a 6563 745f 7365 7474 696e 6773  project_settings
-000006f0: da09 6174 7472 5f6e 616d 6572 2300 0000  ..attr_namer#...
-00000700: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00000710: 196f 7665 7272 6964 655f 6672 6f6d 5f63  .override_from_c
-00000720: 6f6e 6669 675f 6669 6c65 2b00 0000 7312  onfig_file+...s.
-00000730: 0000 0000 0108 0104 0208 0208 010a 0108  ................
-00000740: 0212 0112 017a 2253 6574 7469 6e67 732e  .....z"Settings.
-00000750: 6f76 6572 7269 6465 5f66 726f 6d5f 636f  override_from_co
-00000760: 6e66 6967 5f66 696c 654e 2911 720b 0000  nfig_fileN).r...
-00000770: 0072 0c00 0000 720d 0000 0072 0500 0000  .r....r....r....
-00000780: da17 4445 4641 554c 545f 434f 4d50 4152  ..DEFAULT_COMPAR
-00000790: 4544 5f42 5241 4e43 4872 0700 0000 720e  ED_BRANCHr....r.
-000007a0: 0000 0072 0f00 0000 da19 4445 4641 554c  ...r......DEFAUL
-000007b0: 545f 4d41 585f 4348 414e 4745 445f 4649  T_MAX_CHANGED_FI
-000007c0: 4c45 5372 0800 0000 7210 0000 00da 1644  LESr....r......D
-000007d0: 4546 4155 4c54 5f4d 4158 5f49 4e53 4552  EFAULT_MAX_INSER
-000007e0: 5449 4f4e 5372 0900 0000 da15 4445 4641  TIONSr......DEFA
-000007f0: 554c 545f 4d41 585f 4445 4c45 5449 4f4e  ULT_MAX_DELETION
-00000800: 5372 0a00 0000 7204 0000 0072 2e00 0000  Sr....r....r....
-00000810: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
-00000820: 1200 0000 7225 0000 0024 0000 0073 0a00  ....r%...$...s..
-00000830: 0000 0a02 0e01 0e01 0e01 0e02 7225 0000  ............r%..
-00000840: 0029 0dda 0b64 6174 6163 6c61 7373 6573  .)...dataclasses
-00000850: da07 7061 7468 6c69 6272 0200 0000 da06  ..pathlibr......
-00000860: 7479 7069 6e67 7203 0000 0072 0400 0000  typingr....r....
-00000870: da0b 6769 745f 6c69 6d69 7465 7272 0500  ..git_limiterr..
-00000880: 0000 721c 0000 00da 0964 6174 6163 6c61  ..r......datacla
-00000890: 7373 7206 0000 0072 1300 0000 7225 0000  ssr....r....r%..
-000008a0: 0072 1100 0000 7211 0000 0072 1100 0000  .r....r....r....
-000008b0: 7212 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000008c0: 0000 0073 1200 0000 0801 0c01 1002 0c01  ...s............
-000008d0: 0803 0401 1007 0e13 0401                 ..........
+00000040: 0100 6400 6403 6c03 6d04 5a04 0100 6400  ..d.d.l.m.Z...d.
+00000050: 6401 6c05 5a05 6400 6404 6c06 6d07 5a07  d.l.Z.d.d.l.m.Z.
+00000060: 0100 6500 6a08 4700 6405 6406 8400 6406  ..e.j.G.d.d...d.
+00000070: 8302 8301 5a09 4700 6407 6408 8400 6408  ....Z.G.d.d...d.
+00000080: 8302 5a0a 6500 6a08 4700 6409 640a 8400  ..Z.e.j.G.d.d...
+00000090: 640a 8302 8301 5a0b 6401 5300 290b e900  d.....Z.d.S.)...
+000000a0: 0000 004e 2901 da04 5061 7468 2901 da08  ...N)...Path)...
+000000b0: 4f70 7469 6f6e 616c 2901 da09 636f 6e73  Optional)...cons
+000000c0: 7461 6e74 7363 0000 0000 0000 0000 0000  tantsc..........
+000000d0: 0000 0000 0000 0300 0000 4000 0000 734e  ..........@...sN
+000000e0: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
+000000f0: 0365 0465 0519 0065 0664 023c 0064 015a  .e.e...e.d.<.d.Z
+00000100: 0765 0465 0819 0065 0664 033c 0064 015a  .e.e...e.d.<.d.Z
+00000110: 0965 0465 0819 0065 0664 043c 0064 015a  .e.e...e.d.<.d.Z
+00000120: 0a65 0465 0819 0065 0664 053c 0064 0153  .e.e...e.d.<.d.S
+00000130: 0029 06da 1550 7950 726f 6a65 6374 546f  .)...PyProjectTo
+00000140: 6f6c 5365 7474 696e 6773 4eda 0f63 6f6d  olSettingsN..com
+00000150: 7061 7265 645f 6272 616e 6368 da11 6d61  pared_branch..ma
+00000160: 785f 6368 616e 6765 645f 6669 6c65 73da  x_changed_files.
+00000170: 0e6d 6178 5f69 6e73 6572 7469 6f6e 73da  .max_insertions.
+00000180: 0d6d 6178 5f64 656c 6574 696f 6e73 290b  .max_deletions).
+00000190: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+000001a0: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+000001b0: 6d65 5f5f 7206 0000 0072 0300 0000 da03  me__r....r......
+000001c0: 7374 72da 0f5f 5f61 6e6e 6f74 6174 696f  str..__annotatio
+000001d0: 6e73 5f5f 7207 0000 00da 0369 6e74 7208  ns__r......intr.
+000001e0: 0000 0072 0900 0000 a900 7210 0000 0072  ...r......r....r
+000001f0: 1000 0000 fa4c 2f55 7365 7273 2f73 6572  .....L/Users/ser
+00000200: 6765 796b 6f6e 696b 2f50 7963 6861 726d  geykonik/Pycharm
+00000210: 5072 6f6a 6563 7473 2f64 6966 665f 6c69  Projects/diff_li
+00000220: 6d69 742f 6769 745f 6c69 6d69 7465 722f  mit/git_limiter/
+00000230: 636f 6e66 6967 2f73 6574 7469 6e67 732e  config/settings.
+00000240: 7079 7205 0000 000a 0000 0073 0800 0000  pyr........s....
+00000250: 0a02 1001 1001 1001 7205 0000 0063 0000  ........r....c..
+00000260: 0000 0000 0000 0000 0000 0000 0000 0300  ................
+00000270: 0000 4000 0000 732e 0000 0065 005a 0164  ..@...s....e.Z.d
+00000280: 005a 0264 015a 0365 0464 0264 039c 0264  .Z.d.Z.e.d.d...d
+00000290: 0464 0584 045a 0565 0664 069c 0164 0764  .d...Z.e.d...d.d
+000002a0: 0884 045a 0764 0253 0029 09da 0f50 7950  ...Z.d.S.)...PyP
+000002b0: 726f 6a65 6374 5265 6164 6572 7a0b 6769  rojectReaderz.gi
+000002c0: 742d 6c69 6d69 7465 724e 2902 da07 636f  t-limiterN)...co
+000002d0: 6e74 656e 74da 0672 6574 7572 6e63 0200  ntent..returnc..
+000002e0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+000002f0: 0000 4300 0000 730a 0000 007c 017c 005f  ..C...s....|.|._
+00000300: 0064 0053 0029 014e a901 7213 0000 0029  .d.S.).N..r....)
+00000310: 02da 0473 656c 6672 1300 0000 7210 0000  ...selfr....r...
+00000320: 0072 1000 0000 7211 0000 00da 085f 5f69  .r....r......__i
+00000330: 6e69 745f 5f15 0000 0073 0200 0000 0001  nit__....s......
+00000340: 7a18 5079 5072 6f6a 6563 7452 6561 6465  z.PyProjectReade
+00000350: 722e 5f5f 696e 6974 5f5f 2901 7214 0000  r.__init__).r...
+00000360: 0063 0100 0000 0000 0000 0000 0000 0800  .c..............
+00000370: 0000 0500 0000 4300 0000 735c 0000 0074  ......C...s\...t
+00000380: 00a0 017c 006a 02a1 017d 017c 01a0 0364  ...|.j...}.|...d
+00000390: 01a1 017d 027c 02a0 037c 006a 0469 00a1  ...}.|...|.j.i..
+000003a0: 027d 0369 007d 047c 03a0 05a1 0044 005d  .}.i.}.|.....D.]
+000003b0: 1c5c 027d 057d 067c 05a0 0664 0264 03a1  .\.}.}.|...d.d..
+000003c0: 027d 077c 067c 047c 073c 0071 3074 0766  .}.|.|.|.<.q0t.f
+000003d0: 0069 007c 04a4 018e 0153 0029 044e da04  .i.|.....S.).N..
+000003e0: 746f 6f6c da01 2dda 015f 2908 da05 746f  tool..-.._)...to
+000003f0: 6d6c 69da 056c 6f61 6473 7213 0000 00da  mli..loadsr.....
+00000400: 0367 6574 da09 4e41 4d45 5350 4143 45da  .get..NAMESPACE.
+00000410: 0569 7465 6d73 da07 7265 706c 6163 6572  .items..replacer
+00000420: 0500 0000 2908 7216 0000 005a 0974 6f6d  ....).r....Z.tom
+00000430: 6c5f 6469 6374 5a05 746f 6f6c 735a 1467  l_dictZ.toolsZ.g
+00000440: 6974 5f6c 696d 6974 6572 5f73 6574 7469  it_limiter_setti
+00000450: 6e67 735a 1c67 6974 5f6c 696d 6974 6572  ngsZ.git_limiter
+00000460: 5f73 6574 7469 6e67 735f 636c 6561 6e65  _settings_cleane
+00000470: 64da 036b 6579 da05 7661 6c75 655a 0e73  d..key..valueZ.s
+00000480: 6e61 6b65 5f63 6173 655f 6b65 7972 1000  nake_case_keyr..
+00000490: 0000 7210 0000 0072 1100 0000 da04 7265  ..r....r......re
+000004a0: 6164 1800 0000 7310 0000 0000 010c 010a  ad....s.........
+000004b0: 010e 0204 0110 010c 010a 027a 1450 7950  ...........z.PyP
+000004c0: 726f 6a65 6374 5265 6164 6572 2e72 6561  rojectReader.rea
+000004d0: 6429 0872 0a00 0000 720b 0000 0072 0c00  d).r....r....r..
+000004e0: 0000 721e 0000 0072 0d00 0000 7217 0000  ..r....r....r...
+000004f0: 0072 0500 0000 7223 0000 0072 1000 0000  .r....r#...r....
+00000500: 7210 0000 0072 1000 0000 7211 0000 0072  r....r....r....r
+00000510: 1200 0000 1200 0000 7306 0000 0008 0104  ........s.......
+00000520: 0210 0372 1200 0000 6300 0000 0000 0000  ...r....c.......
+00000530: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000540: 0073 5800 0000 6500 5a01 6400 5a02 5500  .sX...e.Z.d.Z.U.
+00000550: 6503 6a04 5a05 6506 6507 6401 3c00 6503  e.j.Z.e.e.d.<.e.
+00000560: 6a08 5a09 650a 6507 6402 3c00 6503 6a0b  j.Z.e.e.d.<.e.j.
+00000570: 5a0c 650a 6507 6403 3c00 6503 6a0d 5a0e  Z.e.e.d.<.e.j.Z.
+00000580: 650a 6507 6404 3c00 650f 6506 1900 6405  e.e.d.<.e.e...d.
+00000590: 9c01 6406 6407 8404 5a10 6408 5300 2909  ..d.d...Z.d.S.).
+000005a0: da08 5365 7474 696e 6773 7206 0000 0072  ..Settingsr....r
+000005b0: 0700 0000 7208 0000 0072 0900 0000 2901  ....r....r....).
+000005c0: da0b 636f 6e66 6967 5f70 6174 6863 0200  ..config_pathc..
+000005d0: 0000 0000 0000 0000 0000 0800 0000 0500  ................
+000005e0: 0000 4300 0000 7364 0000 007c 0164 0075  ..C...sd...|.d.u
+000005f0: 0072 0c64 0053 0074 007c 0183 017d 027c  .r.d.S.t.|...}.|
+00000600: 02a0 01a1 007d 0374 027c 0364 018d 017d  .....}.t.|.d...}
+00000610: 047c 04a0 03a1 007d 057c 056a 04a0 05a1  .|.....}.|.j....
+00000620: 0044 005d 265c 027d 067d 077c 0764 0075  .D.]&\.}.}.|.d.u
+00000630: 0172 3874 067c 007c 0683 0272 3874 077c  .r8t.|.|...r8t.|
+00000640: 007c 067c 0783 0301 0071 3864 0053 0029  .|.|.....q8d.S.)
+00000650: 024e 7215 0000 0029 0872 0200 0000 da09  .Nr....).r......
+00000660: 7265 6164 5f74 6578 7472 1200 0000 7223  read_textr....r#
+00000670: 0000 00da 085f 5f64 6963 745f 5f72 1f00  .....__dict__r..
+00000680: 0000 da07 6861 7361 7474 72da 0773 6574  ....hasattr..set
+00000690: 6174 7472 2908 7216 0000 0072 2500 0000  attr).r....r%...
+000006a0: da0b 636f 6e66 6967 5f66 696c 655a 1170  ..config_fileZ.p
+000006b0: 7970 726f 6a65 6374 5f63 6f6e 7465 6e74  yproject_content
+000006c0: 5a10 7079 7072 6f6a 6563 745f 7265 6164  Z.pyproject_read
+000006d0: 6572 5a12 7079 7072 6f6a 6563 745f 7365  erZ.pyproject_se
+000006e0: 7474 696e 6773 da09 6174 7472 5f6e 616d  ttings..attr_nam
+000006f0: 6572 2200 0000 7210 0000 0072 1000 0000  er"...r....r....
+00000700: 7211 0000 00da 196f 7665 7272 6964 655f  r......override_
+00000710: 6672 6f6d 5f63 6f6e 6669 675f 6669 6c65  from_config_file
+00000720: 2c00 0000 7312 0000 0000 0108 0104 0208  ,...s...........
+00000730: 0208 010a 0108 0212 0112 017a 2253 6574  ...........z"Set
+00000740: 7469 6e67 732e 6f76 6572 7269 6465 5f66  tings.override_f
+00000750: 726f 6d5f 636f 6e66 6967 5f66 696c 654e  rom_config_fileN
+00000760: 2911 720a 0000 0072 0b00 0000 720c 0000  ).r....r....r...
+00000770: 0072 0400 0000 da17 4445 4641 554c 545f  .r......DEFAULT_
+00000780: 434f 4d50 4152 4544 5f42 5241 4e43 4872  COMPARED_BRANCHr
+00000790: 0600 0000 720d 0000 0072 0e00 0000 da19  ....r....r......
+000007a0: 4445 4641 554c 545f 4d41 585f 4348 414e  DEFAULT_MAX_CHAN
+000007b0: 4745 445f 4649 4c45 5372 0700 0000 720f  GED_FILESr....r.
+000007c0: 0000 00da 1644 4546 4155 4c54 5f4d 4158  .....DEFAULT_MAX
+000007d0: 5f49 4e53 4552 5449 4f4e 5372 0800 0000  _INSERTIONSr....
+000007e0: da15 4445 4641 554c 545f 4d41 585f 4445  ..DEFAULT_MAX_DE
+000007f0: 4c45 5449 4f4e 5372 0900 0000 7203 0000  LETIONSr....r...
+00000800: 0072 2c00 0000 7210 0000 0072 1000 0000  .r,...r....r....
+00000810: 7210 0000 0072 1100 0000 7224 0000 0025  r....r....r$...%
+00000820: 0000 0073 0a00 0000 0a02 0e01 0e01 0e01  ...s............
+00000830: 0e02 7224 0000 0029 0cda 0b64 6174 6163  ..r$...)...datac
+00000840: 6c61 7373 6573 da07 7061 7468 6c69 6272  lasses..pathlibr
+00000850: 0200 0000 da06 7479 7069 6e67 7203 0000  ......typingr...
+00000860: 0072 1b00 0000 da0b 6769 745f 6c69 6d69  .r......git_limi
+00000870: 7465 7272 0400 0000 da09 6461 7461 636c  terr......datacl
+00000880: 6173 7372 0500 0000 7212 0000 0072 2400  assr....r....r$.
+00000890: 0000 7210 0000 0072 1000 0000 7210 0000  ..r....r....r...
+000008a0: 0072 1100 0000 da08 3c6d 6f64 756c 653e  .r......<module>
+000008b0: 0100 0000 7312 0000 0008 010c 010c 0208  ....s...........
+000008c0: 020c 0304 0110 070e 1304 01              ...........
```

### Comparing `git_limiter-0.1.0/git_limiter/config/settings.py` & `git_limiter-0.1.1/git_limiter/config/settings.py`

 * *Files identical despite different names*

### Comparing `git_limiter-0.1.0/git_limiter/parsers/__pycache__/base.cpython-39.pyc` & `git_limiter-0.1.1/git_limiter/parsers/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `git_limiter-0.1.0/git_limiter/parsers/__pycache__/max_diff.cpython-39.pyc` & `git_limiter-0.1.1/git_limiter/parsers/__pycache__/max_diff.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `git_limiter-0.1.0/git_limiter/parsers/base.py` & `git_limiter-0.1.1/git_limiter/parsers/base.py`

 * *Files identical despite different names*

### Comparing `git_limiter-0.1.0/git_limiter/parsers/max_diff.py` & `git_limiter-0.1.1/git_limiter/parsers/max_diff.py`

 * *Files identical despite different names*

### Comparing `git_limiter-0.1.0/git_limiter/stats.py` & `git_limiter-0.1.1/git_limiter/stats.py`

 * *Files identical despite different names*

### Comparing `git_limiter-0.1.0/git_limiter/terminal/__pycache__/base.cpython-39.pyc` & `git_limiter-0.1.1/git_limiter/terminal/__pycache__/base.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `git_limiter-0.1.0/git_limiter/terminal/__pycache__/rich_terminal.cpython-39.pyc` & `git_limiter-0.1.1/git_limiter/terminal/__pycache__/rich_terminal.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Apr  8 04:56:43 2023 UTC, .py size: 272 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 0bf4 3064 1001 0000  a.........0d....
+00000000: 610d 0d0a 0000 0000 6042 3164 1001 0000  a.......`B1d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3e00 0000 6400  .....@...s>...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6503 8300 5a06 4700 6404 6405 8400  ..e...Z.G.d.d...
 00000060: 6405 6505 8303 5a07 6406 5300 2907 e900  d.e...Z.d.S.)...
 00000070: 0000 0029 01da 084f 7074 696f 6e61 6c29  ...)...Optional)
```

### Comparing `git_limiter-0.1.0/pyproject.toml` & `git_limiter-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "git-limiter"
-version = "0.1.0"
+version = "0.1.1"
 description = "Tool allowing to prevent commiting huge diffs"
 authors = ["Sergei Konik <s.konik.dev@gmail.com>"]
 packages = [{include = "git_limiter"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "^8.1.3"
```

### Comparing `git_limiter-0.1.0/PKG-INFO` & `git_limiter-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-limiter
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tool allowing to prevent commiting huge diffs
 Author: Sergei Konik
 Author-email: s.konik.dev@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

