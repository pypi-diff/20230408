# Comparing `tmp/ntlog-0.0.tar.gz` & `tmp/ntlog-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntlog-0.0.tar", last modified: Fri Apr  7 22:10:38 2023, max compression
+gzip compressed data, was "ntlog-0.1.tar", last modified: Sat Apr  8 07:37:18 2023, max compression
```

## Comparing `ntlog-0.0.tar` & `ntlog-0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2834 2023-04-07 22:09:24.716096 ntlog-0.0/README.rst
--rw-r--r--   0        0        0        0 2023-04-07 19:25:16.421568 ntlog-0.0/ntlog/__init__.py
--rwxr-xr-x   0        0        0     3424 2023-04-07 21:44:31.921572 ntlog-0.0/ntlog/main.py
--rw-r--r--   0        0        0      451 2023-04-07 22:04:58.578288 ntlog-0.0/pyproject.toml
--rw-r--r--   0        0        0     3151 1970-01-01 00:00:00.000000 ntlog-0.0/PKG-INFO
+-rw-r--r--   0        0        0     3212 2023-04-08 07:31:29.150131 ntlog-0.1/README.rst
+-rw-r--r--   0        0        0        0 2023-04-07 19:25:16.421568 ntlog-0.1/ntlog/__init__.py
+-rwxr-xr-x   0        0        0     3902 2023-04-08 07:31:29.149131 ntlog-0.1/ntlog/main.py
+-rw-r--r--   0        0        0     1113 2023-04-08 07:31:29.150131 ntlog-0.1/pyproject.toml
+-rw-r--r--   0        0        0     4187 1970-01-01 00:00:00.000000 ntlog-0.1/PKG-INFO
```

### Comparing `ntlog-0.0/README.rst` & `ntlog-0.1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-ntLog — Append a file into an running NestedText log
-====================================================
+ntLog — a NestedText logfile aggregation utility
+================================================
 
 .. image:: https://pepy.tech/badge/ntlog/month
     :target: https://pepy.tech/project/ntlog
 
 ..  image:: https://github.com/KenKundert/ntlog/actions/workflows/build.yaml/badge.svg
     :target: https://github.com/KenKundert/ntlog/actions/workflows/build.yaml
 
@@ -13,16 +13,16 @@
 .. image:: https://img.shields.io/pypi/v/ntlog.svg
     :target: https://pypi.python.org/pypi/ntlog
 
 .. image:: https://img.shields.io/pypi/pyversions/ntlog.svg
     :target: https://pypi.python.org/pypi/ntlog/
 
 :Author: Ken Kundert
-:Version: 0.0
-:Released: 2023-04-07
+:Version: 0.1
+:Released: 2023-04-08
 
 *ntLog* is a simple command line utility used to append discretely generated log 
 files into a running log formulated as a `NestedText <nestedtext.org>`_ file.  
 You can specify limits on how many log entries there are or how old they should 
 be.  Any entries that do not satisfy the limits are purged.
 
 A discrete log file is a log file generated by program that runs at regular 
@@ -43,27 +43,38 @@
         -k, --keep-for [days]    drop entries older than this [default: 7]
         -n, --max-entries [N]    maximum number of log entries to keep
         -N, --min-entries [N]    minimum number of log entries to keep [default: 1]
         -d, --delete             delete given logfile after incorporating it
         -h, --help               print this usage message
 
 When run, *ntLog* copies the contents of ``<logfile>`` into ``<logfile>.nt``.
-Any log entries that are older than ``--keep-for`` days are deleted.  If the 
-number of entries exceeds ``--max-entries``, the oldest entries are deleted.
+
+Log entries older than ``--keep-for`` days are deleted.  If units are not 
+specified, ``--keep-for`` is given in days.  However you can directly specify 
+the units in terms of seconds (s, sec, second, seconds), minutes (m, min, 
+minute, minutes), hours (h, hr, hour, hours), days (d, day, days), weeks (w, W, 
+week, weeks), months (M, month, months), and years (y, Y, year, years).
+
+If the number of entries exceeds ``--max-entries``, the oldest entries are 
+deleted even if they are younger than the ``--keep-for`` limit.
+
 If ``--delete`` is specified, the given log file is deleted after its contents 
 are incorporated into the running log file.
 
 The key used when filing log entries into the *NestedText* document is the 
-timestamp for the modification time of the file.  The given logfile is always 
-kept, even if it is older than the specified limit.
+timestamp of the modification time of the given log file.
+
+The given log file is always kept, even if it is older than the ``--keep-for`` 
+limit.
 
 Log entries are sorted from most recent to oldest, with the most recent at the 
 top of the *NestedText* file.  The one exception to this rule is that the given 
 log file is always listed first, even if its modification time is older than 
 existing log entries.
 
+
 Installation
 ------------
 
 Install with::
 
     pip install ntlog
```

### Comparing `ntlog-0.0/ntlog/main.py` & `ntlog-0.1/ntlog/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,22 +11,23 @@
     -n, --max-entries [N]    maximum number of log entries to keep
     -N, --min-entries [N]    minimum number of log entries to keep [default: 1]
     -d, --delete             delete given logfile after incorporating it
 
 Copies <logfile> into <logfile>.nt while deleting any log entries that are older 
 than the limit specified by --keep-for.
 """
-__version__ = '0.0'
-__released__ = '2023-04-07'
+__version__ = '0.1'
+__released__ = '2023-04-08'
 
 
 # IMPORTS {{{1
 from docopt import docopt
 from inform import fatal, full_stop, os_error
 from pathlib import Path
+from quantiphy import Quantity, UnitConversion, QuantiPhyError
 import nestedtext as nt
 import arrow
 
 # UTILITIES {{{1
 # to_int() {{{2
 def to_int(number):
     try:
@@ -40,24 +41,34 @@
 
 # trim_dict() {{{2
 def trim_dict(d, max_entries):
     # trim the dictionary such that it contains only the max_entries most
     # recently added items
     return dict(list(d.items())[:max_entries])
 
+# TIME CONVERSIONS {{{1
+UnitConversion("s", "sec second seconds")
+UnitConversion("s", "m min minute minutes", 60)
+UnitConversion("s", "h hr hour hours", 60*60)
+UnitConversion("s", "d day days", 24*60*60)
+UnitConversion("s", "w W week weeks", 7*24*60*60)
+UnitConversion("s", "M month months", 30*24*60*60)
+UnitConversion("s", "y Y year years", 365*24*60*60)
+Quantity.set_prefs(ignore_sf=True)
+
 # MAIN {{{1
 def main():
     # Command line {{{2
     cmdline = docopt(__doc__)
     logfile = cmdline['<logfile>']
-    keep_for = cmdline['--keep-for']
+    keep_for = Quantity(cmdline['--keep-for'], 'd', scale='s')
     max_entries = to_int(cmdline['--max-entries'])
     min_entries = to_int(cmdline['--min-entries'])
     delete_given_log = cmdline['--delete']
-    oldest = arrow.now().shift(days=-float(keep_for))
+    oldest = arrow.now().shift(seconds=-keep_for)
 
     # Load the running log, append the logfile, and write it out again {{{2
     try:
         logfile = Path(logfile)
         running_logfile = logfile.with_suffix('.log.nt')
 
         # load running log
```
