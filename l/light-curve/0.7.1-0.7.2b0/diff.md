# Comparing `tmp/light_curve-0.7.1.tar.gz` & `tmp/light_curve-0.7.2b0.tar.gz`

## Comparing `light_curve-0.7.1.tar` & `light_curve-0.7.2b0.tar`

### file list

```diff
@@ -1,96 +1,97 @@
--rw-r--r--   0        0        0     1595 1970-01-01 00:00:00.000000 light_curve-0.7.1/Cargo.toml
--rw-r--r--   0     1001      122       91 2023-03-17 00:53:06.000000 light_curve-0.7.1/.gitignore
--rw-r--r--   0     1001      122    75073 2023-03-17 00:53:06.000000 light_curve-0.7.1/.readme/benchplot.png
--rw-r--r--   0     1001      122    21488 2023-03-17 00:53:06.000000 light_curve-0.7.1/README.md
--rw-r--r--   0     1001      122        7 2023-03-17 00:53:06.000000 light_curve-0.7.1/docs/.gitignore
--rw-r--r--   0     1001      122      634 2023-03-17 00:53:06.000000 light_curve-0.7.1/docs/Makefile
--rw-r--r--   0     1001      122     2028 2023-03-17 00:53:06.000000 light_curve-0.7.1/docs/conf.py
--rw-r--r--   0     1001      122      697 2023-03-17 00:53:06.000000 light_curve-0.7.1/docs/index.rst
--rw-r--r--   0     1001      122      795 2023-03-17 00:53:06.000000 light_curve-0.7.1/docs/make.bat
--rw-r--r--   0     1001      122       14 2023-03-17 00:53:06.000000 light_curve-0.7.1/docs/requirements.txt
--rw-r--r--   0     1001      122      271 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/__init__.py
--rw-r--r--   0     1001      122      288 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_ext.py
--rw-r--r--   0     1001      122     1011 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/__init__.py
--rw-r--r--   0     1001      122        0 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/__init__.py
--rw-r--r--   0     1001      122     2482 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/_base.py
--rw-r--r--   0     1001      122     1136 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/_base_meta.py
--rw-r--r--   0     1001      122      303 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/_lstsq.py
--rw-r--r--   0     1001      122      321 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/adnormal.py
--rw-r--r--   0     1001      122      232 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/amplitude.py
--rw-r--r--   0     1001      122      409 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/beyondnstd.py
--rw-r--r--   0     1001      122     1309 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/bins.py
--rw-r--r--   0     1001      122      365 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/cusum.py
--rw-r--r--   0     1001      122      329 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/eta.py
--rw-r--r--   0     1001      122      382 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/etae.py
--rw-r--r--   0     1001      122      365 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/excvar.py
--rw-r--r--   0     1001      122     1081 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/extractor.py
--rw-r--r--   0     1001      122     1998 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/flux_n_not_det_before_fd.py
--rw-r--r--   0     1001      122      414 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/intpercrange.py
--rw-r--r--   0     1001      122      476 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/kurtosis.py
--rw-r--r--   0     1001      122      618 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/linfit.py
--rw-r--r--   0     1001      122      455 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/lintrend.py
--rw-r--r--   0     1001      122     2099 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/magnitude_n_not_det_before_fd.py
--rw-r--r--   0     1001      122      531 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/magnpratio.py
--rw-r--r--   0     1001      122      371 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/maxslope.py
--rw-r--r--   0     1001      122      217 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/mean.py
--rw-r--r--   0     1001      122      253 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/meanvar.py
--rw-r--r--   0     1001      122      282 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/medabsdev.py
--rw-r--r--   0     1001      122      435 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/medbufrperc.py
--rw-r--r--   0     1001      122      223 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/median.py
--rw-r--r--   0     1001      122     2641 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/otsusplit.py
--rw-r--r--   0     1001      122      506 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/pdiffmperc.py
--rw-r--r--   0     1001      122      309 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/percampl.py
--rw-r--r--   0     1001      122      377 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/redchi2.py
--rw-r--r--   0     1001      122      236 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/skew.py
--rw-r--r--   0     1001      122      250 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/stdev.py
--rw-r--r--   0     1001      122      419 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/stetsonk.py
--rw-r--r--   0     1001      122      265 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/features/weightmean.py
--rw-r--r--   0     1001      122      596 2023-03-17 00:53:06.000000 light_curve-0.7.1/light_curve/light_curve_py/warnings.py
--rw-r--r--   0     1001      122     5158 2023-03-17 00:53:06.000000 light_curve-0.7.1/pyproject.toml
--rw-r--r--   0     1001      122     1395 2023-03-17 00:53:06.000000 light_curve-0.7.1/src/check.rs
--rw-r--r--   0     1001      122     2245 2023-03-17 00:53:06.000000 light_curve-0.7.1/src/cont_array.rs
--rw-r--r--   0     1001      122    51012 2023-03-17 00:53:06.000000 light_curve-0.7.1/src/dmdt.rs
--rw-r--r--   0     1001      122     1369 2023-03-17 00:53:06.000000 light_curve-0.7.1/src/errors.rs
--rw-r--r--   0     1001      122    51044 2023-03-17 00:53:06.000000 light_curve-0.7.1/src/features.rs
--rw-r--r--   0     1001      122     3513 2023-03-17 00:53:06.000000 light_curve-0.7.1/src/lib.rs
--rw-r--r--   0     1001      122     4269 2023-03-17 00:53:06.000000 light_curve-0.7.1/src/ln_prior.rs
--rw-r--r--   0     1001      122     3600 2023-03-17 00:53:06.000000 light_curve-0.7.1/src/np_array.rs
--rw-r--r--   0     1001      122        0 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/__init__.py
--rw-r--r--   0     1001      122        0 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_ext/__init__.py
--rw-r--r--   0     1001      122    12272 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_ext/test_dmdt.py
--rw-r--r--   0     1001      122     7990 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_ext/test_feature.py
--rw-r--r--   0     1001      122      786 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_ext/test_ln_prior.py
--rw-r--r--   0     1001      122        0 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/__init__.py
--rw-r--r--   0     1001      122      304 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_adnormal.py
--rw-r--r--   0     1001      122      289 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_amplitude.py
--rw-r--r--   0     1001      122      516 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_beyondnstd.py
--rw-r--r--   0     1001      122     2058 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_bins.py
--rw-r--r--   0     1001      122      964 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_call.py
--rw-r--r--   0     1001      122      302 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_cusum.py
--rw-r--r--   0     1001      122      311 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_eta.py
--rw-r--r--   0     1001      122      562 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_etae.py
--rw-r--r--   0     1001      122      359 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_excvar.py
--rw-r--r--   0     1001      122     1905 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_extractor.py
--rw-r--r--   0     1001      122      478 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_intpercrange.py
--rw-r--r--   0     1001      122      497 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_kurtosis.py
--rw-r--r--   0     1001      122      702 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_linfit.py
--rw-r--r--   0     1001      122      939 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_lintrend.py
--rw-r--r--   0     1001      122      608 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_magnpratio.py
--rw-r--r--   0     1001      122      297 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_maxslope.py
--rw-r--r--   0     1001      122      450 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_mean.py
--rw-r--r--   0     1001      122      326 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_meanvar.py
--rw-r--r--   0     1001      122      335 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_medabsdev.py
--rw-r--r--   0     1001      122      317 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_medbufrperc.py
--rw-r--r--   0     1001      122      509 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_median.py
--rw-r--r--   0     1001      122     1579 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_n_not_det_before_fd.py
--rw-r--r--   0     1001      122     1307 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_otsusplit.py
--rw-r--r--   0     1001      122      336 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_pdiffmperc.py
--rw-r--r--   0     1001      122      321 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_percampl.py
--rw-r--r--   0     1001      122      650 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_redchi2.py
--rw-r--r--   0     1001      122      302 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_skew.py
--rw-r--r--   0     1001      122      348 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_stdev.py
--rw-r--r--   0     1001      122      673 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_stetsonk.py
--rw-r--r--   0     1001      122      351 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/light_curve_py/test_weightmean.py
--rw-r--r--   0     1001      122    23632 2023-03-17 00:53:06.000000 light_curve-0.7.1/tests/test_w_bench.py
--rw-r--r--   0     1001      122    45045 2023-03-17 00:53:06.000000 light_curve-0.7.1/Cargo.lock
--rw-r--r--   0        0        0    22578 1970-01-01 00:00:00.000000 light_curve-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1682 1970-01-01 00:00:00.000000 light_curve-0.7.2b0/Cargo.toml
+-rw-r--r--   0     1001      122       91 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/.gitignore
+-rw-r--r--   0     1001      122    75073 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/.readme/benchplot.png
+-rw-r--r--   0     1001      122    21785 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/README.md
+-rw-r--r--   0     1001      122        7 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/docs/.gitignore
+-rw-r--r--   0     1001      122      634 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/docs/Makefile
+-rw-r--r--   0     1001      122     2028 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/docs/conf.py
+-rw-r--r--   0     1001      122      697 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/docs/index.rst
+-rw-r--r--   0     1001      122      795 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/docs/make.bat
+-rw-r--r--   0     1001      122       14 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/docs/requirements.txt
+-rw-r--r--   0     1001      122      271 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/__init__.py
+-rw-r--r--   0     1001      122      288 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_ext.py
+-rw-r--r--   0     1001      122     1011 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/__init__.py
+-rw-r--r--   0     1001      122        0 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/__init__.py
+-rw-r--r--   0     1001      122     2482 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/_base.py
+-rw-r--r--   0     1001      122     1136 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/_base_meta.py
+-rw-r--r--   0     1001      122      303 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/_lstsq.py
+-rw-r--r--   0     1001      122      321 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/adnormal.py
+-rw-r--r--   0     1001      122      232 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/amplitude.py
+-rw-r--r--   0     1001      122      409 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/beyondnstd.py
+-rw-r--r--   0     1001      122     1309 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/bins.py
+-rw-r--r--   0     1001      122      365 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/cusum.py
+-rw-r--r--   0     1001      122      329 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/eta.py
+-rw-r--r--   0     1001      122      382 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/etae.py
+-rw-r--r--   0     1001      122      365 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/excvar.py
+-rw-r--r--   0     1001      122     1081 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/extractor.py
+-rw-r--r--   0     1001      122     1998 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/flux_n_not_det_before_fd.py
+-rw-r--r--   0     1001      122      414 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/intpercrange.py
+-rw-r--r--   0     1001      122      476 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/kurtosis.py
+-rw-r--r--   0     1001      122      618 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/linfit.py
+-rw-r--r--   0     1001      122      455 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/lintrend.py
+-rw-r--r--   0     1001      122     2099 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/magnitude_n_not_det_before_fd.py
+-rw-r--r--   0     1001      122      531 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/magnpratio.py
+-rw-r--r--   0     1001      122      371 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/maxslope.py
+-rw-r--r--   0     1001      122      217 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/mean.py
+-rw-r--r--   0     1001      122      253 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/meanvar.py
+-rw-r--r--   0     1001      122      282 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/medabsdev.py
+-rw-r--r--   0     1001      122      435 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/medbufrperc.py
+-rw-r--r--   0     1001      122      223 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/median.py
+-rw-r--r--   0     1001      122     2641 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/otsusplit.py
+-rw-r--r--   0     1001      122      506 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/pdiffmperc.py
+-rw-r--r--   0     1001      122      309 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/percampl.py
+-rw-r--r--   0     1001      122      377 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/redchi2.py
+-rw-r--r--   0     1001      122      236 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/skew.py
+-rw-r--r--   0     1001      122      250 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/stdev.py
+-rw-r--r--   0     1001      122      419 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/stetsonk.py
+-rw-r--r--   0     1001      122      265 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/features/weightmean.py
+-rw-r--r--   0     1001      122      596 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/light_curve/light_curve_py/warnings.py
+-rw-r--r--   0     1001      122     6058 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/pyproject.toml
+-rw-r--r--   0     1001      122     1395 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/check.rs
+-rw-r--r--   0     1001      122     2245 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/cont_array.rs
+-rw-r--r--   0     1001      122    50948 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/dmdt.rs
+-rw-r--r--   0     1001      122     1504 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/errors.rs
+-rw-r--r--   0     1001      122    63506 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/features.rs
+-rw-r--r--   0     1001      122     3528 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/lib.rs
+-rw-r--r--   0     1001      122     4269 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/ln_prior.rs
+-rw-r--r--   0     1001      122     3600 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/np_array.rs
+-rw-r--r--   0     1001      122     4450 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/src/transform.rs
+-rw-r--r--   0     1001      122        0 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/__init__.py
+-rw-r--r--   0     1001      122        0 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_ext/__init__.py
+-rw-r--r--   0     1001      122    12272 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_ext/test_dmdt.py
+-rw-r--r--   0     1001      122     9675 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_ext/test_feature.py
+-rw-r--r--   0     1001      122      786 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_ext/test_ln_prior.py
+-rw-r--r--   0     1001      122        0 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/__init__.py
+-rw-r--r--   0     1001      122      304 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_adnormal.py
+-rw-r--r--   0     1001      122      289 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_amplitude.py
+-rw-r--r--   0     1001      122      516 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_beyondnstd.py
+-rw-r--r--   0     1001      122     2058 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_bins.py
+-rw-r--r--   0     1001      122      964 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_call.py
+-rw-r--r--   0     1001      122      302 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_cusum.py
+-rw-r--r--   0     1001      122      311 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_eta.py
+-rw-r--r--   0     1001      122      562 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_etae.py
+-rw-r--r--   0     1001      122      359 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_excvar.py
+-rw-r--r--   0     1001      122     1905 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_extractor.py
+-rw-r--r--   0     1001      122      478 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_intpercrange.py
+-rw-r--r--   0     1001      122      497 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_kurtosis.py
+-rw-r--r--   0     1001      122      702 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_linfit.py
+-rw-r--r--   0     1001      122      939 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_lintrend.py
+-rw-r--r--   0     1001      122      608 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_magnpratio.py
+-rw-r--r--   0     1001      122      297 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_maxslope.py
+-rw-r--r--   0     1001      122      450 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_mean.py
+-rw-r--r--   0     1001      122      326 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_meanvar.py
+-rw-r--r--   0     1001      122      335 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_medabsdev.py
+-rw-r--r--   0     1001      122      317 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_medbufrperc.py
+-rw-r--r--   0     1001      122      509 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_median.py
+-rw-r--r--   0     1001      122     1579 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_n_not_det_before_fd.py
+-rw-r--r--   0     1001      122     1307 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_otsusplit.py
+-rw-r--r--   0     1001      122      336 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_pdiffmperc.py
+-rw-r--r--   0     1001      122      321 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_percampl.py
+-rw-r--r--   0     1001      122      650 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_redchi2.py
+-rw-r--r--   0     1001      122      302 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_skew.py
+-rw-r--r--   0     1001      122      348 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_stdev.py
+-rw-r--r--   0     1001      122      673 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_stetsonk.py
+-rw-r--r--   0     1001      122      351 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/light_curve_py/test_weightmean.py
+-rw-r--r--   0     1001      122    23632 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/tests/test_w_bench.py
+-rw-r--r--   0     1001      122    48850 2023-04-07 20:58:17.000000 light_curve-0.7.2b0/Cargo.lock
+-rw-r--r--   0        0        0    23378 1970-01-01 00:00:00.000000 light_curve-0.7.2b0/PKG-INFO
```

### Comparing `light_curve-0.7.1/Cargo.toml` & `light_curve-0.7.2b0/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [package]
 name = "light-curve-python"
-version = "0.7.1"
+version = "0.7.2-beta.0"
 authors = ["Konstantin Malanchev <hombit@gmail.com>", "Anastasia Lavrukhina <lavrukhina.ad@gmail.com>"]
 description = "Feature extractor from noisy time series"
 readme = "README.md"
 repository = "https://github.com/light-curve/light-curve-python"
 license = "GPL-3.0-or-later"
 edition = "2021"
-rust-version = "1.60"
+rust-version = "1.62"
 
 [lib]
 name = "light_curve"
 crate-type = ["cdylib"]
 
 [profile.release]
 lto = true
@@ -28,30 +28,31 @@
 
 [dependencies]
 # it is a dependency of intel-mkl-tool, we pin it to temporary solve
 # https://github.com/rust-math/intel-mkl-src/issues/68
 anyhow = "<1.0.49"
 const_format = "0.2.30"
 conv = "0.3.3"
+enum-iterator = "1.1.0,<1.2.0" # 1.2.0 requires MSRV 1.63
 enumflags2 = { version = "0.7.5", features = ["serde"] }
 itertools = "0.10.5"
 macro_const = "0.1.0"
 ndarray = { version = "0.15.3", features = ["rayon"] }
 numpy = "0.18.0"
 num_cpus = "1.13.0"
 num-traits = "0.2"
-pyo3 = {version = "0.18.1", features = ["extension-module"]}
+pyo3 = {version = "0.18.2", features = ["extension-module", "multiple-pymethods"]}
 rand = "0.8.5"
 rand_xoshiro = "0.6.0"
 thiserror = "1.0.37"
 serde = { version = "1", features = ["derive"] }
 serde-pickle = "1"
 rayon = "1.6.1"
 unzip3 = "1.0.0"
 
 [dependencies.light-curve-dmdt]
 version = "0.7.1"
 features = ["serde"]
 
 [dependencies.light-curve-feature]
-version = "0.5.4"
+version = "0.5.5"
 default_features = false
```

### Comparing `light_curve-0.7.1/.readme/benchplot.png` & `light_curve-0.7.2b0/.readme/benchplot.png`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/README.md` & `light_curve-0.7.2b0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 We also provide `light-curve-python` package which is just an "alias" to the main `light-curve` package.
 
 Minimum supported Python version is 3.7.
 We provide binary wheels via [PyPi](https://pypi.org/project/light-curve/) for number of platforms and architectures, both for CPython and PyPy.
 
 ### Support matrix
 
-| Arch \ OS   | Linux glibc | Linux musl                     | macOS                                                          | Windows                                                                |
-| ----------- |-------------|--------------------------------|----------------------------------------------------------------|------------------------------------------------------------------------|
-| **x86-64**  | wheel (MKL) | wheel (MKL)                    | wheel                                                          | not tested https://github.com/light-curve/light-curve-python/issues/12 |
-| **i686**    | src         | src                            | —                                                              | not tested                                                             |
-| **aarch64** | wheel       | wheel                          | src https://github.com/light-curve/light-curve-python/issues/5 | not tested                                                             |
-| **ppc64le** | wheel       | not tested (no Rust toolchain) | —                                                              | —                                                                      |
+| Arch \ OS   | Linux glibc | Linux musl                     | macOS                                                          | Windows https://github.com/light-curve/light-curve-python/issues/186 |
+| ----------- |-------------|--------------------------------|----------------------------------------------------------------|----------------------------------------------------------------------|
+| **x86-64**  | wheel (MKL) | wheel (MKL)                    | wheel                                                          | wheel (no Ceres, no GSL)                                             |
+| **i686**    | src         | src                            | —                                                              | not tested                                                           |
+| **aarch64** | wheel       | wheel                          | src https://github.com/light-curve/light-curve-python/issues/5 | not tested                                                           |
+| **ppc64le** | wheel       | not tested (no Rust toolchain) | —                                                              | —                                                                    |
 
-- "wheel": binary wheel is available on pypi.org, local building is not required for the platform, the only pre-requirement is a recent `pip` version. For Linux x86-64 we provide binary wheels built with Intel MKL for better periodogram perfromance, which is not a default build option.
+- "wheel": binary wheel is available on pypi.org, local building is not required for the platform, the only pre-requirement is a recent `pip` version. For Linux x86-64 we provide binary wheels built with Intel MKL for better periodogram performance, which is not a default build option. For Windows x86-64 we provide wheel with no Ceres and no GSL support, which is not a default build option.
 - "src": the package is confirmed to be built and pass unit tests locally, but testing and package building is not supported by CI. It is required to have the [GNU scientific library (GSL)](https://www.gnu.org/software/gsl/) v2.1+ and the [Rust toolchain](https://rust-lang.org) v1.57+ to install it via `pip install`.
 - "not tested": building from the source code is not tested, please report us building status via issue/PR/email.
 
 We build aarch64 macOS 12.0+ Python 3.8+ wheels locally and submit them running this command in `light-curve` directory:
 ```
 rm -rf ./wheelhouse
 CIBW_BUILD='cp3*-macosx_arm64' CIBW_ENVIRONMENT="MACOSX_DEPLOYMENT_TARGET=12.0 MATURIN_PEP517_ARGS='--locked --no-default-features --features ceres-source,fftw-source,gsl'" CIBW_BEFORE_ALL='curl https://sh.rustup.rs -sSf | sh -s -- --default-toolchain stable -y; brew install gsl' python3 -mcibuildwheel --platform macos
@@ -38,14 +38,15 @@
 ```
 
 ## Feature evaluators
 
 Most of the classes implement various feature evaluators useful for light-curve based
 astrophysical source classification and characterisation.
 
+<!-- name: test_feature_evaluators_basic -->
 ```python
 import light_curve as lc
 import numpy as np
 
 # Time values can be non-evenly separated but must be an ascending array
 n = 101
 t = np.linspace(0.0, 1.0, n)
@@ -79,21 +80,23 @@
 
 If you confident in your inputs you could use `sorted = True` (`t` is in ascending order)
 and `check = False` (no NaNs in inputs, no infs in `t` or `m`) for better performance.
 Note that if your inputs are not valid and are not validated by
 `sorted=None` and `check=True` (default values) then all kind of bad things could happen.
 
 Print feature classes list
+<!-- name: test_feature_evaluators_list -->
 ```python
 import light_curve as lc
 
 print([x for x in dir(lc) if hasattr(getattr(lc, x), "names")])
 ```
 
 Read feature docs
+<!-- name: test_feature_evaluators_help -->
 ```python
 import light_curve as lc
 
 help(lc.BazinFit)
 ```
 
 ### Experimental extractors
@@ -101,14 +104,15 @@
 From the technical point of view the package consists of two parts: a wrapper for [`light-curve-feature` Rust crate](https://crates.io/crates/light-curve-feature) (`light_curve_ext` sub-package) and pure Python sub-package `light_curve_py`.
 We use the Python implementation of feature extractors to test Rust implementation and to implement new experimental extractors.
 Please note, that the Python implementation is much slower for the most of the extractors and doesn't provide the same functionality as the Rust implementation.
 However, the Python implementation provides some new feature extractors you can find useful.
 
 You can manually use extractors from both implementations:
 
+<!-- name: test_experimental_extractors -->
 ```python
 import numpy as np
 from numpy.testing import assert_allclose
 from light_curve.light_curve_ext import LinearTrend as RustLinearTrend
 from light_curve.light_curve_py import LinearTrend as PythonLinearTrend
 
 rust_fe = RustLinearTrend()
@@ -413,14 +417,15 @@
 
 See benchmarks' descriptions in more details in ["Performant feature extraction for photometric time series"](https://arxiv.org/abs/2302.10837).
 
 ## dm-dt map
 
 Class `DmDt` provides dm–dt mapper (based on [Mahabal et al. 2011](https://ui.adsabs.harvard.edu/abs/2011BASI...39..387M/abstract), [Soraisam et al. 2020](https://ui.adsabs.harvard.edu/abs/2020ApJ...892..112S/abstract)). It is a Python wrapper for [`light-curve-dmdt` Rust crate](https://crates.io/crates/light-curve-dmdt).
 
+<!-- name: test_dmdt -->
 ```python
 import numpy as np
 from light_curve import DmDt
 from numpy.testing import assert_array_equal
 
 dmdt = DmDt.from_borders(min_lgdt=0, max_lgdt=np.log10(3), max_abs_dm=3, lgdt_size=2, dm_size=4, norm=[])
```

### Comparing `light_curve-0.7.1/docs/Makefile` & `light_curve-0.7.2b0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/docs/conf.py` & `light_curve-0.7.2b0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/docs/index.rst` & `light_curve-0.7.2b0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/docs/make.bat` & `light_curve-0.7.2b0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/light_curve/light_curve_py/__init__.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/__init__.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/light_curve/light_curve_py/features/_base.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/_base.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/light_curve/light_curve_py/features/_base_meta.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/_base_meta.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/light_curve/light_curve_py/features/bins.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/bins.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/light_curve/light_curve_py/features/extractor.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/extractor.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/light_curve/light_curve_py/features/flux_n_not_det_before_fd.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/flux_n_not_det_before_fd.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/light_curve/light_curve_py/features/linfit.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/linfit.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/light_curve/light_curve_py/features/magnitude_n_not_det_before_fd.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/magnitude_n_not_det_before_fd.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/light_curve/light_curve_py/features/magnpratio.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/magnpratio.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/light_curve/light_curve_py/features/otsusplit.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/features/otsusplit.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/light_curve/light_curve_py/warnings.py` & `light_curve-0.7.2b0/light_curve/light_curve_py/warnings.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/pyproject.toml` & `light_curve-0.7.2b0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,31 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Rust",
     "Topic :: Scientific/Engineering :: Astronomy",
 ]
 
+[project.optional-dependencies]
+test = [
+    "feets",
+    "joblib",
+    "numpy",
+    "pandas",
+    "pytest",
+    "pytest-benchmark",
+    "markdown-pytest",
+    "pytest-subtests",
+]
+dev = [
+    "light-curve[test]",
+    "black",
+    "ruff",
+]
+
 [tool.setuptools]
 # We load these from Cargo.toml
 dynamic = [
     "authors",
     "description",
     "license",
     "readme",
@@ -79,35 +96,25 @@
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 # requires pytest-benchmark
 addopts = "-ra --import-mode=append --benchmark-min-time=0.1 --benchmark-max-time=5.0 --benchmark-sort=mean --benchmark-disable"
 testpaths = [
     "tests/",
-    "README.md", # requires pytest-markdown
+    "README.md", # requires markdown-pytest
 ]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py37,py38,py39,py310,py311
 isolated_build = True
 
 [testenv]
-deps =
-    feets
-    joblib
-    numpy
-    pandas
-    pytest
-    pytest-benchmark
-    pytest-markdown
-    pytest-subtests
-    ruff
-    scipy
+extras = dev
 commands =
     pytest README.md tests/ light_curve/
     ruff .
 """
 
 
 # Test
@@ -116,15 +123,15 @@
 # For testing we use only platforms for which scipy binary wheels are available
 [[tool.cibuildwheel.overrides]]
 select = "cp*-manylinux_x86_64 cp*-manylinux_aarch64 cp*-macosx*"
 test-command = "pytest {package}/README.md {package}/light_curve/ {package}/tests/ --ignore {package}/tests/test_w_bench.py"
 test-requires = [
     "pytest",
     "pytest-benchmark",
-    "pytest-markdown",
+    "markdown-pytest",
     "pytest-subtests",
     "numpy",
     "scipy",
 ]
 
 [tool.cibuildwheel]
 # We use our own images which include Rust, GSL and platform-optimised FFTW
@@ -159,12 +166,24 @@
 before-all = [
     # Install Rust
     "curl https://sh.rustup.rs -sSf | sh -s -- --default-toolchain stable -y",
     # Install FFTW and GSL
     "brew install ceres-solver fftw gsl",
 ]
 
+# We miss Rust installation here because it is not so simple on Windows
+[tool.cibuildwheel.windows]
+# fftw-src downloads FFTW DLLs, so fftw-sys doesn't link FFTW statically. We need to repair the wheel with these DLLs.
+before-all = [
+    "curl -o %USERPROFILE%\\Downloads\\fftw-dll64.zip https://fftw.org/pub/fftw/fftw-3.3.5-dll64.zip",
+    "powershell -command \"Expand-Archive -Path %USERPROFILE%\\Downloads\\fftw-dll64.zip -DestinationPath %USERPROFILE%\\Downloads\\fftw-dll64\"",
+]
+before-build = ["pip install delvewheel"]
+repair-wheel-command = "delvewheel repair --add-path=%USERPROFILE%\\Downloads\\fftw-dll64 -w {dest_dir} {wheel}"
+# We do not support Ceres and GSL on Windows
+environment = { "MATURIN_PEP517_ARGS" = "--locked --no-default-features --features fftw-source" }
+
 # Build with Intel MKL on Linux x86_64
 [[tool.cibuildwheel.overrides]]
 select = "*linux_x86_64"
 # We use system Ceres because it is available as a static library in our build environment
 environment = { "PATH" = "$PATH:$HOME/.cargo/bin", "MATURIN_PEP517_ARGS" = "--locked --no-default-features --features ceres-system,fftw-mkl,gsl" }
```

### Comparing `light_curve-0.7.1/src/check.rs` & `light_curve-0.7.2b0/src/check.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/src/cont_array.rs` & `light_curve-0.7.2b0/src/cont_array.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/src/dmdt.rs` & `light_curve-0.7.2b0/src/dmdt.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#![allow(clippy::borrow_deref_ref)] // https://github.com/rust-lang/rust-clippy/issues/8971
-#![allow(clippy::redundant_closure)] // false positive for pyo3(signature(arg=vec![]))
-
 use crate::check::check_sorted;
 use crate::cont_array::{ContArray, ContCowArray};
 use crate::errors::{Exception, Res};
 use crate::np_array::Arr;
 
 use conv::{ApproxFrom, ApproxInto, ConvAsUtil};
 use enumflags2::{bitflags, BitFlags};
@@ -809,14 +806,17 @@
 ///     Number of observations in each dt for a list of arrays
 /// points_batches(lcs, sorted=None, batch_size=1, yield_index=False, shuffle=False, drop_nobs=0, random_seed=None)
 ///     Gives a reusable iterable which yields dmdt-maps
 /// gausses_batches(lcs, sorted=None, batch_size=1, yield_index=False, shuffle=False, drop_nobs=0, random_seed=None)
 ///     Gives a reusable iterable which yields smeared dmdt-maps
 ///
 #[pyclass(module = "light_curve.light_curve_ext")]
+#[pyo3(
+    text_signature = "(dt, dm, *, dt_type='auto', dm_type='auto', norm=[], n_jobs=-1, approx_erf=False)"
+)]
 #[derive(Serialize, Deserialize, Clone)]
 pub struct DmDt {
     dmdt_f64: GenericDmDt<f64>,
     dmdt_f32: GenericDmDt<f32>,
 }
 
 impl DmDt {
@@ -969,25 +969,25 @@
 impl DmDt {
     #[allow(clippy::too_many_arguments)]
     #[new]
     #[pyo3(signature = (
         dt,
         dm,
         *,
-        dm_type = "auto",
         dt_type = "auto",
+        dm_type = "auto",
         norm=vec![],
         n_jobs = -1,
         approx_erf = false
     ))]
     fn __new__<'a>(
         dt: Arr<'a, f64>,
         dm: Arr<'a, f64>,
-        dm_type: &str,
         dt_type: &str,
+        dm_type: &str,
         norm: Vec<&str>,
         n_jobs: i64,
         approx_erf: bool,
     ) -> Res<Self> {
         let (dt_grid_f32, dt_grid_f64) = Self::grids(dt.as_array(), dt_type)?;
         let (dm_grid_f32, dm_grid_f64) = Self::grids(dm.as_array(), dm_type)?;
```

### Comparing `light_curve-0.7.1/src/errors.rs` & `light_curve-0.7.2b0/src/errors.rs`

 * *Files 9% similar despite different names*

```diff
@@ -7,38 +7,42 @@
 use std::result::Result;
 use thiserror::Error;
 
 import_exception!(pickle, PicklingError);
 import_exception!(pickle, UnpicklingError);
 
 #[allow(clippy::enum_variant_names)]
-#[derive(Clone, Error, Debug)]
+#[derive(Error, Debug)]
 #[error("{0}")]
 pub(crate) enum Exception {
     // builtins
     IndexError(String),
     NotImplementedError(String),
     RuntimeError(String),
     TypeError(String),
     ValueError(String),
     // pickle
     PicklingError(String),
     UnpicklingError(String),
+    // some exception from pyo3 which we need to handle
+    PyO3(#[from] PyErr),
 }
 
 impl From<Exception> for PyErr {
     fn from(err: Exception) -> PyErr {
         match err {
             // builtins
             Exception::IndexError(err) => PyIndexError::new_err(err),
             Exception::NotImplementedError(err) => PyNotImplementedError::new_err(err),
             Exception::RuntimeError(err) => PyRuntimeError::new_err(err),
             Exception::TypeError(err) => PyTypeError::new_err(err),
             Exception::ValueError(err) => PyValueError::new_err(err),
             // pickle
             Exception::PicklingError(err) => PicklingError::new_err(err),
             Exception::UnpicklingError(err) => UnpicklingError::new_err(err),
+            // pyo3
+            Exception::PyO3(err) => err,
         }
     }
 }
 
 pub(crate) type Res<T> = Result<T, Exception>;
```

### Comparing `light_curve-0.7.1/src/lib.rs` & `light_curve-0.7.2b0/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 mod np_array;
 mod check;
 mod cont_array;
 mod dmdt;
 mod errors;
 mod features;
 mod ln_prior;
+mod transform;
 
 /// High-performance time-series feature extractor
 ///
 /// The module provides a collection of features to be extracted from unevenly separated
 /// time-series. This module if based on Rust crates `light-curve-feature` & `light-curve-dmdt`.
 ///
 /// dm-lg(dt) maps generator is represented by `DmDt` class, while all other classes are
```

### Comparing `light_curve-0.7.1/src/ln_prior.rs` & `light_curve-0.7.2b0/src/ln_prior.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/src/np_array.rs` & `light_curve-0.7.2b0/src/np_array.rs`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/light_curve_ext/test_dmdt.py` & `light_curve-0.7.2b0/tests/light_curve_ext/test_dmdt.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/light_curve_ext/test_feature.py` & `light_curve-0.7.2b0/tests/light_curve_ext/test_feature.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,51 +5,66 @@
 import numpy as np
 import pytest
 from numpy.testing import assert_allclose, assert_array_equal
 
 import light_curve.light_curve_ext as lc
 
 
-def _feature_classes(module, exclude_parametric=True):
-    for name, obj in inspect.getmembers(module):
+def _feature_classes(module, *, exclude_parametric=True):
+    for name, member in inspect.getmembers(module):
         if name.startswith("_"):
             continue
-        if inspect.ismodule(obj):
-            yield from _feature_classes(obj)
-        if not inspect.isclass(obj):
+        if inspect.ismodule(member):
+            yield from _feature_classes(member)
+        if not inspect.isclass(member):
             continue
-        if not issubclass(obj, lc._FeatureEvaluator):
+        if not issubclass(member, lc._FeatureEvaluator):
             continue
         # Skip classes with non-trivial constructors
         if exclude_parametric:
             try:
-                obj()
+                member()
             except TypeError:
                 continue
-        yield obj
+        yield member
 
 
-non_param_feature_classes = frozenset(_feature_classes(lc, True))
-all_feature_classes = frozenset(_feature_classes(lc, False))
+non_param_feature_classes = frozenset(_feature_classes(lc, exclude_parametric=True))
+assert len(non_param_feature_classes) > 0
+
+all_feature_classes = frozenset(_feature_classes(lc, exclude_parametric=False))
+assert len(all_feature_classes) > 0
+
+
+def get_new_args_kwargs(cls):
+    if hasattr(cls, "__getnewargs_ex__"):
+        return cls.__getnewargs_ex__()
+    if hasattr(cls, "__getnewargs__"):
+        args = cls.__getnewargs__()
+        return args, {}
+    return (), {}
+
+
+def new_default(cls, **kwargs):
+    args, kwargs_ = get_new_args_kwargs(cls)
+    kwargs = dict(kwargs_, **kwargs)
+    return cls(*args, **kwargs)
 
 
 def construct_example_objects(cls, *, parametric_variants=1, rng=None):
     # Extractor is special
     if cls is lc.Extractor:
         return [cls(lc.BeyondNStd(1.5), lc.LinearFit())]
 
     # No mandatory arguments
     if not hasattr(cls, "__getnewargs__"):
         return [cls()]
 
     # default mandatory arguments
-    if hasattr(cls, "__getnewargs_ex__"):
-        args, kwargs = cls.__getnewargs_ex__()
-    else:
-        args, kwargs = cls.__getnewargs__(), {}
+    args, kwargs = get_new_args_kwargs(cls)
 
     # Add Mean feature for metafeatures
     args = [[lc.Mean()] if arg == () else arg for arg in args]
 
     objects = [cls(*args, **kwargs)]
     # Nothing to mutate
     if not any(isinstance(arg, float) for arg in args + list(kwargs.values())):
@@ -86,14 +101,47 @@
     t = np.sort(rng.normal(0, 1, n))
     m = t.copy()
     sigma = np.full_like(t, 0.1)
 
     return t, m, sigma
 
 
+@pytest.mark.parametrize("cls", list(all_feature_classes))
+def test_available_transforms(cls):
+    # All available features should consume transform=None
+    none = new_default(cls, transform=None)
+
+    # If transform consumes False it
+    # 1) should give the same feature as transform=None
+    # 2) should be able to consume transform=True
+    try:
+        false = new_default(cls, transform=False)
+    except NotImplementedError:
+        return
+    # It would be better to compare objects themselves, but __eq__ is not implemented yet
+    # https://github.com/light-curve/light-curve-python/issues/148
+    assert false.names == none.names
+    true = new_default(cls, transform=True)
+    # Check if transform=True is not the same as transform=False
+    default_transform = getattr(cls, "default_transform", None)
+    if default_transform != "identity":
+        assert true.names != false.names
+
+    # Both attributes should be present or absent
+    assert hasattr(cls, "supported_transforms") == hasattr(cls, "default_transform")
+
+    if not hasattr(cls, "supported_transforms"):
+        return
+
+    assert cls.default_transform in cls.supported_transforms
+
+    for transform in cls.supported_transforms + ["default"]:
+        new_default(cls, transform=transform)
+
+
 @pytest.mark.parametrize("feature", gen_feature_evaluators(parametric_variants=2))
 def test_negative_strides(feature):
     t = np.linspace(1, 0, 20)[::-2]
     m = np.exp(t)[:]
     err = np.random.uniform(0.1, 0.2, t.shape)
     feature(t, m, err)
```

### Comparing `light_curve-0.7.1/tests/light_curve_ext/test_ln_prior.py` & `light_curve-0.7.2b0/tests/light_curve_ext/test_ln_prior.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/light_curve_py/test_beyondnstd.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_beyondnstd.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/light_curve_py/test_bins.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_bins.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/light_curve_py/test_call.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_call.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/light_curve_py/test_etae.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_etae.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/light_curve_py/test_extractor.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_extractor.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/light_curve_py/test_linfit.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_linfit.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/light_curve_py/test_lintrend.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_lintrend.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/light_curve_py/test_magnpratio.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_magnpratio.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/light_curve_py/test_n_not_det_before_fd.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_n_not_det_before_fd.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/light_curve_py/test_otsusplit.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_otsusplit.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/light_curve_py/test_redchi2.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_redchi2.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/light_curve_py/test_stetsonk.py` & `light_curve-0.7.2b0/tests/light_curve_py/test_stetsonk.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/tests/test_w_bench.py` & `light_curve-0.7.2b0/tests/test_w_bench.py`

 * *Files identical despite different names*

### Comparing `light_curve-0.7.1/Cargo.lock` & `light_curve-0.7.2b0/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -167,17 +167,17 @@
 dependencies = [
  "num",
  "time",
 ]
 
 [[package]]
 name = "cmake"
-version = "0.1.49"
+version = "0.1.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db34956e100b30725f2eb215f90d4871051239535632f84fea3bc92722c66b7c"
+checksum = "a31c789563b815f77f4250caee12365734369f942439b7defd71e18a48197130"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "codespan-reporting"
 version = "0.11.1"
@@ -272,14 +272,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
 dependencies = [
  "cfg-if 1.0.0",
 ]
 
 [[package]]
+name = "ctor"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dd4056f63fce3b82d852c3da92b08ea59959890813a7f4ce9c0ff85b10cf301b"
+dependencies = [
+ "quote",
+ "syn 2.0.13",
+]
+
+[[package]]
 name = "curl"
 version = "0.4.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "509bd11746c7ac09ebd19f0b17782eae80aadee26237658a6b4808afb5c11a22"
 dependencies = [
  "curl-sys",
  "libc",
@@ -288,17 +298,17 @@
  "schannel",
  "socket2",
  "winapi 0.3.9",
 ]
 
 [[package]]
 name = "curl-sys"
-version = "0.4.60+curl-7.88.1"
+version = "0.4.61+curl-8.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "717abe2cb465a5da6ce06617388a3980c9a2844196734bec8ccb8e575250f13f"
+checksum = "14d05c10f541ae6f3bc5b3d923c20001f47db7d5f0b2bc6ad16490133842db79"
 dependencies = [
  "cc",
  "libc",
  "libz-sys",
  "openssl-sys",
  "pkg-config",
  "vcpkg",
@@ -331,15 +341,15 @@
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
 version = "1.0.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61b50bc93ba22c27b0d31128d2d130a0a6b3d267ae27ef7e4fae2167dfe8781c"
@@ -348,28 +358,28 @@
 name = "cxxbridge-macro"
 version = "1.0.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "39e61fda7e62115119469c7b3591fd913ecca96fb766cfd3f2e2502ab7bc87a5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "derive_more"
 version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
 dependencies = [
  "convert_case",
  "proc-macro2",
  "quote",
  "rustc_version",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "dirs"
 version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "13aea89a5c93364a98e9b37b2fa237effbb694d5cfe01c5b70941f7eb087d5e3"
@@ -408,44 +418,64 @@
 checksum = "d903b65b48e77869a8ca98db3f4cbe0756892d69dafdcc6255580dfa6b5745f9"
 dependencies = [
  "error-chain",
  "rand 0.3.23",
 ]
 
 [[package]]
+name = "enum-iterator"
+version = "1.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "45a0ac4aeb3a18f92eaf09c6bb9b3ac30ff61ca95514fc58cbead1c9a6bf5401"
+dependencies = [
+ "enum-iterator-derive",
+]
+
+[[package]]
+name = "enum-iterator-derive"
+version = "1.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "355f93763ef7b0ae1c43c4d8eccc9d5848d84ad1a1d8ce61c421d1ac85a19d05"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "enum_dispatch"
 version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "11f36e95862220b211a6e2aa5eca09b4fa391b13cd52ceb8035a24bf65a79de2"
 dependencies = [
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "enumflags2"
-version = "0.7.5"
+version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e75d4cd21b95383444831539909fbb14b9dc3fdceb2a6f5d36577329a1f55ccb"
+checksum = "0044ebdf7fbb2a772e0c0233a9d3173c5cd8af8ae7078d4c5188af44ffffaa4b"
 dependencies = [
  "enumflags2_derive",
  "serde",
 ]
 
 [[package]]
 name = "enumflags2_derive"
-version = "0.7.4"
+version = "0.7.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f58dc3c5e468259f19f2d46304a6b28f1c3d034442e14b322d2b850e36f6d5ae"
+checksum = "9d2c772ccdbdfd1967b4f5d79d17c98ebf92009fdcc838db7aa434462f600c26"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "error-chain"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9435d864e017c3c6afeac1654189b06cdb491cf2ff73dbf0d73b0f292f42ff8"
@@ -491,22 +521,22 @@
  "intel-mkl-src",
  "libc",
  "num-complex 0.3.1",
 ]
 
 [[package]]
 name = "filetime"
-version = "0.2.20"
+version = "0.2.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a3de6e8d11b22ff9edc6d916f890800597d60f8b2da1caf2955c274638d6412"
+checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
 dependencies = [
  "cfg-if 1.0.0",
  "libc",
  "redox_syscall",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "flate2"
 version = "1.0.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
@@ -536,24 +566,35 @@
 name = "fuchsia-cprng"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a06f77d526c1a601b7c4cdd98f54b5eaabffc14d5f2f0296febdc7f357c6d3ba"
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if 1.0.0",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
+name = "ghost"
+version = "0.1.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e77ac7b51b8e6313251737fcef4b1c01a2ea102bde68415b62c0ee9268fec357"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.13",
+]
+
+[[package]]
 name = "gimli"
 version = "0.27.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad0a93d233ebf96623465aad4046a8d3aa4da22d4f4beba5388838c8a434bbb4"
 
 [[package]]
 name = "glob"
@@ -574,17 +615,17 @@
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
@@ -615,14 +656,24 @@
  "glob",
  "pkg-config",
  "tar",
  "zstd",
 ]
 
 [[package]]
+name = "inventory"
+version = "0.3.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7741301a6d6a9b28ce77c0fb77a4eb116b6bc8f3bef09923f7743d059c4157d3"
+dependencies = [
+ "ctor",
+ "ghost",
+]
+
+[[package]]
 name = "iter-read"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c397ca3ea05ad509c4ec451fea28b4771236a376ca1c69fd5143aae0cf8f93c4"
 
 [[package]]
 name = "itertools"
@@ -677,17 +728,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.141"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
 
 [[package]]
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
@@ -717,17 +768,17 @@
  "num-traits",
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "light-curve-feature"
-version = "0.5.4"
+version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6786d3521e14b51f96a53cc41d28e62c098e545121362f076db6f878d1514a4a"
+checksum = "5cb1fb325fd280c3866c1431320bf7a215dfb23c6691cc13127f99593c150633"
 dependencies = [
  "GSL",
  "anyhow",
  "ceres-solver",
  "conv",
  "emcee",
  "enum_dispatch",
@@ -736,29 +787,31 @@
  "lazy_static 1.4.0",
  "libm",
  "macro_const",
  "ndarray 0.15.6",
  "ndarray-stats",
  "num-complex 0.3.1",
  "num-traits",
+ "paste",
  "rand 0.3.23",
  "schemars",
  "serde",
  "thiserror",
  "thread_local 1.1.4",
  "unzip3",
 ]
 
 [[package]]
 name = "light-curve-python"
-version = "0.7.1"
+version = "0.7.2-beta.0"
 dependencies = [
  "anyhow",
  "const_format",
  "conv",
+ "enum-iterator",
  "enumflags2",
  "itertools 0.10.5",
  "light-curve-dmdt",
  "light-curve-feature",
  "macro_const",
  "ndarray 0.15.6",
  "num-traits",
@@ -1016,19 +1069,18 @@
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.81"
+version = "0.9.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176be2629957c157240f68f61f2d0053ad3a4ecfdd9ebf1e6521d18d9635cf67"
+checksum = "3a20eace9dc2d82904039cb76dcf50fb1a0bba071cfd1629720b5d6f1ddba0fa"
 dependencies = [
- "autocfg",
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
@@ -1070,79 +1122,80 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.52"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d0e1ae9e836cc3beddd63db0df682593d7e2d3d891ae8c9083d2113e1744224"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
+checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
 dependencies = [
  "cfg-if 1.0.0",
  "indoc",
+ "inventory",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "75439f995d07ddfad42b192dfcf3bc66a7ecfd8b4a1f5f6f046aa5c2c5d7677d"
+checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "839526a5c07a17ff44823679b68add4a58004de00512a95b6c1c98a6dcac0ee5"
+checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
+checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.1"
+version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
+checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
 version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
@@ -1301,17 +1354,17 @@
 name = "regex-syntax"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9ec002c35e86791825ed294b50008eea9ddfc8def4420124fbc6b08db834957"
 
 [[package]]
 name = "rustc-demangle"
-version = "0.1.21"
+version = "0.1.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ef03e0a2b150c7a90d01faf6254c9c48a41e95fb2a8c2ac1c6f0d2b9aefc342"
+checksum = "d4a36c42d1873f9a77c53bde094f9664d9891bc604a45b4798fd2c389ed12e5b"
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
@@ -1356,15 +1409,15 @@
 version = "0.8.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "109da1e6b197438deb6db99952990c7f959572794b80ff93707d55a232545e7c"
 dependencies = [
  "proc-macro2",
  "quote",
  "serde_derive_internals",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
@@ -1379,17 +1432,17 @@
 name = "semver"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 
 [[package]]
 name = "serde"
-version = "1.0.156"
+version = "1.0.159"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "314b5b092c0ade17c00142951e50ced110ec27cea304b1037c6969246c2469a4"
+checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-pickle"
 version = "1.1.1"
@@ -1401,39 +1454,39 @@
  "num-bigint",
  "num-traits",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.156"
+version = "1.0.159"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d7e29c4601e36bcec74a223228dce795f4cd3616341a4af93520ca1a837c087d"
+checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "serde_derive_internals"
 version = "0.26.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85bf8229e7920a9f636479437026331ce11aa132b4dde37d121944a44d6e5f3c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.94"
+version = "1.0.95"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c533a59c9d8a93a09c6ab31f0fd5e5f4dd1b8fc9434804029839884765d04ea"
+checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1460,14 +1513,25 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "tar"
 version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b55807c0344e1e6c04d7c965f5289c39a8d94ae23ed5c0b57aabac549f871c6"
 dependencies = [
  "filetime",
  "libc",
@@ -1487,30 +1551,30 @@
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.39"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5ab016db510546d856297882807df8da66a16fb8c4101cb8b30054b0d5b2d9c"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.39"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5420d42e90af0c38c3290abcca25b9b3bdf379fc9f55c528f53a269d9c9a267e"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.13",
 ]
 
 [[package]]
 name = "thread-id"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9539db560102d1cef46b8b78ce737ff0bb64e7e18d35b2a5688f7d097d0ff03"
@@ -1647,90 +1711,156 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
 name = "xattr"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d1526bbe5aaeb5eb06885f4d987bcdfa5e23187055de9b83fe00156a821fabc"
 dependencies = [
  "libc",
 ]
```

### Comparing `light_curve-0.7.1/PKG-INFO` & `light_curve-0.7.2b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,36 @@
 Metadata-Version: 2.1
 Name: light-curve
-Version: 0.7.1
+Version: 0.7.2b0
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Dist: numpy
 Requires-Dist: scipy
+Requires-Dist: feets; extra == 'test'
+Requires-Dist: joblib; extra == 'test'
+Requires-Dist: numpy; extra == 'test'
+Requires-Dist: pandas; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
+Requires-Dist: pytest-benchmark; extra == 'test'
+Requires-Dist: markdown-pytest; extra == 'test'
+Requires-Dist: pytest-subtests; extra == 'test'
+Requires-Dist: light-curve[test]; extra == 'dev'
+Requires-Dist: black; extra == 'dev'
+Requires-Dist: ruff; extra == 'dev'
+Provides-Extra: test
+Provides-Extra: dev
 Summary: Feature extractor from noisy time series
 Author: Konstantin Malanchev <hombit@gmail.com>, Anastasia Lavrukhina <lavrukhina.ad@gmail.com>
 Author-email: Konstantin Malanchev <hombit@gmail.com>, Anastasia Lavrukhina <lavrukhina.ad@gmail.com>
 License: GPL-3.0-or-later
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/light-curve/light-curve-python
@@ -39,22 +52,22 @@
 We also provide `light-curve-python` package which is just an "alias" to the main `light-curve` package.
 
 Minimum supported Python version is 3.7.
 We provide binary wheels via [PyPi](https://pypi.org/project/light-curve/) for number of platforms and architectures, both for CPython and PyPy.
 
 ### Support matrix
 
-| Arch \ OS   | Linux glibc | Linux musl                     | macOS                                                          | Windows                                                                |
-| ----------- |-------------|--------------------------------|----------------------------------------------------------------|------------------------------------------------------------------------|
-| **x86-64**  | wheel (MKL) | wheel (MKL)                    | wheel                                                          | not tested https://github.com/light-curve/light-curve-python/issues/12 |
-| **i686**    | src         | src                            | —                                                              | not tested                                                             |
-| **aarch64** | wheel       | wheel                          | src https://github.com/light-curve/light-curve-python/issues/5 | not tested                                                             |
-| **ppc64le** | wheel       | not tested (no Rust toolchain) | —                                                              | —                                                                      |
+| Arch \ OS   | Linux glibc | Linux musl                     | macOS                                                          | Windows https://github.com/light-curve/light-curve-python/issues/186 |
+| ----------- |-------------|--------------------------------|----------------------------------------------------------------|----------------------------------------------------------------------|
+| **x86-64**  | wheel (MKL) | wheel (MKL)                    | wheel                                                          | wheel (no Ceres, no GSL)                                             |
+| **i686**    | src         | src                            | —                                                              | not tested                                                           |
+| **aarch64** | wheel       | wheel                          | src https://github.com/light-curve/light-curve-python/issues/5 | not tested                                                           |
+| **ppc64le** | wheel       | not tested (no Rust toolchain) | —                                                              | —                                                                    |
 
-- "wheel": binary wheel is available on pypi.org, local building is not required for the platform, the only pre-requirement is a recent `pip` version. For Linux x86-64 we provide binary wheels built with Intel MKL for better periodogram perfromance, which is not a default build option.
+- "wheel": binary wheel is available on pypi.org, local building is not required for the platform, the only pre-requirement is a recent `pip` version. For Linux x86-64 we provide binary wheels built with Intel MKL for better periodogram performance, which is not a default build option. For Windows x86-64 we provide wheel with no Ceres and no GSL support, which is not a default build option.
 - "src": the package is confirmed to be built and pass unit tests locally, but testing and package building is not supported by CI. It is required to have the [GNU scientific library (GSL)](https://www.gnu.org/software/gsl/) v2.1+ and the [Rust toolchain](https://rust-lang.org) v1.57+ to install it via `pip install`.
 - "not tested": building from the source code is not tested, please report us building status via issue/PR/email.
 
 We build aarch64 macOS 12.0+ Python 3.8+ wheels locally and submit them running this command in `light-curve` directory:
 ```
 rm -rf ./wheelhouse
 CIBW_BUILD='cp3*-macosx_arm64' CIBW_ENVIRONMENT="MACOSX_DEPLOYMENT_TARGET=12.0 MATURIN_PEP517_ARGS='--locked --no-default-features --features ceres-source,fftw-source,gsl'" CIBW_BEFORE_ALL='curl https://sh.rustup.rs -sSf | sh -s -- --default-toolchain stable -y; brew install gsl' python3 -mcibuildwheel --platform macos
@@ -62,14 +75,15 @@
 ```
 
 ## Feature evaluators
 
 Most of the classes implement various feature evaluators useful for light-curve based
 astrophysical source classification and characterisation.
 
+<!-- name: test_feature_evaluators_basic -->
 ```python
 import light_curve as lc
 import numpy as np
 
 # Time values can be non-evenly separated but must be an ascending array
 n = 101
 t = np.linspace(0.0, 1.0, n)
@@ -103,21 +117,23 @@
 
 If you confident in your inputs you could use `sorted = True` (`t` is in ascending order)
 and `check = False` (no NaNs in inputs, no infs in `t` or `m`) for better performance.
 Note that if your inputs are not valid and are not validated by
 `sorted=None` and `check=True` (default values) then all kind of bad things could happen.
 
 Print feature classes list
+<!-- name: test_feature_evaluators_list -->
 ```python
 import light_curve as lc
 
 print([x for x in dir(lc) if hasattr(getattr(lc, x), "names")])
 ```
 
 Read feature docs
+<!-- name: test_feature_evaluators_help -->
 ```python
 import light_curve as lc
 
 help(lc.BazinFit)
 ```
 
 ### Experimental extractors
@@ -125,14 +141,15 @@
 From the technical point of view the package consists of two parts: a wrapper for [`light-curve-feature` Rust crate](https://crates.io/crates/light-curve-feature) (`light_curve_ext` sub-package) and pure Python sub-package `light_curve_py`.
 We use the Python implementation of feature extractors to test Rust implementation and to implement new experimental extractors.
 Please note, that the Python implementation is much slower for the most of the extractors and doesn't provide the same functionality as the Rust implementation.
 However, the Python implementation provides some new feature extractors you can find useful.
 
 You can manually use extractors from both implementations:
 
+<!-- name: test_experimental_extractors -->
 ```python
 import numpy as np
 from numpy.testing import assert_allclose
 from light_curve.light_curve_ext import LinearTrend as RustLinearTrend
 from light_curve.light_curve_py import LinearTrend as PythonLinearTrend
 
 rust_fe = RustLinearTrend()
@@ -437,14 +454,15 @@
 
 See benchmarks' descriptions in more details in ["Performant feature extraction for photometric time series"](https://arxiv.org/abs/2302.10837).
 
 ## dm-dt map
 
 Class `DmDt` provides dm–dt mapper (based on [Mahabal et al. 2011](https://ui.adsabs.harvard.edu/abs/2011BASI...39..387M/abstract), [Soraisam et al. 2020](https://ui.adsabs.harvard.edu/abs/2020ApJ...892..112S/abstract)). It is a Python wrapper for [`light-curve-dmdt` Rust crate](https://crates.io/crates/light-curve-dmdt).
 
+<!-- name: test_dmdt -->
 ```python
 import numpy as np
 from light_curve import DmDt
 from numpy.testing import assert_array_equal
 
 dmdt = DmDt.from_borders(min_lgdt=0, max_lgdt=np.log10(3), max_abs_dm=3, lgdt_size=2, dm_size=4, norm=[])
```

