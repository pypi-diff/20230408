# Comparing `tmp/denovonear-0.9.8.tar.gz` & `tmp/denovonear-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/denovonear-0.9.8.tar", last modified: Thu Oct 28 22:28:22 2021, max compression
+gzip compressed data, was "dist/denovonear-0.9.9.tar", last modified: Mon Nov  1 18:32:35 2021, max compression
```

## Comparing `denovonear-0.9.8.tar` & `denovonear-0.9.9.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-10-28 22:28:22.430583 denovonear-0.9.8/
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     1069 2021-10-26 22:35:55.000000 denovonear-0.9.8/LICENSE.txt
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      371 2021-10-26 22:35:55.000000 denovonear-0.9.8/MANIFEST.in
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     6958 2021-10-28 22:28:22.430045 denovonear-0.9.8/PKG-INFO
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     5364 2021-10-26 22:35:55.000000 denovonear-0.9.8/README.md
-drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-10-28 22:28:22.402453 denovonear-0.9.8/data/
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      178 2021-10-26 22:35:55.000000 denovonear-0.9.8/data/example.grch38.dnms.txt
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      319 2021-10-26 22:35:55.000000 denovonear-0.9.8/data/example_de_novos.txt
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      108 2021-10-26 22:35:55.000000 denovonear-0.9.8/data/example_gene_ids.txt
-drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-10-28 22:28:22.416031 denovonear-0.9.8/denovonear/
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)       97 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/__init__.py
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    10865 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/__main__.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     4041 2021-10-27 18:39:13.000000 denovonear-0.9.8/denovonear/cluster_test.py
-drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-10-28 22:28:22.418418 denovonear-0.9.8/denovonear/data/
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     5568 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/data/rates.txt
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     4529 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/ensembl_cache.py
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     5496 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/ensembl_requester.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     1748 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/frameshift_rate.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)   633490 2021-10-28 22:08:38.000000 denovonear-0.9.8/denovonear/gencode.cpp
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    12024 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/gencode.pyx
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2393 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/load_de_novos.py
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     7718 2021-10-27 18:41:31.000000 denovonear-0.9.8/denovonear/load_gene.py
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      875 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/load_mutation_rates.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      497 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/log_transform_rates.py
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2077 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/rate_limiter.py
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2524 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/rate_limiter_retries.py
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     1948 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/simulate.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)   259924 2021-10-28 22:08:38.000000 denovonear-0.9.8/denovonear/site_specific_rates.cpp
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     3414 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/site_specific_rates.pyx
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)   664734 2021-10-28 22:08:38.000000 denovonear-0.9.8/denovonear/transcript.cpp
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     3161 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/transcript.pxd
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    14961 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/transcript.pyx
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)   252239 2021-10-28 22:08:38.000000 denovonear-0.9.8/denovonear/weights.cpp
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     1709 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/weights.pxd
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     5156 2021-10-26 22:35:55.000000 denovonear-0.9.8/denovonear/weights.pyx
-drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-10-28 22:28:22.418114 denovonear-0.9.8/denovonear.egg-info/
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     6958 2021-10-28 22:28:22.000000 denovonear-0.9.8/denovonear.egg-info/PKG-INFO
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     1662 2021-10-28 22:28:22.000000 denovonear-0.9.8/denovonear.egg-info/SOURCES.txt
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        1 2021-10-28 22:28:22.000000 denovonear-0.9.8/denovonear.egg-info/dependency_links.txt
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)       57 2021-10-28 22:28:22.000000 denovonear-0.9.8/denovonear.egg-info/entry_points.txt
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)       56 2021-10-28 22:28:22.000000 denovonear-0.9.8/denovonear.egg-info/requires.txt
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)       11 2021-10-28 22:28:22.000000 denovonear-0.9.8/denovonear.egg-info/top_level.txt
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)       70 2021-10-26 22:35:55.000000 denovonear-0.9.8/pyproject.toml
-drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-10-28 22:28:22.418729 denovonear-0.9.8/scripts/
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     6157 2021-10-26 22:35:55.000000 denovonear-0.9.8/scripts/run_batch.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)       38 2021-10-28 22:28:22.430765 denovonear-0.9.8/setup.cfg
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2682 2021-10-28 22:28:14.000000 denovonear-0.9.8/setup.py
-drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-10-28 22:28:22.423393 denovonear-0.9.8/src/
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     4220 2021-10-26 22:35:55.000000 denovonear-0.9.8/src/gencode.cpp
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      830 2021-10-26 22:35:55.000000 denovonear-0.9.8/src/gencode.h
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     3472 2021-10-28 01:11:19.000000 denovonear-0.9.8/src/gtf.cpp
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      799 2021-10-26 22:35:55.000000 denovonear-0.9.8/src/gtf.h
-drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-10-28 22:28:22.424108 denovonear-0.9.8/src/gzstream/
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     5093 2021-10-26 22:38:14.000000 denovonear-0.9.8/src/gzstream/gzstream.C
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     4603 2021-10-26 22:38:14.000000 denovonear-0.9.8/src/gzstream/gzstream.h
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     6764 2021-10-26 22:35:55.000000 denovonear-0.9.8/src/simulate.cpp
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      737 2021-10-26 22:35:55.000000 denovonear-0.9.8/src/simulate.h
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     5701 2021-10-28 22:28:14.000000 denovonear-0.9.8/src/site_rates.cpp
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2094 2021-10-26 22:35:55.000000 denovonear-0.9.8/src/site_rates.h
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    26675 2021-10-26 22:35:55.000000 denovonear-0.9.8/src/tx.cpp
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     3216 2021-10-26 22:35:55.000000 denovonear-0.9.8/src/tx.h
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2635 2021-10-26 22:35:55.000000 denovonear-0.9.8/src/weighted_choice.cpp
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      879 2021-10-26 22:35:55.000000 denovonear-0.9.8/src/weighted_choice.h
-drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-10-28 22:28:22.429335 denovonear-0.9.8/tests/
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-10-26 22:35:55.000000 denovonear-0.9.8/tests/__init__.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2443 2021-10-26 22:35:55.000000 denovonear-0.9.8/tests/test_cluster_test.py
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     6787 2021-10-26 22:35:55.000000 denovonear-0.9.8/tests/test_ensembl_cache.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     8400 2021-10-27 18:25:32.000000 denovonear-0.9.8/tests/test_ensembl_requester.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2306 2021-10-26 22:35:55.000000 denovonear-0.9.8/tests/test_frameshift_rate.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    25012 2021-10-26 22:35:55.000000 denovonear-0.9.8/tests/test_gencode.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2945 2021-10-26 22:35:55.000000 denovonear-0.9.8/tests/test_geometric_mean.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    11664 2021-10-26 22:35:55.000000 denovonear-0.9.8/tests/test_load_gene.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     1575 2021-10-26 22:35:55.000000 denovonear-0.9.8/tests/test_log_transform.py
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    11820 2021-10-26 22:35:55.000000 denovonear-0.9.8/tests/test_sequence_methods.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     3620 2021-10-26 22:35:55.000000 denovonear-0.9.8/tests/test_simulate_p_value.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     3031 2021-10-26 22:35:55.000000 denovonear-0.9.8/tests/test_simulations.py
--rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    19674 2021-10-26 22:35:55.000000 denovonear-0.9.8/tests/test_site_rates.py
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    16512 2021-10-26 22:35:55.000000 denovonear-0.9.8/tests/test_transcript.py
--rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     6332 2021-10-26 22:35:55.000000 denovonear-0.9.8/tests/test_weighted_choice.py
+drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-11-01 18:32:35.101909 denovonear-0.9.9/
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     1069 2021-10-26 22:35:55.000000 denovonear-0.9.9/LICENSE.txt
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      371 2021-10-26 22:35:55.000000 denovonear-0.9.9/MANIFEST.in
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     6958 2021-11-01 18:32:35.101424 denovonear-0.9.9/PKG-INFO
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     5364 2021-10-26 22:35:55.000000 denovonear-0.9.9/README.md
+drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-11-01 18:32:35.061813 denovonear-0.9.9/data/
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      178 2021-10-26 22:35:55.000000 denovonear-0.9.9/data/example.grch38.dnms.txt
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      319 2021-10-26 22:35:55.000000 denovonear-0.9.9/data/example_de_novos.txt
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      108 2021-10-26 22:35:55.000000 denovonear-0.9.9/data/example_gene_ids.txt
+drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-11-01 18:32:35.081781 denovonear-0.9.9/denovonear/
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)       97 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/__init__.py
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    10865 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/__main__.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     4041 2021-10-27 18:39:13.000000 denovonear-0.9.9/denovonear/cluster_test.py
+drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-11-01 18:32:35.084148 denovonear-0.9.9/denovonear/data/
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     5568 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/data/rates.txt
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     4529 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/ensembl_cache.py
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     5496 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/ensembl_requester.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     1748 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/frameshift_rate.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)   638262 2021-11-01 18:32:34.000000 denovonear-0.9.9/denovonear/gencode.cpp
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    12278 2021-11-01 18:32:25.000000 denovonear-0.9.9/denovonear/gencode.pyx
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2393 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/load_de_novos.py
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     7718 2021-10-27 18:41:31.000000 denovonear-0.9.9/denovonear/load_gene.py
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      875 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/load_mutation_rates.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      497 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/log_transform_rates.py
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2077 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/rate_limiter.py
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2524 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/rate_limiter_retries.py
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     1948 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/simulate.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)   259924 2021-10-28 22:08:38.000000 denovonear-0.9.9/denovonear/site_specific_rates.cpp
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     3414 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/site_specific_rates.pyx
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)   664734 2021-10-28 22:08:38.000000 denovonear-0.9.9/denovonear/transcript.cpp
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     3161 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/transcript.pxd
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    14961 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/transcript.pyx
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)   252239 2021-10-28 22:08:38.000000 denovonear-0.9.9/denovonear/weights.cpp
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     1709 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/weights.pxd
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     5156 2021-10-26 22:35:55.000000 denovonear-0.9.9/denovonear/weights.pyx
+drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-11-01 18:32:35.083808 denovonear-0.9.9/denovonear.egg-info/
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     6958 2021-11-01 18:32:34.000000 denovonear-0.9.9/denovonear.egg-info/PKG-INFO
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     1662 2021-11-01 18:32:34.000000 denovonear-0.9.9/denovonear.egg-info/SOURCES.txt
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        1 2021-11-01 18:32:34.000000 denovonear-0.9.9/denovonear.egg-info/dependency_links.txt
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)       57 2021-11-01 18:32:34.000000 denovonear-0.9.9/denovonear.egg-info/entry_points.txt
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)       56 2021-11-01 18:32:34.000000 denovonear-0.9.9/denovonear.egg-info/requires.txt
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)       11 2021-11-01 18:32:34.000000 denovonear-0.9.9/denovonear.egg-info/top_level.txt
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)       70 2021-10-26 22:35:55.000000 denovonear-0.9.9/pyproject.toml
+drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-11-01 18:32:35.084713 denovonear-0.9.9/scripts/
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     6157 2021-10-26 22:35:55.000000 denovonear-0.9.9/scripts/run_batch.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)       38 2021-11-01 18:32:35.102018 denovonear-0.9.9/setup.cfg
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2682 2021-11-01 18:32:25.000000 denovonear-0.9.9/setup.py
+drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-11-01 18:32:35.090535 denovonear-0.9.9/src/
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     4220 2021-10-26 22:35:55.000000 denovonear-0.9.9/src/gencode.cpp
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      830 2021-10-26 22:35:55.000000 denovonear-0.9.9/src/gencode.h
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     3472 2021-10-28 01:11:19.000000 denovonear-0.9.9/src/gtf.cpp
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      799 2021-10-26 22:35:55.000000 denovonear-0.9.9/src/gtf.h
+drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-11-01 18:32:35.091989 denovonear-0.9.9/src/gzstream/
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     5093 2021-10-26 22:38:14.000000 denovonear-0.9.9/src/gzstream/gzstream.C
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     4603 2021-10-26 22:38:14.000000 denovonear-0.9.9/src/gzstream/gzstream.h
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     6764 2021-10-26 22:35:55.000000 denovonear-0.9.9/src/simulate.cpp
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      737 2021-10-26 22:35:55.000000 denovonear-0.9.9/src/simulate.h
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     5701 2021-10-28 22:28:14.000000 denovonear-0.9.9/src/site_rates.cpp
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2094 2021-10-26 22:35:55.000000 denovonear-0.9.9/src/site_rates.h
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    26675 2021-10-26 22:35:55.000000 denovonear-0.9.9/src/tx.cpp
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     3216 2021-10-26 22:35:55.000000 denovonear-0.9.9/src/tx.h
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2635 2021-10-26 22:35:55.000000 denovonear-0.9.9/src/weighted_choice.cpp
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)      879 2021-10-26 22:35:55.000000 denovonear-0.9.9/src/weighted_choice.h
+drwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-11-01 18:32:35.100450 denovonear-0.9.9/tests/
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)        0 2021-10-26 22:35:55.000000 denovonear-0.9.9/tests/__init__.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2443 2021-10-26 22:35:55.000000 denovonear-0.9.9/tests/test_cluster_test.py
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     6787 2021-10-26 22:35:55.000000 denovonear-0.9.9/tests/test_ensembl_cache.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     8400 2021-10-27 18:25:32.000000 denovonear-0.9.9/tests/test_ensembl_requester.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2306 2021-10-26 22:35:55.000000 denovonear-0.9.9/tests/test_frameshift_rate.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    25012 2021-10-26 22:35:55.000000 denovonear-0.9.9/tests/test_gencode.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     2945 2021-10-26 22:35:55.000000 denovonear-0.9.9/tests/test_geometric_mean.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    11664 2021-10-26 22:35:55.000000 denovonear-0.9.9/tests/test_load_gene.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     1575 2021-10-26 22:35:55.000000 denovonear-0.9.9/tests/test_log_transform.py
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    11820 2021-10-26 22:35:55.000000 denovonear-0.9.9/tests/test_sequence_methods.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     3620 2021-10-26 22:35:55.000000 denovonear-0.9.9/tests/test_simulate_p_value.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     3031 2021-10-26 22:35:55.000000 denovonear-0.9.9/tests/test_simulations.py
+-rw-r--r--   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    19674 2021-10-26 22:35:55.000000 denovonear-0.9.9/tests/test_site_rates.py
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)    16512 2021-10-26 22:35:55.000000 denovonear-0.9.9/tests/test_transcript.py
+-rwxr-xr-x   0 jmcrae   (953725719) ILLUMINA\Domain Users (897801646)     6332 2021-10-26 22:35:55.000000 denovonear-0.9.9/tests/test_weighted_choice.py
```

### Comparing `denovonear-0.9.8/LICENSE.txt` & `denovonear-0.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/PKG-INFO` & `denovonear-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denovonear
-Version: 0.9.8
+Version: 0.9.9
 Summary: Package to examine de novo clustering
 Home-page: https://github.com/jeremymcrae/denovonear
 Author: Jeremy McRae
 Author-email: jeremy.mcrae@gmail.com
 License: MIT
 Description: ![travis](https://travis-ci.org/jeremymcrae/denovonear.svg?branch=master)
```

### Comparing `denovonear-0.9.8/README.md` & `denovonear-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/__main__.py` & `denovonear-0.9.9/denovonear/__main__.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/cluster_test.py` & `denovonear-0.9.9/denovonear/cluster_test.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/data/rates.txt` & `denovonear-0.9.9/denovonear/data/rates.txt`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/ensembl_cache.py` & `denovonear-0.9.9/denovonear/ensembl_cache.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/ensembl_requester.py` & `denovonear-0.9.9/denovonear/ensembl_requester.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/frameshift_rate.py` & `denovonear-0.9.9/denovonear/frameshift_rate.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/gencode.cpp` & `denovonear-0.9.9/denovonear/gencode.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.24 */
+/* Generated by Cython 0.29.21 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "src/gencode.h",
             "src/gtf.h",
@@ -34,25 +34,23 @@
             "src/gzstream/gzstream.C"
         ]
     },
     "module_name": "denovonear.gencode"
 }
 END: Cython Metadata */
 
-#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
-#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_24"
-#define CYTHON_HEX_VERSION 0x001D18F0
+#define CYTHON_ABI "0_29_21"
+#define CYTHON_HEX_VERSION 0x001D15F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -476,33 +474,25 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
   #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
                                               0 : _PyUnicode_Ready((PyObject *)(op)))
-  #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
-  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
   #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
   #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
@@ -955,85 +945,85 @@
   std::vector<bool>  _principal;
   PyObject *_chrom;
   int _start;
   int _end;
 };
 
 
-/* "denovonear/gencode.pyx":238
+/* "denovonear/gencode.pyx":243
  *         return any(tx.in_coding_region(pos) for tx in self._transcripts)
  * 
  * cdef class Gencode:             # <<<<<<<<<<<<<<
  *     cdef dict genes
  *     cdef list coords
  */
 struct __pyx_obj_10denovonear_7gencode_Gencode {
   PyObject_HEAD
   PyObject *genes;
   PyObject *coords;
 };
 
 
-/* "denovonear/gencode.pyx":233
+/* "denovonear/gencode.pyx":238
  *         return self._to_Transcript(self._max_by_cds(principal))
  * 
  *     def in_any_tx_cds(self, pos):             # <<<<<<<<<<<<<<
  *         ''' find if a pos is in coding region of any transcript of a gene
  *         '''
  */
 struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds {
   PyObject_HEAD
   PyObject *__pyx_v_pos;
   struct __pyx_obj_10denovonear_7gencode_Gene *__pyx_v_self;
 };
 
 
-/* "denovonear/gencode.pyx":236
+/* "denovonear/gencode.pyx":241
  *         ''' find if a pos is in coding region of any transcript of a gene
  *         '''
  *         return any(tx.in_coding_region(pos) for tx in self._transcripts)             # <<<<<<<<<<<<<<
  * 
  * cdef class Gencode:
  */
 struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_1_genexpr {
   PyObject_HEAD
   struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds *__pyx_outer_scope;
   Tx __pyx_v_tx;
 };
 
 
-/* "denovonear/gencode.pyx":268
+/* "denovonear/gencode.pyx":273
  *         self._sort()
  * 
  *     def _sort(self):             # <<<<<<<<<<<<<<
  *         self.coords = sorted(((x.chrom, x.start, x.end), symbol) for symbol, x in self.genes.items())
  * 
  */
 struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_2__sort {
   PyObject_HEAD
   struct __pyx_obj_10denovonear_7gencode_Gencode *__pyx_v_self;
 };
 
 
-/* "denovonear/gencode.pyx":269
+/* "denovonear/gencode.pyx":274
  * 
  *     def _sort(self):
  *         self.coords = sorted(((x.chrom, x.start, x.end), symbol) for symbol, x in self.genes.items())             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
 struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_3_genexpr {
   PyObject_HEAD
   struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_2__sort *__pyx_outer_scope;
   PyObject *__pyx_v_symbol;
   PyObject *__pyx_v_x;
 };
 
 
-/* "denovonear/gencode.pyx":277
+/* "denovonear/gencode.pyx":282
  *     def __getitem__(self, symbol):
  *         return self.genes[symbol]
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         for x in self.genes:
  *             yield x
  */
 struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_4___iter__ {
@@ -1043,30 +1033,30 @@
   PyObject *__pyx_t_0;
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   int __pyx_t_3;
 };
 
 
-/* "denovonear/gencode.pyx":330
+/* "denovonear/gencode.pyx":335
  *             return right
  * 
  *     def in_region(self, chrom, start, end):             # <<<<<<<<<<<<<<
  *         ''' find genes within a genomic region
  * 
  */
 struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_5_in_region {
   PyObject_HEAD
   PyObject *__pyx_v_left;
   PyObject *__pyx_v_right;
   struct __pyx_obj_10denovonear_7gencode_Gencode *__pyx_v_self;
 };
 
 
-/* "denovonear/gencode.pyx":345
+/* "denovonear/gencode.pyx":350
  *         right = bisect.bisect_left(self.coords, ((chrom, end, end), 'AAAA'))
  * 
  *         genes = (self.genes[self.coords[i][1]] for i in range(left, right))             # <<<<<<<<<<<<<<
  *         return [x for x in genes if x.chrom == chrom]
  * 
  */
 struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_6_genexpr {
@@ -1379,14 +1369,23 @@
     (likely(PyDict_CheckExact(obj)) ?\
      __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
 #else
 #define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
 #define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
 #endif
 
+/* IncludeStringH.proto */
+#include <string.h>
+
+/* BytesEquals.proto */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
+
+/* UnicodeEquals.proto */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
+
 /* PyObjectFormatSimple.proto */
 #if CYTHON_COMPILING_IN_PYPY
     #define __Pyx_PyObject_FormatSimple(s, f) (\
         likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
         PyObject_Format(s, f))
 #elif PY_MAJOR_VERSION < 3
     #define __Pyx_PyObject_FormatSimple(s, f) (\
@@ -1401,17 +1400,14 @@
         PyObject_Format(s, f))
 #else
     #define __Pyx_PyObject_FormatSimple(s, f) (\
         likely(PyUnicode_CheckExact(s)) ? (Py_INCREF(s), s) :\
         PyObject_Format(s, f))
 #endif
 
-/* IncludeStringH.proto */
-#include <string.h>
-
 /* JoinPyUnicode.proto */
 static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
                                       Py_UCS4 max_char);
 
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
@@ -1447,20 +1443,14 @@
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
-/* BytesEquals.proto */
-static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
-
-/* UnicodeEquals.proto */
-static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
-
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -1555,19 +1545,14 @@
 
 /* dict_iter.proto */
 static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* dict, int is_dict, PyObject* method_name,
                                                    Py_ssize_t* p_orig_length, int* p_is_dict);
 static CYTHON_INLINE int __Pyx_dict_iter_next(PyObject* dict_or_iter, Py_ssize_t orig_length, Py_ssize_t* ppos,
                                               PyObject** pkey, PyObject** pvalue, PyObject** pitem, int is_dict);
 
-/* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
-#define __Pyx_HAS_GCC_DIAGNOSTIC
-#endif
-
 /* BuildPyUnicode.proto */
 static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
                                                 int prepend_sign, char padding_char);
 
 /* CIntToPyUnicode.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_Py_ssize_t(Py_ssize_t value, Py_ssize_t width, char padding_char, char format_char);
 
@@ -1663,15 +1648,21 @@
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
 /* None.proto */
 #include <new>
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
+
 static PyObject* __pyx_convert__to_py_struct__gencode_3a__3a_GTFLine(struct gencode::GTFLine s);
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value);
+
 /* CppExceptionConversion.proto */
 #ifndef __Pyx_CppExn2PyErr
 #include <new>
 #include <typeinfo>
 #include <stdexcept>
 #include <ios>
 static void __Pyx_CppExn2PyErr() {
@@ -1707,28 +1698,22 @@
   {
     PyErr_SetString(PyExc_RuntimeError, "Unknown exception");
   }
 }
 #endif
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
@@ -1790,15 +1775,14 @@
     PyObject *gi_weakreflist;
     PyObject *classobj;
     PyObject *yieldfrom;
     PyObject *gi_name;
     PyObject *gi_qualname;
     PyObject *gi_modulename;
     PyObject *gi_code;
-    PyObject *gi_frame;
     int resume_label;
     char is_running;
 } __pyx_CoroutineObject;
 static __pyx_CoroutineObject *__Pyx__Coroutine_New(
     PyTypeObject *type, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
     PyObject *name, PyObject *qualname, PyObject *module_name);
 static __pyx_CoroutineObject *__Pyx__Coroutine_NewInit(
@@ -1900,17 +1884,17 @@
 
 /* Implementation of 'denovonear.gencode' */
 static PyObject *__pyx_builtin_chr;
 static PyObject *__pyx_builtin_IndexError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_ValueError;
-static const char __pyx_k_[] = "\", ";
-static const char __pyx_k__2[] = ":";
-static const char __pyx_k__3[] = "-";
+static const char __pyx_k_[] = "-";
+static const char __pyx_k__2[] = "\", ";
+static const char __pyx_k__3[] = ":";
 static const char __pyx_k__4[] = ")";
 static const char __pyx_k__6[] = "";
 static const char __pyx_k_chr[] = "chr";
 static const char __pyx_k_end[] = "end";
 static const char __pyx_k_pos[] = "pos";
 static const char __pyx_k_seq[] = "seq";
 static const char __pyx_k_AAAA[] = "AAAA";
@@ -1975,14 +1959,15 @@
 static const char __pyx_k_Gencode___iter[] = "Gencode.__iter__";
 static const char __pyx_k_Gencode_n_genes[] = "Gencode(n_genes=";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_transcript_type[] = "transcript_type";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_denovonear_gencode[] = "denovonear.gencode";
 static const char __pyx_k_get_genomic_offset[] = "get_genomic_offset";
+static const char __pyx_k_reverse_complement[] = "reverse_complement";
 static const char __pyx_k_sort_locals_genexpr[] = "_sort.<locals>.genexpr";
 static const char __pyx_k_get_genomic_sequence[] = "get_genomic_sequence";
 static const char __pyx_k_opening_genome_fasta[] = "opening genome fasta: ";
 static const char __pyx_k_denovonear_transcript[] = "denovonear.transcript";
 static const char __pyx_k_can_t_find_any_genes_on[] = "can't find any genes on ";
 static const char __pyx_k_in_region_locals_genexpr[] = "in_region.<locals>.genexpr";
 static const char __pyx_k_no_transcripts_in_gene_yet[] = "no transcripts in gene yet";
@@ -2056,14 +2041,15 @@
 static PyObject *__pyx_n_s_pos;
 static PyObject *__pyx_n_s_pyfaidx;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
+static PyObject *__pyx_n_s_reverse_complement;
 static PyObject *__pyx_n_s_send;
 static PyObject *__pyx_n_s_seq;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_sort;
 static PyObject *__pyx_n_s_sort_locals_genexpr;
 static PyObject *__pyx_n_s_start;
@@ -3098,14 +3084,15 @@
   std::string __pyx_t_6;
   int __pyx_t_7;
   long __pyx_t_8;
   Py_ssize_t __pyx_t_9;
   PyObject *(*__pyx_t_10)(PyObject *);
   std::vector<int>  __pyx_t_11;
   Tx __pyx_t_12;
+  PyObject *__pyx_t_13 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_transcript", 0);
 
   /* "denovonear/gencode.pyx":99
  *         time wasted, so long as we don't do this millions of times.
@@ -3621,15 +3608,15 @@
   __pyx_v_seq = __pyx_t_6;
 
   /* "denovonear/gencode.pyx":121
  * 
  *         cdef string seq = _tx.get_genomic_sequence().encode('utf8')
  *         cdef int offset = _tx.get_genomic_offset()             # <<<<<<<<<<<<<<
  *         if len(seq) > 0:
- *             tx.add_genomic_sequence(seq, offset)
+ *             if chr(strand) == '-':
  */
   __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v__tx, __pyx_n_s_get_genomic_offset); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_1)) {
@@ -3648,57 +3635,160 @@
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_offset = __pyx_t_7;
 
   /* "denovonear/gencode.pyx":122
  *         cdef string seq = _tx.get_genomic_sequence().encode('utf8')
  *         cdef int offset = _tx.get_genomic_offset()
  *         if len(seq) > 0:             # <<<<<<<<<<<<<<
- *             tx.add_genomic_sequence(seq, offset)
- *         self.add_tx(tx, False)
+ *             if chr(strand) == '-':
+ *                 _tx.reverse_complement(seq)
  */
   __pyx_t_5 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_seq); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_9 = PyObject_Length(__pyx_t_5); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 122, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_2 = ((__pyx_t_9 > 0) != 0);
   if (__pyx_t_2) {
 
     /* "denovonear/gencode.pyx":123
  *         cdef int offset = _tx.get_genomic_offset()
  *         if len(seq) > 0:
+ *             if chr(strand) == '-':             # <<<<<<<<<<<<<<
+ *                 _tx.reverse_complement(seq)
+ *                 seq = _tx.reverse_complement(seq).encode('utf8')
+ */
+    __pyx_t_5 = __Pyx_PyInt_From_char(__pyx_v_strand); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_chr, __pyx_t_5); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_4, __pyx_kp_u_, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (__pyx_t_2) {
+
+      /* "denovonear/gencode.pyx":124
+ *         if len(seq) > 0:
+ *             if chr(strand) == '-':
+ *                 _tx.reverse_complement(seq)             # <<<<<<<<<<<<<<
+ *                 seq = _tx.reverse_complement(seq).encode('utf8')
+ *             tx.add_genomic_sequence(seq, offset)
+ */
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v__tx, __pyx_n_s_reverse_complement); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 124, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_1 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_seq); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_3 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+        __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
+        if (likely(__pyx_t_3)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+          __Pyx_INCREF(__pyx_t_3);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_5, function);
+        }
+      }
+      __pyx_t_4 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_3, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_1);
+      __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 124, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+      /* "denovonear/gencode.pyx":125
+ *             if chr(strand) == '-':
+ *                 _tx.reverse_complement(seq)
+ *                 seq = _tx.reverse_complement(seq).encode('utf8')             # <<<<<<<<<<<<<<
+ *             tx.add_genomic_sequence(seq, offset)
+ *         self.add_tx(tx, False)
+ */
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v__tx, __pyx_n_s_reverse_complement); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_3 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_seq); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 125, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __pyx_t_13 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+        __pyx_t_13 = PyMethod_GET_SELF(__pyx_t_1);
+        if (likely(__pyx_t_13)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+          __Pyx_INCREF(__pyx_t_13);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_1, function);
+        }
+      }
+      __pyx_t_5 = (__pyx_t_13) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_13, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_3);
+      __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 125, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_5, __pyx_n_s_encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_5 = NULL;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+        __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+        if (likely(__pyx_t_5)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+          __Pyx_INCREF(__pyx_t_5);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_1, function);
+        }
+      }
+      __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_n_u_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_n_u_utf8);
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_4); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 125, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_v_seq = __pyx_t_6;
+
+      /* "denovonear/gencode.pyx":123
+ *         cdef int offset = _tx.get_genomic_offset()
+ *         if len(seq) > 0:
+ *             if chr(strand) == '-':             # <<<<<<<<<<<<<<
+ *                 _tx.reverse_complement(seq)
+ *                 seq = _tx.reverse_complement(seq).encode('utf8')
+ */
+    }
+
+    /* "denovonear/gencode.pyx":126
+ *                 _tx.reverse_complement(seq)
+ *                 seq = _tx.reverse_complement(seq).encode('utf8')
  *             tx.add_genomic_sequence(seq, offset)             # <<<<<<<<<<<<<<
  *         self.add_tx(tx, False)
  * 
  */
     try {
       __pyx_v_tx.add_genomic_sequence(__pyx_v_seq, __pyx_v_offset);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 123, __pyx_L1_error)
+      __PYX_ERR(0, 126, __pyx_L1_error)
     }
 
     /* "denovonear/gencode.pyx":122
  *         cdef string seq = _tx.get_genomic_sequence().encode('utf8')
  *         cdef int offset = _tx.get_genomic_offset()
  *         if len(seq) > 0:             # <<<<<<<<<<<<<<
- *             tx.add_genomic_sequence(seq, offset)
- *         self.add_tx(tx, False)
+ *             if chr(strand) == '-':
+ *                 _tx.reverse_complement(seq)
  */
   }
 
-  /* "denovonear/gencode.pyx":124
- *         if len(seq) > 0:
+  /* "denovonear/gencode.pyx":127
+ *                 seq = _tx.reverse_complement(seq).encode('utf8')
  *             tx.add_genomic_sequence(seq, offset)
  *         self.add_tx(tx, False)             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
-  __pyx_t_5 = ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_self->__pyx_vtab)->add_tx(__pyx_v_self, __pyx_v_tx, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 124, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_4 = ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_self->__pyx_vtab)->add_tx(__pyx_v_self, __pyx_v_tx, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "denovonear/gencode.pyx":92
  *         self.end = max(self.end, tx.get_end())
  * 
  *     def add_transcript(self, _tx):             # <<<<<<<<<<<<<<
  *         ''' add a Transcript to the gene object
  * 
@@ -3708,24 +3798,25 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_13);
   __Pyx_AddTraceback("denovonear.gencode.Gene.add_transcript", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_x);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":126
+/* "denovonear/gencode.pyx":129
  *         self.add_tx(tx, False)
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         chrom = self.chrom
  *         return f'Gene("{self.symbol}", {chrom}:{self.start}-{self.end})'
  */
 
@@ -3752,103 +3843,103 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "denovonear/gencode.pyx":127
+  /* "denovonear/gencode.pyx":130
  * 
  *     def __repr__(self):
  *         chrom = self.chrom             # <<<<<<<<<<<<<<
  *         return f'Gene("{self.symbol}", {chrom}:{self.start}-{self.end})'
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_chrom); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_chrom); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_chrom = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":128
+  /* "denovonear/gencode.pyx":131
  *     def __repr__(self):
  *         chrom = self.chrom
  *         return f'Gene("{self.symbol}", {chrom}:{self.start}-{self.end})'             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_3 = 127;
   __Pyx_INCREF(__pyx_kp_u_Gene);
   __pyx_t_2 += 6;
   __Pyx_GIVEREF(__pyx_kp_u_Gene);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Gene);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_symbol); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_symbol); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_5);
   __pyx_t_5 = 0;
-  __Pyx_INCREF(__pyx_kp_u_);
+  __Pyx_INCREF(__pyx_kp_u__2);
   __pyx_t_2 += 3;
-  __Pyx_GIVEREF(__pyx_kp_u_);
-  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_);
-  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_chrom, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_kp_u__2);
+  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__2);
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_v_chrom, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_5);
   __pyx_t_5 = 0;
-  __Pyx_INCREF(__pyx_kp_u__2);
+  __Pyx_INCREF(__pyx_kp_u__3);
   __pyx_t_2 += 1;
-  __Pyx_GIVEREF(__pyx_kp_u__2);
-  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u__2);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_start); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_kp_u__3);
+  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u__3);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_start); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_t_4);
   __pyx_t_4 = 0;
-  __Pyx_INCREF(__pyx_kp_u__3);
+  __Pyx_INCREF(__pyx_kp_u_);
   __pyx_t_2 += 1;
-  __Pyx_GIVEREF(__pyx_kp_u__3);
-  PyTuple_SET_ITEM(__pyx_t_1, 6, __pyx_kp_u__3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __Pyx_GIVEREF(__pyx_kp_u_);
+  PyTuple_SET_ITEM(__pyx_t_1, 6, __pyx_kp_u_);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 7, __pyx_t_5);
   __pyx_t_5 = 0;
   __Pyx_INCREF(__pyx_kp_u__4);
   __pyx_t_2 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__4);
   PyTuple_SET_ITEM(__pyx_t_1, 8, __pyx_kp_u__4);
-  __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 9, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 9, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":126
+  /* "denovonear/gencode.pyx":129
  *         self.add_tx(tx, False)
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         chrom = self.chrom
  *         return f'Gene("{self.symbol}", {chrom}:{self.start}-{self.end})'
  */
 
@@ -3862,15 +3953,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_chrom);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":131
+/* "denovonear/gencode.pyx":134
  * 
  *     @property
  *     def symbol(self):             # <<<<<<<<<<<<<<
  *         return self._symbol.decode('utf8')
  * 
  */
 
@@ -3892,29 +3983,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "denovonear/gencode.pyx":132
+  /* "denovonear/gencode.pyx":135
  *     @property
  *     def symbol(self):
  *         return self._symbol.decode('utf8')             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_self->_symbol, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_self->_symbol, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":131
+  /* "denovonear/gencode.pyx":134
  * 
  *     @property
  *     def symbol(self):             # <<<<<<<<<<<<<<
  *         return self._symbol.decode('utf8')
  * 
  */
 
@@ -3925,15 +4016,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":135
+/* "denovonear/gencode.pyx":138
  * 
  *     @property
  *     def chrom(self):             # <<<<<<<<<<<<<<
  *         return self._chrom
  *     @chrom.setter
  */
 
@@ -3951,42 +4042,42 @@
 }
 
 static PyObject *__pyx_pf_10denovonear_7gencode_4Gene_5chrom___get__(struct __pyx_obj_10denovonear_7gencode_Gene *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "denovonear/gencode.pyx":136
+  /* "denovonear/gencode.pyx":139
  *     @property
  *     def chrom(self):
  *         return self._chrom             # <<<<<<<<<<<<<<
  *     @chrom.setter
  *     def chrom(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_chrom);
   __pyx_r = __pyx_v_self->_chrom;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":135
+  /* "denovonear/gencode.pyx":138
  * 
  *     @property
  *     def chrom(self):             # <<<<<<<<<<<<<<
  *         return self._chrom
  *     @chrom.setter
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":138
+/* "denovonear/gencode.pyx":141
  *         return self._chrom
  *     @chrom.setter
  *     def chrom(self, value):             # <<<<<<<<<<<<<<
  *         self._chrom = value
  * 
  */
 
@@ -4008,31 +4099,31 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "denovonear/gencode.pyx":139
+  /* "denovonear/gencode.pyx":142
  *     @chrom.setter
  *     def chrom(self, value):
  *         self._chrom = value             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 139, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 142, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_chrom);
   __Pyx_DECREF(__pyx_v_self->_chrom);
   __pyx_v_self->_chrom = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":138
+  /* "denovonear/gencode.pyx":141
  *         return self._chrom
  *     @chrom.setter
  *     def chrom(self, value):             # <<<<<<<<<<<<<<
  *         self._chrom = value
  * 
  */
 
@@ -4044,15 +4135,15 @@
   __Pyx_AddTraceback("denovonear.gencode.Gene.chrom.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":142
+/* "denovonear/gencode.pyx":145
  * 
  *     @property
  *     def start(self):             # <<<<<<<<<<<<<<
  *         return self._start
  *     @start.setter
  */
 
@@ -4074,29 +4165,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "denovonear/gencode.pyx":143
+  /* "denovonear/gencode.pyx":146
  *     @property
  *     def start(self):
  *         return self._start             # <<<<<<<<<<<<<<
  *     @start.setter
  *     def start(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_start); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":142
+  /* "denovonear/gencode.pyx":145
  * 
  *     @property
  *     def start(self):             # <<<<<<<<<<<<<<
  *         return self._start
  *     @start.setter
  */
 
@@ -4107,15 +4198,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":145
+/* "denovonear/gencode.pyx":148
  *         return self._start
  *     @start.setter
  *     def start(self, value):             # <<<<<<<<<<<<<<
  *         self._start = value
  * 
  */
 
@@ -4137,25 +4228,25 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "denovonear/gencode.pyx":146
+  /* "denovonear/gencode.pyx":149
  *     @start.setter
  *     def start(self, value):
  *         self._start = value             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 146, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 149, __pyx_L1_error)
   __pyx_v_self->_start = __pyx_t_1;
 
-  /* "denovonear/gencode.pyx":145
+  /* "denovonear/gencode.pyx":148
  *         return self._start
  *     @start.setter
  *     def start(self, value):             # <<<<<<<<<<<<<<
  *         self._start = value
  * 
  */
 
@@ -4166,15 +4257,15 @@
   __Pyx_AddTraceback("denovonear.gencode.Gene.start.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":149
+/* "denovonear/gencode.pyx":152
  * 
  *     @property
  *     def end(self):             # <<<<<<<<<<<<<<
  *         return self._end
  *     @end.setter
  */
 
@@ -4196,29 +4287,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "denovonear/gencode.pyx":150
+  /* "denovonear/gencode.pyx":153
  *     @property
  *     def end(self):
  *         return self._end             # <<<<<<<<<<<<<<
  *     @end.setter
  *     def end(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":149
+  /* "denovonear/gencode.pyx":152
  * 
  *     @property
  *     def end(self):             # <<<<<<<<<<<<<<
  *         return self._end
  *     @end.setter
  */
 
@@ -4229,15 +4320,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":152
+/* "denovonear/gencode.pyx":155
  *         return self._end
  *     @end.setter
  *     def end(self, value):             # <<<<<<<<<<<<<<
  *         self._end = value
  * 
  */
 
@@ -4259,25 +4350,25 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "denovonear/gencode.pyx":153
+  /* "denovonear/gencode.pyx":156
  *     @end.setter
  *     def end(self, value):
  *         self._end = value             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 153, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 156, __pyx_L1_error)
   __pyx_v_self->_end = __pyx_t_1;
 
-  /* "denovonear/gencode.pyx":152
+  /* "denovonear/gencode.pyx":155
  *         return self._end
  *     @end.setter
  *     def end(self, value):             # <<<<<<<<<<<<<<
  *         self._end = value
  * 
  */
 
@@ -4288,15 +4379,15 @@
   __Pyx_AddTraceback("denovonear.gencode.Gene.end.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":156
+/* "denovonear/gencode.pyx":159
  * 
  *     @property
  *     def strand(self):             # <<<<<<<<<<<<<<
  *         if self._transcripts.size() > 0:
  *             return chr(self._transcripts[0].get_strand())
  */
 
@@ -4320,64 +4411,64 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "denovonear/gencode.pyx":157
+  /* "denovonear/gencode.pyx":160
  *     @property
  *     def strand(self):
  *         if self._transcripts.size() > 0:             # <<<<<<<<<<<<<<
  *             return chr(self._transcripts[0].get_strand())
  *         raise IndexError('no transcripts in gene yet')
  */
   __pyx_t_1 = ((__pyx_v_self->_transcripts.size() > 0) != 0);
   if (__pyx_t_1) {
 
-    /* "denovonear/gencode.pyx":158
+    /* "denovonear/gencode.pyx":161
  *     def strand(self):
  *         if self._transcripts.size() > 0:
  *             return chr(self._transcripts[0].get_strand())             # <<<<<<<<<<<<<<
  *         raise IndexError('no transcripts in gene yet')
  * 
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_char((__pyx_v_self->_transcripts[0]).get_strand()); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_char((__pyx_v_self->_transcripts[0]).get_strand()); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_chr, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_chr, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 161, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "denovonear/gencode.pyx":157
+    /* "denovonear/gencode.pyx":160
  *     @property
  *     def strand(self):
  *         if self._transcripts.size() > 0:             # <<<<<<<<<<<<<<
  *             return chr(self._transcripts[0].get_strand())
  *         raise IndexError('no transcripts in gene yet')
  */
   }
 
-  /* "denovonear/gencode.pyx":159
+  /* "denovonear/gencode.pyx":162
  *         if self._transcripts.size() > 0:
  *             return chr(self._transcripts[0].get_strand())
  *         raise IndexError('no transcripts in gene yet')             # <<<<<<<<<<<<<<
  * 
  *     cdef _convert_exons(self, vector[Region] exons):
  */
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_IndexError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_Raise(__pyx_t_3, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __PYX_ERR(0, 159, __pyx_L1_error)
+  __PYX_ERR(0, 162, __pyx_L1_error)
 
-  /* "denovonear/gencode.pyx":156
+  /* "denovonear/gencode.pyx":159
  * 
  *     @property
  *     def strand(self):             # <<<<<<<<<<<<<<
  *         if self._transcripts.size() > 0:
  *             return chr(self._transcripts[0].get_strand())
  */
 
@@ -4389,15 +4480,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":161
+/* "denovonear/gencode.pyx":164
  *         raise IndexError('no transcripts in gene yet')
  * 
  *     cdef _convert_exons(self, vector[Region] exons):             # <<<<<<<<<<<<<<
  *         ''' convert vector of exon Regions to list of lists
  * 
  */
 
@@ -4412,52 +4503,52 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_convert_exons", 0);
 
-  /* "denovonear/gencode.pyx":167
+  /* "denovonear/gencode.pyx":170
  *         Transcript object.
  *         '''
  *         return [[y.start, y.end] for y in exons]             # <<<<<<<<<<<<<<
  * 
  *     cdef _to_Transcript(self, Tx tx):
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = __pyx_v_exons.begin();
     for (;;) {
       if (!(__pyx_t_2 != __pyx_v_exons.end())) break;
       __pyx_t_3 = *__pyx_t_2;
       ++__pyx_t_2;
       __pyx_8genexpr1__pyx_v_y = __pyx_t_3;
-      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_8genexpr1__pyx_v_y.start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_8genexpr1__pyx_v_y.start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 170, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_8genexpr1__pyx_v_y.end); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 167, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_8genexpr1__pyx_v_y.end); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 170, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = PyList_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 167, __pyx_L1_error)
+      __pyx_t_6 = PyList_New(2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 170, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GIVEREF(__pyx_t_4);
       PyList_SET_ITEM(__pyx_t_6, 0, __pyx_t_4);
       __Pyx_GIVEREF(__pyx_t_5);
       PyList_SET_ITEM(__pyx_t_6, 1, __pyx_t_5);
       __pyx_t_4 = 0;
       __pyx_t_5 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 167, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 170, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     }
   } /* exit inner scope */
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":161
+  /* "denovonear/gencode.pyx":164
  *         raise IndexError('no transcripts in gene yet')
  * 
  *     cdef _convert_exons(self, vector[Region] exons):             # <<<<<<<<<<<<<<
  *         ''' convert vector of exon Regions to list of lists
  * 
  */
 
@@ -4471,15 +4562,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":169
+/* "denovonear/gencode.pyx":172
  *         return [[y.start, y.end] for y in exons]
  * 
  *     cdef _to_Transcript(self, Tx tx):             # <<<<<<<<<<<<<<
  *         ''' construct Transcript (python object) from Tx (c++ object)
  *         '''
  */
 
@@ -4499,295 +4590,349 @@
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
+  std::string __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_to_Transcript", 0);
 
-  /* "denovonear/gencode.pyx":172
+  /* "denovonear/gencode.pyx":175
  *         ''' construct Transcript (python object) from Tx (c++ object)
  *         '''
  *         offset = 10 if tx.get_genomic_offset() == 0 else tx.get_genomic_offset()             # <<<<<<<<<<<<<<
  *         chrom = tx.get_chrom().decode('utf8')
  *         start = tx.get_start()
  */
   if (((__pyx_v_tx.get_genomic_offset() == 0) != 0)) {
     __Pyx_INCREF(__pyx_int_10);
     __pyx_t_1 = __pyx_int_10;
   } else {
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_tx.get_genomic_offset()); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_tx.get_genomic_offset()); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __pyx_t_2 = 0;
   }
   __pyx_v_offset = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":173
+  /* "denovonear/gencode.pyx":176
  *         '''
  *         offset = 10 if tx.get_genomic_offset() == 0 else tx.get_genomic_offset()
  *         chrom = tx.get_chrom().decode('utf8')             # <<<<<<<<<<<<<<
  *         start = tx.get_start()
  *         end = tx.get_end()
  */
-  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_tx.get_chrom(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_tx.get_chrom(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_chrom = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":174
+  /* "denovonear/gencode.pyx":177
  *         offset = 10 if tx.get_genomic_offset() == 0 else tx.get_genomic_offset()
  *         chrom = tx.get_chrom().decode('utf8')
  *         start = tx.get_start()             # <<<<<<<<<<<<<<
  *         end = tx.get_end()
  *         exons = self._convert_exons(tx.get_exons())
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_tx.get_start()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_tx.get_start()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_start = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":175
+  /* "denovonear/gencode.pyx":178
  *         chrom = tx.get_chrom().decode('utf8')
  *         start = tx.get_start()
  *         end = tx.get_end()             # <<<<<<<<<<<<<<
  *         exons = self._convert_exons(tx.get_exons())
  *         cds = self._convert_exons(tx.get_cds())
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_tx.get_end()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_tx.get_end()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_end = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":176
+  /* "denovonear/gencode.pyx":179
  *         start = tx.get_start()
  *         end = tx.get_end()
  *         exons = self._convert_exons(tx.get_exons())             # <<<<<<<<<<<<<<
  *         cds = self._convert_exons(tx.get_cds())
  *         seq = tx.get_genomic_sequence().decode('utf8')
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_self->__pyx_vtab)->_convert_exons(__pyx_v_self, __pyx_v_tx.get_exons()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_self->__pyx_vtab)->_convert_exons(__pyx_v_self, __pyx_v_tx.get_exons()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_exons = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":177
+  /* "denovonear/gencode.pyx":180
  *         end = tx.get_end()
  *         exons = self._convert_exons(tx.get_exons())
  *         cds = self._convert_exons(tx.get_cds())             # <<<<<<<<<<<<<<
  *         seq = tx.get_genomic_sequence().decode('utf8')
  *         if seq == '':
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_self->__pyx_vtab)->_convert_exons(__pyx_v_self, __pyx_v_tx.get_cds()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_self->__pyx_vtab)->_convert_exons(__pyx_v_self, __pyx_v_tx.get_cds()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_cds = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":178
+  /* "denovonear/gencode.pyx":181
  *         exons = self._convert_exons(tx.get_exons())
  *         cds = self._convert_exons(tx.get_cds())
  *         seq = tx.get_genomic_sequence().decode('utf8')             # <<<<<<<<<<<<<<
  *         if seq == '':
  *             seq = None
  */
-  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_tx.get_genomic_sequence(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_tx.get_genomic_sequence(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_seq = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":179
+  /* "denovonear/gencode.pyx":182
  *         cds = self._convert_exons(tx.get_cds())
  *         seq = tx.get_genomic_sequence().decode('utf8')
  *         if seq == '':             # <<<<<<<<<<<<<<
  *             seq = None
  *         if seq is None and __genome_ is not None:
  */
-  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_v_seq, __pyx_kp_u__6, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_v_seq, __pyx_kp_u__6, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 182, __pyx_L1_error)
   if (__pyx_t_3) {
 
-    /* "denovonear/gencode.pyx":180
+    /* "denovonear/gencode.pyx":183
  *         seq = tx.get_genomic_sequence().decode('utf8')
  *         if seq == '':
  *             seq = None             # <<<<<<<<<<<<<<
  *         if seq is None and __genome_ is not None:
  *             seq = __genome_[chrom][start-1-offset:end-1+offset].seq.upper()
  */
     __Pyx_INCREF(Py_None);
     __Pyx_DECREF_SET(__pyx_v_seq, Py_None);
 
-    /* "denovonear/gencode.pyx":179
+    /* "denovonear/gencode.pyx":182
  *         cds = self._convert_exons(tx.get_cds())
  *         seq = tx.get_genomic_sequence().decode('utf8')
  *         if seq == '':             # <<<<<<<<<<<<<<
  *             seq = None
  *         if seq is None and __genome_ is not None:
  */
   }
 
-  /* "denovonear/gencode.pyx":181
+  /* "denovonear/gencode.pyx":184
  *         if seq == '':
  *             seq = None
  *         if seq is None and __genome_ is not None:             # <<<<<<<<<<<<<<
  *             seq = __genome_[chrom][start-1-offset:end-1+offset].seq.upper()
- *         strand = self.strand
+ *         strand = chr(tx.get_strand())
  */
   __pyx_t_4 = (__pyx_v_seq == Py_None);
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
   } else {
     __pyx_t_3 = __pyx_t_5;
     goto __pyx_L5_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_genome); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_genome); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_5 = (__pyx_t_1 != Py_None);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_4 = (__pyx_t_5 != 0);
   __pyx_t_3 = __pyx_t_4;
   __pyx_L5_bool_binop_done:;
   if (__pyx_t_3) {
 
-    /* "denovonear/gencode.pyx":182
+    /* "denovonear/gencode.pyx":185
  *             seq = None
  *         if seq is None and __genome_ is not None:
  *             seq = __genome_[chrom][start-1-offset:end-1+offset].seq.upper()             # <<<<<<<<<<<<<<
- *         strand = self.strand
- *         tx_id = tx.get_name().decode('utf8')
+ *         strand = chr(tx.get_strand())
+ *         if strand == '-':
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_genome); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_genome); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_v_chrom); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetItem(__pyx_t_2, __pyx_v_chrom); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyInt_SubtractObjC(__pyx_v_start, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_SubtractObjC(__pyx_v_start, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = PyNumber_Subtract(__pyx_t_2, __pyx_v_offset); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_7 = PyNumber_Subtract(__pyx_t_2, __pyx_v_offset); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyInt_SubtractObjC(__pyx_v_end, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_SubtractObjC(__pyx_v_end, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = PyNumber_Add(__pyx_t_2, __pyx_v_offset); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_8 = PyNumber_Add(__pyx_t_2, __pyx_v_offset); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_t_6, 0, 0, &__pyx_t_7, &__pyx_t_8, NULL, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_t_6, 0, 0, &__pyx_t_7, &__pyx_t_8, NULL, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_seq); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_seq); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_upper); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_upper); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __pyx_t_8 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_8)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_8);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_seq, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "denovonear/gencode.pyx":181
+    /* "denovonear/gencode.pyx":184
  *         if seq == '':
  *             seq = None
  *         if seq is None and __genome_ is not None:             # <<<<<<<<<<<<<<
  *             seq = __genome_[chrom][start-1-offset:end-1+offset].seq.upper()
- *         strand = self.strand
+ *         strand = chr(tx.get_strand())
  */
   }
 
-  /* "denovonear/gencode.pyx":183
+  /* "denovonear/gencode.pyx":186
  *         if seq is None and __genome_ is not None:
  *             seq = __genome_[chrom][start-1-offset:end-1+offset].seq.upper()
- *         strand = self.strand             # <<<<<<<<<<<<<<
+ *         strand = chr(tx.get_strand())             # <<<<<<<<<<<<<<
+ *         if strand == '-':
+ *             seq = tx.reverse_complement(seq.encode('utf8')).decode('utf8')
+ */
+  __pyx_t_1 = __Pyx_PyInt_From_char(__pyx_v_tx.get_strand()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_chr, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_strand = __pyx_t_2;
+  __pyx_t_2 = 0;
+
+  /* "denovonear/gencode.pyx":187
+ *             seq = __genome_[chrom][start-1-offset:end-1+offset].seq.upper()
+ *         strand = chr(tx.get_strand())
+ *         if strand == '-':             # <<<<<<<<<<<<<<
+ *             seq = tx.reverse_complement(seq.encode('utf8')).decode('utf8')
+ *         tx_id = tx.get_name().decode('utf8')
+ */
+  __pyx_t_3 = (__Pyx_PyUnicode_Equals(__pyx_v_strand, __pyx_kp_u_, Py_EQ)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
+  if (__pyx_t_3) {
+
+    /* "denovonear/gencode.pyx":188
+ *         strand = chr(tx.get_strand())
+ *         if strand == '-':
+ *             seq = tx.reverse_complement(seq.encode('utf8')).decode('utf8')             # <<<<<<<<<<<<<<
  *         tx_id = tx.get_name().decode('utf8')
  *         return Transcript(tx_id, chrom, start, end, strand, exons, cds, seq, offset=offset)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_strand); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v_strand = __pyx_t_1;
-  __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_seq, __pyx_n_s_encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_8 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_8)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_8);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
+      }
+    }
+    __pyx_t_2 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_8, __pyx_n_u_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_n_u_utf8);
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 188, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_v_tx.reverse_complement(__pyx_t_9), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF_SET(__pyx_v_seq, __pyx_t_2);
+    __pyx_t_2 = 0;
 
-  /* "denovonear/gencode.pyx":184
+    /* "denovonear/gencode.pyx":187
  *             seq = __genome_[chrom][start-1-offset:end-1+offset].seq.upper()
- *         strand = self.strand
+ *         strand = chr(tx.get_strand())
+ *         if strand == '-':             # <<<<<<<<<<<<<<
+ *             seq = tx.reverse_complement(seq.encode('utf8')).decode('utf8')
+ *         tx_id = tx.get_name().decode('utf8')
+ */
+  }
+
+  /* "denovonear/gencode.pyx":189
+ *         if strand == '-':
+ *             seq = tx.reverse_complement(seq.encode('utf8')).decode('utf8')
  *         tx_id = tx.get_name().decode('utf8')             # <<<<<<<<<<<<<<
  *         return Transcript(tx_id, chrom, start, end, strand, exons, cds, seq, offset=offset)
  * 
  */
-  __pyx_t_1 = __Pyx_decode_cpp_string(__pyx_v_tx.get_name(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v_tx_id = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_2 = __Pyx_decode_cpp_string(__pyx_v_tx.get_name(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_tx_id = __pyx_t_2;
+  __pyx_t_2 = 0;
 
-  /* "denovonear/gencode.pyx":185
- *         strand = self.strand
+  /* "denovonear/gencode.pyx":190
+ *             seq = tx.reverse_complement(seq.encode('utf8')).decode('utf8')
  *         tx_id = tx.get_name().decode('utf8')
  *         return Transcript(tx_id, chrom, start, end, strand, exons, cds, seq, offset=offset)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Transcript); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Transcript); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyTuple_New(8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_tx_id);
   __Pyx_GIVEREF(__pyx_v_tx_id);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_tx_id);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_tx_id);
   __Pyx_INCREF(__pyx_v_chrom);
   __Pyx_GIVEREF(__pyx_v_chrom);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_chrom);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_chrom);
   __Pyx_INCREF(__pyx_v_start);
   __Pyx_GIVEREF(__pyx_v_start);
-  PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_v_start);
+  PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_v_start);
   __Pyx_INCREF(__pyx_v_end);
   __Pyx_GIVEREF(__pyx_v_end);
-  PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_v_end);
+  PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_v_end);
   __Pyx_INCREF(__pyx_v_strand);
   __Pyx_GIVEREF(__pyx_v_strand);
-  PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_v_strand);
+  PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_v_strand);
   __Pyx_INCREF(__pyx_v_exons);
   __Pyx_GIVEREF(__pyx_v_exons);
-  PyTuple_SET_ITEM(__pyx_t_2, 5, __pyx_v_exons);
+  PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_v_exons);
   __Pyx_INCREF(__pyx_v_cds);
   __Pyx_GIVEREF(__pyx_v_cds);
-  PyTuple_SET_ITEM(__pyx_t_2, 6, __pyx_v_cds);
+  PyTuple_SET_ITEM(__pyx_t_1, 6, __pyx_v_cds);
   __Pyx_INCREF(__pyx_v_seq);
   __Pyx_GIVEREF(__pyx_v_seq);
-  PyTuple_SET_ITEM(__pyx_t_2, 7, __pyx_v_seq);
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 185, __pyx_L1_error)
+  PyTuple_SET_ITEM(__pyx_t_1, 7, __pyx_v_seq);
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_offset, __pyx_v_offset) < 0) __PYX_ERR(0, 185, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 185, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_offset, __pyx_v_offset) < 0) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 190, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_r = __pyx_t_7;
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":169
+  /* "denovonear/gencode.pyx":172
  *         return [[y.start, y.end] for y in exons]
  * 
  *     cdef _to_Transcript(self, Tx tx):             # <<<<<<<<<<<<<<
  *         ''' construct Transcript (python object) from Tx (c++ object)
  *         '''
  */
 
@@ -4811,15 +4956,15 @@
   __Pyx_XDECREF(__pyx_v_strand);
   __Pyx_XDECREF(__pyx_v_tx_id);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":188
+/* "denovonear/gencode.pyx":193
  * 
  *     @property
  *     def transcripts(self):             # <<<<<<<<<<<<<<
  *         ''' get list of Transcripts for gene, with genomic DNA included
  *         '''
  */
 
@@ -4846,43 +4991,43 @@
   Tx __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "denovonear/gencode.pyx":191
+  /* "denovonear/gencode.pyx":196
  *         ''' get list of Transcripts for gene, with genomic DNA included
  *         '''
  *         return [self._to_Transcript(x) for x in self._transcripts]             # <<<<<<<<<<<<<<
  * 
  *     cdef int _cds_len(self, Tx tx):
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_3 = &__pyx_v_self->_transcripts;
     __pyx_t_2 = __pyx_t_3->begin();
     for (;;) {
       if (!(__pyx_t_2 != __pyx_t_3->end())) break;
       __pyx_t_4 = *__pyx_t_2;
       ++__pyx_t_2;
       __pyx_8genexpr2__pyx_v_x = __pyx_t_4;
-      __pyx_t_5 = ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_self->__pyx_vtab)->_to_Transcript(__pyx_v_self, __pyx_8genexpr2__pyx_v_x); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 191, __pyx_L1_error)
+      __pyx_t_5 = ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_self->__pyx_vtab)->_to_Transcript(__pyx_v_self, __pyx_8genexpr2__pyx_v_x); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 196, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 191, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 196, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
   } /* exit inner scope */
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":188
+  /* "denovonear/gencode.pyx":193
  * 
  *     @property
  *     def transcripts(self):             # <<<<<<<<<<<<<<
  *         ''' get list of Transcripts for gene, with genomic DNA included
  *         '''
  */
 
@@ -4894,15 +5039,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":193
+/* "denovonear/gencode.pyx":198
  *         return [self._to_Transcript(x) for x in self._transcripts]
  * 
  *     cdef int _cds_len(self, Tx tx):             # <<<<<<<<<<<<<<
  *         ''' get length of coding sequence for a Tx object based transcript
  *         '''
  */
 
@@ -4912,40 +5057,40 @@
   __Pyx_RefNannyDeclarations
   struct CDS_coords __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_cds_len", 0);
 
-  /* "denovonear/gencode.pyx":196
+  /* "denovonear/gencode.pyx":201
  *         ''' get length of coding sequence for a Tx object based transcript
  *         '''
  *         cdef CDS_coords coords = tx.get_coding_distance(tx.get_cds_end())             # <<<<<<<<<<<<<<
  *         return coords.position + 1
  * 
  */
   try {
     __pyx_t_1 = __pyx_v_tx.get_coding_distance(__pyx_v_tx.get_cds_end());
   } catch(...) {
     __Pyx_CppExn2PyErr();
-    __PYX_ERR(0, 196, __pyx_L1_error)
+    __PYX_ERR(0, 201, __pyx_L1_error)
   }
   __pyx_v_coords = __pyx_t_1;
 
-  /* "denovonear/gencode.pyx":197
+  /* "denovonear/gencode.pyx":202
  *         '''
  *         cdef CDS_coords coords = tx.get_coding_distance(tx.get_cds_end())
  *         return coords.position + 1             # <<<<<<<<<<<<<<
  * 
  *     cdef Tx _max_by_cds(self, vector[Tx] transcripts):
  */
   __pyx_r = (__pyx_v_coords.position + 1);
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":193
+  /* "denovonear/gencode.pyx":198
  *         return [self._to_Transcript(x) for x in self._transcripts]
  * 
  *     cdef int _cds_len(self, Tx tx):             # <<<<<<<<<<<<<<
  *         ''' get length of coding sequence for a Tx object based transcript
  *         '''
  */
 
@@ -4954,15 +5099,15 @@
   __Pyx_WriteUnraisable("denovonear.gencode.Gene._cds_len", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":199
+/* "denovonear/gencode.pyx":204
  *         return coords.position + 1
  * 
  *     cdef Tx _max_by_cds(self, vector[Tx] transcripts):             # <<<<<<<<<<<<<<
  *         ''' get longest transcript by CDS length
  *         '''
  */
 
@@ -4974,117 +5119,117 @@
   Tx __pyx_r;
   __Pyx_RefNannyDeclarations
   std::vector<Tx> ::iterator __pyx_t_1;
   Tx __pyx_t_2;
   int __pyx_t_3;
   __Pyx_RefNannySetupContext("_max_by_cds", 0);
 
-  /* "denovonear/gencode.pyx":203
+  /* "denovonear/gencode.pyx":208
  *         '''
  *         cdef Tx max_tx
  *         length = 0             # <<<<<<<<<<<<<<
  *         for tx in transcripts:
  *             curr_len = self._cds_len(tx)
  */
   __pyx_v_length = 0;
 
-  /* "denovonear/gencode.pyx":204
+  /* "denovonear/gencode.pyx":209
  *         cdef Tx max_tx
  *         length = 0
  *         for tx in transcripts:             # <<<<<<<<<<<<<<
  *             curr_len = self._cds_len(tx)
  *             if curr_len > length:
  */
   __pyx_t_1 = __pyx_v_transcripts.begin();
   for (;;) {
     if (!(__pyx_t_1 != __pyx_v_transcripts.end())) break;
     __pyx_t_2 = *__pyx_t_1;
     ++__pyx_t_1;
     __pyx_v_tx = __pyx_t_2;
 
-    /* "denovonear/gencode.pyx":205
+    /* "denovonear/gencode.pyx":210
  *         length = 0
  *         for tx in transcripts:
  *             curr_len = self._cds_len(tx)             # <<<<<<<<<<<<<<
  *             if curr_len > length:
  *                 length = curr_len
  */
     __pyx_v_curr_len = ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_self->__pyx_vtab)->_cds_len(__pyx_v_self, __pyx_v_tx);
 
-    /* "denovonear/gencode.pyx":206
+    /* "denovonear/gencode.pyx":211
  *         for tx in transcripts:
  *             curr_len = self._cds_len(tx)
  *             if curr_len > length:             # <<<<<<<<<<<<<<
  *                 length = curr_len
  *                 max_tx = tx
  */
     __pyx_t_3 = ((__pyx_v_curr_len > __pyx_v_length) != 0);
     if (__pyx_t_3) {
 
-      /* "denovonear/gencode.pyx":207
+      /* "denovonear/gencode.pyx":212
  *             curr_len = self._cds_len(tx)
  *             if curr_len > length:
  *                 length = curr_len             # <<<<<<<<<<<<<<
  *                 max_tx = tx
  *         return max_tx
  */
       __pyx_v_length = __pyx_v_curr_len;
 
-      /* "denovonear/gencode.pyx":208
+      /* "denovonear/gencode.pyx":213
  *             if curr_len > length:
  *                 length = curr_len
  *                 max_tx = tx             # <<<<<<<<<<<<<<
  *         return max_tx
  * 
  */
       __pyx_v_max_tx = __pyx_v_tx;
 
-      /* "denovonear/gencode.pyx":206
+      /* "denovonear/gencode.pyx":211
  *         for tx in transcripts:
  *             curr_len = self._cds_len(tx)
  *             if curr_len > length:             # <<<<<<<<<<<<<<
  *                 length = curr_len
  *                 max_tx = tx
  */
     }
 
-    /* "denovonear/gencode.pyx":204
+    /* "denovonear/gencode.pyx":209
  *         cdef Tx max_tx
  *         length = 0
  *         for tx in transcripts:             # <<<<<<<<<<<<<<
  *             curr_len = self._cds_len(tx)
  *             if curr_len > length:
  */
   }
 
-  /* "denovonear/gencode.pyx":209
+  /* "denovonear/gencode.pyx":214
  *                 length = curr_len
  *                 max_tx = tx
  *         return max_tx             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __pyx_r = __pyx_v_max_tx;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":199
+  /* "denovonear/gencode.pyx":204
  *         return coords.position + 1
  * 
  *     cdef Tx _max_by_cds(self, vector[Tx] transcripts):             # <<<<<<<<<<<<<<
  *         ''' get longest transcript by CDS length
  *         '''
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":212
+/* "denovonear/gencode.pyx":217
  * 
  *     @property
  *     def canonical(self):             # <<<<<<<<<<<<<<
  *         ''' find the canonical transcript for a gene.
  * 
  */
 
@@ -5113,104 +5258,104 @@
   std::vector<Tx>  __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "denovonear/gencode.pyx":223
+  /* "denovonear/gencode.pyx":228
  *         '''
  *         cdef vector[Tx] principal
  *         for i in range(self._transcripts.size()):             # <<<<<<<<<<<<<<
  *             if self._principal[i]:
  *                 principal.push_back(self._transcripts[i])
  */
   __pyx_t_1 = __pyx_v_self->_transcripts.size();
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "denovonear/gencode.pyx":224
+    /* "denovonear/gencode.pyx":229
  *         cdef vector[Tx] principal
  *         for i in range(self._transcripts.size()):
  *             if self._principal[i]:             # <<<<<<<<<<<<<<
  *                 principal.push_back(self._transcripts[i])
  * 
  */
     __pyx_t_4 = ((__pyx_v_self->_principal[__pyx_v_i]) != 0);
     if (__pyx_t_4) {
 
-      /* "denovonear/gencode.pyx":225
+      /* "denovonear/gencode.pyx":230
  *         for i in range(self._transcripts.size()):
  *             if self._principal[i]:
  *                 principal.push_back(self._transcripts[i])             # <<<<<<<<<<<<<<
  * 
  *         if principal.size() == 0:
  */
       try {
         __pyx_v_principal.push_back((__pyx_v_self->_transcripts[__pyx_v_i]));
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 225, __pyx_L1_error)
+        __PYX_ERR(0, 230, __pyx_L1_error)
       }
 
-      /* "denovonear/gencode.pyx":224
+      /* "denovonear/gencode.pyx":229
  *         cdef vector[Tx] principal
  *         for i in range(self._transcripts.size()):
  *             if self._principal[i]:             # <<<<<<<<<<<<<<
  *                 principal.push_back(self._transcripts[i])
  * 
  */
     }
   }
 
-  /* "denovonear/gencode.pyx":227
+  /* "denovonear/gencode.pyx":232
  *                 principal.push_back(self._transcripts[i])
  * 
  *         if principal.size() == 0:             # <<<<<<<<<<<<<<
  *             principal = self._transcripts
  * 
  */
   __pyx_t_4 = ((__pyx_v_principal.size() == 0) != 0);
   if (__pyx_t_4) {
 
-    /* "denovonear/gencode.pyx":228
+    /* "denovonear/gencode.pyx":233
  * 
  *         if principal.size() == 0:
  *             principal = self._transcripts             # <<<<<<<<<<<<<<
  * 
  *         # cdef Tx tx = self._max_by_cds(principal)
  */
     __pyx_t_5 = __pyx_v_self->_transcripts;
     __pyx_v_principal = __pyx_t_5;
 
-    /* "denovonear/gencode.pyx":227
+    /* "denovonear/gencode.pyx":232
  *                 principal.push_back(self._transcripts[i])
  * 
  *         if principal.size() == 0:             # <<<<<<<<<<<<<<
  *             principal = self._transcripts
  * 
  */
   }
 
-  /* "denovonear/gencode.pyx":231
+  /* "denovonear/gencode.pyx":236
  * 
  *         # cdef Tx tx = self._max_by_cds(principal)
  *         return self._to_Transcript(self._max_by_cds(principal))             # <<<<<<<<<<<<<<
  * 
  *     def in_any_tx_cds(self, pos):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_6 = ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_self->__pyx_vtab)->_to_Transcript(__pyx_v_self, ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_self->__pyx_vtab)->_max_by_cds(__pyx_v_self, __pyx_v_principal)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 231, __pyx_L1_error)
+  __pyx_t_6 = ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_self->__pyx_vtab)->_to_Transcript(__pyx_v_self, ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_self->__pyx_vtab)->_max_by_cds(__pyx_v_self, __pyx_v_principal)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 236, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":212
+  /* "denovonear/gencode.pyx":217
  * 
  *     @property
  *     def canonical(self):             # <<<<<<<<<<<<<<
  *         ''' find the canonical transcript for a gene.
  * 
  */
 
@@ -5221,15 +5366,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":233
+/* "denovonear/gencode.pyx":238
  *         return self._to_Transcript(self._max_by_cds(principal))
  * 
  *     def in_any_tx_cds(self, pos):             # <<<<<<<<<<<<<<
  *         ''' find if a pos is in coding region of any transcript of a gene
  *         '''
  */
 
@@ -5244,15 +5389,15 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_10denovonear_7gencode_4Gene_13in_any_tx_cds_2generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "denovonear/gencode.pyx":236
+/* "denovonear/gencode.pyx":241
  *         ''' find if a pos is in coding region of any transcript of a gene
  *         '''
  *         return any(tx.in_coding_region(pos) for tx in self._transcripts)             # <<<<<<<<<<<<<<
  * 
  * cdef class Gencode:
  */
 
@@ -5264,23 +5409,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_1_genexpr *)__pyx_tp_new_10denovonear_7gencode___pyx_scope_struct_1_genexpr(__pyx_ptype_10denovonear_7gencode___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 236, __pyx_L1_error)
+    __PYX_ERR(0, 241, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10denovonear_7gencode_4Gene_13in_any_tx_cds_2generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_in_any_tx_cds_locals_genexpr, __pyx_n_s_denovonear_gencode); if (unlikely(!gen)) __PYX_ERR(0, 236, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10denovonear_7gencode_4Gene_13in_any_tx_cds_2generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_in_any_tx_cds_locals_genexpr, __pyx_n_s_denovonear_gencode); if (unlikely(!gen)) __PYX_ERR(0, 241, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -5309,25 +5454,25 @@
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 236, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 236, __pyx_L1_error) }
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 241, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 241, __pyx_L1_error) }
   __pyx_t_2 = &__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self->_transcripts;
   __pyx_t_1 = __pyx_t_2->begin();
   for (;;) {
     if (!(__pyx_t_1 != __pyx_t_2->end())) break;
     __pyx_t_3 = *__pyx_t_1;
     ++__pyx_t_1;
     __pyx_cur_scope->__pyx_v_tx = __pyx_t_3;
-    if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_pos)) { __Pyx_RaiseClosureNameError("pos"); __PYX_ERR(0, 236, __pyx_L1_error) }
-    __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_pos); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 236, __pyx_L1_error)
+    if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_pos)) { __Pyx_RaiseClosureNameError("pos"); __PYX_ERR(0, 241, __pyx_L1_error) }
+    __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_pos); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 241, __pyx_L1_error)
     __pyx_t_5 = (__pyx_cur_scope->__pyx_v_tx.in_coding_region(__pyx_t_4) != 0);
     if (__pyx_t_5) {
       __Pyx_XDECREF(__pyx_r);
       __Pyx_INCREF(Py_True);
       __pyx_r = Py_True;
       goto __pyx_L0;
     }
@@ -5351,81 +5496,79 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":233
+/* "denovonear/gencode.pyx":238
  *         return self._to_Transcript(self._max_by_cds(principal))
  * 
  *     def in_any_tx_cds(self, pos):             # <<<<<<<<<<<<<<
  *         ''' find if a pos is in coding region of any transcript of a gene
  *         '''
  */
 
 static PyObject *__pyx_pf_10denovonear_7gencode_4Gene_6in_any_tx_cds(struct __pyx_obj_10denovonear_7gencode_Gene *__pyx_v_self, PyObject *__pyx_v_pos) {
   struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds *__pyx_cur_scope;
-  PyObject *__pyx_gb_10denovonear_7gencode_4Gene_13in_any_tx_cds_2generator1 = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("in_any_tx_cds", 0);
   __pyx_cur_scope = (struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds *)__pyx_tp_new_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds(__pyx_ptype_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 233, __pyx_L1_error)
+    __PYX_ERR(0, 238, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __pyx_cur_scope->__pyx_v_pos = __pyx_v_pos;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_v_pos);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_pos);
 
-  /* "denovonear/gencode.pyx":236
+  /* "denovonear/gencode.pyx":241
  *         ''' find if a pos is in coding region of any transcript of a gene
  *         '''
  *         return any(tx.in_coding_region(pos) for tx in self._transcripts)             # <<<<<<<<<<<<<<
  * 
  * cdef class Gencode:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_pf_10denovonear_7gencode_4Gene_13in_any_tx_cds_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_1 = __pyx_pf_10denovonear_7gencode_4Gene_13in_any_tx_cds_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_Generator_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Generator_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":233
+  /* "denovonear/gencode.pyx":238
  *         return self._to_Transcript(self._max_by_cds(principal))
  * 
  *     def in_any_tx_cds(self, pos):             # <<<<<<<<<<<<<<
  *         ''' find if a pos is in coding region of any transcript of a gene
  *         '''
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("denovonear.gencode.Gene.in_any_tx_cds", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_gb_10denovonear_7gencode_4Gene_13in_any_tx_cds_2generator1);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
@@ -5537,15 +5680,15 @@
   __Pyx_AddTraceback("denovonear.gencode.Gene.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":241
+/* "denovonear/gencode.pyx":246
  *     cdef dict genes
  *     cdef list coords
  *     def __cinit__(self, gencode=None, fasta=None, coding_only=True):             # <<<<<<<<<<<<<<
  *         ''' initialise Gencode
  * 
  */
 
@@ -5597,15 +5740,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_coding_only);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 241, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 246, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -5617,15 +5760,15 @@
     }
     __pyx_v_gencode = values[0];
     __pyx_v_fasta = values[1];
     __pyx_v_coding_only = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 241, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 246, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("denovonear.gencode.Gencode.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10denovonear_7gencode_7Gencode___cinit__(((struct __pyx_obj_10denovonear_7gencode_Gencode *)__pyx_v_self), __pyx_v_gencode, __pyx_v_fasta, __pyx_v_coding_only);
 
@@ -5652,54 +5795,54 @@
   std::vector<struct gencode::NamedTx> ::iterator __pyx_t_9;
   struct gencode::NamedTx __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "denovonear/gencode.pyx":249
+  /* "denovonear/gencode.pyx":254
  *             coding: restrict to protein_coding only by default
  *         '''
  *         self.genes = {}             # <<<<<<<<<<<<<<
  *         if fasta:
  *             logging.info(f'opening genome fasta: {fasta}')
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 249, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->genes);
   __Pyx_DECREF(__pyx_v_self->genes);
   __pyx_v_self->genes = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":250
+  /* "denovonear/gencode.pyx":255
  *         '''
  *         self.genes = {}
  *         if fasta:             # <<<<<<<<<<<<<<
  *             logging.info(f'opening genome fasta: {fasta}')
  *             global __genome_
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_fasta); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 250, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_fasta); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 255, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "denovonear/gencode.pyx":251
+    /* "denovonear/gencode.pyx":256
  *         self.genes = {}
  *         if fasta:
  *             logging.info(f'opening genome fasta: {fasta}')             # <<<<<<<<<<<<<<
  *             global __genome_
  *             __genome_ = Fasta(str(fasta))
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 251, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_logging); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 256, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 251, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_info); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 256, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_v_fasta, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 251, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_FormatSimple(__pyx_v_fasta, __pyx_empty_unicode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 256, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_kp_u_opening_genome_fasta, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 251, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyUnicode_Concat(__pyx_kp_u_opening_genome_fasta, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 256, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -5707,73 +5850,73 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "denovonear/gencode.pyx":253
+    /* "denovonear/gencode.pyx":258
  *             logging.info(f'opening genome fasta: {fasta}')
  *             global __genome_
  *             __genome_ = Fasta(str(fasta))             # <<<<<<<<<<<<<<
  *         logging.info(f'opening gencode annotations: {gencode}')
  *         cdef vector[NamedTx] transcripts
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Fasta); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Fasta); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 258, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_fasta); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 253, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_fasta); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 258, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 253, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 258, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (PyDict_SetItem(__pyx_d, __pyx_n_s_genome, __pyx_t_1) < 0) __PYX_ERR(0, 253, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_d, __pyx_n_s_genome, __pyx_t_1) < 0) __PYX_ERR(0, 258, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "denovonear/gencode.pyx":250
+    /* "denovonear/gencode.pyx":255
  *         '''
  *         self.genes = {}
  *         if fasta:             # <<<<<<<<<<<<<<
  *             logging.info(f'opening genome fasta: {fasta}')
  *             global __genome_
  */
   }
 
-  /* "denovonear/gencode.pyx":254
+  /* "denovonear/gencode.pyx":259
  *             global __genome_
  *             __genome_ = Fasta(str(fasta))
  *         logging.info(f'opening gencode annotations: {gencode}')             # <<<<<<<<<<<<<<
  *         cdef vector[NamedTx] transcripts
  *         cdef Gene curr
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_logging); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 254, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_logging); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_info); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 254, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_info); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_gencode, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 254, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_v_gencode, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_opening_gencode_annotations, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 254, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_kp_u_opening_gencode_annotations, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -5781,217 +5924,217 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 254, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":257
+  /* "denovonear/gencode.pyx":262
  *         cdef vector[NamedTx] transcripts
  *         cdef Gene curr
  *         if gencode is not None:             # <<<<<<<<<<<<<<
  *             transcripts = open_gencode(str(gencode).encode('utf8'), coding_only)
  *             for x in transcripts:
  */
   __pyx_t_2 = (__pyx_v_gencode != Py_None);
   __pyx_t_6 = (__pyx_t_2 != 0);
   if (__pyx_t_6) {
 
-    /* "denovonear/gencode.pyx":258
+    /* "denovonear/gencode.pyx":263
  *         cdef Gene curr
  *         if gencode is not None:
  *             transcripts = open_gencode(str(gencode).encode('utf8'), coding_only)             # <<<<<<<<<<<<<<
  *             for x in transcripts:
  *                 symbol = x.symbol.decode('utf8')
  */
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_gencode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 258, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_gencode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = PyUnicode_AsUTF8String(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 258, __pyx_L1_error)
+    __pyx_t_5 = PyUnicode_AsUTF8String(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_7 = __pyx_convert_string_from_py_std__in_string(__pyx_t_5); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 258, __pyx_L1_error)
+    __pyx_t_7 = __pyx_convert_string_from_py_std__in_string(__pyx_t_5); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 263, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_coding_only); if (unlikely((__pyx_t_8 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 258, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_v_coding_only); if (unlikely((__pyx_t_8 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 263, __pyx_L1_error)
     __pyx_v_transcripts = gencode::open_gencode(__pyx_t_7, __pyx_t_8);
 
-    /* "denovonear/gencode.pyx":259
+    /* "denovonear/gencode.pyx":264
  *         if gencode is not None:
  *             transcripts = open_gencode(str(gencode).encode('utf8'), coding_only)
  *             for x in transcripts:             # <<<<<<<<<<<<<<
  *                 symbol = x.symbol.decode('utf8')
  *                 if symbol not in self.genes:
  */
     __pyx_t_9 = __pyx_v_transcripts.begin();
     for (;;) {
       if (!(__pyx_t_9 != __pyx_v_transcripts.end())) break;
       __pyx_t_10 = *__pyx_t_9;
       ++__pyx_t_9;
       __pyx_v_x = __pyx_t_10;
 
-      /* "denovonear/gencode.pyx":260
+      /* "denovonear/gencode.pyx":265
  *             transcripts = open_gencode(str(gencode).encode('utf8'), coding_only)
  *             for x in transcripts:
  *                 symbol = x.symbol.decode('utf8')             # <<<<<<<<<<<<<<
  *                 if symbol not in self.genes:
  *                     self.genes[symbol] = Gene(symbol.encode('utf8'))
  */
-      __pyx_t_5 = __Pyx_decode_cpp_string(__pyx_v_x.symbol, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 260, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_decode_cpp_string(__pyx_v_x.symbol, 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_XDECREF_SET(__pyx_v_symbol, __pyx_t_5);
       __pyx_t_5 = 0;
 
-      /* "denovonear/gencode.pyx":261
+      /* "denovonear/gencode.pyx":266
  *             for x in transcripts:
  *                 symbol = x.symbol.decode('utf8')
  *                 if symbol not in self.genes:             # <<<<<<<<<<<<<<
  *                     self.genes[symbol] = Gene(symbol.encode('utf8'))
  *                 curr = self.genes[symbol]
  */
       if (unlikely(__pyx_v_self->genes == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-        __PYX_ERR(0, 261, __pyx_L1_error)
+        __PYX_ERR(0, 266, __pyx_L1_error)
       }
-      __pyx_t_6 = (__Pyx_PyDict_ContainsTF(__pyx_v_symbol, __pyx_v_self->genes, Py_NE)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 261, __pyx_L1_error)
+      __pyx_t_6 = (__Pyx_PyDict_ContainsTF(__pyx_v_symbol, __pyx_v_self->genes, Py_NE)); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 266, __pyx_L1_error)
       __pyx_t_2 = (__pyx_t_6 != 0);
       if (__pyx_t_2) {
 
-        /* "denovonear/gencode.pyx":262
+        /* "denovonear/gencode.pyx":267
  *                 symbol = x.symbol.decode('utf8')
  *                 if symbol not in self.genes:
  *                     self.genes[symbol] = Gene(symbol.encode('utf8'))             # <<<<<<<<<<<<<<
  *                 curr = self.genes[symbol]
  *                 curr.add_tx(x.tx, x.is_principal)
  */
-        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_symbol, __pyx_n_s_encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_symbol, __pyx_n_s_encode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_t_3 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
           __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_1);
           if (likely(__pyx_t_3)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
             __Pyx_INCREF(__pyx_t_3);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_1, function);
           }
         }
         __pyx_t_5 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_3, __pyx_n_u_utf8) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_n_u_utf8);
         __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 262, __pyx_L1_error)
+        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 267, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-        __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10denovonear_7gencode_Gene), __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 262, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_10denovonear_7gencode_Gene), __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 267, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         if (unlikely(__pyx_v_self->genes == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 262, __pyx_L1_error)
+          __PYX_ERR(0, 267, __pyx_L1_error)
         }
-        if (unlikely(PyDict_SetItem(__pyx_v_self->genes, __pyx_v_symbol, __pyx_t_1) < 0)) __PYX_ERR(0, 262, __pyx_L1_error)
+        if (unlikely(PyDict_SetItem(__pyx_v_self->genes, __pyx_v_symbol, __pyx_t_1) < 0)) __PYX_ERR(0, 267, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-        /* "denovonear/gencode.pyx":261
+        /* "denovonear/gencode.pyx":266
  *             for x in transcripts:
  *                 symbol = x.symbol.decode('utf8')
  *                 if symbol not in self.genes:             # <<<<<<<<<<<<<<
  *                     self.genes[symbol] = Gene(symbol.encode('utf8'))
  *                 curr = self.genes[symbol]
  */
       }
 
-      /* "denovonear/gencode.pyx":263
+      /* "denovonear/gencode.pyx":268
  *                 if symbol not in self.genes:
  *                     self.genes[symbol] = Gene(symbol.encode('utf8'))
  *                 curr = self.genes[symbol]             # <<<<<<<<<<<<<<
  *                 curr.add_tx(x.tx, x.is_principal)
  *                 self.genes[symbol] = curr
  */
       if (unlikely(__pyx_v_self->genes == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 263, __pyx_L1_error)
+        __PYX_ERR(0, 268, __pyx_L1_error)
       }
-      __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_self->genes, __pyx_v_symbol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 263, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_self->genes, __pyx_v_symbol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 268, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_10denovonear_7gencode_Gene))))) __PYX_ERR(0, 263, __pyx_L1_error)
+      if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_10denovonear_7gencode_Gene))))) __PYX_ERR(0, 268, __pyx_L1_error)
       __Pyx_XDECREF_SET(__pyx_v_curr, ((struct __pyx_obj_10denovonear_7gencode_Gene *)__pyx_t_1));
       __pyx_t_1 = 0;
 
-      /* "denovonear/gencode.pyx":264
+      /* "denovonear/gencode.pyx":269
  *                     self.genes[symbol] = Gene(symbol.encode('utf8'))
  *                 curr = self.genes[symbol]
  *                 curr.add_tx(x.tx, x.is_principal)             # <<<<<<<<<<<<<<
  *                 self.genes[symbol] = curr
  *         self._sort()
  */
-      __pyx_t_1 = ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_curr->__pyx_vtab)->add_tx(__pyx_v_curr, __pyx_v_x.tx, __pyx_v_x.is_principal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 264, __pyx_L1_error)
+      __pyx_t_1 = ((struct __pyx_vtabstruct_10denovonear_7gencode_Gene *)__pyx_v_curr->__pyx_vtab)->add_tx(__pyx_v_curr, __pyx_v_x.tx, __pyx_v_x.is_principal); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 269, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "denovonear/gencode.pyx":265
+      /* "denovonear/gencode.pyx":270
  *                 curr = self.genes[symbol]
  *                 curr.add_tx(x.tx, x.is_principal)
  *                 self.genes[symbol] = curr             # <<<<<<<<<<<<<<
  *         self._sort()
  * 
  */
       if (unlikely(__pyx_v_self->genes == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 265, __pyx_L1_error)
+        __PYX_ERR(0, 270, __pyx_L1_error)
       }
-      if (unlikely(PyDict_SetItem(__pyx_v_self->genes, __pyx_v_symbol, ((PyObject *)__pyx_v_curr)) < 0)) __PYX_ERR(0, 265, __pyx_L1_error)
+      if (unlikely(PyDict_SetItem(__pyx_v_self->genes, __pyx_v_symbol, ((PyObject *)__pyx_v_curr)) < 0)) __PYX_ERR(0, 270, __pyx_L1_error)
 
-      /* "denovonear/gencode.pyx":259
+      /* "denovonear/gencode.pyx":264
  *         if gencode is not None:
  *             transcripts = open_gencode(str(gencode).encode('utf8'), coding_only)
  *             for x in transcripts:             # <<<<<<<<<<<<<<
  *                 symbol = x.symbol.decode('utf8')
  *                 if symbol not in self.genes:
  */
     }
 
-    /* "denovonear/gencode.pyx":257
+    /* "denovonear/gencode.pyx":262
  *         cdef vector[NamedTx] transcripts
  *         cdef Gene curr
  *         if gencode is not None:             # <<<<<<<<<<<<<<
  *             transcripts = open_gencode(str(gencode).encode('utf8'), coding_only)
  *             for x in transcripts:
  */
   }
 
-  /* "denovonear/gencode.pyx":266
+  /* "denovonear/gencode.pyx":271
  *                 curr.add_tx(x.tx, x.is_principal)
  *                 self.genes[symbol] = curr
  *         self._sort()             # <<<<<<<<<<<<<<
  * 
  *     def _sort(self):
  */
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_sort); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_sort); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 271, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":241
+  /* "denovonear/gencode.pyx":246
  *     cdef dict genes
  *     cdef list coords
  *     def __cinit__(self, gencode=None, fasta=None, coding_only=True):             # <<<<<<<<<<<<<<
  *         ''' initialise Gencode
  * 
  */
 
@@ -6008,15 +6151,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_curr);
   __Pyx_XDECREF(__pyx_v_symbol);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":268
+/* "denovonear/gencode.pyx":273
  *         self._sort()
  * 
  *     def _sort(self):             # <<<<<<<<<<<<<<
  *         self.coords = sorted(((x.chrom, x.start, x.end), symbol) for symbol, x in self.genes.items())
  * 
  */
 
@@ -6030,15 +6173,15 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_10denovonear_7gencode_7Gencode_5_sort_2generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "denovonear/gencode.pyx":269
+/* "denovonear/gencode.pyx":274
  * 
  *     def _sort(self):
  *         self.coords = sorted(((x.chrom, x.start, x.end), symbol) for symbol, x in self.genes.items())             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
 
@@ -6050,23 +6193,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_3_genexpr *)__pyx_tp_new_10denovonear_7gencode___pyx_scope_struct_3_genexpr(__pyx_ptype_10denovonear_7gencode___pyx_scope_struct_3_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_3_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 269, __pyx_L1_error)
+    __PYX_ERR(0, 274, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_2__sort *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10denovonear_7gencode_7Gencode_5_sort_2generator2, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_sort_locals_genexpr, __pyx_n_s_denovonear_gencode); if (unlikely(!gen)) __PYX_ERR(0, 269, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10denovonear_7gencode_7Gencode_5_sort_2generator2, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_sort_locals_genexpr, __pyx_n_s_denovonear_gencode); if (unlikely(!gen)) __PYX_ERR(0, 274, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6099,68 +6242,68 @@
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 269, __pyx_L1_error)
-  __pyx_r = PyList_New(0); if (unlikely(!__pyx_r)) __PYX_ERR(0, 269, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_r = PyList_New(0); if (unlikely(!__pyx_r)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_r);
   __pyx_t_2 = 0;
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 269, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 274, __pyx_L1_error) }
   if (unlikely(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self->genes == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-    __PYX_ERR(0, 269, __pyx_L1_error)
+    __PYX_ERR(0, 274, __pyx_L1_error)
   }
-  __pyx_t_5 = __Pyx_dict_iterator(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self->genes, 1, __pyx_n_s_items, (&__pyx_t_3), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_dict_iterator(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self->genes, 1, __pyx_n_s_items, (&__pyx_t_3), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_1);
   __pyx_t_1 = __pyx_t_5;
   __pyx_t_5 = 0;
   while (1) {
     __pyx_t_7 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_3, &__pyx_t_2, &__pyx_t_5, &__pyx_t_6, NULL, __pyx_t_4);
     if (unlikely(__pyx_t_7 == 0)) break;
-    if (unlikely(__pyx_t_7 == -1)) __PYX_ERR(0, 269, __pyx_L1_error)
+    if (unlikely(__pyx_t_7 == -1)) __PYX_ERR(0, 274, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_symbol);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_symbol, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_x);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_x, __pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_6);
     __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_x, __pyx_n_s_chrom); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 269, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_x, __pyx_n_s_chrom); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 274, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_x, __pyx_n_s_start); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 269, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_x, __pyx_n_s_start); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 274, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_x, __pyx_n_s_end); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 269, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_x, __pyx_n_s_end); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 274, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 269, __pyx_L1_error)
+    __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 274, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_GIVEREF(__pyx_t_6);
     PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_6);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_8);
     PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_t_8);
     __pyx_t_6 = 0;
     __pyx_t_5 = 0;
     __pyx_t_8 = 0;
-    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 269, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 274, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_GIVEREF(__pyx_t_9);
     PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_9);
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_symbol);
     __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_symbol);
     PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_cur_scope->__pyx_v_symbol);
     __pyx_t_9 = 0;
-    if (unlikely(__Pyx_ListComp_Append(__pyx_r, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 269, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_r, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 274, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   goto __pyx_L0;
@@ -6179,69 +6322,68 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":268
+/* "denovonear/gencode.pyx":273
  *         self._sort()
  * 
  *     def _sort(self):             # <<<<<<<<<<<<<<
  *         self.coords = sorted(((x.chrom, x.start, x.end), symbol) for symbol, x in self.genes.items())
  * 
  */
 
 static PyObject *__pyx_pf_10denovonear_7gencode_7Gencode_2_sort(struct __pyx_obj_10denovonear_7gencode_Gencode *__pyx_v_self) {
   struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_2__sort *__pyx_cur_scope;
-  PyObject *__pyx_gb_10denovonear_7gencode_7Gencode_5_sort_2generator2 = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_sort", 0);
   __pyx_cur_scope = (struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_2__sort *)__pyx_tp_new_10denovonear_7gencode___pyx_scope_struct_2__sort(__pyx_ptype_10denovonear_7gencode___pyx_scope_struct_2__sort, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_2__sort *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 268, __pyx_L1_error)
+    __PYX_ERR(0, 273, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
 
-  /* "denovonear/gencode.pyx":269
+  /* "denovonear/gencode.pyx":274
  * 
  *     def _sort(self):
  *         self.coords = sorted(((x.chrom, x.start, x.end), symbol) for symbol, x in self.genes.items())             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
-  __pyx_t_2 = __pyx_pf_10denovonear_7gencode_7Gencode_5_sort_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_2 = __pyx_pf_10denovonear_7gencode_7Gencode_5_sort_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_Generator_Next(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Generator_Next(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_1 = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_4 = PyList_Sort(__pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 269, __pyx_L1_error)
+  __pyx_t_4 = PyList_Sort(__pyx_t_1); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_cur_scope->__pyx_v_self->coords);
   __Pyx_DECREF(__pyx_cur_scope->__pyx_v_self->coords);
   __pyx_cur_scope->__pyx_v_self->coords = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":268
+  /* "denovonear/gencode.pyx":273
  *         self._sort()
  * 
  *     def _sort(self):             # <<<<<<<<<<<<<<
  *         self.coords = sorted(((x.chrom, x.start, x.end), symbol) for symbol, x in self.genes.items())
  * 
  */
 
@@ -6251,22 +6393,21 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("denovonear.gencode.Gencode._sort", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
-  __Pyx_XDECREF(__pyx_gb_10denovonear_7gencode_7Gencode_5_sort_2generator2);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":271
+/* "denovonear/gencode.pyx":276
  *         self.coords = sorted(((x.chrom, x.start, x.end), symbol) for symbol, x in self.genes.items())
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f'Gencode(n_genes={len(self)})'
  *     def __len__(self):
  */
 
@@ -6292,49 +6433,49 @@
   Py_ssize_t __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "denovonear/gencode.pyx":272
+  /* "denovonear/gencode.pyx":277
  * 
  *     def __repr__(self):
  *         return f'Gencode(n_genes={len(self)})'             # <<<<<<<<<<<<<<
  *     def __len__(self):
  *         return len(self.genes)
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_3 = 127;
   __Pyx_INCREF(__pyx_kp_u_Gencode_n_genes);
   __pyx_t_2 += 16;
   __Pyx_GIVEREF(__pyx_kp_u_Gencode_n_genes);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Gencode_n_genes);
-  __pyx_t_4 = PyObject_Length(((PyObject *)__pyx_v_self)); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 272, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_4, 0, ' ', 'd'); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_4 = PyObject_Length(((PyObject *)__pyx_v_self)); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_4, 0, ' ', 'd'); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_5);
   __pyx_t_5 = 0;
   __Pyx_INCREF(__pyx_kp_u__4);
   __pyx_t_2 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__4);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__4);
-  __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 272, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":271
+  /* "denovonear/gencode.pyx":276
  *         self.coords = sorted(((x.chrom, x.start, x.end), symbol) for symbol, x in self.genes.items())
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f'Gencode(n_genes={len(self)})'
  *     def __len__(self):
  */
 
@@ -6346,15 +6487,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":273
+/* "denovonear/gencode.pyx":278
  *     def __repr__(self):
  *         return f'Gencode(n_genes={len(self)})'
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.genes)
  *     def __getitem__(self, symbol):
  */
 
@@ -6377,33 +6518,33 @@
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "denovonear/gencode.pyx":274
+  /* "denovonear/gencode.pyx":279
  *         return f'Gencode(n_genes={len(self)})'
  *     def __len__(self):
  *         return len(self.genes)             # <<<<<<<<<<<<<<
  *     def __getitem__(self, symbol):
  *         return self.genes[symbol]
  */
   __pyx_t_1 = __pyx_v_self->genes;
   __Pyx_INCREF(__pyx_t_1);
   if (unlikely(__pyx_t_1 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 274, __pyx_L1_error)
+    __PYX_ERR(0, 279, __pyx_L1_error)
   }
-  __pyx_t_2 = PyDict_Size(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_2 = PyDict_Size(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 279, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":273
+  /* "denovonear/gencode.pyx":278
  *     def __repr__(self):
  *         return f'Gencode(n_genes={len(self)})'
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self.genes)
  *     def __getitem__(self, symbol):
  */
 
@@ -6413,15 +6554,15 @@
   __Pyx_AddTraceback("denovonear.gencode.Gencode.__len__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":275
+/* "denovonear/gencode.pyx":280
  *     def __len__(self):
  *         return len(self.genes)
  *     def __getitem__(self, symbol):             # <<<<<<<<<<<<<<
  *         return self.genes[symbol]
  *     def __iter__(self):
  */
 
@@ -6443,33 +6584,33 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "denovonear/gencode.pyx":276
+  /* "denovonear/gencode.pyx":281
  *         return len(self.genes)
  *     def __getitem__(self, symbol):
  *         return self.genes[symbol]             # <<<<<<<<<<<<<<
  *     def __iter__(self):
  *         for x in self.genes:
  */
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(__pyx_v_self->genes == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 276, __pyx_L1_error)
+    __PYX_ERR(0, 281, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_self->genes, __pyx_v_symbol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_GetItem(__pyx_v_self->genes, __pyx_v_symbol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":275
+  /* "denovonear/gencode.pyx":280
  *     def __len__(self):
  *         return len(self.genes)
  *     def __getitem__(self, symbol):             # <<<<<<<<<<<<<<
  *         return self.genes[symbol]
  *     def __iter__(self):
  */
 
@@ -6481,15 +6622,15 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_10denovonear_7gencode_7Gencode_12generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "denovonear/gencode.pyx":277
+/* "denovonear/gencode.pyx":282
  *     def __getitem__(self, symbol):
  *         return self.genes[symbol]
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         for x in self.genes:
  *             yield x
  */
 
@@ -6514,23 +6655,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 0);
   __pyx_cur_scope = (struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_4___iter__ *)__pyx_tp_new_10denovonear_7gencode___pyx_scope_struct_4___iter__(__pyx_ptype_10denovonear_7gencode___pyx_scope_struct_4___iter__, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_4___iter__ *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 277, __pyx_L1_error)
+    __PYX_ERR(0, 282, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10denovonear_7gencode_7Gencode_12generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter, __pyx_n_s_Gencode___iter, __pyx_n_s_denovonear_gencode); if (unlikely(!gen)) __PYX_ERR(0, 277, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10denovonear_7gencode_7Gencode_12generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_iter, __pyx_n_s_Gencode___iter, __pyx_n_s_denovonear_gencode); if (unlikely(!gen)) __PYX_ERR(0, 282, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6561,44 +6702,44 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 277, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 282, __pyx_L1_error)
 
-  /* "denovonear/gencode.pyx":278
+  /* "denovonear/gencode.pyx":283
  *         return self.genes[symbol]
  *     def __iter__(self):
  *         for x in self.genes:             # <<<<<<<<<<<<<<
  *             yield x
  * 
  */
   __pyx_t_2 = 0;
   if (unlikely(__pyx_cur_scope->__pyx_v_self->genes == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 278, __pyx_L1_error)
+    __PYX_ERR(0, 283, __pyx_L1_error)
   }
-  __pyx_t_5 = __Pyx_dict_iterator(__pyx_cur_scope->__pyx_v_self->genes, 1, ((PyObject *)NULL), (&__pyx_t_3), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 278, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_dict_iterator(__pyx_cur_scope->__pyx_v_self->genes, 1, ((PyObject *)NULL), (&__pyx_t_3), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 283, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_1);
   __pyx_t_1 = __pyx_t_5;
   __pyx_t_5 = 0;
   while (1) {
     __pyx_t_6 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_3, &__pyx_t_2, &__pyx_t_5, NULL, NULL, __pyx_t_4);
     if (unlikely(__pyx_t_6 == 0)) break;
-    if (unlikely(__pyx_t_6 == -1)) __PYX_ERR(0, 278, __pyx_L1_error)
+    if (unlikely(__pyx_t_6 == -1)) __PYX_ERR(0, 283, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_x);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_x, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "denovonear/gencode.pyx":279
+    /* "denovonear/gencode.pyx":284
  *     def __iter__(self):
  *         for x in self.genes:
  *             yield x             # <<<<<<<<<<<<<<
  * 
  *     def add_gene(self, gene):
  */
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_x);
@@ -6617,20 +6758,20 @@
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_1);
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
     __pyx_t_4 = __pyx_cur_scope->__pyx_t_3;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 279, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 284, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
-  /* "denovonear/gencode.pyx":277
+  /* "denovonear/gencode.pyx":282
  *     def __getitem__(self, symbol):
  *         return self.genes[symbol]
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         for x in self.genes:
  *             yield x
  */
 
@@ -6648,15 +6789,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":281
+/* "denovonear/gencode.pyx":286
  *             yield x
  * 
  *     def add_gene(self, gene):             # <<<<<<<<<<<<<<
  *         ''' add another gene to the Gencode object
  *         '''
  */
 
@@ -6683,84 +6824,84 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_gene", 0);
 
-  /* "denovonear/gencode.pyx":284
+  /* "denovonear/gencode.pyx":289
  *         ''' add another gene to the Gencode object
  *         '''
  *         if gene.symbol not in self.genes:             # <<<<<<<<<<<<<<
  *             self.genes[gene.symbol] = gene
  *         self._sort()
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_gene, __pyx_n_s_symbol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_gene, __pyx_n_s_symbol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (unlikely(__pyx_v_self->genes == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 284, __pyx_L1_error)
+    __PYX_ERR(0, 289, __pyx_L1_error)
   }
-  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(__pyx_t_1, __pyx_v_self->genes, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 284, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyDict_ContainsTF(__pyx_t_1, __pyx_v_self->genes, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "denovonear/gencode.pyx":285
+    /* "denovonear/gencode.pyx":290
  *         '''
  *         if gene.symbol not in self.genes:
  *             self.genes[gene.symbol] = gene             # <<<<<<<<<<<<<<
  *         self._sort()
  * 
  */
     if (unlikely(__pyx_v_self->genes == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 285, __pyx_L1_error)
+      __PYX_ERR(0, 290, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_gene, __pyx_n_s_symbol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 285, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_gene, __pyx_n_s_symbol); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(PyDict_SetItem(__pyx_v_self->genes, __pyx_t_1, __pyx_v_gene) < 0)) __PYX_ERR(0, 285, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_self->genes, __pyx_t_1, __pyx_v_gene) < 0)) __PYX_ERR(0, 290, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "denovonear/gencode.pyx":284
+    /* "denovonear/gencode.pyx":289
  *         ''' add another gene to the Gencode object
  *         '''
  *         if gene.symbol not in self.genes:             # <<<<<<<<<<<<<<
  *             self.genes[gene.symbol] = gene
  *         self._sort()
  */
   }
 
-  /* "denovonear/gencode.pyx":286
+  /* "denovonear/gencode.pyx":291
  *         if gene.symbol not in self.genes:
  *             self.genes[gene.symbol] = gene
  *         self._sort()             # <<<<<<<<<<<<<<
  * 
  *     def distance(self, gene, chrom, pos):
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_sort); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 286, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_sort); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 291, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_1 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 286, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 291, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":281
+  /* "denovonear/gencode.pyx":286
  *             yield x
  * 
  *     def add_gene(self, gene):             # <<<<<<<<<<<<<<
  *         ''' add another gene to the Gencode object
  *         '''
  */
 
@@ -6775,15 +6916,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":288
+/* "denovonear/gencode.pyx":293
  *         self._sort()
  * 
  *     def distance(self, gene, chrom, pos):             # <<<<<<<<<<<<<<
  *         ''' get distance to nearest boundary of a gene
  *         '''
  */
 
@@ -6821,40 +6962,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_gene)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_chrom)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("distance", 1, 3, 3, 1); __PYX_ERR(0, 288, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("distance", 1, 3, 3, 1); __PYX_ERR(0, 293, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pos)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("distance", 1, 3, 3, 2); __PYX_ERR(0, 288, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("distance", 1, 3, 3, 2); __PYX_ERR(0, 293, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "distance") < 0)) __PYX_ERR(0, 288, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "distance") < 0)) __PYX_ERR(0, 293, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_gene = values[0];
     __pyx_v_chrom = values[1];
     __pyx_v_pos = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("distance", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 288, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("distance", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 293, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("denovonear.gencode.Gencode.distance", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10denovonear_7gencode_7Gencode_15distance(((struct __pyx_obj_10denovonear_7gencode_Gencode *)__pyx_v_self), __pyx_v_gene, __pyx_v_chrom, __pyx_v_pos);
 
@@ -6872,118 +7013,118 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("distance", 0);
 
-  /* "denovonear/gencode.pyx":291
+  /* "denovonear/gencode.pyx":296
  *         ''' get distance to nearest boundary of a gene
  *         '''
  *         if gene.chrom != chrom:             # <<<<<<<<<<<<<<
  *             return None
  *         if gene.start <= pos <= gene.end:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_gene, __pyx_n_s_chrom); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_gene, __pyx_n_s_chrom); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 296, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_v_chrom, Py_NE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_v_chrom, Py_NE); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 296, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 296, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_3) {
 
-    /* "denovonear/gencode.pyx":292
+    /* "denovonear/gencode.pyx":297
  *         '''
  *         if gene.chrom != chrom:
  *             return None             # <<<<<<<<<<<<<<
  *         if gene.start <= pos <= gene.end:
  *             return 0
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "denovonear/gencode.pyx":291
+    /* "denovonear/gencode.pyx":296
  *         ''' get distance to nearest boundary of a gene
  *         '''
  *         if gene.chrom != chrom:             # <<<<<<<<<<<<<<
  *             return None
  *         if gene.start <= pos <= gene.end:
  */
   }
 
-  /* "denovonear/gencode.pyx":293
+  /* "denovonear/gencode.pyx":298
  *         if gene.chrom != chrom:
  *             return None
  *         if gene.start <= pos <= gene.end:             # <<<<<<<<<<<<<<
  *             return 0
  *         return min(abs(gene.start - pos), abs(gene.end - pos))
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_gene, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 293, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_gene, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_t_2, __pyx_v_pos, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 293, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_t_2, __pyx_v_pos, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
   if (__Pyx_PyObject_IsTrue(__pyx_t_1)) {
     __Pyx_DECREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_gene, __pyx_n_s_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 293, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_gene, __pyx_n_s_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 298, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyObject_RichCompare(__pyx_v_pos, __pyx_t_4, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 293, __pyx_L1_error)
+    __pyx_t_1 = PyObject_RichCompare(__pyx_v_pos, __pyx_t_4, Py_LE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 298, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 293, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 298, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_3) {
 
-    /* "denovonear/gencode.pyx":294
+    /* "denovonear/gencode.pyx":299
  *             return None
  *         if gene.start <= pos <= gene.end:
  *             return 0             # <<<<<<<<<<<<<<
  *         return min(abs(gene.start - pos), abs(gene.end - pos))
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_int_0);
     __pyx_r = __pyx_int_0;
     goto __pyx_L0;
 
-    /* "denovonear/gencode.pyx":293
+    /* "denovonear/gencode.pyx":298
  *         if gene.chrom != chrom:
  *             return None
  *         if gene.start <= pos <= gene.end:             # <<<<<<<<<<<<<<
  *             return 0
  *         return min(abs(gene.start - pos), abs(gene.end - pos))
  */
   }
 
-  /* "denovonear/gencode.pyx":295
+  /* "denovonear/gencode.pyx":300
  *         if gene.start <= pos <= gene.end:
  *             return 0
  *         return min(abs(gene.start - pos), abs(gene.end - pos))             # <<<<<<<<<<<<<<
  * 
  *     def nearest(self, chrom, pos):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_gene, __pyx_n_s_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 295, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_gene, __pyx_n_s_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyNumber_Subtract(__pyx_t_1, __pyx_v_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 295, __pyx_L1_error)
+  __pyx_t_2 = PyNumber_Subtract(__pyx_t_1, __pyx_v_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyNumber_Absolute(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 295, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyNumber_Absolute(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_gene, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 295, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_gene, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyNumber_Subtract(__pyx_t_2, __pyx_v_pos); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 295, __pyx_L1_error)
+  __pyx_t_4 = PyNumber_Subtract(__pyx_t_2, __pyx_v_pos); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyNumber_Absolute(__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 295, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyNumber_Absolute(__pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 295, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 295, __pyx_L1_error)
+  __pyx_t_5 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_5); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 300, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   if (__pyx_t_3) {
     __Pyx_INCREF(__pyx_t_1);
     __pyx_t_4 = __pyx_t_1;
   } else {
     __Pyx_INCREF(__pyx_t_2);
     __pyx_t_4 = __pyx_t_2;
@@ -6991,15 +7132,15 @@
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_INCREF(__pyx_t_4);
   __pyx_r = __pyx_t_4;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":288
+  /* "denovonear/gencode.pyx":293
  *         self._sort()
  * 
  *     def distance(self, gene, chrom, pos):             # <<<<<<<<<<<<<<
  *         ''' get distance to nearest boundary of a gene
  *         '''
  */
 
@@ -7013,15 +7154,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":297
+/* "denovonear/gencode.pyx":302
  *         return min(abs(gene.start - pos), abs(gene.end - pos))
  * 
  *     def nearest(self, chrom, pos):             # <<<<<<<<<<<<<<
  *         ''' find the nearest gene to a genomic chrom, pos coordinate
  *         '''
  */
 
@@ -7056,32 +7197,32 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_chrom)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pos)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("nearest", 1, 2, 2, 1); __PYX_ERR(0, 297, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("nearest", 1, 2, 2, 1); __PYX_ERR(0, 302, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "nearest") < 0)) __PYX_ERR(0, 297, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "nearest") < 0)) __PYX_ERR(0, 302, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
     __pyx_v_chrom = values[0];
     __pyx_v_pos = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("nearest", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 297, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("nearest", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 302, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("denovonear.gencode.Gencode.nearest", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10denovonear_7gencode_7Gencode_17nearest(((struct __pyx_obj_10denovonear_7gencode_Gencode *)__pyx_v_self), __pyx_v_chrom, __pyx_v_pos);
 
@@ -7112,79 +7253,79 @@
   int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("nearest", 0);
   __Pyx_INCREF(__pyx_v_chrom);
 
-  /* "denovonear/gencode.pyx":300
+  /* "denovonear/gencode.pyx":305
  *         ''' find the nearest gene to a genomic chrom, pos coordinate
  *         '''
  *         chrom = f'chr{chrom}' if not chrom.startswith('chr') else chrom             # <<<<<<<<<<<<<<
  *         i = bisect.bisect_left(self.coords, ((chrom, pos, pos), 'AAAA'))
  *         i = min(i, len(self.coords) - 1)  # ensure we don't go past the last gene
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_chrom, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_chrom, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 305, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_n_u_chr) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_u_chr);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 300, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 305, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 305, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (((!__pyx_t_5) != 0)) {
-    __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_chrom, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 300, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_chrom, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 305, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_n_u_chr, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 300, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_n_u_chr, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 305, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
     __Pyx_INCREF(__pyx_v_chrom);
     __pyx_t_1 = __pyx_v_chrom;
   }
   __Pyx_DECREF_SET(__pyx_v_chrom, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":301
+  /* "denovonear/gencode.pyx":306
  *         '''
  *         chrom = f'chr{chrom}' if not chrom.startswith('chr') else chrom
  *         i = bisect.bisect_left(self.coords, ((chrom, pos, pos), 'AAAA'))             # <<<<<<<<<<<<<<
  *         i = min(i, len(self.coords) - 1)  # ensure we don't go past the last gene
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_bisect); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_bisect); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_bisect_left); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_bisect_left); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_chrom);
   __Pyx_GIVEREF(__pyx_v_chrom);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_chrom);
   __Pyx_INCREF(__pyx_v_pos);
   __Pyx_GIVEREF(__pyx_v_pos);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_pos);
   __Pyx_INCREF(__pyx_v_pos);
   __Pyx_GIVEREF(__pyx_v_pos);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_v_pos);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 301, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
   __Pyx_INCREF(__pyx_n_u_AAAA);
   __Pyx_GIVEREF(__pyx_n_u_AAAA);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_n_u_AAAA);
   __pyx_t_3 = 0;
@@ -7199,323 +7340,323 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_self->coords, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_v_self->coords, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 301, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 306, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_v_self->coords);
     __Pyx_GIVEREF(__pyx_v_self->coords);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_self->coords);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 301, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_i = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":302
+  /* "denovonear/gencode.pyx":307
  *         chrom = f'chr{chrom}' if not chrom.startswith('chr') else chrom
  *         i = bisect.bisect_left(self.coords, ((chrom, pos, pos), 'AAAA'))
  *         i = min(i, len(self.coords) - 1)  # ensure we don't go past the last gene             # <<<<<<<<<<<<<<
  * 
  *         if chrom != self[self.coords[i][1]].chrom:
  */
   __pyx_t_1 = __pyx_v_self->coords;
   __Pyx_INCREF(__pyx_t_1);
   if (unlikely(__pyx_t_1 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 302, __pyx_L1_error)
+    __PYX_ERR(0, 307, __pyx_L1_error)
   }
-  __pyx_t_8 = PyList_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_t_8 = PyList_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 307, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_9 = (__pyx_t_8 - 1);
   __Pyx_INCREF(__pyx_v_i);
   __pyx_t_1 = __pyx_v_i;
-  __pyx_t_7 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_t_7 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 307, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_7, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_7, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 307, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 302, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 307, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_5) {
-    __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 302, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 307, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_2 = __pyx_t_4;
     __pyx_t_4 = 0;
   } else {
     __Pyx_INCREF(__pyx_t_1);
     __pyx_t_2 = __pyx_t_1;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = __pyx_t_2;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF_SET(__pyx_v_i, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":304
+  /* "denovonear/gencode.pyx":309
  *         i = min(i, len(self.coords) - 1)  # ensure we don't go past the last gene
  * 
  *         if chrom != self[self.coords[i][1]].chrom:             # <<<<<<<<<<<<<<
  *             # the gene coords are in a single sorted list (by chrom and pos), and
  *             # we can match to the next chrom, just step back to the previous chrom
  */
   if (unlikely(__pyx_v_self->coords == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 304, __pyx_L1_error)
+    __PYX_ERR(0, 309, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->coords, __pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->coords, __pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 309, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_chrom); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_chrom); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 309, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_chrom, __pyx_t_2, Py_NE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_chrom, __pyx_t_2, Py_NE); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 304, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 309, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_5) {
 
-    /* "denovonear/gencode.pyx":307
+    /* "denovonear/gencode.pyx":312
  *             # the gene coords are in a single sorted list (by chrom and pos), and
  *             # we can match to the next chrom, just step back to the previous chrom
  *             i -= 1             # <<<<<<<<<<<<<<
  * 
  *         if pos < self[self.coords[i][1]].start:
  */
-    __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 307, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 1, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 312, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF_SET(__pyx_v_i, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "denovonear/gencode.pyx":304
+    /* "denovonear/gencode.pyx":309
  *         i = min(i, len(self.coords) - 1)  # ensure we don't go past the last gene
  * 
  *         if chrom != self[self.coords[i][1]].chrom:             # <<<<<<<<<<<<<<
  *             # the gene coords are in a single sorted list (by chrom and pos), and
  *             # we can match to the next chrom, just step back to the previous chrom
  */
   }
 
-  /* "denovonear/gencode.pyx":309
+  /* "denovonear/gencode.pyx":314
  *             i -= 1
  * 
  *         if pos < self[self.coords[i][1]].start:             # <<<<<<<<<<<<<<
  *             left = self[self.coords[max(i - 1, 0)][1]]
  *             right = self[self.coords[i][1]]
  */
   if (unlikely(__pyx_v_self->coords == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 309, __pyx_L1_error)
+    __PYX_ERR(0, 314, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->coords, __pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->coords, __pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_pos, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_pos, __pyx_t_2, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_5) {
 
-    /* "denovonear/gencode.pyx":310
+    /* "denovonear/gencode.pyx":315
  * 
  *         if pos < self[self.coords[i][1]].start:
  *             left = self[self.coords[max(i - 1, 0)][1]]             # <<<<<<<<<<<<<<
  *             right = self[self.coords[i][1]]
  *         else:
  */
     if (unlikely(__pyx_v_self->coords == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 310, __pyx_L1_error)
+      __PYX_ERR(0, 315, __pyx_L1_error)
     }
     __pyx_t_10 = 0;
-    __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_SubtractObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 315, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 310, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_t_10); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 315, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = PyObject_RichCompare(__pyx_t_4, __pyx_t_1, Py_GT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 310, __pyx_L1_error)
+    __pyx_t_7 = PyObject_RichCompare(__pyx_t_4, __pyx_t_1, Py_GT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 315, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 310, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 315, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (__pyx_t_5) {
-      __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 310, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyInt_From_long(__pyx_t_10); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 315, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_2 = __pyx_t_7;
       __pyx_t_7 = 0;
     } else {
       __Pyx_INCREF(__pyx_t_1);
       __pyx_t_2 = __pyx_t_1;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->coords, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->coords, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 315, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 310, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 315, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 310, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 315, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_left = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "denovonear/gencode.pyx":311
+    /* "denovonear/gencode.pyx":316
  *         if pos < self[self.coords[i][1]].start:
  *             left = self[self.coords[max(i - 1, 0)][1]]
  *             right = self[self.coords[i][1]]             # <<<<<<<<<<<<<<
  *         else:
  *             left = self[self.coords[i][1]]
  */
     if (unlikely(__pyx_v_self->coords == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 311, __pyx_L1_error)
+      __PYX_ERR(0, 316, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->coords, __pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 311, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->coords, __pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 316, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 311, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 316, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 311, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 316, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_right = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "denovonear/gencode.pyx":309
+    /* "denovonear/gencode.pyx":314
  *             i -= 1
  * 
  *         if pos < self[self.coords[i][1]].start:             # <<<<<<<<<<<<<<
  *             left = self[self.coords[max(i - 1, 0)][1]]
  *             right = self[self.coords[i][1]]
  */
     goto __pyx_L4;
   }
 
-  /* "denovonear/gencode.pyx":313
+  /* "denovonear/gencode.pyx":318
  *             right = self[self.coords[i][1]]
  *         else:
  *             left = self[self.coords[i][1]]             # <<<<<<<<<<<<<<
  *             right = self[self.coords[min(i + 1, len(self.coords) - 1)][1]]
  * 
  */
   /*else*/ {
     if (unlikely(__pyx_v_self->coords == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 313, __pyx_L1_error)
+      __PYX_ERR(0, 318, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->coords, __pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->coords, __pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 313, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 313, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_left = __pyx_t_1;
     __pyx_t_1 = 0;
 
-    /* "denovonear/gencode.pyx":314
+    /* "denovonear/gencode.pyx":319
  *         else:
  *             left = self[self.coords[i][1]]
  *             right = self[self.coords[min(i + 1, len(self.coords) - 1)][1]]             # <<<<<<<<<<<<<<
  * 
  *         left_delta = self.distance(left, chrom, pos)
  */
     if (unlikely(__pyx_v_self->coords == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 314, __pyx_L1_error)
+      __PYX_ERR(0, 319, __pyx_L1_error)
     }
     __pyx_t_1 = __pyx_v_self->coords;
     __Pyx_INCREF(__pyx_t_1);
     if (unlikely(__pyx_t_1 == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-      __PYX_ERR(0, 314, __pyx_L1_error)
+      __PYX_ERR(0, 319, __pyx_L1_error)
     }
-    __pyx_t_9 = PyList_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 314, __pyx_L1_error)
+    __pyx_t_9 = PyList_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_8 = (__pyx_t_9 - 1);
-    __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 314, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_AddObjC(__pyx_v_i, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_7 = PyInt_FromSsize_t(__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 314, __pyx_L1_error)
+    __pyx_t_7 = PyInt_FromSsize_t(__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_4 = PyObject_RichCompare(__pyx_t_7, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 314, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_t_7, __pyx_t_1, Py_LT); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 314, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__pyx_t_5) {
-      __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 314, __pyx_L1_error)
+      __pyx_t_4 = PyInt_FromSsize_t(__pyx_t_8); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 319, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_t_2 = __pyx_t_4;
       __pyx_t_4 = 0;
     } else {
       __Pyx_INCREF(__pyx_t_1);
       __pyx_t_2 = __pyx_t_1;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->coords, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 314, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(__pyx_v_self->coords, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 314, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 314, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 319, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_v_right = __pyx_t_1;
     __pyx_t_1 = 0;
   }
   __pyx_L4:;
 
-  /* "denovonear/gencode.pyx":316
+  /* "denovonear/gencode.pyx":321
  *             right = self[self.coords[min(i + 1, len(self.coords) - 1)][1]]
  * 
  *         left_delta = self.distance(left, chrom, pos)             # <<<<<<<<<<<<<<
  *         right_delta = self.distance(right, chrom, pos)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 316, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -7524,58 +7665,58 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_v_left, __pyx_v_chrom, __pyx_v_pos};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 316, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 321, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_4, __pyx_v_left, __pyx_v_chrom, __pyx_v_pos};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 316, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 321, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 316, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 321, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_INCREF(__pyx_v_left);
     __Pyx_GIVEREF(__pyx_v_left);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_left);
     __Pyx_INCREF(__pyx_v_chrom);
     __Pyx_GIVEREF(__pyx_v_chrom);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_v_chrom);
     __Pyx_INCREF(__pyx_v_pos);
     __Pyx_GIVEREF(__pyx_v_pos);
     PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_6, __pyx_v_pos);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 316, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 321, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_left_delta = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":317
+  /* "denovonear/gencode.pyx":322
  * 
  *         left_delta = self.distance(left, chrom, pos)
  *         right_delta = self.distance(right, chrom, pos)             # <<<<<<<<<<<<<<
  * 
  *         if right_delta is None and left_delta is None:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 317, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_distance); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_7 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -7584,51 +7725,51 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_v_right, __pyx_v_chrom, __pyx_v_pos};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_7, __pyx_v_right, __pyx_v_chrom, __pyx_v_pos};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 3+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_1);
   } else
   #endif
   {
-    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 317, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3+__pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 322, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     if (__pyx_t_7) {
       __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_INCREF(__pyx_v_right);
     __Pyx_GIVEREF(__pyx_v_right);
     PyTuple_SET_ITEM(__pyx_t_4, 0+__pyx_t_6, __pyx_v_right);
     __Pyx_INCREF(__pyx_v_chrom);
     __Pyx_GIVEREF(__pyx_v_chrom);
     PyTuple_SET_ITEM(__pyx_t_4, 1+__pyx_t_6, __pyx_v_chrom);
     __Pyx_INCREF(__pyx_v_pos);
     __Pyx_GIVEREF(__pyx_v_pos);
     PyTuple_SET_ITEM(__pyx_t_4, 2+__pyx_t_6, __pyx_v_pos);
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_4, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 322, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_right_delta = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":319
+  /* "denovonear/gencode.pyx":324
  *         right_delta = self.distance(right, chrom, pos)
  * 
  *         if right_delta is None and left_delta is None:             # <<<<<<<<<<<<<<
  *             raise ValueError(f"can't find any genes on {chrom}")
  *         if right_delta is None:
  */
   __pyx_t_11 = (__pyx_v_right_delta == Py_None);
@@ -7640,154 +7781,154 @@
   }
   __pyx_t_12 = (__pyx_v_left_delta == Py_None);
   __pyx_t_11 = (__pyx_t_12 != 0);
   __pyx_t_5 = __pyx_t_11;
   __pyx_L6_bool_binop_done:;
   if (unlikely(__pyx_t_5)) {
 
-    /* "denovonear/gencode.pyx":320
+    /* "denovonear/gencode.pyx":325
  * 
  *         if right_delta is None and left_delta is None:
  *             raise ValueError(f"can't find any genes on {chrom}")             # <<<<<<<<<<<<<<
  *         if right_delta is None:
  *             return left
  */
-    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_chrom, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 320, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_FormatSimple(__pyx_v_chrom, __pyx_empty_unicode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 325, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_can_t_find_any_genes_on, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 320, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyUnicode_Concat(__pyx_kp_u_can_t_find_any_genes_on, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 325, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 320, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 325, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 320, __pyx_L1_error)
+    __PYX_ERR(0, 325, __pyx_L1_error)
 
-    /* "denovonear/gencode.pyx":319
+    /* "denovonear/gencode.pyx":324
  *         right_delta = self.distance(right, chrom, pos)
  * 
  *         if right_delta is None and left_delta is None:             # <<<<<<<<<<<<<<
  *             raise ValueError(f"can't find any genes on {chrom}")
  *         if right_delta is None:
  */
   }
 
-  /* "denovonear/gencode.pyx":321
+  /* "denovonear/gencode.pyx":326
  *         if right_delta is None and left_delta is None:
  *             raise ValueError(f"can't find any genes on {chrom}")
  *         if right_delta is None:             # <<<<<<<<<<<<<<
  *             return left
  *         elif left_delta is None:
  */
   __pyx_t_5 = (__pyx_v_right_delta == Py_None);
   __pyx_t_11 = (__pyx_t_5 != 0);
   if (__pyx_t_11) {
 
-    /* "denovonear/gencode.pyx":322
+    /* "denovonear/gencode.pyx":327
  *             raise ValueError(f"can't find any genes on {chrom}")
  *         if right_delta is None:
  *             return left             # <<<<<<<<<<<<<<
  *         elif left_delta is None:
  *             return right
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_left);
     __pyx_r = __pyx_v_left;
     goto __pyx_L0;
 
-    /* "denovonear/gencode.pyx":321
+    /* "denovonear/gencode.pyx":326
  *         if right_delta is None and left_delta is None:
  *             raise ValueError(f"can't find any genes on {chrom}")
  *         if right_delta is None:             # <<<<<<<<<<<<<<
  *             return left
  *         elif left_delta is None:
  */
   }
 
-  /* "denovonear/gencode.pyx":323
+  /* "denovonear/gencode.pyx":328
  *         if right_delta is None:
  *             return left
  *         elif left_delta is None:             # <<<<<<<<<<<<<<
  *             return right
  *         elif left_delta < right_delta:
  */
   __pyx_t_11 = (__pyx_v_left_delta == Py_None);
   __pyx_t_5 = (__pyx_t_11 != 0);
   if (__pyx_t_5) {
 
-    /* "denovonear/gencode.pyx":324
+    /* "denovonear/gencode.pyx":329
  *             return left
  *         elif left_delta is None:
  *             return right             # <<<<<<<<<<<<<<
  *         elif left_delta < right_delta:
  *             return left
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_right);
     __pyx_r = __pyx_v_right;
     goto __pyx_L0;
 
-    /* "denovonear/gencode.pyx":323
+    /* "denovonear/gencode.pyx":328
  *         if right_delta is None:
  *             return left
  *         elif left_delta is None:             # <<<<<<<<<<<<<<
  *             return right
  *         elif left_delta < right_delta:
  */
   }
 
-  /* "denovonear/gencode.pyx":325
+  /* "denovonear/gencode.pyx":330
  *         elif left_delta is None:
  *             return right
  *         elif left_delta < right_delta:             # <<<<<<<<<<<<<<
  *             return left
  *         else:
  */
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_left_delta, __pyx_v_right_delta, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 325, __pyx_L1_error)
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 325, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_left_delta, __pyx_v_right_delta, Py_LT); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 330, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_5) {
 
-    /* "denovonear/gencode.pyx":326
+    /* "denovonear/gencode.pyx":331
  *             return right
  *         elif left_delta < right_delta:
  *             return left             # <<<<<<<<<<<<<<
  *         else:
  *             return right
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_left);
     __pyx_r = __pyx_v_left;
     goto __pyx_L0;
 
-    /* "denovonear/gencode.pyx":325
+    /* "denovonear/gencode.pyx":330
  *         elif left_delta is None:
  *             return right
  *         elif left_delta < right_delta:             # <<<<<<<<<<<<<<
  *             return left
  *         else:
  */
   }
 
-  /* "denovonear/gencode.pyx":328
+  /* "denovonear/gencode.pyx":333
  *             return left
  *         else:
  *             return right             # <<<<<<<<<<<<<<
  * 
  *     def in_region(self, chrom, start, end):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_right);
     __pyx_r = __pyx_v_right;
     goto __pyx_L0;
   }
 
-  /* "denovonear/gencode.pyx":297
+  /* "denovonear/gencode.pyx":302
  *         return min(abs(gene.start - pos), abs(gene.end - pos))
  * 
  *     def nearest(self, chrom, pos):             # <<<<<<<<<<<<<<
  *         ''' find the nearest gene to a genomic chrom, pos coordinate
  *         '''
  */
 
@@ -7808,15 +7949,15 @@
   __Pyx_XDECREF(__pyx_v_right_delta);
   __Pyx_XDECREF(__pyx_v_chrom);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":330
+/* "denovonear/gencode.pyx":335
  *             return right
  * 
  *     def in_region(self, chrom, start, end):             # <<<<<<<<<<<<<<
  *         ''' find genes within a genomic region
  * 
  */
 
@@ -7854,54 +7995,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_chrom)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("in_region", 1, 3, 3, 1); __PYX_ERR(0, 330, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("in_region", 1, 3, 3, 1); __PYX_ERR(0, 335, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("in_region", 1, 3, 3, 2); __PYX_ERR(0, 330, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("in_region", 1, 3, 3, 2); __PYX_ERR(0, 335, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "in_region") < 0)) __PYX_ERR(0, 330, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "in_region") < 0)) __PYX_ERR(0, 335, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_chrom = values[0];
     __pyx_v_start = values[1];
     __pyx_v_end = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("in_region", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 330, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("in_region", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 335, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("denovonear.gencode.Gencode.in_region", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_10denovonear_7gencode_7Gencode_19in_region(((struct __pyx_obj_10denovonear_7gencode_Gencode *)__pyx_v_self), __pyx_v_chrom, __pyx_v_start, __pyx_v_end);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_10denovonear_7gencode_7Gencode_9in_region_2generator3(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "denovonear/gencode.pyx":345
+/* "denovonear/gencode.pyx":350
  *         right = bisect.bisect_left(self.coords, ((chrom, end, end), 'AAAA'))
  * 
  *         genes = (self.genes[self.coords[i][1]] for i in range(left, right))             # <<<<<<<<<<<<<<
  *         return [x for x in genes if x.chrom == chrom]
  * 
  */
 
@@ -7913,23 +8054,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_6_genexpr *)__pyx_tp_new_10denovonear_7gencode___pyx_scope_struct_6_genexpr(__pyx_ptype_10denovonear_7gencode___pyx_scope_struct_6_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_6_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 345, __pyx_L1_error)
+    __PYX_ERR(0, 350, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_5_in_region *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10denovonear_7gencode_7Gencode_9in_region_2generator3, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_in_region_locals_genexpr, __pyx_n_s_denovonear_gencode); if (unlikely(!gen)) __PYX_ERR(0, 345, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_10denovonear_7gencode_7Gencode_9in_region_2generator3, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_in_region_locals_genexpr, __pyx_n_s_denovonear_gencode); if (unlikely(!gen)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -7959,88 +8100,88 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 345, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_left)) { __Pyx_RaiseClosureNameError("left"); __PYX_ERR(0, 345, __pyx_L1_error) }
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_right)) { __Pyx_RaiseClosureNameError("right"); __PYX_ERR(0, 345, __pyx_L1_error) }
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 345, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 350, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_left)) { __Pyx_RaiseClosureNameError("left"); __PYX_ERR(0, 350, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_right)) { __Pyx_RaiseClosureNameError("right"); __PYX_ERR(0, 350, __pyx_L1_error) }
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_left);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_left);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_cur_scope->__pyx_outer_scope->__pyx_v_left);
   __Pyx_INCREF(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_right);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_right);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_cur_scope->__pyx_outer_scope->__pyx_v_right);
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_range, __pyx_t_1, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
     __pyx_t_1 = __pyx_t_2; __Pyx_INCREF(__pyx_t_1); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 345, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 345, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 350, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 345, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 350, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 345, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_3); __Pyx_INCREF(__pyx_t_2); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(0, 350, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_4(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 345, __pyx_L1_error)
+          else __PYX_ERR(0, 350, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_i);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_i, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_2);
     __pyx_t_2 = 0;
-    if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 345, __pyx_L1_error) }
+    if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 350, __pyx_L1_error) }
     if (unlikely(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self->genes == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 345, __pyx_L1_error)
+      __PYX_ERR(0, 350, __pyx_L1_error)
     }
-    if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 345, __pyx_L1_error) }
+    if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self)) { __Pyx_RaiseClosureNameError("self"); __PYX_ERR(0, 350, __pyx_L1_error) }
     if (unlikely(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self->coords == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 345, __pyx_L1_error)
+      __PYX_ERR(0, 350, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self->coords, __pyx_cur_scope->__pyx_v_i); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self->coords, __pyx_cur_scope->__pyx_v_i); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 345, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt(__pyx_t_2, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self->genes, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 345, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_self->genes, __pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     __Pyx_XGIVEREF(__pyx_t_1);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_3;
@@ -8053,15 +8194,15 @@
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_1);
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_4 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 345, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 350, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -8077,26 +8218,25 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":330
+/* "denovonear/gencode.pyx":335
  *             return right
  * 
  *     def in_region(self, chrom, start, end):             # <<<<<<<<<<<<<<
  *         ''' find genes within a genomic region
  * 
  */
 
 static PyObject *__pyx_pf_10denovonear_7gencode_7Gencode_19in_region(struct __pyx_obj_10denovonear_7gencode_Gencode *__pyx_v_self, PyObject *__pyx_v_chrom, PyObject *__pyx_v_start, PyObject *__pyx_v_end) {
   struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_5_in_region *__pyx_cur_scope;
   PyObject *__pyx_v_genes = NULL;
-  PyObject *__pyx_gb_10denovonear_7gencode_7Gencode_9in_region_2generator3 = 0;
   PyObject *__pyx_8genexpr6__pyx_v_x = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -8109,88 +8249,88 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("in_region", 0);
   __pyx_cur_scope = (struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_5_in_region *)__pyx_tp_new_10denovonear_7gencode___pyx_scope_struct_5_in_region(__pyx_ptype_10denovonear_7gencode___pyx_scope_struct_5_in_region, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_10denovonear_7gencode___pyx_scope_struct_5_in_region *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 330, __pyx_L1_error)
+    __PYX_ERR(0, 335, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_v_self = __pyx_v_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_v_self);
   __Pyx_INCREF(__pyx_v_chrom);
 
-  /* "denovonear/gencode.pyx":341
+  /* "denovonear/gencode.pyx":346
  *             list of Gene objects
  *         '''
  *         chrom = f'chr{chrom}' if not chrom.startswith('chr') else chrom             # <<<<<<<<<<<<<<
  *         left = bisect.bisect_left(self.coords, ((chrom, start, start), 'AAAA'))
  *         right = bisect.bisect_left(self.coords, ((chrom, end, end), 'AAAA'))
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_chrom, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_chrom, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_n_u_chr) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_u_chr);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (((!__pyx_t_5) != 0)) {
-    __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_chrom, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_FormatSimple(__pyx_v_chrom, __pyx_empty_unicode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 346, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_n_u_chr, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 341, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyUnicode_Concat(__pyx_n_u_chr, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 346, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
     __Pyx_INCREF(__pyx_v_chrom);
     __pyx_t_1 = __pyx_v_chrom;
   }
   __Pyx_DECREF_SET(__pyx_v_chrom, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":342
+  /* "denovonear/gencode.pyx":347
  *         '''
  *         chrom = f'chr{chrom}' if not chrom.startswith('chr') else chrom
  *         left = bisect.bisect_left(self.coords, ((chrom, start, start), 'AAAA'))             # <<<<<<<<<<<<<<
  *         right = bisect.bisect_left(self.coords, ((chrom, end, end), 'AAAA'))
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_bisect); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 342, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_bisect); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_bisect_left); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 342, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_bisect_left); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 342, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_chrom);
   __Pyx_GIVEREF(__pyx_v_chrom);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_chrom);
   __Pyx_INCREF(__pyx_v_start);
   __Pyx_GIVEREF(__pyx_v_start);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_start);
   __Pyx_INCREF(__pyx_v_start);
   __Pyx_GIVEREF(__pyx_v_start);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_v_start);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 342, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 347, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3);
   __Pyx_INCREF(__pyx_n_u_AAAA);
   __Pyx_GIVEREF(__pyx_n_u_AAAA);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_n_u_AAAA);
   __pyx_t_3 = 0;
@@ -8205,74 +8345,74 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_cur_scope->__pyx_v_self->coords, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 342, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 347, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[3] = {__pyx_t_3, __pyx_cur_scope->__pyx_v_self->coords, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 342, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 347, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 342, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 347, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_3) {
       __Pyx_GIVEREF(__pyx_t_3); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_3); __pyx_t_3 = NULL;
     }
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self->coords);
     __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_self->coords);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_cur_scope->__pyx_v_self->coords);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 342, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 347, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_left = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":343
+  /* "denovonear/gencode.pyx":348
  *         chrom = f'chr{chrom}' if not chrom.startswith('chr') else chrom
  *         left = bisect.bisect_left(self.coords, ((chrom, start, start), 'AAAA'))
  *         right = bisect.bisect_left(self.coords, ((chrom, end, end), 'AAAA'))             # <<<<<<<<<<<<<<
  * 
  *         genes = (self.genes[self.coords[i][1]] for i in range(left, right))
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_bisect); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 343, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_bisect); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_bisect_left); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 343, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_bisect_left); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 348, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 343, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 348, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_chrom);
   __Pyx_GIVEREF(__pyx_v_chrom);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_chrom);
   __Pyx_INCREF(__pyx_v_end);
   __Pyx_GIVEREF(__pyx_v_end);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_end);
   __Pyx_INCREF(__pyx_v_end);
   __Pyx_GIVEREF(__pyx_v_end);
   PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_v_end);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 343, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 348, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __Pyx_INCREF(__pyx_n_u_AAAA);
   __Pyx_GIVEREF(__pyx_n_u_AAAA);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_n_u_AAAA);
   __pyx_t_2 = 0;
@@ -8287,137 +8427,137 @@
       __Pyx_DECREF_SET(__pyx_t_7, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_7)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_cur_scope->__pyx_v_self->coords, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 343, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_cur_scope->__pyx_v_self->coords, __pyx_t_4};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 343, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   } else
   #endif
   {
-    __pyx_t_3 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 343, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
     __Pyx_INCREF(__pyx_cur_scope->__pyx_v_self->coords);
     __Pyx_GIVEREF(__pyx_cur_scope->__pyx_v_self->coords);
     PyTuple_SET_ITEM(__pyx_t_3, 0+__pyx_t_6, __pyx_cur_scope->__pyx_v_self->coords);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_3, 1+__pyx_t_6, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 343, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 348, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_right = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":345
+  /* "denovonear/gencode.pyx":350
  *         right = bisect.bisect_left(self.coords, ((chrom, end, end), 'AAAA'))
  * 
  *         genes = (self.genes[self.coords[i][1]] for i in range(left, right))             # <<<<<<<<<<<<<<
  *         return [x for x in genes if x.chrom == chrom]
  * 
  */
-  __pyx_t_1 = __pyx_pf_10denovonear_7gencode_7Gencode_9in_region_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 345, __pyx_L1_error)
+  __pyx_t_1 = __pyx_pf_10denovonear_7gencode_7Gencode_9in_region_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_genes = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":346
+  /* "denovonear/gencode.pyx":351
  * 
  *         genes = (self.genes[self.coords[i][1]] for i in range(left, right))
  *         return [x for x in genes if x.chrom == chrom]             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 346, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 351, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (likely(PyList_CheckExact(__pyx_v_genes)) || PyTuple_CheckExact(__pyx_v_genes)) {
       __pyx_t_7 = __pyx_v_genes; __Pyx_INCREF(__pyx_t_7); __pyx_t_8 = 0;
       __pyx_t_9 = NULL;
     } else {
-      __pyx_t_8 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_v_genes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 346, __pyx_L5_error)
+      __pyx_t_8 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_v_genes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 351, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
-      __pyx_t_9 = Py_TYPE(__pyx_t_7)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 346, __pyx_L5_error)
+      __pyx_t_9 = Py_TYPE(__pyx_t_7)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 351, __pyx_L5_error)
     }
     for (;;) {
       if (likely(!__pyx_t_9)) {
         if (likely(PyList_CheckExact(__pyx_t_7))) {
           if (__pyx_t_8 >= PyList_GET_SIZE(__pyx_t_7)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_8); __Pyx_INCREF(__pyx_t_3); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 346, __pyx_L5_error)
+          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_8); __Pyx_INCREF(__pyx_t_3); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 351, __pyx_L5_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_7, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 346, __pyx_L5_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_7, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 351, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         } else {
           if (__pyx_t_8 >= PyTuple_GET_SIZE(__pyx_t_7)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_8); __Pyx_INCREF(__pyx_t_3); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 346, __pyx_L5_error)
+          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_8); __Pyx_INCREF(__pyx_t_3); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 351, __pyx_L5_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_7, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 346, __pyx_L5_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_7, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 351, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         }
       } else {
         __pyx_t_3 = __pyx_t_9(__pyx_t_7);
         if (unlikely(!__pyx_t_3)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 346, __pyx_L5_error)
+            else __PYX_ERR(0, 351, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_3);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr6__pyx_v_x, __pyx_t_3);
       __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr6__pyx_v_x, __pyx_n_s_chrom); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 346, __pyx_L5_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr6__pyx_v_x, __pyx_n_s_chrom); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 351, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_chrom, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 346, __pyx_L5_error)
+      __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_chrom, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 351, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 346, __pyx_L5_error)
+      __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 351, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       if (__pyx_t_5) {
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_8genexpr6__pyx_v_x))) __PYX_ERR(0, 346, __pyx_L5_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_8genexpr6__pyx_v_x))) __PYX_ERR(0, 351, __pyx_L5_error)
       }
     }
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_x); __pyx_8genexpr6__pyx_v_x = 0;
     goto __pyx_L9_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_x); __pyx_8genexpr6__pyx_v_x = 0;
     goto __pyx_L1_error;
     __pyx_L9_exit_scope:;
   } /* exit inner scope */
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "denovonear/gencode.pyx":330
+  /* "denovonear/gencode.pyx":335
  *             return right
  * 
  *     def in_region(self, chrom, start, end):             # <<<<<<<<<<<<<<
  *         ''' find genes within a genomic region
  * 
  */
 
@@ -8428,24 +8568,23 @@
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_AddTraceback("denovonear.gencode.Gencode.in_region", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_genes);
-  __Pyx_XDECREF(__pyx_gb_10denovonear_7gencode_7Gencode_9in_region_2generator3);
   __Pyx_XDECREF(__pyx_8genexpr6__pyx_v_x);
   __Pyx_XDECREF(__pyx_v_chrom);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "denovonear/gencode.pyx":348
+/* "denovonear/gencode.pyx":353
  *         return [x for x in genes if x.chrom == chrom]
  * 
  *     def __exit__(self):             # <<<<<<<<<<<<<<
  *         ''' cleanup at exit
  *         '''
  */
 
@@ -8470,50 +8609,50 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "denovonear/gencode.pyx":352
+  /* "denovonear/gencode.pyx":357
  *         '''
  *         global __genome_
  *         __genome_.close()             # <<<<<<<<<<<<<<
  *         __genome_ = None
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_genome); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 352, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_genome); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_close); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 352, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_close); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_2) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 352, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 357, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "denovonear/gencode.pyx":353
+  /* "denovonear/gencode.pyx":358
  *         global __genome_
  *         __genome_.close()
  *         __genome_ = None             # <<<<<<<<<<<<<<
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_genome, Py_None) < 0) __PYX_ERR(0, 353, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_genome, Py_None) < 0) __PYX_ERR(0, 358, __pyx_L1_error)
 
-  /* "denovonear/gencode.pyx":348
+  /* "denovonear/gencode.pyx":353
  *         return [x for x in genes if x.chrom == chrom]
  * 
  *     def __exit__(self):             # <<<<<<<<<<<<<<
  *         ''' cleanup at exit
  *         '''
  */
 
@@ -10360,14 +10499,15 @@
   {&__pyx_n_s_pos, __pyx_k_pos, sizeof(__pyx_k_pos), 0, 0, 1, 1},
   {&__pyx_n_s_pyfaidx, __pyx_k_pyfaidx, sizeof(__pyx_k_pyfaidx), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
+  {&__pyx_n_s_reverse_complement, __pyx_k_reverse_complement, sizeof(__pyx_k_reverse_complement), 0, 0, 1, 1},
   {&__pyx_n_s_send, __pyx_k_send, sizeof(__pyx_k_send), 0, 0, 1, 1},
   {&__pyx_n_s_seq, __pyx_k_seq, sizeof(__pyx_k_seq), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_sort, __pyx_k_sort, sizeof(__pyx_k_sort), 0, 0, 1, 1},
   {&__pyx_n_s_sort_locals_genexpr, __pyx_k_sort_locals_genexpr, sizeof(__pyx_k_sort_locals_genexpr), 0, 0, 1, 1},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
@@ -10381,35 +10521,35 @@
   {&__pyx_n_s_tx_id, __pyx_k_tx_id, sizeof(__pyx_k_tx_id), 0, 0, 1, 1},
   {&__pyx_n_s_upper, __pyx_k_upper, sizeof(__pyx_k_upper), 0, 0, 1, 1},
   {&__pyx_n_u_utf8, __pyx_k_utf8, sizeof(__pyx_k_utf8), 0, 1, 0, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_chr = __Pyx_GetBuiltinName(__pyx_n_s_chr); if (!__pyx_builtin_chr) __PYX_ERR(0, 64, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 159, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 223, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 162, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 228, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 320, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 325, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "denovonear/gencode.pyx":159
+  /* "denovonear/gencode.pyx":162
  *         if self._transcripts.size() > 0:
  *             return chr(self._transcripts[0].get_strand())
  *         raise IndexError('no transcripts in gene yet')             # <<<<<<<<<<<<<<
  * 
  *     cdef _convert_exons(self, vector[Region] exons):
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_no_transcripts_in_gene_yet); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 159, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_no_transcripts_in_gene_yet); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -10517,73 +10657,73 @@
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10denovonear_7gencode_Gene.tp_dictoffset && __pyx_type_10denovonear_7gencode_Gene.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10denovonear_7gencode_Gene.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   if (__Pyx_SetVtable(__pyx_type_10denovonear_7gencode_Gene.tp_dict, __pyx_vtabptr_10denovonear_7gencode_Gene) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Gene_2, (PyObject *)&__pyx_type_10denovonear_7gencode_Gene) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10denovonear_7gencode_Gene) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __pyx_ptype_10denovonear_7gencode_Gene = &__pyx_type_10denovonear_7gencode_Gene;
-  if (PyType_Ready(&__pyx_type_10denovonear_7gencode_Gencode) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10denovonear_7gencode_Gencode) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10denovonear_7gencode_Gencode.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10denovonear_7gencode_Gencode.tp_dictoffset && __pyx_type_10denovonear_7gencode_Gencode.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10denovonear_7gencode_Gencode.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Gencode, (PyObject *)&__pyx_type_10denovonear_7gencode_Gencode) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10denovonear_7gencode_Gencode) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Gencode, (PyObject *)&__pyx_type_10denovonear_7gencode_Gencode) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_10denovonear_7gencode_Gencode) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
   __pyx_ptype_10denovonear_7gencode_Gencode = &__pyx_type_10denovonear_7gencode_Gencode;
-  if (PyType_Ready(&__pyx_type_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds) < 0) __PYX_ERR(0, 233, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds.tp_dictoffset && __pyx_type_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds = &__pyx_type_10denovonear_7gencode___pyx_scope_struct__in_any_tx_cds;
-  if (PyType_Ready(&__pyx_type_10denovonear_7gencode___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 236, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10denovonear_7gencode___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10denovonear_7gencode___pyx_scope_struct_1_genexpr.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10denovonear_7gencode___pyx_scope_struct_1_genexpr.tp_dictoffset && __pyx_type_10denovonear_7gencode___pyx_scope_struct_1_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10denovonear_7gencode___pyx_scope_struct_1_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10denovonear_7gencode___pyx_scope_struct_1_genexpr = &__pyx_type_10denovonear_7gencode___pyx_scope_struct_1_genexpr;
-  if (PyType_Ready(&__pyx_type_10denovonear_7gencode___pyx_scope_struct_2__sort) < 0) __PYX_ERR(0, 268, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10denovonear_7gencode___pyx_scope_struct_2__sort) < 0) __PYX_ERR(0, 273, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10denovonear_7gencode___pyx_scope_struct_2__sort.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10denovonear_7gencode___pyx_scope_struct_2__sort.tp_dictoffset && __pyx_type_10denovonear_7gencode___pyx_scope_struct_2__sort.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10denovonear_7gencode___pyx_scope_struct_2__sort.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10denovonear_7gencode___pyx_scope_struct_2__sort = &__pyx_type_10denovonear_7gencode___pyx_scope_struct_2__sort;
-  if (PyType_Ready(&__pyx_type_10denovonear_7gencode___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 269, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10denovonear_7gencode___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 274, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10denovonear_7gencode___pyx_scope_struct_3_genexpr.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10denovonear_7gencode___pyx_scope_struct_3_genexpr.tp_dictoffset && __pyx_type_10denovonear_7gencode___pyx_scope_struct_3_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10denovonear_7gencode___pyx_scope_struct_3_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10denovonear_7gencode___pyx_scope_struct_3_genexpr = &__pyx_type_10denovonear_7gencode___pyx_scope_struct_3_genexpr;
-  if (PyType_Ready(&__pyx_type_10denovonear_7gencode___pyx_scope_struct_4___iter__) < 0) __PYX_ERR(0, 277, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10denovonear_7gencode___pyx_scope_struct_4___iter__) < 0) __PYX_ERR(0, 282, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10denovonear_7gencode___pyx_scope_struct_4___iter__.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10denovonear_7gencode___pyx_scope_struct_4___iter__.tp_dictoffset && __pyx_type_10denovonear_7gencode___pyx_scope_struct_4___iter__.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10denovonear_7gencode___pyx_scope_struct_4___iter__.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10denovonear_7gencode___pyx_scope_struct_4___iter__ = &__pyx_type_10denovonear_7gencode___pyx_scope_struct_4___iter__;
-  if (PyType_Ready(&__pyx_type_10denovonear_7gencode___pyx_scope_struct_5_in_region) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10denovonear_7gencode___pyx_scope_struct_5_in_region) < 0) __PYX_ERR(0, 335, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10denovonear_7gencode___pyx_scope_struct_5_in_region.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10denovonear_7gencode___pyx_scope_struct_5_in_region.tp_dictoffset && __pyx_type_10denovonear_7gencode___pyx_scope_struct_5_in_region.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10denovonear_7gencode___pyx_scope_struct_5_in_region.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10denovonear_7gencode___pyx_scope_struct_5_in_region = &__pyx_type_10denovonear_7gencode___pyx_scope_struct_5_in_region;
-  if (PyType_Ready(&__pyx_type_10denovonear_7gencode___pyx_scope_struct_6_genexpr) < 0) __PYX_ERR(0, 345, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_10denovonear_7gencode___pyx_scope_struct_6_genexpr) < 0) __PYX_ERR(0, 350, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_10denovonear_7gencode___pyx_scope_struct_6_genexpr.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_10denovonear_7gencode___pyx_scope_struct_6_genexpr.tp_dictoffset && __pyx_type_10denovonear_7gencode___pyx_scope_struct_6_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_10denovonear_7gencode___pyx_scope_struct_6_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_10denovonear_7gencode___pyx_scope_struct_6_genexpr = &__pyx_type_10denovonear_7gencode___pyx_scope_struct_6_genexpr;
@@ -10773,17 +10913,19 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #ifdef WITH_THREAD /* Python build with threading support? */
   PyEval_InitThreads();
   #endif
+  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("gencode", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -11138,15 +11280,15 @@
 #endif
 #endif
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
+    ternaryfunc call = func->ob_type->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -11225,15 +11367,15 @@
         return __Pyx_PyFunction_FastCall(func, &arg, 1);
     }
 #endif
     if (likely(PyCFunction_Check(func))) {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
             return __Pyx_PyObject_CallMethO(func, arg);
 #if CYTHON_FAST_PYCCALL
-        } else if (__Pyx_PyFastCFunction_Check(func)) {
+        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
             return __Pyx_PyCFunction_FastCall(func, &arg, 1);
 #endif
         }
     }
     return __Pyx__PyObject_CallOneArg(func, arg);
 }
 #else
@@ -11561,15 +11703,15 @@
         size = PyByteArray_GET_SIZE(c);
         if (likely(size == 1)) {
             return (unsigned char) PyByteArray_AS_STRING(c)[0];
         }
 #endif
     } else {
         PyErr_Format(PyExc_TypeError,
-            "ord() expected string of length 1, but %.200s found", Py_TYPE(c)->tp_name);
+            "ord() expected string of length 1, but %.200s found", c->ob_type->tp_name);
         return (long)(Py_UCS4)-1;
     }
     PyErr_Format(PyExc_TypeError,
         "ord() expected a character, but string of length %zd found", size);
     return (long)(Py_UCS4)-1;
 }
 
@@ -11593,14 +11735,163 @@
         return NULL;
     }
     Py_INCREF(value);
     return value;
 }
 #endif
 
+/* BytesEquals */
+static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+    if (s1 == s2) {
+        return (equals == Py_EQ);
+    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
+        const char *ps1, *ps2;
+        Py_ssize_t length = PyBytes_GET_SIZE(s1);
+        if (length != PyBytes_GET_SIZE(s2))
+            return (equals == Py_NE);
+        ps1 = PyBytes_AS_STRING(s1);
+        ps2 = PyBytes_AS_STRING(s2);
+        if (ps1[0] != ps2[0]) {
+            return (equals == Py_NE);
+        } else if (length == 1) {
+            return (equals == Py_EQ);
+        } else {
+            int result;
+#if CYTHON_USE_UNICODE_INTERNALS
+            Py_hash_t hash1, hash2;
+            hash1 = ((PyBytesObject*)s1)->ob_shash;
+            hash2 = ((PyBytesObject*)s2)->ob_shash;
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                return (equals == Py_NE);
+            }
+#endif
+            result = memcmp(ps1, ps2, (size_t)length);
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
+        return (equals == Py_NE);
+    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
+        return (equals == Py_NE);
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+#endif
+}
+
+/* UnicodeEquals */
+static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
+#if CYTHON_COMPILING_IN_PYPY
+    return PyObject_RichCompareBool(s1, s2, equals);
+#else
+#if PY_MAJOR_VERSION < 3
+    PyObject* owned_ref = NULL;
+#endif
+    int s1_is_unicode, s2_is_unicode;
+    if (s1 == s2) {
+        goto return_eq;
+    }
+    s1_is_unicode = PyUnicode_CheckExact(s1);
+    s2_is_unicode = PyUnicode_CheckExact(s2);
+#if PY_MAJOR_VERSION < 3
+    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
+        owned_ref = PyUnicode_FromObject(s2);
+        if (unlikely(!owned_ref))
+            return -1;
+        s2 = owned_ref;
+        s2_is_unicode = 1;
+    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
+        owned_ref = PyUnicode_FromObject(s1);
+        if (unlikely(!owned_ref))
+            return -1;
+        s1 = owned_ref;
+        s1_is_unicode = 1;
+    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
+        return __Pyx_PyBytes_Equals(s1, s2, equals);
+    }
+#endif
+    if (s1_is_unicode & s2_is_unicode) {
+        Py_ssize_t length;
+        int kind;
+        void *data1, *data2;
+        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
+            return -1;
+        length = __Pyx_PyUnicode_GET_LENGTH(s1);
+        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
+            goto return_ne;
+        }
+#if CYTHON_USE_UNICODE_INTERNALS
+        {
+            Py_hash_t hash1, hash2;
+        #if CYTHON_PEP393_ENABLED
+            hash1 = ((PyASCIIObject*)s1)->hash;
+            hash2 = ((PyASCIIObject*)s2)->hash;
+        #else
+            hash1 = ((PyUnicodeObject*)s1)->hash;
+            hash2 = ((PyUnicodeObject*)s2)->hash;
+        #endif
+            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
+                goto return_ne;
+            }
+        }
+#endif
+        kind = __Pyx_PyUnicode_KIND(s1);
+        if (kind != __Pyx_PyUnicode_KIND(s2)) {
+            goto return_ne;
+        }
+        data1 = __Pyx_PyUnicode_DATA(s1);
+        data2 = __Pyx_PyUnicode_DATA(s2);
+        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
+            goto return_ne;
+        } else if (length == 1) {
+            goto return_eq;
+        } else {
+            int result = memcmp(data1, data2, (size_t)(length * kind));
+            #if PY_MAJOR_VERSION < 3
+            Py_XDECREF(owned_ref);
+            #endif
+            return (equals == Py_EQ) ? (result == 0) : (result != 0);
+        }
+    } else if ((s1 == Py_None) & s2_is_unicode) {
+        goto return_ne;
+    } else if ((s2 == Py_None) & s1_is_unicode) {
+        goto return_ne;
+    } else {
+        int result;
+        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
+        #if PY_MAJOR_VERSION < 3
+        Py_XDECREF(owned_ref);
+        #endif
+        if (!py_result)
+            return -1;
+        result = __Pyx_PyObject_IsTrue(py_result);
+        Py_DECREF(py_result);
+        return result;
+    }
+return_eq:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_EQ);
+return_ne:
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(owned_ref);
+    #endif
+    return (equals == Py_NE);
+#endif
+}
+
 /* JoinPyUnicode */
 static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
                                       CYTHON_UNUSED Py_UCS4 max_char) {
 #if CYTHON_USE_UNICODE_INTERNALS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     PyObject *result_uval;
     int result_ukind;
     Py_ssize_t i, char_pos;
@@ -11838,163 +12129,14 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
-/* BytesEquals */
-static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
-#if CYTHON_COMPILING_IN_PYPY
-    return PyObject_RichCompareBool(s1, s2, equals);
-#else
-    if (s1 == s2) {
-        return (equals == Py_EQ);
-    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
-        const char *ps1, *ps2;
-        Py_ssize_t length = PyBytes_GET_SIZE(s1);
-        if (length != PyBytes_GET_SIZE(s2))
-            return (equals == Py_NE);
-        ps1 = PyBytes_AS_STRING(s1);
-        ps2 = PyBytes_AS_STRING(s2);
-        if (ps1[0] != ps2[0]) {
-            return (equals == Py_NE);
-        } else if (length == 1) {
-            return (equals == Py_EQ);
-        } else {
-            int result;
-#if CYTHON_USE_UNICODE_INTERNALS
-            Py_hash_t hash1, hash2;
-            hash1 = ((PyBytesObject*)s1)->ob_shash;
-            hash2 = ((PyBytesObject*)s2)->ob_shash;
-            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
-                return (equals == Py_NE);
-            }
-#endif
-            result = memcmp(ps1, ps2, (size_t)length);
-            return (equals == Py_EQ) ? (result == 0) : (result != 0);
-        }
-    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
-        return (equals == Py_NE);
-    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
-        return (equals == Py_NE);
-    } else {
-        int result;
-        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
-        if (!py_result)
-            return -1;
-        result = __Pyx_PyObject_IsTrue(py_result);
-        Py_DECREF(py_result);
-        return result;
-    }
-#endif
-}
-
-/* UnicodeEquals */
-static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
-#if CYTHON_COMPILING_IN_PYPY
-    return PyObject_RichCompareBool(s1, s2, equals);
-#else
-#if PY_MAJOR_VERSION < 3
-    PyObject* owned_ref = NULL;
-#endif
-    int s1_is_unicode, s2_is_unicode;
-    if (s1 == s2) {
-        goto return_eq;
-    }
-    s1_is_unicode = PyUnicode_CheckExact(s1);
-    s2_is_unicode = PyUnicode_CheckExact(s2);
-#if PY_MAJOR_VERSION < 3
-    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
-        owned_ref = PyUnicode_FromObject(s2);
-        if (unlikely(!owned_ref))
-            return -1;
-        s2 = owned_ref;
-        s2_is_unicode = 1;
-    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
-        owned_ref = PyUnicode_FromObject(s1);
-        if (unlikely(!owned_ref))
-            return -1;
-        s1 = owned_ref;
-        s1_is_unicode = 1;
-    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
-        return __Pyx_PyBytes_Equals(s1, s2, equals);
-    }
-#endif
-    if (s1_is_unicode & s2_is_unicode) {
-        Py_ssize_t length;
-        int kind;
-        void *data1, *data2;
-        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
-            return -1;
-        length = __Pyx_PyUnicode_GET_LENGTH(s1);
-        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
-            goto return_ne;
-        }
-#if CYTHON_USE_UNICODE_INTERNALS
-        {
-            Py_hash_t hash1, hash2;
-        #if CYTHON_PEP393_ENABLED
-            hash1 = ((PyASCIIObject*)s1)->hash;
-            hash2 = ((PyASCIIObject*)s2)->hash;
-        #else
-            hash1 = ((PyUnicodeObject*)s1)->hash;
-            hash2 = ((PyUnicodeObject*)s2)->hash;
-        #endif
-            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
-                goto return_ne;
-            }
-        }
-#endif
-        kind = __Pyx_PyUnicode_KIND(s1);
-        if (kind != __Pyx_PyUnicode_KIND(s2)) {
-            goto return_ne;
-        }
-        data1 = __Pyx_PyUnicode_DATA(s1);
-        data2 = __Pyx_PyUnicode_DATA(s2);
-        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
-            goto return_ne;
-        } else if (length == 1) {
-            goto return_eq;
-        } else {
-            int result = memcmp(data1, data2, (size_t)(length * kind));
-            #if PY_MAJOR_VERSION < 3
-            Py_XDECREF(owned_ref);
-            #endif
-            return (equals == Py_EQ) ? (result == 0) : (result != 0);
-        }
-    } else if ((s1 == Py_None) & s2_is_unicode) {
-        goto return_ne;
-    } else if ((s2 == Py_None) & s1_is_unicode) {
-        goto return_ne;
-    } else {
-        int result;
-        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
-        #if PY_MAJOR_VERSION < 3
-        Py_XDECREF(owned_ref);
-        #endif
-        if (!py_result)
-            return -1;
-        result = __Pyx_PyObject_IsTrue(py_result);
-        Py_DECREF(py_result);
-        return result;
-    }
-return_eq:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(owned_ref);
-    #endif
-    return (equals == Py_EQ);
-return_ne:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(owned_ref);
-    #endif
-    return (equals == Py_NE);
-#endif
-}
-
 /* GetItemInt */
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
     if (!j) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
@@ -12851,27 +12993,30 @@
         #else
            typedef unsigned __int16  uint16_t;
         #endif
     #endif
 #else
    #include <stdint.h>
 #endif
+#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define GCC_DIAGNOSTIC
+#endif
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_Py_ssize_t(Py_ssize_t value, Py_ssize_t width, char padding_char, char format_char) {
     char digits[sizeof(Py_ssize_t)*3+2];
     char *dpos, *end = digits + sizeof(Py_ssize_t)*3+2;
     const char *hex_digits = DIGITS_HEX;
     Py_ssize_t length, ulength;
     int prepend_sign, last_one_off;
     Py_ssize_t remaining;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#ifdef GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const Py_ssize_t neg_one = (Py_ssize_t) -1, const_zero = (Py_ssize_t) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#ifdef GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (format_char == 'X') {
         hex_digits += 16;
         format_char = 'x';
     }
@@ -13615,14 +13760,45 @@
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
 static PyObject* __pyx_convert__to_py_struct__gencode_3a__3a_GTFLine(struct gencode::GTFLine s) {
   PyObject* res;
   PyObject* member;
   res = __Pyx_PyDict_NewPresized(9); if (unlikely(!res)) return NULL;
   member = __pyx_convert_PyObject_string_to_py_std__in_string(s.chrom); if (unlikely(!member)) goto bad;
   if (unlikely(PyDict_SetItem(res, __pyx_n_s_chrom, member) < 0)) goto bad;
   Py_DECREF(member);
@@ -13652,122 +13828,101 @@
   Py_DECREF(member);
   return res;
   bad:
   Py_XDECREF(member);
   Py_DECREF(res);
   return NULL;
 }
-/* CIntFromPyVerify */
-#define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
-#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
-#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
-    {\
-        func_type value = func_value;\
-        if (sizeof(target_type) < sizeof(func_type)) {\
-            if (unlikely(value != (func_type) (target_type) value)) {\
-                func_type zero = 0;\
-                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
-                    return (target_type) -1;\
-                if (is_unsigned && unlikely(value < zero))\
-                    goto raise_neg_overflow;\
-                else\
-                    goto raise_overflow;\
-            }\
-        }\
-        return (target_type) value;\
-    }
-
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
+    const char neg_one = (char) ((char) 0 - (char) 1), const_zero = (char) 0;
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
+        if (sizeof(char) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
+        } else if (sizeof(char) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(char) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(int) <= sizeof(long)) {
+        if (sizeof(char) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(char) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
+        return _PyLong_FromByteArray(bytes, sizeof(char),
                                      little, !is_unsigned);
     }
 }
 
+/* CIntFromPyVerify */
+#define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
+#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
+#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
+    {\
+        func_type value = func_value;\
+        if (sizeof(target_type) < sizeof(func_type)) {\
+            if (unlikely(value != (func_type) (target_type) value)) {\
+                func_type zero = 0;\
+                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
+                    return (target_type) -1;\
+                if (is_unsigned && unlikely(value < zero))\
+                    goto raise_neg_overflow;\
+                else\
+                    goto raise_overflow;\
+            }\
+        }\
+        return (target_type) value;\
+    }
+
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_char(char value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const char neg_one = (char) -1, const_zero = (char) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(char) < sizeof(long)) {
+        if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(char) <= sizeof(unsigned long)) {
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(char) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(char) <= sizeof(long)) {
+        if (sizeof(long) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(char) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(char),
+        return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -13948,22 +14103,15 @@
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const size_t neg_one = (size_t) -1, const_zero = (size_t) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const size_t neg_one = (size_t) ((size_t) 0 - (size_t) 1), const_zero = (size_t) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(size_t) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(size_t, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -14142,62 +14290,17 @@
     return (size_t) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to size_t");
     return (size_t) -1;
 }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -14853,38 +14956,14 @@
                 exc = __Pyx_PyExc_StopAsyncIteration;
             #endif
             __Pyx_PyErr_SetNone(exc);
         }
     }
     return retval;
 }
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
-static CYTHON_INLINE
-PyObject *__Pyx_PyGen_Send(PyGenObject *gen, PyObject *arg) {
-#if PY_VERSION_HEX <= 0x030A00A1
-    return _PyGen_Send(gen, arg);
-#else
-    PyObject *result;
-    if (PyIter_Send((PyObject*)gen, arg ? arg : Py_None, &result) == PYGEN_RETURN) {
-        if (PyAsyncGen_CheckExact(gen)) {
-            assert(result == Py_None);
-            PyErr_SetNone(PyExc_StopAsyncIteration);
-        }
-        else if (result == Py_None) {
-            PyErr_SetNone(PyExc_StopIteration);
-        }
-        else {
-            _PyGen_SetStopIterationValue(result);
-        }
-        Py_CLEAR(result);
-    }
-    return result;
-#endif
-}
-#endif
 static CYTHON_INLINE
 PyObject *__Pyx_Coroutine_FinishDelegation(__pyx_CoroutineObject *gen) {
     PyObject *ret;
     PyObject *val = NULL;
     __Pyx_Coroutine_Undelegate(gen);
     __Pyx_PyGen__FetchStopIterationValue(__Pyx_PyThreadState_Current, &val);
     ret = __Pyx_Coroutine_SendEx(gen, val, 0);
@@ -14913,20 +14992,20 @@
         #ifdef __Pyx_AsyncGen_USED
         if (__pyx_PyAsyncGenASend_CheckExact(yf)) {
             ret = __Pyx_async_gen_asend_send(yf, value);
         } else
         #endif
         #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
         if (PyGen_CheckExact(yf)) {
-            ret = __Pyx_PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
+            ret = _PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
         } else
         #endif
         #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03050000 && defined(PyCoro_CheckExact) && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
         if (PyCoro_CheckExact(yf)) {
-            ret = __Pyx_PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
+            ret = _PyGen_Send((PyGenObject*)yf, value == Py_None ? NULL : value);
         } else
         #endif
         {
             if (value == Py_None)
                 ret = Py_TYPE(yf)->tp_iternext(yf);
             else
                 ret = __Pyx_PyObject_CallMethod1(yf, __pyx_n_s_send, value);
@@ -15002,15 +15081,15 @@
         #ifdef __Pyx_Generator_USED
         if (__Pyx_Generator_CheckExact(yf)) {
             ret = __Pyx_Generator_Next(yf);
         } else
         #endif
         #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03030000 && (defined(__linux__) || PY_VERSION_HEX >= 0x030600B3)
         if (PyGen_CheckExact(yf)) {
-            ret = __Pyx_PyGen_Send((PyGenObject*)yf, NULL);
+            ret = _PyGen_Send((PyGenObject*)yf, NULL);
         } else
         #endif
         #ifdef __Pyx_Coroutine_USED
         if (__Pyx_Coroutine_Check(yf)) {
             ret = __Pyx_Coroutine_Send(yf, Py_None);
         } else
         #endif
@@ -15162,15 +15241,14 @@
     __Pyx_Coroutine_ExceptionClear(&gen->gi_exc_state);
 #ifdef __Pyx_AsyncGen_USED
     if (__Pyx_AsyncGen_CheckExact(self)) {
         Py_CLEAR(((__pyx_PyAsyncGenObject*)gen)->ag_finalizer);
     }
 #endif
     Py_CLEAR(gen->gi_code);
-    Py_CLEAR(gen->gi_frame);
     Py_CLEAR(gen->gi_name);
     Py_CLEAR(gen->gi_qualname);
     Py_CLEAR(gen->gi_modulename);
     return 0;
 }
 static void __Pyx_Coroutine_dealloc(PyObject *self) {
     __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
@@ -15179,15 +15257,15 @@
         PyObject_ClearWeakRefs(self);
     if (gen->resume_label >= 0) {
         PyObject_GC_Track(self);
 #if PY_VERSION_HEX >= 0x030400a1 && CYTHON_USE_TP_FINALIZE
         if (PyObject_CallFinalizerFromDealloc(self))
 #else
         Py_TYPE(gen)->tp_del(self);
-        if (Py_REFCNT(self) > 0)
+        if (self->ob_refcnt > 0)
 #endif
         {
             return;
         }
         PyObject_GC_UnTrack(self);
     }
 #ifdef __Pyx_AsyncGen_USED
@@ -15206,15 +15284,15 @@
     __pyx_CoroutineObject *gen = (__pyx_CoroutineObject *) self;
     __Pyx_PyThreadState_declare
     if (gen->resume_label < 0) {
         return;
     }
 #if !CYTHON_USE_TP_FINALIZE
     assert(self->ob_refcnt == 0);
-    __Pyx_SET_REFCNT(self, 1);
+    self->ob_refcnt = 1;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&error_type, &error_value, &error_traceback);
 #ifdef __Pyx_AsyncGen_USED
     if (__Pyx_AsyncGen_CheckExact(self)) {
         __pyx_PyAsyncGenObject *agen = (__pyx_PyAsyncGenObject*)self;
         PyObject *finalizer = agen->ag_finalizer;
@@ -15273,25 +15351,25 @@
                 PyErr_WriteUnraisable(self);
         } else {
             Py_DECREF(res);
         }
     }
     __Pyx_ErrRestore(error_type, error_value, error_traceback);
 #if !CYTHON_USE_TP_FINALIZE
-    assert(Py_REFCNT(self) > 0);
+    assert(self->ob_refcnt > 0);
     if (--self->ob_refcnt == 0) {
         return;
     }
     {
-        Py_ssize_t refcnt = Py_REFCNT(self);
+        Py_ssize_t refcnt = self->ob_refcnt;
         _Py_NewReference(self);
-        __Pyx_SET_REFCNT(self, refcnt);
+        self->ob_refcnt = refcnt;
     }
 #if CYTHON_COMPILING_IN_CPYTHON
-    assert(PyType_IS_GC(Py_TYPE(self)) &&
+    assert(PyType_IS_GC(self->ob_type) &&
            _Py_AS_GC(self)->gc.gc_refs != _PyGC_REFS_UNTRACKED);
     _Py_DEC_REFTOTAL;
 #endif
 #ifdef COUNT_ALLOCS
     --Py_TYPE(self)->tp_frees;
     --Py_TYPE(self)->tp_allocs;
 #endif
@@ -15349,35 +15427,14 @@
     }
     tmp = self->gi_qualname;
     Py_INCREF(value);
     self->gi_qualname = value;
     Py_XDECREF(tmp);
     return 0;
 }
-static PyObject *
-__Pyx_Coroutine_get_frame(__pyx_CoroutineObject *self, CYTHON_UNUSED void *context)
-{
-    PyObject *frame = self->gi_frame;
-    if (!frame) {
-        if (unlikely(!self->gi_code)) {
-            Py_RETURN_NONE;
-        }
-        frame = (PyObject *) PyFrame_New(
-            PyThreadState_Get(),            /*PyThreadState *tstate,*/
-            (PyCodeObject*) self->gi_code,  /*PyCodeObject *code,*/
-            __pyx_d,                 /*PyObject *globals,*/
-            0                               /*PyObject *locals*/
-        );
-        if (unlikely(!frame))
-            return NULL;
-        self->gi_frame = frame;
-    }
-    Py_INCREF(frame);
-    return frame;
-}
 static __pyx_CoroutineObject *__Pyx__Coroutine_New(
             PyTypeObject* type, __pyx_coroutine_body_t body, PyObject *code, PyObject *closure,
             PyObject *name, PyObject *qualname, PyObject *module_name) {
     __pyx_CoroutineObject *gen = PyObject_GC_New(__pyx_CoroutineObject, type);
     if (unlikely(!gen))
         return NULL;
     return __Pyx__Coroutine_NewInit(gen, body, code, closure, name, qualname, module_name);
@@ -15403,15 +15460,14 @@
     gen->gi_qualname = qualname;
     Py_XINCREF(name);
     gen->gi_name = name;
     Py_XINCREF(module_name);
     gen->gi_modulename = module_name;
     Py_XINCREF(code);
     gen->gi_code = code;
-    gen->gi_frame = NULL;
     PyObject_GC_Track(gen);
     return gen;
 }
 
 /* PatchModuleWithCoroutine */
 static PyObject* __Pyx_Coroutine_patch_module(PyObject* module, const char* py_code) {
 #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
@@ -15527,16 +15583,14 @@
     {0, 0, 0, 0, 0}
 };
 static PyGetSetDef __pyx_Generator_getsets[] = {
     {(char *) "__name__", (getter)__Pyx_Coroutine_get_name, (setter)__Pyx_Coroutine_set_name,
      (char*) PyDoc_STR("name of the generator"), 0},
     {(char *) "__qualname__", (getter)__Pyx_Coroutine_get_qualname, (setter)__Pyx_Coroutine_set_qualname,
      (char*) PyDoc_STR("qualified name of the generator"), 0},
-    {(char *) "gi_frame", (getter)__Pyx_Coroutine_get_frame, NULL,
-     (char*) PyDoc_STR("Frame of the generator"), 0},
     {0, 0, 0, 0, 0}
 };
 static PyTypeObject __pyx_GeneratorType_type = {
     PyVarObject_HEAD_INIT(0, 0)
     "generator",
     sizeof(__pyx_CoroutineObject),
     0,
```

### Comparing `denovonear-0.9.8/denovonear/gencode.pyx` & `denovonear-0.9.9/denovonear/gencode.pyx`

 * *Files 3% similar despite different names*

```diff
@@ -116,14 +116,17 @@
         cdef Tx tx = Tx(tx_id, chrom, start, end, strand)
         tx.set_exons(exons, cds)
         tx.set_cds(cds)
         
         cdef string seq = _tx.get_genomic_sequence().encode('utf8')
         cdef int offset = _tx.get_genomic_offset()
         if len(seq) > 0:
+            if chr(strand) == '-':
+                _tx.reverse_complement(seq)
+                seq = _tx.reverse_complement(seq).encode('utf8')
             tx.add_genomic_sequence(seq, offset)
         self.add_tx(tx, False)
     
     def __repr__(self):
         chrom = self.chrom
         return f'Gene("{self.symbol}", {chrom}:{self.start}-{self.end})'
     
@@ -176,15 +179,17 @@
         exons = self._convert_exons(tx.get_exons())
         cds = self._convert_exons(tx.get_cds())
         seq = tx.get_genomic_sequence().decode('utf8')
         if seq == '':
             seq = None
         if seq is None and __genome_ is not None:
             seq = __genome_[chrom][start-1-offset:end-1+offset].seq.upper()
-        strand = self.strand
+        strand = chr(tx.get_strand())
+        if strand == '-':
+            seq = tx.reverse_complement(seq.encode('utf8')).decode('utf8')
         tx_id = tx.get_name().decode('utf8')
         return Transcript(tx_id, chrom, start, end, strand, exons, cds, seq, offset=offset)
     
     @property
     def transcripts(self):
         ''' get list of Transcripts for gene, with genomic DNA included
         '''
```

### Comparing `denovonear-0.9.8/denovonear/load_de_novos.py` & `denovonear-0.9.9/denovonear/load_de_novos.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/load_gene.py` & `denovonear-0.9.9/denovonear/load_gene.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/load_mutation_rates.py` & `denovonear-0.9.9/denovonear/load_mutation_rates.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/rate_limiter.py` & `denovonear-0.9.9/denovonear/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/rate_limiter_retries.py` & `denovonear-0.9.9/denovonear/rate_limiter_retries.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/simulate.py` & `denovonear-0.9.9/denovonear/simulate.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/site_specific_rates.cpp` & `denovonear-0.9.9/denovonear/site_specific_rates.cpp`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/site_specific_rates.pyx` & `denovonear-0.9.9/denovonear/site_specific_rates.pyx`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/transcript.cpp` & `denovonear-0.9.9/denovonear/transcript.cpp`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/transcript.pxd` & `denovonear-0.9.9/denovonear/transcript.pxd`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/transcript.pyx` & `denovonear-0.9.9/denovonear/transcript.pyx`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/weights.cpp` & `denovonear-0.9.9/denovonear/weights.cpp`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/weights.pxd` & `denovonear-0.9.9/denovonear/weights.pxd`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear/weights.pyx` & `denovonear-0.9.9/denovonear/weights.pyx`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/denovonear.egg-info/PKG-INFO` & `denovonear-0.9.9/denovonear.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denovonear
-Version: 0.9.8
+Version: 0.9.9
 Summary: Package to examine de novo clustering
 Home-page: https://github.com/jeremymcrae/denovonear
 Author: Jeremy McRae
 Author-email: jeremy.mcrae@gmail.com
 License: MIT
 Description: ![travis](https://travis-ci.org/jeremymcrae/denovonear.svg?branch=master)
```

### Comparing `denovonear-0.9.8/denovonear.egg-info/SOURCES.txt` & `denovonear-0.9.9/denovonear.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/scripts/run_batch.py` & `denovonear-0.9.9/scripts/run_batch.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/setup.py` & `denovonear-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         language="c++"),
     ])
 
 setup(name="denovonear",
     description='Package to examine de novo clustering',
     long_description=io.open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
-    version="0.9.8",
+    version="0.9.9",
     author="Jeremy McRae",
     author_email="jeremy.mcrae@gmail.com",
     license="MIT",
     url='https://github.com/jeremymcrae/denovonear',
     packages=["denovonear"],
     install_requires=[
         'aiohttp >= 3.0',
```

### Comparing `denovonear-0.9.8/src/gencode.cpp` & `denovonear-0.9.9/src/gencode.cpp`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/src/gencode.h` & `denovonear-0.9.9/src/gencode.h`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/src/gtf.cpp` & `denovonear-0.9.9/src/gtf.cpp`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/src/gtf.h` & `denovonear-0.9.9/src/gtf.h`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/src/gzstream/gzstream.C` & `denovonear-0.9.9/src/gzstream/gzstream.C`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/src/gzstream/gzstream.h` & `denovonear-0.9.9/src/gzstream/gzstream.h`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/src/simulate.cpp` & `denovonear-0.9.9/src/simulate.cpp`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/src/simulate.h` & `denovonear-0.9.9/src/simulate.h`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/src/site_rates.cpp` & `denovonear-0.9.9/src/site_rates.cpp`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/src/site_rates.h` & `denovonear-0.9.9/src/site_rates.h`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/src/tx.cpp` & `denovonear-0.9.9/src/tx.cpp`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/src/tx.h` & `denovonear-0.9.9/src/tx.h`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/src/weighted_choice.cpp` & `denovonear-0.9.9/src/weighted_choice.cpp`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/src/weighted_choice.h` & `denovonear-0.9.9/src/weighted_choice.h`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/tests/test_cluster_test.py` & `denovonear-0.9.9/tests/test_cluster_test.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/tests/test_ensembl_cache.py` & `denovonear-0.9.9/tests/test_ensembl_cache.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/tests/test_ensembl_requester.py` & `denovonear-0.9.9/tests/test_ensembl_requester.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/tests/test_frameshift_rate.py` & `denovonear-0.9.9/tests/test_frameshift_rate.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/tests/test_gencode.py` & `denovonear-0.9.9/tests/test_gencode.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/tests/test_geometric_mean.py` & `denovonear-0.9.9/tests/test_geometric_mean.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/tests/test_load_gene.py` & `denovonear-0.9.9/tests/test_load_gene.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/tests/test_log_transform.py` & `denovonear-0.9.9/tests/test_log_transform.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/tests/test_sequence_methods.py` & `denovonear-0.9.9/tests/test_sequence_methods.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/tests/test_simulate_p_value.py` & `denovonear-0.9.9/tests/test_simulate_p_value.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/tests/test_simulations.py` & `denovonear-0.9.9/tests/test_simulations.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/tests/test_site_rates.py` & `denovonear-0.9.9/tests/test_site_rates.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/tests/test_transcript.py` & `denovonear-0.9.9/tests/test_transcript.py`

 * *Files identical despite different names*

### Comparing `denovonear-0.9.8/tests/test_weighted_choice.py` & `denovonear-0.9.9/tests/test_weighted_choice.py`

 * *Files identical despite different names*

