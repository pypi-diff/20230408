# Comparing `tmp/pure-checker-2.0.tar.gz` & `tmp/pure-checker-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure-checker-2.0.tar", last modified: Mon Mar 13 13:32:23 2023, max compression
+gzip compressed data, was "pure-checker-2.1.tar", last modified: Fri Apr  7 23:24:29 2023, max compression
```

## Comparing `pure-checker-2.0.tar` & `pure-checker-2.1.tar`

### file list

```diff
@@ -1,241 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.224310 pure-checker-2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-13 13:32:15.000000 pure-checker-2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-03-13 13:32:15.000000 pure-checker-2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-13 13:32:15.000000 pure-checker-2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-03-13 13:32:23.224310 pure-checker-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-03-13 13:32:15.000000 pure-checker-2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.200310 pure-checker-2.0/include/
--rw-r--r--   0 runner    (1001) docker     (123)    60218 2023-03-13 13:32:15.000000 pure-checker-2.0/include/pure.h
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-03-13 13:32:15.000000 pure-checker-2.0/include/pure_constants.h
--rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-03-13 13:32:15.000000 pure-checker-2.0/include/pure_errors.h
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-03-13 13:32:15.000000 pure-checker-2.0/include/pure_routines.h
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-03-13 13:32:15.000000 pure-checker-2.0/include/pure_signatures.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.204310 pure-checker-2.0/include/zlib/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)    78553 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/FAQ
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/INDEX
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    13680 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/README
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/adler32.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.204310 pure-checker-2.0/include/zlib/amiga/
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/amiga/Makefile.pup
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/amiga/Makefile.sas
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/compress.c
--rwxr-xr-x   0 runner    (1001) docker     (123)    28244 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/configure
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.204310 pure-checker-2.0/include/zlib/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/README.contrib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.208310 pure-checker-2.0/include/zlib/contrib/ada/
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/ada/buffer_demo.adb
--rw-r--r--   0 runner    (1001) docker     (123)     4467 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/ada/mtest.adb
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/ada/read.adb
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/ada/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13180 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/ada/test.adb
--rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/ada/zlib-streams.adb
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/ada/zlib-streams.ads
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/ada/zlib-thin.adb
--rw-r--r--   0 runner    (1001) docker     (123)    15819 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/ada/zlib-thin.ads
--rw-r--r--   0 runner    (1001) docker     (123)    20400 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/ada/zlib.adb
--rw-r--r--   0 runner    (1001) docker     (123)    13594 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/ada/zlib.ads
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/ada/zlib.gpr
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.208310 pure-checker-2.0/include/zlib/contrib/amd64/
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/amd64/amd64-match.S
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.208310 pure-checker-2.0/include/zlib/contrib/asm686/
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/asm686/README.686
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/asm686/match.S
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.208310 pure-checker-2.0/include/zlib/contrib/blast/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/blast/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/blast/README
--rw-r--r--   0 runner    (1001) docker     (123)    18162 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/blast/blast.c
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/blast/blast.h
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/blast/test.pk
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/blast/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.208310 pure-checker-2.0/include/zlib/contrib/delphi/
--rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/delphi/ZLib.pas
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/delphi/ZLibConst.pas
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/delphi/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/delphi/zlibd32.mak
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.208310 pure-checker-2.0/include/zlib/contrib/gcc_gvmat64/
--rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/gcc_gvmat64/gvmat64.S
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.208310 pure-checker-2.0/include/zlib/contrib/infback9/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/infback9/README
--rw-r--r--   0 runner    (1001) docker     (123)    21629 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/infback9/infback9.c
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/infback9/infback9.h
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/infback9/inffix9.h
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/infback9/inflate9.h
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/infback9/inftree9.c
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/infback9/inftree9.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.208310 pure-checker-2.0/include/zlib/contrib/inflate86/
--rw-r--r--   0 runner    (1001) docker     (123)    40608 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/inflate86/inffas86.c
--rw-r--r--   0 runner    (1001) docker     (123)    42842 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/inflate86/inffast.S
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.208310 pure-checker-2.0/include/zlib/contrib/iostream/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/iostream/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/iostream/zfstream.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/iostream/zfstream.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.208310 pure-checker-2.0/include/zlib/contrib/iostream2/
--rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/iostream2/zstream.h
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/iostream2/zstream_test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.212310 pure-checker-2.0/include/zlib/contrib/iostream3/
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/iostream3/README
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/iostream3/TODO
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/iostream3/test.cc
--rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/iostream3/zfstream.cc
--rw-r--r--   0 runner    (1001) docker     (123)    12240 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/iostream3/zfstream.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.212310 pure-checker-2.0/include/zlib/contrib/masmx64/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/masmx64/bld_ml64.bat
--rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/masmx64/gvmat64.asm
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/masmx64/inffas8664.c
--rw-r--r--   0 runner    (1001) docker     (123)    10583 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/masmx64/inffasx64.asm
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/masmx64/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.212310 pure-checker-2.0/include/zlib/contrib/masmx86/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/masmx86/bld_ml32.bat
--rw-r--r--   0 runner    (1001) docker     (123)    16392 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/masmx86/inffas32.asm
--rw-r--r--   0 runner    (1001) docker     (123)    15825 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/masmx86/match686.asm
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/masmx86/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.212310 pure-checker-2.0/include/zlib/contrib/minizip/
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/MiniZip64_Changes.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/MiniZip64_info.txt
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/configure.ac
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/crypt.h
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/ioapi.c
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/ioapi.h
--rw-r--r--   0 runner    (1001) docker     (123)    14223 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/iowin32.c
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/iowin32.h
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/make_vms.com
--rw-r--r--   0 runner    (1001) docker     (123)    17763 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/miniunz.c
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/miniunzip.1
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/minizip.1
--rw-r--r--   0 runner    (1001) docker     (123)    15034 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/minizip.c
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/minizip.pc.in
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/mztools.c
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/mztools.h
--rw-r--r--   0 runner    (1001) docker     (123)    71055 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/unzip.c
--rw-r--r--   0 runner    (1001) docker     (123)    16352 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/unzip.h
--rw-r--r--   0 runner    (1001) docker     (123)    65842 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/zip.c
--rw-r--r--   0 runner    (1001) docker     (123)    15366 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/minizip/zip.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.216310 pure-checker-2.0/include/zlib/contrib/pascal/
--rw-r--r--   0 runner    (1001) docker     (123)    15687 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/pascal/example.pas
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/pascal/readme.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/pascal/zlibd32.mak
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/pascal/zlibpas.pas
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.216310 pure-checker-2.0/include/zlib/contrib/puff/
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/puff/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/puff/README
--rw-r--r--   0 runner    (1001) docker     (123)    37883 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/puff/puff.c
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/puff/puff.h
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/puff/pufftest.c
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/puff/zeros.raw
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.216310 pure-checker-2.0/include/zlib/contrib/testzlib/
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/testzlib/testzlib.c
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/testzlib/testzlib.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.216310 pure-checker-2.0/include/zlib/contrib/untgz/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/untgz/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/untgz/Makefile.msc
--rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/contrib/untgz/untgz.c
--rw-r--r--   0 runner    (1001) docker     (123)    14053 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/crc32.c
--rw-r--r--   0 runner    (1001) docker     (123)    30562 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/crc32.h
--rw-r--r--   0 runner    (1001) docker     (123)    78889 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/deflate.c
--rw-r--r--   0 runner    (1001) docker     (123)    13150 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/deflate.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.216310 pure-checker-2.0/include/zlib/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     9335 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/doc/algorithm.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20502 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/doc/rfc1950.txt
--rw-r--r--   0 runner    (1001) docker     (123)    36944 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/doc/rfc1951.txt
--rw-r--r--   0 runner    (1001) docker     (123)    25037 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/doc/rfc1952.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/doc/txtvsbin.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.216310 pure-checker-2.0/include/zlib/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/examples/README.examples
--rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/examples/enough.c
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/examples/fitblk.c
--rw-r--r--   0 runner    (1001) docker     (123)    25943 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/examples/gun.c
--rw-r--r--   0 runner    (1001) docker     (123)    16977 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/examples/gzappend.c
--rw-r--r--   0 runner    (1001) docker     (123)    14132 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/examples/gzjoin.c
--rw-r--r--   0 runner    (1001) docker     (123)    41479 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/examples/gzlog.c
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/examples/gzlog.h
--rw-r--r--   0 runner    (1001) docker     (123)    29824 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/examples/zlib_how.html
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/examples/zpipe.c
--rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/examples/zran.c
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/gzclose.c
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/gzguts.h
--rw-r--r--   0 runner    (1001) docker     (123)    16600 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/gzlib.c
--rw-r--r--   0 runner    (1001) docker     (123)    20430 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/gzread.c
--rw-r--r--   0 runner    (1001) docker     (123)    19256 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/gzwrite.c
--rw-r--r--   0 runner    (1001) docker     (123)    22715 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/infback.c
--rw-r--r--   0 runner    (1001) docker     (123)    12978 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/inffast.c
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/inffast.h
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/inffixed.h
--rw-r--r--   0 runner    (1001) docker     (123)    54800 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/inflate.c
--rw-r--r--   0 runner    (1001) docker     (123)     6618 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/inflate.h
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/inftrees.c
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/inftrees.h
--rw-r--r--   0 runner    (1001) docker     (123)    26402 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/make_vms.com
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.220310 pure-checker-2.0/include/zlib/msdos/
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/msdos/Makefile.bor
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/msdos/Makefile.dj2
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/msdos/Makefile.emx
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/msdos/Makefile.msc
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/msdos/Makefile.tc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.220310 pure-checker-2.0/include/zlib/nintendods/
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/nintendods/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/nintendods/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.220310 pure-checker-2.0/include/zlib/old/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/old/Makefile.emx
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/old/Makefile.riscos
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/old/README
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/old/descrip.mms
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.220310 pure-checker-2.0/include/zlib/old/os2/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/old/os2/Makefile.os2
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/old/os2/zlib.def
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/old/visual-basic.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.220310 pure-checker-2.0/include/zlib/os400/
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/os400/README400
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/os400/bndsrc
--rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/os400/make.sh
--rw-r--r--   0 runner    (1001) docker     (123)    32795 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/os400/zlib.inc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.220310 pure-checker-2.0/include/zlib/qnx/
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/qnx/package.qpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.220310 pure-checker-2.0/include/zlib/test/
--rw-r--r--   0 runner    (1001) docker     (123)    16888 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/test/example.c
--rw-r--r--   0 runner    (1001) docker     (123)    24723 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/test/infcover.c
--rw-r--r--   0 runner    (1001) docker     (123)    15797 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/test/minigzip.c
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/treebuild.xml
--rw-r--r--   0 runner    (1001) docker     (123)    43761 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/trees.c
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/trees.h
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/uncompr.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.220310 pure-checker-2.0/include/zlib/watcom/
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/watcom/watcom_f.mak
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/watcom/watcom_l.mak
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.220310 pure-checker-2.0/include/zlib/win32/
--rw-r--r--   0 runner    (1001) docker     (123)    17921 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/win32/DLL_FAQ.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/win32/Makefile.bor
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/win32/Makefile.gcc
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/win32/Makefile.msc
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/win32/README-WIN32.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/win32/VisualC.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/win32/zlib.def
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/win32/zlib1.rc
--rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/zconf.h
--rw-r--r--   0 runner    (1001) docker     (123)    16349 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/zconf.h.cmakein
--rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/zconf.h.in
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/zlib.3
--rw-r--r--   0 runner    (1001) docker     (123)    19318 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/zlib.3.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    96239 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/zlib.h
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/zlib.pc.cmakein
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/zlib.pc.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     3895 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/zlib2ansi
--rw-r--r--   0 runner    (1001) docker     (123)     7304 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/zutil.c
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-03-13 13:32:15.000000 pure-checker-2.0/include/zlib/zutil.h
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-03-13 13:32:15.000000 pure-checker-2.0/pure_checker.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.220310 pure-checker-2.0/pure_checker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-03-13 13:32:23.000000 pure-checker-2.0/pure_checker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-03-13 13:32:23.000000 pure-checker-2.0/pure_checker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 13:32:23.000000 pure-checker-2.0/pure_checker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-13 13:32:23.000000 pure-checker-2.0/pure_checker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-13 13:32:15.000000 pure-checker-2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 13:32:23.224310 pure-checker-2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-13 13:32:15.000000 pure-checker-2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 13:32:23.220310 pure-checker-2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-13 13:32:15.000000 pure-checker-2.0/tests/test_pure_py.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:24:29.152142 pure-checker-2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-07 23:24:21.000000 pure-checker-2.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-07 23:24:21.000000 pure-checker-2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-07 23:24:21.000000 pure-checker-2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-04-07 23:24:29.152142 pure-checker-2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-07 23:24:21.000000 pure-checker-2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:24:29.152142 pure-checker-2.1/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    60212 2023-04-07 23:24:21.000000 pure-checker-2.1/include/pure.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-04-07 23:24:21.000000 pure-checker-2.1/include/pure_constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20660 2023-04-07 23:24:21.000000 pure-checker-2.1/include/pure_errors.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-04-07 23:24:21.000000 pure-checker-2.1/include/pure_routines.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-07 23:24:21.000000 pure-checker-2.1/include/pure_signatures.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-07 23:24:21.000000 pure-checker-2.1/pure_checker.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:24:29.152142 pure-checker-2.1/pure_checker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11784 2023-04-07 23:24:29.000000 pure-checker-2.1/pure_checker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-07 23:24:29.000000 pure-checker-2.1/pure_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:24:29.000000 pure-checker-2.1/pure_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-07 23:24:29.000000 pure-checker-2.1/pure_checker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-07 23:24:21.000000 pure-checker-2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 23:24:29.152142 pure-checker-2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-07 23:24:21.000000 pure-checker-2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:24:29.152142 pure-checker-2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)   152397 2023-04-07 23:24:21.000000 pure-checker-2.1/tests/test_pure_py.py
```

### Comparing `pure-checker-2.0/LICENSE` & `pure-checker-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pure-checker-2.0/PKG-INFO` & `pure-checker-2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-checker
-Version: 2.0
+Version: 2.1
 Summary: A static analysis file format checker.
 Author: Joran Dirk Greef (Ronomon), Maxim Vainstein (Microsoft), Milind Solage (Microsoft), Patrik Vicol (Microsoft), Stacy Sheperson (Microsoft)
 Maintainer-email: Seb <me@sebjo.se>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 Ronomon CC
         
@@ -22,14 +22,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # @sebdroid/pure-checker
 [![Build](https://github.com/sebdroid/pure-checker/actions/workflows/build_wheels.yml/badge.svg)](https://github.com/sebdroid/pure-checker/actions/workflows/build_wheels.yml)
```

### Comparing `pure-checker-2.0/README.md` & `pure-checker-2.1/README.md`

 * *Files identical despite different names*

### Comparing `pure-checker-2.0/include/pure.h` & `pure-checker-2.1/include/pure.h`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,21 @@
 #define PURE_H
 
 #include <assert.h>
 #include <stdint.h>
 #include <stdlib.h>
 #include <string.h>
 #include <stdio.h>
+#include <zlib.h>
 
 #include "pure_constants.h"
 #include "pure_errors.h"
 #include "pure_signatures.h"
 #include "pure_routines.h"
 
-#include "zlib/zlib.h"
-
 typedef struct pure_ctx {
   uint64_t flags;
   uint64_t depth;
   uint64_t files;
   uint64_t archives;
   uint64_t size;
   uint64_t compressed_size;
```

### Comparing `pure-checker-2.0/include/pure_constants.h` & `pure-checker-2.1/include/pure_constants.h`

 * *Files identical despite different names*

### Comparing `pure-checker-2.0/include/pure_errors.h` & `pure-checker-2.1/include/pure_errors.h`

 * *Files identical despite different names*

### Comparing `pure-checker-2.0/include/pure_routines.h` & `pure-checker-2.1/include/pure_routines.h`

 * *Files identical despite different names*

### Comparing `pure-checker-2.0/include/pure_signatures.h` & `pure-checker-2.1/include/pure_signatures.h`

 * *Files identical despite different names*

### Comparing `pure-checker-2.0/pure_checker.c` & `pure-checker-2.1/pure_checker.c`

 * *Files identical despite different names*

### Comparing `pure-checker-2.0/pure_checker.egg-info/PKG-INFO` & `pure-checker-2.1/pure_checker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-checker
-Version: 2.0
+Version: 2.1
 Summary: A static analysis file format checker.
 Author: Joran Dirk Greef (Ronomon), Maxim Vainstein (Microsoft), Milind Solage (Microsoft), Patrik Vicol (Microsoft), Stacy Sheperson (Microsoft)
 Maintainer-email: Seb <me@sebjo.se>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 Ronomon CC
         
@@ -22,14 +22,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
 
 # @sebdroid/pure-checker
 [![Build](https://github.com/sebdroid/pure-checker/actions/workflows/build_wheels.yml/badge.svg)](https://github.com/sebdroid/pure-checker/actions/workflows/build_wheels.yml)
```

### Comparing `pure-checker-2.0/pyproject.toml` & `pure-checker-2.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 # pyproject.toml
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pure-checker"  # as it would appear on PyPI
-version = "2.0"
+version = "2.1"
+requires-python = ">=3.9"
 description = "A static analysis file format checker."
 readme = "README.md"
 authors = [
   {name = "Joran Dirk Greef (Ronomon)"},
   {name = "Maxim Vainstein (Microsoft)"},
   {name = "Milind Solage (Microsoft)"},
   {name = "Patrik Vicol (Microsoft)"},
   {name = "Stacy Sheperson (Microsoft)"},
 ]
 maintainers = [
   {name = "Seb", email = "me@sebjo.se"},
 ]
-license = {file = "LICENSE"}
+license = {file = "LICENSE"}
+
+[tool.cibuildwheel]
+test-requires = "pytest"
+skip = ["cp36-*", "cp37-*", "cp38-*", "*-musllinux*"]
+test-command = "pytest {package}/tests"
+manylinux-x86_64-image = "manylinux_2_28"
+
+[tool.cibuildwheel.linux]
+before-all = "yum install -y zlib-devel"
+archs = ["x86_64"]
```

