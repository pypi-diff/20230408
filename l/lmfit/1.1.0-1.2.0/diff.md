# Comparing `tmp/lmfit-1.1.0.tar.gz` & `tmp/lmfit-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmfit-1.1.0.tar", last modified: Mon Nov 28 04:57:02 2022, max compression
+gzip compressed data, was "lmfit-1.2.0.tar", last modified: Sat Apr  8 19:48:27 2023, max compression
```

## Comparing `lmfit-1.1.0.tar` & `lmfit-1.2.0.tar`

### file list

```diff
@@ -1,201 +1,203 @@
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.423685 lmfit-1.1.0/
--rw-r--r--   0 Newville   (501) staff       (20)      308 2022-11-05 18:38:23.000000 lmfit-1.1.0/.codecov.yml
--rw-r--r--   0 Newville   (501) staff       (20)      393 2022-11-05 18:38:23.000000 lmfit-1.1.0/.gitattributes
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.398196 lmfit-1.1.0/.github/
--rw-r--r--   0 Newville   (501) staff       (20)     5158 2022-11-05 18:38:23.000000 lmfit-1.1.0/.github/CONTRIBUTING.md
--rw-r--r--   0 Newville   (501) staff       (20)     2465 2022-11-05 18:38:23.000000 lmfit-1.1.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 Newville   (501) staff       (20)     2211 2022-11-05 18:38:23.000000 lmfit-1.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 Newville   (501) staff       (20)      502 2022-11-05 18:38:23.000000 lmfit-1.1.0/.github/dependabot.yml
--rw-r--r--   0 Newville   (501) staff       (20)      264 2022-11-05 18:38:23.000000 lmfit-1.1.0/.gitignore
--rw-r--r--   0 Newville   (501) staff       (20)     1675 2022-11-28 04:13:55.000000 lmfit-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 Newville   (501) staff       (20)     3015 2022-11-05 18:38:23.000000 lmfit-1.1.0/AUTHORS.txt
--rw-r--r--   0 Newville   (501) staff       (20)     3670 2022-11-05 18:38:23.000000 lmfit-1.1.0/LICENSE
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.403387 lmfit-1.1.0/NIST_STRD/
--rw-r--r--   0 Newville   (501) staff       (20)     6869 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Bennett5.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1713 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/BoxBOD.dat
--rw-r--r--   0 Newville   (501) staff       (20)     7558 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Chwirut1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3060 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Chwirut2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1990 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/DanWood.dat
--rw-r--r--   0 Newville   (501) staff       (20)     6761 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/ENSO.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2773 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Eckerle4.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8098 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Gauss1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8100 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Gauss2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     8102 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Gauss3.dat
--rw-r--r--   0 Newville   (501) staff       (20)     9276 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Hahn1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     5858 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Kirby2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2945 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Lanczos1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2601 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Lanczos2.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2574 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Lanczos3.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2305 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/MGH09.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2335 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/MGH10.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3078 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/MGH17.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1853 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Misra1a.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1845 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Misra1b.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1839 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Misra1c.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1843 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Misra1d.dat
--rw-r--r--   0 Newville   (501) staff       (20)     6401 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Models
--rw-r--r--   0 Newville   (501) staff       (20)     7001 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Nelson.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1873 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Rat42.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2072 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Rat43.dat
--rw-r--r--   0 Newville   (501) staff       (20)     2486 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Roszman1.dat
--rw-r--r--   0 Newville   (501) staff       (20)     3026 2022-11-05 18:38:23.000000 lmfit-1.1.0/NIST_STRD/Thurber.dat
--rw-r--r--   0 Newville   (501) staff       (20)     5721 2022-11-28 04:57:02.423884 lmfit-1.1.0/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)     4220 2022-11-05 18:38:23.000000 lmfit-1.1.0/README.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.403846 lmfit-1.1.0/asv_benchmarking/
--rw-r--r--   0 Newville   (501) staff       (20)       43 2022-11-05 18:38:23.000000 lmfit-1.1.0/asv_benchmarking/README.md
--rw-r--r--   0 Newville   (501) staff       (20)     2793 2022-11-05 18:38:23.000000 lmfit-1.1.0/asv_benchmarking/asv.conf.json
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.404128 lmfit-1.1.0/asv_benchmarking/benchmarks/
--rw-r--r--   0 Newville   (501) staff       (20)        0 2022-11-05 18:38:23.000000 lmfit-1.1.0/asv_benchmarking/benchmarks/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)     4394 2022-11-05 18:38:23.000000 lmfit-1.1.0/asv_benchmarking/benchmarks/benchmarks.py
--rw-r--r--   0 Newville   (501) staff       (20)      350 2022-11-05 18:38:23.000000 lmfit-1.1.0/asv_benchmarking/run_benchmark_code.py
--rw-r--r--   0 Newville   (501) staff       (20)    12175 2022-11-26 13:21:41.000000 lmfit-1.1.0/azure-pipelines.yml
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.407091 lmfit-1.1.0/doc/
--rw-r--r--   0 Newville   (501) staff       (20)     4460 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/Makefile
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.407252 lmfit-1.1.0/doc/_static/
--rw-r--r--   0 Newville   (501) staff       (20)        0 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/_static/empty
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.407371 lmfit-1.1.0/doc/_templates/
--rw-r--r--   0 Newville   (501) staff       (20)      756 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/_templates/indexsidebar.html
--rw-r--r--   0 Newville   (501) staff       (20)     3499 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/bounds.rst
--rw-r--r--   0 Newville   (501) staff       (20)    30644 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/builtin_models.rst
--rw-r--r--   0 Newville   (501) staff       (20)     6527 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/conf.py
--rw-r--r--   0 Newville   (501) staff       (20)     9005 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/confidence.rst
--rw-r--r--   0 Newville   (501) staff       (20)     8108 2022-11-08 21:32:24.000000 lmfit-1.1.0/doc/constraints.rst
--rw-r--r--   0 Newville   (501) staff       (20)      223 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/contents.rst
--rwxr-xr-x   0 Newville   (501) staff       (20)     1943 2022-11-08 21:32:18.000000 lmfit-1.1.0/doc/doc_examples_to_gallery.py
--rw-r--r--   0 Newville   (501) staff       (20)    12177 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/faq.rst
--rwxr-xr-x   0 Newville   (501) staff       (20)      660 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/filter_spurious_link_from_html.py
--rw-r--r--   0 Newville   (501) staff       (20)    34852 2022-11-08 21:32:24.000000 lmfit-1.1.0/doc/fitting.rst
--rw-r--r--   0 Newville   (501) staff       (20)     2916 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/index.rst
--rw-r--r--   0 Newville   (501) staff       (20)     5036 2022-11-26 13:21:41.000000 lmfit-1.1.0/doc/installation.rst
--rw-r--r--   0 Newville   (501) staff       (20)     7944 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/intro.rst
--rw-r--r--   0 Newville   (501) staff       (20)      941 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/make.bat
--rw-r--r--   0 Newville   (501) staff       (20)    38552 2022-11-21 20:58:02.000000 lmfit-1.1.0/doc/model.rst
--rw-r--r--   0 Newville   (501) staff       (20)     4131 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/parameters.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.407640 lmfit-1.1.0/doc/sphinx/
--rw-r--r--   0 Newville   (501) staff       (20)      460 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/sphinx/ext_imgmath.py
--rw-r--r--   0 Newville   (501) staff       (20)      407 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/sphinx/ext_mathjax.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.395640 lmfit-1.1.0/doc/sphinx/theme/
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.408051 lmfit-1.1.0/doc/sphinx/theme/sphinx13/
--rw-r--r--   0 Newville   (501) staff       (20)     7546 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/sphinx/theme/sphinx13/basic_layout.html
--rw-r--r--   0 Newville   (501) staff       (20)     3080 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/sphinx/theme/sphinx13/layout.html
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.409063 lmfit-1.1.0/doc/sphinx/theme/sphinx13/static/
--rw-r--r--   0 Newville   (501) staff       (20)      429 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/sphinx/theme/sphinx13/static/bodybg.png
--rw-r--r--   0 Newville   (501) staff       (20)      180 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/sphinx/theme/sphinx13/static/footerbg.png
--rw-r--r--   0 Newville   (501) staff       (20)      189 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/sphinx/theme/sphinx13/static/headerbg.png
--rw-r--r--   0 Newville   (501) staff       (20)      149 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/sphinx/theme/sphinx13/static/listitem.png
--rw-r--r--   0 Newville   (501) staff       (20)     9907 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/sphinx/theme/sphinx13/static/lmfitheader.png
--rw-r--r--   0 Newville   (501) staff       (20)      183 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/sphinx/theme/sphinx13/static/relbg.png
--rw-r--r--   0 Newville   (501) staff       (20)     7978 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/sphinx/theme/sphinx13/static/sphinx13.css
--rw-r--r--   0 Newville   (501) staff       (20)       72 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/sphinx/theme/sphinx13/theme.conf
--rw-r--r--   0 Newville   (501) staff       (20)     1500 2022-11-05 18:38:23.000000 lmfit-1.1.0/doc/support.rst
--rw-r--r--   0 Newville   (501) staff       (20)    23635 2022-11-28 04:19:43.000000 lmfit-1.1.0/doc/whatsnew.rst
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.415830 lmfit-1.1.0/examples/
--rw-r--r--   0 Newville   (501) staff       (20)     8195 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/NIST_Gauss2.dat
--rw-r--r--   0 Newville   (501) staff       (20)      419 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/README.txt
--rw-r--r--   0 Newville   (501) staff       (20)     1352 2022-11-08 18:05:54.000000 lmfit-1.1.0/examples/doc_builtinmodels_nistgauss.py
--rw-r--r--   0 Newville   (501) staff       (20)     1010 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_builtinmodels_nistgauss2.py
--rw-r--r--   0 Newville   (501) staff       (20)     1307 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_builtinmodels_peakmodels.py
--rw-r--r--   0 Newville   (501) staff       (20)     1938 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_builtinmodels_splinemodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      784 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_builtinmodels_stepmodel.py
--rw-r--r--   0 Newville   (501) staff       (20)     1998 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_confidence_advanced.py
--rw-r--r--   0 Newville   (501) staff       (20)      504 2022-11-23 14:06:24.000000 lmfit-1.1.0/examples/doc_confidence_basic.py
--rw-r--r--   0 Newville   (501) staff       (20)     3359 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_fitting_emcee.py
--rw-r--r--   0 Newville   (501) staff       (20)     1144 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_fitting_withreport.py
--rw-r--r--   0 Newville   (501) staff       (20)     1791 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_model_composite.py
--rw-r--r--   0 Newville   (501) staff       (20)      651 2022-11-06 22:24:00.000000 lmfit-1.1.0/examples/doc_model_gaussian.py
--rw-r--r--   0 Newville   (501) staff       (20)      626 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_model_loadmodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      396 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_model_loadmodelresult.py
--rw-r--r--   0 Newville   (501) staff       (20)      397 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_model_loadmodelresult2.py
--rw-r--r--   0 Newville   (501) staff       (20)      337 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_model_savemodel.py
--rw-r--r--   0 Newville   (501) staff       (20)      423 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_model_savemodelresult.py
--rw-r--r--   0 Newville   (501) staff       (20)      932 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_model_savemodelresult2.py
--rw-r--r--   0 Newville   (501) staff       (20)      819 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_model_two_components.py
--rw-r--r--   0 Newville   (501) staff       (20)      834 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_model_uncertainty.py
--rw-r--r--   0 Newville   (501) staff       (20)     3154 2022-11-21 20:58:02.000000 lmfit-1.1.0/examples/doc_model_uncertainty2.py
--rw-r--r--   0 Newville   (501) staff       (20)      994 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_model_with_iter_callback.py
--rw-r--r--   0 Newville   (501) staff       (20)      775 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_model_with_nan_policy.py
--rw-r--r--   0 Newville   (501) staff       (20)     1283 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_parameters_basic.py
--rw-r--r--   0 Newville   (501) staff       (20)     1235 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/doc_parameters_valuesdict.py
--rw-r--r--   0 Newville   (501) staff       (20)     7704 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_Model_interface.py
--rw-r--r--   0 Newville   (501) staff       (20)    17663 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_brute.py
--rw-r--r--   0 Newville   (501) staff       (20)     4731 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_complex_resonator_model.py
--rw-r--r--   0 Newville   (501) staff       (20)     4548 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_confidence_interval.py
--rw-r--r--   0 Newville   (501) staff       (20)     3331 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_detect_outliers.py
--rw-r--r--   0 Newville   (501) staff       (20)     1795 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_diffev.py
--rw-r--r--   0 Newville   (501) staff       (20)     4098 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_emcee_Model_interface.py
--rw-r--r--   0 Newville   (501) staff       (20)     1273 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_expression_model.py
--rw-r--r--   0 Newville   (501) staff       (20)     2742 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_fit_multi_datasets.py
--rw-r--r--   0 Newville   (501) staff       (20)     1687 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_fit_with_algebraic_constraint.py
--rw-r--r--   0 Newville   (501) staff       (20)     2176 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_fit_with_bounds.py
--rw-r--r--   0 Newville   (501) staff       (20)     2666 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_fit_with_derivfunc.py
--rw-r--r--   0 Newville   (501) staff       (20)     2248 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_fit_with_inequality.py
--rw-r--r--   0 Newville   (501) staff       (20)     2383 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_reduce_fcn.py
--rw-r--r--   0 Newville   (501) staff       (20)     2915 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_sympy.py
--rw-r--r--   0 Newville   (501) staff       (20)     6112 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_two_dimensional_peak.py
--rw-r--r--   0 Newville   (501) staff       (20)      851 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/example_use_pandas.py
--rw-r--r--   0 Newville   (501) staff       (20)     7777 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/lmfit_emcee_model_selection.py
--rw-r--r--   0 Newville   (501) staff       (20)     2373 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/model1d_gauss.dat
--rw-r--r--   0 Newville   (501) staff       (20)     1987 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/peak.csv
--rw-r--r--   0 Newville   (501) staff       (20)     2464 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/sinedata.dat
--rw-r--r--   0 Newville   (501) staff       (20)     9496 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/test_peak.dat
--rw-r--r--   0 Newville   (501) staff       (20)    11611 2022-11-05 18:38:23.000000 lmfit-1.1.0/examples/test_splinepeak.dat
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.417482 lmfit-1.1.0/lmfit/
--rw-r--r--   0 Newville   (501) staff       (20)     1941 2022-11-05 18:38:23.000000 lmfit-1.1.0/lmfit/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)    10016 2022-11-05 18:38:23.000000 lmfit-1.1.0/lmfit/_ampgo.py
--rw-r--r--   0 Newville   (501) staff       (20)    14872 2022-11-05 18:38:23.000000 lmfit-1.1.0/lmfit/confidence.py
--rw-r--r--   0 Newville   (501) staff       (20)     4808 2022-11-05 18:38:23.000000 lmfit-1.1.0/lmfit/jsonutils.py
--rw-r--r--   0 Newville   (501) staff       (20)    16911 2022-11-08 21:32:24.000000 lmfit-1.1.0/lmfit/lineshapes.py
--rw-r--r--   0 Newville   (501) staff       (20)   105145 2022-11-26 13:21:41.000000 lmfit-1.1.0/lmfit/minimizer.py
--rw-r--r--   0 Newville   (501) staff       (20)    80242 2022-11-21 20:58:02.000000 lmfit-1.1.0/lmfit/model.py
--rw-r--r--   0 Newville   (501) staff       (20)    65950 2022-11-08 21:32:24.000000 lmfit-1.1.0/lmfit/models.py
--rw-r--r--   0 Newville   (501) staff       (20)    33222 2022-11-08 17:36:35.000000 lmfit-1.1.0/lmfit/parameter.py
--rw-r--r--   0 Newville   (501) staff       (20)    13720 2022-11-05 18:38:23.000000 lmfit-1.1.0/lmfit/printfuncs.py
--rw-r--r--   0 Newville   (501) staff       (20)      176 2022-11-28 04:57:02.000000 lmfit-1.1.0/lmfit/version.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.418166 lmfit-1.1.0/lmfit.egg-info/
--rw-r--r--   0 Newville   (501) staff       (20)     5721 2022-11-28 04:57:02.000000 lmfit-1.1.0/lmfit.egg-info/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)     4897 2022-11-28 04:57:02.000000 lmfit-1.1.0/lmfit.egg-info/SOURCES.txt
--rw-r--r--   0 Newville   (501) staff       (20)        1 2022-11-28 04:57:02.000000 lmfit-1.1.0/lmfit.egg-info/dependency_links.txt
--rw-r--r--   0 Newville   (501) staff       (20)      665 2022-11-28 04:57:02.000000 lmfit-1.1.0/lmfit.egg-info/requires.txt
--rw-r--r--   0 Newville   (501) staff       (20)        6 2022-11-28 04:57:02.000000 lmfit-1.1.0/lmfit.egg-info/top_level.txt
--rwxr-xr-x   0 Newville   (501) staff       (20)     1010 2022-11-05 18:38:23.000000 lmfit-1.1.0/publish_docs.sh
--rw-r--r--   0 Newville   (501) staff       (20)      202 2022-11-05 18:38:23.000000 lmfit-1.1.0/pyproject.toml
--rw-r--r--   0 Newville   (501) staff       (20)     2445 2022-11-28 04:57:02.424527 lmfit-1.1.0/setup.cfg
--rw-r--r--   0 Newville   (501) staff       (20)       92 2022-11-05 18:38:23.000000 lmfit-1.1.0/setup.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2022-11-28 04:57:02.423534 lmfit-1.1.0/tests/
--rw-r--r--   0 Newville   (501) staff       (20)     6109 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/NISTModels.py
--rw-r--r--   0 Newville   (501) staff       (20)        0 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)      893 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/conftest.py
--rw-r--r--   0 Newville   (501) staff       (20)     1374 2022-11-20 20:10:41.000000 lmfit-1.1.0/tests/test_1variable.py
--rw-r--r--   0 Newville   (501) staff       (20)     7097 2022-11-20 20:10:41.000000 lmfit-1.1.0/tests/test_NIST_Strd.py
--rw-r--r--   0 Newville   (501) staff       (20)     3951 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_algebraic_constraint.py
--rw-r--r--   0 Newville   (501) staff       (20)     5196 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_ampgo.py
--rw-r--r--   0 Newville   (501) staff       (20)     1238 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_basicfit.py
--rw-r--r--   0 Newville   (501) staff       (20)     3911 2022-11-26 13:21:41.000000 lmfit-1.1.0/tests/test_basinhopping.py
--rw-r--r--   0 Newville   (501) staff       (20)     1900 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_bounded_jacobian.py
--rw-r--r--   0 Newville   (501) staff       (20)     1413 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_bounds.py
--rw-r--r--   0 Newville   (501) staff       (20)    11428 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_brute.py
--rw-r--r--   0 Newville   (501) staff       (20)    11953 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_builtin_models.py
--rw-r--r--   0 Newville   (501) staff       (20)     9251 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_confidence.py
--rw-r--r--   0 Newville   (501) staff       (20)     9909 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_covariance_matrix.py
--rw-r--r--   0 Newville   (501) staff       (20)     1235 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_custom_independentvar.py
--rw-r--r--   0 Newville   (501) staff       (20)      612 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_default_kws.py
--rw-r--r--   0 Newville   (501) staff       (20)     2595 2022-11-26 13:21:41.000000 lmfit-1.1.0/tests/test_dual_annealing.py
--rw-r--r--   0 Newville   (501) staff       (20)     4364 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_itercb.py
--rw-r--r--   0 Newville   (501) staff       (20)     3066 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_jsonutils.py
--rw-r--r--   0 Newville   (501) staff       (20)     6200 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_least_squares.py
--rw-r--r--   0 Newville   (501) staff       (20)     4804 2022-11-08 21:32:24.000000 lmfit-1.1.0/tests/test_lineshapes.py
--rw-r--r--   0 Newville   (501) staff       (20)      781 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_manypeaks_speed.py
--rw-r--r--   0 Newville   (501) staff       (20)     3689 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_max_nfev.py
--rw-r--r--   0 Newville   (501) staff       (20)      545 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_minimizer.py
--rw-r--r--   0 Newville   (501) staff       (20)    50384 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_model.py
--rw-r--r--   0 Newville   (501) staff       (20)     8904 2022-11-21 20:58:02.000000 lmfit-1.1.0/tests/test_model_saveload.py
--rw-r--r--   0 Newville   (501) staff       (20)     4354 2022-11-21 20:58:02.000000 lmfit-1.1.0/tests/test_model_uncertainties.py
--rw-r--r--   0 Newville   (501) staff       (20)     4463 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_models.py
--rw-r--r--   0 Newville   (501) staff       (20)     2181 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_multidatasets.py
--rw-r--r--   0 Newville   (501) staff       (20)    22900 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_nose.py
--rw-r--r--   0 Newville   (501) staff       (20)     1168 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_pandas.py
--rw-r--r--   0 Newville   (501) staff       (20)    19779 2022-11-20 20:10:41.000000 lmfit-1.1.0/tests/test_parameter.py
--rw-r--r--   0 Newville   (501) staff       (20)    19772 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_parameters.py
--rw-r--r--   0 Newville   (501) staff       (20)    14520 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_printfuncs.py
--rw-r--r--   0 Newville   (501) staff       (20)     4784 2022-11-26 13:21:41.000000 lmfit-1.1.0/tests/test_shgo.py
--rw-r--r--   0 Newville   (501) staff       (20)     1503 2022-11-05 18:38:23.000000 lmfit-1.1.0/tests/test_stepmodel.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.419321 lmfit-1.2.0/
+-rw-r--r--   0 Newville   (501) staff       (20)      308 2023-02-23 19:14:07.000000 lmfit-1.2.0/.codecov.yml
+-rw-r--r--   0 Newville   (501) staff       (20)      393 2023-02-23 19:14:07.000000 lmfit-1.2.0/.gitattributes
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.388061 lmfit-1.2.0/.github/
+-rw-r--r--   0 Newville   (501) staff       (20)     5158 2023-02-23 19:14:07.000000 lmfit-1.2.0/.github/CONTRIBUTING.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2465 2023-02-23 19:14:07.000000 lmfit-1.2.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2211 2023-02-23 19:14:07.000000 lmfit-1.2.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 Newville   (501) staff       (20)      502 2023-02-23 19:14:07.000000 lmfit-1.2.0/.github/dependabot.yml
+-rw-r--r--   0 Newville   (501) staff       (20)      323 2023-03-30 18:04:00.000000 lmfit-1.2.0/.gitignore
+-rw-r--r--   0 Newville   (501) staff       (20)     1676 2023-03-30 18:04:00.000000 lmfit-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 Newville   (501) staff       (20)     3015 2023-02-23 19:14:07.000000 lmfit-1.2.0/AUTHORS.txt
+-rw-r--r--   0 Newville   (501) staff       (20)     3670 2023-02-23 19:14:07.000000 lmfit-1.2.0/LICENSE
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.392814 lmfit-1.2.0/NIST_STRD/
+-rw-r--r--   0 Newville   (501) staff       (20)     6869 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Bennett5.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1713 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/BoxBOD.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     7558 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Chwirut1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3060 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Chwirut2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1990 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/DanWood.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     6761 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/ENSO.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2773 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Eckerle4.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8098 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Gauss1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8100 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Gauss2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     8102 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Gauss3.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     9276 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Hahn1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     5858 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Kirby2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2945 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Lanczos1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2601 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Lanczos2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2574 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Lanczos3.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2305 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/MGH09.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2335 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/MGH10.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3078 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/MGH17.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1853 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Misra1a.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1845 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Misra1b.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1839 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Misra1c.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1843 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Misra1d.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     6401 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Models
+-rw-r--r--   0 Newville   (501) staff       (20)     7001 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Nelson.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1873 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Rat42.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2072 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Rat43.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     2486 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Roszman1.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     3026 2023-02-23 19:14:07.000000 lmfit-1.2.0/NIST_STRD/Thurber.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     5721 2023-04-08 19:48:27.419483 lmfit-1.2.0/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)     4220 2023-02-23 19:14:07.000000 lmfit-1.2.0/README.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.393340 lmfit-1.2.0/asv_benchmarking/
+-rw-r--r--   0 Newville   (501) staff       (20)       43 2023-02-23 19:14:07.000000 lmfit-1.2.0/asv_benchmarking/README.md
+-rw-r--r--   0 Newville   (501) staff       (20)     2793 2023-02-23 19:14:07.000000 lmfit-1.2.0/asv_benchmarking/asv.conf.json
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.393653 lmfit-1.2.0/asv_benchmarking/benchmarks/
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2023-02-23 19:14:07.000000 lmfit-1.2.0/asv_benchmarking/benchmarks/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4394 2023-02-23 19:14:07.000000 lmfit-1.2.0/asv_benchmarking/benchmarks/benchmarks.py
+-rw-r--r--   0 Newville   (501) staff       (20)      350 2023-02-23 19:14:07.000000 lmfit-1.2.0/asv_benchmarking/run_benchmark_code.py
+-rw-r--r--   0 Newville   (501) staff       (20)    12176 2023-03-26 20:21:53.000000 lmfit-1.2.0/azure-pipelines.yml
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.397899 lmfit-1.2.0/doc/
+-rw-r--r--   0 Newville   (501) staff       (20)     4386 2023-04-04 03:22:28.000000 lmfit-1.2.0/doc/Makefile
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.398268 lmfit-1.2.0/doc/_static/
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/_static/empty
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.398392 lmfit-1.2.0/doc/_templates/
+-rw-r--r--   0 Newville   (501) staff       (20)      756 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/_templates/indexsidebar.html
+-rw-r--r--   0 Newville   (501) staff       (20)     3499 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/bounds.rst
+-rw-r--r--   0 Newville   (501) staff       (20)    30647 2023-03-30 18:04:00.000000 lmfit-1.2.0/doc/builtin_models.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     6527 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/conf.py
+-rw-r--r--   0 Newville   (501) staff       (20)    15659 2023-03-30 18:04:00.000000 lmfit-1.2.0/doc/confidence.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     8110 2023-03-30 18:04:00.000000 lmfit-1.2.0/doc/constraints.rst
+-rw-r--r--   0 Newville   (501) staff       (20)      223 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/contents.rst
+-rwxr-xr-x   0 Newville   (501) staff       (20)     1943 2023-04-04 02:11:28.000000 lmfit-1.2.0/doc/doc_examples_to_gallery.py
+-rw-r--r--   0 Newville   (501) staff       (20)    12177 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/faq.rst
+-rwxr-xr-x   0 Newville   (501) staff       (20)      660 2023-04-04 02:10:04.000000 lmfit-1.2.0/doc/filter_spurious_link_from_html.py
+-rw-r--r--   0 Newville   (501) staff       (20)    34852 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/fitting.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     2915 2023-03-30 18:04:00.000000 lmfit-1.2.0/doc/index.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     5102 2023-03-30 18:04:00.000000 lmfit-1.2.0/doc/installation.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     9268 2023-03-30 18:04:00.000000 lmfit-1.2.0/doc/intro.rst
+-rw-r--r--   0 Newville   (501) staff       (20)      941 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/make.bat
+-rw-r--r--   0 Newville   (501) staff       (20)    43359 2023-04-04 03:22:28.000000 lmfit-1.2.0/doc/model.rst
+-rw-r--r--   0 Newville   (501) staff       (20)     4611 2023-03-30 18:04:00.000000 lmfit-1.2.0/doc/parameters.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.398767 lmfit-1.2.0/doc/sphinx/
+-rw-r--r--   0 Newville   (501) staff       (20)      460 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/ext_imgmath.py
+-rw-r--r--   0 Newville   (501) staff       (20)      407 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/ext_mathjax.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.384628 lmfit-1.2.0/doc/sphinx/theme/
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.399235 lmfit-1.2.0/doc/sphinx/theme/sphinx13/
+-rw-r--r--   0 Newville   (501) staff       (20)     7546 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/basic_layout.html
+-rw-r--r--   0 Newville   (501) staff       (20)     3080 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/layout.html
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.400444 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/
+-rw-r--r--   0 Newville   (501) staff       (20)      429 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/bodybg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      180 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/footerbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      189 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/headerbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)      149 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/listitem.png
+-rw-r--r--   0 Newville   (501) staff       (20)     9907 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/lmfitheader.png
+-rw-r--r--   0 Newville   (501) staff       (20)      183 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/relbg.png
+-rw-r--r--   0 Newville   (501) staff       (20)     7978 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/sphinx13.css
+-rw-r--r--   0 Newville   (501) staff       (20)       72 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/sphinx/theme/sphinx13/theme.conf
+-rw-r--r--   0 Newville   (501) staff       (20)     1500 2023-02-23 19:14:07.000000 lmfit-1.2.0/doc/support.rst
+-rw-r--r--   0 Newville   (501) staff       (20)    25910 2023-04-07 18:31:26.000000 lmfit-1.2.0/doc/whatsnew.rst
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.408328 lmfit-1.2.0/examples/
+-rw-r--r--   0 Newville   (501) staff       (20)     8195 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/NIST_Gauss2.dat
+-rw-r--r--   0 Newville   (501) staff       (20)      419 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/README.txt
+-rw-r--r--   0 Newville   (501) staff       (20)     1419 2023-04-01 13:56:41.000000 lmfit-1.2.0/examples/doc_builtinmodels_nistgauss.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1010 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_builtinmodels_nistgauss2.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1364 2023-04-07 18:31:26.000000 lmfit-1.2.0/examples/doc_builtinmodels_peakmodels.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1961 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_builtinmodels_splinemodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      784 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_builtinmodels_stepmodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1964 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_confidence_advanced.py
+-rw-r--r--   0 Newville   (501) staff       (20)      481 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_confidence_basic.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3850 2023-04-01 13:56:41.000000 lmfit-1.2.0/examples/doc_confidence_chi2_maps.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3359 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_fitting_emcee.py
+-rw-r--r--   0 Newville   (501) staff       (20)      969 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_fitting_withreport.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1953 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_composite.py
+-rw-r--r--   0 Newville   (501) staff       (20)      651 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_model_gaussian.py
+-rw-r--r--   0 Newville   (501) staff       (20)      774 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_loadmodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      531 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_loadmodelresult.py
+-rw-r--r--   0 Newville   (501) staff       (20)      537 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_loadmodelresult2.py
+-rw-r--r--   0 Newville   (501) staff       (20)      337 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_model_savemodel.py
+-rw-r--r--   0 Newville   (501) staff       (20)      423 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_model_savemodelresult.py
+-rw-r--r--   0 Newville   (501) staff       (20)      996 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_savemodelresult2.py
+-rw-r--r--   0 Newville   (501) staff       (20)      862 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_two_components.py
+-rw-r--r--   0 Newville   (501) staff       (20)      834 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_model_uncertainty.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3148 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_uncertainty2.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1051 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_model_with_iter_callback.py
+-rw-r--r--   0 Newville   (501) staff       (20)      775 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/doc_model_with_nan_policy.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1499 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_parameters_basic.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1252 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/doc_parameters_valuesdict.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7666 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/example_Model_interface.py
+-rw-r--r--   0 Newville   (501) staff       (20)    17926 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/example_brute.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4731 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/example_complex_resonator_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4378 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/example_confidence_interval.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3331 2023-03-25 15:55:57.000000 lmfit-1.2.0/examples/example_detect_outliers.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1795 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/example_diffev.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4098 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/example_emcee_Model_interface.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1273 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/example_expression_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2716 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/example_fit_multi_datasets.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1417 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/example_fit_with_algebraic_constraint.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2161 2023-04-01 13:56:41.000000 lmfit-1.2.0/examples/example_fit_with_bounds.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2666 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/example_fit_with_derivfunc.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2190 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/example_fit_with_inequality.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2378 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/example_reduce_fcn.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2915 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/example_sympy.py
+-rw-r--r--   0 Newville   (501) staff       (20)     6112 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/example_two_dimensional_peak.py
+-rw-r--r--   0 Newville   (501) staff       (20)      851 2023-04-04 02:16:59.000000 lmfit-1.2.0/examples/example_use_pandas.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7776 2023-03-30 18:04:00.000000 lmfit-1.2.0/examples/lmfit_emcee_model_selection.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2373 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/model1d_gauss.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     1987 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/peak.csv
+-rw-r--r--   0 Newville   (501) staff       (20)     2464 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/sinedata.dat
+-rw-r--r--   0 Newville   (501) staff       (20)     9496 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/test_peak.dat
+-rw-r--r--   0 Newville   (501) staff       (20)    11611 2023-02-23 19:14:07.000000 lmfit-1.2.0/examples/test_splinepeak.dat
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.411539 lmfit-1.2.0/lmfit/
+-rw-r--r--   0 Newville   (501) staff       (20)     1956 2023-03-30 18:04:00.000000 lmfit-1.2.0/lmfit/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)    10016 2023-02-23 19:14:07.000000 lmfit-1.2.0/lmfit/_ampgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)    15312 2023-04-01 13:56:41.000000 lmfit-1.2.0/lmfit/confidence.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4808 2023-02-23 19:14:07.000000 lmfit-1.2.0/lmfit/jsonutils.py
+-rw-r--r--   0 Newville   (501) staff       (20)    16911 2023-02-23 19:14:07.000000 lmfit-1.2.0/lmfit/lineshapes.py
+-rw-r--r--   0 Newville   (501) staff       (20)   105393 2023-04-01 13:56:41.000000 lmfit-1.2.0/lmfit/minimizer.py
+-rw-r--r--   0 Newville   (501) staff       (20)    84175 2023-04-01 14:38:49.000000 lmfit-1.2.0/lmfit/model.py
+-rw-r--r--   0 Newville   (501) staff       (20)    65998 2023-02-24 16:55:16.000000 lmfit-1.2.0/lmfit/models.py
+-rw-r--r--   0 Newville   (501) staff       (20)    36709 2023-04-07 18:31:26.000000 lmfit-1.2.0/lmfit/parameter.py
+-rw-r--r--   0 Newville   (501) staff       (20)    15394 2023-04-01 13:56:41.000000 lmfit-1.2.0/lmfit/printfuncs.py
+-rw-r--r--   0 Newville   (501) staff       (20)      160 2023-04-08 19:48:27.000000 lmfit-1.2.0/lmfit/version.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.412183 lmfit-1.2.0/lmfit.egg-info/
+-rw-r--r--   0 Newville   (501) staff       (20)     5721 2023-04-08 19:48:27.000000 lmfit-1.2.0/lmfit.egg-info/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)     4971 2023-04-08 19:48:27.000000 lmfit-1.2.0/lmfit.egg-info/SOURCES.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        1 2023-04-08 19:48:27.000000 lmfit-1.2.0/lmfit.egg-info/dependency_links.txt
+-rw-r--r--   0 Newville   (501) staff       (20)      685 2023-04-08 19:48:27.000000 lmfit-1.2.0/lmfit.egg-info/requires.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        6 2023-04-08 19:48:27.000000 lmfit-1.2.0/lmfit.egg-info/top_level.txt
+-rwxr-xr-x   0 Newville   (501) staff       (20)     1010 2023-02-23 19:14:07.000000 lmfit-1.2.0/publish_docs.sh
+-rw-r--r--   0 Newville   (501) staff       (20)      202 2023-02-23 19:14:07.000000 lmfit-1.2.0/pyproject.toml
+-rw-r--r--   0 Newville   (501) staff       (20)     2456 2023-04-08 19:48:27.420089 lmfit-1.2.0/setup.cfg
+-rw-r--r--   0 Newville   (501) staff       (20)       92 2023-02-23 19:14:07.000000 lmfit-1.2.0/setup.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2023-04-08 19:48:27.419186 lmfit-1.2.0/tests/
+-rw-r--r--   0 Newville   (501) staff       (20)     6109 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/NISTModels.py
+-rw-r--r--   0 Newville   (501) staff       (20)        0 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)      893 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/conftest.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5656 2023-03-30 18:04:00.000000 lmfit-1.2.0/tests/gauss_modelresult_lmfit100.sav
+-rw-r--r--   0 Newville   (501) staff       (20)     1374 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_1variable.py
+-rw-r--r--   0 Newville   (501) staff       (20)     7097 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_NIST_Strd.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3951 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_algebraic_constraint.py
+-rw-r--r--   0 Newville   (501) staff       (20)     5193 2023-03-30 18:04:00.000000 lmfit-1.2.0/tests/test_ampgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1238 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_basicfit.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3911 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_basinhopping.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1900 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_bounded_jacobian.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1413 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_bounds.py
+-rw-r--r--   0 Newville   (501) staff       (20)    11428 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_brute.py
+-rw-r--r--   0 Newville   (501) staff       (20)    11953 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_builtin_models.py
+-rw-r--r--   0 Newville   (501) staff       (20)     9251 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_confidence.py
+-rw-r--r--   0 Newville   (501) staff       (20)     9987 2023-04-01 13:56:41.000000 lmfit-1.2.0/tests/test_covariance_matrix.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1235 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_custom_independentvar.py
+-rw-r--r--   0 Newville   (501) staff       (20)      612 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_default_kws.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2595 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_dual_annealing.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4364 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_itercb.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3066 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_jsonutils.py
+-rw-r--r--   0 Newville   (501) staff       (20)     6266 2023-03-30 18:04:00.000000 lmfit-1.2.0/tests/test_least_squares.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4804 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_lineshapes.py
+-rw-r--r--   0 Newville   (501) staff       (20)      781 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_manypeaks_speed.py
+-rw-r--r--   0 Newville   (501) staff       (20)     3689 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_max_nfev.py
+-rw-r--r--   0 Newville   (501) staff       (20)      545 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_minimizer.py
+-rw-r--r--   0 Newville   (501) staff       (20)    51749 2023-03-30 18:04:00.000000 lmfit-1.2.0/tests/test_model.py
+-rw-r--r--   0 Newville   (501) staff       (20)    10484 2023-03-30 18:04:00.000000 lmfit-1.2.0/tests/test_model_saveload.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4354 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_model_uncertainties.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4965 2023-03-30 18:04:00.000000 lmfit-1.2.0/tests/test_models.py
+-rw-r--r--   0 Newville   (501) staff       (20)     2181 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_multidatasets.py
+-rw-r--r--   0 Newville   (501) staff       (20)    24031 2023-04-01 13:56:41.000000 lmfit-1.2.0/tests/test_nose.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1168 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_pandas.py
+-rw-r--r--   0 Newville   (501) staff       (20)    19779 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_parameter.py
+-rw-r--r--   0 Newville   (501) staff       (20)    21287 2023-04-07 18:31:26.000000 lmfit-1.2.0/tests/test_parameters.py
+-rw-r--r--   0 Newville   (501) staff       (20)    14990 2023-04-01 13:56:41.000000 lmfit-1.2.0/tests/test_printfuncs.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4784 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_shgo.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1503 2023-02-23 19:14:07.000000 lmfit-1.2.0/tests/test_stepmodel.py
```

### Comparing `lmfit-1.1.0/.github/CONTRIBUTING.md` & `lmfit-1.2.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/.github/ISSUE_TEMPLATE.md` & `lmfit-1.2.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/.github/PULL_REQUEST_TEMPLATE.md` & `lmfit-1.2.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/.pre-commit-config.yaml` & `lmfit-1.2.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 exclude: 'doc/conf.py'
 
 repos:
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.2.2
+    rev: v3.3.1
     hooks:
     -   id: pyupgrade
         args: [--py37-plus]
 
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
@@ -25,37 +25,37 @@
 -   repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
     -   id: flake8
         additional_dependencies: [flake8-deprecated, flake8-mutable]
 
 -   repo: https://github.com/PyCQA/isort/
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
     -   id: isort
 
 -   repo: local
     hooks:
     -   id: rstcheck
         name: rstcheck
         entry: rstcheck --report-level WARNING
         files: '.rst'
         language: python
         additional_dependencies: [rstcheck, sphinx]
 
 -   repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
     -   id: rst-backticks
     -   id: rst-directive-colons
     -   id: rst-inline-touching-normal
     -   id: python-check-blanket-noqa
 
 -   repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
     -   id: codespell
         files: '.py|.rst'
         exclude: 'doc/doc_examples_to_gallery.py'
         # escaped characters currently do not work correctly
         # so \nnumber is considered a spelling error....
         args: ["-L nnumber", "-L mone"]
```

### Comparing `lmfit-1.1.0/AUTHORS.txt` & `lmfit-1.2.0/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/LICENSE` & `lmfit-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Bennett5.dat` & `lmfit-1.2.0/NIST_STRD/Bennett5.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/BoxBOD.dat` & `lmfit-1.2.0/NIST_STRD/BoxBOD.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Chwirut1.dat` & `lmfit-1.2.0/NIST_STRD/Chwirut1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Chwirut2.dat` & `lmfit-1.2.0/NIST_STRD/Chwirut2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/DanWood.dat` & `lmfit-1.2.0/NIST_STRD/DanWood.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/ENSO.dat` & `lmfit-1.2.0/NIST_STRD/ENSO.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Eckerle4.dat` & `lmfit-1.2.0/NIST_STRD/Eckerle4.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Gauss1.dat` & `lmfit-1.2.0/NIST_STRD/Gauss1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Gauss2.dat` & `lmfit-1.2.0/NIST_STRD/Gauss2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Gauss3.dat` & `lmfit-1.2.0/NIST_STRD/Gauss3.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Hahn1.dat` & `lmfit-1.2.0/NIST_STRD/Hahn1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Kirby2.dat` & `lmfit-1.2.0/NIST_STRD/Kirby2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Lanczos1.dat` & `lmfit-1.2.0/NIST_STRD/Lanczos1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Lanczos2.dat` & `lmfit-1.2.0/NIST_STRD/Lanczos2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Lanczos3.dat` & `lmfit-1.2.0/NIST_STRD/Lanczos3.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/MGH09.dat` & `lmfit-1.2.0/NIST_STRD/MGH09.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/MGH10.dat` & `lmfit-1.2.0/NIST_STRD/MGH10.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/MGH17.dat` & `lmfit-1.2.0/NIST_STRD/MGH17.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Misra1a.dat` & `lmfit-1.2.0/NIST_STRD/Misra1a.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Misra1b.dat` & `lmfit-1.2.0/NIST_STRD/Misra1b.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Misra1c.dat` & `lmfit-1.2.0/NIST_STRD/Misra1c.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Misra1d.dat` & `lmfit-1.2.0/NIST_STRD/Misra1d.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Models` & `lmfit-1.2.0/NIST_STRD/Models`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Nelson.dat` & `lmfit-1.2.0/NIST_STRD/Nelson.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Rat42.dat` & `lmfit-1.2.0/NIST_STRD/Rat42.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Rat43.dat` & `lmfit-1.2.0/NIST_STRD/Rat43.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Roszman1.dat` & `lmfit-1.2.0/NIST_STRD/Roszman1.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/NIST_STRD/Thurber.dat` & `lmfit-1.2.0/NIST_STRD/Thurber.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/PKG-INFO` & `lmfit-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmfit
-Version: 1.1.0
+Version: 1.2.0
 Summary: Least-Squares Minimization with Bounds and Constraints
 Home-page: https://lmfit.github.io//lmfit-py/
 Author: LMFit Development Team
 Author-email: matt.newville@gmail.com
 License: BSD 3-Clause
 Project-URL: Source, https://github.com/lmfit/lmfit-py
 Project-URL: Changelog, https://lmfit.github.io/lmfit-py/whatsnew.html
```

### Comparing `lmfit-1.1.0/README.rst` & `lmfit-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/asv_benchmarking/asv.conf.json` & `lmfit-1.2.0/asv_benchmarking/asv.conf.json`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/asv_benchmarking/benchmarks/benchmarks.py` & `lmfit-1.2.0/asv_benchmarking/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/azure-pipelines.yml` & `lmfit-1.2.0/azure-pipelines.yml`

 * *Files 1% similar despite different names*

```diff
@@ -257,27 +257,27 @@
             ##curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
             ##python3.12 get-pip.py --user
             python3.12 -m ensurepip --upgrade
             pip3.12 install -U build pip setuptools wheel pybind11 cython || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install build, pip, setuptools, wheel, pybind11, and cython'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
-            export numpy_version=1.23.5
+            export numpy_version=1.24.1
             wget https://github.com/numpy/numpy/releases/download/v${numpy_version}/numpy-${numpy_version}.tar.gz
             tar xzvf numpy-${numpy_version}.tar.gz
             cd numpy-${numpy_version}
             python3.12 setup.py install --user || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install latest available version of NumPy'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
             pip3.12 install -U pythran || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install pythran'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
-            export scipy_version=1.9.3
+            export scipy_version=1.10.0
             wget https://github.com/scipy/scipy/releases/download/v${scipy_version}/scipy-${scipy_version}.tar.gz
             tar xzvf scipy-${scipy_version}.tar.gz
             cd scipy-${scipy_version}
             python3.12 setup.py install --user || echo -e "\043#vso[task.logissue type=warning;] Allowed failure for development version!!"
           displayName: 'Install latest available version of SciPy'
         - script: |
             export PATH=/home/vsts/.local/bin:$PATH
```

### Comparing `lmfit-1.1.0/doc/Makefile` & `lmfit-1.2.0/doc/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 .PHONY: help clean html dirhtml pickle json htmlhelp qthelp latex changes linkcheck doctest latexpdf htmlzip
 .PHONY: all pdf gallery debug
 
 html:  gallery
 	cp sphinx/ext_mathjax.py extensions.py
 	$(SPHINXBUILD) -b html $(SPHINX_OUTPUT) $(SPHINX_OPTS) . $(BUILDDIR)/html
-	./filter_spurious_link_from_html.py
 	@echo
 	@echo "html build finished: $(BUILDDIR)/html."
 
 debug:  gallery
 	cp sphinx/ext_mathjax.py extensions.py
 	$(SPHINXBUILD) -b html $(SPHINX_OUTPUT) $(SPHINX_DEBUGOPTS) . $(BUILDDIR)/html
 	@echo
@@ -34,15 +33,14 @@
 
 examples/index.rst:
 	./doc_examples_to_gallery.py
 
 htmlzip: html
 	cp sphinx/ext_mathjax.py extensions.py
 	$(SPHINXBUILD) -b html $(SPHINX_OUTPUT) $(SPHINX_OPTS) . $(BUILDDIR)/lmfit_doc
-	./filter_spurious_link_from_html.py
 	cd $(BUILDDIR) && zip -pur html/lmfit_doc.zip lmfit_doc
 
 epub: gallery
 	cp sphinx/ext_imgmath.py extensions.py
 	$(SPHINXBUILD) -b epub  $(SPHINX_OUTPUT) $(SPHINX_OPTS) . $(BUILDDIR)/epub
 	mkdir -p $(BUILDDIR)/html
 	cp -pr $(BUILDDIR)/epub/*.epub $(BUILDDIR)/html/.
```

### Comparing `lmfit-1.1.0/doc/_templates/indexsidebar.html` & `lmfit-1.2.0/doc/_templates/indexsidebar.html`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/doc/bounds.rst` & `lmfit-1.2.0/doc/bounds.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/doc/builtin_models.rst` & `lmfit-1.2.0/doc/builtin_models.rst`

 * *Files 0% similar despite different names*

```diff
@@ -402,14 +402,15 @@
 shape, with longer tails, should be used. Perhaps a Lorentzian would be
 better? To do this, we simply replace ``GaussianModel`` with
 ``LorentzianModel`` to get a :class:`LorentzianModel`:
 
 .. jupyter-execute::
 
     from lmfit.models import LorentzianModel
+
     mod = LorentzianModel()
 
 with the rest of the script as above. Perhaps predictably, the first thing
 we try gives results that are worse by comparing the fit statistics:
 
 .. jupyter-execute::
     :hide-code:
@@ -430,14 +431,15 @@
 
 The tails are now too big, and the value for :math:`\chi^2` almost doubled.
 A Voigt model does a better job. Using :class:`VoigtModel`, this is as simple as using:
 
 .. jupyter-execute::
 
     from lmfit.models import VoigtModel
+
     mod = VoigtModel()
 
 with all the rest of the script as above. This gives:
 
 .. jupyter-execute::
     :hide-code:
 
@@ -613,14 +615,15 @@
 
     def index_of(arrval, value):
 	"""Return index of array *at or below* value."""
 	if value < min(arrval):
 	    return 0
 	return max(np.where(arrval <= value)[0])
 
+
     ix1 = index_of(x, 75)
     ix2 = index_of(x, 135)
     ix3 = index_of(x, 175)
 
     exp_mod.guess(y[:ix1], x=x[:ix1])
     gauss1.guess(y[ix1:ix2], x=x[ix1:ix2])
     gauss2.guess(y[ix2:ix3], x=x[ix2:ix3])
```

### Comparing `lmfit-1.1.0/doc/conf.py` & `lmfit-1.2.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/doc/constraints.rst` & `lmfit-1.2.0/doc/constraints.rst`

 * *Files 1% similar despite different names*

```diff
@@ -191,17 +191,19 @@
 
 and then initialize the :class:`Minimizer` class with this parameter set:
 
 .. jupyter-execute::
 
     from lmfit import Minimizer
 
+
     def userfcn(x, params):
         pass
 
+
     fitter = Minimizer(userfcn, pars)
 
 Alternatively, one can first initialize the :class:`Minimizer` class and
 add the function to the `asteval`_ interpreter of :attr:`Minimizer.params`
 afterwards:
 
 .. jupyter-execute::
```

### Comparing `lmfit-1.1.0/doc/doc_examples_to_gallery.py` & `lmfit-1.2.0/doc/doc_examples_to_gallery.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/doc/faq.rst` & `lmfit-1.2.0/doc/faq.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/doc/filter_spurious_link_from_html.py` & `lmfit-1.2.0/doc/filter_spurious_link_from_html.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/doc/fitting.rst` & `lmfit-1.2.0/doc/fitting.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/doc/index.rst` & `lmfit-1.2.0/doc/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
   * Many :ref:`built-in models <builtin_models_chapter>` for common
     lineshapes are included and ready to use.
 
 The lmfit package is Free software, using an Open Source license. The
 software and this document are works in progress. If you are interested in
 participating in this effort please use the `lmfit GitHub repository`_.
 
-
 .. toctree::
    :maxdepth: 2
 
    intro
    installation
    support
    faq
```

### Comparing `lmfit-1.1.0/doc/installation.rst` & `lmfit-1.2.0/doc/installation.rst`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 .. _asteval: https://github.com/newville/asteval
 .. _uncertainties: https://github.com/lebigot/uncertainties
 .. _numdifftools: https://github.com/pbrod/numdifftools
 .. _contributing.md: https://github.com/lmfit/lmfit-py/blob/master/.github/CONTRIBUTING.md
 .. _corner: https://github.com/dfm/corner.py
 .. _sphinx: https://www.sphinx-doc.org
 .. _jupyter_sphinx: https://jupyter-sphinx.readthedocs.io
+.. _ipykernel: https://github.com/ipython/ipykernel
 .. _sphinxcontrib-svg2pdfconverter: https://github.com/missinglinkelectronics/sphinxcontrib-svg2pdfconverter
 .. _cairosvg: https://cairosvg.org/
 .. _Pillow: https://python-pillow.org/
 .. _sphinx-gallery: https://sphinx-gallery.github.io/stable/index.html
 .. _flaky: https://github.com/box/flaky
 .. _SymPy: https://www.sympy.org/
 .. _Latexmk: https://ctan.org/pkg/latexmk/
@@ -47,16 +48,16 @@
 packages are required. Some functionality requires the `emcee`_ (version 3+),
 `corner`_, `pandas`_, `Jupyter`_, `matplotlib`_, `dill`_, or `numdifftools`_
 packages. These are not installed automatically, but we highly recommend each
 of them.
 
 For building the documentation and generating the examples gallery, `matplotlib`_,
 `emcee`_ (version 3+), `corner`_, `Sphinx`_, `sphinx-gallery`_, `jupyter_sphinx`_,
-`Pillow`_, and `SymPy`_ are required. For generating the PDF documentation, the Python
-packages `sphinxcontrib-svg2pdfconverter`_ and `cairosvg`_ are also required,
+`ipykernel`_, `Pillow`_, and `SymPy`_ are required. For generating the PDF documentation,
+the Python packages `sphinxcontrib-svg2pdfconverter`_ and `cairosvg`_ are also required,
 as well as the LaTex package `Latexmk`_ (which is included by default in some
 LaTex distributions).
 
 Please refer to ``setup.cfg`` under ``options.extras_require`` for a list of all
 dependencies that are needed if you want to participate in the development of lmfit.
 You can install all these dependencies automatically by doing ``pip install lmfit[all]``,
 or select only a subset (e.g., ``dev```, ``doc``, or ``test``).
```

### Comparing `lmfit-1.1.0/doc/intro.rst` & `lmfit-1.2.0/doc/intro.rst`

 * *Files 26% similar despite different names*

```diff
@@ -76,46 +76,48 @@
 Though it is wonderful to be able to use Python for such optimization
 problems, and the SciPy library is robust and easy to use, the approach
 here is not terribly different from how one would do the same fit in C or
 Fortran. There are several practical challenges to using this approach,
 including:
 
   a) The user has to keep track of the order of the variables, and their
-     meaning -- ``variables[0]`` is the ``amplitude``, ``variables[2]`` is
-     the ``frequency``, and so on, although there is no intrinsic meaning
-     to this order.
-
-  b) If the user wants to fix a particular variable (*not* vary it in the
-     fit), the residual function has to be altered to have fewer variables,
-     and have the corresponding constant value passed in some other way.
-     While reasonable for simple cases, this quickly becomes a significant
-     work for more complex models, and greatly complicates modeling for
-     people not intimately familiar with the details of the fitting code.
-
-  c) There is no simple, robust way to put bounds on values for the
-     variables, or enforce mathematical relationships between the
-     variables. In fact, the optimization methods that do provide
-     bounds, require bounds to be set for all variables with separate
-     arrays that are in the same arbitrary order as variable values.
-     Again, this is acceptable for small or one-off cases, but becomes
-     painful if the fitting model needs to change.
-
-These shortcomings are due to the use of traditional arrays to hold the
-variables, which matches closely the implementation of the underlying
-Fortran code, but does not fit very well with Python's rich selection of
-objects and data structures. The key concept in lmfit is to define and use
-:class:`Parameter` objects instead of plain floating point numbers as the
-variables for the fit. Using :class:`Parameter` objects (or the closely
-related :class:`Parameters` -- a dictionary of :class:`Parameter` objects),
-allows one to:
+     meaning -- ``variables[0]`` is the ``amplitude``, ``variables[2]`` is the
+     ``frequency``, and so on, although there is no intrinsic meaning to this
+     order.
+  b) If the user wants to fix a particular variable (*not* vary it in the fit),
+     the residual function has to be altered to have fewer variables, and have
+     the corresponding constant value passed in some other way. While
+     reasonable for simple cases, this quickly becomes a significant work for
+     more complex models, and greatly complicates modeling for people not
+     intimately familiar with the details of the fitting code.
+  c) There is no simple, robust way to put bounds on values for the variables,
+     or enforce mathematical relationships between the variables. While some
+     optimization methods in SciPy do provide bounds, they require bounds to
+     be set for all variables with separate arrays that are in the same
+     arbitrary order as variable values. Again, this is acceptable for small
+     or one-off cases, but becomes painful if the fitting model needs to
+     change.
+  d) In some cases, constraints can be placed on Parameter values, but this is
+     a pretty opaque and complex process.
+
+While these shortcomings can be worked around with some work, they are all
+essentially due to the use of arrays or lists to hold the variables.
+This closely matches the implementation of the underlying Fortran code, but
+does not fit very well with Python's rich selection of objects and data
+structures. The key concept in lmfit is to define and use :class:`Parameter`
+objects instead of plain floating point numbers as the variables for the
+fit. Using :class:`Parameter` objects (or the closely related
+:class:`Parameters` -- a dictionary of :class:`Parameter` objects), allows one
+to do the following:
 
    a) forget about the order of variables and refer to Parameters
       by meaningful names.
    b) place bounds on Parameters as attributes, without worrying about
-      preserving the order of arrays for variables and boundaries.
+      preserving the order of arrays for variables and boundaries, and without
+      relying on the solver to support bounds itself.
    c) fix Parameters, without having to rewrite the objective function.
    d) place algebraic constraints on Parameters.
 
 To illustrate the value of this approach, we can rewrite the above example
 for the decaying sine wave as:
 
 .. jupyter-execute::
@@ -140,47 +142,79 @@
     params.add('amp', value=10)
     params.add('decay', value=0.007)
     params.add('phase', value=0.2)
     params.add('frequency', value=3.0)
 
     out = minimize(residual, params, args=(x, data, uncertainty))
 
-At first look, we simply replaced a list of values with a dictionary,
-accessed by name -- not a huge improvement. But each of the named
-:class:`Parameter` in the :class:`Parameters` object holds additional
-attributes to modify the value during the fit. For example, Parameters can
-be fixed or bounded. This can be done during definition:
+
+At first look, we simply replaced a list of values with a dictionary, so that
+we can access Parameters by name. Just by itself, this is better as it allows
+separation of the objective function from the code using it.
+
+Note that creation of Parameters here could also be done as:
+
+.. versionadded:: 1.2.0
 
 .. jupyter-execute::
 
-    params = Parameters()
-    params.add('amp', value=10, vary=False)
-    params.add('decay', value=0.007, min=0.0)
-    params.add('phase', value=0.2)
-    params.add('frequency', value=3.0, max=10)
+    from lmfit import create_params
+
+    params = create_params(amp=10, decay=0.007, phase=0.2, frequency=3.0)
+
+
+where keyword/value pairs set Parameter names and their initial values.
+
+Either when using :func:`create_param` or :class:`Parameters`, the resulting
+``params`` object is an instance of :class:`Parameters`, which acts like a
+dictionary, with keys being the Parameter name and values being individual
+:class:`Parameter` objects. These :class:`Parameter` objects hold the value
+and several other attributes that control how a Parameter acts. For example,
+Parameters can be fixed or bounded; setting attributes to control this
+behavior can be done during definition, as with:
+
+
+.. jupyter-execute::
+
+   params = Parameters()
+   params.add('amp', value=10, vary=False)
+   params.add('decay', value=0.007, min=0.0)
+   params.add('phase', value=0.2)
+   params.add('frequency', value=3.0, max=10)
+
+
+Here ``vary=False`` will prevent the value from changing in the fit, and
+``min=0.0`` will set a lower bound on that parameter's value. The same thing
+can be accomplished by providing a dictionary of attribute values to
+:func:`create_params`:
+
+.. versionadded:: 1.2.0
+
+.. jupyter-execute::
+
+   params = create_params(amp={'value': 10, 'vary': False},
+                          decay={'value': 0.007, 'min': 0},
+                          phase=0.2,
+                          frequency={'value': 3.0, 'max':10})
 
-where ``vary=False`` will prevent the value from changing in the fit, and
-``min=0.0`` will set a lower bound on that parameter's value. It can also
-be done later by setting the corresponding attributes after they have been
-created:
+Parameter attributes can also be modified after they have been created:
 
 .. jupyter-execute::
 
     params['amp'].vary = False
     params['decay'].min = 0.10
 
-Importantly, our objective function remains unchanged. This means the
-objective function can simply express the parametrized phenomenon to be
-modeled, and is separate from the choice of parameters to be varied in the
-fit.
+Importantly, our objective function remains unchanged. This means the objective
+function can simply express the parametrized phenomenon to be calculated,
+accessing Parameter values by name and separating the choice of parameters to
+be varied in the fit.
 
 The ``params`` object can be copied and modified to make many user-level
-changes to the model and fitting process. Of course, most of the
-information about how your data is modeled goes into the objective
-function, but the approach here allows some external control; that is,
-control by the **user** performing the fit, instead of by the author of the
-objective function.
-
-Finally, in addition to the :class:`Parameters` approach to fitting data,
-lmfit allows switching optimization methods without changing the objective
-function, provides tools for generating fitting reports, and provides a
-better determination of Parameters confidence levels.
+changes to the model and fitting process. Of course, most of the information
+about how your data is modeled goes into the objective function, but the
+approach here allows some external control; that is, control by the **user**
+performing the fit, instead of by the author of the objective function.
+
+Finally, in addition to the :class:`Parameters` approach to fitting data, lmfit
+allows switching optimization methods without changing the objective function,
+provides tools for generating fitting reports, and provides a better
+determination of Parameters confidence levels.
```

### Comparing `lmfit-1.1.0/doc/make.bat` & `lmfit-1.2.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/doc/model.rst` & `lmfit-1.2.0/doc/model.rst`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     %matplotlib inline
     %config InlineBackend.figure_format = 'svg'
 
 .. jupyter-execute::
 
     from numpy import exp, linspace, random
 
+
     def gaussian(x, amp, cen, wid):
         return amp * exp(-(x-cen)**2 / wid)
 
 We want to use this function to fit to data :math:`y(x)` represented by the
 arrays ``y`` and ``x``.  With :scipydoc:`optimize.curve_fit`, this would be:
 
 .. jupyter-execute::
@@ -103,29 +104,31 @@
 independent variable is ``x``, and the parameters are named ``amp``,
 ``cen``, and ``wid``, and -- all taken directly from the signature of the
 model function. As we will see below, you can modify the default
 assignment of independent variable / arguments and specify yourself what
 the independent variable is and which function arguments should be identified
 as parameter names.
 
-The Parameters are *not* created when the model is created. The model knows
-what the parameters should be named, but nothing about the scale and
-range of your data. You will normally have to make these parameters and
-assign initial values and other attributes. To help you do this, each
-model has a :meth:`make_params` method that will generate parameters with
-the expected names:
+:class:`~lmfit.parameter.Parameters` are *not* created when the model is
+created. The model knows what the parameters should be named, but nothing about
+the scale and range of your data. To help you create Parameters for a Model,
+each model has a :meth:`make_params` method that will generate parameters with
+the expected names. You will have to do this, or make Parameters some other way
+(say, with :func:`~lmfit.parameter.create_params`), and assign initial values
+for all Parameters. You can also assign other attributes when doing this:
 
 .. jupyter-execute::
 
     params = gmodel.make_params()
 
 This creates the :class:`~lmfit.parameter.Parameters` but does not
 automatically give them initial values since it has no idea what the scale
-should be. You can set initial values for parameters with keyword
-arguments to :meth:`make_params`:
+should be. If left unspecified, the initial values will be ``-Inf``, which will
+generally fail to give useful results. You can set initial values for
+parameters with keyword arguments to :meth:`make_params`:
 
 .. jupyter-execute::
 
     params = gmodel.make_params(cen=0.3, amp=3, wid=1.25)
 
 or assign them (and other parameter properties) after the
 :class:`~lmfit.parameter.Parameters` class has been created.
@@ -227,20 +230,18 @@
 
 .. automethod:: Model.fit
 
 .. automethod:: Model.guess
 
 .. automethod:: Model.make_params
 
-
 .. automethod:: Model.set_param_hint
 
    See :ref:`model_param_hints_section`.
 
-
 .. automethod:: Model.print_param_hints
 
 
 :class:`Model` class Attributes
 -------------------------------
 
 .. attribute:: func
@@ -290,18 +291,17 @@
    ``g1_amplitude``, ``g1_center``, and ``g1_sigma``. This can be
    essential to avoid name collision in composite models.
 
 
 Determining parameter names and independent variables for a function
 --------------------------------------------------------------------
 
-The :class:`Model` created from the supplied function ``func`` will create
-a :class:`~lmfit.parameter.Parameters` object, and names are inferred from the function
-arguments, and a residual function is automatically constructed.
-
+The :class:`Model` created from the supplied function ``func`` will create a
+:class:`~lmfit.parameter.Parameters` object, and names are inferred from the
+function` arguments, and a residual function is automatically constructed.
 
 By default, the independent variable is taken as the first argument to the
 function. You can, of course, explicitly set this, and will need to do so
 if the independent variable is not first in the list, or if there is actually
 more than one independent variable.
 
 If not specified, Parameters are constructed from all positional arguments
@@ -380,14 +380,15 @@
     def decay2(t, tau, N=10, check_positive=False):
         if check_positive:
             arg = abs(t)/max(1.e-9, abs(tau))
         else:
             arg = t/tau
         return N*np.exp(arg)
 
+
     mod = Model(decay2)
     params = mod.make_params()
     print('Parameters:')
     for pname, par in params.items():
         print(pname, par)
 
 Here, even though ``N`` is a keyword argument to the function, it is turned
@@ -424,31 +425,37 @@
     for pname, par in params.items():
         print(pname, par)
 
 You would refer to these parameters as ``f1_amplitude`` and so forth, and
 the model will know to map these to the ``amplitude`` argument of ``myfunc``.
 
 
-Initializing model parameters
------------------------------
+Initializing model parameter values
+-----------------------------------
 
-As mentioned above, the parameters created by :meth:`Model.make_params` are
-generally created with invalid initial values of ``None``. These values
-**must** be initialized in order for the model to be evaluated or used in a
-fit. There are four different ways to do this initialization that can be
-used in any combination:
+As mentioned above, creating a model does not automatically create the
+corresponding :class:`~lmfit.parameter.Parameters`. These can be created with
+either the :func:`create_params` function, or the :meth:`Model.make_params`
+method of the corresponding instance of :class:`Model`.
+
+When creating Parameters, each parameter is created with invalid initial value
+of ``-Inf`` if it is not set explicitly. That is to say, parameter values
+**must** be initialized in order for the model to evaluate a finite result or
+used in a fit. There are a few different ways to do this:
 
   1. You can supply initial values in the definition of the model function.
   2. You can initialize the parameters when creating parameters with :meth:`Model.make_params`.
-  3. You can give parameter hints with :meth:`Model.set_param_hint`.
-  4. You can supply initial values for the parameters when you use the
+  3. You can create a Parameters object with :class:`Parameters` or :func:`create_params`.
+  4. You can supply initial values for the parameters when calling
      :meth:`Model.eval` or :meth:`Model.fit` methods.
 
-Of course these methods can be mixed, allowing you to overwrite initial
-values at any point in the process of defining and using the model.
+Generally, using the :meth:`Model.make_params` method is recommended. The methods
+described above can be mixed, allowing you to overwrite initial values at any point
+in the process of defining and using the model.
+
 
 Initializing values in the function definition
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 To supply initial values for parameters in the definition of the model
 function, you can simply supply a default value:
 
@@ -469,46 +476,58 @@
 initial value will always be available for the parameter.
 
 
 Initializing values with :meth:`Model.make_params`
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 When creating parameters with :meth:`Model.make_params` you can specify initial
-values. To do this, use keyword arguments for the parameter names and
-initial values:
+values. To do this, use keyword arguments for the parameter names. You can
+either set initial values as numbers (floats or ints) or as dictionaries with
+keywords of (``value``, ``vary``, ``min``, ``max``, ``expr``, ``brute_step``,
+and ``is_init_value``) to specify these parameter attributes.
 
 .. jupyter-execute::
 
     mod = Model(myfunc)
+
+    # simply supply initial values
     pars = mod.make_params(a=3, b=0.5)
 
+    # supply initial values, attributes for bounds, etcetera:
+    pars_bounded = mod.make_params(a=dict(value=3, min=0),
+                                   b=dict(value=0.5, vary=False))
+
 
-Initializing values by setting parameter hints
+Creating a :class:`Parameters` object directly
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-After a model has been created, but prior to creating parameters with
-:meth:`Model.make_params`, you can set parameter hints. These allows you to set
-not only a default initial value but also to set other parameter attributes
-controlling bounds, whether it is varied in the fit, or a constraint
-expression. To set a parameter hint, you can use :meth:`Model.set_param_hint`,
-as with:
+You can also create your own Parameters directly using :func:`create_params`.
+This is independent of using the :class:`Model` class, but is essentially
+equivalent to :meth:`Model.make_params` except with less checking of errors for
+model prefixes and so on.
 
 .. jupyter-execute::
 
+    from lmfit import create_params
+
     mod = Model(myfunc)
-    mod.set_param_hint('a', value=1.0)
-    mod.set_param_hint('b', value=0.3, min=0, max=1.0)
-    pars = mod.make_params()
 
-Parameter hints are discussed in more detail in section
-:ref:`model_param_hints_section`.
+    # simply supply initial values
+    pars = create_params(a=3, b=0.5)
+
+    # supply initial values and attributes for bounds, etc:
+    pars_bounded = create_params(a=dict(value=3, min=0),
+                                 b=dict(value=0.5, vary=False))
 
+Because less error checking is done, :meth:`Model.make_params` should probably
+be preferred when using Models.
 
-Initializing values when using a model
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Initializing parameter values for a model with keyword arguments
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Finally, you can explicitly supply initial values when using a model. That
 is, as with :meth:`Model.make_params`, you can include values as keyword
 arguments to either the :meth:`Model.eval` or :meth:`Model.fit` methods:
 
 .. jupyter-execute::
 
@@ -523,49 +542,118 @@
 :meth:`Model.fit`.
 
 .. _model_param_hints_section:
 
 Using parameter hints
 ---------------------
 
-After a model has been created, you can give it hints for how to create
-parameters with :meth:`Model.make_params`.  This allows you to set not only a
-default initial value but also to set other parameter attributes
-controlling bounds, whether it is varied in the fit, or a constraint
-expression. To set a parameter hint, you can use :meth:`Model.set_param_hint`,
+After a model has been created, but prior to creating parameters with
+:meth:`Model.make_params`, you can define parameter hints for that model. This
+allows you to set other parameter attributes for bounds, whether it is varied in
+the fit, or set a default constraint expression for a parameter. You can also
+set the initial value, but that is not really the intention of the method,
+which is to really to let you say that about the idealized Model, for example
+that some values may not make sense for some parameters, or that some parameters
+might be a small change from another parameter and so be fixed or constrained
+by default.
+
+To set a parameter hint, you can use :meth:`Model.set_param_hint`,
 as with:
 
 .. jupyter-execute::
 
     mod = Model(myfunc)
-    mod.set_param_hint('a', value=1.0)
-    mod.set_param_hint('b', value=0.3, min=0, max=1.0)
+    mod.set_param_hint('bounded_parameter', min=0, max=1.0)
+    pars = mod.make_params()
+
+Parameter hints are discussed in more detail in section
+:ref:`model_param_hints_section`.
 
 Parameter hints are stored in a model's :attr:`param_hints` attribute,
 which is simply a nested dictionary:
 
 .. jupyter-execute::
 
     print('Parameter hints:')
     for pname, par in mod.param_hints.items():
         print(pname, par)
 
-You can change this dictionary directly, or with the :meth:`Model.set_param_hint`
+You can change this dictionary directly or use the :meth:`Model.set_param_hint`
 method. Either way, these parameter hints are used by :meth:`Model.make_params`
 when making parameters.
 
-An important feature of parameter hints is that you can force the creation
-of new parameters with parameter hints. This can be useful to make derived
-parameters with constraint expressions. For example to get the full-width
-at half maximum of a Gaussian model, one could use a parameter hint of:
+Parameter hints also allow you to create new parameters. This can be useful to
+make derived parameters with constraint expressions. For example to get the
+full-width at half maximum of a Gaussian model, one could use a parameter hint
+of:
 
 .. jupyter-execute::
 
     mod = Model(gaussian)
-    mod.set_param_hint('fwhm', expr='2.3548*sigma')
+    mod.set_param_hint('wid', min=0)
+    mod.set_param_hint('fwhm', expr='2.3548*wid')
+    params = mod.make_params(amp={'value': 10, 'min':0.1, 'max':2000},
+                             cen=5.5, wid=1.25)
+    params.pretty_print()
+
+With that definition, the value (and uncertainty) of the ``fwhm`` parameter
+will be reported in the output of any fit done with that model.
+
+.. _model_data_coercion_section:
+
+Data Types for data  and independent data with ``Model``
+-------------------------------------------------------------
+
+The model as defined by your model function will use the independent
+variable(s) you specify to best match the data you provide.  The model is meant
+to be an abstract representation for data, but when you do a fit with
+:meth:`Model.fit`, you really need to pass in values for the data to be modeled
+and the independent data used to calculate that data.
+
+The mathematical solvers used by ``lmfit`` all work exclusively with
+1-dimensional numpy arrays of datatype (dtype) ``float64``.  The value of the
+calculation ``(model-data)*weights`` using the calculation of your model
+function, and the data and weights you pass in *will be coerced* to an
+1-dimensional ndarray with dtype ``float64`` when it is passed to the solver.
+
+If the data you pass to :meth:`Model.fit` is not an ndarray of dtype
+``float64`` but is instead a tuples of numbers, a list of numbers, or a
+``pandas.Series``, it will be coerced into an ndarray.  If your data is a list,
+tuple, or Series of complex numbers, it *will be coerced* to an ndarray with
+dtype ``complex128``.
+
+If your data is a numpy array of dtype ``float32``, it *will not be coerced* to
+``float64``, as we assume this was an intentional choice.  That may make all of
+the calculations done in your model function be in single-precision which may
+make fits less sensitive, but the values will be converted to ``float64``
+before being sent to the solver, so the fit should work.
+
+The independent data for models using ``Model`` are meant to be truly
+independent, and not **not** required to be strictly numerical or objects that
+are easily converted to arrays of numbers.  That is, independent data for a
+model could be a dictionary, an instance of a user-defined class, or other type
+of structured data.  You can use independent data any way you want in your
+model function.
+
+But, as with almost all the examples given here, independent data is often also
+a 1-dimensonal array of values, say ``x``, and a simple view of the fit would be
+to plot the data as ``y`` as a function of ``x``.  Again, this is not required, but
+it is very common.  Because of this very common usage, if your independent data
+is a tuple or list of numbers or ``pandas.Series``, it *will be coerced* to be
+an ndarray of dtype ``float64``.  But as with the primary data, if your
+independent data is an ndarray of some different dtype (``float32``,
+``uint16``, etc), it *will not be coerced* to ``float64``, as we assume this
+was intentional.
+
+.. note::
+
+  Data and independent data that are tuples or lists of numbers, or
+  ``panda.Series`` will be coerced to an ndarray of dtype ``float64`` before
+  passing to the model function.  Data with other dtypes (or independent data
+  of other object types such as dicts) will not be coerced to ``float64``.
 
 
 .. _model_saveload_sec:
 
 Saving and Loading Models
 -------------------------
 
@@ -658,14 +746,16 @@
 
 .. automethod:: ModelResult.eval_components
 
 .. automethod:: ModelResult.fit
 
 .. automethod:: ModelResult.fit_report
 
+.. automethod:: ModelResult.summary
+
 .. automethod:: ModelResult.conf_interval
 
 .. automethod:: ModelResult.ci_report
 
 .. automethod:: ModelResult.eval_uncertainty
 
 .. automethod:: ModelResult.plot
```

### Comparing `lmfit-1.1.0/doc/parameters.rst` & `lmfit-1.2.0/doc/parameters.rst`

 * *Files 6% similar despite different names*

```diff
@@ -87,14 +87,26 @@
 
    Saving Parameters with user-added functions to the ``_asteval``
    interpreter using :meth::`dump` and :meth:`dumps` may not be easily
    recovered with the :meth:`load` and :meth:`loads`. See
    :ref:`model_saveload_sec` for further discussion.
 
 
+The :func:`create_params` function
+==================================
+
+The :func:`create_params` function is probably the easiest method for making
+:class:`Parameters` objects, as it allows defining Parameter names by keyword
+with values either being the numerical initial value for the Parameter or being
+a dictionary with keyword/value pairs for ``value`` as well as other Parameter
+attribute such as ``min``, ``max``, ``expr``, and so forth.
+
+.. autofunction:: create_params
+
+
 Simple Example
 ==============
 
 A basic example making use of :class:`~lmfit.parameter.Parameters` and the
 :func:`~lmfit.minimizer.minimize` function (discussed in the next chapter)
 might look like this:
```

### Comparing `lmfit-1.1.0/doc/sphinx/theme/sphinx13/basic_layout.html` & `lmfit-1.2.0/doc/sphinx/theme/sphinx13/basic_layout.html`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/doc/sphinx/theme/sphinx13/layout.html` & `lmfit-1.2.0/doc/sphinx/theme/sphinx13/layout.html`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/doc/sphinx/theme/sphinx13/static/lmfitheader.png` & `lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/lmfitheader.png`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/doc/sphinx/theme/sphinx13/static/sphinx13.css` & `lmfit-1.2.0/doc/sphinx/theme/sphinx13/static/sphinx13.css`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/doc/support.rst` & `lmfit-1.2.0/doc/support.rst`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/doc/whatsnew.rst` & `lmfit-1.2.0/doc/whatsnew.rst`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,49 @@
 .. _lmfit GitHub repository: https://github.com/lmfit/lmfit-py
 
 This section discusses changes between versions, especially changes
 significant to the use and behavior of the library. This is not meant
 to be a comprehensive list of changes. For such a complete record,
 consult the `lmfit GitHub repository`_.
 
+.. _whatsnew_120_label:
+
+Version 1.2.0 Release Notes (April 05, 2023)
+=================================================
+
+New features:
+
+- add ``create_params`` function (PR #844)
+- add ``chi2_out`` and ``nsigma`` options to ``conf_interval2d()``
+- add ``ModelResult.summary()`` to return many resulting fit statistics and attributes into a JSON-able dict.
+- add ``correl_table()`` function to ``lmfit.printfuncs`` and ``correl_mode`` option to ``fit_report()`` and
+  ``ModelResult.fit_report()`` to optionally display a RST-formatted table of a correlation matrix.
+
+Bug fixes/enhancements:
+
+- fix bug when setting ``param.vary=True`` for a constrained parameter (Issue #859; PR #860)
+- fix bug in reported uncertainties for constrained parameters by better propating uncertainties (Issue #855; PR #856)
+- Coercing of user input data and independent data for ``Model`` to float64 ndarrays is somewhat less aggressive and
+  will not increase the precision of numpy ndarrays (see :ref:`model_data_coercion_section` for details). The resulting
+  calculation from a model or objective function is more aggressively coerced to float64.  (Issue #850; PR #853)
+- the default value of ``epsfcn`` is increased to 1.e-10 to allow for handling of data with precision less than float64
+  (Issue #850; PR #853)
+- fix ``conf_interval2d`` to use "increase chi-square by sigma**2*reduced chi-square" to give the ``sigma``-level
+  probabilities (Issue #848; PR #852)
+- fix reading of older ``ModelResult`` (Issue #845; included in PR #844)
+- fix deepcopy of ``Parameters`` and user data (mguhyo; PR #837)
+- improve ``Model.make_params`` and ``create_params`` to take optional dict of Parameter attributes (PR #844)
+- fix reporting of ``nfev`` from ``least_squares`` to better reflect actual number of function calls (Issue #842; PR #844)
+- fix bug in ``Model.eval`` when mixing parameters and keyword arguments (PR #844, #839)
+- re-adds ``residual`` to saved ``Model`` result (PR #844, #830)
+- ``ConstantModel`` and ``ComplexConstantModel`` will return an ndarray of the same shape as the independent variable
+  ``x`` (JeppeKlitgaard, Issue #840; PR #841)
+- update tests for latest versions of NumPy and SciPy.
+- many fixes of doc typos and updates of dependencies, pre-commit hooks, and CI.
+
 .. _whatsnew_110_label:
 
 Version 1.1.0 Release Notes (November 27, 2022)
 =================================================
 
 New features:
```

### Comparing `lmfit-1.1.0/examples/NIST_Gauss2.dat` & `lmfit-1.2.0/examples/NIST_Gauss2.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/doc_builtinmodels_nistgauss.py` & `lmfit-1.2.0/examples/doc_builtinmodels_nistgauss.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,33 +8,29 @@
 x = dat[:, 1]
 y = dat[:, 0]
 
 exp_mod = ExponentialModel(prefix='exp_')
 pars = exp_mod.guess(y, x=x)
 
 gauss1 = GaussianModel(prefix='g1_')
-pars.update(gauss1.make_params())
-
-pars['g1_center'].set(value=105, min=75, max=125)
-pars['g1_sigma'].set(value=15, min=3)
-pars['g1_amplitude'].set(value=2000, min=10)
+pars.update(gauss1.make_params(center=dict(value=105, min=75, max=125),
+                               sigma=dict(value=15, min=0),
+                               amplitude=dict(value=2000, min=0)))
 
 gauss2 = GaussianModel(prefix='g2_')
-pars.update(gauss2.make_params())
-
-pars['g2_center'].set(value=155, min=125, max=175)
-pars['g2_sigma'].set(value=15, min=3)
-pars['g2_amplitude'].set(value=2000, min=10)
+pars.update(gauss2.make_params(center=dict(value=155, min=125, max=175),
+                               sigma=dict(value=15, min=0),
+                               amplitude=dict(value=2000, min=0)))
 
 mod = gauss1 + gauss2 + exp_mod
 
 init = mod.eval(pars, x=x)
 out = mod.fit(y, pars, x=x)
 
-print(out.fit_report(min_correl=0.5))
+print(out.fit_report(correl_mode='table'))
 
 fig, axes = plt.subplots(1, 2, figsize=(12.8, 4.8))
 axes[0].plot(x, y)
 axes[0].plot(x, init, '--', label='initial fit')
 axes[0].plot(x, out.best_fit, '-', label='best fit')
 axes[0].legend()
```

### Comparing `lmfit-1.1.0/examples/doc_builtinmodels_nistgauss2.py` & `lmfit-1.2.0/examples/doc_builtinmodels_nistgauss2.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/doc_builtinmodels_peakmodels.py` & `lmfit-1.2.0/examples/doc_builtinmodels_peakmodels.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,51 +10,53 @@
 
 
 # Gaussian model
 mod = GaussianModel()
 pars = mod.guess(y, x=x)
 out = mod.fit(y, pars, x=x)
 
-print(out.fit_report(min_correl=0.25))
+print(out.fit_report(correl_mode='table'))
 
 plt.plot(x, y)
 plt.plot(x, out.best_fit, '-', label='Gaussian Model')
 plt.legend()
 plt.show()
 
 
 # Lorentzian model
 mod = LorentzianModel()
 pars = mod.guess(y, x=x)
 out = mod.fit(y, pars, x=x)
 
-print(out.fit_report(min_correl=0.25))
+print(out.fit_report(correl_mode='table'))
 
 plt.figure()
 plt.plot(x, y, '-')
 plt.plot(x, out.best_fit, '-', label='Lorentzian Model')
 plt.legend()
 plt.show()
 
 
 # Voigt model
 mod = VoigtModel()
 pars = mod.guess(y, x=x)
 out = mod.fit(y, pars, x=x)
 
-print(out.fit_report(min_correl=0.25))
+print(out.fit_report(correl_mode='table'))
 
 fig, axes = plt.subplots(1, 2, figsize=(12.8, 4.8))
 
 axes[0].plot(x, y, '-')
 axes[0].plot(x, out.best_fit, '-', label='Voigt Model\ngamma constrained')
 axes[0].legend()
 
-# free gamma parameter
-pars['gamma'].set(value=0.7, vary=True, expr='')
+# allow the gamma parameter to vary in the fit
+pars['gamma'].vary = True
 out_gamma = mod.fit(y, pars, x=x)
+print(out.fit_report(correl_mode='table'))
+
 axes[1].plot(x, y, '-')
 axes[1].plot(x, out_gamma.best_fit, '-', label='Voigt Model\ngamma unconstrained')
 axes[1].legend()
 
 plt.show()
 # <end examples/doc_builtinmodels_peakmodels.py>
```

### Comparing `lmfit-1.1.0/examples/doc_builtinmodels_splinemodel.py` & `lmfit-1.2.0/examples/doc_builtinmodels_splinemodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,31 +7,29 @@
 data = np.loadtxt('test_splinepeak.dat')
 x = data[:, 0]
 y = data[:, 1]
 
 plt.plot(x, y, label='data')
 
 model = GaussianModel(prefix='peak_')
-params = model.make_params(amplitude=8, center=16, sigma=1)
+params = model.make_params(amplitude=dict(value=8, min=0),
+                           center=dict(value=16, min=5, max=25),
+                           sigma=dict(value=1, min=0))
 
 # make a background spline with knots evenly spaced over the background,
 # but sort of skipping over where the peak is
 knot_xvals3 = np.array([1, 3, 5, 7, 9, 11, 13, 15, 17, 19, 21, 23, 25])
 knot_xvals2 = np.array([1, 3, 5, 7, 9, 11, 13,   16,   19, 21, 23, 25])  # noqa: E241
 knot_xvals1 = np.array([1, 3, 5, 7, 9, 11, 13,         19, 21, 23, 25])  # noqa: E241
 
 bkg = SplineModel(prefix='bkg_', xknots=knot_xvals1)
 params.update(bkg.guess(y, x))
 
 model = model + bkg
 
-params['peak_center'].min = 10
-params['peak_center'].max = 20
-params['peak_amplitude'].min = 0
-
 plt.plot(x, model.eval(params, x=x), label='initial')
 
 out = model.fit(y, params, x=x)
 print(out.fit_report(min_correl=0.3))
 comps = out.eval_components()
 
 plt.plot(x, out.best_fit, label='best fit')
```

### Comparing `lmfit-1.1.0/examples/doc_builtinmodels_stepmodel.py` & `lmfit-1.2.0/examples/doc_builtinmodels_stepmodel.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/doc_confidence_advanced.py` & `lmfit-1.2.0/examples/doc_confidence_advanced.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 
 import lmfit
 
 x = np.linspace(1, 10, 250)
 np.random.seed(0)
 y = 3.0*np.exp(-x/2) - 5.0*np.exp(-(x-0.1)/10.) + 0.1*np.random.randn(x.size)
 
-p = lmfit.Parameters()
-p.add_many(('a1', 4.), ('a2', 4.), ('t1', 3.), ('t2', 3.))
+p = lmfit.create_params(a1=4, a2=4, t1=3, t2=3)
 
 
 def residual(p):
     return p['a1']*np.exp(-x/p['t1']) + p['a2']*np.exp(-(x-0.1)/p['t2']) - y
 
 
 # create Minimizer
```

### Comparing `lmfit-1.1.0/examples/doc_fitting_emcee.py` & `lmfit-1.2.0/examples/doc_fitting_emcee.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/doc_fitting_withreport.py` & `lmfit-1.2.0/examples/doc_fitting_withreport.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 # <examples/doc_fitting_withreport.py>
 from numpy import exp, linspace, pi, random, sign, sin
 
-from lmfit import Parameters, fit_report, minimize
+from lmfit import create_params, fit_report, minimize
 
-p_true = Parameters()
-p_true.add('amp', value=14.0)
-p_true.add('period', value=5.46)
-p_true.add('shift', value=0.123)
-p_true.add('decay', value=0.032)
+p_true = create_params(amp=14.0, period=5.46, shift=0.123, decay=0.032)
 
 
 def residual(pars, x, data=None):
     """Model a decaying sine wave and subtract data."""
     vals = pars.valuesdict()
     amp = vals['amp']
     per = vals['period']
@@ -27,17 +23,13 @@
 
 
 random.seed(0)
 x = linspace(0.0, 250., 1001)
 noise = random.normal(scale=0.7215, size=x.size)
 data = residual(p_true, x) + noise
 
-fit_params = Parameters()
-fit_params.add('amp', value=13.0)
-fit_params.add('period', value=2)
-fit_params.add('shift', value=0.0)
-fit_params.add('decay', value=0.02)
+fit_params = create_params(amp=13, period=2, shift=0, decay=0.02)
 
 out = minimize(residual, fit_params, args=(x,), kws={'data': data})
 
 print(fit_report(out))
 # <end examples/doc_fitting_withreport.py>
```

### Comparing `lmfit-1.1.0/examples/doc_model_composite.py` & `lmfit-1.2.0/examples/doc_model_composite.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,19 +28,22 @@
     out = np.convolve(tmp, kernel, mode='valid')
     noff = int((len(out) - npts) / 2)
     return out[noff:noff+npts]
 
 
 # create Composite Model using the custom convolution operator
 mod = CompositeModel(Model(jump), Model(gaussian), convolve)
-pars = mod.make_params(amplitude=1, center=3.5, sigma=1.5, mid=5.0)
 
-# 'mid' and 'center' should be completely correlated, and 'mid' is
-# used as an integer index, so a very poor fit variable:
-pars['mid'].vary = False
+# create parameters for model.  Note that 'mid' and 'center' will be highly
+# correlated. Since 'mid' is used as an integer index, it will be very
+# hard to fit, so we fix its value
+pars = mod.make_params(amplitude=dict(value=1, min=0),
+                       center=3.5,
+                       sigma=dict(value=1.5, min=0),
+                       mid=dict(value=4, vary=False))
 
 # fit this model to data array y
 result = mod.fit(y, params=pars, x=x)
 
 print(result.fit_report())
 
 # generate components
```

### Comparing `lmfit-1.1.0/examples/doc_model_gaussian.py` & `lmfit-1.2.0/examples/doc_model_gaussian.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/doc_model_two_components.py` & `lmfit-1.2.0/examples/doc_model_two_components.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 
 def line(x, slope, intercept):
     """a line"""
     return slope*x + intercept
 
 
 mod = Model(gaussian) + Model(line)
-pars = mod.make_params(amp=5, cen=5, wid=1, slope=0, intercept=1)
+pars = mod.make_params(amp=5, cen=5, wid={'value': 1, 'min': 0},
+                       slope=0, intercept=1)
 
 result = mod.fit(y, pars, x=x)
-
 print(result.fit_report())
 
 plt.plot(x, y, 'o')
 plt.plot(x, result.init_fit, '--', label='initial fit')
 plt.plot(x, result.best_fit, '-', label='best fit')
 plt.legend()
 plt.show()
```

### Comparing `lmfit-1.1.0/examples/doc_model_uncertainty.py` & `lmfit-1.2.0/examples/doc_model_uncertainty.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/doc_model_uncertainty2.py` & `lmfit-1.2.0/examples/doc_model_uncertainty2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,19 @@
                            g1_center=100,
                            g1_sigma=10,
                            g2_amplitude=3000,
                            g2_center=150,
                            g2_sigma=10)
 
 result = model.fit(y, params, x=x)
-
 print(result.fit_report(min_correl=0.5))
 
-
 comps = result.eval_components(x=x)
 dely = result.eval_uncertainty(sigma=3)
 
-
 fig, axes = plt.subplots(2, 2, figsize=(12.8, 9.6))
 
 axes[0][0].plot(x, y, 'o', color='#99002299', markersize=3, label='data')
 axes[0][0].plot(x, result.best_fit, '-', label='best fit')
 axes[0][0].plot(x, result.init_fit, '--', label='initial fit')
 axes[0][0].set_title('data, initial fit, and best-fit')
 axes[0][0].legend()
@@ -40,15 +37,14 @@
 axes[0][1].plot(x, y, 'o', color='#99002299', markersize=3, label='data')
 axes[0][1].plot(x, result.best_fit, '-', label='best fit')
 axes[0][1].fill_between(x, result.best_fit-dely, result.best_fit+dely,
                         color="#8A8A8A", label=r'3-$\sigma$ band')
 axes[0][1].set_title('data, best-fit, and uncertainty band')
 axes[0][1].legend()
 
-
 axes[1][0].plot(x, result.best_fit, '-', label=r'best fit, 3-$\sigma$ band')
 axes[1][0].fill_between(x,
                         result.best_fit-result.dely,
                         result.best_fit+result.dely,
                         color="#8A8A8A")
 
 axes[1][0].plot(x, comps['bkg_'], label=r'background, 3-$\sigma$ band')
@@ -66,19 +62,18 @@
 axes[1][0].plot(x, comps['g2_'], label=r'Gaussian #2, 3-$\sigma$ band')
 axes[1][0].fill_between(x,
                         comps['g2_']-result.dely_comps['g2_'],
                         comps['g2_']+result.dely_comps['g2_'],
                         color="#8A8A8A")
 axes[1][0].set_title('model components with uncertainty bands')
 axes[1][0].legend()
-#
+
 axes[1][1].plot(x, result.best_fit, '-', label='best fit')
 axes[1][1].plot(x, 10*result.dely, label=r'3-$\sigma$ total (x10)')
 axes[1][1].plot(x, 10*result.dely_comps['bkg_'], label=r'3-$\sigma$ background (x10)')
 axes[1][1].plot(x, 10*result.dely_comps['g1_'], label=r'3-$\sigma$ Gaussian #1 (x10)')
 axes[1][1].plot(x, 10*result.dely_comps['g2_'], label=r'3-$\sigma$ Gaussian #2 (x10)')
 axes[1][1].set_title('uncertainties for model components')
 axes[1][1].legend()
 
 plt.show()
-
 # <end examples/doc_model_uncertainty2.py>
```

### Comparing `lmfit-1.1.0/examples/doc_model_with_iter_callback.py` & `lmfit-1.2.0/examples/doc_model_with_iter_callback.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,20 +13,19 @@
 x = linspace(0., 20, 401)
 y = gaussian(x, amplitude=24.56, center=7.6543, sigma=1.23)
 random.seed(2021)
 y = y - .20*x + 3.333 + random.normal(scale=0.23, size=x.size)
 
 mod = GaussianModel(prefix='peak_') + LinearModel(prefix='bkg_')
 
-pars = mod.make_params()
-pars['peak_amplitude'].value = 3.0
-pars['peak_center'].value = 6.0
-pars['peak_sigma'].value = 2.0
-pars['bkg_intercept'].value = 0.0
-pars['bkg_slope'].value = 0.0
+pars = mod.make_params(peak_amplitude=dict(value=3.0, min=0),
+                       peak_center=dict(value=6.0, min=0, max=20),
+                       peak_sigma=2.0,
+                       bkg_intercept=0,
+                       bkg_slope=0)
 
 out = mod.fit(y, pars, x=x, iter_cb=per_iteration)
 
 plt.plot(x, y, '--')
 
 print(f'Nfev = {out.nfev}')
 print(out.fit_report())
```

### Comparing `lmfit-1.1.0/examples/doc_model_with_nan_policy.py` & `lmfit-1.2.0/examples/doc_model_with_nan_policy.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/doc_parameters_basic.py` & `lmfit-1.2.0/examples/doc_parameters_basic.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # <examples/doc_parameters_basic.py>
 import numpy as np
 
-from lmfit import Minimizer, Parameters, report_fit
+from lmfit import Minimizer, Parameters, create_params, report_fit
 
 # create data to be fitted
 x = np.linspace(0, 15, 301)
 np.random.seed(2021)
 data = (5.0 * np.sin(2.0*x - 0.1) * np.exp(-x*x*0.025) +
         np.random.normal(size=x.size, scale=0.2))
 
@@ -24,14 +24,20 @@
 # create a set of Parameters
 params = Parameters()
 params.add('amp', value=10, min=0)
 params.add('decay', value=0.1)
 params.add('shift', value=0.0, min=-np.pi/2., max=np.pi/2.)
 params.add('omega', value=3.0)
 
+# ... or use
+params = create_params(amp=dict(value=10, min=0),
+                       decay=0.1,
+                       omega=3,
+                       shift=dict(value=0, min=-np.pi/2, max=np.pi/2))
+
 # do fit, here with the default leastsq algorithm
 minner = Minimizer(fcn2min, params, fcn_args=(x, data))
 result = minner.minimize()
 
 # calculate final result
 final = data + result.residual
```

### Comparing `lmfit-1.1.0/examples/doc_parameters_valuesdict.py` & `lmfit-1.2.0/examples/doc_parameters_valuesdict.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # <examples/doc_parameters_valuesdict.py>
 import numpy as np
 
-from lmfit import Minimizer, Parameters, report_fit
+from lmfit import Minimizer, create_params, report_fit
 
 # create data to be fitted
 x = np.linspace(0, 15, 301)
 np.random.seed(2021)
 data = (5.0 * np.sin(2.0*x - 0.1) * np.exp(-x*x*0.025) +
         np.random.normal(size=x.size, scale=0.2))
 
@@ -16,19 +16,18 @@
     v = params.valuesdict()
 
     model = v['amp'] * np.sin(x * v['omega'] + v['shift']) * np.exp(-x*x*v['decay'])
     return model - data
 
 
 # create a set of Parameters
-params = Parameters()
-params.add('amp', value=10, min=0)
-params.add('decay', value=0.1)
-params.add('shift', value=0.0, min=-np.pi/2., max=np.pi/2)
-params.add('omega', value=3.0)
+params = create_params(amp=dict(value=10, min=0),
+                       decay=0.1,
+                       omega=3.0,
+                       shift=dict(value=0.0, min=-np.pi/2., max=np.pi/2))
 
 # do fit, here with the default leastsq algorithm
 minner = Minimizer(fcn2min, params, fcn_args=(x, data))
 result = minner.minimize()
 
 # calculate final result
 final = data + result.residual
```

### Comparing `lmfit-1.1.0/examples/example_Model_interface.py` & `lmfit-1.2.0/examples/example_Model_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,19 +76,15 @@
 
 ###############################################################################
 # **Defining Parameters in Advance**
 #
 # Passing parameters to ``fit`` can become unwieldy. As an alternative, you
 # can extract the parameters from ``model`` like so, set them individually,
 # and pass them to ``fit``.
-params = model.make_params()
-
-params['N'].value = 10
-params['tau'].value = 1
-params['tau'].min = 0
+params = model.make_params(N=10, tau={'value': 1, 'min': 0})
 
 result = model.fit(data, params, t=t)
 report_fit(result.params)
 
 ##############################################################################
 # Keyword arguments override ``params``, resetting ``value`` and all other
 # properties (``min``, ``max``, ``vary``).
```

### Comparing `lmfit-1.1.0/examples/example_brute.py` & `lmfit-1.2.0/examples/example_brute.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,45 +14,48 @@
 # (see below).
 import copy
 
 from matplotlib.colors import LogNorm
 import matplotlib.pyplot as plt
 import numpy as np
 
-from lmfit import Minimizer, Parameters, fit_report
+from lmfit import Minimizer, create_params, fit_report
 
 ###############################################################################
 # Let's start with the example given in the documentation of SciPy:
 #
 # "We illustrate the use of brute to seek the global minimum of a function of
 # two variables that is given as the sum of a positive-definite quadratic and
 # two deep “Gaussian-shaped” craters. Specifically, define the objective
 # function ``f`` as the sum of three other functions, ``f = f1 + f2 + f3``. We
 # suppose each of these has a signature ``(z, *params), where z = (x, y)``,
 # and params and the functions are as defined below."
 #
 # First, we create a set of Parameters where all variables except ``x`` and
 # ``y`` are given fixed values.
-params = Parameters()
-params.add_many(
-        ('a', 2, False),
-        ('b', 3, False),
-        ('c', 7, False),
-        ('d', 8, False),
-        ('e', 9, False),
-        ('f', 10, False),
-        ('g', 44, False),
-        ('h', -1, False),
-        ('i', 2, False),
-        ('j', 26, False),
-        ('k', 1, False),
-        ('l', -2, False),
-        ('scale', 0.5, False),
-        ('x', 0.0, True),
-        ('y', 0.0, True))
+# Just as in the documentation we will do a grid search between ``-4`` and
+# ``4`` and use a stepsize of ``0.25``. The bounds can be set as usual with
+# the ``min`` and ``max`` attributes, and the stepsize is set using
+# ``brute_step``.
+
+params = create_params(a=dict(value=2, vary=False),
+                       b=dict(value=3, vary=False),
+                       c=dict(value=7, vary=False),
+                       d=dict(value=8, vary=False),
+                       e=dict(value=9, vary=False),
+                       f=dict(value=10, vary=False),
+                       g=dict(value=44, vary=False),
+                       h=dict(value=-1, vary=False),
+                       i=dict(value=2, vary=False),
+                       j=dict(value=26, vary=False),
+                       k=dict(value=1, vary=False),
+                       l=dict(value=-2, vary=False),
+                       scale=dict(value=0.5, vary=False),
+                       x=dict(value=0.0, vary=True, min=-4, max=4, brute_step=0.25),
+                       y=dict(value=0.0, vary=True, min=-4, max=4, brute_step=0.25))
 
 ###############################################################################
 # Second, create the three functions and the objective function:
 
 
 def f1(p):
     par = p.valuesdict()
@@ -74,22 +77,14 @@
 
 
 def f(params):
     return f1(params) + f2(params) + f3(params)
 
 
 ###############################################################################
-# Just as in the documentation we will do a grid search between ``-4`` and
-# ``4`` and use a stepsize of ``0.25``. The bounds can be set as usual with
-# the ``min`` and ``max`` attributes, and the stepsize is set using
-# ``brute_step``.
-params['x'].set(min=-4, max=4, brute_step=0.25)
-params['y'].set(min=-4, max=4, brute_step=0.25)
-
-###############################################################################
 # Performing the actual grid search is done with:
 fitter = Minimizer(f, params)
 result = fitter.minimize(method='brute')
 
 ###############################################################################
 # , which will increment ``x`` and ``y`` between ``-4`` in increments of
 # ``0.25`` until ``4`` (not inclusive).
@@ -144,40 +139,36 @@
     shift = params['shift']
     omega = params['omega']
     decay = params['decay']
     model = amp * np.sin(x*omega + shift) * np.exp(-x*x*decay)
     return model - data
 
 
-# create a set of Parameters
-params = Parameters()
-params.add('amp', value=7, min=2.5)
-params.add('decay', value=0.05)
-params.add('shift', value=0.0, min=-np.pi/2., max=np.pi/2)
-params.add('omega', value=3, max=5)
-
 ###############################################################################
 # In contrast to the implementation in SciPy (as shown in the first example),
-# varying parameters do not need to have finite bounds in lmfit. However, in
-# that case they **do** need the ``brute_step`` attribute specified, so let's
-# do that:
-params['amp'].set(brute_step=0.25)
-params['decay'].set(brute_step=0.005)
-params['omega'].set(brute_step=0.25)
+# varying parameters do not need to have finite bounds in lmfit. However, if a
+# parameter does not have finite bounds, then it does need a ``brute_step``
+# attribute specified:
+params = create_params(amp=dict(value=7, min=2.5, brute_step=0.25),
+                       decay=dict(value=0.05, brute_step=0.005),
+                       shift=dict(value=0.0, min=-np.pi/2., max=np.pi/2),
+                       omega=dict(value=3, max=5, brute_step=0.25))
 
 ###############################################################################
 # Our initial parameter set is now defined as shown below and this will
 # determine how the grid is set-up.
 params.pretty_print()
 
 ###############################################################################
 # First, we initialize a ``Minimizer`` and perform the grid search:
 fitter = Minimizer(fcn2min, params, fcn_args=(x, data))
 result_brute = fitter.minimize(method='brute', Ns=25, keep=25)
 
+print(fit_report(result_brute))
+
 ###############################################################################
 # We used two new parameters here: ``Ns`` and ``keep``. The parameter ``Ns``
 # determines the \'number of grid points along the axes\' similarly to its usage
 # in SciPy. Together with ``brute_step``, ``min`` and ``max`` for a Parameter
 # it will dictate how the grid is set-up:
 #
 # **(1)** finite bounds are specified ("SciPy implementation"): uses
@@ -394,7 +385,8 @@
     if output is not None:
         plt.savefig(output)
 
 
 ###############################################################################
 # and finally, to generated the figure:
 plot_results_brute(result_brute, best_vals=True, varlabels=None)
+plt.show()
```

### Comparing `lmfit-1.1.0/examples/example_complex_resonator_model.py` & `lmfit-1.2.0/examples/example_complex_resonator_model.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/example_confidence_interval.py` & `lmfit-1.2.0/examples/example_confidence_interval.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ==============================
 
 """
 import matplotlib.pyplot as plt
 from numpy import argsort, exp, linspace, pi, random, sign, sin, unique
 from scipy.interpolate import interp1d
 
-from lmfit import (Minimizer, Parameters, conf_interval, conf_interval2d,
+from lmfit import (Minimizer, conf_interval, conf_interval2d, create_params,
                    report_ci, report_fit)
 
 ###############################################################################
 # Define the residual function, specify "true" parameter values, and generate
 # a synthetic data set with some noise:
 
 
@@ -22,32 +22,24 @@
         shift = shift - sign(shift)*pi
     model = pars['amp']*sin(shift + x/pars['period']) * exp(-argu)
     if data is None:
         return model
     return model - data
 
 
-p_true = Parameters()
-p_true.add('amp', value=14.0)
-p_true.add('period', value=5.33)
-p_true.add('shift', value=0.123)
-p_true.add('decay', value=0.010)
+p_true = create_params(amp=14.0, period=5.33, shift=0.123, decay=0.010)
 
 x = linspace(0.0, 250.0, 2500)
 random.seed(2021)
 noise = random.normal(scale=0.7215, size=x.size)
 data = residual(p_true, x) + noise
 
 ###############################################################################
 # Create fitting parameters and set initial values:
-fit_params = Parameters()
-fit_params.add('amp', value=13.0)
-fit_params.add('period', value=2)
-fit_params.add('shift', value=0.0)
-fit_params.add('decay', value=0.02)
+fit_params = create_params(amp=13.0, period=2, shift=0.0, decay=0.020)
 
 ###############################################################################
 # Set-up the minimizer and perform the fit using ``leastsq`` algorithm, and
 # show the report:
 mini = Minimizer(residual, fit_params, fcn_args=(x,), fcn_kws={'data': data})
 out = mini.leastsq()
```

### Comparing `lmfit-1.1.0/examples/example_detect_outliers.py` & `lmfit-1.2.0/examples/example_detect_outliers.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/example_diffev.py` & `lmfit-1.2.0/examples/example_diffev.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/example_emcee_Model_interface.py` & `lmfit-1.2.0/examples/example_emcee_Model_interface.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/example_expression_model.py` & `lmfit-1.2.0/examples/example_expression_model.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/example_fit_multi_datasets.py` & `lmfit-1.2.0/examples/example_fit_multi_datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,14 @@
 
 ###############################################################################
 # Create five simulated Gaussian data sets
 np.random.seed(2021)
 x = np.linspace(-1, 2, 151)
 data = []
 for _ in np.arange(5):
-    params = Parameters()
     amp = 0.60 + 9.50*np.random.rand()
     cen = -0.20 + 1.20*np.random.rand()
     sig = 0.25 + 0.03*np.random.rand()
     dat = gauss(x, amp, cen, sig) + np.random.normal(size=x.size, scale=0.1)
     data.append(dat)
 data = np.array(data)
```

### Comparing `lmfit-1.1.0/examples/example_fit_with_bounds.py` & `lmfit-1.2.0/examples/example_fit_with_bounds.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,24 +10,20 @@
 The example below shows how to set boundaries using the ``min`` and ``max``
 attributes to fitting parameters.
 
 """
 import matplotlib.pyplot as plt
 from numpy import exp, linspace, pi, random, sign, sin
 
-from lmfit import Parameters, minimize
+from lmfit import create_params, minimize
 from lmfit.printfuncs import report_fit
 
 ###############################################################################
-# Define the 'correct' Parameter values and residual function:
-p_true = Parameters()
-p_true.add('amp', value=14.0)
-p_true.add('period', value=5.4321)
-p_true.add('shift', value=0.12345)
-p_true.add('decay', value=0.01000)
+# create the 'true' Parameter values and residual function:
+p_true = create_params(amp=14.0, period=5.4321, shift=0.12345, decay=0.010)
 
 
 def residual(pars, x, data=None):
     argu = (x * pars['decay'])**2
     shift = pars['shift']
     if abs(shift) > pi/2:
         shift = shift - sign(shift)*pi
@@ -40,25 +36,25 @@
 ###############################################################################
 # Generate synthetic data and initialize fitting Parameters:
 random.seed(0)
 x = linspace(0, 250, 1500)
 noise = random.normal(scale=2.8, size=x.size)
 data = residual(p_true, x) + noise
 
-fit_params = Parameters()
-fit_params.add('amp', value=13, max=20, min=0)
-fit_params.add('period', value=2, max=10)
-fit_params.add('shift', value=0, max=pi/2., min=-pi/2.)
-fit_params.add('decay', value=0.02, max=0.1, min=0)
+fit_params = create_params(amp=dict(value=13, max=20, min=0),
+                           period=dict(value=2, max=10),
+                           shift=dict(value=0, max=pi/2., min=-pi/2.),
+                           decay=dict(value=0.02, max=0.1, min=0))
 
 ###############################################################################
 # Perform the fit and show the results:
 out = minimize(residual, fit_params, args=(x,), kws={'data': data})
 fit = residual(out.params, x)
 
 ###############################################################################
-report_fit(out, modelpars=p_true)
+report_fit(out, modelpars=p_true, correl_mode='table')
 
 ###############################################################################
 plt.plot(x, data, 'o', label='data')
 plt.plot(x, fit, label='best fit')
 plt.legend()
+plt.show()
```

### Comparing `lmfit-1.1.0/examples/example_fit_with_derivfunc.py` & `lmfit-1.2.0/examples/example_fit_with_derivfunc.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/example_reduce_fcn.py` & `lmfit-1.2.0/examples/example_reduce_fcn.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,19 +39,16 @@
 x = np.linspace(0, 10, 101)
 y = offset + amp * np.sin(omega*x) * np.exp(-x/decay)
 yn = y + np.random.normal(size=y.size, scale=0.250)
 
 outliers = np.random.randint(int(len(x)/3.0), len(x), int(len(x)/12))
 yn[outliers] += 5*np.random.random(len(outliers))
 
-params = lmfit.Parameters()
-params.add('offset', 2.0)
-params.add('omega', 3.3)
-params.add('amp', 2.5)
-params.add('decay', 1.0, min=0)
+params = lmfit.create_params(offset=2.0, omega=3.3, amp=2.5,
+                             decay=dict(value=1, min=0))
 
 ###############################################################################
 # Perform fits using the ``L-BFGS-B`` method with different ``reduce_fcn``:
 method = 'L-BFGS-B'
 o1 = lmfit.minimize(resid, params, args=(x, yn), method=method)
 print("# Fit using sum of squares:\n")
 lmfit.report_fit(o1)
@@ -64,7 +61,8 @@
 
 ###############################################################################
 plt.plot(x, y, 'o', label='true function')
 plt.plot(x, yn, '--*', label='with noise+outliers')
 plt.plot(x, yn+o1.residual, '-', label='sum of squares fit')
 plt.plot(x, yn+o2.residual, '-', label='robust fit')
 plt.legend()
+plt.show()
```

### Comparing `lmfit-1.1.0/examples/example_sympy.py` & `lmfit-1.2.0/examples/example_sympy.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/example_two_dimensional_peak.py` & `lmfit-1.2.0/examples/example_two_dimensional_peak.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/example_use_pandas.py` & `lmfit-1.2.0/examples/example_use_pandas.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/lmfit_emcee_model_selection.py` & `lmfit-1.2.0/examples/lmfit_emcee_model_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Model Selection using lmfit and emcee
 =====================================
 
-FIXME: this is a useful examples; however, it doesn't run correctly anymore as
+FIXME: this is a useful example; however, it doesn't run correctly anymore as
 the PTSampler was removed in emcee v3...
 
 """
 ###############################################################################
 # `lmfit.emcee` can be used to obtain the posterior probability distribution
 # of parameters, given a set of experimental data. This notebook shows how it
 # can be used for Bayesian model selection.
```

### Comparing `lmfit-1.1.0/examples/model1d_gauss.dat` & `lmfit-1.2.0/examples/model1d_gauss.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/peak.csv` & `lmfit-1.2.0/examples/peak.csv`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/sinedata.dat` & `lmfit-1.2.0/examples/sinedata.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/test_peak.dat` & `lmfit-1.2.0/examples/test_peak.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/examples/test_splinepeak.dat` & `lmfit-1.2.0/examples/test_splinepeak.dat`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/lmfit/__init__.py` & `lmfit-1.2.0/lmfit/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,13 +33,13 @@
 Copyright (c) 2022 Lmfit Developers ; BSD-3 license ; see LICENSE
 
 """
 from asteval import Interpreter
 
 from .confidence import conf_interval, conf_interval2d
 from .minimizer import Minimizer, MinimizerException, minimize
-from .parameter import Parameter, Parameters
+from .parameter import Parameter, Parameters, create_params
 from .printfuncs import ci_report, fit_report, report_ci, report_fit
 from .model import Model, CompositeModel
 from . import lineshapes, models
 
 from lmfit.version import version as __version__
```

### Comparing `lmfit-1.1.0/lmfit/_ampgo.py` & `lmfit-1.2.0/lmfit/_ampgo.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/lmfit/confidence.py` & `lmfit-1.2.0/lmfit/confidence.py`

 * *Files 3% similar despite different names*

```diff
@@ -349,15 +349,15 @@
             x = [i.value for i in out.params.values()]
             self.trace_dict[para.name].append(x + [prob])
         self.params[para.name] = save_para
         return prob - offset
 
 
 def conf_interval2d(minimizer, result, x_name, y_name, nx=10, ny=10,
-                    limits=None, prob_func=None):
+                    limits=None, prob_func=None, nsigma=5, chi2_out=False):
     r"""Calculate confidence regions for two fixed parameters.
 
     The method itself is explained in `conf_interval`: here we are fixing
     two parameters.
 
     Parameters
     ----------
@@ -366,88 +366,93 @@
     result : MinimizerResult
         The result of running minimize().
     x_name : str
         The name of the parameter which will be the x direction.
     y_name : str
         The name of the parameter which will be the y direction.
     nx : int, optional
-        Number of points in the x direction.
+        Number of points in the x direction (default is 10).
     ny : int, optional
-        Number of points in the y direction.
+        Number of points in the y direction (default is 10).
     limits : tuple, optional
         Should have the form ``((x_upper, x_lower), (y_upper, y_lower))``.
-        If not given, the default is 5.0*std-errors in each direction.
-    prob_func : None or callable, optional
-        Function to calculate the probability from the optimized chi-square.
-        Default is None and uses the built-in function `f_compare`
-        (i.e., F-test).
+        If not given, the default is nsigma*stderr in each direction.
+    prob_func : None or callable, deprecated
+        Starting with version 1.2, this argument is unused and has no effect.
+    nsigma : float or int, optional
+        Multiplier of stderr for limits (default is 5).
+    chi2_out: bool
+        Whether to return chi-square at each coordinate instead of probability.
 
     Returns
     -------
     x : numpy.ndarray
         X-coordinates (same shape as `nx`).
     y : numpy.ndarray
         Y-coordinates (same shape as `ny`).
     grid : numpy.ndarray
-        Grid containing the calculated probabilities (with shape
-        ``(nx, ny)``).
+        2-D array (with shape ``(nx, ny)``) containing the calculated
+        probabilities or chi-square.
 
     See Also
     --------
     conf_interval
 
     Examples
     --------
     >>> mini = Minimizer(some_func, params)
     >>> result = mini.leastsq()
     >>> x, y, gr = conf_interval2d(mini, result, 'para1','para2')
     >>> plt.contour(x,y,gr)
 
     """
+    if prob_func is not None:
+        msg = "'prob_func' has no effect and will be removed in version 1.4."
+        raise DeprecationWarning(msg)
+
     params = result.params
 
-    best_chi = result.chisqr
+    best_chisqr = result.chisqr
+    redchi = result.redchi
     org = copy_vals(result.params)
 
-    if prob_func is None:
-        prob_func = f_compare
-
     x = params[x_name]
     y = params[y_name]
 
     if limits is None:
-        (x_upper, x_lower) = (x.value + 5 * x.stderr, x.value - 5 * x.stderr)
-        (y_upper, y_lower) = (y.value + 5 * y.stderr, y.value - 5 * y.stderr)
+        (x_upper, x_lower) = (x.value + nsigma * x.stderr, x.value - nsigma * x.stderr)
+        (y_upper, y_lower) = (y.value + nsigma * y.stderr, y.value - nsigma * y.stderr)
     elif len(limits) == 2:
         (x_upper, x_lower) = limits[0]
         (y_upper, y_lower) = limits[1]
 
     x_points = np.linspace(x_lower, x_upper, nx)
     y_points = np.linspace(y_lower, y_upper, ny)
     grid = np.dstack(np.meshgrid(x_points, y_points))
 
-    x.vary = False
-    y.vary = False
+    x.vary, y.vary = False, False
 
-    def calc_prob(vals, restore=False):
-        """Calculate the probability."""
-        if restore:
-            restore_vals(org, result.params)
-        x.value = vals[0]
-        y.value = vals[1]
-        save_x = result.params[x.name]
-        save_y = result.params[y.name]
-        result.params[x.name] = x
-        result.params[y.name] = y
+    def calc_chisqr(vals, restore=False):
+        """Calculate chi-square for a set of parameter values."""
+        save_x = x.value
+        save_y = y.value
+        result.params[x.name].value = vals[0]
+        result.params[y.name].value = vals[1]
         minimizer.prepare_fit(params=result.params)
         out = minimizer.leastsq()
-        prob = prob_func(result, out)
-        result.params[x.name] = save_x
-        result.params[y.name] = save_y
-        return prob
-
-    out = x_points, y_points, np.apply_along_axis(calc_prob, -1, grid)
+        result.params[x.name].value = save_x
+        result.params[y.name].value = save_y
+        return out.chisqr
+
+    # grid of chi-square
+    out_mat = np.apply_along_axis(calc_chisqr, -1, grid)
+
+    # compute grid of sigma values from chi-square
+    if not chi2_out:
+        chisqr0 = out_mat.min()
+        chisqr0 = min(best_chisqr, chisqr0)
+        out_mat = np.sqrt((out_mat-chisqr0)/redchi)
 
     x.vary, y.vary = True, True
     restore_vals(org, result.params)
-    result.chisqr = best_chi
-    return out
+    result.chisqr = best_chisqr
+    return x_points, y_points, out_mat
```

### Comparing `lmfit-1.1.0/lmfit/jsonutils.py` & `lmfit-1.2.0/lmfit/jsonutils.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/lmfit/lineshapes.py` & `lmfit-1.2.0/lmfit/lineshapes.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/lmfit/minimizer.py` & `lmfit-1.2.0/lmfit/minimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,18 @@
     _names = kwargs.get('_names', None)
     _asteval = _pars._asteval
     if (_obj is None or _pars is None or _names is None or
             _asteval is None or _obj._expr_ast is None):
         return 0
     for val, name in zip(vals, _names):
         _asteval.symtable[name] = val
+
+    # re-evaluate all constraint parameters to
+    # force the propagation of uncertainties
+    [p._getval() for p in _pars.values()]
     return _asteval.eval(_obj._expr_ast)
 
 
 wrap_ueval = uncertainties.wrap(asteval_with_uncertainties)
 
 
 def eval_stderr(obj, uvars, _names, _pars):
@@ -593,15 +597,15 @@
         if self._abort:
             self.result.residual = out
             self.result.aborted = True
             self.result.message = "Fit aborted by user callback. Could not estimate error-bars."
             self.result.success = False
             raise AbortFitException("fit aborted by user.")
         else:
-            return _nan_policy(np.asarray(out).ravel(),
+            return _nan_policy(np.asfarray(out).ravel(),
                                nan_policy=self.nan_policy)
 
     def __jacobian(self, fvars):
         """Return analytical jacobian to be used with Levenberg-Marquardt.
 
         modified 02-01-2012 by Glenn Jones, Aberystwyth University
         modified 06-29-2015 by M Newville to apply gradient scaling for
@@ -1601,15 +1605,18 @@
         if not result.aborted:
             result.nfev -= 1
             result.residual = self.__residual(ret.x, False)
         result._calculate_statistics()
 
         if not result.aborted:
             for attr in ret:
-                setattr(result, attr, ret[attr])
+                outattr = attr
+                if attr == 'nfev':
+                    outattr = 'least_squares_nfev'
+                setattr(result, outattr, ret[attr])
 
             result.x = np.atleast_1d(result.x)
 
             # calculate the cov_x and estimate uncertainties/correlations
             try:
                 if issparse(ret.jac):
                     hess = (ret.jac.T * ret.jac).toarray()
@@ -1663,17 +1670,17 @@
         result.nfev -= 2  # correct for "pre-fit" initialization/checks
         variables = result._init_vals_internal
 
         # Note: we set max number of function evaluations here, and send twice
         # that value to the solver so it essentially never stops on its own
         self.set_max_nfev(max_nfev, 2000*(result.nvarys+1))
 
-        lskws = dict(Dfun=None, full_output=1, col_deriv=0, ftol=1.49012e-08,
-                     xtol=1.49012e-08, gtol=0.0, maxfev=2*self.max_nfev,
-                     epsfcn=None, factor=100, diag=None)
+        lskws = dict(Dfun=None, full_output=1, col_deriv=0, ftol=1.5e-8,
+                     xtol=1.5e-8, gtol=0.0, maxfev=2*self.max_nfev,
+                     epsfcn=1.e-10, factor=100, diag=None)
 
         if 'maxfev' in kws:
             warnings.warn(maxeval_warning.format('maxfev', thisfuncname()),
                           RuntimeWarning)
             kws.pop('maxfev')
 
         lskws.update(self.kws)
```

### Comparing `lmfit-1.1.0/lmfit/model.py` & `lmfit-1.2.0/lmfit/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -548,24 +548,31 @@
                 raise ValueError(self._invalid_par % (arg, fname))
         # the following as been changed from OrderedSet for the time being.
         self._param_names = names[:]
 
     def set_param_hint(self, name, **kwargs):
         """Set *hints* to use when creating parameters with `make_params()`.
 
-        This is especially convenient for setting initial values. The
-        `name` can include the models `prefix` or not. The hint given can
-        also include optional bounds and constraints
+        The given hint can include optional bounds and constraints
         ``(value, vary, min, max, expr)``, which will be used by
-        `make_params()` when building default parameters.
+        `Model.make_params()` when building default parameters.
+
+        While this can be used to set initial values, `Model.make_params` or
+        the function `create_params` should be preferred for creating
+        parameters with initial values.
+
+        The intended use here is to control how a Model should create
+        parameters, such as setting bounds that are required by the mathematics
+        of the model (for example, that a peak width cannot be negative), or to
+        define common constrained parameters.
 
         Parameters
         ----------
         name : str
-            Parameter name.
+            Parameter name, can include the models `prefix` or not.
         **kwargs : optional
             Arbitrary keyword arguments, needs to be a Parameter attribute.
             Can be any of the following:
 
             - value : float, optional
                 Numerical Parameter value.
             - vary : bool, optional
@@ -579,15 +586,14 @@
                 bound).
             - expr : str, optional
                 Mathematical expression used to constrain the value during
                 the fit.
 
         Example
         --------
-
         >>> model = GaussianModel()
         >>> model.set_param_hint('sigma', min=0)
 
         """
         npref = len(self._prefix)
         if npref > 0 and name.startswith(self._prefix):
             name = name[npref:]
@@ -626,32 +632,47 @@
         """Create a Parameters object for a Model.
 
         Parameters
         ----------
         verbose : bool, optional
             Whether to print out messages (default is False).
         **kwargs : optional
-            Parameter names and initial values.
+            Parameter names and initial values or dictionaries of
+                 values and attributes.
 
         Returns
         ---------
         params : Parameters
             Parameters object for the Model.
 
         Notes
         -----
-        1. The parameters may or may not have decent initial values for
-        each parameter.
+        1. Parameter values can be numbers (floats or ints) to set the parameter
+           value, or dictionaries with any of the following keywords:
+           ``value``, ``vary``, ``min``, ``max``, ``expr``, ``brute_step``,
+           ``is_init_value`` to set those parameter attributes.
 
-        2. This applies any default values or parameter hints that may
-        have been set.
+        2. This method will also apply any default values or parameter hints
+           that may have been defined for the model.
+
+        Example
+        --------
+        >>> gmodel = GaussianModel(prefix='peak_') + LinearModel(prefix='bkg_')
+        >>> gmodel.make_params(peak_center=3200, bkg_offset=0, bkg_slope=0,
+        ...                    peak_amplitdue=dict(value=100, min=2),
+        ...                    peak_sigma=dict(value=25, min=0, max=1000))
 
         """
         params = Parameters()
 
+        def setpar(par, val):
+            if isinstance(val, (float, int)):
+                val = {'value': val}
+            par.set(**val)
+
         # make sure that all named parameters are in params
         for name in self.param_names:
             if name in params:
                 par = params[name]
             else:
                 par = Parameter(name=name)
             par._delay_asteval = True
@@ -667,19 +688,17 @@
             if basename in self.param_hints:
                 hint = self.param_hints[basename]
                 for item in self._hint_names:
                     if item in hint:
                         setattr(par, item, hint[item])
             # apply values passed in through kw args
             if basename in kwargs:
-                # kw parameter names with no prefix
-                par.value = kwargs[basename]
+                setpar(par, kwargs[basename])
             if name in kwargs:
-                # kw parameter names with prefix
-                par.value = kwargs[name]
+                setpar(par, kwargs[basename])
             params.add(par)
             if verbose:
                 print(f' - Adding parameter "{name}"')
 
         # next build parameters defined in param_hints
         # note that composites may define their own additional
         # convenience parameters here
@@ -693,15 +712,15 @@
                 if verbose:
                     print(f' - Adding parameter for hint "{name}"')
             par._delay_asteval = True
             for item in self._hint_names:
                 if item in hint:
                     setattr(par, item, hint[item])
             if basename in kwargs:
-                par.value = kwargs[basename]
+                setpar(par, kwargs[basename])
             # Add the new parameter to self._param_names
             if name not in self._param_names:
                 self._param_names.append(name)
 
         for p in params.values():
             p._delay_asteval = False
         return params
@@ -799,14 +818,25 @@
         if params is None:
             params = {}
         if kwargs is None:
             kwargs = {}
         out = {}
         out.update(self.opts)
 
+        # 0: if a keyword argument is going to overwrite a parameter,
+        #    save that value so it can be restored before returning
+        saved_values = {}
+        for name, val in kwargs.items():
+            if name in params:
+                saved_values[name] = params[name].value
+                params[name].value = val
+
+        if len(saved_values) > 0:
+            params.update_constraints()
+
         # 1. fill in in all parameter values
         for name, par in params.items():
             if strip:
                 name = self._strip_prefix(name)
             if name in self._func_allargs or self._func_haskeywords:
                 out[name] = par.value
 
@@ -815,22 +845,24 @@
         if len(self._prefix) > 0:
             for fullname in self._param_names:
                 if fullname in params:
                     name = self._strip_prefix(fullname)
                     if name in self._func_allargs or self._func_haskeywords:
                         out[name] = params[fullname].value
 
-        # 3. kwargs handled slightly differently -- may set param value too!
+        # 3. kwargs might directly update function arguments
         for name, val in kwargs.items():
             if strip:
                 name = self._strip_prefix(name)
             if name in self._func_allargs or self._func_haskeywords:
                 out[name] = val
-                if name in params:
-                    params[name].value = val
+
+        # 4. finally, reset any values that have overwritten parameter values
+        for name, val in saved_values.items():
+            params[name].value = val
         return out
 
     def _make_all_args(self, params=None, **kwargs):
         """Generate **all** function args for all functions."""
         args = {}
         for key, val in self.make_funcargs(params, kwargs).items():
             args[f"{self._prefix}{key}"] = val
@@ -850,26 +882,27 @@
         -------
         numpy.ndarray, float, int or complex
             Value of model given the parameters and other arguments.
 
         Notes
         -----
         1. if `params` is None, the values for all parameters are expected
-        to be provided as keyword arguments. If `params` is given, and a
-        keyword argument for a parameter value is also given, the keyword
-        argument will be used.
+        to be provided as keyword arguments.
 
-        2. all non-parameter arguments for the model function, **including
+        2. If `params` is given, and a keyword argument for a parameter value
+        is also given, the keyword argument will be used in place of the value
+        in the value in `params`.
+
+        3. all non-parameter arguments for the model function, **including
         all the independent variables** will need to be passed in using
         keyword arguments.
 
-        3. The return type depends on the model function. For many of the
-        built-models it is a `numpy.ndarray`, with the exception of
-        `ConstantModel` and `ComplexConstantModel`, which return a `float`/`int`
-        or `complex` value.
+        4. The return types are generally `numpy.ndarray`, but may depends on
+        the model function and input independent variables. That is, return
+        values may be Python `float`, `int`, or  `complex` values.
 
         """
         return self.func(**self.make_funcargs(params, kwargs))
 
     @property
     def components(self):
         """Return components for composite model."""
@@ -940,41 +973,35 @@
         Returns
         -------
         ModelResult
 
         Notes
         -----
         1. if `params` is None, the values for all parameters are expected
-        to be provided as keyword arguments. If `params` is given, and a
-        keyword argument for a parameter value is also given, the keyword
-        argument will be used.
+        to be provided as keyword arguments. Mixing `params` and
+        keyword arguments is deprecated (see `Model.eval`).
 
         2. all non-parameter arguments for the model function, **including
         all the independent variables** will need to be passed in using
         keyword arguments.
 
-        3. Parameters (however passed in), are copied on input, so the
-        original Parameter objects are unchanged, and the updated values
-        are in the returned `ModelResult`.
+        3. Parameters are copied on input, so that the original Parameter objects
+        are unchanged, and the updated values are in the returned `ModelResult`.
 
         Examples
         --------
         Take ``t`` to be the independent variable and data to be the curve
         we will fit. Use keyword arguments to set initial guesses:
 
         >>> result = my_model.fit(data, tau=5, N=3, t=t)
 
         Or, for more control, pass a Parameters object.
 
         >>> result = my_model.fit(data, params, t=t)
 
-        Keyword arguments override Parameters.
-
-        >>> result = my_model.fit(data, params, tau=5, t=t)
-
         """
         if params is None:
             params = self.make_params(verbose=verbose)
         else:
             params = deepcopy(params)
 
         # If any kwargs match parameter names, override params.
@@ -1023,30 +1050,33 @@
 
         # If independent_vars and data are alignable (pandas), align them,
         # and apply the mask from above if there is one.
         for var in self.independent_vars:
             if not np.isscalar(kwargs[var]):
                 kwargs[var] = _align(kwargs[var], mask, data)
 
-        # Make sure `dtype` for data is always `float64` or `complex128`
-        if np.isrealobj(data):
-            data = np.asfarray(data)
-        elif np.iscomplexobj(data):
-            data = np.asarray(data, dtype='complex128')
-
-        # Coerce `dtype` for independent variable(s) to `float64` or
-        # `complex128` when the variable has one of the following types: list,
-        # tuple, numpy.ndarray, or pandas.Series
+        def coerce_arraylike(x):
+            """
+            coerce lists, tuples, and pandas Series to float64 or complex128,
+            but leave other ndarrays of different dtypes and objects unchanged
+            """
+            if isinstance(x, (list, tuple, Series)):
+                if np.isrealobj(x):
+                    return np.asfarray(x)
+                elif np.iscomplexobj(x):
+                    return np.asarray(x, dtype='complex128')
+            return x
+
+        # coerce data and independent variable(s) that are 'array-like' (list,
+        # tuples, pandas Series) to float64/complex128. Note: this will not
+        # alter the dtype of data or independent variables that are already
+        # ndarrays but with dtype other than float64/complex128.
+        data = coerce_arraylike(data)
         for var in self.independent_vars:
-            var_data = kwargs[var]
-            if isinstance(var_data, (list, tuple, np.ndarray, Series)):
-                if np.isrealobj(var_data):
-                    kwargs[var] = np.asfarray(var_data)
-                elif np.iscomplexobj(var_data):
-                    kwargs[var] = np.asarray(var_data, dtype='complex128')
+            kwargs[var] = coerce_arraylike(kwargs[var])
 
         if fit_kws is None:
             fit_kws = {}
 
         output = ModelResult(self, params, method=method, iter_cb=iter_cb,
                              scale_covar=scale_covar, fcn_kws=kwargs,
                              nan_policy=self.nan_policy, calc_covar=calc_covar,
@@ -1608,15 +1638,15 @@
             Text of formatted report on confidence intervals.
 
         """
         return ci_report(self.conf_interval(**kwargs),
                          with_offset=with_offset, ndigits=ndigits)
 
     def fit_report(self, modelpars=None, show_correl=True,
-                   min_correl=0.1, sort_pars=False):
+                   min_correl=0.1, sort_pars=False, correl_mode='list'):
         """Return a printable fit report.
 
         The report contains fit statistics and best-fit values with
         uncertainties and correlations.
 
 
         Parameters
@@ -1629,34 +1659,93 @@
             Smallest correlation in absolute value to show (default is 0.1).
         sort_pars : callable, optional
             Whether to show parameter names sorted in alphanumerical order
             (default is False). If False, then the parameters will be
             listed in the order as they were added to the Parameters
             dictionary. If callable, then this (one argument) function is
             used to extract a comparison key from each list element.
+        correl_mode : {'list', table'} str, optional
+            Mode for how to show correlations. Can be either 'list' (default)
+            to show a sorted (if ``sort_pars`` is True) list of correlation
+            values, or 'table' to show a complete, formatted table of
+            correlations.
 
         Returns
         -------
         str
             Multi-line text of fit report.
 
         """
-        report = fit_report(self, modelpars=modelpars,
-                            show_correl=show_correl,
-                            min_correl=min_correl, sort_pars=sort_pars)
+        report = fit_report(self, modelpars=modelpars, show_correl=show_correl,
+                            min_correl=min_correl, sort_pars=sort_pars,
+                            correl_mode=correl_mode)
+
         modname = self.model._reprstring(long=True)
         return f'[[Model]]\n    {modname}\n{report}'
 
     def _repr_html_(self, show_correl=True, min_correl=0.1):
         """Return a HTML representation of parameters data."""
         report = fitreport_html_table(self, show_correl=show_correl,
                                       min_correl=min_correl)
         modname = self.model._reprstring(long=True)
         return f"<h2> Model</h2> {modname} {report}"
 
+    def summary(self):
+        """Return a dictionary with statistics and attributes of a ModelResult.
+
+        Returns
+        -------
+        dict
+            Dictionary of statistics and many attributes from a ModelResult.
+
+        Notes
+        ------
+        1. values for data arrays are not included.
+
+        2. The result summary dictionary will include the following entries:
+
+          ``model``, ``method``, ``ndata``, ``nvarys``, ``nfree``, ``chisqr``,
+          ``redchi``, ``aic``, ``bic``, ``rsquared``, ``nfev``, ``max_nfev``,
+          ``aborted``, ``errorbars``, ``success``, ``message``,
+          ``lmdif_message``, ``ier``, ``nan_policy``, ``scale_covar``,
+          ``calc_covar``, ``ci_out``, ``col_deriv``, ``flatchain``,
+          ``call_kws``, ``var_names``, ``user_options``, ``kws``,
+          ``init_values``, ``best_values``, and ``params``.
+
+        where 'params' is a list of parameter "states": tuples with entries of
+        ``(name, value, vary, expr, min, max, brute_step, stderr, correl,
+        init_value, user_data)``.
+
+        3. The result will include only plain Python objects, and so should be
+        easily serializable with JSON or similar tools.
+
+        """
+        summary = {'model': self.model._reprstring(long=True),
+                   'method': self.method}
+
+        for attr in ('ndata', 'nvarys', 'nfree', 'chisqr', 'redchi', 'aic',
+                     'bic', 'rsquared', 'nfev', 'max_nfev', 'aborted',
+                     'errorbars', 'success', 'message', 'lmdif_message', 'ier',
+                     'nan_policy', 'scale_covar', 'calc_covar', 'ci_out',
+                     'col_deriv', 'flatchain', 'call_kws', 'var_names',
+                     'user_options', 'kws', 'init_values', 'best_values'):
+            val = getattr(self, attr, None)
+            if isinstance(val, np.float64):
+                val = float(val)
+            elif isinstance(val, (np.int32, np.int64)):
+                val = int(val)
+            elif isinstance(val, np.bool_):
+                val = bool(val)
+            elif isinstance(val, bytes):
+                val = str(val, encoding='UTF-8')
+            summary[attr] = val
+
+        summary['params'] = [par.__getstate__() for par in self.params.values()]
+        return summary
+
     def dumps(self, **kws):
         """Represent ModelResult as a JSON string.
 
         Parameters
         ----------
         **kws : optional
             Keyword arguments that are passed to `json.dumps`.
@@ -1678,18 +1767,17 @@
         out['unique_symbols'] = {key: encode4js(pasteval.symtable[key])
                                  for key in pasteval.user_defined_symbols()}
 
         for attr in ('aborted', 'aic', 'best_values', 'bic', 'chisqr',
                      'ci_out', 'col_deriv', 'covar', 'errorbars', 'flatchain',
                      'ier', 'init_values', 'lmdif_message', 'message',
                      'method', 'nan_policy', 'ndata', 'nfev', 'nfree',
-                     'nvarys', 'redchi', 'rsquared', 'scale_covar',
+                     'nvarys', 'redchi', 'residual', 'rsquared', 'scale_covar',
                      'calc_covar', 'success', 'userargs', 'userkws', 'values',
                      'var_names', 'weights', 'user_options'):
-
             try:
                 val = getattr(self, attr)
             except AttributeError:
                 continue
             if isinstance(val, np.bool_):
                 val = bool(val)
 
@@ -1754,28 +1842,23 @@
         if 'model' not in modres or 'params' not in modres:
             raise AttributeError('ModelResult.loads() needs valid ModelResult')
 
         # model
         self.model = _buildmodel(decode4js(modres['model']), funcdefs=funcdefs)
 
         # params
-        self.params = Parameters()
-        self.init_params = Parameters()
-        state = {'unique_symbols': modres['unique_symbols'], 'params': []}
-        ini_state = {'unique_symbols': modres['unique_symbols'], 'params': []}
-        for parstate in modres['params']:
-            _par = Parameter(name='')
-            _par.__setstate__(parstate)
-            state['params'].append(_par)
-            _par = Parameter(name='')
-            _par.__setstate__(parstate)
-            ini_state['params'].append(_par)
-
-        self.params.__setstate__(state)
-        self.init_params.__setstate__(ini_state)
+        for target in ('params', 'init_params'):
+            state = {'unique_symbols': modres['unique_symbols'], 'params': []}
+            for parstate in modres['params']:
+                _par = Parameter(name='')
+                _par.__setstate__(parstate)
+                state['params'].append(_par)
+            _params = Parameters()
+            _params.__setstate__(state)
+            setattr(self, target, _params)
 
         for attr in ('aborted', 'aic', 'best_fit', 'best_values', 'bic',
                      'chisqr', 'ci_out', 'col_deriv', 'covar', 'data',
                      'errorbars', 'fjac', 'flatchain', 'ier', 'init_fit',
                      'init_values', 'kws', 'lmdif_message', 'message',
                      'method', 'nan_policy', 'ndata', 'nfev', 'nfree',
                      'nvarys', 'redchi', 'residual', 'rsquared', 'scale_covar',
```

### Comparing `lmfit-1.1.0/lmfit/models.py` & `lmfit-1.2.0/lmfit/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
 
     def __init__(self, independent_vars=['x'], prefix='', nan_policy='raise',
                  **kwargs):
         kwargs.update({'prefix': prefix, 'nan_policy': nan_policy,
                        'independent_vars': independent_vars})
 
         def constant(x, c=0.0):
-            return c
+            return c * np.ones(np.shape(x))
         super().__init__(constant, **kwargs)
 
     def guess(self, data, x=None, **kwargs):
         """Estimate initial model parameter values from data."""
         pars = self.make_params()
 
         pars[f'{self.prefix}c'].set(value=data.mean())
@@ -194,15 +194,15 @@
 
     def __init__(self, independent_vars=['x'], prefix='', nan_policy='raise',
                  name=None, **kwargs):
         kwargs.update({'prefix': prefix, 'nan_policy': nan_policy,
                        'independent_vars': independent_vars})
 
         def constant(x, re=0., im=0.):
-            return re + 1j*im
+            return (re + 1j*im) * np.ones(np.shape(x))
         super().__init__(constant, **kwargs)
 
     def guess(self, data, x=None, **kwargs):
         """Estimate initial model parameter values from data."""
         pars = self.make_params()
         pars[f'{self.prefix}re'].set(value=data.real.mean())
         pars[f'{self.prefix}im'].set(value=data.imag.mean())
```

### Comparing `lmfit-1.1.0/lmfit/parameter.py` & `lmfit-1.2.0/lmfit/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,33 +87,39 @@
         The method needs to make sure that `asteval` is available and that
         all individual Parameter objects are copied.
 
         """
         _pars = self.__class__()
 
         # find the symbols that were added by users, not during construction
-        unique_symbols = {key: self._asteval.symtable[key]
-                          for key in self._asteval.user_defined_symbols()}
+        unique_symbols = {}
+        for key in self._asteval.user_defined_symbols():
+            try:
+                val = deepcopy(self._asteval.symtable[key])
+                unique_symbols[key] = val
+            except (TypeError, ValueError):
+                unique_symbols[key] = self._asteval.symtable[key]
+
         _pars._asteval.symtable.update(unique_symbols)
 
         # we're just about to add a lot of Parameter objects to the newly
         parameter_list = []
         for key, par in self.items():
             if isinstance(par, Parameter):
                 param = Parameter(name=par.name,
                                   value=par.value,
                                   min=par.min,
                                   max=par.max)
                 param.vary = par.vary
                 param.brute_step = par.brute_step
                 param.stderr = par.stderr
-                param.correl = par.correl
+                param.correl = deepcopy(par.correl)
                 param.init_value = par.init_value
                 param.expr = par.expr
-                param.user_data = par.user_data
+                param.user_data = deepcopy(par.user_data)
                 parameter_list.append(param)
 
         _pars.add_many(*parameter_list)
 
         return _pars
 
     def __setitem__(self, key, par):
@@ -315,14 +321,57 @@
             print(line.format(name_len=name_len, n=colwidth, p=precision,
                               f=fmt, **pvalues))
 
     def _repr_html_(self):
         """Return a HTML representation of parameters data."""
         return params_html_table(self)
 
+    def set(self, **kws):
+        """Set Parameter values and other attributes.
+
+        Parameters
+        ----------
+        **kws : optional
+            Parameter names and initial values or dictionaries of
+                 values and attributes.
+
+        Returns
+        -------
+        None
+
+        Notes
+        -----
+        1. keyword arguments will be used to create parameter names.
+        2. values can either be numbers (floats or integers) to set the
+           parameter value, or can be dictionaries with any of the following
+           keywords: ``value``, ``vary``, ``min``, ``max``, ``expr``,
+           ``brute_step``, or ``is_init_value`` to set those parameter attributes.
+        3. for each parameter,  ``is_init_value`` controls whether to set
+           ``init_value`` when setting ``value``, and defaults to True.
+
+        Examples
+        --------
+        >>> params = Parameters()
+        >>> params.add('xvar', value=0.50, min=0, max=1)
+        >>> params.add('yvar', expr='1.0 - xvar')
+        >>> params.set(xvar=0.80, zvar={'value':3, 'min':0})
+
+        """
+        for name, val in kws.items():
+            if name not in self:
+                self.__setitem__(name, Parameter(value=-inf, name=name,
+                                                 vary=True, min=-inf, max=inf,
+                                                 expr=None, brute_step=None))
+            par = self.__getitem__(name)
+            if isinstance(val, (float, int)):
+                val = {'value': val}
+            if 'is_init_value' not in val:
+                val['is_init_value'] = True
+            par.set(**val)
+
     def add(self, name, value=None, vary=True, min=-inf, max=inf, expr=None,
             brute_step=None):
         """Add a Parameter.
 
         Parameters
         ----------
         name : str or Parameter
@@ -586,28 +635,28 @@
         """
         self.name = name
         self.user_data = user_data
         self.init_value = value
         self.min = min
         self.max = max
         self.brute_step = brute_step
-        self.vary = vary
+        self._vary = vary
         self._expr = expr
         self._expr_ast = None
         self._expr_eval = None
         self._expr_deps = []
         self._delay_asteval = False
         self.stderr = None
         self.correl = None
         self.from_internal = lambda val: val
         self._val = value
         self._init_bounds()
 
     def set(self, value=None, vary=None, min=None, max=None, expr=None,
-            brute_step=None):
+            brute_step=None, is_init_value=True):
         """Set or update Parameter attributes.
 
         Parameters
         ----------
         value : float, optional
             Numerical Parameter value.
         vary : bool, optional
@@ -620,14 +669,16 @@
             ``numpy.inf``.
         expr : str, optional
             Mathematical expression used to constrain the value during the
             fit. To remove a constraint you must supply an empty string.
         brute_step : float, optional
             Step size for grid points in the `brute` method. To remove the
             step size you must use ``0``.
+        is_init_value: bool, optional
+            Whether to set value as `init_value`, when setting value.
 
         Notes
         -----
         Each argument to `set()` has a default value of None, which will
         leave the current value for the attribute unchanged. Thus, to lift
         a lower or upper bound, passing in None will not work. Instead,
         you must set these to ``-numpy.inf`` or ``numpy.inf``, as with::
@@ -647,28 +698,31 @@
         Finally, to clear the brute_step size, pass ``0``, not None::
 
             par.set(brute_step=None)  # leaves brute_step unchanged
             par.set(brute_step=0)     # removes brute_step
 
         """
         if vary is not None:
-            self.vary = vary
+            self._vary = vary
             if vary:
                 self.__set_expression('')
 
         if min is not None:
             self.min = min
 
         if max is not None:
             self.max = max
 
         # need to set this after min and max, so that it will use new
         # bounds in the setter for value
         if value is not None:
+            is_init_value = is_init_value or self.value in (None, -inf, inf)
             self.value = value
+            if is_init_value:
+                self.init_value = value
             self.__set_expression("")
 
         if expr is not None:
             self.__set_expression(expr)
 
         if brute_step is not None:
             if brute_step == 0.0:
@@ -693,36 +747,36 @@
             self._val = self.max
         if self._val < self.min:
             self._val = self.min
         self.setup_bounds()
 
     def __getstate__(self):
         """Get state for pickle."""
-        return (self.name, self.value, self.vary, self.expr, self.min,
+        return (self.name, self.value, self._vary, self.expr, self.min,
                 self.max, self.brute_step, self.stderr, self.correl,
                 self.init_value, self.user_data)
 
     def __setstate__(self, state):
         """Set state for pickle."""
-        (self.name, _value, self.vary, self.expr, self.min, self.max,
+        (self.name, _value, self._vary, self.expr, self.min, self.max,
          self.brute_step, self.stderr, self.correl, self.init_value,
          self.user_data) = state
         self._expr_ast = None
         self._expr_eval = None
         self._expr_deps = []
         self._delay_asteval = False
         self._val = _value
         self._init_bounds()
         self.value = _value
 
     def __repr__(self):
         """Return printable representation of a Parameter object."""
         s = []
         sval = f"value={repr(self._getval())}"
-        if not self.vary and self._expr is None:
+        if not self._vary and self._expr is None:
             sval += " (fixed)"
         elif self.stderr is not None:
             sval += f" +/- {self.stderr:.3g}"
         s.append(sval)
         s.append(f"bounds=[{repr(self.min)}:{repr(self.max)}]")
         if self._expr is not None:
             s.append(f"expr='{self.expr}'")
@@ -825,14 +879,26 @@
                 self._val = self.min
         if not hasattr(self, '_expr_eval'):
             self._expr_eval = None
         if self._expr_eval is not None:
             self._expr_eval.symtable[self.name] = self._val
 
     @property
+    def vary(self):
+        """Return whether the parameter is variable"""
+        return self._vary
+
+    @vary.setter
+    def vary(self, val):
+        """Set whether a parameter is varied"""
+        self._vary = val
+        if val:
+            self.__set_expression('')
+
+    @property
     def expr(self):
         """Return the mathematical expression used to constrain the value in fit."""
         return self._expr
 
     @expr.setter
     def expr(self, val):
         """Set the mathematical expression used to constrain the value in fit.
@@ -843,15 +909,15 @@
         self.__set_expression(val)
 
     def __set_expression(self, val):
         if val == '':
             val = None
         self._expr = val
         if val is not None:
-            self.vary = False
+            self._vary = False
         if not hasattr(self, '_expr_eval'):
             self._expr_eval = None
         if val is None:
             self._expr_ast = None
         if val is not None and self._expr_eval is not None:
             self._expr_eval.error = []
             self._expr_eval.error_msg = None
@@ -978,7 +1044,41 @@
     def __rpow__(self, other):
         """** (right)"""
         return other ** self._getval()
 
     def __rsub__(self, other):
         """- (right)"""
         return other - self._getval()
+
+
+def create_params(**kws):
+    """Create lmfit.Parameters instance and set initial values and attributes.
+
+    Parameters
+    ----------
+    **kws
+        keywords are parameter names, value are dictionaries of Parameter
+        values and attributes.
+
+    Returns
+    -------
+    Parameters instance
+
+    Notes
+    -----
+    1. keyword arguments will be used to create parameter names.
+    2. values can either be numbers (floats or integers) to set the parameter
+       value, or can be dictionaries with any of the following keywords:
+       ``value``, ``vary``, ``min``, ``max``, ``expr``, ``brute_step``, or
+       ``is_init_value`` to set those parameter attributes.
+    3. for each parameter,  ``is_init_value`` controls whether to set
+       ``init_value`` when setting ``value``, and defaults to True.
+
+    Examples
+    --------
+    >>> params = create_params(amplitude=2, center=200,
+                               sigma={'value': 3, 'min':0},
+                               fwhm={'expr': '2.0*sigma'})
+    """
+    params = Parameters()
+    params.set(**kws)
+    return params
```

### Comparing `lmfit-1.1.0/lmfit/printfuncs.py` & `lmfit-1.2.0/lmfit/printfuncs.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,18 +54,23 @@
         String of specified length.
 
     Notes
     ------
     Positive values will have leading blank.
 
     """
+    if val is None or isinstance(val, bool):
+        return f'{repr(val):>{length}s}'
     try:
         expon = int(log10(abs(val)))
     except (OverflowError, ValueError):
         expon = 0
+    except TypeError:
+        return f'{repr(val):>{length}s}'
+
     length = max(length, 7)
     form = 'e'
     prec = length - 7
     if abs(expon) > 99:
         prec -= 1
     elif ((expon > 0 and expon < (prec+4)) or
           (expon <= 0 and -expon < (prec-1))):
@@ -73,15 +78,15 @@
         prec += 4
         if expon > 0:
             prec -= expon
     return f'{val:{length}.{prec}{form}}'
 
 
 def fit_report(inpars, modelpars=None, show_correl=True, min_correl=0.1,
-               sort_pars=False):
+               sort_pars=False, correl_mode='list'):
     """Generate a report of the fitting results.
 
     The report contains the best-fit values for the parameters and their
     uncertainties and correlations.
 
     Parameters
     ----------
@@ -95,14 +100,19 @@
         Smallest correlation in absolute value to show (default is 0.1).
     sort_pars : bool or callable, optional
         Whether to show parameter names sorted in alphanumerical order. If
         False (default), then the parameters will be listed in the order
         they were added to the Parameters dictionary. If callable, then
         this (one argument) function is used to extract a comparison key
         from each list element.
+    correl_mode : {'list', table'} str, optional
+        Mode for how to show correlations. Can be either 'list' (default)
+        to show a sorted (if ``sort_pars`` is True) list of correlation
+        values, or 'table' to show a complete, formatted table of
+        correlations.
 
     Returns
     -------
     str
         Multi-line text of fit report.
 
     """
@@ -182,15 +192,19 @@
         if par.vary:
             add(f"    {nout} {sval} {inval}")
         elif par.expr is not None:
             add(f"    {nout} {sval} == '{par.expr}'")
         else:
             add(f"    {nout} {par.value: .7g} (fixed)")
 
-    if show_correl:
+    if show_correl and correl_mode.startswith('tab'):
+        add('[[Correlations]] ')
+        for line in correl_table(params).split('\n'):
+            buff.append('  %s' % line)
+    elif show_correl:
         correls = {}
         for i, name in enumerate(parnames):
             par = params[name]
             if not par.vary:
                 continue
             if hasattr(par, 'correl') and par.correl is not None:
                 for name2 in parnames[i+1:]:
@@ -202,15 +216,15 @@
         sort_correl.reverse()
         if len(sort_correl) > 0:
             add('[[Correlations]] (unreported correlations are < '
                 f'{min_correl:.3f})')
             maxlen = max(len(k) for k in list(correls.keys()))
         for name, val in sort_correl:
             lspace = max(0, maxlen - len(name))
-            add(f"    C({name}){(' '*30)[:lspace]} = {val:.3f}")
+            add(f"    C({name}){(' '*30)[:lspace]} = {val:+.4f}")
     return '\n'.join(buff)
 
 
 def fitreport_html_table(result, show_correl=True, min_correl=0.1):
     """Generate a report of the fitting result as an HTML table.
 
     Parameters
@@ -265,19 +279,55 @@
         if len(correls) > 0:
             sort_correls = sorted(correls, key=lambda val: abs(val[2]))
             sort_correls.reverse()
             extra = f'(unreported correlations are < {min_correl:.3f})'
             add(f'<h2>Correlations {extra}</h2>')
             add('<table>')
             for name1, name2, val in sort_correls:
-                stat_row(name1, name2, f"{val:.4f}")
+                stat_row(name1, name2, f"{val:+.4f}")
             add('</table>')
     return ''.join(html)
 
 
+def correl_table(params):
+    """Return a printable correlation table for a Parameters object."""
+    varnames = [vname for vname in params if params[vname].vary]
+    nwid = max(8, max([len(vname) for vname in varnames])) + 1
+
+    def sfmt(a):
+        return f" {a:{nwid}s}"
+
+    def ffmt(a):
+        return sfmt(f"{a:+.4f}")
+
+    title = ['', sfmt('Variable')]
+    title.extend([sfmt(vname) for vname in varnames])
+
+    title = '|'.join(title) + '|'
+    bar = [''] + ['-'*(nwid+1) for i in range(len(varnames)+1)] + ['']
+    bar = '+'.join(bar)
+
+    buff = [bar, title, bar]
+
+    for vname, par in params.items():
+        if not par.vary:
+            continue
+        line = ['', sfmt(vname)]
+        for vother in varnames:
+            if vother == vname:
+                line.append(ffmt(1))
+            elif vother in par.correl:
+                line.append(ffmt(par.correl[vother]))
+            else:
+                line.append('unknown')
+        buff.append('|'.join(line) + '|')
+    buff.append(bar)
+    return '\n'.join(buff)
+
+
 def params_html_table(params):
     """Return an HTML representation of Parameters.
 
     Parameters
     ----------
     params : Parameters
         Object containing the Parameters of the model.
```

### Comparing `lmfit-1.1.0/lmfit.egg-info/PKG-INFO` & `lmfit-1.2.0/lmfit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmfit
-Version: 1.1.0
+Version: 1.2.0
 Summary: Least-Squares Minimization with Bounds and Constraints
 Home-page: https://lmfit.github.io//lmfit-py/
 Author: LMFit Development Team
 Author-email: matt.newville@gmail.com
 License: BSD 3-Clause
 Project-URL: Source, https://github.com/lmfit/lmfit-py
 Project-URL: Changelog, https://lmfit.github.io/lmfit-py/whatsnew.html
```

### Comparing `lmfit-1.1.0/lmfit.egg-info/SOURCES.txt` & `lmfit-1.2.0/lmfit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 examples/doc_builtinmodels_nistgauss.py
 examples/doc_builtinmodels_nistgauss2.py
 examples/doc_builtinmodels_peakmodels.py
 examples/doc_builtinmodels_splinemodel.py
 examples/doc_builtinmodels_stepmodel.py
 examples/doc_confidence_advanced.py
 examples/doc_confidence_basic.py
+examples/doc_confidence_chi2_maps.py
 examples/doc_fitting_emcee.py
 examples/doc_fitting_withreport.py
 examples/doc_model_composite.py
 examples/doc_model_gaussian.py
 examples/doc_model_loadmodel.py
 examples/doc_model_loadmodelresult.py
 examples/doc_model_loadmodelresult2.py
@@ -144,14 +145,15 @@
 lmfit.egg-info/SOURCES.txt
 lmfit.egg-info/dependency_links.txt
 lmfit.egg-info/requires.txt
 lmfit.egg-info/top_level.txt
 tests/NISTModels.py
 tests/__init__.py
 tests/conftest.py
+tests/gauss_modelresult_lmfit100.sav
 tests/test_1variable.py
 tests/test_NIST_Strd.py
 tests/test_algebraic_constraint.py
 tests/test_ampgo.py
 tests/test_basicfit.py
 tests/test_basinhopping.py
 tests/test_bounded_jacobian.py
```

### Comparing `lmfit-1.1.0/lmfit.egg-info/requires.txt` & `lmfit-1.2.0/lmfit.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 flaky
 pytest
 pytest-cov
 cairosvg
 corner
 dill
 emcee>=3.0.0
+ipykernel
 jupyter_sphinx>=0.2.4
 matplotlib
 numdifftools
 pandas
 Pillow
 Sphinx
 sphinx-gallery>=0.10
@@ -37,14 +38,15 @@
 twine
 
 [doc]
 cairosvg
 corner
 dill
 emcee>=3.0.0
+ipykernel
 jupyter_sphinx>=0.2.4
 matplotlib
 numdifftools
 pandas
 Pillow
 Sphinx
 sphinx-gallery>=0.10
```

### Comparing `lmfit-1.1.0/publish_docs.sh` & `lmfit-1.2.0/publish_docs.sh`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/setup.cfg` & `lmfit-1.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 	pre-commit
 	twine
 doc = 
 	cairosvg
 	corner
 	dill
 	emcee>=3.0.0
+	ipykernel
 	jupyter_sphinx>=0.2.4
 	matplotlib
 	numdifftools
 	pandas
 	Pillow
 	pycairo;platform_system=="Windows"
 	Sphinx
```

### Comparing `lmfit-1.1.0/tests/NISTModels.py` & `lmfit-1.2.0/tests/NISTModels.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/conftest.py` & `lmfit-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_1variable.py` & `lmfit-1.2.0/tests/test_1variable.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_NIST_Strd.py` & `lmfit-1.2.0/tests/test_NIST_Strd.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_algebraic_constraint.py` & `lmfit-1.2.0/tests/test_algebraic_constraint.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_ampgo.py` & `lmfit-1.2.0/tests/test_ampgo.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,22 +100,22 @@
         minimizer_Alpine02.minimize(method='ampgo', **kws)
 
 
 @pytest.mark.skipif(sys.version_info.major == 2,
                     reason="does not throw an exception in Python 2")
 def test_ampgo_local_opts(minimizer_Alpine02):
     """Test AMPGO algorithm, pass local_opts to solver."""
-    # use local_opts to pass maxiter to the local optimizer: providing a string
+    # use local_opts to pass maxfun to the local optimizer: providing a string
     # whereas an integer is required, this should throw an error.
-    kws = {'local_opts': {'maxiter': 'string'}}
+    kws = {'local_opts': {'maxfun': 'string'}}
     with pytest.raises(TypeError):
         minimizer_Alpine02.minimize(method='ampgo', **kws)
 
     # for coverage: make sure that both occurrences are reached
-    kws = {'local_opts': {'maxiter': 10}, 'maxfunevals': 50}
+    kws = {'local_opts': {'maxfun': 10}, 'maxfunevals': 50}
     minimizer_Alpine02.minimize(method='ampgo', **kws)
 
 
 def test_ampgo_incorrect_length_for_bounds():
     """Test for ValueError when bounds are given for only some parameters."""
     def func(x):
         return x[0]**2 + 10.0*x[1]
```

### Comparing `lmfit-1.1.0/tests/test_basicfit.py` & `lmfit-1.2.0/tests/test_basicfit.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_basinhopping.py` & `lmfit-1.2.0/tests/test_basinhopping.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_bounded_jacobian.py` & `lmfit-1.2.0/tests/test_bounded_jacobian.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_bounds.py` & `lmfit-1.2.0/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_brute.py` & `lmfit-1.2.0/tests/test_brute.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_builtin_models.py` & `lmfit-1.2.0/tests/test_builtin_models.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_confidence.py` & `lmfit-1.2.0/tests/test_confidence.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_covariance_matrix.py` & `lmfit-1.2.0/tests/test_covariance_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,46 +37,47 @@
     params = Parameters()
     params.add('amp', value=10, min=0, max=50)
     params.add('decay', value=0.1, min=0, max=10)
     params.add('shift', value=0.0, min=-pi/2., max=pi/2.)
     params.add('omega', value=3.0, min=0, max=np.inf)
 
     # do fit, here with leastsq model
-    result = minimize(fcn2min, params, args=(x, data))
+    result = minimize(fcn2min, params, args=(x, data),
+                      epsfcn=1.e-14)
 
     # assert that the real parameters are found
     for para, val in zip(result.params.values(), [5, 0.025, -.1, 2]):
         check(para, val)
 
     # assert that the covariance matrix is correct [cf. lmfit v0.9.10]
     cov_x = np.array([
         [1.42428250e-03, 9.45395985e-06, -4.33997922e-05, 1.07362106e-05],
         [9.45395985e-06, 1.84110424e-07, -2.90588963e-07, 7.19107184e-08],
         [-4.33997922e-05, -2.90588963e-07, 9.53427031e-05, -2.37750362e-05],
         [1.07362106e-05, 7.19107184e-08, -2.37750362e-05, 9.60952336e-06]])
-    assert_allclose(result.covar, cov_x, rtol=1.5e-6)
+    assert_allclose(result.covar, cov_x, rtol=1.e-3, atol=1.e-6)
 
     # assert that stderr and correlations are correct [cf. lmfit v0.9.10]
-    assert_almost_equal(result.params['amp'].stderr, 0.03773967, decimal=6)
-    assert_almost_equal(result.params['decay'].stderr, 4.2908e-04, decimal=6)
-    assert_almost_equal(result.params['shift'].stderr, 0.00976436, decimal=6)
-    assert_almost_equal(result.params['omega'].stderr, 0.00309992, decimal=6)
+    assert_almost_equal(result.params['amp'].stderr, 0.03773967, decimal=4)
+    assert_almost_equal(result.params['decay'].stderr, 4.2908e-04, decimal=4)
+    assert_almost_equal(result.params['shift'].stderr, 0.00976436, decimal=4)
+    assert_almost_equal(result.params['omega'].stderr, 0.00309992, decimal=4)
 
     assert_almost_equal(result.params['amp'].correl['decay'],
-                        0.5838166760743324, decimal=6)
+                        0.5838166760743324, decimal=4)
     assert_almost_equal(result.params['amp'].correl['shift'],
-                        -0.11777303073961824, decimal=6)
+                        -0.11777303073961824, decimal=4)
     assert_almost_equal(result.params['amp'].correl['omega'],
-                        0.09177027400788784, decimal=6)
+                        0.09177027400788784, decimal=4)
     assert_almost_equal(result.params['decay'].correl['shift'],
-                        -0.0693579417651835, decimal=6)
+                        -0.0693579417651835, decimal=4)
     assert_almost_equal(result.params['decay'].correl['omega'],
-                        0.05406342001021014, decimal=6)
+                        0.05406342001021014, decimal=4)
     assert_almost_equal(result.params['shift'].correl['omega'],
-                        -0.7854644476455469, decimal=6)
+                        -0.7854644476455469, decimal=4)
 
 
 def test_bounds_expression():
     # load data to be fitted
     data = np.loadtxt(os.path.join(os.path.dirname(__file__), '..', 'examples',
                                    'test_peak.dat'))
     x = data[:, 0]
@@ -85,31 +86,31 @@
     # define the model and initialize parameters
     mod = VoigtModel()
     params = mod.guess(y, x=x)
     params['amplitude'].set(min=0, max=100)
     params['center'].set(min=5, max=10)
 
     # do fit, here with leastsq model
-    result = mod.fit(y, params, x=x)
+    result = mod.fit(y, params, x=x, fit_kws={'epsfcn': 1.e-14})
 
     # assert that stderr and correlations are correct [cf. lmfit v0.9.10]
-    assert_almost_equal(result.params['sigma'].stderr, 0.00368468, decimal=6)
-    assert_almost_equal(result.params['center'].stderr, 0.00505496, decimal=6)
+    assert_almost_equal(result.params['sigma'].stderr, 0.00368468, decimal=4)
+    assert_almost_equal(result.params['center'].stderr, 0.00505496, decimal=4)
     assert_almost_equal(result.params['amplitude'].stderr, 0.13861506,
-                        decimal=6)
-    assert_almost_equal(result.params['gamma'].stderr, 0.00368468, decimal=6)
-    assert_almost_equal(result.params['fwhm'].stderr, 0.00806917, decimal=6)
-    assert_almost_equal(result.params['height'].stderr, 0.03009459, decimal=6)
+                        decimal=4)
+    assert_almost_equal(result.params['gamma'].stderr, 0.00368468, decimal=4)
+    assert_almost_equal(result.params['fwhm'].stderr, 0.01326862028, decimal=4)
+    assert_almost_equal(result.params['height'].stderr, 0.0395990, decimal=4)
 
     assert_almost_equal(result.params['sigma'].correl['center'],
-                        -4.6623973788006615e-05, decimal=6)
+                        -4.6623973788006615e-05, decimal=4)
     assert_almost_equal(result.params['sigma'].correl['amplitude'],
-                        0.651304091954038, decimal=6)
+                        0.651304091954038, decimal=4)
     assert_almost_equal(result.params['center'].correl['amplitude'],
-                        -4.390334984618851e-05, decimal=6)
+                        -4.390334984618851e-05, decimal=4)
 
 
 @pytest.mark.parametrize("fit_method", ['nelder', 'lbfgs'])
 def test_numdifftools_no_bounds(fit_method):
     pytest.importorskip("numdifftools")
 
     np.random.seed(7)
```

### Comparing `lmfit-1.1.0/tests/test_custom_independentvar.py` & `lmfit-1.2.0/tests/test_custom_independentvar.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_default_kws.py` & `lmfit-1.2.0/tests/test_default_kws.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_dual_annealing.py` & `lmfit-1.2.0/tests/test_dual_annealing.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_itercb.py` & `lmfit-1.2.0/tests/test_itercb.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_jsonutils.py` & `lmfit-1.2.0/tests/test_jsonutils.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_least_squares.py` & `lmfit-1.2.0/tests/test_least_squares.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,16 @@
         params['sigma'].set(min=0, max=1)
         params['center'].set(min=5, max=15)
     else:
         params['sigma'].set(min=-np.inf)
 
     # do fit with least_squares and leastsq algorithm
     result = mod.fit(y, params, x=x, method='least_squares')
-    result_lsq = mod.fit(y, params, x=x, method='leastsq')
+    result_lsq = mod.fit(y, params, x=x, method='leastsq',
+                         fit_kws={'epsfcn': 1.e-14})
 
     # assert that fit converged to the same result
     vals = [result.params[p].value for p in result.params.valuesdict()]
     vals_lsq = [result_lsq.params[p].value for p in
                 result_lsq.params.valuesdict()]
     assert_allclose(vals, vals_lsq, rtol=1e-5)
     assert_allclose(result.chisqr, result_lsq.chisqr)
@@ -99,15 +100,16 @@
     # those from the covariance matrix estimated from the Jacbian matrix in
     # least_squares are similar
     for par1 in result.var_names:
         cor = [result.params[par1].correl[par2] for par2 in
                result.params[par1].correl.keys()]
         cor_lsq = [result_lsq.params[par1].correl[par2] for par2 in
                    result_lsq.params[par1].correl.keys()]
-        assert_allclose(cor, cor_lsq, rtol=1e-2)
+
+        assert_allclose(cor, cor_lsq, rtol=0.01, atol=1.e-6)
 
 
 def test_least_squares_solver_options(peakdata, capsys):
     """Test least_squares algorithm, pass options to solver."""
     x = peakdata[0]
     y = peakdata[1]
     mod = VoigtModel()
```

### Comparing `lmfit-1.1.0/tests/test_lineshapes.py` & `lmfit-1.2.0/tests/test_lineshapes.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_manypeaks_speed.py` & `lmfit-1.2.0/tests/test_manypeaks_speed.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_max_nfev.py` & `lmfit-1.2.0/tests/test_max_nfev.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_minimizer.py` & `lmfit-1.2.0/tests/test_minimizer.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_model.py` & `lmfit-1.2.0/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import sys
 import unittest
 import warnings
 
 import numpy as np
 from numpy.testing import assert_allclose
 import pytest
+from scipy import __version__ as scipy_version
 
 import lmfit
 from lmfit import Model, models
 from lmfit.lineshapes import gaussian, lorentzian
 from lmfit.model import get_reducer, propagate_err
 from lmfit.models import PseudoVoigtModel
 
@@ -353,16 +354,16 @@
         Model(func_invalid_var)
 
     msg = r"Invalid parameter name \('weights'\) for function func_invalid_par"
     with pytest.raises(ValueError, match=msg):
         Model(func_invalid_par)
 
 
-input_dtypes = [(np.int32, np.float64), (np.float32, np.float64),
-                (np.complex64, np.complex128), ('list', np.float64),
+input_dtypes = [(np.int32, np.int32), (np.float32, np.float32),
+                (np.complex64, np.complex64), ('list', np.float64),
                 ('tuple', np.float64), ('pandas-real', np.float64),
                 ('pandas-complex', np.complex128)]
 
 
 @pytest.mark.parametrize('input_dtype, expected_dtype', input_dtypes)
 def test_coercion_of_input_data(peakdata, input_dtype, expected_dtype):
     """Test for coercion of 'data' and 'independent_vars'.
@@ -482,14 +483,44 @@
     assert fig.axes[1].get_title() == ''
 
     fig = result.plot(ax_fit_kws={'title': 'ax_fit_kws'}, title='test')
     assert fig.axes[0].get_title() == 'test'
     assert fig.axes[1].get_title() == ''
 
 
+def test_eval_with_kwargs():
+    # Check eval() with both params and kwargs, even when there are
+    # constraints
+    x = np.linspace(0, 30, 301)
+    np.random.seed(13)
+    y1 = (gaussian(x, amplitude=10, center=12.0, sigma=2.5) +
+          gaussian(x, amplitude=20, center=19.0, sigma=2.5))
+
+    y2 = (gaussian(x, amplitude=10, center=12.0, sigma=1.5) +
+          gaussian(x, amplitude=20, center=19.0, sigma=2.5))
+
+    model = Model(gaussian, prefix='g1_') + Model(gaussian, prefix='g2_')
+    params = model.make_params(g1_amplitude=10, g1_center=12.0, g1_sigma=1,
+                               g2_amplitude=20, g2_center=19.0,
+                               g2_sigma={'expr': 'g1_sigma'})
+
+    r1 = model.eval(params, g1_sigma=2.5, x=x)
+    assert_allclose(r1, y1, atol=1.e-3)
+
+    assert params['g2_sigma'].value == 1
+    assert params['g1_sigma'].value == 1
+
+    params['g1_sigma'].value = 1.5
+    params['g2_sigma'].expr = None
+    params['g2_sigma'].value = 2.5
+
+    r2 = model.eval(params, x=x)
+    assert_allclose(r2, y2, atol=1.e-3)
+
+
 def test_guess_requires_x():
     """Test to make sure that ``guess()`` method requires the argument ``x``.
 
     The ``guess`` method needs ``x`` values (i.e., the independent variable)
     to estimate initial parameters, but this was not a required argument.
     See GH #747.
 
@@ -1180,20 +1211,27 @@
         result = lambda: mod.fit(y, params, x=x, nan_policy='raise')
         msg = ('NaN values detected in your input data or the output of your '
                'objective/model function - fitting algorithms cannot handle this!')
         self.assertRaisesRegex(ValueError, msg, result)
 
         # with propagate, should get no error, but bad results
         result = mod.fit(y, params, x=x, nan_policy='propagate')
-        self.assertTrue(result.success)
-        self.assertTrue(np.isnan(result.chisqr))
-        self.assertTrue(np.isnan(result.aic))
-        self.assertFalse(result.errorbars)
-        self.assertTrue(result.params['amplitude'].stderr is None)
-        self.assertTrue(abs(result.params['amplitude'].value - 20.0) < 0.001)
+
+        # for SciPy v1.10+ this results in an AbortFitException, even with
+        # `max_nfev=100000`:
+        #   lmfit.minimizer.AbortFitException: fit aborted: too many function
+        #   evaluations xxxxx
+        if int(scipy_version.split('.')[1]) < 10:
+            self.assertTrue(np.isnan(result.chisqr))
+            self.assertTrue(np.isnan(result.aic))
+            self.assertFalse(result.errorbars)
+            self.assertTrue(result.params['amplitude'].stderr is None)
+            self.assertTrue(abs(result.params['amplitude'].value - 20.0) < 0.001)
+        else:
+            pass
 
         # with omit, should get good results
         result = mod.fit(y, params, x=x, nan_policy='omit')
         self.assertTrue(result.success)
         self.assertTrue(result.chisqr > 2.0)
         self.assertTrue(result.aic < -100)
         self.assertTrue(result.errorbars)
```

### Comparing `lmfit-1.1.0/tests/test_model_saveload.py` & `lmfit-1.2.0/tests/test_model_saveload.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Tests for saving/loading Models and ModelResults."""
 
+import json
 import os
 import time
 
 import numpy as np
 from numpy.testing import assert_allclose
 import pytest
 
@@ -17,14 +18,16 @@
 
 y, x = np.loadtxt(os.path.join(os.path.dirname(__file__), '..',
                                'examples', 'NIST_Gauss2.dat')).T
 
 SAVE_MODEL = 'model_1.sav'
 SAVE_MODELRESULT = 'modelresult_1.sav'
 
+MODELRESULT_LMFIT_1_0 = 'gauss_modelresult_lmfit100.sav'
+
 
 def clear_savefile(fname):
     """Remove save files so that tests start fresh."""
     try:
         os.unlink(fname)
     except OSError:
         pass
@@ -62,32 +65,32 @@
     model = gauss1 + gauss2 + exp_mod
     return model, params
 
 
 def check_fit_results(result):
     """Check the result of optimization."""
     assert result.nvarys == 8
-    assert_allclose(result.chisqr, 1247.528209)
-    assert_allclose(result.aic, 417.864631)
+    assert_allclose(result.chisqr, 1247.528209, rtol=1.0e-5)
+    assert_allclose(result.aic, 417.864631, rtol=1.0e-5)
 
     pars = result.params
-    assert_allclose(pars['exp_decay'], 90.950886)
-    assert_allclose(pars['exp_amplitude'], 99.018328)
+    assert_allclose(pars['exp_decay'], 90.950886, rtol=1.0e-5)
+    assert_allclose(pars['exp_amplitude'], 99.018328, rtol=1.0e-5)
 
-    assert_allclose(pars['g1_sigma'], 16.672575)
-    assert_allclose(pars['g1_center'], 107.030954)
-    assert_allclose(pars['g1_amplitude'], 4257.773192)
-    assert_allclose(pars['g1_fwhm'], 39.260914)
-    assert_allclose(pars['g1_height'], 101.880231)
-
-    assert_allclose(pars['g2_sigma'], 13.806948)
-    assert_allclose(pars['g2_center'], 153.270101)
-    assert_allclose(pars['g2_amplitude'], 2493.417703)
-    assert_allclose(pars['g2_fwhm'], 32.512878)
-    assert_allclose(pars['g2_height'], 72.045593)
+    assert_allclose(pars['g1_sigma'], 16.672575, rtol=1.0e-5)
+    assert_allclose(pars['g1_center'], 107.030954, rtol=1.0e-5)
+    assert_allclose(pars['g1_amplitude'], 4257.773192, rtol=1.0e-5)
+    assert_allclose(pars['g1_fwhm'], 39.260914, rtol=1.0e-5)
+    assert_allclose(pars['g1_height'], 101.880231, rtol=1.0e-5)
+
+    assert_allclose(pars['g2_sigma'], 13.806948, rtol=1.0e-5)
+    assert_allclose(pars['g2_center'], 153.270101, rtol=1.0e-5)
+    assert_allclose(pars['g2_amplitude'], 2493.417703, rtol=1.0e-5)
+    assert_allclose(pars['g2_fwhm'], 32.512878, rtol=1.0e-5)
+    assert_allclose(pars['g2_height'], 72.045593, rtol=1.0e-5)
 
 
 @pytest.mark.parametrize("dill", [False, True])
 def test_save_load_model(dill):
     """Save/load Model with/without dill."""
     if dill:
         pytest.importorskip("dill")
@@ -144,19 +147,27 @@
     text = ''
     with open(SAVE_MODELRESULT) as fh:
         text = fh.read()
     assert 12000 < len(text) < 60000  # depending on whether dill is present
 
     # load the saved ModelResult from file and compare results
     result_saved = load_modelresult(SAVE_MODELRESULT)
+    assert result_saved.residual is not None
     check_fit_results(result_saved)
 
     clear_savefile(SAVE_MODEL)
 
 
+def test_load_legacy_modelresult():
+    """Load legacy ModelResult."""
+    fname = os.path.join(os.path.dirname(__file__), MODELRESULT_LMFIT_1_0)
+    result_saved = load_modelresult(fname)
+    assert result_saved is not None
+
+
 def test_saveload_modelresult_attributes():
     """Test for restoring all attributes of the ModelResult."""
     model, params = create_model_params(x, y)
     result = model.fit(y, params, x=x)
     save_modelresult(result, SAVE_MODELRESULT)
 
     time.sleep(0.25)
@@ -236,14 +247,15 @@
     result = gmod.fit(y, x=x, amp=5, cen=5, wid=1)
     save_modelresult(result, savefile)
     time.sleep(0.25)
 
     result2 = load_modelresult(savefile)
 
     assert result2 is not None
+    assert result2.residual is not None
     assert result2.init_fit is not None
     assert_allclose((result2.init_fit - result.init_fit).sum() + 1.00, 1.00,
                     rtol=1.0e-2)
     os.unlink(savefile)
 
 
 def test_saveload_usersyms():
@@ -268,10 +280,39 @@
     assert_allclose(result.params['sigma'], 1.075487, rtol=1.0e-5)
     assert_allclose(result.params['center'], 8.489738, rtol=1.0e-5)
     assert_allclose(result.params['height'], 0.557778, rtol=1.0e-5)
 
     time.sleep(0.25)
     result2 = load_modelresult(savefile)
 
+    assert result2.residual is not None
     assert_allclose(result2.params['sigma'], 1.075487, rtol=1.0e-5)
     assert_allclose(result2.params['center'], 8.489738, rtol=1.0e-5)
     assert_allclose(result2.params['height'], 0.557778, rtol=1.0e-5)
+
+
+def test_modelresult_summary():
+    """Test summary() method of ModelResult.
+    """
+    x = np.linspace(0, 20, 501)
+    y = gaussian(x, 1.1, 8.5, 2) + lorentzian(x, 1.7, 8.5, 1.5)
+    np.random.seed(20)
+    y = y + np.random.normal(size=len(x), scale=0.025)
+
+    model = VoigtModel()
+    pars = model.guess(y, x=x)
+    result = model.fit(y, pars, x=x)
+
+    summary = result.summary()
+
+    assert isinstance(summary, dict)
+
+    for attr in ('ndata', 'nvarys', 'nfree', 'chisqr', 'redchi', 'aic',
+                 'bic', 'rsquared', 'nfev', 'max_nfev', 'aborted',
+                 'errorbars', 'success', 'message', 'lmdif_message', 'ier',
+                 'nan_policy', 'scale_covar', 'calc_covar', 'ci_out',
+                 'col_deriv', 'flatchain', 'call_kws', 'var_names',
+                 'user_options', 'kws', 'init_values', 'best_values'):
+        val = summary.get(attr, '__INVALID__')
+        assert val != '__INVALID__'
+
+    assert len(json.dumps(summary)) > 100
```

### Comparing `lmfit-1.1.0/tests/test_model_uncertainties.py` & `lmfit-1.2.0/tests/test_model_uncertainties.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_models.py` & `lmfit-1.2.0/tests/test_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -117,14 +117,29 @@
     assert params['amplitude'] < 5.0
     assert params['frequency'] > 0.1
     assert params['frequency'] < 1.5
     assert params['shift'] > 0.0
     assert params['shift'] < 1.0
 
 
+def testSineModel_make_params():
+    mod = lmfit.models.SineModel()
+    pars = mod.make_params(amplitude=1.5, frequency=0.5,
+                           shift=dict(value=0.4, min=-10, max=10))
+
+    assert pars['amplitude'].value > 1.4
+    assert pars['amplitude'].value < 1.6
+    assert pars['amplitude'].min == 0
+    assert pars['amplitude'].max > 1e99
+    assert pars['shift'].value > 0.35
+    assert pars['shift'].value < 0.45
+    assert pars['shift'].min < -9.5
+    assert pars['shift'].max > 9.5
+
+
 def testSplineModel():
     x = np.linspace(0, 25, 501)
     y = gaussian(x, amplitude=10, center=16.2, sigma=0.8) + 3 + 0.03*x + np.sin(x/4)
 
     model = GaussianModel(prefix='peak_')
     params = model.make_params(amplitude=8, center=16, sigma=1)
```

### Comparing `lmfit-1.1.0/tests/test_multidatasets.py` & `lmfit-1.2.0/tests/test_multidatasets.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_nose.py` & `lmfit-1.2.0/tests/test_nose.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from scipy.optimize import rosen_der
 from uncertainties import ufloat
 
 from lmfit import Minimizer, Parameters, minimize
 from lmfit.lineshapes import gaussian
 from lmfit.minimizer import (HAS_EMCEE, SCALAR_METHODS, MinimizerResult,
                              _nan_policy)
+from lmfit.models import SineModel
 
 try:
     import numdifftools  # noqa: F401
     HAS_NUMDIFFTOOLS = True
 except ImportError:
     HAS_NUMDIFFTOOLS = False
 
@@ -313,14 +314,40 @@
     assert_allclose(y.std_dev, 0.2, rtol=1.e-7)
 
     y = x - x
     assert_allclose(y.nominal_value, 0.0, rtol=1.e-7)
     assert_allclose(y.std_dev, 0.0, rtol=1.e-7)
 
 
+def test_stderr_propagation():
+    """Test propagation of uncertainties to constraint expressions."""
+    model = SineModel()
+    params = model.make_params(amplitude=1, frequency=9.0, shift=0)
+    params.add("period", expr="1/frequency")
+    params.add("period_2a", expr="2*period")
+    params.add("period_2b", expr="2/frequency")
+    params.add("thing_1", expr="shift + frequency")
+    params.add("thing_2", expr="shift + 1/period")
+
+    np.random.seed(3)
+    xs = np.linspace(0, 1, 51)
+    ys = np.sin(7.45 * xs) + 0.01 * np.random.normal(size=xs.shape)
+
+    result = model.fit(ys, x=xs, params=params)
+
+    opars = result.params
+    assert_allclose(opars['period'].stderr, 1.1587e-04, rtol=1.e-3)
+    assert_allclose(opars['period_2b'].stderr, 2.3175e-04, rtol=1.e-3)
+    assert_allclose(opars['thing_1'].stderr, 0.0037291, rtol=1.e-3)
+
+    assert_allclose(opars['period_2a'].stderr, 2*opars['period'].stderr, rtol=1.e-5)
+    assert_allclose(opars['period_2b'].stderr, opars['period_2a'].stderr, rtol=1.e-5)
+    assert_allclose(opars['thing_1'].stderr, opars['thing_2'].stderr, rtol=1.e-5)
+
+
 class CommonMinimizerTest(unittest.TestCase):
 
     def setUp(self):
         """
         test scale minimizers except newton-cg (needs jacobian) and
         anneal (doesn't work out of the box).
         """
```

### Comparing `lmfit-1.1.0/tests/test_pandas.py` & `lmfit-1.2.0/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_parameter.py` & `lmfit-1.2.0/tests/test_parameter.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_parameters.py` & `lmfit-1.2.0/tests/test_parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """Tests for the Parameters class."""
 
-
 from copy import copy, deepcopy
+import os
 import pickle
 
 import numpy as np
 from numpy.testing import assert_allclose
 import pytest
 
 import lmfit
+from lmfit.models import VoigtModel
 
 
 @pytest.fixture
 def parameters():
     """Initialize a Parameters class for tests."""
     pars = lmfit.Parameters()
     pars.add(lmfit.Parameter(name='a', value=10.0, vary=True, min=-100.0,
                              max=100.0, expr=None, brute_step=5.0,
                              user_data=1))
     pars.add(lmfit.Parameter(name='b', value=0.0, vary=True, min=-250.0,
                              max=250.0, expr="2.0*a", brute_step=25.0,
-                             user_data=2.5))
+                             user_data={'test': 123}))
     exp_attr_values_A = ('a', 10.0, True, -100.0, 100.0, None, 5.0, 1)
-    exp_attr_values_B = ('b', 20.0, False, -250.0, 250.0, "2.0*a", 25.0, 2.5)
+    exp_attr_values_B = ('b', 20.0, False, -250.0, 250.0, "2.0*a", 25.0, {'test': 123})
     assert_parameter_attributes(pars['a'], exp_attr_values_A)
     assert_parameter_attributes(pars['b'], exp_attr_values_B)
     return pars, exp_attr_values_A, exp_attr_values_B
 
 
 def assert_parameter_attributes(par, expected):
     """Assert that parameter attributes have the expected values."""
@@ -54,15 +55,17 @@
     """Tests for copying a Parameters class; all use the __deepcopy__ method."""
     pars, exp_attr_values_A, exp_attr_values_B = parameters
 
     copy_pars = copy(pars)
     pars_copy = pars.copy()
     pars__copy__ = pars.__copy__()
 
+    # modifying the original parameters should not modify the copies
     pars['a'].set(value=100)
+    pars['b'].user_data['test'] = 456
 
     for copied in [copy_pars, pars_copy, pars__copy__]:
         assert isinstance(copied, lmfit.Parameters)
         assert copied != pars
         assert copied._asteval is not None
         assert copied._asteval.symtable is not None
         assert_parameter_attributes(copied['a'], exp_attr_values_A)
@@ -581,7 +584,53 @@
     assert 'x*3' in p1['y'].expr
     assert len(p1['y']._expr_eval.error) == 0
 
     with pytest.raises(SyntaxError):
         p1['y'].set(expr='t+')
     assert len(p1['y']._expr_eval.error) > 0
     assert_allclose(p1['y'].value, 34.0)
+
+
+def test_create_params():
+    """Tests for create_params() function."""
+    pars1 = lmfit.create_params(a=8, b=9,
+                                c=dict(value=3, min=0, max=10),
+                                d=dict(expr='a+b/c'),
+                                e=dict(value=10000, brute_step=4))
+
+    assert pars1['a'].value == 8
+    assert pars1['b'].value == 9
+    assert pars1['c'].value == 3
+    assert pars1['c'].min == 0
+    assert pars1['c'].max == 10
+    assert pars1['d'].expr == 'a+b/c'
+    assert pars1['d'].value == 11
+    assert pars1['e'].value == 10000
+    assert pars1['e'].brute_step == 4
+
+
+def test_unset_constrained_param():
+    """test 'unsetting' a constrained parameter by
+    just setting `param.vary = True`
+
+    """
+    data = np.loadtxt(os.path.join(os.path.dirname(__file__), '..',
+                                   'examples', 'test_peak.dat'))
+    x = data[:, 0]
+    y = data[:, 1]
+
+    # initial fit
+    mod = VoigtModel()
+    params = mod.guess(y, x=x)
+    out1 = mod.fit(y, params, x=x)
+
+    assert out1.nvarys == 3
+    assert out1.chisqr < 20.0
+
+    # now just gamma to vary
+    params['gamma'].vary = True
+    out2 = mod.fit(y, params, x=x)
+
+    assert out2.nvarys == 4
+    assert out2.chisqr < out1.chisqr
+    assert out2.rsquared > out1.rsquared
+    assert out2.params['gamma'].correl['sigma'] < -0.6
```

### Comparing `lmfit-1.1.0/tests/test_printfuncs.py` & `lmfit-1.2.0/tests/test_printfuncs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import pytest
 
 import lmfit
 from lmfit import (Minimizer, Parameters, ci_report, conf_interval, fit_report,
                    report_ci, report_fit)
 from lmfit.lineshapes import gaussian
 from lmfit.models import GaussianModel
-from lmfit.printfuncs import (alphanumeric_sort, fitreport_html_table,
-                              getfloat_attr, gformat)
+from lmfit.printfuncs import (alphanumeric_sort, correl_table,
+                              fitreport_html_table, getfloat_attr, gformat)
 
 np.random.seed(0)
 
 
 @pytest.fixture
 def params():
     """Return a lmfit.Parameters class with initial values."""
@@ -198,14 +198,30 @@
         return len(s)
 
     report_split = fitresult.fit_report(sort_pars=sort_length).split('\n')
     indx_vars = report_split.index('[[Variables]]')
     assert 'fwhm' in report_split[indx_vars+1]
 
 
+def test_correl_table(fitresult, capsys):
+    """Verify that ``correl_table`` is not empty."""
+    table_lines = correl_table(fitresult.params).split('\n')
+    nvarys = fitresult.nvarys
+
+    assert len(table_lines) == nvarys+4
+    assert len(table_lines[5]) > nvarys*10
+
+
+def test_fit_report_correl_table(fitresult, capsys):
+    """Verify that ``correl_table`` is not empty."""
+    out = fitresult.fit_report(correl_mode='table')
+    assert '[[Correlations]]' in out
+    assert '----+' in out
+
+
 def test_report_fit(fitresult, capsys):
     """Verify that the fit report is printed when using report_fit."""
     # report_fit with MinimizerResult/ModelResult as argument gives full
     # output of fitting results (except for [[Model]])
     report_fit(fitresult)
     report_headers = ['[[Fit Statistics]]', '[[Variables]]',
                       '[[Correlations]] (unreported correlations are < 0.100)']
@@ -302,19 +318,19 @@
     indices = [i for i, val in enumerate(report_split) if
                ('sigma:' in val or 'center:' in val or 'amplitude:' in val)]
     for indx in indices:
         assert 'model_value' in report_split[indx]
 
 
 def test_report_parvalue_non_numeric(fitresult):
-    """Verify that a non-numeric value is caught (can this ever happens?)."""
+    """Verify that a non-numeric value is handled gracefully."""
     fitresult.params['center'].value = None
     fitresult.params['center'].stderr = None
     report = fitresult.fit_report()
-    assert 'center:     Non Numeric Value?' in report
+    assert len(report) > 50
 
 
 def test_report_zero_value_spercent(fitresult):
     """Verify that ZeroDivisionError in spercent calc. gives empty string."""
     fitresult.params['center'].value = 0
     fitresult.params['center'].stderr = 0.1
     report_split = fitresult.fit_report().split('\n')
```

### Comparing `lmfit-1.1.0/tests/test_shgo.py` & `lmfit-1.2.0/tests/test_shgo.py`

 * *Files identical despite different names*

### Comparing `lmfit-1.1.0/tests/test_stepmodel.py` & `lmfit-1.2.0/tests/test_stepmodel.py`

 * *Files identical despite different names*

