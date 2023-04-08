# Comparing `tmp/dycw_utilities-0.8.5.tar.gz` & `tmp/dycw_utilities-0.8.6.tar.gz`

## Comparing `dycw_utilities-0.8.5.tar` & `dycw_utilities-0.8.6.tar`

### file list

```diff
@@ -1,222 +1,222 @@
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/.envrc
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/.rgiginore
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/Makefile
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/conftest.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/noxfile.py
--rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/requirements-dev.txt
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/requirements.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/.github/workflows/pull-request.yml
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/.github/workflows/push.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/conftest.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_airium.py
--rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_atomicwrites.py
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_beartype.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_bidict.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_class_name.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_clean_dir.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_cryptography.py
--rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_cvxpy.py
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_datetime.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_email.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_enum.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_errors.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_fastapi.py
--rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_fastparquet.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_fpdf2.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_getpass.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_git.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_hashlib.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_hatch.py
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_iterables.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_json.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_logging.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_memory_profiler.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_modules.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_monitor_memory.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_more_itertools.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_os.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_pathlib.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_pickle.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_pqdm.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_pyinstrument.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_pypi_server.py
--rw-r--r--   0        0        0     5473 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_pytest.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_pytest_check.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_random.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_re.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_scipy.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_semver.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_sentinel.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_socket.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_subprocess.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_sys.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_tempfile.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_text.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_timer.py
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_tqdm.py
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_typed_settings.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_types.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_typing.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_warnings.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_zipfile.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/test_zoneinfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/attrs/__init__.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/attrs/test_attrs.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/attrs/test_xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/click/__init__.py
--rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/click/test_click.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/click/test_luigi.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/click/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/holoviews/__init__.py
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/holoviews/test_holoviews.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/holoviews/test_xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/hypothesis/__init__.py
--rw-r--r--   0        0        0    10520 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/hypothesis/test_hypothesis.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/hypothesis/test_luigi.py
--rw-r--r--   0        0        0    17438 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/hypothesis/test_numpy.py
--rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/hypothesis/test_pandas.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/hypothesis/test_semver.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/hypothesis/test_sqlalchemy.py
--rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/hypothesis/test_xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/loguru/__init__.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/loguru/script_to_test_luigi.py
--rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/loguru/test_loguru.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/luigi/__init__.py
--rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/luigi/test_attrs.py
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/luigi/test_luigi.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/luigi/test_semver.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/luigi/test_server.py
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/luigi/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/math/__init__.py
--rw-r--r--   0        0        0    16876 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/math/test_math.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/math/test_typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/modules/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/modules/standalone.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/modules/package_with/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/modules/package_with/outer_1.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/modules/package_with/outer_2.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/modules/package_with/subpackage/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/modules/package_with/subpackage/inner_1.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/modules/package_with/subpackage/inner_2.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/modules/package_with/subpackage/inner_3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/modules/package_without/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/modules/package_without/module_1.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/modules/package_without/module_2.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/numpy/__init__.py
--rw-r--r--   0        0        0    45851 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/numpy/test_numpy.py
--rw-r--r--   0        0        0    19109 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/numpy/test_typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/pandas/__init__.py
--rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/pandas/test_pandas.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/pandas/test_typing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/sqlalchemy/test_fastparquet.py
--rw-r--r--   0        0        0    14095 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/sqlalchemy/test_pandas.py
--rw-r--r--   0        0        0    38826 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/sqlalchemy/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/xarray/__init__.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/xarray/test_typing.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/xarray/test_xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/zarr/__init__.py
--rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/zarr/test_xarray.py
--rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/tests/zarr/test_zarr.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/__init__.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/airium.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/atomicwrites.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/beartype.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/bidict.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/class_name.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/cryptography.py
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/cvxpy.py
--rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/datetime.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/email.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/enum.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/errors.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/fastapi.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/fastparquet.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/fpdf2.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/getpass.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/git.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/hashlib.py
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/hatch.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/iterables.py
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/json.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/logging.py
--rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/loguru.py
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/memory_profiler.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/modules.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/more_itertools.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/os.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/pathlib.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/pickle.py
--rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/pqdm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/py.typed
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/pyinstrument.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/pytest.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/pytest_check.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/random.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/re.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/scipy.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/semver.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/sentinel.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/socket.py
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/subprocess.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/sys.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/tempfile.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/text.py
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/timer.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/tqdm.py
--rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/typed_settings.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/types.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/typing.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/warnings.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/zipfile.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/zoneinfo.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/attrs/__init__.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/attrs/xarray.py
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/clean_dir/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/clean_dir/__main__.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/clean_dir/classes.py
--rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/click/__init__.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/click/luigi.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/click/sqlalchemy.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/holoviews/__init__.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/holoviews/xarray.py
--rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/hypothesis/__init__.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/hypothesis/luigi.py
--rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/hypothesis/numpy.py
--rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/hypothesis/pandas.py
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/hypothesis/semver.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/hypothesis/sqlalchemy.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/hypothesis/typing.py
--rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/hypothesis/xarray.py
--rw-r--r--   0        0        0    11310 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/luigi/__init__.py
--rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/luigi/attrs.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/luigi/semver.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/luigi/sqlalchemy.py
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/luigi/server/__init__.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/luigi/server/__main__.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/luigi/server/classes.py
--rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/math/__init__.py
--rw-r--r--   0        0        0    14378 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/math/typing.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/monitor_memory/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/monitor_memory/__main__.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/monitor_memory/classes.py
--rw-r--r--   0        0        0    17896 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/numpy/__init__.py
--rw-r--r--   0        0        0    32371 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/numpy/typing.py
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/pandas/__init__.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/pandas/typing.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/pypi_server/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/pypi_server/__main__.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/pypi_server/classes.py
--rw-r--r--   0        0        0    25497 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/sqlalchemy/fastparquet.py
--rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/sqlalchemy/pandas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/xarray/__init__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/xarray/typing.py
--rw-r--r--   0        0        0    10192 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/zarr/__init__.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/utilities/zarr/xarray.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/.gitignore
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/README.md
--rw-r--r--   0        0        0     7941 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/pyproject.toml
--rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 dycw_utilities-0.8.5/PKG-INFO
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/.envrc
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/.rgiginore
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/Makefile
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/conftest.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/noxfile.py
+-rw-r--r--   0        0        0     8898 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/requirements-dev.txt
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/requirements.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/.github/workflows/pull-request.yml
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/.github/workflows/push.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/conftest.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_airium.py
+-rw-r--r--   0        0        0     3129 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_atomicwrites.py
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_beartype.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_bidict.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_class_name.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_clean_dir.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_cryptography.py
+-rw-r--r--   0        0        0    12950 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_cvxpy.py
+-rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_datetime.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_email.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_enum.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_errors.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_fastapi.py
+-rw-r--r--   0        0        0     9283 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_fastparquet.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_fpdf2.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_getpass.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_git.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_hashlib.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_hatch.py
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_iterables.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_json.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_logging.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_memory_profiler.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_modules.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_monitor_memory.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_more_itertools.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_os.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_pathlib.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_pickle.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_pqdm.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_pyinstrument.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_pypi_server.py
+-rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_pytest.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_pytest_check.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_random.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_re.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_scipy.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_semver.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_sentinel.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_socket.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_subprocess.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_sys.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_tempfile.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_text.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_timer.py
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_tqdm.py
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_typed_settings.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_types.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_typing.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_warnings.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_zipfile.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/test_zoneinfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/attrs/__init__.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/attrs/test_attrs.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/attrs/test_xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/click/__init__.py
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/click/test_click.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/click/test_luigi.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/click/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/holoviews/__init__.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/holoviews/test_holoviews.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/holoviews/test_xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/hypothesis/__init__.py
+-rw-r--r--   0        0        0    10520 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/hypothesis/test_hypothesis.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/hypothesis/test_luigi.py
+-rw-r--r--   0        0        0    17438 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/hypothesis/test_numpy.py
+-rw-r--r--   0        0        0     4351 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/hypothesis/test_pandas.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/hypothesis/test_semver.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/hypothesis/test_sqlalchemy.py
+-rw-r--r--   0        0        0     6672 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/hypothesis/test_xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/loguru/__init__.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/loguru/script_to_test_luigi.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/loguru/test_loguru.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/luigi/__init__.py
+-rw-r--r--   0        0        0     8140 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/luigi/test_attrs.py
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/luigi/test_luigi.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/luigi/test_semver.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/luigi/test_server.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/luigi/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/math/__init__.py
+-rw-r--r--   0        0        0    16876 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/math/test_math.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/math/test_typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/modules/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/modules/standalone.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/modules/package_with/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/modules/package_with/outer_1.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/modules/package_with/outer_2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/modules/package_with/subpackage/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/modules/package_with/subpackage/inner_1.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/modules/package_with/subpackage/inner_2.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/modules/package_with/subpackage/inner_3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/modules/package_without/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/modules/package_without/module_1.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/modules/package_without/module_2.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/numpy/__init__.py
+-rw-r--r--   0        0        0    45851 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/numpy/test_numpy.py
+-rw-r--r--   0        0        0    19109 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/numpy/test_typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/pandas/__init__.py
+-rw-r--r--   0        0        0    10922 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/pandas/test_pandas.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/pandas/test_typing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/sqlalchemy/test_fastparquet.py
+-rw-r--r--   0        0        0    14095 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/sqlalchemy/test_pandas.py
+-rw-r--r--   0        0        0    38826 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/sqlalchemy/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/xarray/__init__.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/xarray/test_typing.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/xarray/test_xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/zarr/__init__.py
+-rw-r--r--   0        0        0     7324 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/zarr/test_xarray.py
+-rw-r--r--   0        0        0    10301 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/tests/zarr/test_zarr.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/__init__.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/airium.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/atomicwrites.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/beartype.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/bidict.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/class_name.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/cryptography.py
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/cvxpy.py
+-rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/datetime.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/email.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/enum.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/errors.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/fastapi.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/fastparquet.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/fpdf2.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/getpass.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/git.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/hashlib.py
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/hatch.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/iterables.py
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/json.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/logging.py
+-rw-r--r--   0        0        0     6924 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/loguru.py
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/memory_profiler.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/modules.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/more_itertools.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/os.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/pathlib.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/pickle.py
+-rw-r--r--   0        0        0     8490 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/pqdm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/py.typed
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/pyinstrument.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/pytest.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/pytest_check.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/random.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/re.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/scipy.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/semver.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/sentinel.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/socket.py
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/subprocess.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/sys.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/tempfile.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/text.py
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/timer.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/tqdm.py
+-rw-r--r--   0        0        0     5853 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/typed_settings.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/types.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/typing.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/warnings.py
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/zipfile.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/zoneinfo.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/attrs/__init__.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/attrs/xarray.py
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/clean_dir/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/clean_dir/__main__.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/clean_dir/classes.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/click/__init__.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/click/luigi.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/click/sqlalchemy.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/holoviews/__init__.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/holoviews/xarray.py
+-rw-r--r--   0        0        0     9369 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/hypothesis/__init__.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/hypothesis/luigi.py
+-rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/hypothesis/numpy.py
+-rw-r--r--   0        0        0     4448 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/hypothesis/pandas.py
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/hypothesis/semver.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/hypothesis/sqlalchemy.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/hypothesis/typing.py
+-rw-r--r--   0        0        0     6071 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/hypothesis/xarray.py
+-rw-r--r--   0        0        0    11310 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/luigi/__init__.py
+-rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/luigi/attrs.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/luigi/semver.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/luigi/sqlalchemy.py
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/luigi/server/__init__.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/luigi/server/__main__.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/luigi/server/classes.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/math/__init__.py
+-rw-r--r--   0        0        0    14378 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/math/typing.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/monitor_memory/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/monitor_memory/__main__.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/monitor_memory/classes.py
+-rw-r--r--   0        0        0    17896 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/numpy/__init__.py
+-rw-r--r--   0        0        0    32371 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/numpy/typing.py
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/pandas/__init__.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/pandas/typing.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/pypi_server/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/pypi_server/__main__.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/pypi_server/classes.py
+-rw-r--r--   0        0        0    25497 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/sqlalchemy/fastparquet.py
+-rw-r--r--   0        0        0    10357 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/sqlalchemy/pandas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/xarray/__init__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/xarray/typing.py
+-rw-r--r--   0        0        0    10192 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/zarr/__init__.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/utilities/zarr/xarray.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/.gitignore
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/README.md
+-rw-r--r--   0        0        0     8112 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/pyproject.toml
+-rw-r--r--   0        0        0     9511 2020-02-02 00:00:00.000000 dycw_utilities-0.8.6/PKG-INFO
```

### Comparing `dycw_utilities-0.8.5/.pre-commit-config.yaml` & `dycw_utilities-0.8.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/noxfile.py` & `dycw_utilities-0.8.6/noxfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/requirements-dev.txt` & `dycw_utilities-0.8.6/requirements-dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -294,22 +294,25 @@
     # via urllib3
 pytest==7.2.2
     # via
     #   dycw-utilities (pyproject.toml)
     #   pytest-check
     #   pytest-cov
     #   pytest-instafail
+    #   pytest-randomly
     #   pytest-rerunfailures
     #   pytest-xdist
 pytest-check==2.1.4
     # via dycw-utilities (pyproject.toml)
 pytest-cov==4.0.0
     # via dycw-utilities (pyproject.toml)
 pytest-instafail==0.5.0
     # via dycw-utilities (pyproject.toml)
+pytest-randomly==3.12.0
+    # via dycw-utilities (pyproject.toml)
 pytest-rerunfailures==11.1.2
     # via dycw-utilities (pyproject.toml)
 pytest-xdist==3.2.1
     # via dycw-utilities (pyproject.toml)
 python-daemon==3.0.1
     # via luigi
 python-dateutil==2.8.2
```

### Comparing `dycw_utilities-0.8.5/.github/workflows/pull-request.yml` & `dycw_utilities-0.8.6/.github/workflows/pull-request.yml`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/.github/workflows/push.yml` & `dycw_utilities-0.8.6/.github/workflows/push.yml`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_airium.py` & `dycw_utilities-0.8.6/tests/test_airium.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_atomicwrites.py` & `dycw_utilities-0.8.6/tests/test_atomicwrites.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_beartype.py` & `dycw_utilities-0.8.6/tests/test_beartype.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_bidict.py` & `dycw_utilities-0.8.6/tests/test_bidict.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_class_name.py` & `dycw_utilities-0.8.6/tests/test_class_name.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_clean_dir.py` & `dycw_utilities-0.8.6/tests/test_clean_dir.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_cryptography.py` & `dycw_utilities-0.8.6/tests/test_cryptography.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_cvxpy.py` & `dycw_utilities-0.8.6/tests/test_cvxpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_datetime.py` & `dycw_utilities-0.8.6/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_email.py` & `dycw_utilities-0.8.6/tests/test_email.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_enum.py` & `dycw_utilities-0.8.6/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_errors.py` & `dycw_utilities-0.8.6/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_fastapi.py` & `dycw_utilities-0.8.6/tests/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_fastparquet.py` & `dycw_utilities-0.8.6/tests/test_fastparquet.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_fpdf2.py` & `dycw_utilities-0.8.6/tests/test_fpdf2.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_git.py` & `dycw_utilities-0.8.6/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_hashlib.py` & `dycw_utilities-0.8.6/tests/test_hashlib.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_iterables.py` & `dycw_utilities-0.8.6/tests/test_iterables.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_json.py` & `dycw_utilities-0.8.6/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_modules.py` & `dycw_utilities-0.8.6/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_monitor_memory.py` & `dycw_utilities-0.8.6/tests/test_monitor_memory.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_more_itertools.py` & `dycw_utilities-0.8.6/tests/test_more_itertools.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_os.py` & `dycw_utilities-0.8.6/tests/test_os.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_pathlib.py` & `dycw_utilities-0.8.6/tests/test_pathlib.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_pickle.py` & `dycw_utilities-0.8.6/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_pqdm.py` & `dycw_utilities-0.8.6/tests/test_pqdm.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_pypi_server.py` & `dycw_utilities-0.8.6/tests/test_pypi_server.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_pytest.py` & `dycw_utilities-0.8.6/tests/test_pytest.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 
 class TestPytestOptions:
     def test_unknown_mark(self, testdir: Any) -> None:
         testdir.makepyfile(
             """
             from pytest import mark
 
-            @mark.slow
+            @mark.unknown
             def test_main():
                 assert True
             """
         )
         result = testdir.runpytest()
         result.assert_outcomes(errors=1)
-        result.stdout.re_match_lines([r".*Unknown pytest\.mark\.slow"])
+        result.stdout.re_match_lines([r".*Unknown pytest\.mark\.unknown"])
 
     def test_configured_mark_unknown_option(self, testdir: Any) -> None:
         testdir.makeconftest(
             """
             from utilities.pytest import add_pytest_configure
 
             def pytest_configure(config):
@@ -88,18 +88,32 @@
     @mark.parametrize(
         ("case", "passed", "skipped", "matches"),
         [
             param(
                 [],
                 1,
                 3,
-                [".*6: pass --slow", ".*10: pass --fast", ".*14: pass --slow --fast"],
+                [
+                    "SKIPPED.*: pass --slow",
+                    "SKIPPED.*: pass --fast",
+                    "SKIPPED.*: pass --slow --fast",
+                ],
+            ),
+            param(
+                ["--slow"],
+                2,
+                2,
+                ["SKIPPED.*: pass --fast", "SKIPPED.*: pass --slow --fast"],
+            ),
+            param(
+                ["--fast"],
+                2,
+                2,
+                ["SKIPPED.*: pass --slow", "SKIPPED.*: pass --slow --fast"],
             ),
-            param(["--slow"], 2, 2, [".*10: pass --fast", ".*14: pass --slow --fast"]),
-            param(["--fast"], 2, 2, [".*6: pass --slow", ".*14: pass --slow --fast"]),
             param(["--slow", "--fast"], 4, 0, []),
         ],
     )
     def test_configured_two_marks_and_options(
         self,
         testdir: Any,
         case: list[str],
@@ -144,15 +158,15 @@
 
             @mark.slow
             @mark.fast
             def test_both():
                 assert True
             """
         )
-        result = testdir.runpytest("-rs", *case)
+        result = testdir.runpytest("-rs", *case, "--randomly-dont-reorganize")
         result.assert_outcomes(passed=passed, skipped=skipped)
         result.stdout.re_match_lines(matches)
 
 
 class TestIsPytest:
     def test_function(self) -> None:
         assert is_pytest()
```

### Comparing `dycw_utilities-0.8.5/tests/test_pytest_check.py` & `dycw_utilities-0.8.6/tests/test_pytest_check.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_re.py` & `dycw_utilities-0.8.6/tests/test_re.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_scipy.py` & `dycw_utilities-0.8.6/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_subprocess.py` & `dycw_utilities-0.8.6/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_tempfile.py` & `dycw_utilities-0.8.6/tests/test_tempfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_text.py` & `dycw_utilities-0.8.6/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_timer.py` & `dycw_utilities-0.8.6/tests/test_timer.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_tqdm.py` & `dycw_utilities-0.8.6/tests/test_tqdm.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_typed_settings.py` & `dycw_utilities-0.8.6/tests/test_typed_settings.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_types.py` & `dycw_utilities-0.8.6/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_warnings.py` & `dycw_utilities-0.8.6/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/test_zipfile.py` & `dycw_utilities-0.8.6/tests/test_zipfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/attrs/test_attrs.py` & `dycw_utilities-0.8.6/tests/attrs/test_attrs.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/attrs/test_xarray.py` & `dycw_utilities-0.8.6/tests/attrs/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/click/test_click.py` & `dycw_utilities-0.8.6/tests/click/test_click.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/click/test_luigi.py` & `dycw_utilities-0.8.6/tests/click/test_luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/click/test_sqlalchemy.py` & `dycw_utilities-0.8.6/tests/click/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/holoviews/test_holoviews.py` & `dycw_utilities-0.8.6/tests/holoviews/test_holoviews.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/holoviews/test_xarray.py` & `dycw_utilities-0.8.6/tests/holoviews/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/hypothesis/test_hypothesis.py` & `dycw_utilities-0.8.6/tests/hypothesis/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/hypothesis/test_luigi.py` & `dycw_utilities-0.8.6/tests/hypothesis/test_luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/hypothesis/test_numpy.py` & `dycw_utilities-0.8.6/tests/hypothesis/test_numpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/hypothesis/test_pandas.py` & `dycw_utilities-0.8.6/tests/hypothesis/test_pandas.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/hypothesis/test_semver.py` & `dycw_utilities-0.8.6/tests/hypothesis/test_semver.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/hypothesis/test_sqlalchemy.py` & `dycw_utilities-0.8.6/tests/hypothesis/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/hypothesis/test_xarray.py` & `dycw_utilities-0.8.6/tests/hypothesis/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/loguru/script_to_test_luigi.py` & `dycw_utilities-0.8.6/tests/loguru/script_to_test_luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/loguru/test_loguru.py` & `dycw_utilities-0.8.6/tests/loguru/test_loguru.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/luigi/test_attrs.py` & `dycw_utilities-0.8.6/tests/luigi/test_attrs.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/luigi/test_luigi.py` & `dycw_utilities-0.8.6/tests/luigi/test_luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/luigi/test_server.py` & `dycw_utilities-0.8.6/tests/luigi/test_server.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/luigi/test_sqlalchemy.py` & `dycw_utilities-0.8.6/tests/luigi/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/math/test_math.py` & `dycw_utilities-0.8.6/tests/math/test_math.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/math/test_typing.py` & `dycw_utilities-0.8.6/tests/math/test_typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/numpy/test_numpy.py` & `dycw_utilities-0.8.6/tests/numpy/test_numpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/numpy/test_typing.py` & `dycw_utilities-0.8.6/tests/numpy/test_typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/pandas/test_pandas.py` & `dycw_utilities-0.8.6/tests/pandas/test_pandas.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/pandas/test_typing.py` & `dycw_utilities-0.8.6/tests/pandas/test_typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/sqlalchemy/test_fastparquet.py` & `dycw_utilities-0.8.6/tests/sqlalchemy/test_fastparquet.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/sqlalchemy/test_pandas.py` & `dycw_utilities-0.8.6/tests/sqlalchemy/test_pandas.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/sqlalchemy/test_sqlalchemy.py` & `dycw_utilities-0.8.6/tests/sqlalchemy/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/xarray/test_typing.py` & `dycw_utilities-0.8.6/tests/xarray/test_typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/zarr/test_xarray.py` & `dycw_utilities-0.8.6/tests/zarr/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/tests/zarr/test_zarr.py` & `dycw_utilities-0.8.6/tests/zarr/test_zarr.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/atomicwrites.py` & `dycw_utilities-0.8.6/utilities/atomicwrites.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/bidict.py` & `dycw_utilities-0.8.6/utilities/bidict.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/cryptography.py` & `dycw_utilities-0.8.6/utilities/cryptography.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/cvxpy.py` & `dycw_utilities-0.8.6/utilities/cvxpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/datetime.py` & `dycw_utilities-0.8.6/utilities/datetime.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/email.py` & `dycw_utilities-0.8.6/utilities/email.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/enum.py` & `dycw_utilities-0.8.6/utilities/enum.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/errors.py` & `dycw_utilities-0.8.6/utilities/errors.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/fastapi.py` & `dycw_utilities-0.8.6/utilities/fastapi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/fastparquet.py` & `dycw_utilities-0.8.6/utilities/fastparquet.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/fpdf2.py` & `dycw_utilities-0.8.6/utilities/fpdf2.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/git.py` & `dycw_utilities-0.8.6/utilities/git.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/hatch.py` & `dycw_utilities-0.8.6/utilities/hatch.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/iterables.py` & `dycw_utilities-0.8.6/utilities/iterables.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/json.py` & `dycw_utilities-0.8.6/utilities/json.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/logging.py` & `dycw_utilities-0.8.6/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/loguru.py` & `dycw_utilities-0.8.6/utilities/loguru.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/memory_profiler.py` & `dycw_utilities-0.8.6/utilities/memory_profiler.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/modules.py` & `dycw_utilities-0.8.6/utilities/modules.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/more_itertools.py` & `dycw_utilities-0.8.6/utilities/more_itertools.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/os.py` & `dycw_utilities-0.8.6/utilities/os.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/pickle.py` & `dycw_utilities-0.8.6/utilities/pickle.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/pqdm.py` & `dycw_utilities-0.8.6/utilities/pqdm.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/pyinstrument.py` & `dycw_utilities-0.8.6/utilities/pyinstrument.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/pytest.py` & `dycw_utilities-0.8.6/utilities/pytest.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/re.py` & `dycw_utilities-0.8.6/utilities/re.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/scipy.py` & `dycw_utilities-0.8.6/utilities/scipy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/sentinel.py` & `dycw_utilities-0.8.6/utilities/sentinel.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/subprocess.py` & `dycw_utilities-0.8.6/utilities/subprocess.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/tempfile.py` & `dycw_utilities-0.8.6/utilities/tempfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/text.py` & `dycw_utilities-0.8.6/utilities/text.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/timer.py` & `dycw_utilities-0.8.6/utilities/timer.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/tqdm.py` & `dycw_utilities-0.8.6/utilities/tqdm.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/typed_settings.py` & `dycw_utilities-0.8.6/utilities/typed_settings.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/types.py` & `dycw_utilities-0.8.6/utilities/types.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/warnings.py` & `dycw_utilities-0.8.6/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/zipfile.py` & `dycw_utilities-0.8.6/utilities/zipfile.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/attrs/__init__.py` & `dycw_utilities-0.8.6/utilities/attrs/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/clean_dir/__init__.py` & `dycw_utilities-0.8.6/utilities/clean_dir/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/clean_dir/classes.py` & `dycw_utilities-0.8.6/utilities/clean_dir/classes.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/click/__init__.py` & `dycw_utilities-0.8.6/utilities/click/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/click/luigi.py` & `dycw_utilities-0.8.6/utilities/click/luigi.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/click/sqlalchemy.py` & `dycw_utilities-0.8.6/utilities/click/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/holoviews/__init__.py` & `dycw_utilities-0.8.6/utilities/holoviews/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/holoviews/xarray.py` & `dycw_utilities-0.8.6/utilities/holoviews/xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/hypothesis/__init__.py` & `dycw_utilities-0.8.6/utilities/hypothesis/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/hypothesis/numpy.py` & `dycw_utilities-0.8.6/utilities/hypothesis/numpy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/hypothesis/pandas.py` & `dycw_utilities-0.8.6/utilities/hypothesis/pandas.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/hypothesis/semver.py` & `dycw_utilities-0.8.6/utilities/hypothesis/semver.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/hypothesis/sqlalchemy.py` & `dycw_utilities-0.8.6/utilities/hypothesis/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/hypothesis/xarray.py` & `dycw_utilities-0.8.6/utilities/hypothesis/xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/luigi/__init__.py` & `dycw_utilities-0.8.6/utilities/luigi/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/luigi/attrs.py` & `dycw_utilities-0.8.6/utilities/luigi/attrs.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/luigi/semver.py` & `dycw_utilities-0.8.6/utilities/luigi/semver.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/luigi/sqlalchemy.py` & `dycw_utilities-0.8.6/utilities/luigi/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/luigi/server/__init__.py` & `dycw_utilities-0.8.6/utilities/luigi/server/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/luigi/server/classes.py` & `dycw_utilities-0.8.6/utilities/luigi/server/classes.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/math/__init__.py` & `dycw_utilities-0.8.6/utilities/math/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/math/typing.py` & `dycw_utilities-0.8.6/utilities/math/typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/monitor_memory/__init__.py` & `dycw_utilities-0.8.6/utilities/monitor_memory/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/monitor_memory/classes.py` & `dycw_utilities-0.8.6/utilities/monitor_memory/classes.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/numpy/__init__.py` & `dycw_utilities-0.8.6/utilities/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/numpy/typing.py` & `dycw_utilities-0.8.6/utilities/numpy/typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/pandas/__init__.py` & `dycw_utilities-0.8.6/utilities/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/pandas/typing.py` & `dycw_utilities-0.8.6/utilities/pandas/typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/pypi_server/__init__.py` & `dycw_utilities-0.8.6/utilities/pypi_server/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/pypi_server/classes.py` & `dycw_utilities-0.8.6/utilities/pypi_server/classes.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/sqlalchemy/__init__.py` & `dycw_utilities-0.8.6/utilities/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/sqlalchemy/fastparquet.py` & `dycw_utilities-0.8.6/utilities/sqlalchemy/fastparquet.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/sqlalchemy/pandas.py` & `dycw_utilities-0.8.6/utilities/sqlalchemy/pandas.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/xarray/typing.py` & `dycw_utilities-0.8.6/utilities/xarray/typing.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/zarr/__init__.py` & `dycw_utilities-0.8.6/utilities/zarr/__init__.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/utilities/zarr/xarray.py` & `dycw_utilities-0.8.6/utilities/zarr/xarray.py`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/.gitignore` & `dycw_utilities-0.8.6/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -123,15 +123,14 @@
 .env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
-.direnv/
 
 # Spyder project settings
 .spyderproject
 .spyproject
 
 # Rope project settings
 .ropeproject
@@ -156,12 +155,11 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
-# jupyter
-*.ipynb
-
-# ruff
+# extra
+.direnv/
 .ruff_cache/
+Untitled.ipynb
```

### Comparing `dycw_utilities-0.8.5/README.md` & `dycw_utilities-0.8.6/README.md`

 * *Files identical despite different names*

### Comparing `dycw_utilities-0.8.5/pyproject.toml` & `dycw_utilities-0.8.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -165,26 +165,32 @@
 ]
 test = [
   "atomicwrites >= 1.4.1",
   "exceptiongroup >= 1.1.1",
   "hypothesis >= 6.71.0",
   "pytest >= 7.2.2",
   "pytest-check >= 2.1.4",
+  "pytest-cov >= 4.0.0",
+  "pytest-instafail >= 0.5.0",
+  "pytest-randomly >= 3.12.0",
+  "pytest-rerunfailures >= 11.1.2",
+  "pytest-xdist >= 3.2.1",
 ]
 # dev
 dev = [
   # main
   "airium",
   "atomicwrites",
   "attrs",
   "bidict",
   "bottleneck",
   "click",
   "cryptography",
   "cvxpy",
+  "exceptiongroup",
   "fastapi",
   "fastparquet",
   "fpdf2",
   "hatch",
   "holoviews",
   "hypothesis",
   "loguru",
@@ -195,40 +201,40 @@
   "pandas",
   "pqdm",
   "psutil",
   "pyinstrument",
   "pypi",
   "pytest",
   "pytest-check",
+  "pytest-cov",
+  "pytest-instafail",
+  "pytest-randomly",
+  "pytest-rerunfailures",
+  "pytest-xdist",
   "scipy",
   "selenium",
   "semver",
   "sqlalchemy",
   "timeout-decorator",
   "tqdm",
   "typed-settings[click]",
   "xarray",
   "zarr",
   # dev
   "black",
   "coverage-conditional-plugin",
   "cx_oracle",
-  "exceptiongroup",
   "freezegun",
   "hatch",
   "hypothesis-sqlalchemy",
   "mysqlclient",
   "nox",
   "pip-tools",
   "psycopg2",
   "pyodbc",
-  "pytest-cov",
-  "pytest-instafail",
-  "pytest-rerunfailures",
-  "pytest-xdist",
   "ruff",
 ]
 
 [project.scripts]
 clean-dir = "utilities.clean_dir:main"
 monitor-memory = "utilities.monitor_memory:main"
 start-luigi-server = "utilities.luigi.server:main"
```

### Comparing `dycw_utilities-0.8.5/PKG-INFO` & `dycw_utilities-0.8.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dycw-utilities
-Version: 0.8.5
+Version: 0.8.6
 Author-email: Derek Wan <d.wan@icloud.com>
 Requires-Python: >=3.9
 Requires-Dist: beartype>=0.12.0
 Requires-Dist: typing-extensions>=4.4.0
 Provides-Extra: airium
 Requires-Dist: airium>=0.2.5; extra == 'airium'
 Provides-Extra: atomicwrites
@@ -82,14 +82,15 @@
 Requires-Dist: pyinstrument; extra == 'dev'
 Requires-Dist: pyodbc; extra == 'dev'
 Requires-Dist: pypi; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-check; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-instafail; extra == 'dev'
+Requires-Dist: pytest-randomly; extra == 'dev'
 Requires-Dist: pytest-rerunfailures; extra == 'dev'
 Requires-Dist: pytest-xdist; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: scipy; extra == 'dev'
 Requires-Dist: selenium; extra == 'dev'
 Requires-Dist: semver; extra == 'dev'
 Requires-Dist: sqlalchemy; extra == 'dev'
@@ -160,14 +161,19 @@
 Requires-Dist: sqlalchemy>=2.0.9; extra == 'sqlalchemy'
 Requires-Dist: timeout-decorator<0.6,>=0.5.0; extra == 'sqlalchemy'
 Provides-Extra: test
 Requires-Dist: atomicwrites>=1.4.1; extra == 'test'
 Requires-Dist: exceptiongroup>=1.1.1; extra == 'test'
 Requires-Dist: hypothesis>=6.71.0; extra == 'test'
 Requires-Dist: pytest-check>=2.1.4; extra == 'test'
+Requires-Dist: pytest-cov>=4.0.0; extra == 'test'
+Requires-Dist: pytest-instafail>=0.5.0; extra == 'test'
+Requires-Dist: pytest-randomly>=3.12.0; extra == 'test'
+Requires-Dist: pytest-rerunfailures>=11.1.2; extra == 'test'
+Requires-Dist: pytest-xdist>=3.2.1; extra == 'test'
 Requires-Dist: pytest>=7.2.2; extra == 'test'
 Provides-Extra: tqdm
 Requires-Dist: tqdm>=4.65.0; extra == 'tqdm'
 Provides-Extra: typed-settings
 Requires-Dist: typed-settings[click]>=23.0.0; extra == 'typed-settings'
 Provides-Extra: xarray
 Requires-Dist: bottleneck>=1.3.7; extra == 'xarray'
```

