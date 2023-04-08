# Comparing `tmp/openstates-6.9.1.tar.gz` & `tmp/openstates-6.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstates-6.9.1.tar", max compression
+gzip compressed data, was "openstates-6.9.2.tar", max compression
```

## Comparing `openstates-6.9.1.tar` & `openstates-6.9.2.tar`

### file list

```diff
@@ -1,286 +1,286 @@
--rw-r--r--   0        0        0     1080 2021-04-27 20:50:33.722134 openstates-6.9.1/LICENSE
--rw-r--r--   0        0        0        0 2020-04-08 21:23:57.750660 openstates-6.9.1/openstates/__init__.py
--rw-r--r--   0        0        0        0 2021-05-03 14:50:07.647616 openstates-6.9.1/openstates/cli/__init__.py
--rw-r--r--   0        0        0    20809 2021-11-08 20:47:02.920405 openstates-6.9.1/openstates/cli/committees.py
--rw-r--r--   0        0        0    11283 2021-11-17 16:44:52.239273 openstates-6.9.1/openstates/cli/convert_us.py
--rw-r--r--   0        0        0     2813 2021-05-27 18:33:47.049306 openstates-6.9.1/openstates/cli/initdb.py
--rw-r--r--   0        0        0    22635 2021-11-08 20:47:02.922541 openstates-6.9.1/openstates/cli/people.py
--rw-r--r--   0        0        0     6919 2021-08-02 18:12:37.031232 openstates-6.9.1/openstates/cli/reports.py
--rw-r--r--   0        0        0        0 2020-04-08 21:23:57.751191 openstates-6.9.1/openstates/cli/tests/__init__.py
--rw-r--r--   0        0        0     5904 2021-05-27 15:21:16.591627 openstates-6.9.1/openstates/cli/tests/test_initdb.py
--rw-r--r--   0        0        0     8305 2021-05-27 15:21:16.592363 openstates-6.9.1/openstates/cli/tests/test_session_report.py
--rw-r--r--   0        0        0      632 2021-05-27 15:21:16.593024 openstates-6.9.1/openstates/cli/tests/test_settings.py
--rw-r--r--   0        0        0    12266 2021-05-27 18:31:42.033886 openstates-6.9.1/openstates/cli/text_extract.py
--rw-r--r--   0        0        0    12229 2021-11-08 20:47:02.923680 openstates-6.9.1/openstates/cli/update.py
--rw-r--r--   0        0        0      915 2021-05-27 18:18:32.164383 openstates-6.9.1/openstates/cli/update_computed.py
--rw-r--r--   0        0        0        0 2020-04-08 21:23:57.751916 openstates-6.9.1/openstates/data/__init__.py
--rw-r--r--   0        0        0       83 2020-04-08 21:23:57.752086 openstates-6.9.1/openstates/data/admin/__init__.py
--rw-r--r--   0        0        0     1417 2021-11-09 21:20:22.981644 openstates-6.9.1/openstates/data/admin/base.py
--rw-r--r--   0        0        0     4245 2021-11-09 21:20:22.983118 openstates-6.9.1/openstates/data/admin/bill.py
--rw-r--r--   0        0        0     2373 2021-11-08 20:47:02.926101 openstates-6.9.1/openstates/data/admin/event.py
--rw-r--r--   0        0        0     3573 2021-11-09 21:20:22.983480 openstates-6.9.1/openstates/data/admin/organization.py
--rw-r--r--   0        0        0     2910 2021-11-09 21:20:22.983825 openstates-6.9.1/openstates/data/admin/other.py
--rw-r--r--   0        0        0     2704 2021-11-09 21:20:22.984175 openstates-6.9.1/openstates/data/admin/person.py
--rw-r--r--   0        0        0     2497 2021-11-09 21:20:22.985495 openstates-6.9.1/openstates/data/admin/reports.py
--rw-r--r--   0        0        0     1783 2021-11-09 21:20:22.986820 openstates-6.9.1/openstates/data/admin/vote.py
--rw-r--r--   0        0        0     6628 2021-11-09 15:34:24.292111 openstates-6.9.1/openstates/data/common.py
--rw-r--r--   0        0        0   104004 2020-09-14 15:27:39.435524 openstates-6.9.1/openstates/data/migrations/0001_initial.py
--rw-r--r--   0        0        0      830 2020-04-23 19:18:11.574663 openstates-6.9.1/openstates/data/migrations/0002_auto_20200422_0028.py
--rw-r--r--   0        0        0      406 2020-04-23 19:18:11.574832 openstates-6.9.1/openstates/data/migrations/0003_auto_20200422_0031.py
--rw-r--r--   0        0        0      435 2020-04-23 19:18:11.574984 openstates-6.9.1/openstates/data/migrations/0004_auto_20200422_0040.py
--rw-r--r--   0        0        0      692 2020-04-23 19:18:11.575081 openstates-6.9.1/openstates/data/migrations/0005_auto_20200423_1100.py
--rw-r--r--   0        0        0      899 2020-04-23 19:18:11.575169 openstates-6.9.1/openstates/data/migrations/0006_auto_20200423_1124.py
--rw-r--r--   0        0        0      951 2020-04-23 19:17:07.852276 openstates-6.9.1/openstates/data/migrations/0007_auto_20200423_1416.py
--rw-r--r--   0        0        0      383 2020-04-28 20:31:10.014271 openstates-6.9.1/openstates/data/migrations/0008_person_current_state.py
--rw-r--r--   0        0        0      948 2020-04-29 14:13:13.638348 openstates-6.9.1/openstates/data/migrations/0009_auto_20200429_0913.py
--rw-r--r--   0        0        0      659 2020-07-22 15:56:29.521217 openstates-6.9.1/openstates/data/migrations/0010_auto_20200721_1604.py
--rw-r--r--   0        0        0      928 2021-04-27 20:50:33.732106 openstates-6.9.1/openstates/data/migrations/0011_auto_20200804_1108.py
--rw-r--r--   0        0        0      477 2020-08-04 20:24:15.725857 openstates-6.9.1/openstates/data/migrations/0012_person_current_role.py
--rw-r--r--   0        0        0      268 2020-08-04 21:54:20.987895 openstates-6.9.1/openstates/data/migrations/0013_remove_person_current_state.py
--rw-r--r--   0        0        0      301 2020-08-05 19:03:00.654334 openstates-6.9.1/openstates/data/migrations/0014_remove_person_current_role_division_id.py
--rw-r--r--   0        0        0      601 2021-04-27 20:50:33.732795 openstates-6.9.1/openstates/data/migrations/0015_auto_20200811_1009.py
--rw-r--r--   0        0        0      636 2021-04-27 20:50:33.733613 openstates-6.9.1/openstates/data/migrations/0016_auto_20200811_1016.py
--rw-r--r--   0        0        0      326 2021-04-27 20:50:33.734102 openstates-6.9.1/openstates/data/migrations/0017_remove_person_summary.py
--rw-r--r--   0        0        0     1119 2021-04-27 20:50:33.734692 openstates-6.9.1/openstates/data/migrations/0018_auto_20200914_1032.py
--rw-r--r--   0        0        0      329 2021-04-27 20:50:33.735213 openstates-6.9.1/openstates/data/migrations/0019_remove_billabstract_date.py
--rw-r--r--   0        0        0      448 2021-04-27 20:50:33.735738 openstates-6.9.1/openstates/data/migrations/0020_auto_20200914_1041.py
--rw-r--r--   0        0        0      338 2021-04-27 20:50:33.736473 openstates-6.9.1/openstates/data/migrations/0021_remove_jurisdiction_feature_flags.py
--rw-r--r--   0        0        0      580 2021-04-27 20:50:33.737107 openstates-6.9.1/openstates/data/migrations/0022_auto_20200914_1054.py
--rw-r--r--   0        0        0      337 2021-04-27 20:50:33.737589 openstates-6.9.1/openstates/data/migrations/0023_remove_personcontactdetail_label.py
--rw-r--r--   0        0        0      444 2021-04-27 20:50:33.738109 openstates-6.9.1/openstates/data/migrations/0024_auto_20200914_1101.py
--rw-r--r--   0        0        0      779 2021-04-27 20:50:33.738527 openstates-6.9.1/openstates/data/migrations/0025_auto_20200914_1216.py
--rw-r--r--   0        0        0     2551 2021-04-27 20:50:33.739141 openstates-6.9.1/openstates/data/migrations/0026_auto_20200923_1312.py
--rw-r--r--   0        0        0      424 2021-04-27 20:50:33.740075 openstates-6.9.1/openstates/data/migrations/0027_auto_20200923_1329.py
--rw-r--r--   0        0        0      836 2021-04-27 20:50:33.741563 openstates-6.9.1/openstates/data/migrations/0028_auto_20201022_1642.py
--rw-r--r--   0        0        0      389 2021-04-27 20:50:33.742302 openstates-6.9.1/openstates/data/migrations/0029_auto_20210203_1946.py
--rw-r--r--   0        0        0      718 2021-04-27 20:50:33.743670 openstates-6.9.1/openstates/data/migrations/0030_auto_20210210_1817.py
--rw-r--r--   0        0        0      914 2021-04-27 20:50:33.744238 openstates-6.9.1/openstates/data/migrations/0031_auto_20210401_1449.py
--rw-r--r--   0        0        0      396 2021-04-27 20:50:33.745131 openstates-6.9.1/openstates/data/migrations/0032_event_dedupe_key.py
--rw-r--r--   0        0        0     1001 2021-04-27 20:50:33.745990 openstates-6.9.1/openstates/data/migrations/0033_auto_20210421_1538.py
--rw-r--r--   0        0        0      497 2021-04-27 20:50:33.746846 openstates-6.9.1/openstates/data/migrations/0034_organization_other_names.py
--rw-r--r--   0        0        0     3813 2021-04-27 20:50:33.747386 openstates-6.9.1/openstates/data/migrations/0035_auto_20210422_1926.py
--rw-r--r--   0        0        0      634 2021-08-02 17:52:53.007515 openstates-6.9.1/openstates/data/migrations/0036_auto_20210802_1752.py
--rw-r--r--   0        0        0     7214 2021-08-02 18:12:37.032552 openstates-6.9.1/openstates/data/migrations/0037_importobjects_runplan_scrapeobjects_scrapereport_sessiondataqualityreport.py
--rw-r--r--   0        0        0      642 2021-11-08 20:47:02.929058 openstates-6.9.1/openstates/data/migrations/0038_auto_20210914_1559.py
--rw-r--r--   0        0        0      807 2021-11-08 20:47:02.929639 openstates-6.9.1/openstates/data/migrations/0039_auto_20210920_1934.py
--rw-r--r--   0        0        0     1203 2021-11-08 20:47:02.930372 openstates-6.9.1/openstates/data/migrations/0040_auto_20210920_2347.py
--rw-r--r--   0        0        0     1810 2021-11-08 20:47:02.930894 openstates-6.9.1/openstates/data/migrations/0041_personoffice.py
--rw-r--r--   0        0        0      299 2021-11-08 20:47:02.931410 openstates-6.9.1/openstates/data/migrations/0042_delete_personcontactdetail.py
--rw-r--r--   0        0        0      404 2021-11-08 20:47:02.933013 openstates-6.9.1/openstates/data/migrations/0043_legislativesession_active.py
--rw-r--r--   0        0        0      435 2021-11-09 15:34:24.293472 openstates-6.9.1/openstates/data/migrations/0044_bill_citations.py
--rw-r--r--   0        0        0        0 2020-04-08 21:23:57.754015 openstates-6.9.1/openstates/data/migrations/__init__.py
--rw-r--r--   0        0        0      926 2021-11-08 20:47:02.933871 openstates-6.9.1/openstates/data/models/__init__.py
--rw-r--r--   0        0        0     4280 2021-11-08 20:47:02.934502 openstates-6.9.1/openstates/data/models/base.py
--rw-r--r--   0        0        0     8257 2021-11-09 15:34:24.295220 openstates-6.9.1/openstates/data/models/bill.py
--rw-r--r--   0        0        0     4901 2020-04-08 21:23:57.754813 openstates-6.9.1/openstates/data/models/division.py
--rw-r--r--   0        0        0     6138 2021-11-08 20:47:02.935417 openstates-6.9.1/openstates/data/models/event.py
--rw-r--r--   0        0        0     2436 2021-11-08 20:47:02.936115 openstates-6.9.1/openstates/data/models/jurisdiction.py
--rw-r--r--   0        0        0    12495 2021-11-08 20:47:02.936924 openstates-6.9.1/openstates/data/models/people_orgs.py
--rw-r--r--   0        0        0     2882 2021-08-02 18:12:37.033618 openstates-6.9.1/openstates/data/models/reports.py
--rw-r--r--   0        0        0     3425 2021-04-27 20:50:33.753470 openstates-6.9.1/openstates/data/models/vote.py
--rw-r--r--   0        0        0        0 2020-04-08 21:23:57.756106 openstates-6.9.1/openstates/data/tests/__init__.py
--rw-r--r--   0        0        0     3458 2021-04-27 20:50:33.754129 openstates-6.9.1/openstates/data/tests/conftest.py
--rw-r--r--   0        0        0    15627 2021-11-08 20:47:02.937864 openstates-6.9.1/openstates/data/tests/test_models.py
--rw-r--r--   0        0        0     1814 2021-11-08 20:47:02.938676 openstates-6.9.1/openstates/exceptions.py
--rw-r--r--   0        0        0     5624 2021-05-27 15:49:11.275776 openstates-6.9.1/openstates/fulltext/__init__.py
--rw-r--r--   0        0        0     4539 2021-05-27 15:49:28.760071 openstates-6.9.1/openstates/fulltext/common.py
--rw-r--r--   0        0        0     1406 2021-05-27 15:42:46.026934 openstates-6.9.1/openstates/fulltext/de.py
--rw-r--r--   0        0        0    19582 2021-05-12 16:17:42.440947 openstates-6.9.1/openstates/fulltext/raw/ak.csv
--rw-r--r--   0        0        0    17854 2021-05-12 16:17:42.441694 openstates-6.9.1/openstates/fulltext/raw/al.csv
--rw-r--r--   0        0        0    15635 2021-05-12 16:17:42.442002 openstates-6.9.1/openstates/fulltext/raw/ar.csv
--rw-r--r--   0        0        0    13377 2021-05-12 16:17:42.442183 openstates-6.9.1/openstates/fulltext/raw/az.csv
--rw-r--r--   0        0        0    14336 2021-05-12 16:17:42.442624 openstates-6.9.1/openstates/fulltext/raw/ca.csv
--rw-r--r--   0        0        0    13723 2021-05-12 16:17:42.443447 openstates-6.9.1/openstates/fulltext/raw/co.csv
--rw-r--r--   0        0        0    13619 2021-05-12 16:17:42.443796 openstates-6.9.1/openstates/fulltext/raw/ct.csv
--rw-r--r--   0        0        0    13844 2021-05-12 16:17:42.443982 openstates-6.9.1/openstates/fulltext/raw/dc.csv
--rw-r--r--   0        0        0    35228 2021-05-12 16:17:42.444228 openstates-6.9.1/openstates/fulltext/raw/de.csv
--rw-r--r--   0        0        0    11260 2021-05-12 16:17:42.444710 openstates-6.9.1/openstates/fulltext/raw/fl.csv
--rw-r--r--   0        0        0    14157 2021-05-12 16:17:42.445573 openstates-6.9.1/openstates/fulltext/raw/ga.csv
--rw-r--r--   0        0        0    25367 2021-05-12 16:17:42.445896 openstates-6.9.1/openstates/fulltext/raw/hi.csv
--rw-r--r--   0        0        0    43184 2021-05-12 16:17:42.446261 openstates-6.9.1/openstates/fulltext/raw/ia.csv
--rw-r--r--   0        0        0    19435 2021-05-12 16:17:42.446760 openstates-6.9.1/openstates/fulltext/raw/id.csv
--rw-r--r--   0        0        0    14703 2021-05-12 16:17:42.447050 openstates-6.9.1/openstates/fulltext/raw/il.csv
--rw-r--r--   0        0        0    14440 2021-05-12 16:17:42.447533 openstates-6.9.1/openstates/fulltext/raw/in.csv
--rw-r--r--   0        0        0    15777 2021-05-12 16:17:42.447834 openstates-6.9.1/openstates/fulltext/raw/ks.csv
--rw-r--r--   0        0        0     3714 2021-05-12 16:17:42.448713 openstates-6.9.1/openstates/fulltext/raw/ky.csv
--rw-r--r--   0        0        0    16826 2021-05-12 16:17:42.449309 openstates-6.9.1/openstates/fulltext/raw/la.csv
--rw-r--r--   0        0        0    12313 2021-05-12 16:17:42.449846 openstates-6.9.1/openstates/fulltext/raw/ma.csv
--rw-r--r--   0        0        0    18330 2021-05-12 16:17:42.450401 openstates-6.9.1/openstates/fulltext/raw/md.csv
--rw-r--r--   0        0        0    46138 2021-05-12 16:17:42.451133 openstates-6.9.1/openstates/fulltext/raw/me.csv
--rw-r--r--   0        0        0    20401 2021-05-12 16:17:42.451417 openstates-6.9.1/openstates/fulltext/raw/mi.csv
--rw-r--r--   0        0        0    17150 2021-05-12 16:17:42.451893 openstates-6.9.1/openstates/fulltext/raw/mn.csv
--rw-r--r--   0        0        0    14045 2021-05-12 16:17:42.452206 openstates-6.9.1/openstates/fulltext/raw/mo.csv
--rw-r--r--   0        0        0    16563 2021-05-12 16:17:42.452768 openstates-6.9.1/openstates/fulltext/raw/ms.csv
--rw-r--r--   0        0        0    11531 2021-05-12 16:17:42.453211 openstates-6.9.1/openstates/fulltext/raw/mt.csv
--rw-r--r--   0        0        0    11173 2021-05-12 16:17:42.453834 openstates-6.9.1/openstates/fulltext/raw/nc.csv
--rw-r--r--   0        0        0    26171 2021-05-12 16:17:42.454853 openstates-6.9.1/openstates/fulltext/raw/nd.csv
--rw-r--r--   0        0        0    14434 2021-05-12 16:17:42.455073 openstates-6.9.1/openstates/fulltext/raw/ne.csv
--rw-r--r--   0        0        0    14745 2021-05-12 16:17:42.455827 openstates-6.9.1/openstates/fulltext/raw/nh.csv
--rw-r--r--   0        0        0    15796 2021-05-12 16:17:42.456384 openstates-6.9.1/openstates/fulltext/raw/nj.csv
--rw-r--r--   0        0        0    21601 2021-05-12 16:17:42.456967 openstates-6.9.1/openstates/fulltext/raw/nm.csv
--rw-r--r--   0        0        0    14776 2021-05-12 16:17:42.457422 openstates-6.9.1/openstates/fulltext/raw/nv.csv
--rw-r--r--   0        0        0    14076 2021-05-12 16:17:42.458172 openstates-6.9.1/openstates/fulltext/raw/ny.csv
--rw-r--r--   0        0        0    15120 2021-05-12 16:17:42.458362 openstates-6.9.1/openstates/fulltext/raw/oh.csv
--rw-r--r--   0        0        0    16028 2021-05-12 16:17:42.458768 openstates-6.9.1/openstates/fulltext/raw/ok.csv
--rw-r--r--   0        0        0    15374 2021-05-12 16:17:42.458925 openstates-6.9.1/openstates/fulltext/raw/or.csv
--rw-r--r--   0        0        0    78160 2021-05-12 16:17:42.467107 openstates-6.9.1/openstates/fulltext/raw/pa.csv
--rw-r--r--   0        0        0    40360 2021-05-12 16:17:42.467850 openstates-6.9.1/openstates/fulltext/raw/pr.csv
--rw-r--r--   0        0        0    21447 2021-05-12 16:17:42.468097 openstates-6.9.1/openstates/fulltext/raw/ri.csv
--rw-r--r--   0        0        0    46905 2021-05-12 16:17:42.468684 openstates-6.9.1/openstates/fulltext/raw/sc.csv
--rw-r--r--   0        0        0    16878 2021-05-12 16:17:42.468877 openstates-6.9.1/openstates/fulltext/raw/sd.csv
--rw-r--r--   0        0        0    20147 2021-05-12 16:17:42.469390 openstates-6.9.1/openstates/fulltext/raw/tn.csv
--rw-r--r--   0        0        0    16034 2021-05-12 16:17:42.469573 openstates-6.9.1/openstates/fulltext/raw/tx.csv
--rw-r--r--   0        0        0    11264 2021-05-12 16:17:42.469900 openstates-6.9.1/openstates/fulltext/raw/ut.csv
--rw-r--r--   0        0        0    14596 2021-05-12 16:17:42.470402 openstates-6.9.1/openstates/fulltext/raw/va.csv
--rw-r--r--   0        0        0     5071 2021-05-12 16:17:42.470793 openstates-6.9.1/openstates/fulltext/raw/vt.csv
--rw-r--r--   0        0        0    14440 2021-05-12 16:17:42.471009 openstates-6.9.1/openstates/fulltext/raw/wa.csv
--rw-r--r--   0        0        0    30123 2021-05-12 16:17:42.471355 openstates-6.9.1/openstates/fulltext/raw/wi.csv
--rw-r--r--   0        0        0    15620 2021-05-12 16:17:42.471525 openstates-6.9.1/openstates/fulltext/raw/wv.csv
--rw-r--r--   0        0        0    11653 2021-05-12 16:17:42.471668 openstates-6.9.1/openstates/fulltext/raw/wy.csv
--rw-r--r--   0        0        0     3463 2021-05-27 15:44:58.883825 openstates-6.9.1/openstates/fulltext/utils.py
--rw-r--r--   0        0        0      219 2021-04-27 20:50:33.755355 openstates-6.9.1/openstates/importers/__init__.py
--rw-r--r--   0        0        0      508 2021-06-02 18:30:04.723456 openstates-6.9.1/openstates/importers/_types.py
--rw-r--r--   0        0        0    21576 2021-11-08 20:47:02.939585 openstates-6.9.1/openstates/importers/base.py
--rw-r--r--   0        0        0     4863 2021-09-24 17:45:55.743994 openstates-6.9.1/openstates/importers/bills.py
--rw-r--r--   0        0        0     1630 2021-04-27 20:50:33.759845 openstates-6.9.1/openstates/importers/computed_fields.py
--rw-r--r--   0        0        0     4454 2021-11-08 20:47:02.940907 openstates-6.9.1/openstates/importers/events.py
--rw-r--r--   0        0        0      787 2021-04-27 20:50:33.761291 openstates-6.9.1/openstates/importers/jurisdiction.py
--rw-r--r--   0        0        0      519 2021-06-02 18:30:04.724224 openstates-6.9.1/openstates/importers/organizations.py
--rw-r--r--   0        0        0        0 2020-04-08 21:23:57.759804 openstates-6.9.1/openstates/importers/tests/__init__.py
--rw-r--r--   0        0        0     7567 2021-11-08 20:47:02.941724 openstates-6.9.1/openstates/importers/tests/test_base_importer.py
--rw-r--r--   0        0        0    18087 2021-04-27 20:50:33.763811 openstates-6.9.1/openstates/importers/tests/test_bill_importer.py
--rw-r--r--   0        0        0     1648 2020-04-24 22:15:15.291393 openstates-6.9.1/openstates/importers/tests/test_computed_fields.py
--rw-r--r--   0        0        0    11463 2021-11-08 20:47:02.942772 openstates-6.9.1/openstates/importers/tests/test_event_importer.py
--rw-r--r--   0        0        0     2502 2021-11-08 20:47:02.943546 openstates-6.9.1/openstates/importers/tests/test_jurisdiction_importer.py
--rw-r--r--   0        0        0    17020 2021-04-27 20:50:33.765562 openstates-6.9.1/openstates/importers/tests/test_vote_event_importer.py
--rw-r--r--   0        0        0     5472 2021-04-27 20:50:33.766493 openstates-6.9.1/openstates/importers/vote_events.py
--rw-r--r--   0        0        0     2067 2021-04-27 20:50:33.767456 openstates-6.9.1/openstates/metadata/__init__.py
--rwxr-xr-x   0        0        0      516 2021-04-27 20:50:33.768557 openstates-6.9.1/openstates/metadata/_creation/create_data.sh
--rw-r--r--   0        0        0     6155 2021-04-27 20:50:33.768976 openstates-6.9.1/openstates/metadata/_creation/jurisdictions.csv
--rw-r--r--   0        0        0    23390 2021-04-27 20:50:33.769240 openstates-6.9.1/openstates/metadata/_creation/orgs.csv
--rw-r--r--   0        0        0    36641 2021-04-27 20:50:33.770331 openstates-6.9.1/openstates/metadata/_creation/settings.yml
--rw-r--r--   0        0        0     7059 2021-05-27 16:03:25.911262 openstates-6.9.1/openstates/metadata/_creation/write_data.py
--rw-r--r--   0        0        0      344 2021-11-08 20:47:02.944419 openstates-6.9.1/openstates/metadata/data/__init__.py
--rw-r--r--   0        0        0     2857 2021-04-27 20:50:33.772048 openstates-6.9.1/openstates/metadata/data/ak.py
--rw-r--r--   0        0        0     1299 2021-04-27 20:50:33.772486 openstates-6.9.1/openstates/metadata/data/al.py
--rw-r--r--   0        0        0     1301 2021-04-27 20:50:33.772662 openstates-6.9.1/openstates/metadata/data/ar.py
--rw-r--r--   0        0        0     1299 2021-04-27 20:50:33.773262 openstates-6.9.1/openstates/metadata/data/az.py
--rw-r--r--   0        0        0     1311 2021-04-27 20:50:33.773573 openstates-6.9.1/openstates/metadata/data/ca.py
--rw-r--r--   0        0        0     1288 2021-04-27 20:50:33.773732 openstates-6.9.1/openstates/metadata/data/co.py
--rw-r--r--   0        0        0     1298 2021-04-27 20:50:33.773913 openstates-6.9.1/openstates/metadata/data/ct.py
--rw-r--r--   0        0        0     2170 2021-04-27 20:50:33.774170 openstates-6.9.1/openstates/metadata/data/dc.py
--rw-r--r--   0        0        0     1291 2021-04-27 20:50:33.774427 openstates-6.9.1/openstates/metadata/data/de.py
--rw-r--r--   0        0        0     1286 2021-04-27 20:50:33.774575 openstates-6.9.1/openstates/metadata/data/fl.py
--rw-r--r--   0        0        0     1291 2021-04-27 20:50:33.774691 openstates-6.9.1/openstates/metadata/data/ga.py
--rw-r--r--   0        0        0     1290 2021-04-27 20:50:33.774824 openstates-6.9.1/openstates/metadata/data/hi.py
--rw-r--r--   0        0        0     1290 2021-04-27 20:50:33.774952 openstates-6.9.1/openstates/metadata/data/ia.py
--rw-r--r--   0        0        0     1303 2021-04-27 20:50:33.775081 openstates-6.9.1/openstates/metadata/data/id.py
--rw-r--r--   0        0        0     1292 2021-04-27 20:50:33.775266 openstates-6.9.1/openstates/metadata/data/il.py
--rw-r--r--   0        0        0     1302 2021-04-27 20:50:33.775438 openstates-6.9.1/openstates/metadata/data/ind.py
--rw-r--r--   0        0        0     1293 2021-04-27 20:50:33.775557 openstates-6.9.1/openstates/metadata/data/ks.py
--rw-r--r--   0        0        0     1293 2021-04-27 20:50:33.775671 openstates-6.9.1/openstates/metadata/data/ky.py
--rw-r--r--   0        0        0     1293 2021-04-27 20:50:33.775797 openstates-6.9.1/openstates/metadata/data/la.py
--rw-r--r--   0        0        0     5085 2021-05-10 18:13:22.365057 openstates-6.9.1/openstates/metadata/data/legacy_districts.py
--rw-r--r--   0        0        0    38486 2021-04-27 20:50:33.776435 openstates-6.9.1/openstates/metadata/data/ma.py
--rw-r--r--   0        0        0     6888 2021-04-27 20:50:33.776624 openstates-6.9.1/openstates/metadata/data/md.py
--rw-r--r--   0        0        0     1286 2021-04-27 20:50:33.776770 openstates-6.9.1/openstates/metadata/data/me.py
--rw-r--r--   0        0        0     1293 2021-04-27 20:50:33.776903 openstates-6.9.1/openstates/metadata/data/mi.py
--rw-r--r--   0        0        0    12705 2021-04-27 20:50:33.777226 openstates-6.9.1/openstates/metadata/data/mn.py
--rw-r--r--   0        0        0     1298 2021-04-27 20:50:33.777411 openstates-6.9.1/openstates/metadata/data/mo.py
--rw-r--r--   0        0        0     1299 2021-04-27 20:50:33.777659 openstates-6.9.1/openstates/metadata/data/ms.py
--rw-r--r--   0        0        0     1277 2021-04-27 20:50:33.777825 openstates-6.9.1/openstates/metadata/data/mt.py
--rw-r--r--   0        0        0     1302 2021-04-27 20:50:33.778060 openstates-6.9.1/openstates/metadata/data/nc.py
--rw-r--r--   0        0        0     1328 2021-04-27 20:50:33.778205 openstates-6.9.1/openstates/metadata/data/nd.py
--rw-r--r--   0        0        0      993 2021-04-27 20:50:33.778324 openstates-6.9.1/openstates/metadata/data/ne.py
--rw-r--r--   0        0        0    38128 2021-04-27 20:50:33.778500 openstates-6.9.1/openstates/metadata/data/nh.py
--rw-r--r--   0        0        0     1312 2021-04-27 20:50:33.778650 openstates-6.9.1/openstates/metadata/data/nj.py
--rw-r--r--   0        0        0     1288 2021-04-27 20:50:33.779162 openstates-6.9.1/openstates/metadata/data/nm.py
--rw-r--r--   0        0        0     1296 2021-04-27 20:50:33.779296 openstates-6.9.1/openstates/metadata/data/nv.py
--rw-r--r--   0        0        0     1301 2021-04-27 20:50:33.779520 openstates-6.9.1/openstates/metadata/data/ny.py
--rw-r--r--   0        0        0     1295 2021-04-27 20:50:33.779661 openstates-6.9.1/openstates/metadata/data/oh.py
--rw-r--r--   0        0        0     1298 2021-04-27 20:50:33.779805 openstates-6.9.1/openstates/metadata/data/ok.py
--rw-r--r--   0        0        0     1296 2021-04-27 20:50:33.779929 openstates-6.9.1/openstates/metadata/data/ore.py
--rw-r--r--   0        0        0     1309 2021-04-27 20:50:33.780047 openstates-6.9.1/openstates/metadata/data/pa.py
--rw-r--r--   0        0        0     5593 2021-04-27 20:50:33.780872 openstates-6.9.1/openstates/metadata/data/pr.py
--rw-r--r--   0        0        0     1296 2021-04-27 20:50:33.781041 openstates-6.9.1/openstates/metadata/data/ri.py
--rw-r--r--   0        0        0     1305 2021-04-27 20:50:33.781178 openstates-6.9.1/openstates/metadata/data/sc.py
--rw-r--r--   0        0        0     4326 2021-04-27 20:50:33.781292 openstates-6.9.1/openstates/metadata/data/sd.py
--rw-r--r--   0        0        0     1366 2021-11-08 20:47:02.945237 openstates-6.9.1/openstates/metadata/data/states.py
--rw-r--r--   0        0        0     1296 2021-04-27 20:50:33.781404 openstates-6.9.1/openstates/metadata/data/tn.py
--rw-r--r--   0        0        0     1282 2021-04-27 20:50:33.781525 openstates-6.9.1/openstates/metadata/data/tx.py
--rw-r--r--   0        0        0     3881 2021-11-08 20:47:02.945996 openstates-6.9.1/openstates/metadata/data/us.py
--rw-r--r--   0        0        0     1284 2021-04-27 20:50:33.782181 openstates-6.9.1/openstates/metadata/data/ut.py
--rw-r--r--   0        0        0     1299 2021-04-27 20:50:33.782308 openstates-6.9.1/openstates/metadata/data/va.py
--rw-r--r--   0        0        0    22141 2021-04-27 20:50:33.782469 openstates-6.9.1/openstates/metadata/data/vt.py
--rw-r--r--   0        0        0     1309 2021-04-27 20:50:33.782649 openstates-6.9.1/openstates/metadata/data/wa.py
--rw-r--r--   0        0        0     1299 2021-04-27 20:50:33.782765 openstates-6.9.1/openstates/metadata/data/wi.py
--rw-r--r--   0        0        0     8132 2021-04-27 20:50:33.782870 openstates-6.9.1/openstates/metadata/data/wv.py
--rw-r--r--   0        0        0     1293 2021-04-27 20:50:33.782981 openstates-6.9.1/openstates/metadata/data/wy.py
--rw-r--r--   0        0        0     2747 2021-04-27 20:50:33.783649 openstates-6.9.1/openstates/metadata/models.py
--rw-r--r--   0        0        0        0 2021-04-27 20:50:33.783725 openstates-6.9.1/openstates/metadata/tests/__init__.py
--rw-r--r--   0        0        0     3044 2021-11-08 20:47:02.946722 openstates-6.9.1/openstates/metadata/tests/test_data.py
--rw-r--r--   0        0        0     3459 2021-11-08 20:47:02.947358 openstates-6.9.1/openstates/metadata/tests/test_helpers.py
--rw-r--r--   0        0        0      108 2021-07-02 18:34:41.247913 openstates-6.9.1/openstates/models/__init__.py
--rw-r--r--   0        0        0     3179 2021-11-08 21:09:17.054949 openstates-6.9.1/openstates/models/committees.py
--rw-r--r--   0        0        0     3428 2021-08-03 20:21:23.421651 openstates-6.9.1/openstates/models/common.py
--rw-r--r--   0        0        0     8762 2021-11-08 20:47:02.948494 openstates-6.9.1/openstates/models/people.py
--rw-r--r--   0        0        0        0 2021-07-02 18:28:03.538725 openstates-6.9.1/openstates/models/tests/__init__.py
--rw-r--r--   0        0        0     9843 2021-11-08 21:09:17.055369 openstates-6.9.1/openstates/models/tests/test_models.py
--rw-r--r--   0        0        0      281 2021-11-08 20:47:02.950177 openstates-6.9.1/openstates/scrape/__init__.py
--rw-r--r--   0        0        0    12243 2021-11-08 20:47:02.951049 openstates-6.9.1/openstates/scrape/base.py
--rw-r--r--   0        0        0     5643 2021-11-09 15:34:24.296489 openstates-6.9.1/openstates/scrape/bill.py
--rw-r--r--   0        0        0     6470 2021-11-08 20:47:02.951679 openstates-6.9.1/openstates/scrape/event.py
--rw-r--r--   0        0        0     3155 2021-11-08 20:47:02.952432 openstates-6.9.1/openstates/scrape/jurisdiction.py
--rw-r--r--   0        0        0     2205 2021-11-08 20:47:02.953756 openstates-6.9.1/openstates/scrape/popolo.py
--rw-r--r--   0        0        0        0 2020-04-08 21:23:57.764942 openstates-6.9.1/openstates/scrape/schemas/__init__.py
--rw-r--r--   0        0        0     5970 2021-11-09 15:34:24.297240 openstates-6.9.1/openstates/scrape/schemas/bill.py
--rw-r--r--   0        0        0     1623 2021-11-08 20:47:02.954623 openstates-6.9.1/openstates/scrape/schemas/common.py
--rw-r--r--   0        0        0     4663 2021-11-08 20:47:02.955696 openstates-6.9.1/openstates/scrape/schemas/event.py
--rw-r--r--   0        0        0     1016 2021-11-08 20:47:02.956436 openstates-6.9.1/openstates/scrape/schemas/jurisdiction.py
--rw-r--r--   0        0        0      731 2021-11-08 20:47:02.957186 openstates-6.9.1/openstates/scrape/schemas/organization.py
--rw-r--r--   0        0        0     1706 2021-04-27 20:50:33.790367 openstates-6.9.1/openstates/scrape/schemas/vote_event.py
--rw-r--r--   0        0        0        0 2020-04-08 21:23:57.767142 openstates-6.9.1/openstates/scrape/tests/__init__.py
--rw-r--r--   0        0        0     8629 2021-11-09 15:34:24.297896 openstates-6.9.1/openstates/scrape/tests/test_bill_scrape.py
--rw-r--r--   0        0        0     5755 2021-11-08 20:47:02.958029 openstates-6.9.1/openstates/scrape/tests/test_event_scrape.py
--rw-r--r--   0        0        0     1930 2021-11-08 20:47:02.958798 openstates-6.9.1/openstates/scrape/tests/test_jurisdiction_scrape.py
--rw-r--r--   0        0        0     3046 2021-11-08 20:47:02.959885 openstates-6.9.1/openstates/scrape/tests/test_model_basics.py
--rw-r--r--   0        0        0     4682 2021-11-08 20:47:02.960708 openstates-6.9.1/openstates/scrape/tests/test_scraper.py
--rw-r--r--   0        0        0     3408 2021-04-27 20:50:33.792727 openstates-6.9.1/openstates/scrape/tests/test_vote_event_scrape.py
--rw-r--r--   0        0        0     3179 2021-04-27 20:50:33.793227 openstates-6.9.1/openstates/scrape/vote_event.py
--rw-r--r--   0        0        0     1171 2021-11-08 20:47:02.961460 openstates-6.9.1/openstates/settings.py
--rw-r--r--   0        0        0      641 2021-08-02 18:12:37.034039 openstates-6.9.1/openstates/test_settings.py
--rw-r--r--   0        0        0      212 2020-04-22 18:59:48.470369 openstates-6.9.1/openstates/utils/__init__.py
--rw-r--r--   0        0        0     4913 2021-05-27 15:50:50.118440 openstates-6.9.1/openstates/utils/ansistrm.py
--rw-r--r--   0        0        0      690 2021-08-02 18:12:37.034545 openstates-6.9.1/openstates/utils/django.py
--rw-r--r--   0        0        0     2219 2021-05-27 15:56:07.106329 openstates-6.9.1/openstates/utils/generic.py
--rw-r--r--   0        0        0      212 2021-05-27 15:56:24.523654 openstates-6.9.1/openstates/utils/metadata.py
--rw-r--r--   0        0        0      272 2021-07-02 18:55:11.811945 openstates-6.9.1/openstates/utils/people/__init__.py
--rw-r--r--   0        0        0     3067 2021-07-27 17:36:01.616887 openstates-6.9.1/openstates/utils/people/general.py
--rw-r--r--   0        0        0     4060 2021-07-02 18:54:53.862860 openstates-6.9.1/openstates/utils/people/images.py
--rw-r--r--   0        0        0    13594 2021-11-08 20:47:02.963062 openstates-6.9.1/openstates/utils/people/lint_people.py
--rw-r--r--   0        0        0    15026 2021-11-09 21:20:22.997390 openstates-6.9.1/openstates/utils/people/merge.py
--rw-r--r--   0        0        0     1563 2021-11-08 20:47:02.964601 openstates-6.9.1/openstates/utils/people/retire.py
--rw-r--r--   0        0        0     9950 2021-11-08 20:47:02.965721 openstates-6.9.1/openstates/utils/people/to_database.py
--rw-r--r--   0        0        0        0 2021-05-25 18:40:17.132549 openstates-6.9.1/openstates/utils/tests/__init__.py
--rw-r--r--   0        0        0      497 2021-05-25 18:40:17.133151 openstates-6.9.1/openstates/utils/tests/django_test_settings.py
--rw-r--r--   0        0        0    12917 2021-11-08 21:09:17.055782 openstates-6.9.1/openstates/utils/tests/test_committees.py
--rw-r--r--   0        0        0     9605 2021-11-08 20:47:02.967632 openstates-6.9.1/openstates/utils/tests/test_lint.py
--rw-r--r--   0        0        0    10070 2021-11-08 20:47:02.980914 openstates-6.9.1/openstates/utils/tests/test_merge.py
--rw-r--r--   0        0        0     1143 2021-07-02 18:51:43.411066 openstates-6.9.1/openstates/utils/tests/test_retire.py
--rw-r--r--   0        0        0     1809 2021-11-08 20:47:02.969415 openstates-6.9.1/openstates/utils/tests/test_summarize.py
--rw-r--r--   0        0        0    11722 2021-11-08 21:09:17.056155 openstates-6.9.1/openstates/utils/tests/test_to_database.py
--rw-r--r--   0        0        0     1159 2021-05-27 15:57:05.871714 openstates-6.9.1/openstates/utils/tests/test_transformers.py
--rw-r--r--   0        0        0      369 2021-07-14 15:54:14.568081 openstates-6.9.1/openstates/utils/tests/testdata/broken-committees/lower-Broken-11111111-9999-9999-9999-222222222222.yml
--rw-r--r--   0        0        0      339 2021-07-14 15:54:18.813637 openstates-6.9.1/openstates/utils/tests/testdata/broken-committees/upper-Broken-11111111-9999-9999-9999-3333333333333.yml
--rw-r--r--   0        0        0      565 2021-07-14 15:52:19.484624 openstates-6.9.1/openstates/utils/tests/testdata/committees/lower-Agriculture-11111111-2222-3333-4444-111111111111.yml
--rw-r--r--   0        0        0      380 2021-07-14 15:53:33.380376 openstates-6.9.1/openstates/utils/tests/testdata/committees/lower-Education-11111111-2222-3333-4444-222222222222.yml
--rw-r--r--   0        0        0      312 2021-07-14 15:53:37.721140 openstates-6.9.1/openstates/utils/tests/testdata/committees/lower-Rules-11111111-2222-3333-4444-444444444444.yml
--rw-r--r--   0        0        0      372 2021-07-14 15:53:40.494001 openstates-6.9.1/openstates/utils/tests/testdata/committees/upper-Education-11111111-2222-3333-4444-3333333333333.yml
--rw-r--r--   0        0        0        0 2021-07-27 17:45:44.117637 openstates-6.9.1/openstates/utils/tests/testdata/data/EMPTY
--rw-r--r--   0        0        0     1258 2021-11-08 20:47:02.970843 openstates-6.9.1/openstates/utils/tests/testdata/people/data/pa/legislature/Pam-Snyder--a2e4a1b2-f0fd-4c35-9e0c-bb009778792f.yml
--rw-r--r--   0        0        0      730 2021-07-14 15:53:06.295239 openstates-6.9.1/openstates/utils/tests/testdata/scraped-committees/0d3e4bee-cbe3-4f9a-a732-1166e1a6c006.json
--rw-r--r--   0        0        0      894 2021-07-14 15:53:09.045606 openstates-6.9.1/openstates/utils/tests/testdata/scraped-committees/b0aabcb0-ad1c-4e05-af8f-3ec0c2de0fe2.json
--rw-r--r--   0        0        0      596 2021-05-27 15:50:29.217162 openstates-6.9.1/openstates/utils/transformers.py
--rw-r--r--   0        0        0     1349 2021-11-17 17:25:59.782643 openstates-6.9.1/pyproject.toml
--rw-r--r--   0        0        0     2421 2021-11-17 17:26:23.853771 openstates-6.9.1/setup.py
--rw-r--r--   0        0        0      970 2021-11-17 17:26:23.854034 openstates-6.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2021-04-27 20:50:33.722134 openstates-6.9.2/LICENSE
+-rw-r--r--   0        0        0        0 2020-04-08 21:23:57.750660 openstates-6.9.2/openstates/__init__.py
+-rw-r--r--   0        0        0        0 2021-05-03 14:50:07.647616 openstates-6.9.2/openstates/cli/__init__.py
+-rw-r--r--   0        0        0    20809 2021-11-08 20:47:02.920405 openstates-6.9.2/openstates/cli/committees.py
+-rw-r--r--   0        0        0    11295 2021-11-17 17:29:00.802912 openstates-6.9.2/openstates/cli/convert_us.py
+-rw-r--r--   0        0        0     2887 2021-11-29 18:23:42.104731 openstates-6.9.2/openstates/cli/initdb.py
+-rw-r--r--   0        0        0    22635 2021-11-08 20:47:02.922541 openstates-6.9.2/openstates/cli/people.py
+-rw-r--r--   0        0        0     6919 2021-08-02 18:12:37.031232 openstates-6.9.2/openstates/cli/reports.py
+-rw-r--r--   0        0        0        0 2020-04-08 21:23:57.751191 openstates-6.9.2/openstates/cli/tests/__init__.py
+-rw-r--r--   0        0        0     5904 2021-05-27 15:21:16.591627 openstates-6.9.2/openstates/cli/tests/test_initdb.py
+-rw-r--r--   0        0        0     8305 2021-05-27 15:21:16.592363 openstates-6.9.2/openstates/cli/tests/test_session_report.py
+-rw-r--r--   0        0        0      632 2021-05-27 15:21:16.593024 openstates-6.9.2/openstates/cli/tests/test_settings.py
+-rw-r--r--   0        0        0    12266 2021-05-27 18:31:42.033886 openstates-6.9.2/openstates/cli/text_extract.py
+-rw-r--r--   0        0        0    12229 2021-11-08 20:47:02.923680 openstates-6.9.2/openstates/cli/update.py
+-rw-r--r--   0        0        0      915 2021-05-27 18:18:32.164383 openstates-6.9.2/openstates/cli/update_computed.py
+-rw-r--r--   0        0        0        0 2020-04-08 21:23:57.751916 openstates-6.9.2/openstates/data/__init__.py
+-rw-r--r--   0        0        0       83 2020-04-08 21:23:57.752086 openstates-6.9.2/openstates/data/admin/__init__.py
+-rw-r--r--   0        0        0     1417 2021-11-09 21:20:22.981644 openstates-6.9.2/openstates/data/admin/base.py
+-rw-r--r--   0        0        0     4245 2021-11-09 21:20:22.983118 openstates-6.9.2/openstates/data/admin/bill.py
+-rw-r--r--   0        0        0     2373 2021-11-08 20:47:02.926101 openstates-6.9.2/openstates/data/admin/event.py
+-rw-r--r--   0        0        0     3573 2021-11-09 21:20:22.983480 openstates-6.9.2/openstates/data/admin/organization.py
+-rw-r--r--   0        0        0     2910 2021-11-09 21:20:22.983825 openstates-6.9.2/openstates/data/admin/other.py
+-rw-r--r--   0        0        0     2704 2021-11-09 21:20:22.984175 openstates-6.9.2/openstates/data/admin/person.py
+-rw-r--r--   0        0        0     2497 2021-11-09 21:20:22.985495 openstates-6.9.2/openstates/data/admin/reports.py
+-rw-r--r--   0        0        0     1783 2021-11-09 21:20:22.986820 openstates-6.9.2/openstates/data/admin/vote.py
+-rw-r--r--   0        0        0     6628 2021-11-09 15:34:24.292111 openstates-6.9.2/openstates/data/common.py
+-rw-r--r--   0        0        0   104004 2020-09-14 15:27:39.435524 openstates-6.9.2/openstates/data/migrations/0001_initial.py
+-rw-r--r--   0        0        0      830 2020-04-23 19:18:11.574663 openstates-6.9.2/openstates/data/migrations/0002_auto_20200422_0028.py
+-rw-r--r--   0        0        0      406 2020-04-23 19:18:11.574832 openstates-6.9.2/openstates/data/migrations/0003_auto_20200422_0031.py
+-rw-r--r--   0        0        0      435 2020-04-23 19:18:11.574984 openstates-6.9.2/openstates/data/migrations/0004_auto_20200422_0040.py
+-rw-r--r--   0        0        0      692 2020-04-23 19:18:11.575081 openstates-6.9.2/openstates/data/migrations/0005_auto_20200423_1100.py
+-rw-r--r--   0        0        0      899 2020-04-23 19:18:11.575169 openstates-6.9.2/openstates/data/migrations/0006_auto_20200423_1124.py
+-rw-r--r--   0        0        0      951 2020-04-23 19:17:07.852276 openstates-6.9.2/openstates/data/migrations/0007_auto_20200423_1416.py
+-rw-r--r--   0        0        0      383 2020-04-28 20:31:10.014271 openstates-6.9.2/openstates/data/migrations/0008_person_current_state.py
+-rw-r--r--   0        0        0      948 2020-04-29 14:13:13.638348 openstates-6.9.2/openstates/data/migrations/0009_auto_20200429_0913.py
+-rw-r--r--   0        0        0      659 2020-07-22 15:56:29.521217 openstates-6.9.2/openstates/data/migrations/0010_auto_20200721_1604.py
+-rw-r--r--   0        0        0      928 2021-04-27 20:50:33.732106 openstates-6.9.2/openstates/data/migrations/0011_auto_20200804_1108.py
+-rw-r--r--   0        0        0      477 2020-08-04 20:24:15.725857 openstates-6.9.2/openstates/data/migrations/0012_person_current_role.py
+-rw-r--r--   0        0        0      268 2020-08-04 21:54:20.987895 openstates-6.9.2/openstates/data/migrations/0013_remove_person_current_state.py
+-rw-r--r--   0        0        0      301 2020-08-05 19:03:00.654334 openstates-6.9.2/openstates/data/migrations/0014_remove_person_current_role_division_id.py
+-rw-r--r--   0        0        0      601 2021-04-27 20:50:33.732795 openstates-6.9.2/openstates/data/migrations/0015_auto_20200811_1009.py
+-rw-r--r--   0        0        0      636 2021-04-27 20:50:33.733613 openstates-6.9.2/openstates/data/migrations/0016_auto_20200811_1016.py
+-rw-r--r--   0        0        0      326 2021-04-27 20:50:33.734102 openstates-6.9.2/openstates/data/migrations/0017_remove_person_summary.py
+-rw-r--r--   0        0        0     1119 2021-04-27 20:50:33.734692 openstates-6.9.2/openstates/data/migrations/0018_auto_20200914_1032.py
+-rw-r--r--   0        0        0      329 2021-04-27 20:50:33.735213 openstates-6.9.2/openstates/data/migrations/0019_remove_billabstract_date.py
+-rw-r--r--   0        0        0      448 2021-04-27 20:50:33.735738 openstates-6.9.2/openstates/data/migrations/0020_auto_20200914_1041.py
+-rw-r--r--   0        0        0      338 2021-04-27 20:50:33.736473 openstates-6.9.2/openstates/data/migrations/0021_remove_jurisdiction_feature_flags.py
+-rw-r--r--   0        0        0      580 2021-04-27 20:50:33.737107 openstates-6.9.2/openstates/data/migrations/0022_auto_20200914_1054.py
+-rw-r--r--   0        0        0      337 2021-04-27 20:50:33.737589 openstates-6.9.2/openstates/data/migrations/0023_remove_personcontactdetail_label.py
+-rw-r--r--   0        0        0      444 2021-04-27 20:50:33.738109 openstates-6.9.2/openstates/data/migrations/0024_auto_20200914_1101.py
+-rw-r--r--   0        0        0      779 2021-04-27 20:50:33.738527 openstates-6.9.2/openstates/data/migrations/0025_auto_20200914_1216.py
+-rw-r--r--   0        0        0     2551 2021-04-27 20:50:33.739141 openstates-6.9.2/openstates/data/migrations/0026_auto_20200923_1312.py
+-rw-r--r--   0        0        0      424 2021-04-27 20:50:33.740075 openstates-6.9.2/openstates/data/migrations/0027_auto_20200923_1329.py
+-rw-r--r--   0        0        0      836 2021-04-27 20:50:33.741563 openstates-6.9.2/openstates/data/migrations/0028_auto_20201022_1642.py
+-rw-r--r--   0        0        0      389 2021-04-27 20:50:33.742302 openstates-6.9.2/openstates/data/migrations/0029_auto_20210203_1946.py
+-rw-r--r--   0        0        0      718 2021-04-27 20:50:33.743670 openstates-6.9.2/openstates/data/migrations/0030_auto_20210210_1817.py
+-rw-r--r--   0        0        0      914 2021-04-27 20:50:33.744238 openstates-6.9.2/openstates/data/migrations/0031_auto_20210401_1449.py
+-rw-r--r--   0        0        0      396 2021-04-27 20:50:33.745131 openstates-6.9.2/openstates/data/migrations/0032_event_dedupe_key.py
+-rw-r--r--   0        0        0     1001 2021-04-27 20:50:33.745990 openstates-6.9.2/openstates/data/migrations/0033_auto_20210421_1538.py
+-rw-r--r--   0        0        0      497 2021-04-27 20:50:33.746846 openstates-6.9.2/openstates/data/migrations/0034_organization_other_names.py
+-rw-r--r--   0        0        0     3813 2021-04-27 20:50:33.747386 openstates-6.9.2/openstates/data/migrations/0035_auto_20210422_1926.py
+-rw-r--r--   0        0        0      634 2021-08-02 17:52:53.007515 openstates-6.9.2/openstates/data/migrations/0036_auto_20210802_1752.py
+-rw-r--r--   0        0        0     7214 2021-08-02 18:12:37.032552 openstates-6.9.2/openstates/data/migrations/0037_importobjects_runplan_scrapeobjects_scrapereport_sessiondataqualityreport.py
+-rw-r--r--   0        0        0      642 2021-11-08 20:47:02.929058 openstates-6.9.2/openstates/data/migrations/0038_auto_20210914_1559.py
+-rw-r--r--   0        0        0      807 2021-11-08 20:47:02.929639 openstates-6.9.2/openstates/data/migrations/0039_auto_20210920_1934.py
+-rw-r--r--   0        0        0     1203 2021-11-08 20:47:02.930372 openstates-6.9.2/openstates/data/migrations/0040_auto_20210920_2347.py
+-rw-r--r--   0        0        0     1810 2021-11-08 20:47:02.930894 openstates-6.9.2/openstates/data/migrations/0041_personoffice.py
+-rw-r--r--   0        0        0      299 2021-11-08 20:47:02.931410 openstates-6.9.2/openstates/data/migrations/0042_delete_personcontactdetail.py
+-rw-r--r--   0        0        0      404 2021-11-08 20:47:02.933013 openstates-6.9.2/openstates/data/migrations/0043_legislativesession_active.py
+-rw-r--r--   0        0        0      435 2021-11-09 15:34:24.293472 openstates-6.9.2/openstates/data/migrations/0044_bill_citations.py
+-rw-r--r--   0        0        0        0 2020-04-08 21:23:57.754015 openstates-6.9.2/openstates/data/migrations/__init__.py
+-rw-r--r--   0        0        0      926 2021-11-08 20:47:02.933871 openstates-6.9.2/openstates/data/models/__init__.py
+-rw-r--r--   0        0        0     4280 2021-11-08 20:47:02.934502 openstates-6.9.2/openstates/data/models/base.py
+-rw-r--r--   0        0        0     8257 2021-11-09 15:34:24.295220 openstates-6.9.2/openstates/data/models/bill.py
+-rw-r--r--   0        0        0     4901 2020-04-08 21:23:57.754813 openstates-6.9.2/openstates/data/models/division.py
+-rw-r--r--   0        0        0     6138 2021-11-08 20:47:02.935417 openstates-6.9.2/openstates/data/models/event.py
+-rw-r--r--   0        0        0     2436 2021-11-08 20:47:02.936115 openstates-6.9.2/openstates/data/models/jurisdiction.py
+-rw-r--r--   0        0        0    12495 2021-11-08 20:47:02.936924 openstates-6.9.2/openstates/data/models/people_orgs.py
+-rw-r--r--   0        0        0     2882 2021-08-02 18:12:37.033618 openstates-6.9.2/openstates/data/models/reports.py
+-rw-r--r--   0        0        0     3425 2021-04-27 20:50:33.753470 openstates-6.9.2/openstates/data/models/vote.py
+-rw-r--r--   0        0        0        0 2020-04-08 21:23:57.756106 openstates-6.9.2/openstates/data/tests/__init__.py
+-rw-r--r--   0        0        0     3458 2021-04-27 20:50:33.754129 openstates-6.9.2/openstates/data/tests/conftest.py
+-rw-r--r--   0        0        0    15627 2021-11-08 20:47:02.937864 openstates-6.9.2/openstates/data/tests/test_models.py
+-rw-r--r--   0        0        0     1814 2021-11-08 20:47:02.938676 openstates-6.9.2/openstates/exceptions.py
+-rw-r--r--   0        0        0     5624 2021-05-27 15:49:11.275776 openstates-6.9.2/openstates/fulltext/__init__.py
+-rw-r--r--   0        0        0     4539 2021-05-27 15:49:28.760071 openstates-6.9.2/openstates/fulltext/common.py
+-rw-r--r--   0        0        0     1406 2021-05-27 15:42:46.026934 openstates-6.9.2/openstates/fulltext/de.py
+-rw-r--r--   0        0        0    19582 2021-05-12 16:17:42.440947 openstates-6.9.2/openstates/fulltext/raw/ak.csv
+-rw-r--r--   0        0        0    17854 2021-05-12 16:17:42.441694 openstates-6.9.2/openstates/fulltext/raw/al.csv
+-rw-r--r--   0        0        0    15635 2021-05-12 16:17:42.442002 openstates-6.9.2/openstates/fulltext/raw/ar.csv
+-rw-r--r--   0        0        0    13377 2021-05-12 16:17:42.442183 openstates-6.9.2/openstates/fulltext/raw/az.csv
+-rw-r--r--   0        0        0    14336 2021-05-12 16:17:42.442624 openstates-6.9.2/openstates/fulltext/raw/ca.csv
+-rw-r--r--   0        0        0    13723 2021-05-12 16:17:42.443447 openstates-6.9.2/openstates/fulltext/raw/co.csv
+-rw-r--r--   0        0        0    13619 2021-05-12 16:17:42.443796 openstates-6.9.2/openstates/fulltext/raw/ct.csv
+-rw-r--r--   0        0        0    13844 2021-05-12 16:17:42.443982 openstates-6.9.2/openstates/fulltext/raw/dc.csv
+-rw-r--r--   0        0        0    35228 2021-05-12 16:17:42.444228 openstates-6.9.2/openstates/fulltext/raw/de.csv
+-rw-r--r--   0        0        0    11260 2021-05-12 16:17:42.444710 openstates-6.9.2/openstates/fulltext/raw/fl.csv
+-rw-r--r--   0        0        0    14157 2021-05-12 16:17:42.445573 openstates-6.9.2/openstates/fulltext/raw/ga.csv
+-rw-r--r--   0        0        0    25367 2021-05-12 16:17:42.445896 openstates-6.9.2/openstates/fulltext/raw/hi.csv
+-rw-r--r--   0        0        0    43184 2021-05-12 16:17:42.446261 openstates-6.9.2/openstates/fulltext/raw/ia.csv
+-rw-r--r--   0        0        0    19435 2021-05-12 16:17:42.446760 openstates-6.9.2/openstates/fulltext/raw/id.csv
+-rw-r--r--   0        0        0    14703 2021-05-12 16:17:42.447050 openstates-6.9.2/openstates/fulltext/raw/il.csv
+-rw-r--r--   0        0        0    14440 2021-05-12 16:17:42.447533 openstates-6.9.2/openstates/fulltext/raw/in.csv
+-rw-r--r--   0        0        0    15777 2021-05-12 16:17:42.447834 openstates-6.9.2/openstates/fulltext/raw/ks.csv
+-rw-r--r--   0        0        0     3714 2021-05-12 16:17:42.448713 openstates-6.9.2/openstates/fulltext/raw/ky.csv
+-rw-r--r--   0        0        0    16826 2021-05-12 16:17:42.449309 openstates-6.9.2/openstates/fulltext/raw/la.csv
+-rw-r--r--   0        0        0    12313 2021-05-12 16:17:42.449846 openstates-6.9.2/openstates/fulltext/raw/ma.csv
+-rw-r--r--   0        0        0    18330 2021-05-12 16:17:42.450401 openstates-6.9.2/openstates/fulltext/raw/md.csv
+-rw-r--r--   0        0        0    46138 2021-05-12 16:17:42.451133 openstates-6.9.2/openstates/fulltext/raw/me.csv
+-rw-r--r--   0        0        0    20401 2021-05-12 16:17:42.451417 openstates-6.9.2/openstates/fulltext/raw/mi.csv
+-rw-r--r--   0        0        0    17150 2021-05-12 16:17:42.451893 openstates-6.9.2/openstates/fulltext/raw/mn.csv
+-rw-r--r--   0        0        0    14045 2021-05-12 16:17:42.452206 openstates-6.9.2/openstates/fulltext/raw/mo.csv
+-rw-r--r--   0        0        0    16563 2021-05-12 16:17:42.452768 openstates-6.9.2/openstates/fulltext/raw/ms.csv
+-rw-r--r--   0        0        0    11531 2021-05-12 16:17:42.453211 openstates-6.9.2/openstates/fulltext/raw/mt.csv
+-rw-r--r--   0        0        0    11173 2021-05-12 16:17:42.453834 openstates-6.9.2/openstates/fulltext/raw/nc.csv
+-rw-r--r--   0        0        0    26171 2021-05-12 16:17:42.454853 openstates-6.9.2/openstates/fulltext/raw/nd.csv
+-rw-r--r--   0        0        0    14434 2021-05-12 16:17:42.455073 openstates-6.9.2/openstates/fulltext/raw/ne.csv
+-rw-r--r--   0        0        0    14745 2021-05-12 16:17:42.455827 openstates-6.9.2/openstates/fulltext/raw/nh.csv
+-rw-r--r--   0        0        0    15796 2021-05-12 16:17:42.456384 openstates-6.9.2/openstates/fulltext/raw/nj.csv
+-rw-r--r--   0        0        0    21601 2021-05-12 16:17:42.456967 openstates-6.9.2/openstates/fulltext/raw/nm.csv
+-rw-r--r--   0        0        0    14776 2021-05-12 16:17:42.457422 openstates-6.9.2/openstates/fulltext/raw/nv.csv
+-rw-r--r--   0        0        0    14076 2021-05-12 16:17:42.458172 openstates-6.9.2/openstates/fulltext/raw/ny.csv
+-rw-r--r--   0        0        0    15120 2021-05-12 16:17:42.458362 openstates-6.9.2/openstates/fulltext/raw/oh.csv
+-rw-r--r--   0        0        0    16028 2021-05-12 16:17:42.458768 openstates-6.9.2/openstates/fulltext/raw/ok.csv
+-rw-r--r--   0        0        0    15374 2021-05-12 16:17:42.458925 openstates-6.9.2/openstates/fulltext/raw/or.csv
+-rw-r--r--   0        0        0    78160 2021-05-12 16:17:42.467107 openstates-6.9.2/openstates/fulltext/raw/pa.csv
+-rw-r--r--   0        0        0    40360 2021-05-12 16:17:42.467850 openstates-6.9.2/openstates/fulltext/raw/pr.csv
+-rw-r--r--   0        0        0    21447 2021-05-12 16:17:42.468097 openstates-6.9.2/openstates/fulltext/raw/ri.csv
+-rw-r--r--   0        0        0    46905 2021-05-12 16:17:42.468684 openstates-6.9.2/openstates/fulltext/raw/sc.csv
+-rw-r--r--   0        0        0    16878 2021-05-12 16:17:42.468877 openstates-6.9.2/openstates/fulltext/raw/sd.csv
+-rw-r--r--   0        0        0    20147 2021-05-12 16:17:42.469390 openstates-6.9.2/openstates/fulltext/raw/tn.csv
+-rw-r--r--   0        0        0    16034 2021-05-12 16:17:42.469573 openstates-6.9.2/openstates/fulltext/raw/tx.csv
+-rw-r--r--   0        0        0    11264 2021-05-12 16:17:42.469900 openstates-6.9.2/openstates/fulltext/raw/ut.csv
+-rw-r--r--   0        0        0    14596 2021-05-12 16:17:42.470402 openstates-6.9.2/openstates/fulltext/raw/va.csv
+-rw-r--r--   0        0        0     5071 2021-05-12 16:17:42.470793 openstates-6.9.2/openstates/fulltext/raw/vt.csv
+-rw-r--r--   0        0        0    14440 2021-05-12 16:17:42.471009 openstates-6.9.2/openstates/fulltext/raw/wa.csv
+-rw-r--r--   0        0        0    30123 2021-05-12 16:17:42.471355 openstates-6.9.2/openstates/fulltext/raw/wi.csv
+-rw-r--r--   0        0        0    15620 2021-05-12 16:17:42.471525 openstates-6.9.2/openstates/fulltext/raw/wv.csv
+-rw-r--r--   0        0        0    11653 2021-05-12 16:17:42.471668 openstates-6.9.2/openstates/fulltext/raw/wy.csv
+-rw-r--r--   0        0        0     3463 2021-05-27 15:44:58.883825 openstates-6.9.2/openstates/fulltext/utils.py
+-rw-r--r--   0        0        0      219 2021-04-27 20:50:33.755355 openstates-6.9.2/openstates/importers/__init__.py
+-rw-r--r--   0        0        0      508 2021-06-02 18:30:04.723456 openstates-6.9.2/openstates/importers/_types.py
+-rw-r--r--   0        0        0    21576 2021-11-08 20:47:02.939585 openstates-6.9.2/openstates/importers/base.py
+-rw-r--r--   0        0        0     4863 2021-09-24 17:45:55.743994 openstates-6.9.2/openstates/importers/bills.py
+-rw-r--r--   0        0        0     1630 2021-04-27 20:50:33.759845 openstates-6.9.2/openstates/importers/computed_fields.py
+-rw-r--r--   0        0        0     4454 2021-11-08 20:47:02.940907 openstates-6.9.2/openstates/importers/events.py
+-rw-r--r--   0        0        0      787 2021-04-27 20:50:33.761291 openstates-6.9.2/openstates/importers/jurisdiction.py
+-rw-r--r--   0        0        0      519 2021-06-02 18:30:04.724224 openstates-6.9.2/openstates/importers/organizations.py
+-rw-r--r--   0        0        0        0 2020-04-08 21:23:57.759804 openstates-6.9.2/openstates/importers/tests/__init__.py
+-rw-r--r--   0        0        0     7567 2021-11-08 20:47:02.941724 openstates-6.9.2/openstates/importers/tests/test_base_importer.py
+-rw-r--r--   0        0        0    18087 2021-04-27 20:50:33.763811 openstates-6.9.2/openstates/importers/tests/test_bill_importer.py
+-rw-r--r--   0        0        0     1648 2020-04-24 22:15:15.291393 openstates-6.9.2/openstates/importers/tests/test_computed_fields.py
+-rw-r--r--   0        0        0    11463 2021-11-08 20:47:02.942772 openstates-6.9.2/openstates/importers/tests/test_event_importer.py
+-rw-r--r--   0        0        0     2502 2021-11-08 20:47:02.943546 openstates-6.9.2/openstates/importers/tests/test_jurisdiction_importer.py
+-rw-r--r--   0        0        0    17020 2021-04-27 20:50:33.765562 openstates-6.9.2/openstates/importers/tests/test_vote_event_importer.py
+-rw-r--r--   0        0        0     5472 2021-04-27 20:50:33.766493 openstates-6.9.2/openstates/importers/vote_events.py
+-rw-r--r--   0        0        0     2067 2021-04-27 20:50:33.767456 openstates-6.9.2/openstates/metadata/__init__.py
+-rwxr-xr-x   0        0        0      516 2021-04-27 20:50:33.768557 openstates-6.9.2/openstates/metadata/_creation/create_data.sh
+-rw-r--r--   0        0        0     6155 2021-04-27 20:50:33.768976 openstates-6.9.2/openstates/metadata/_creation/jurisdictions.csv
+-rw-r--r--   0        0        0    23390 2021-04-27 20:50:33.769240 openstates-6.9.2/openstates/metadata/_creation/orgs.csv
+-rw-r--r--   0        0        0    36641 2021-04-27 20:50:33.770331 openstates-6.9.2/openstates/metadata/_creation/settings.yml
+-rw-r--r--   0        0        0     7059 2021-05-27 16:03:25.911262 openstates-6.9.2/openstates/metadata/_creation/write_data.py
+-rw-r--r--   0        0        0      344 2021-11-08 20:47:02.944419 openstates-6.9.2/openstates/metadata/data/__init__.py
+-rw-r--r--   0        0        0     2857 2021-04-27 20:50:33.772048 openstates-6.9.2/openstates/metadata/data/ak.py
+-rw-r--r--   0        0        0     1299 2021-04-27 20:50:33.772486 openstates-6.9.2/openstates/metadata/data/al.py
+-rw-r--r--   0        0        0     1301 2021-04-27 20:50:33.772662 openstates-6.9.2/openstates/metadata/data/ar.py
+-rw-r--r--   0        0        0     1299 2021-04-27 20:50:33.773262 openstates-6.9.2/openstates/metadata/data/az.py
+-rw-r--r--   0        0        0     1311 2021-04-27 20:50:33.773573 openstates-6.9.2/openstates/metadata/data/ca.py
+-rw-r--r--   0        0        0     1288 2021-04-27 20:50:33.773732 openstates-6.9.2/openstates/metadata/data/co.py
+-rw-r--r--   0        0        0     1298 2021-04-27 20:50:33.773913 openstates-6.9.2/openstates/metadata/data/ct.py
+-rw-r--r--   0        0        0     2170 2021-04-27 20:50:33.774170 openstates-6.9.2/openstates/metadata/data/dc.py
+-rw-r--r--   0        0        0     1291 2021-04-27 20:50:33.774427 openstates-6.9.2/openstates/metadata/data/de.py
+-rw-r--r--   0        0        0     1286 2021-04-27 20:50:33.774575 openstates-6.9.2/openstates/metadata/data/fl.py
+-rw-r--r--   0        0        0     1291 2021-04-27 20:50:33.774691 openstates-6.9.2/openstates/metadata/data/ga.py
+-rw-r--r--   0        0        0     1290 2021-04-27 20:50:33.774824 openstates-6.9.2/openstates/metadata/data/hi.py
+-rw-r--r--   0        0        0     1290 2021-04-27 20:50:33.774952 openstates-6.9.2/openstates/metadata/data/ia.py
+-rw-r--r--   0        0        0     1303 2021-04-27 20:50:33.775081 openstates-6.9.2/openstates/metadata/data/id.py
+-rw-r--r--   0        0        0     1292 2021-04-27 20:50:33.775266 openstates-6.9.2/openstates/metadata/data/il.py
+-rw-r--r--   0        0        0     1302 2021-04-27 20:50:33.775438 openstates-6.9.2/openstates/metadata/data/ind.py
+-rw-r--r--   0        0        0     1293 2021-04-27 20:50:33.775557 openstates-6.9.2/openstates/metadata/data/ks.py
+-rw-r--r--   0        0        0     1293 2021-04-27 20:50:33.775671 openstates-6.9.2/openstates/metadata/data/ky.py
+-rw-r--r--   0        0        0     1293 2021-04-27 20:50:33.775797 openstates-6.9.2/openstates/metadata/data/la.py
+-rw-r--r--   0        0        0     5085 2021-05-10 18:13:22.365057 openstates-6.9.2/openstates/metadata/data/legacy_districts.py
+-rw-r--r--   0        0        0    38486 2021-04-27 20:50:33.776435 openstates-6.9.2/openstates/metadata/data/ma.py
+-rw-r--r--   0        0        0     6888 2021-04-27 20:50:33.776624 openstates-6.9.2/openstates/metadata/data/md.py
+-rw-r--r--   0        0        0     1286 2021-04-27 20:50:33.776770 openstates-6.9.2/openstates/metadata/data/me.py
+-rw-r--r--   0        0        0     1293 2021-04-27 20:50:33.776903 openstates-6.9.2/openstates/metadata/data/mi.py
+-rw-r--r--   0        0        0    12705 2021-04-27 20:50:33.777226 openstates-6.9.2/openstates/metadata/data/mn.py
+-rw-r--r--   0        0        0     1298 2021-04-27 20:50:33.777411 openstates-6.9.2/openstates/metadata/data/mo.py
+-rw-r--r--   0        0        0     1299 2021-04-27 20:50:33.777659 openstates-6.9.2/openstates/metadata/data/ms.py
+-rw-r--r--   0        0        0     1277 2021-04-27 20:50:33.777825 openstates-6.9.2/openstates/metadata/data/mt.py
+-rw-r--r--   0        0        0     1302 2021-04-27 20:50:33.778060 openstates-6.9.2/openstates/metadata/data/nc.py
+-rw-r--r--   0        0        0     1328 2021-04-27 20:50:33.778205 openstates-6.9.2/openstates/metadata/data/nd.py
+-rw-r--r--   0        0        0      993 2021-04-27 20:50:33.778324 openstates-6.9.2/openstates/metadata/data/ne.py
+-rw-r--r--   0        0        0    38128 2021-04-27 20:50:33.778500 openstates-6.9.2/openstates/metadata/data/nh.py
+-rw-r--r--   0        0        0     1312 2021-04-27 20:50:33.778650 openstates-6.9.2/openstates/metadata/data/nj.py
+-rw-r--r--   0        0        0     1288 2021-04-27 20:50:33.779162 openstates-6.9.2/openstates/metadata/data/nm.py
+-rw-r--r--   0        0        0     1296 2021-04-27 20:50:33.779296 openstates-6.9.2/openstates/metadata/data/nv.py
+-rw-r--r--   0        0        0     1301 2021-04-27 20:50:33.779520 openstates-6.9.2/openstates/metadata/data/ny.py
+-rw-r--r--   0        0        0     1295 2021-04-27 20:50:33.779661 openstates-6.9.2/openstates/metadata/data/oh.py
+-rw-r--r--   0        0        0     1298 2021-04-27 20:50:33.779805 openstates-6.9.2/openstates/metadata/data/ok.py
+-rw-r--r--   0        0        0     1296 2021-04-27 20:50:33.779929 openstates-6.9.2/openstates/metadata/data/ore.py
+-rw-r--r--   0        0        0     1309 2021-04-27 20:50:33.780047 openstates-6.9.2/openstates/metadata/data/pa.py
+-rw-r--r--   0        0        0     5593 2021-04-27 20:50:33.780872 openstates-6.9.2/openstates/metadata/data/pr.py
+-rw-r--r--   0        0        0     1296 2021-04-27 20:50:33.781041 openstates-6.9.2/openstates/metadata/data/ri.py
+-rw-r--r--   0        0        0     1305 2021-04-27 20:50:33.781178 openstates-6.9.2/openstates/metadata/data/sc.py
+-rw-r--r--   0        0        0     4326 2021-04-27 20:50:33.781292 openstates-6.9.2/openstates/metadata/data/sd.py
+-rw-r--r--   0        0        0     1366 2021-11-08 20:47:02.945237 openstates-6.9.2/openstates/metadata/data/states.py
+-rw-r--r--   0        0        0     1296 2021-04-27 20:50:33.781404 openstates-6.9.2/openstates/metadata/data/tn.py
+-rw-r--r--   0        0        0     1282 2021-04-27 20:50:33.781525 openstates-6.9.2/openstates/metadata/data/tx.py
+-rw-r--r--   0        0        0     3881 2021-11-08 20:47:02.945996 openstates-6.9.2/openstates/metadata/data/us.py
+-rw-r--r--   0        0        0     1284 2021-04-27 20:50:33.782181 openstates-6.9.2/openstates/metadata/data/ut.py
+-rw-r--r--   0        0        0     1299 2021-04-27 20:50:33.782308 openstates-6.9.2/openstates/metadata/data/va.py
+-rw-r--r--   0        0        0    22141 2021-04-27 20:50:33.782469 openstates-6.9.2/openstates/metadata/data/vt.py
+-rw-r--r--   0        0        0     1309 2021-04-27 20:50:33.782649 openstates-6.9.2/openstates/metadata/data/wa.py
+-rw-r--r--   0        0        0     1299 2021-04-27 20:50:33.782765 openstates-6.9.2/openstates/metadata/data/wi.py
+-rw-r--r--   0        0        0     8132 2021-04-27 20:50:33.782870 openstates-6.9.2/openstates/metadata/data/wv.py
+-rw-r--r--   0        0        0     1293 2021-04-27 20:50:33.782981 openstates-6.9.2/openstates/metadata/data/wy.py
+-rw-r--r--   0        0        0     2747 2021-04-27 20:50:33.783649 openstates-6.9.2/openstates/metadata/models.py
+-rw-r--r--   0        0        0        0 2021-04-27 20:50:33.783725 openstates-6.9.2/openstates/metadata/tests/__init__.py
+-rw-r--r--   0        0        0     3044 2021-11-08 20:47:02.946722 openstates-6.9.2/openstates/metadata/tests/test_data.py
+-rw-r--r--   0        0        0     3459 2021-11-08 20:47:02.947358 openstates-6.9.2/openstates/metadata/tests/test_helpers.py
+-rw-r--r--   0        0        0      108 2021-07-02 18:34:41.247913 openstates-6.9.2/openstates/models/__init__.py
+-rw-r--r--   0        0        0     3352 2021-11-18 16:29:28.164046 openstates-6.9.2/openstates/models/committees.py
+-rw-r--r--   0        0        0     3428 2021-08-03 20:21:23.421651 openstates-6.9.2/openstates/models/common.py
+-rw-r--r--   0        0        0     8762 2021-11-08 20:47:02.948494 openstates-6.9.2/openstates/models/people.py
+-rw-r--r--   0        0        0        0 2021-07-02 18:28:03.538725 openstates-6.9.2/openstates/models/tests/__init__.py
+-rw-r--r--   0        0        0     9843 2021-11-08 21:09:17.055369 openstates-6.9.2/openstates/models/tests/test_models.py
+-rw-r--r--   0        0        0      281 2021-11-08 20:47:02.950177 openstates-6.9.2/openstates/scrape/__init__.py
+-rw-r--r--   0        0        0    12243 2021-11-08 20:47:02.951049 openstates-6.9.2/openstates/scrape/base.py
+-rw-r--r--   0        0        0     5643 2021-11-09 15:34:24.296489 openstates-6.9.2/openstates/scrape/bill.py
+-rw-r--r--   0        0        0     6470 2021-11-08 20:47:02.951679 openstates-6.9.2/openstates/scrape/event.py
+-rw-r--r--   0        0        0     3155 2021-11-08 20:47:02.952432 openstates-6.9.2/openstates/scrape/jurisdiction.py
+-rw-r--r--   0        0        0     2205 2021-11-08 20:47:02.953756 openstates-6.9.2/openstates/scrape/popolo.py
+-rw-r--r--   0        0        0        0 2020-04-08 21:23:57.764942 openstates-6.9.2/openstates/scrape/schemas/__init__.py
+-rw-r--r--   0        0        0     5970 2021-11-09 15:34:24.297240 openstates-6.9.2/openstates/scrape/schemas/bill.py
+-rw-r--r--   0        0        0     1623 2021-11-08 20:47:02.954623 openstates-6.9.2/openstates/scrape/schemas/common.py
+-rw-r--r--   0        0        0     4663 2021-11-08 20:47:02.955696 openstates-6.9.2/openstates/scrape/schemas/event.py
+-rw-r--r--   0        0        0     1016 2021-11-08 20:47:02.956436 openstates-6.9.2/openstates/scrape/schemas/jurisdiction.py
+-rw-r--r--   0        0        0      731 2021-11-08 20:47:02.957186 openstates-6.9.2/openstates/scrape/schemas/organization.py
+-rw-r--r--   0        0        0     1706 2021-04-27 20:50:33.790367 openstates-6.9.2/openstates/scrape/schemas/vote_event.py
+-rw-r--r--   0        0        0        0 2020-04-08 21:23:57.767142 openstates-6.9.2/openstates/scrape/tests/__init__.py
+-rw-r--r--   0        0        0     8629 2021-11-09 15:34:24.297896 openstates-6.9.2/openstates/scrape/tests/test_bill_scrape.py
+-rw-r--r--   0        0        0     5755 2021-11-08 20:47:02.958029 openstates-6.9.2/openstates/scrape/tests/test_event_scrape.py
+-rw-r--r--   0        0        0     1930 2021-11-08 20:47:02.958798 openstates-6.9.2/openstates/scrape/tests/test_jurisdiction_scrape.py
+-rw-r--r--   0        0        0     3046 2021-11-08 20:47:02.959885 openstates-6.9.2/openstates/scrape/tests/test_model_basics.py
+-rw-r--r--   0        0        0     4682 2021-11-08 20:47:02.960708 openstates-6.9.2/openstates/scrape/tests/test_scraper.py
+-rw-r--r--   0        0        0     3408 2021-04-27 20:50:33.792727 openstates-6.9.2/openstates/scrape/tests/test_vote_event_scrape.py
+-rw-r--r--   0        0        0     3179 2021-04-27 20:50:33.793227 openstates-6.9.2/openstates/scrape/vote_event.py
+-rw-r--r--   0        0        0     1171 2021-11-08 20:47:02.961460 openstates-6.9.2/openstates/settings.py
+-rw-r--r--   0        0        0      641 2021-08-02 18:12:37.034039 openstates-6.9.2/openstates/test_settings.py
+-rw-r--r--   0        0        0      212 2020-04-22 18:59:48.470369 openstates-6.9.2/openstates/utils/__init__.py
+-rw-r--r--   0        0        0     4913 2021-05-27 15:50:50.118440 openstates-6.9.2/openstates/utils/ansistrm.py
+-rw-r--r--   0        0        0      690 2021-08-02 18:12:37.034545 openstates-6.9.2/openstates/utils/django.py
+-rw-r--r--   0        0        0     2219 2021-05-27 15:56:07.106329 openstates-6.9.2/openstates/utils/generic.py
+-rw-r--r--   0        0        0      212 2021-05-27 15:56:24.523654 openstates-6.9.2/openstates/utils/metadata.py
+-rw-r--r--   0        0        0      272 2021-07-02 18:55:11.811945 openstates-6.9.2/openstates/utils/people/__init__.py
+-rw-r--r--   0        0        0     3067 2021-07-27 17:36:01.616887 openstates-6.9.2/openstates/utils/people/general.py
+-rw-r--r--   0        0        0     4060 2021-07-02 18:54:53.862860 openstates-6.9.2/openstates/utils/people/images.py
+-rw-r--r--   0        0        0    13594 2021-11-08 20:47:02.963062 openstates-6.9.2/openstates/utils/people/lint_people.py
+-rw-r--r--   0        0        0    15026 2021-11-09 21:20:22.997390 openstates-6.9.2/openstates/utils/people/merge.py
+-rw-r--r--   0        0        0     1563 2021-11-08 20:47:02.964601 openstates-6.9.2/openstates/utils/people/retire.py
+-rw-r--r--   0        0        0     9950 2021-11-08 20:47:02.965721 openstates-6.9.2/openstates/utils/people/to_database.py
+-rw-r--r--   0        0        0        0 2021-05-25 18:40:17.132549 openstates-6.9.2/openstates/utils/tests/__init__.py
+-rw-r--r--   0        0        0      497 2021-05-25 18:40:17.133151 openstates-6.9.2/openstates/utils/tests/django_test_settings.py
+-rw-r--r--   0        0        0    12917 2021-11-08 21:09:17.055782 openstates-6.9.2/openstates/utils/tests/test_committees.py
+-rw-r--r--   0        0        0     9605 2021-11-08 20:47:02.967632 openstates-6.9.2/openstates/utils/tests/test_lint.py
+-rw-r--r--   0        0        0    10070 2021-11-08 20:47:02.980914 openstates-6.9.2/openstates/utils/tests/test_merge.py
+-rw-r--r--   0        0        0     1143 2021-07-02 18:51:43.411066 openstates-6.9.2/openstates/utils/tests/test_retire.py
+-rw-r--r--   0        0        0     1809 2021-11-08 20:47:02.969415 openstates-6.9.2/openstates/utils/tests/test_summarize.py
+-rw-r--r--   0        0        0    11722 2021-11-08 21:09:17.056155 openstates-6.9.2/openstates/utils/tests/test_to_database.py
+-rw-r--r--   0        0        0     1159 2021-05-27 15:57:05.871714 openstates-6.9.2/openstates/utils/tests/test_transformers.py
+-rw-r--r--   0        0        0      369 2021-07-14 15:54:14.568081 openstates-6.9.2/openstates/utils/tests/testdata/broken-committees/lower-Broken-11111111-9999-9999-9999-222222222222.yml
+-rw-r--r--   0        0        0      339 2021-07-14 15:54:18.813637 openstates-6.9.2/openstates/utils/tests/testdata/broken-committees/upper-Broken-11111111-9999-9999-9999-3333333333333.yml
+-rw-r--r--   0        0        0      565 2021-07-14 15:52:19.484624 openstates-6.9.2/openstates/utils/tests/testdata/committees/lower-Agriculture-11111111-2222-3333-4444-111111111111.yml
+-rw-r--r--   0        0        0      380 2021-07-14 15:53:33.380376 openstates-6.9.2/openstates/utils/tests/testdata/committees/lower-Education-11111111-2222-3333-4444-222222222222.yml
+-rw-r--r--   0        0        0      312 2021-07-14 15:53:37.721140 openstates-6.9.2/openstates/utils/tests/testdata/committees/lower-Rules-11111111-2222-3333-4444-444444444444.yml
+-rw-r--r--   0        0        0      372 2021-07-14 15:53:40.494001 openstates-6.9.2/openstates/utils/tests/testdata/committees/upper-Education-11111111-2222-3333-4444-3333333333333.yml
+-rw-r--r--   0        0        0        0 2021-07-27 17:45:44.117637 openstates-6.9.2/openstates/utils/tests/testdata/data/EMPTY
+-rw-r--r--   0        0        0     1258 2021-11-08 20:47:02.970843 openstates-6.9.2/openstates/utils/tests/testdata/people/data/pa/legislature/Pam-Snyder--a2e4a1b2-f0fd-4c35-9e0c-bb009778792f.yml
+-rw-r--r--   0        0        0      730 2021-07-14 15:53:06.295239 openstates-6.9.2/openstates/utils/tests/testdata/scraped-committees/0d3e4bee-cbe3-4f9a-a732-1166e1a6c006.json
+-rw-r--r--   0        0        0      894 2021-07-14 15:53:09.045606 openstates-6.9.2/openstates/utils/tests/testdata/scraped-committees/b0aabcb0-ad1c-4e05-af8f-3ec0c2de0fe2.json
+-rw-r--r--   0        0        0      596 2021-05-27 15:50:29.217162 openstates-6.9.2/openstates/utils/transformers.py
+-rw-r--r--   0        0        0     1349 2021-11-29 18:28:45.697545 openstates-6.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2421 2021-11-29 18:29:11.928372 openstates-6.9.2/setup.py
+-rw-r--r--   0        0        0      970 2021-11-29 18:29:11.928722 openstates-6.9.2/PKG-INFO
```

### Comparing `openstates-6.9.1/LICENSE` & `openstates-6.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/cli/committees.py` & `openstates-6.9.2/openstates/cli/committees.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/cli/convert_us.py` & `openstates-6.9.2/openstates/cli/convert_us.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     return "ocd-person/" + str(uuid.uuid5(US_UUID_NAMESPACE, bioguide))
 
 
 def make_org_id(id_: str) -> str:
     return "ocd-organization/" + str(uuid.uuid5(US_UUID_NAMESPACE, id_))
 
 
-def _fix_bad_dashes(phone):
+def _fix_bad_dashes(phone: str) -> str:
     return phone.replace("–", "-")
 
 
 def get_district_offices() -> defaultdict[str, list[Office]]:
     district_offices = defaultdict(list)
     url = "https://theunitedstates.io/congress-legislators/legislators-district-offices.json"
     entries = requests.get(url).json()
```

### Comparing `openstates-6.9.1/openstates/cli/initdb.py` & `openstates-6.9.2/openstates/cli/initdb.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # type: ignore
 # too many django types in this to type for now
 from ..metadata import STATES_BY_ABBR
 from ..utils.django import init_django
+from django.core import management
 from django.db import transaction  # type: ignore
 
 
 def create_division(division_id: str, name: str):
     from ..data.models import Division
 
     return Division.objects.get_or_create(
@@ -84,9 +85,10 @@
     for name, state in STATES_BY_ABBR.items():
         print("loading", name)
         create_full_jurisdiction(state)
 
 
 def main() -> None:
     init_django()
+    management.call_command("migrate")
     with transaction.atomic():
         load_jurisdictions()
```

### Comparing `openstates-6.9.1/openstates/cli/people.py` & `openstates-6.9.2/openstates/cli/people.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/cli/reports.py` & `openstates-6.9.2/openstates/cli/reports.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/cli/tests/test_initdb.py` & `openstates-6.9.2/openstates/cli/tests/test_initdb.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/cli/tests/test_session_report.py` & `openstates-6.9.2/openstates/cli/tests/test_session_report.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/cli/tests/test_settings.py` & `openstates-6.9.2/openstates/cli/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/cli/text_extract.py` & `openstates-6.9.2/openstates/cli/text_extract.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/cli/update.py` & `openstates-6.9.2/openstates/cli/update.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/cli/update_computed.py` & `openstates-6.9.2/openstates/cli/update_computed.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/admin/base.py` & `openstates-6.9.2/openstates/data/admin/base.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/admin/bill.py` & `openstates-6.9.2/openstates/data/admin/bill.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/admin/event.py` & `openstates-6.9.2/openstates/data/admin/event.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/admin/organization.py` & `openstates-6.9.2/openstates/data/admin/organization.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/admin/other.py` & `openstates-6.9.2/openstates/data/admin/other.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/admin/person.py` & `openstates-6.9.2/openstates/data/admin/person.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/admin/reports.py` & `openstates-6.9.2/openstates/data/admin/reports.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/admin/vote.py` & `openstates-6.9.2/openstates/data/admin/vote.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/common.py` & `openstates-6.9.2/openstates/data/common.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0001_initial.py` & `openstates-6.9.2/openstates/data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0002_auto_20200422_0028.py` & `openstates-6.9.2/openstates/data/migrations/0002_auto_20200422_0028.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0005_auto_20200423_1100.py` & `openstates-6.9.2/openstates/data/migrations/0005_auto_20200423_1100.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0006_auto_20200423_1124.py` & `openstates-6.9.2/openstates/data/migrations/0006_auto_20200423_1124.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0007_auto_20200423_1416.py` & `openstates-6.9.2/openstates/data/migrations/0007_auto_20200423_1416.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0009_auto_20200429_0913.py` & `openstates-6.9.2/openstates/data/migrations/0009_auto_20200429_0913.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0010_auto_20200721_1604.py` & `openstates-6.9.2/openstates/data/migrations/0010_auto_20200721_1604.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0011_auto_20200804_1108.py` & `openstates-6.9.2/openstates/data/migrations/0011_auto_20200804_1108.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0015_auto_20200811_1009.py` & `openstates-6.9.2/openstates/data/migrations/0015_auto_20200811_1009.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0016_auto_20200811_1016.py` & `openstates-6.9.2/openstates/data/migrations/0016_auto_20200811_1016.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0018_auto_20200914_1032.py` & `openstates-6.9.2/openstates/data/migrations/0018_auto_20200914_1032.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0022_auto_20200914_1054.py` & `openstates-6.9.2/openstates/data/migrations/0022_auto_20200914_1054.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0025_auto_20200914_1216.py` & `openstates-6.9.2/openstates/data/migrations/0025_auto_20200914_1216.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0026_auto_20200923_1312.py` & `openstates-6.9.2/openstates/data/migrations/0026_auto_20200923_1312.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0028_auto_20201022_1642.py` & `openstates-6.9.2/openstates/data/migrations/0028_auto_20201022_1642.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0030_auto_20210210_1817.py` & `openstates-6.9.2/openstates/data/migrations/0030_auto_20210210_1817.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0031_auto_20210401_1449.py` & `openstates-6.9.2/openstates/data/migrations/0031_auto_20210401_1449.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0033_auto_20210421_1538.py` & `openstates-6.9.2/openstates/data/migrations/0033_auto_20210421_1538.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0035_auto_20210422_1926.py` & `openstates-6.9.2/openstates/data/migrations/0035_auto_20210422_1926.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0036_auto_20210802_1752.py` & `openstates-6.9.2/openstates/data/migrations/0036_auto_20210802_1752.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0037_importobjects_runplan_scrapeobjects_scrapereport_sessiondataqualityreport.py` & `openstates-6.9.2/openstates/data/migrations/0037_importobjects_runplan_scrapeobjects_scrapereport_sessiondataqualityreport.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0038_auto_20210914_1559.py` & `openstates-6.9.2/openstates/data/migrations/0038_auto_20210914_1559.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0039_auto_20210920_1934.py` & `openstates-6.9.2/openstates/data/migrations/0039_auto_20210920_1934.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0040_auto_20210920_2347.py` & `openstates-6.9.2/openstates/data/migrations/0040_auto_20210920_2347.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/migrations/0041_personoffice.py` & `openstates-6.9.2/openstates/data/migrations/0041_personoffice.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/models/__init__.py` & `openstates-6.9.2/openstates/data/models/__init__.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/models/base.py` & `openstates-6.9.2/openstates/data/models/base.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/models/bill.py` & `openstates-6.9.2/openstates/data/models/bill.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/models/division.py` & `openstates-6.9.2/openstates/data/models/division.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/models/event.py` & `openstates-6.9.2/openstates/data/models/event.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/models/jurisdiction.py` & `openstates-6.9.2/openstates/data/models/jurisdiction.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/models/people_orgs.py` & `openstates-6.9.2/openstates/data/models/people_orgs.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/models/reports.py` & `openstates-6.9.2/openstates/data/models/reports.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/models/vote.py` & `openstates-6.9.2/openstates/data/models/vote.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/tests/conftest.py` & `openstates-6.9.2/openstates/data/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/data/tests/test_models.py` & `openstates-6.9.2/openstates/data/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/exceptions.py` & `openstates-6.9.2/openstates/exceptions.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/__init__.py` & `openstates-6.9.2/openstates/fulltext/__init__.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/common.py` & `openstates-6.9.2/openstates/fulltext/common.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/de.py` & `openstates-6.9.2/openstates/fulltext/de.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ak.csv` & `openstates-6.9.2/openstates/fulltext/raw/ak.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/al.csv` & `openstates-6.9.2/openstates/fulltext/raw/al.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ar.csv` & `openstates-6.9.2/openstates/fulltext/raw/ar.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/az.csv` & `openstates-6.9.2/openstates/fulltext/raw/az.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ca.csv` & `openstates-6.9.2/openstates/fulltext/raw/ca.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/co.csv` & `openstates-6.9.2/openstates/fulltext/raw/co.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ct.csv` & `openstates-6.9.2/openstates/fulltext/raw/ct.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/dc.csv` & `openstates-6.9.2/openstates/fulltext/raw/dc.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/de.csv` & `openstates-6.9.2/openstates/fulltext/raw/de.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/fl.csv` & `openstates-6.9.2/openstates/fulltext/raw/fl.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ga.csv` & `openstates-6.9.2/openstates/fulltext/raw/ga.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/hi.csv` & `openstates-6.9.2/openstates/fulltext/raw/hi.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ia.csv` & `openstates-6.9.2/openstates/fulltext/raw/ia.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/id.csv` & `openstates-6.9.2/openstates/fulltext/raw/id.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/il.csv` & `openstates-6.9.2/openstates/fulltext/raw/il.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/in.csv` & `openstates-6.9.2/openstates/fulltext/raw/in.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ks.csv` & `openstates-6.9.2/openstates/fulltext/raw/ks.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ky.csv` & `openstates-6.9.2/openstates/fulltext/raw/ky.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/la.csv` & `openstates-6.9.2/openstates/fulltext/raw/la.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ma.csv` & `openstates-6.9.2/openstates/fulltext/raw/ma.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/md.csv` & `openstates-6.9.2/openstates/fulltext/raw/md.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/me.csv` & `openstates-6.9.2/openstates/fulltext/raw/me.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/mi.csv` & `openstates-6.9.2/openstates/fulltext/raw/mi.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/mn.csv` & `openstates-6.9.2/openstates/fulltext/raw/mn.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/mo.csv` & `openstates-6.9.2/openstates/fulltext/raw/mo.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ms.csv` & `openstates-6.9.2/openstates/fulltext/raw/ms.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/mt.csv` & `openstates-6.9.2/openstates/fulltext/raw/mt.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/nc.csv` & `openstates-6.9.2/openstates/fulltext/raw/nc.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/nd.csv` & `openstates-6.9.2/openstates/fulltext/raw/nd.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ne.csv` & `openstates-6.9.2/openstates/fulltext/raw/ne.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/nh.csv` & `openstates-6.9.2/openstates/fulltext/raw/nh.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/nj.csv` & `openstates-6.9.2/openstates/fulltext/raw/nj.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/nm.csv` & `openstates-6.9.2/openstates/fulltext/raw/nm.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/nv.csv` & `openstates-6.9.2/openstates/fulltext/raw/nv.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ny.csv` & `openstates-6.9.2/openstates/fulltext/raw/ny.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/oh.csv` & `openstates-6.9.2/openstates/fulltext/raw/oh.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ok.csv` & `openstates-6.9.2/openstates/fulltext/raw/ok.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/or.csv` & `openstates-6.9.2/openstates/fulltext/raw/or.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/pa.csv` & `openstates-6.9.2/openstates/fulltext/raw/pa.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/pr.csv` & `openstates-6.9.2/openstates/fulltext/raw/pr.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ri.csv` & `openstates-6.9.2/openstates/fulltext/raw/ri.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/sc.csv` & `openstates-6.9.2/openstates/fulltext/raw/sc.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/sd.csv` & `openstates-6.9.2/openstates/fulltext/raw/sd.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/tn.csv` & `openstates-6.9.2/openstates/fulltext/raw/tn.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/tx.csv` & `openstates-6.9.2/openstates/fulltext/raw/tx.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/ut.csv` & `openstates-6.9.2/openstates/fulltext/raw/ut.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/va.csv` & `openstates-6.9.2/openstates/fulltext/raw/va.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/vt.csv` & `openstates-6.9.2/openstates/fulltext/raw/vt.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/wa.csv` & `openstates-6.9.2/openstates/fulltext/raw/wa.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/wi.csv` & `openstates-6.9.2/openstates/fulltext/raw/wi.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/wv.csv` & `openstates-6.9.2/openstates/fulltext/raw/wv.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/raw/wy.csv` & `openstates-6.9.2/openstates/fulltext/raw/wy.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/fulltext/utils.py` & `openstates-6.9.2/openstates/fulltext/utils.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/importers/base.py` & `openstates-6.9.2/openstates/importers/base.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/importers/bills.py` & `openstates-6.9.2/openstates/importers/bills.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/importers/computed_fields.py` & `openstates-6.9.2/openstates/importers/computed_fields.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/importers/events.py` & `openstates-6.9.2/openstates/importers/events.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/importers/jurisdiction.py` & `openstates-6.9.2/openstates/importers/jurisdiction.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/importers/organizations.py` & `openstates-6.9.2/openstates/importers/organizations.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/importers/tests/test_base_importer.py` & `openstates-6.9.2/openstates/importers/tests/test_base_importer.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/importers/tests/test_bill_importer.py` & `openstates-6.9.2/openstates/importers/tests/test_bill_importer.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/importers/tests/test_computed_fields.py` & `openstates-6.9.2/openstates/importers/tests/test_computed_fields.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/importers/tests/test_event_importer.py` & `openstates-6.9.2/openstates/importers/tests/test_event_importer.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/importers/tests/test_jurisdiction_importer.py` & `openstates-6.9.2/openstates/importers/tests/test_jurisdiction_importer.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/importers/tests/test_vote_event_importer.py` & `openstates-6.9.2/openstates/importers/tests/test_vote_event_importer.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/importers/vote_events.py` & `openstates-6.9.2/openstates/importers/vote_events.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/__init__.py` & `openstates-6.9.2/openstates/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/_creation/create_data.sh` & `openstates-6.9.2/openstates/metadata/_creation/create_data.sh`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/_creation/jurisdictions.csv` & `openstates-6.9.2/openstates/metadata/_creation/jurisdictions.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/_creation/orgs.csv` & `openstates-6.9.2/openstates/metadata/_creation/orgs.csv`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/_creation/settings.yml` & `openstates-6.9.2/openstates/metadata/_creation/settings.yml`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/_creation/write_data.py` & `openstates-6.9.2/openstates/metadata/_creation/write_data.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ak.py` & `openstates-6.9.2/openstates/metadata/data/ak.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/al.py` & `openstates-6.9.2/openstates/metadata/data/al.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ar.py` & `openstates-6.9.2/openstates/metadata/data/ar.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/az.py` & `openstates-6.9.2/openstates/metadata/data/az.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ca.py` & `openstates-6.9.2/openstates/metadata/data/ca.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/co.py` & `openstates-6.9.2/openstates/metadata/data/co.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ct.py` & `openstates-6.9.2/openstates/metadata/data/ct.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/dc.py` & `openstates-6.9.2/openstates/metadata/data/dc.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/de.py` & `openstates-6.9.2/openstates/metadata/data/de.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/fl.py` & `openstates-6.9.2/openstates/metadata/data/fl.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ga.py` & `openstates-6.9.2/openstates/metadata/data/ga.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/hi.py` & `openstates-6.9.2/openstates/metadata/data/hi.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ia.py` & `openstates-6.9.2/openstates/metadata/data/ia.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/id.py` & `openstates-6.9.2/openstates/metadata/data/id.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/il.py` & `openstates-6.9.2/openstates/metadata/data/il.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ind.py` & `openstates-6.9.2/openstates/metadata/data/ind.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ks.py` & `openstates-6.9.2/openstates/metadata/data/ks.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ky.py` & `openstates-6.9.2/openstates/metadata/data/ky.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/la.py` & `openstates-6.9.2/openstates/metadata/data/la.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/legacy_districts.py` & `openstates-6.9.2/openstates/metadata/data/legacy_districts.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ma.py` & `openstates-6.9.2/openstates/metadata/data/ma.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/md.py` & `openstates-6.9.2/openstates/metadata/data/md.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/me.py` & `openstates-6.9.2/openstates/metadata/data/me.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/mi.py` & `openstates-6.9.2/openstates/metadata/data/mi.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/mn.py` & `openstates-6.9.2/openstates/metadata/data/mn.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/mo.py` & `openstates-6.9.2/openstates/metadata/data/mo.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ms.py` & `openstates-6.9.2/openstates/metadata/data/ms.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/mt.py` & `openstates-6.9.2/openstates/metadata/data/mt.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/nc.py` & `openstates-6.9.2/openstates/metadata/data/nc.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/nd.py` & `openstates-6.9.2/openstates/metadata/data/nd.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ne.py` & `openstates-6.9.2/openstates/metadata/data/ne.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/nh.py` & `openstates-6.9.2/openstates/metadata/data/nh.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/nj.py` & `openstates-6.9.2/openstates/metadata/data/nj.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/nm.py` & `openstates-6.9.2/openstates/metadata/data/nm.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/nv.py` & `openstates-6.9.2/openstates/metadata/data/nv.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ny.py` & `openstates-6.9.2/openstates/metadata/data/ny.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/oh.py` & `openstates-6.9.2/openstates/metadata/data/oh.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ok.py` & `openstates-6.9.2/openstates/metadata/data/ok.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ore.py` & `openstates-6.9.2/openstates/metadata/data/ore.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/pa.py` & `openstates-6.9.2/openstates/metadata/data/pa.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/pr.py` & `openstates-6.9.2/openstates/metadata/data/pr.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ri.py` & `openstates-6.9.2/openstates/metadata/data/ri.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/sc.py` & `openstates-6.9.2/openstates/metadata/data/sc.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/sd.py` & `openstates-6.9.2/openstates/metadata/data/sd.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/states.py` & `openstates-6.9.2/openstates/metadata/data/states.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/tn.py` & `openstates-6.9.2/openstates/metadata/data/tn.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/tx.py` & `openstates-6.9.2/openstates/metadata/data/tx.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/us.py` & `openstates-6.9.2/openstates/metadata/data/us.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/ut.py` & `openstates-6.9.2/openstates/metadata/data/ut.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/va.py` & `openstates-6.9.2/openstates/metadata/data/va.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/vt.py` & `openstates-6.9.2/openstates/metadata/data/vt.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/wa.py` & `openstates-6.9.2/openstates/metadata/data/wa.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/wi.py` & `openstates-6.9.2/openstates/metadata/data/wi.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/wv.py` & `openstates-6.9.2/openstates/metadata/data/wv.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/data/wy.py` & `openstates-6.9.2/openstates/metadata/data/wy.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/models.py` & `openstates-6.9.2/openstates/metadata/models.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/tests/test_data.py` & `openstates-6.9.2/openstates/metadata/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/metadata/tests/test_helpers.py` & `openstates-6.9.2/openstates/metadata/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/models/committees.py` & `openstates-6.9.2/openstates/models/committees.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,21 @@
     role: str
     person_id: typing.Optional[str] = None
 
     _validate_person_id = validator("person_id", allow_reuse=True)(validate_ocd_person)
     _validate_name = validator("name", allow_reuse=True)(validate_str_no_newline)
     _validate_role = validator("role", allow_reuse=True)(validate_str_no_newline)
 
+    @validator("name")
+    def not_blank(cls, val: str) -> str:
+        val = val.strip()
+        if not val:
+            raise ValueError("empty name")
+        return val
+
 
 class ScrapeCommittee(BaseModel):
     name: str
     chamber: CommitteeChamber
     classification: CommitteeType = CommitteeType.COMMITTEE
     parent: typing.Optional[str] = None
     sources: typing.List[Link] = []
```

### Comparing `openstates-6.9.1/openstates/models/common.py` & `openstates-6.9.2/openstates/models/common.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/models/people.py` & `openstates-6.9.2/openstates/models/people.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/models/tests/test_models.py` & `openstates-6.9.2/openstates/models/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/base.py` & `openstates-6.9.2/openstates/scrape/base.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/bill.py` & `openstates-6.9.2/openstates/scrape/bill.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/event.py` & `openstates-6.9.2/openstates/scrape/event.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/jurisdiction.py` & `openstates-6.9.2/openstates/scrape/jurisdiction.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/popolo.py` & `openstates-6.9.2/openstates/scrape/popolo.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/schemas/bill.py` & `openstates-6.9.2/openstates/scrape/schemas/bill.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/schemas/common.py` & `openstates-6.9.2/openstates/scrape/schemas/common.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/schemas/event.py` & `openstates-6.9.2/openstates/scrape/schemas/event.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/schemas/jurisdiction.py` & `openstates-6.9.2/openstates/scrape/schemas/jurisdiction.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/schemas/organization.py` & `openstates-6.9.2/openstates/scrape/schemas/organization.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/schemas/vote_event.py` & `openstates-6.9.2/openstates/scrape/schemas/vote_event.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/tests/test_bill_scrape.py` & `openstates-6.9.2/openstates/scrape/tests/test_bill_scrape.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/tests/test_event_scrape.py` & `openstates-6.9.2/openstates/scrape/tests/test_event_scrape.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/tests/test_jurisdiction_scrape.py` & `openstates-6.9.2/openstates/scrape/tests/test_jurisdiction_scrape.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/tests/test_model_basics.py` & `openstates-6.9.2/openstates/scrape/tests/test_model_basics.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/tests/test_scraper.py` & `openstates-6.9.2/openstates/scrape/tests/test_scraper.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/tests/test_vote_event_scrape.py` & `openstates-6.9.2/openstates/scrape/tests/test_vote_event_scrape.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/scrape/vote_event.py` & `openstates-6.9.2/openstates/scrape/vote_event.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/settings.py` & `openstates-6.9.2/openstates/settings.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/test_settings.py` & `openstates-6.9.2/openstates/test_settings.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/ansistrm.py` & `openstates-6.9.2/openstates/utils/ansistrm.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/django.py` & `openstates-6.9.2/openstates/utils/django.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/generic.py` & `openstates-6.9.2/openstates/utils/generic.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/people/general.py` & `openstates-6.9.2/openstates/utils/people/general.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/people/images.py` & `openstates-6.9.2/openstates/utils/people/images.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/people/lint_people.py` & `openstates-6.9.2/openstates/utils/people/lint_people.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/people/merge.py` & `openstates-6.9.2/openstates/utils/people/merge.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/people/retire.py` & `openstates-6.9.2/openstates/utils/people/retire.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/people/to_database.py` & `openstates-6.9.2/openstates/utils/people/to_database.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/tests/test_committees.py` & `openstates-6.9.2/openstates/utils/tests/test_committees.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/tests/test_lint.py` & `openstates-6.9.2/openstates/utils/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/tests/test_merge.py` & `openstates-6.9.2/openstates/utils/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/tests/test_retire.py` & `openstates-6.9.2/openstates/utils/tests/test_retire.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/tests/test_summarize.py` & `openstates-6.9.2/openstates/utils/tests/test_summarize.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/tests/test_to_database.py` & `openstates-6.9.2/openstates/utils/tests/test_to_database.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/tests/test_transformers.py` & `openstates-6.9.2/openstates/utils/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/tests/testdata/committees/lower-Agriculture-11111111-2222-3333-4444-111111111111.yml` & `openstates-6.9.2/openstates/utils/tests/testdata/committees/lower-Agriculture-11111111-2222-3333-4444-111111111111.yml`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/tests/testdata/people/data/pa/legislature/Pam-Snyder--a2e4a1b2-f0fd-4c35-9e0c-bb009778792f.yml` & `openstates-6.9.2/openstates/utils/tests/testdata/people/data/pa/legislature/Pam-Snyder--a2e4a1b2-f0fd-4c35-9e0c-bb009778792f.yml`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/tests/testdata/scraped-committees/0d3e4bee-cbe3-4f9a-a732-1166e1a6c006.json` & `openstates-6.9.2/openstates/utils/tests/testdata/scraped-committees/0d3e4bee-cbe3-4f9a-a732-1166e1a6c006.json`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/tests/testdata/scraped-committees/b0aabcb0-ad1c-4e05-af8f-3ec0c2de0fe2.json` & `openstates-6.9.2/openstates/utils/tests/testdata/scraped-committees/b0aabcb0-ad1c-4e05-af8f-3ec0c2de0fe2.json`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/openstates/utils/transformers.py` & `openstates-6.9.2/openstates/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `openstates-6.9.1/pyproject.toml` & `openstates-6.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openstates"
-version = "6.9.1"
+version = "6.9.2"
 description = "core infrastructure for the openstates project"
 authors = ["James Turk <james@openstates.org>"]
 license = "MIT"
 
 [tool.poetry.scripts]
 os-update = 'openstates.cli.update:main'
 os-initdb = 'openstates.cli.initdb:main'
```

### Comparing `openstates-6.9.1/setup.py` & `openstates-6.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                      'os-text-extract = openstates.cli.text_extract:main',
                      'os-update = openstates.cli.update:main',
                      'os-update-computed = openstates.cli.update_computed:main',
                      'os-us-to-yaml = openstates.cli.convert_us:main']}
 
 setup_kwargs = {
     'name': 'openstates',
-    'version': '6.9.1',
+    'version': '6.9.2',
     'description': 'core infrastructure for the openstates project',
     'long_description': None,
     'author': 'James Turk',
     'author_email': 'james@openstates.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `openstates-6.9.1/PKG-INFO` & `openstates-6.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstates
-Version: 6.9.1
+Version: 6.9.2
 Summary: core infrastructure for the openstates project
 License: MIT
 Author: James Turk
 Author-email: james@openstates.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

