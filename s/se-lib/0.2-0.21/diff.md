# Comparing `tmp/se_lib-0.2.tar.gz` & `tmp/se_lib-0.21.tar.gz`

## Comparing `se_lib-0.2.tar` & `se_lib-0.21.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.2/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.2/selib/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 se_lib-0.2/selib/__init__.py
--rw-r--r--   0        0        0    44577 2020-02-02 00:00:00.000000 se_lib-0.2/selib/selib.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.2/LICENSE
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 se_lib-0.2/README.md
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 se_lib-0.2/pyproject.toml
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 se_lib-0.2/PKG-INFO
+-rw-r--r--   0        0        0     8196 2020-02-02 00:00:00.000000 se_lib-0.21/.DS_Store
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 se_lib-0.21/.gitattributes
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 se_lib-0.21/selib/.DS_Store
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 se_lib-0.21/selib/__init__.py
+-rw-r--r--   0        0        0    57249 2020-02-02 00:00:00.000000 se_lib-0.21/selib/selib.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 se_lib-0.21/LICENSE
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 se_lib-0.21/README.md
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 se_lib-0.21/pyproject.toml
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 se_lib-0.21/PKG-INFO
```

### Comparing `se_lib-0.2/.DS_Store` & `se_lib-0.21/.DS_Store`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1800 0000 0800  ....Bud1........
 00000010: 0000 1800 0000 100b 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0002 0000 0000 0000 0019  ................
-00000050: 0000 0001 0000 1000 496c 6f63 626c 6f62  ........Ilocblob
-00000060: 0000 0010 0000 0000 0000 0000 0000 0000  ................
+00000040: 0000 0000 0000 0002 0000 0000 0000 001d  ................
+00000050: 0000 0001 0000 1000 6c67 3153 636f 6d70  ........lg1Scomp
+00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,97 +250,97 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0019 0000 0004  ................
-00001010: 0064 0069 0073 0074 496c 6f63 626c 6f62  .d.i.s.tIlocblob
-00001020: 0000 0010 0000 0041 0000 002e ffff ffff  .......A........
-00001030: ffff 0000 0000 0004 0064 0069 0073 0074  .........d.i.s.t
-00001040: 6277 7370 626c 6f62 0000 00be 6270 6c69  bwspblob....bpli
-00001050: 7374 3030 d601 0203 0405 0607 0707 070b  st00............
-00001060: 075d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
-00001070: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00001080: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00001090: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-000010a0: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-000010b0: 5369 6465 6261 7209 0909 095f 101e 7b7b  Sidebar...._..{{
-000010c0: 2d31 3430 342c 202d 3130 3535 7d2c 207b  -1404, -1055}, {
-000010d0: 3134 3034 2c20 3139 3136 7d7d 0908 1523  1404, 1916}}...#
-000010e0: 2f3b 525f 6b6c 6d6e 6f90 0000 0000 0000  /;R_klmno.......
-000010f0: 0101 0000 0000 0000 000d 0000 0000 0000  ................
-00001100: 0000 0000 0000 0000 0091 0000 0004 0064  ...............d
-00001110: 0069 0073 0074 6473 636c 626f 6f6c 0100  .i.s.tdsclbool..
-00001120: 0000 0400 6400 6900 7300 746c 6731 5363  ....d.i.s.tlg1Sc
-00001130: 6f6d 7000 0000 0000 0087 e300 0000 0400  omp.............
-00001140: 6400 6900 7300 746d 6f44 4462 6c6f 6200  d.i.s.tmoDDblob.
-00001150: 0000 084c 7611 c94c e3c4 4100 0000 0400  ...Lv..L..A.....
-00001160: 6400 6900 7300 746d 6f64 4462 6c6f 6200  d.i.s.tmodDblob.
-00001170: 0000 0869 b05e 094c e3c4 4100 0000 0400  ...i.^.L..A.....
-00001180: 6400 6900 7300 7470 6831 5363 6f6d 7000  d.i.s.tph1Scomp.
-00001190: 0000 0000 00a0 0000 0000 0400 6400 6900  ............d.i.
-000011a0: 7300 7476 5372 6e6c 6f6e 6700 0000 0100  s.tvSrnlong.....
-000011b0: 0000 0700 4c00 4900 4300 4500 4e00 5300  ....L.I.C.E.N.S.
-000011c0: 4549 6c6f 6362 6c6f 6200 0000 1000 0000  EIlocblob.......
-000011d0: af00 0000 2eff ffff ffff ff00 0000 0000  ................
-000011e0: 0e00 7000 7900 7000 7200 6f00 6a00 6500  ..p.y.p.r.o.j.e.
-000011f0: 6300 7400 2e00 7400 6f00 6d00 6c49 6c6f  c.t...t.o.m.lIlo
-00001200: 6362 6c6f 6200 0000 1000 0001 1d00 0000  cblob...........
-00001210: 2eff ffff ffff ff00 0000 0000 0900 5200  ..............R.
-00001220: 4500 4100 4400 4d00 4500 2e00 6d00 6449  E.A.D.M.E...m.dI
-00001230: 6c6f 6362 6c6f 6200 0000 1000 0001 f900  locblob.........
-00001240: 0000 2eff ffff ffff ff00 0000 0000 0500  ................
-00001250: 7300 6500 6c00 6900 6249 6c6f 6362 6c6f  s.e.l.i.bIlocblo
-00001260: 6200 0000 1000 0002 6700 0000 2eff ffff  b.......g.......
-00001270: ffff ff00 0000 0000 0500 7300 6500 6c00  ..........s.e.l.
-00001280: 6900 6262 7773 7062 6c6f 6200 0000 bd62  i.bbwspblob....b
-00001290: 706c 6973 7430 30d6 0102 0304 0506 0707  plist00.........
-000012a0: 0707 0b07 5d53 686f 7753 7461 7475 7342  ....]ShowStatusB
-000012b0: 6172 5b53 686f 7754 6f6f 6c62 6172 5b53  ar[ShowToolbar[S
-000012c0: 686f 7754 6162 5669 6577 5f10 1443 6f6e  howTabView_..Con
-000012d0: 7461 696e 6572 5368 6f77 5369 6465 6261  tainerShowSideba
-000012e0: 725c 5769 6e64 6f77 426f 756e 6473 5b53  r\WindowBounds[S
-000012f0: 686f 7753 6964 6562 6172 0909 0909 5f10  howSidebar...._.
-00001300: 1d7b 7b2d 3134 3430 2c20 2d38 3337 7d2c  .{{-1440, -837},
-00001310: 207b 3133 3831 2c20 3231 3832 7d7d 0908   {1381, 2182}}..
-00001320: 1523 2f3b 525f 6b6c 6d6e 6f8f 0000 0000  .#/;R_klmno.....
-00001330: 0000 0101 0000 0000 0000 000d 0000 0000  ................
-00001340: 0000 0000 0000 0000 0000 0090 0000 0005  ................
-00001350: 0073 0065 006c 0069 0062 6473 636c 626f  .s.e.l.i.bdsclbo
-00001360: 6f6c 0100 0000 0500 7300 6500 6c00 6900  ol......s.e.l.i.
-00001370: 626c 6731 5363 6f6d 7000 0000 0000 00c6  blg1Scomp.......
-00001380: c700 0000 0500 7300 6500 6c00 6900 626d  ......s.e.l.i.bm
-00001390: 6f44 4462 6c6f 6200 0000 08c1 7e30 614c  oDDblob.....~0aL
-000013a0: e3c4 4100 0000 0500 7300 6500 6c00 6900  ..A.....s.e.l.i.
-000013b0: 626d 6f64 4462 6c6f 6200 0000 08c1 7e30  bmodDblob.....~0
-000013c0: 614c e3c4 4100 0000 0500 7300 6500 6c00  aL..A.....s.e.l.
-000013d0: 6900 6270 6831 5363 6f6d 7000 0000 0000  i.bph1Scomp.....
-000013e0: 00e0 0000 0000 0500 7300 6500 6c00 6900  ........s.e.l.i.
-000013f0: 6276 5372 6e6c 6f6e 6700 0000 0100 0000  bvSrnlong.......
-00001400: 0500 7400 6500 7300 7400 7349 6c6f 6362  ..t.e.s.t.sIlocb
-00001410: 6c6f 6200 0000 1000 0002 d500 0000 2eff  lob.............
-00001420: ffff ffff ff00 0000 0000 0500 7400 6500  ............t.e.
-00001430: 7300 7400 7364 7363 6c62 6f6f 6c01 0000  s.t.sdsclbool...
-00001440: 0005 0074 0065 0073 0074 0073 6c67 3153  ...t.e.s.t.slg1S
-00001450: 636f 6d70 0000 0000 0000 0000 0000 0005  comp............
-00001460: 0074 0065 0073 0074 0073 6d6f 4444 626c  .t.e.s.t.smoDDbl
-00001470: 6f62 0000 0008 ef3e 9a4d 87e2 c441 0000  ob.....>.M...A..
-00001480: 0005 0074 0065 0073 0074 0073 6d6f 6444  ...t.e.s.t.smodD
-00001490: 626c 6f62 0000 0008 ef3e 9a4d 87e2 c441  blob.....>.M...A
-000014a0: 0000 0005 0074 0065 0073 0074 0073 7068  .....t.e.s.t.sph
-000014b0: 3153 636f 6d70 0000 0000 0000 0000 0000  1Scomp..........
-000014c0: 0000 0001 0200 0000 0000 0001 0400 0000  ................
-000014d0: 0000 0001 0800 0000 0000 0001 1000 0000  ................
-000014e0: 0000 0001 2000 0000 0000 0001 4000 0000  .... .......@...
-000014f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001500: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001510: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001000: 0000 0000 0000 0000 0000 001d 0000 0004  ................
+00001010: 002e 0067 0069 0074 6c67 3153 636f 6d70  ...g.i.tlg1Scomp
+00001020: 0000 0000 0001 c6c7 0000 0004 002e 0067  ...............g
+00001030: 0069 0074 6d6f 4444 626c 6f62 0000 0008  .i.tmoDDblob....
+00001040: 4aeb 5880 64f0 c441 0000 0004 002e 0067  J.X.d..A.......g
+00001050: 0069 0074 6d6f 6444 626c 6f62 0000 0008  .i.tmodDblob....
+00001060: 4aeb 5880 64f0 c441 0000 0004 002e 0067  J.X.d..A.......g
+00001070: 0069 0074 7068 3153 636f 6d70 0000 0000  .i.tph1Scomp....
+00001080: 0004 e000 0000 0004 0064 0069 0073 0074  .........d.i.s.t
+00001090: 496c 6f63 626c 6f62 0000 0010 0000 0041  Ilocblob.......A
+000010a0: 0000 002e ffff ffff ffff 0000 0000 0004  ................
+000010b0: 0064 0069 0073 0074 6277 7370 626c 6f62  .d.i.s.tbwspblob
+000010c0: 0000 00bd 6270 6c69 7374 3030 d601 0203  ....bplist00....
+000010d0: 0405 0607 0709 070b 075d 5368 6f77 5374  .........]ShowSt
+000010e0: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
+000010f0: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+00001100: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+00001110: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00001120: 6e64 735b 5368 6f77 5369 6465 6261 7209  nds[ShowSidebar.
+00001130: 0908 095f 101d 7b7b 2d31 3430 362c 202d  ..._..{{-1406, -
+00001140: 3330 327d 2c20 7b31 3430 342c 2031 3931  302}, {1404, 191
+00001150: 367d 7d09 0815 232f 3b52 5f6b 6c6d 6e6f  6}}...#/;R_klmno
+00001160: 8f00 0000 0000 0001 0100 0000 0000 0000  ................
+00001170: 0d00 0000 0000 0000 0000 0000 0000 0000  ................
+00001180: 9000 0000 0400 6400 6900 7300 7464 7363  ......d.i.s.tdsc
+00001190: 6c62 6f6f 6c01 0000 0004 0064 0069 0073  lbool......d.i.s
+000011a0: 0074 6c67 3153 636f 6d70 0000 0000 0001  .tlg1Scomp......
+000011b0: 0b5f 0000 0004 0064 0069 0073 0074 6d6f  ._.....d.i.s.tmo
+000011c0: 4444 626c 6f62 0000 0008 7e87 06c8 64f0  DDblob....~...d.
+000011d0: c441 0000 0004 0064 0069 0073 0074 6d6f  .A.....d.i.s.tmo
+000011e0: 6444 626c 6f62 0000 0008 7e87 06c8 64f0  dDblob....~...d.
+000011f0: c441 0000 0004 0064 0069 0073 0074 7068  .A.....d.i.s.tph
+00001200: 3153 636f 6d70 0000 0000 0001 4000 0000  1Scomp......@...
+00001210: 0004 0064 0069 0073 0074 7653 726e 6c6f  ...d.i.s.tvSrnlo
+00001220: 6e67 0000 0001 0000 0007 004c 0049 0043  ng.........L.I.C
+00001230: 0045 004e 0053 0045 496c 6f63 626c 6f62  .E.N.S.EIlocblob
+00001240: 0000 0010 0000 00af 0000 002e ffff ffff  ................
+00001250: ffff 0000 0000 000e 0070 0079 0070 0072  .........p.y.p.r
+00001260: 006f 006a 0065 0063 0074 002e 0074 006f  .o.j.e.c.t...t.o
+00001270: 006d 006c 496c 6f63 626c 6f62 0000 0010  .m.lIlocblob....
+00001280: 0000 011d 0000 002e ffff ffff ffff 0000  ................
+00001290: 0000 0009 0052 0045 0041 0044 004d 0045  .....R.E.A.D.M.E
+000012a0: 002e 006d 0064 496c 6f63 626c 6f62 0000  ...m.dIlocblob..
+000012b0: 0010 0000 01f9 0000 002e ffff ffff ffff  ................
+000012c0: 0000 0000 0005 0073 0065 006c 0069 0062  .......s.e.l.i.b
+000012d0: 496c 6f63 626c 6f62 0000 0010 0000 0267  Ilocblob.......g
+000012e0: 0000 002e ffff ffff ffff 0000 0000 0005  ................
+000012f0: 0073 0065 006c 0069 0062 6277 7370 626c  .s.e.l.i.bbwspbl
+00001300: 6f62 0000 00bd 6270 6c69 7374 3030 d601  ob....bplist00..
+00001310: 0203 0405 0607 0709 070b 075d 5368 6f77  ...........]Show
+00001320: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
+00001330: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
+00001340: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
+00001350: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
+00001360: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
+00001370: 7209 0908 095f 101d 7b7b 2d31 3431 372c  r...._..{{-1417,
+00001380: 202d 3133 387d 2c20 7b31 3430 342c 2031   -138}, {1404, 1
+00001390: 3931 367d 7d09 0815 232f 3b52 5f6b 6c6d  916}}...#/;R_klm
+000013a0: 6e6f 8f00 0000 0000 0001 0100 0000 0000  no..............
+000013b0: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
+000013c0: 0000 9000 0000 0500 7300 6500 6c00 6900  ........s.e.l.i.
+000013d0: 6264 7363 6c62 6f6f 6c01 0000 0005 0073  bdsclbool......s
+000013e0: 0065 006c 0069 0062 6c67 3153 636f 6d70  .e.l.i.blg1Scomp
+000013f0: 0000 0000 0000 f955 0000 0005 0073 0065  .......U.....s.e
+00001400: 006c 0069 0062 6d6f 4444 626c 6f62 0000  .l.i.bmoDDblob..
+00001410: 0008 e7af bd52 62f0 c441 0000 0005 0073  .....Rb..A.....s
+00001420: 0065 006c 0069 0062 6d6f 6444 626c 6f62  .e.l.i.bmodDblob
+00001430: 0000 0008 e7af bd52 62f0 c441 0000 0005  .......Rb..A....
+00001440: 0073 0065 006c 0069 0062 7068 3153 636f  .s.e.l.i.bph1Sco
+00001450: 6d70 0000 0000 0001 2000 0000 0005 0073  mp...... ......s
+00001460: 0065 006c 0069 0062 7653 726e 6c6f 6e67  .e.l.i.bvSrnlong
+00001470: 0000 0001 0000 0005 0074 0065 0073 0074  .........t.e.s.t
+00001480: 0073 496c 6f63 626c 6f62 0000 0010 0000  .sIlocblob......
+00001490: 02d5 0000 002e ffff ffff ffff 0000 0000  ................
+000014a0: 0005 0074 0065 0073 0074 0073 6473 636c  ...t.e.s.t.sdscl
+000014b0: 626f 6f6c 0100 0000 0500 7400 6500 7300  bool......t.e.s.
+000014c0: 7400 736c 6731 5363 6f6d 7000 0000 0000  t.slg1Scomp.....
+000014d0: 0000 0000 0000 0500 7400 6500 7300 7400  ........t.e.s.t.
+000014e0: 736d 6f44 4462 6c6f 6200 0000 08ef 3e9a  smoDDblob.....>.
+000014f0: 4d87 e2c4 4100 0000 0500 7400 6500 7300  M...A.....t.e.s.
+00001500: 7400 736d 6f64 4462 6c6f 6200 0000 08ef  t.smodDblob.....
+00001510: 3e9a 4d87 e2c4 4100 0000 0500 7400 6500  >.M...A.....t.e.
+00001520: 7300 7400 7370 6831 5363 6f6d 7000 0000  s.t.sph1Scomp...
 00001530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001540: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -457,18 +457,18 @@
 00001c80: 0000 0000 0100 0100 0000 0000 0100 0200  ................
 00001c90: 0000 0000 0100 0400 0000 0000 0100 0800  ................
 00001ca0: 0000 0000 0100 1000 0000 0000 0100 2000  .............. .
 00001cb0: 0000 0000 0100 4000 0000 0000 0100 8000  ......@.........
 00001cc0: 0000 0000 0101 0000 0000 0000 0102 0000  ................
 00001cd0: 0000 0000 0104 0000 0000 0000 0108 0000  ................
 00001ce0: 0000 0000 0110 0000 0000 0000 0120 0000  ............. ..
-00001cf0: 0000 0000 0140 0000 0000 0000 0000 0000  .....@..........
-00001d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001cf0: 0000 0000 0140 0000 0000 0000 0000 7300  .....@........s.
+00001d00: 7400 736d 6f64 4462 6c6f 6200 0000 08ef  t.smodDblob.....
+00001d10: 3e9a 4d87 e2c4 4100 0000 0500 7400 6500  >.M...A.....t.e.
+00001d20: 7300 7400 7370 6831 5363 6f6d 7000 0000  s.t.sph1Scomp...
 00001d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `se_lib-0.2/selib/.DS_Store` & `se_lib-0.21/selib/.DS_Store`

 * *Files identical despite different names*

### Comparing `se_lib-0.2/selib/selib.py` & `se_lib-0.21/selib/selib.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-SElib Version .193
+se-lib Version .196
 
 Copyright (c) 2022-2023 Ray Madachy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
@@ -86,14 +86,34 @@
        transform="translate(292,474.36218)"
        id="path26"
        style="stroke-width:2.64666px" />
   </g>
 </svg>"""
 
 def context_diagram(system, external_systems, filename=None, format='svg', engine='neato'):
+    """
+    Returns a context diagram.
+
+    Parameters
+    ----------
+    system_name : string
+        The name of the system to label the diagram.
+    external_systems : list of strings
+        Names of the external systems that interact with the system in a list.
+    filename : string, optional
+        A filename for the output not including a filename extension. The extension will specified by the format parameter.
+    format : string, optional
+        The file format of the graphic output. Note that bitmap formats (png, bmp, or jpeg) will not be as sharp as the default svg vector format and most particularly when magnified.
+
+    Returns
+    -------
+    g : graph object view
+        Save the graph source code to file, and open the rendered result in its default viewing application. PyML calls the Graphviz API for this.
+
+    """
     wrap_width = 20
     def wrap(text): return textwrap.fill(
         text, width=wrap_width, break_long_words=False)
     node_attr = {'color': 'black', 'fontsize': '11', 'fontname': 'arial',
                  'shape': 'box'}  # 'fontname': 'arial',
     c = graphviz.Graph('G', node_attr=node_attr,
                        filename=filename, format=format, engine=engine)
@@ -120,14 +140,39 @@
     if filename != None:
         activity.render()  # render and save file, clean up temporary dot source file (no extension) after successful rendering with (cleanup=True) doesn't work on windows "permission denied"
         #os.remove(filename) also doesn't work on windows "permission denied"
     return activity
 
 
 def use_case_diagram(system_name, actors, use_cases, interactions, use_case_relationships, filename=None, format='svg'):
+    """ Draw a use case diagram.
+
+    Parameters
+    ----------
+    system_name : string
+        The name of the system to label the diagram.
+    actors : list of strings
+        Names of the outside actors that interact with the system in the use cases in a list.
+    use_cases : list of strings
+        Names of the use cases in a list.
+    interactions : list of tuples
+        A list of the interactions to be drawn between actors and use cases. Each interaction is a tuple containing an actor and use case in the form ("actor name", "use case name") indicating an arrow drawn from the actor to the use case. Interactions are graph edges.
+    use_case_relationships : list of tuples, optional
+        A list of the relationships, or associations to be drawn between use cases. Each relationship is a tuple containing a use case pair and type relationship in the form ("use case 1", "use case 2", "relationship") indicating an arrow drawn from the first to the second use case. Relationship types are "<<include>>", "<<extend>>" and "generalization".
+    filename : string, optional
+        A filename for the output not including a filename extension. The extension will specified by the format parameter.
+    format : string, optional
+        The file format of the graphic output. Note that bitmap formats (png, bmp, or jpeg) will not be as sharp as the default svg vector format and most particularly when magnified.
+
+    Returns
+    -------
+    g : graph object view
+        Save the graph source code to file, and open the rendered result in its default viewing application. PyML calls the Graphviz API for this.
+
+    """
     wrap_width = 15
     def wrap(text): return textwrap.fill(
         text, width=wrap_width, break_long_words=False)
     node_attr = {'color': 'black', 'fontname': 'arial',
                  'fontsize': '11',  'width': '0.'}
     edge_attr = {'arrowsize': '.5', 'fontname': 'arial', 'fontsize': '11', }
     u = graphviz.Digraph('G', filename=filename, node_attr=node_attr,
@@ -160,14 +205,37 @@
     if filename != None:
         u.render()  # render and save file, clean up temporary dot source file (no extension) after successful rendering with (cleanup=True) doesn't work on windows "permission denied"
         #os.remove(filename) also doesn't work on windows "permission denied"
     return u
 
 
 def sequence_diagram(system_name, actors, objects, actions, filename=None, format='svg'):
+    """ Returns a sequence diagram.
+
+    Parameters
+    ----------
+    system_name : string
+        The name of the system to label the diagram.
+    actors : list of strings
+        Names of the outside actors that participate in the activity sequence in a list.
+    objects : list of strings
+        Names of the system objects that participate in the activity sequence in a list.
+    actions : list of tuples
+        A chronologically ordered list describing the sequence of actions to be drawn. Each action is a tuple containing the action source, target and action name (or data/control passed) in the form ("source", "target", "action name") indicating a labeled horizontal arrow drawn between them.
+    filename : string, optional
+        A filename for the output not including a filename extension. The extension will specified by the format parameter.
+    format : string, optional
+        The file format of the graphic output. Note that bitmap formats (png, bmp, or jpeg) will not be as sharp as the default svg vector format and most particularly when magnified.
+
+    Returns
+    -------
+    g : graph object view
+        Save the graph source code to file, and open the rendered result in its default viewing application. PyML calls the Graphviz API for this.
+
+    """
     verbose = False
     wrap_width = 40
     def wrap(text): return textwrap.fill(
         text, width=wrap_width, break_long_words=False)
     graph_attr = {'rankdir': 'LR', 'color': 'black'}
     node_attr = {'shape': 'point', 'color': 'none',
                  'fontname': 'arial', 'fontsize': '11',  'width': '0.'}
@@ -231,14 +299,34 @@
     if filename != None:
         g.render()  # render and save file, clean up temporary dot source file (no extension) after successful rendering with (cleanup=True) doesn't work on windows "permission denied"
         #os.remove(filename) also doesn't work on windows "permission denied"
     return g
 
 
 def design_structure_matrix(elements, element_dependencies, filename=None, format='svg'):
+    """
+    Draw a design structure matrix of system elements and their dependencies. Matrix elements may represent tasks (process activities), system parameters or attributes.
+
+    Parameters
+    ----------
+    elements : list of strings
+        Names of the matrix elements as the row and column headings in a list.
+    element_dependencies : list of tuples
+        A list of tuples describing the relationships between elements. Each relationship is a tuple containing the relationship input element, output element and optionally a custom label (or other object) to mark the relationship in the form ("input element", "output element", "relationship label"). The default marking denoting a relationship is an uppercase 'X', therefore, the shortened tuple relationship ("input element", "output element") is equivalent to ("input element", "output element", "X"). A custom label can be specified as html code for styling of the font type, font color, cell color, etc. Images and unicode characters can be inserted this way, or other html markup for lists, tables, etc.
+    filename : string, optional
+        A filename for the output not including a filename extension. The extension will specified by the format parameter.
+    format : string, optional
+        The file format of the graphic output. Note that bitmap formats (png, bmp, or jpeg) will not be as sharp as the default svg vector format and most particularly when magnified.
+
+    Returns
+    -------
+    g : graph object view
+        The rendered graph for display. It will be automatically displayed in Jupyter Notebooks or IPython consoles. With other Python editors it can be displayed in the associated console by typing the returned graph name (e.g., call the function with an assignment such as ``dsm = design_structure_matrix(...)`` and then type ``dsm`` in the console). If a filename is optionally provided, the rendered graph will also be saved as a file in the specified format. PyML calls the Graphviz API for this.
+
+    """
     cell_width = 20  # pixels
 
     dependency_elements = [dependency[0:2]
                            for dependency in element_dependencies]
 
     node_string = '<table border="0" cellborder="1"  cellspacing="0">'
     for row, element in enumerate((['']+elements)):
@@ -278,14 +366,34 @@
     if filename != None:
         dsm.render()  # render and save file, clean up temporary dot source file (no extension) after successful rendering with (cleanup=True) doesn't work on windows "permission denied"
         #os.remove(filename) also doesn't work on windows "permission denied"
     return dsm
 
 
 def wbs_diagram(decompositions, filename=None, format='svg', rankdir='TB'):
+    """
+    Draw a work breakdown structure as a tree hierarchy. Decompositions describe the parent-child relationships.
+
+    Parameters
+    ----------
+    decompositions : list of tuples
+        A list of tuples describing the work decomposition relationships. Each relationship is a tuple containing the parent element followed by the child element.
+    filename : string, optional
+        A filename for the output not including a filename extension. The extension will specified by the format parameter.
+    format : string, optional
+        The file format of the graphic output. Note that bitmap formats (png, bmp, or jpeg) will not be as sharp as the default svg vector format and most particularly when magnified.
+    rankdir : string, optional
+        The direction to display the tree from the parent node. The default ``rankdir='TB'`` denotes top to bottom for a vertical tree decomposition. It can diagrammed horizontally by providing rankdir='LR' to designate left to right.
+
+    Returns
+    -------
+    g : graph object view
+        The rendered graph for display. It will be automatically displayed in Jupyter Notebooks or IPython consoles. With other Python editors it can be displayed in the associated console by typing the returned graph name (e.g., call the function with an assignment such as ``wbs = wbs_diagram(...)`` and then type ``wbs`` in the console). If a filename is optionally provided, the rendered graph will also be saved as a file in the specified format. PyML calls the Graphviz API for this.
+
+    """
     node_attr = {'color': 'black', 'fontsize': '11',
                  'shape': 'box'}  # 'fontname': 'arial',
     edge_attr = {'arrowsize': '.5', 'fontname': 'arial', 'fontsize': '11', }
     activity = graphviz.Digraph('G', filename=filename, node_attr=node_attr,
                                 edge_attr=edge_attr, engine="dot", format='svg')
     activity.attr(rankdir=rankdir, splines='ortho')  # rankdir='LR'
     activity.edges(decompositions)
@@ -310,14 +418,43 @@
         #os.remove(filename) also doesn't work on windows "permission denied"
     return activity
 
 
 
 
 def fault_tree_diagram(ft, filename=None, format='svg'):
+    """ Returns a fault tree diagram.
+
+    Parameters
+    ----------
+    ft : list of tuples
+        A list of the faults as a tree hierarchy. Each fault is defined in a tuple containing the fault name, type, and underlying faults (if any) in the form
+        ``("fault name", "fault name", list of fault branches)``
+        with the branches as a list in the form
+        ``["branch 1 name", "branch 2 name", ... "branch n name"]``
+        to identify the adjoining faults. All basic events will have a blank list
+        ``[]`` since they are the bottom leaves in the tree.
+
+        The top event must be in the first row, but all other events can be in any order. They may begrouped by their event paths or by hierarchical levels as convenient. Event types can be conditional "and"s, conditional "or"s, or basic events (leaves). The following spellings are recognized as valid designations for event types:
+
+        And: "And" "and" "AND" \n
+        Or: "Or" "or" "OR" \n
+        Basic: "Basic" "basic" "BASIC"
+
+    filename : string, optional
+        A filename for the output not including a filename extension. The extension will specified by the format parameter.
+    format : string, optional
+        The file format of the graphic output. Note that bitmap formats (png, bmp, or jpeg) will not be as sharp as the default svg vector format and most particularly when magnified.
+
+    Returns
+    -------
+    g : graph object view
+        Save the graph source code to file, and open the rendered result in its default viewing application. PyML calls the Graphviz API for this.
+
+    """
     verbose = False
     wrap_width = 15
     def wrap(text): return textwrap.fill(
         text, width=wrap_width, break_long_words=False).replace("\n", "<BR/>")
     node_attr = {'color': 'black', 'fontsize': '11',
                  'shape': 'plaintext'}  # 'fontname': 'arial',
     edge_attr = {'arrowtail': 'none', 'arrowsize': '0', 'dir': 'both', 'penwidth': '2', 'fontname': 'arial', 'fontsize': '11', } #https://graphviz.org/docs/attr-types/arrowType/
@@ -945,14 +1082,34 @@
     def is_acyclic(self):
         g = dict((node.name, tuple(child.name for child in node.to_nodes))
                  for node in self.nodes)
         return not cyclic(g)
 
 
 def critical_path_diagram(tasks, task_dependencies, filename=None, format='svg'):
+    """
+    Compute and draw the critical path between dependent tasks as the longest in duration from start to finish.
+
+    Parameters
+    ----------
+    tasks : list of tuples where each contains a task name and dictionary for duration time
+        A list of tuples where each one contains a task name and dictionary for its duration time (where keyword = "Duration" and value is a number).
+    task_dependencies : list of tuples
+        A list of tuples describing the dependency relationships between tasks. Each relationship is a tuple containing the predecessor task followed by its successor task. These must be the same named tasks in the task list input above.
+    filename : string, optional
+        A filename for the output not including a filename extension. The extension will specified by the format parameter.
+    format : string, optional
+        The file format of the graphic output. Note that bitmap formats (png, bmp, or jpeg) will not be as sharp as the default svg vector format and most particularly when magnified.
+
+    Returns
+    -------
+    g : graph object view
+        The rendered graph for display. It will be automatically displayed in Jupyter Notebooks or IPython consoles. With other Python editors it can be displayed in the associated console by typing the returned graph name (e.g., call the function with an assignment such as ``critical_path = critical_path_diagram(...)`` and then type ``critical_path`` in the console). If a filename is optionally provided, the rendered graph will also be saved as a file in the specified format. PyML calls the Graphviz API for this.
+
+    """
     node_attr = {'color': 'black', 'fontsize': '11',
                  'shape': 'box'}  # 'fontname': 'arial',
     edge_attr = {'arrowsize': '.5', 'fontname': 'arial',
                  'fontsize': '11', 'color': 'black'}
     critical_path = graphviz.Digraph(
         'G', filename=filename, node_attr=node_attr, edge_attr=edge_attr, engine="dot", format='svg')
     critical_path.attr(rankdir='LR',)
@@ -1050,14 +1207,43 @@
             events_quant_dict_labeled[event+prob_string(event, events_quant_dict[event]['prob'])]['branches'][index] = branch_label
 
     simple_ft_quantititive = [(event, events_quant_dict_labeled[event]['type'], events_quant_dict_labeled[event]['branches']) for event in events_quant_dict_labeled]
 
     return(fault_tree_diagram(simple_ft_quantititive, filename=filename, format=format))
 
 def fault_tree_cutsets(fault_tree):
+    """ Returns a fault tree cutset.
+
+    Parameters
+    ----------
+    ft : list of tuples
+        A list of the faults as a tree hierarchy. Each fault is defined in a tuple containing the fault name, type, and underlying faults (if any) in the form
+        ``("fault name", "fault name", list of fault branches)``
+        with the branches as a list in the form
+        ``["branch 1 name", "branch 2 name", ... "branch n name"]``
+        to identify the adjoining faults. All basic events will have a blank list
+        ``[]`` since they are the bottom leaves in the tree.
+
+        The top event must be in the first row, but all other events can be in any order. They may begrouped by their event paths or by hierarchical levels as convenient. Event types can be conditional "and"s, conditional "or"s, or basic events (leaves). The following spellings are recognized as valid designations for event types:
+
+        And: "And" "and" "AND" \n
+        Or: "Or" "or" "OR" \n
+        Basic: "Basic" "basic" "BASIC"
+
+    filename : string, optional
+        A filename for the output not including a filename extension. The extension will specified by the format parameter.
+    format : string, optional
+        The file format of the graphic output. Note that bitmap formats (png, bmp, or jpeg) will not be as sharp as the default svg vector format and most particularly when magnified.
+
+    Returns
+    -------
+    cutsets : list of lists
+        Returns a list of cutsets, where each is defined as a list of events.
+
+    """
     cutsets = mocus(fault_tree)
     print("Minimal Cutsets:\nNumber  Event List")
     for num, cutset in enumerate(cutsets):
         print(num+1,'  ', cutset)
 
 import os
 import itertools
@@ -1161,22 +1347,15 @@
             ps = cs_helper(i, j, ps, dic_ft)
             #print(f'{ps=}') # rm
         except BaseException:
             break
     return(ps)
 
 def mocus(fault_tree):
-    '''
-    ===============================================================================
-        MOCUS algorithm for finding cutsets
-        Authors: Umair Siddique, Ray Madachy
-        Description: Accepts a fault tree and generates the minimal cutsets
-        License: MIT
-    ===============================================================================
-    '''
+
     verbose = False
     fault_tree_copy = deepcopy(fault_tree) # to avoid top row "and" rewrite in cs_helper
     cs = []
     cs = mocus_init(fault_tree_copy)
     css = list(map(lambda x: list(set(x)), cs))
     css.sort(key=len)
     for a, b in itertools.combinations(css, 2):
@@ -1184,8 +1363,48 @@
         if set(a) <= set(b):
             try:
                 css.remove(b)
             except BaseException:
                 continue
     if verbose: print(f'***{css=}') # rm
     ft = copy
-    return(css)
+    return(css)
+
+# system dynamics simulation functions
+def add_flow(name, equation):
+    """
+    Adds a flow to the model
+
+    Parameters
+    ----------
+    name: str
+      The name of the flow 
+    equation: str
+      Equation for the flow using other named model variables
+    """
+    global model
+    model += f"""
+                <flow name="{name}">
+                    <doc>{name}</doc>
+                    <eqn>{equation}</eqn>
+                </flow>"""
+    build_model()
+
+def plot_graph(*outputs):
+    """
+    displays matplotlib graph for each model variable
+
+    Parameters
+    ----------
+    variables: variable name or list of variable names to plot on graph
+
+    Returns:
+    ----------
+    matplotlib graph
+    """
+    #print (outputs, len(outputs))
+    for var in outputs:
+        fig, axis = plot.subplots(figsize=(4, 3))
+        axis.set(xlabel='Time', ylabel=var)
+        axis.plot(output.index, output[var].values, label=var)
+        if len(outputs) > 1: axis.legend(loc="best", )
+        plot.show()
```

### Comparing `se_lib-0.2/LICENSE` & `se_lib-0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `se_lib-0.2/README.md` & `se_lib-0.21/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Systems Engineering Library (se-lib)
-se-lib Version .2
+Version .2
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `se_lib-0.2/PKG-INFO` & `se_lib-0.21/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: se-lib
-Version: 0.2
+Version: 0.21
 Summary: Systems Engineering Library (se-lib)
-Project-URL: Homepage, http://pyml.fun
+Project-URL: Homepage, http://se-lib.org
 Author-email: se-lib Development Team <info@se-lib.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Systems Engineering Library (se-lib)
-se-lib Version .2
+Version .2
 
 Copyright (c) 2022-2023 se-lib Development Team
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

