# Comparing `tmp/fixit-0.1.4.tar.gz` & `tmp/fixit-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fixit-0.1.4.tar", last modified: Fri Jul 30 20:15:52 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `fixit-0.1.4.tar` & `fixit-2.0.0a1.tar`

### file list

```diff
@@ -1,127 +1,95 @@
-drwxr-xr-x   0 lisroach   (501) staff       (20)        0 2021-07-30 20:15:52.000000 fixit-0.1.4/
--rw-r--r--   0 lisroach   (501) staff       (20)      244 2021-03-10 21:32:00.000000 fixit-0.1.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 lisroach   (501) staff       (20)       58 2021-03-10 21:32:00.000000 fixit-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 lisroach   (501) staff       (20)     3725 2021-03-10 21:32:00.000000 fixit-0.1.4/LICENSE
--rw-r--r--   0 lisroach   (501) staff       (20)      147 2021-06-01 22:55:21.000000 fixit-0.1.4/MANIFEST.in
--rw-r--r--   0 lisroach   (501) staff       (20)     5735 2021-07-30 20:15:52.000000 fixit-0.1.4/PKG-INFO
--rw-r--r--   0 lisroach   (501) staff       (20)     4102 2021-03-10 21:32:00.000000 fixit-0.1.4/README.rst
-drwxr-xr-x   0 lisroach   (501) staff       (20)        0 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit/
--rw-r--r--   0 lisroach   (501) staff       (20)      596 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/__init__.py
--rw-r--r--   0 lisroach   (501) staff       (20)      208 2021-07-30 20:13:55.000000 fixit-0.1.4/fixit/_version.py
-drwxr-xr-x   0 lisroach   (501) staff       (20)        0 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit/cli/
--rw-r--r--   0 lisroach   (501) staff       (20)     9159 2021-05-26 20:35:31.000000 fixit-0.1.4/fixit/cli/__init__.py
--rw-r--r--   0 lisroach   (501) staff       (20)     3791 2021-06-01 22:49:28.000000 fixit-0.1.4/fixit/cli/add_new_rule.py
--rw-r--r--   0 lisroach   (501) staff       (20)    10724 2021-07-30 20:13:43.000000 fixit-0.1.4/fixit/cli/apply_fix.py
--rw-r--r--   0 lisroach   (501) staff       (20)     7496 2021-07-30 20:13:43.000000 fixit-0.1.4/fixit/cli/args.py
--rw-r--r--   0 lisroach   (501) staff       (20)     2356 2021-04-19 21:46:55.000000 fixit-0.1.4/fixit/cli/formatter.py
--rw-r--r--   0 lisroach   (501) staff       (20)     2977 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/cli/full_repo_metadata.py
--rw-r--r--   0 lisroach   (501) staff       (20)      409 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/cli/init_config.py
--rw-r--r--   0 lisroach   (501) staff       (20)     8203 2021-07-30 20:13:43.000000 fixit-0.1.4/fixit/cli/insert_suppressions.py
--rw-r--r--   0 lisroach   (501) staff       (20)     1267 2021-04-02 22:20:47.000000 fixit-0.1.4/fixit/cli/main.py
--rw-r--r--   0 lisroach   (501) staff       (20)     5997 2021-07-30 20:13:55.000000 fixit-0.1.4/fixit/cli/run_rules.py
-drwxr-xr-x   0 lisroach   (501) staff       (20)        0 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit/cli/tests/
--rw-r--r--   0 lisroach   (501) staff       (20)      177 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/cli/tests/__init__.py
--rw-r--r--   0 lisroach   (501) staff       (20)      878 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/cli/tests/test_args.py
--rw-r--r--   0 lisroach   (501) staff       (20)     3028 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/cli/tests/test_formatter.py
--rw-r--r--   0 lisroach   (501) staff       (20)     3630 2021-05-26 19:02:27.000000 fixit-0.1.4/fixit/cli/tests/test_ipc.py
--rw-r--r--   0 lisroach   (501) staff       (20)     3867 2021-05-26 19:02:27.000000 fixit-0.1.4/fixit/cli/tests/test_lint_opts.py
--rw-r--r--   0 lisroach   (501) staff       (20)     5510 2021-05-26 20:35:31.000000 fixit-0.1.4/fixit/cli/tests/test_type_inference.py
--rw-r--r--   0 lisroach   (501) staff       (20)      713 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/cli/utils.py
-drwxr-xr-x   0 lisroach   (501) staff       (20)        0 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit/common/
--rw-r--r--   0 lisroach   (501) staff       (20)      177 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/__init__.py
--rw-r--r--   0 lisroach   (501) staff       (20)     6901 2021-06-01 22:49:28.000000 fixit-0.1.4/fixit/common/autofix.py
--rw-r--r--   0 lisroach   (501) staff       (20)     5023 2021-07-30 20:13:49.000000 fixit-0.1.4/fixit/common/base.py
-drwxr-xr-x   0 lisroach   (501) staff       (20)        0 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit/common/cli/
--rw-r--r--   0 lisroach   (501) staff       (20)      368 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/cli/__init__.py
--rw-r--r--   0 lisroach   (501) staff       (20)      625 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/cli/args.py
--rw-r--r--   0 lisroach   (501) staff       (20)      312 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/cli/formatter.py
--rw-r--r--   0 lisroach   (501) staff       (20)     1560 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/comments.py
--rw-r--r--   0 lisroach   (501) staff       (20)     5097 2021-07-30 20:13:49.000000 fixit-0.1.4/fixit/common/config.py
--rw-r--r--   0 lisroach   (501) staff       (20)     2007 2021-07-30 20:13:49.000000 fixit-0.1.4/fixit/common/config.schema.json
--rw-r--r--   0 lisroach   (501) staff       (20)     4265 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/document.py
--rw-r--r--   0 lisroach   (501) staff       (20)     6100 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/flake8_compat.py
--rw-r--r--   0 lisroach   (501) staff       (20)     3558 2021-05-26 21:43:53.000000 fixit-0.1.4/fixit/common/full_repo_metadata.py
--rw-r--r--   0 lisroach   (501) staff       (20)     4286 2021-06-02 20:31:21.000000 fixit-0.1.4/fixit/common/generate_pyre_fixtures.py
--rw-r--r--   0 lisroach   (501) staff       (20)    10998 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/ignores.py
--rw-r--r--   0 lisroach   (501) staff       (20)     6470 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/insert_suppressions.py
--rw-r--r--   0 lisroach   (501) staff       (20)     3084 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/line_mapping.py
--rw-r--r--   0 lisroach   (501) staff       (20)     2197 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/pseudo_rule.py
--rw-r--r--   0 lisroach   (501) staff       (20)     4099 2021-06-01 22:49:29.000000 fixit-0.1.4/fixit/common/report.py
--rw-r--r--   0 lisroach   (501) staff       (20)     9989 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/testing.py
-drwxr-xr-x   0 lisroach   (501) staff       (20)        0 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit/common/tests/
--rw-r--r--   0 lisroach   (501) staff       (20)      177 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/tests/__init__.py
-drwxr-xr-x   0 lisroach   (501) staff       (20)        0 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit/common/tests/dummy_package/
--rw-r--r--   0 lisroach   (501) staff       (20)      177 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/tests/dummy_package/__init__.py
--rw-r--r--   0 lisroach   (501) staff       (20)      309 2021-07-30 20:13:49.000000 fixit-0.1.4/fixit/common/tests/dummy_package/dummy_1.py
--rw-r--r--   0 lisroach   (501) staff       (20)      262 2021-04-30 00:00:22.000000 fixit-0.1.4/fixit/common/tests/dummy_package/dummy_2.py
-drwxr-xr-x   0 lisroach   (501) staff       (20)        0 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit/common/tests/dummy_package/dummy_subpackage/
--rw-r--r--   0 lisroach   (501) staff       (20)      177 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/tests/dummy_package/dummy_subpackage/__init__.py
--rw-r--r--   0 lisroach   (501) staff       (20)      436 2021-07-30 20:13:49.000000 fixit-0.1.4/fixit/common/tests/dummy_package/dummy_subpackage/dummy.py
--rw-r--r--   0 lisroach   (501) staff       (20)     5804 2021-04-22 22:01:07.000000 fixit-0.1.4/fixit/common/tests/test_autofix.py
--rw-r--r--   0 lisroach   (501) staff       (20)     1457 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/tests/test_comments.py
--rw-r--r--   0 lisroach   (501) staff       (20)     2321 2021-07-30 20:13:49.000000 fixit-0.1.4/fixit/common/tests/test_config.py
--rw-r--r--   0 lisroach   (501) staff       (20)     2018 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/tests/test_flake8_compat.py
--rw-r--r--   0 lisroach   (501) staff       (20)     3931 2021-05-26 21:43:53.000000 fixit-0.1.4/fixit/common/tests/test_full_repo_metadata.py
--rw-r--r--   0 lisroach   (501) staff       (20)      639 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/tests/test_get_code.py
--rw-r--r--   0 lisroach   (501) staff       (20)    14026 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/tests/test_ignores.py
--rw-r--r--   0 lisroach   (501) staff       (20)     5592 2021-07-30 20:13:49.000000 fixit-0.1.4/fixit/common/tests/test_imports.py
--rw-r--r--   0 lisroach   (501) staff       (20)    14793 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/tests/test_insert_suppressions.py
--rw-r--r--   0 lisroach   (501) staff       (20)     4037 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/tests/test_line_mapping.py
--rw-r--r--   0 lisroach   (501) staff       (20)     2546 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/tests/test_pseudo_rule.py
--rw-r--r--   0 lisroach   (501) staff       (20)     1455 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/tests/test_report.py
--rw-r--r--   0 lisroach   (501) staff       (20)    17947 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/common/tests/test_unused_suppressions.py
--rw-r--r--   0 lisroach   (501) staff       (20)    11378 2021-06-01 22:49:29.000000 fixit-0.1.4/fixit/common/unused_suppressions.py
--rw-r--r--   0 lisroach   (501) staff       (20)     6673 2021-07-30 20:13:49.000000 fixit-0.1.4/fixit/common/utils.py
--rw-r--r--   0 lisroach   (501) staff       (20)        0 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/py.typed
--rw-r--r--   0 lisroach   (501) staff       (20)     8109 2021-07-30 20:13:43.000000 fixit-0.1.4/fixit/rule_lint_engine.py
-drwxr-xr-x   0 lisroach   (501) staff       (20)        0 2021-07-30 20:15:52.000000 fixit-0.1.4/fixit/rules/
--rw-r--r--   0 lisroach   (501) staff       (20)      177 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/__init__.py
--rw-r--r--   0 lisroach   (501) staff       (20)     5335 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/add_file_header.py
--rw-r--r--   0 lisroach   (501) staff       (20)     2996 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/avoid_or_in_except.py
--rw-r--r--   0 lisroach   (501) staff       (20)    14878 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/await_async_call.py
--rw-r--r--   0 lisroach   (501) staff       (20)     6436 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/chained_instance_check.py
--rw-r--r--   0 lisroach   (501) staff       (20)     9167 2021-06-02 20:31:21.000000 fixit-0.1.4/fixit/rules/cls_in_classmethod.py
--rw-r--r--   0 lisroach   (501) staff       (20)     3522 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/compare_primitives_by_equal.py
--rw-r--r--   0 lisroach   (501) staff       (20)     4280 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/compare_singleton_primitives_by_is.py
--rw-r--r--   0 lisroach   (501) staff       (20)     8073 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/explicit_frozen_dataclass.py
--rw-r--r--   0 lisroach   (501) staff       (20)     1415 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/flake8_compat.py
--rw-r--r--   0 lisroach   (501) staff       (20)     2372 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/gather_sequential_await.py
--rw-r--r--   0 lisroach   (501) staff       (20)    20975 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/import_constraints.py
--rw-r--r--   0 lisroach   (501) staff       (20)     1415 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/no_assert_equals.py
--rw-r--r--   0 lisroach   (501) staff       (20)     4336 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/no_assert_true_for_comparison.py
--rw-r--r--   0 lisroach   (501) staff       (20)     3929 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/no_implicit_concat.py
--rw-r--r--   0 lisroach   (501) staff       (20)     1856 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/no_inherit_from_object.py
--rw-r--r--   0 lisroach   (501) staff       (20)     5776 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/no_namedtuple.py
--rw-r--r--   0 lisroach   (501) staff       (20)     4467 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/no_redundant_arguments_super.py
--rw-r--r--   0 lisroach   (501) staff       (20)     2090 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/no_redundant_fstring.py
--rw-r--r--   0 lisroach   (501) staff       (20)     2686 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/no_redundant_lambda.py
--rw-r--r--   0 lisroach   (501) staff       (20)     2311 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/no_redundant_list_comprehension.py
--rw-r--r--   0 lisroach   (501) staff       (20)     4197 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/no_static_if_condition.py
--rw-r--r--   0 lisroach   (501) staff       (20)     8221 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/no_string_type_annotation.py
--rw-r--r--   0 lisroach   (501) staff       (20)     4276 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/replace_union_with_optional.py
--rw-r--r--   0 lisroach   (501) staff       (20)     5667 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/rewrite_to_comprehension.py
--rw-r--r--   0 lisroach   (501) staff       (20)     5484 2021-03-31 19:22:11.000000 fixit-0.1.4/fixit/rules/rewrite_to_literal.py
--rw-r--r--   0 lisroach   (501) staff       (20)     3522 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/sorted_attributes_rule.py
--rw-r--r--   0 lisroach   (501) staff       (20)     6344 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/use_assert_in.py
--rw-r--r--   0 lisroach   (501) staff       (20)     5696 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/use_assert_is_not_none.py
--rw-r--r--   0 lisroach   (501) staff       (20)     3739 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/use_classname_as_code.py
--rw-r--r--   0 lisroach   (501) staff       (20)     8864 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/use_fstring.py
--rw-r--r--   0 lisroach   (501) staff       (20)     9038 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/use_is_none_on_optional.py
--rw-r--r--   0 lisroach   (501) staff       (20)     1875 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/rules/use_lint_fixme_comment.py
--rw-r--r--   0 lisroach   (501) staff       (20)     4438 2021-06-01 22:49:29.000000 fixit-0.1.4/fixit/rules/use_types_from_typing.py
-drwxr-xr-x   0 lisroach   (501) staff       (20)        0 2021-07-30 20:15:52.000000 fixit-0.1.4/fixit/tests/
--rw-r--r--   0 lisroach   (501) staff       (20)      641 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/tests/__init__.py
--rw-r--r--   0 lisroach   (501) staff       (20)     2161 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/tests/test_import_constraints.py
--rw-r--r--   0 lisroach   (501) staff       (20)     5542 2021-03-10 21:32:00.000000 fixit-0.1.4/fixit/tests/test_rule_lint_engine.py
-drwxr-xr-x   0 lisroach   (501) staff       (20)        0 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit.egg-info/
--rw-r--r--   0 lisroach   (501) staff       (20)     5735 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit.egg-info/PKG-INFO
--rw-r--r--   0 lisroach   (501) staff       (20)     3570 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit.egg-info/SOURCES.txt
--rw-r--r--   0 lisroach   (501) staff       (20)        1 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit.egg-info/dependency_links.txt
--rw-r--r--   0 lisroach   (501) staff       (20)       47 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit.egg-info/entry_points.txt
--rw-r--r--   0 lisroach   (501) staff       (20)        1 2021-03-10 22:31:14.000000 fixit-0.1.4/fixit.egg-info/not-zip-safe
--rw-r--r--   0 lisroach   (501) staff       (20)      280 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit.egg-info/requires.txt
--rw-r--r--   0 lisroach   (501) staff       (20)        6 2021-07-30 20:15:51.000000 fixit-0.1.4/fixit.egg-info/top_level.txt
--rw-r--r--   0 lisroach   (501) staff       (20)      252 2021-03-10 21:32:00.000000 fixit-0.1.4/requirements-dev.txt
--rw-r--r--   0 lisroach   (501) staff       (20)       86 2021-07-30 20:13:49.000000 fixit-0.1.4/requirements.txt
--rw-r--r--   0 lisroach   (501) staff       (20)       38 2021-07-30 20:15:52.000000 fixit-0.1.4/setup.cfg
--rw-r--r--   0 lisroach   (501) staff       (20)     2265 2021-03-10 21:32:00.000000 fixit-0.1.4/setup.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.editorconfig
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.flake8
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.mailmap
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.pyre_configuration
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.readthedocs.yml
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.watchmanconfig
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 fixit-2.0.0a1/CHANGELOG.md
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 fixit-2.0.0a1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 fixit-2.0.0a1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 fixit-2.0.0a1/makefile
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/api.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/changelog.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/code-of-conduct.rst
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/conf.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/contributing.rst
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/guide.rst
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/index.rst
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/proposals.rst
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/why.rst
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/custom.css
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/fbopensource.png
+-rw-r--r--   0        0        0    21530 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/opensource.png
+-rw-r--r--   0        0        0    22163 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/icon.png
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/icon.svg
+-rw-r--r--   0        0        0    21638 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/icon_whilte.png
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/icon_white.svg
+-rw-r--r--   0        0        0    37225 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/logo.png
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/logo.svg
+-rw-r--r--   0        0        0    36486 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/logo_whilte.png
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_static/logo/logo_white.svg
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_templates/badges.html
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/_templates/meta.html
+-rw-r--r--   0        0        0    30722 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/guide/builtins.rst
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/guide/commands.rst
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/guide/configuration.rst
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/guide/integrations.rst
+-rw-r--r--   0        0        0     5184 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/guide/quickstart.rst
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/proposals/fp1.md
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 fixit-2.0.0a1/docs/proposals/fp2.rst
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 fixit-2.0.0a1/scripts/check_copyright.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 fixit-2.0.0a1/scripts/document_rules.py
+-rwxr-xr-x   0        0        0     3360 2020-02-02 00:00:00.000000 fixit-2.0.0a1/scripts/migrate_rule_to_fixit2.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/__main__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/__version__.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/api.py
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/cli.py
+-rw-r--r--   0        0        0    13174 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/config.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/engine.py
+-rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/ftypes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/py.typed
+-rw-r--r--   0        0        0     4386 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rule.py
+-rw-r--r--   0        0        0    10073 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/testing.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/util.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/local/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/__init__.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/avoid_or_in_except.py
+-rw-r--r--   0        0        0     6429 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/chained_instance_check.py
+-rw-r--r--   0        0        0     9284 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/cls_in_classmethod.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/compare_primitives_by_equal.py
+-rw-r--r--   0        0        0     4282 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/compare_singleton_primitives_by_is.py
+-rw-r--r--   0        0        0     8867 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/explicit_frozen_dataclass.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_assert_equals.py
+-rw-r--r--   0        0        0     4338 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_assert_true_for_comparison.py
+-rw-r--r--   0        0        0     1982 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_inherit_from_object.py
+-rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_namedtuple.py
+-rw-r--r--   0        0        0     4436 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_redundant_arguments_super.py
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_redundant_fstring.py
+-rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_redundant_lambda.py
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_redundant_list_comprehension.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_static_if_condition.py
+-rw-r--r--   0        0        0     8563 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/no_string_type_annotation.py
+-rw-r--r--   0        0        0     4157 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/replace_union_with_optional.py
+-rw-r--r--   0        0        0     5817 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/rewrite_to_comprehension.py
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/rewrite_to_literal.py
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/sorted_attributes_rule.py
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/use_assert_in.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/use_assert_is_not_none.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/use_classname_as_code.py
+-rw-r--r--   0        0        0     9303 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/use_fstring.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/use_lint_fixme_comment.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/rules/use_types_from_typing.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/tests/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/tests/__main__.py
+-rw-r--r--   0        0        0    13344 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/tests/config.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/tests/ftypes.py
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/tests/rule.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 fixit-2.0.0a1/src/fixit/tests/smoke.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 fixit-2.0.0a1/.gitignore
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 fixit-2.0.0a1/LICENSE
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 fixit-2.0.0a1/README.rst
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 fixit-2.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     7747 2020-02-02 00:00:00.000000 fixit-2.0.0a1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fixit-0.1.4/LICENSE` & `fixit-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `fixit-0.1.4/fixit/common/testing.py` & `fixit-2.0.0a1/src/fixit/testing.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,53 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+import re
+import textwrap
 import unittest
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Callable, Dict, Mapping, Optional, Sequence, Type, Union, cast
+from typing import (
+    Any,
+    Callable,
+    Collection,
+    Dict,
+    List,
+    Mapping,
+    Optional,
+    Sequence,
+    Type,
+    Union,
+)
 
-from libcst.metadata import MetadataWrapper
+from moreorless import unified_diff
 
-from fixit.common.base import CstLintRule
-from fixit.common.generate_pyre_fixtures import get_fixture_path
-from fixit.common.report import BaseLintRuleReport
-from fixit.common.utils import (
-    InvalidTestCase,
-    LintRuleCollectionT,
-    ValidTestCase,
-    _dedent,
-    gen_type_inference_wrapper,
-)
-from fixit.rule_lint_engine import lint_file
+from .engine import LintRunner
+from .ftypes import Config
+from .rule import InvalidTestCase, LintRule, ValidTestCase
+
+
+def _dedent(src: str) -> str:
+    src = re.sub(r"\A\n", "", src)
+    return textwrap.dedent(src)
+
+
+def get_fixture_path(
+    fixture_top_dir: Path, rule_module: str, rules_package: str
+) -> Path:
+    subpackage: str = rule_module.split(f"{rules_package}.", 1)[-1]
+    fixture_subdir = subpackage.replace(".", "/")
+    return fixture_top_dir / fixture_subdir
 
 
-def validate_patch(report: BaseLintRuleReport, test_case: InvalidTestCase) -> None:
+def validate_patch(report: Any, test_case: InvalidTestCase) -> None:
     patch = report.patch
-    expected_replacement = test_case.expected_replacement
+    expected_replacement = test_case.expected_replacement  # type: ignore
 
     if patch is None:
         if expected_replacement is not None:
             raise AssertionError(
                 "The rule for this test case has no auto-fix, but expected source was specified."
             )
         return
@@ -47,190 +65,195 @@
             + f"Expected:\n{expected_replacement}\n"
             + f"But found:\n{patched_code}"
         )
 
 
 @dataclass(frozen=True)
 class TestCasePrecursor:
-    rule: Type[CstLintRule]
+    rule: LintRule
     test_methods: Mapping[
         str,
         Union[ValidTestCase, InvalidTestCase],
     ]
     fixture_paths: Mapping[str, Path]
 
 
 class LintRuleTestCase(unittest.TestCase):
     def _test_method(
         self,
         test_case: Union[ValidTestCase, InvalidTestCase],
-        rule: Type[CstLintRule],
-        fixture_file: Optional[Path] = None,
+        rule: LintRule,
     ) -> None:
-        cst_wrapper: Optional[MetadataWrapper] = None
-        if fixture_file is not None:
-            cst_wrapper = gen_type_inference_wrapper(test_case.code, fixture_file)
-        reports = lint_file(
-            Path(test_case.filename),
-            _dedent(test_case.code).encode("utf-8"),
-            config=test_case.config,
-            rules={rule},
-            cst_wrapper=cst_wrapper,
+        config = Config()
+        path = Path(
+            "valid.py" if isinstance(test_case, ValidTestCase) else "invalid.py"
         )
+        source_code = _dedent(test_case.code)
+        runner = LintRunner(path, source_code.encode())
+        reports = list(runner.collect_violations([rule], config))
+
         if isinstance(test_case, ValidTestCase):
             self.assertEqual(
                 len(reports),
                 0,
                 'Expected zero reports for this "valid" test case. Instead, found:\n'
                 + "\n".join(str(e) for e in reports),
             )
-        else:
-            self.assertGreater(
-                len(reports),
-                0,
-                'Expected a report for this "invalid" test case but `self.report` was '
-                + "not called:\n"
-                + test_case.code,
-            )
-            self.assertLessEqual(
-                len(reports),
-                1,
-                'Expected one report from this "invalid" test case. Found multiple:\n'
-                + "\n".join(str(e) for e in reports),
-            )
+            return
+
+        self.assertGreater(
+            len(reports),
+            0,
+            'Expected a report for this "invalid" test case but `self.report` was '
+            + "not called:\n"
+            + test_case.code,
+        )
+        self.assertLessEqual(
+            len(reports),
+            1,
+            'Expected one report from this "invalid" test case. Found multiple:\n'
+            + "\n".join(str(e) for e in reports),
+        )
 
-            # pyre-fixme[16]: `Collection` has no attribute `__getitem__`.
-            report = reports[0]
+        report = reports[0]
 
-            if not (test_case.line is None or test_case.line == report.line):
-                raise AssertionError(
-                    f"Expected line: {test_case.line} but found line: {report.line}"
-                )
-
-            if not (test_case.column is None or test_case.column == report.column):
-                raise AssertionError(
-                    f"Expected column: {test_case.column} but found column: {report.column}"
-                )
-            kind = test_case.kind if test_case.kind is not None else rule.__name__
-            if kind != report.code:
-                raise AssertionError(
-                    f"Expected:\n    {test_case.expected_str}\nBut found:\n    {report}"
-                )
-            if (
-                test_case.expected_message is not None
-                and test_case.expected_message != report.message
-            ):
-                raise AssertionError(
-                    f"Expected message:\n    {test_case.expected_message}\nBut got:\n    {report.message}"
-                )
+        if test_case.range is not None:
+            self.assertEqual(test_case.range, report.range)
 
-            validate_patch(report, test_case)
+        if test_case.expected_message is not None:
+            self.assertEqual(test_case.expected_message, report.message)
+
+        if test_case.expected_replacement:
+            # make sure we produced expected final code
+            expected_code = _dedent(test_case.expected_replacement)
+            modified_code = runner.apply_replacements([report]).decode()
+            self.assertMultiLineEqual(expected_code, modified_code)
+
+            # make sure we generated a reasonable diff
+            expected_diff = unified_diff(
+                source_code, expected_code, filename=path.name, n=1
+            )
+            self.assertEqual(expected_diff, report.diff)
 
 
 def _gen_test_methods_for_rule(
-    rule: Type[CstLintRule], fixture_dir: Path, rules_package: str
+    rule: LintRule, fixture_dir: Path, rules_package: str
 ) -> TestCasePrecursor:
-    """Aggregates all of the cases inside a single CstLintRule's VALID and INVALID attributes
-    and maps them to altered names with a `test_` prefix so that 'unittest' can discover them
-    later on and an index postfix so that individual tests can be selected from the command line.
+    """
+    Aggregates all of the cases inside a single LintRule's VALID and INVALID
+    attributes and maps them to altered names with a `test_` prefix so that 'unittest'
+    can discover them later on and an index postfix so that individual tests can be
+    selected from the command line.
     """
     valid_tcs = {}
     invalid_tcs = {}
-    requires_fixtures = False
     fixture_paths: Dict[str, Path] = {}
-    fixture_subdir: Path = get_fixture_path(fixture_dir, rule.__module__, rules_package)
-    if issubclass(rule, CstLintRule):
+    for idx, test_case_or_str in enumerate(rule.VALID):
+        name = f"test_VALID_{idx}"
+        valid_test_case = (
+            ValidTestCase(code=test_case_or_str)
+            if isinstance(test_case_or_str, str)
+            else test_case_or_str
+        )
+        valid_tcs[name] = valid_test_case
+    for idx, inv_test_case_or_str in enumerate(rule.INVALID):
+        name = f"test_INVALID_{idx}"
+        invalid_test_case = (
+            InvalidTestCase(code=inv_test_case_or_str)
+            if isinstance(inv_test_case_or_str, str)
+            else inv_test_case_or_str
+        )
+        invalid_tcs[name] = invalid_test_case
 
-        if rule.requires_metadata_caches():
-            requires_fixtures = True
-        if hasattr(rule, "VALID"):
-            for idx, test_case in enumerate(getattr(rule, "VALID")):
-                name = f"test_VALID_{idx}"
-                valid_tcs[name] = test_case
-                if requires_fixtures:
-                    fixture_paths[name] = (
-                        fixture_subdir / f"{rule.__name__}_VALID_{idx}.json"
-                    )
-        if hasattr(rule, "INVALID"):
-            for idx, test_case in enumerate(getattr(rule, "INVALID")):
-                name = f"test_INVALID_{idx}"
-                invalid_tcs[name] = test_case
-                if requires_fixtures:
-                    fixture_paths[name] = (
-                        fixture_subdir / f"{rule.__name__}_INVALID_{idx}.json"
-                    )
     return TestCasePrecursor(
         rule=rule,
         test_methods={**valid_tcs, **invalid_tcs},
         fixture_paths=fixture_paths,
     )
 
 
 def _gen_all_test_methods(
-    rules: LintRuleCollectionT, fixture_dir: Path, rules_package: str
+    rules: Collection[LintRule], fixture_dir: Path, rules_package: str
 ) -> Sequence[TestCasePrecursor]:
     """
     Converts all passed-in lint rules to type `TestCasePrecursor` to ease further TestCase
     creation later on.
     """
     cases = []
     for rule in rules:
-        if not issubclass(rule, CstLintRule):
+        if not isinstance(rule, LintRule):
             continue
         test_cases_for_rule = _gen_test_methods_for_rule(
-            cast(Type[CstLintRule], rule), fixture_dir, rules_package
+            rule, fixture_dir, rules_package
         )
         cases.append(test_cases_for_rule)
     return cases
 
 
 def add_lint_rule_tests_to_module(
     module_attrs: Dict[str, Any],
-    rules: LintRuleCollectionT,
+    rules: Collection[LintRule],
     test_case_type: Type[unittest.TestCase] = LintRuleTestCase,
     custom_test_method_name: str = "_test_method",
-    fixture_dir: Path = Path(""),
+    fixture_dir: Optional[Path] = None,
     rules_package: str = "",
 ) -> None:
     """
     Generates classes inheriting from `unittest.TestCase` from the data available in `rules` and adds these to module_attrs.
     The goal is to facilitate unit test discovery by Python's `unittest` framework. This will provide the capability of
     testing your lint rules by running commands such as `python -m unittest <your testing module name>`.
 
     module_attrs: A dictionary of attributes we want to add these test cases to. If adding to a module, you can pass `globals()` as the argument.
 
-    rules: A collection of classes extending `CstLintRule` to be converted to test cases.
+    rules: A collection of classes extending `LintRule` to be converted to test cases.
 
     test_case_type: A class extending Python's `unittest.TestCase` that implements a custom test method for testing lint rules to serve as a stencil for test cases.
     New classes will be generated, and named after each lint rule. They will inherit directly from the class passed into `test_case_type`.
     If argument is omitted, will default to the `LintRuleTestCase` class from fixit.common.testing.
 
     custom_test_method_name: A member method of the class passed into `test_case_type` parameter that contains the logic around asserting success or failure of
-    CstLintRule's `ValidTestCase` and `InvalidTestCase` test cases. The method will be dynamically renamed to `test_<VALID/INVALID>_<test case index>` for discovery
+    LintRule's `ValidTestCase` and `InvalidTestCase` test cases. The method will be dynamically renamed to `test_<VALID/INVALID>_<test case index>` for discovery
     by unittest. If argument is omitted, `add_lint_rule_tests_to_module` will look for a test method named `_test_method` member of `test_case_type`.
 
     fixture_dir: The directory in which fixture files for the passed rules live. Necessary only if any lint rules require fixture data for testing.
 
     rules_package: The name of the rules package. This will be used during the search for fixture files and provides insight into the structure of the fixture directory.
     The structure of the fixture directory is automatically assumed to mirror the structure of the rules package, eg: `<rules_package>.submodule.module.rule_class` should
     have fixture files in `<fixture_dir>/submodule/module/rule_class/`.
     """
+    if fixture_dir is not None or rules_package:
+        raise NotImplementedError("fixtures are not implemented in tests yet")
+    if fixture_dir is None:
+        fixture_dir = Path("")
+    test_case_classes: List[Type[unittest.TestCase]] = []
     for test_case in _gen_all_test_methods(rules, fixture_dir, rules_package):
-        rule_name = test_case.rule.__name__
+        rule_name = type(test_case.rule).__name__
         test_methods_to_add: Dict[str, Callable] = {}
 
         for test_method_name, test_method_data in test_case.test_methods.items():
             fixture_file = test_case.fixture_paths.get(test_method_name)
 
             def test_method(
                 self: Type[unittest.TestCase],
                 data: Union[ValidTestCase, InvalidTestCase] = test_method_data,
-                rule: Type[CstLintRule] = test_case.rule,
-                fixture_file: Optional[str] = fixture_file,
+                rule: LintRule = test_case.rule,
+                fixture_file: Optional[Path] = fixture_file,
             ) -> None:
-                return getattr(self, custom_test_method_name)(data, rule, fixture_file)
+                # instantiate a new rule for every test
+                rule_ty = type(rule)
+                return getattr(self, custom_test_method_name)(data, rule_ty())
 
             test_method.__name__ = test_method_name
             test_methods_to_add[test_method_name] = test_method
 
         test_case_class = type(rule_name, (test_case_type,), test_methods_to_add)
+        test_case_classes.append(test_case_class)
         module_attrs[rule_name] = test_case_class
+
+    # Rewrite the module for each generated test case to match the location calling
+    # this function. This enables better integration with test case discovery methods
+    # that depend on listing test cases separately from running them.
+    if "__package__" in module_attrs:
+        test_module = module_attrs.get("__package__")
+        assert isinstance(test_module, str)
+        for test_case_class in test_case_classes:
+            test_case_class.__module__ = test_module
```

### Comparing `fixit-0.1.4/fixit/rules/avoid_or_in_except.py` & `fixit-2.0.0a1/src/fixit/rules/avoid_or_in_except.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import libcst as cst
 import libcst.matchers as m
```

### Comparing `fixit-0.1.4/fixit/rules/chained_instance_check.py` & `fixit-2.0.0a1/src/fixit/rules/chained_instance_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Dict, Iterator, List, Set, Tuple
 
 import libcst as cst
 import libcst.matchers as m
 from libcst.metadata import QualifiedName, QualifiedNameProvider, QualifiedNameSource
 
-from fixit import (
-    CstContext,
-    CstLintRule,
-    InvalidTestCase as Invalid,
-    ValidTestCase as Valid,
-)
+from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
 
 
 _ISINSTANCE = QualifiedName(
     name="builtins.isinstance", source=QualifiedNameSource.BUILTIN
 )
 
 
@@ -94,16 +89,16 @@
             expected_replacement=(
                 "isinstance(x, (a, b)) or isinstance(y, (c, d)) or isinstance(z, e)"
                 + " or isinstance(q, (f, g, h))"
             ),
         ),
     ]
 
-    def __init__(self, context: CstContext) -> None:
-        super().__init__(context)
+    def __init__(self) -> None:
+        super().__init__()
         self.seen_boolean_operations: Set[cst.BooleanOperation] = set()
 
     def visit_BooleanOperation(self, node: cst.BooleanOperation) -> None:
         if node in self.seen_boolean_operations:
             return None
 
         stack = tuple(self.unwrap(node))
@@ -143,15 +138,15 @@
             yield node
 
     def collect_targets(
         self, stack: Tuple[cst.BaseExpression, ...]
     ) -> Tuple[
         List[cst.BaseExpression], Dict[cst.BaseExpression, List[cst.BaseExpression]]
     ]:
-        targets = {}
+        targets: Dict[cst.BaseExpression, List[cst.BaseExpression]] = {}
         operands = []
 
         for operand in stack:
             if m.matches(
                 operand, m.Call(func=m.DoNotCare(), args=[m.Arg(), m.Arg(~m.Tuple())])
             ):
                 call = cst.ensure_type(operand, cst.Call)
```

### Comparing `fixit-0.1.4/fixit/rules/cls_in_classmethod.py` & `fixit-2.0.0a1/src/fixit/rules/cls_in_classmethod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import List, Union
 
 import libcst as cst
@@ -228,14 +228,18 @@
                 QualifiedName(
                     name="builtins.classmethod", source=QualifiedNameSource.BUILTIN
                 ),
             )
             for decorator in node.decorators
         ):
             return  # If it's not a @classmethod, we are not interested.
+
+        repl: Union[
+            cst.CSTNode, cst.RemovalSentinel, cst.FlattenSentinel[cst.FunctionDef]
+        ]
         if not node.params.params:
             # No params, but there must be the 'cls' param.
             # Note that pyre[47] already catches this, but we also generate
             # an autofix, so it still makes sense for us to report it here.
             new_params = node.params.with_changes(
                 params=(cst.Param(name=cst.Name(value=CLS)),)
             )
```

### Comparing `fixit-0.1.4/fixit/rules/compare_primitives_by_equal.py` & `fixit-2.0.0a1/src/fixit/rules/compare_primitives_by_equal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import libcst as cst
 
 from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
```

### Comparing `fixit-0.1.4/fixit/rules/compare_singleton_primitives_by_is.py` & `fixit-2.0.0a1/src/fixit/rules/compare_singleton_primitives_by_is.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import FrozenSet, Union
 
 import libcst as cst
```

### Comparing `fixit-0.1.4/fixit/rules/explicit_frozen_dataclass.py` & `fixit-2.0.0a1/src/fixit/rules/explicit_frozen_dataclass.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,24 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import libcst as cst
 import libcst.matchers as m
 from libcst._nodes.whitespace import SimpleWhitespace
 from libcst.metadata import QualifiedName, QualifiedNameProvider, QualifiedNameSource
 
-from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
+from fixit import (
+    CodePosition,
+    CodeRange,
+    CstLintRule,
+    InvalidTestCase as Invalid,
+    ValidTestCase as Valid,
+)
 
 
 class ExplicitFrozenDataclassRule(CstLintRule):
     """
     Encourages the use of frozen dataclass objects by telling users to specify the
     kwarg.
 
@@ -67,165 +73,165 @@
             """
             from dataclasses import dataclass
             @some_unrelated_decorator
             @dataclass  # not called as a function
             @another_unrelated_decorator
             class Cls: pass
             """,
-            line=3,
             expected_replacement="""
             from dataclasses import dataclass
             @some_unrelated_decorator
             @dataclass(frozen=True)  # not called as a function
             @another_unrelated_decorator
             class Cls: pass
             """,
+            range=CodeRange(start=CodePosition(3, 0), end=CodePosition(3, 10)),
         ),
         Invalid(
             """
             from dataclasses import dataclass
             @dataclass()  # called as a function, no kwargs
             class Cls: pass
             """,
-            line=2,
             expected_replacement="""
             from dataclasses import dataclass
             @dataclass(frozen=True)  # called as a function, no kwargs
             class Cls: pass
             """,
+            range=CodeRange(start=CodePosition(2, 0), end=CodePosition(2, 12)),
         ),
         Invalid(
             """
             from dataclasses import dataclass
             @dataclass(other_kwarg=False)
             class Cls: pass
             """,
-            line=2,
             expected_replacement="""
             from dataclasses import dataclass
             @dataclass(other_kwarg=False, frozen=True)
             class Cls: pass
             """,
+            range=CodeRange(start=CodePosition(2, 0), end=CodePosition(2, 29)),
         ),
         Invalid(
             """
             import dataclasses
             @dataclasses.dataclass
             class Cls: pass
             """,
-            line=2,
             expected_replacement="""
             import dataclasses
             @dataclasses.dataclass(frozen=True)
             class Cls: pass
             """,
+            range=CodeRange(start=CodePosition(2, 0), end=CodePosition(2, 22)),
         ),
         Invalid(
             """
             import dataclasses
             @dataclasses.dataclass()
             class Cls: pass
             """,
-            line=2,
             expected_replacement="""
             import dataclasses
             @dataclasses.dataclass(frozen=True)
             class Cls: pass
             """,
+            range=CodeRange(start=CodePosition(2, 0), end=CodePosition(2, 24)),
         ),
         Invalid(
             """
             import dataclasses
             @dataclasses.dataclass(other_kwarg=False)
             class Cls: pass
             """,
-            line=2,
             expected_replacement="""
             import dataclasses
             @dataclasses.dataclass(other_kwarg=False, frozen=True)
             class Cls: pass
             """,
+            range=CodeRange(start=CodePosition(2, 0), end=CodePosition(2, 41)),
         ),
         Invalid(
             """
             from dataclasses import dataclass as dc
             @dc
             class Cls: pass
             """,
-            line=2,
             expected_replacement="""
             from dataclasses import dataclass as dc
             @dc(frozen=True)
             class Cls: pass
             """,
+            range=CodeRange(start=CodePosition(2, 0), end=CodePosition(2, 3)),
         ),
         Invalid(
             """
             from dataclasses import dataclass as dc
             @dc()
             class Cls: pass
             """,
-            line=2,
             expected_replacement="""
             from dataclasses import dataclass as dc
             @dc(frozen=True)
             class Cls: pass
             """,
+            range=CodeRange(start=CodePosition(2, 0), end=CodePosition(2, 5)),
         ),
         Invalid(
             """
             from dataclasses import dataclass as dc
             @dc(other_kwarg=False)
             class Cls: pass
             """,
-            line=2,
             expected_replacement="""
             from dataclasses import dataclass as dc
             @dc(other_kwarg=False, frozen=True)
             class Cls: pass
             """,
+            range=CodeRange(start=CodePosition(2, 0), end=CodePosition(2, 22)),
         ),
         Invalid(
             """
             import dataclasses as dc
             @dc.dataclass
             class Cls: pass
             """,
-            line=2,
             expected_replacement="""
             import dataclasses as dc
             @dc.dataclass(frozen=True)
             class Cls: pass
             """,
+            range=CodeRange(start=CodePosition(2, 0), end=CodePosition(2, 13)),
         ),
         Invalid(
             """
             import dataclasses as dc
             @dc.dataclass()
             class Cls: pass
             """,
-            line=2,
             expected_replacement="""
             import dataclasses as dc
             @dc.dataclass(frozen=True)
             class Cls: pass
             """,
+            range=CodeRange(start=CodePosition(2, 0), end=CodePosition(2, 15)),
         ),
         Invalid(
             """
             import dataclasses as dc
             @dc.dataclass(other_kwarg=False)
             class Cls: pass
             """,
-            line=2,
             expected_replacement="""
             import dataclasses as dc
             @dc.dataclass(other_kwarg=False, frozen=True)
             class Cls: pass
             """,
+            range=CodeRange(start=CodePosition(2, 0), end=CodePosition(2, 32)),
         ),
     ]
 
     def visit_ClassDef(self, node: cst.ClassDef) -> None:
         for d in node.decorators:
             decorator = d.decorator
             if QualifiedNameProvider.has_name(
@@ -238,16 +244,18 @@
                 if isinstance(decorator, cst.Call):
                     func = decorator.func
                     args = decorator.args
                 else:  # decorator is either cst.Name or cst.Attribute
                     args = ()
                     func = decorator
 
-                # pyre-fixme[29]: `typing.Union[typing.Callable(tuple.__iter__)[[], typing.Iterator[Variable[_T_co](covariant)]], typing.Callable(typing.Sequence.__iter__)[[], typing.Iterator[cst._nodes.expression.Arg]]]` is not a function.
-                if not any(m.matches(arg.keyword, m.Name("frozen")) for arg in args):
+                # pyre-fixme[6]: Expected `Union[cst._maybe_sentinel.MaybeSentinel,
+                #  cst._nodes.base.CSTNode, cst._removal_sentinel.RemovalSentinel]` for
+                #  1st param but got `Optional[cst._nodes.expression.Name]`.
+                if not any(m.matches(arg.keyword, m.Name("frozen")) for arg in args):  # type: ignore
                     new_decorator = cst.Call(
                         func=func,
                         args=list(args)
                         + [
                             cst.Arg(
                                 keyword=cst.Name("frozen"),
                                 value=cst.Name("True"),
```

### Comparing `fixit-0.1.4/fixit/rules/no_assert_equals.py` & `fixit-2.0.0a1/src/fixit/rules/no_assert_equals.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import libcst as cst
 import libcst.matchers as m
```

### Comparing `fixit-0.1.4/fixit/rules/no_assert_true_for_comparison.py` & `fixit-2.0.0a1/src/fixit/rules/no_assert_true_for_comparison.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Sequence
 
 import libcst as cst
```

### Comparing `fixit-0.1.4/fixit/rules/no_inherit_from_object.py` & `fixit-2.0.0a1/src/fixit/rules/no_inherit_from_object.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import libcst as cst
 import libcst.matchers as m
 
-from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
+from fixit import (
+    CodePosition,
+    CodeRange,
+    CstLintRule,
+    InvalidTestCase as Invalid,
+    ValidTestCase as Valid,
+)
 
 
 class NoInheritFromObjectRule(CstLintRule):
     """
     In Python 3, a class is inherited from ``object`` by default.
     Explicitly inheriting from ``object`` is redundant, so removing it keeps the code simpler.
     """
@@ -25,29 +31,27 @@
         ),
     ]
     INVALID = [
         Invalid(
             """
             class B(object):
                 pass""",
-            line=1,
-            column=1,
             expected_replacement="""
                 class B:
                     pass""",
+            range=CodeRange(start=CodePosition(1, 0), end=CodePosition(2, 8)),
         ),
         Invalid(
             """
             class B(object, A):
                 pass""",
-            line=1,
-            column=1,
             expected_replacement="""
                 class B(A):
                     pass""",
+            range=CodeRange(start=CodePosition(1, 0), end=CodePosition(2, 8)),
         ),
     ]
 
     def visit_ClassDef(self, node: cst.ClassDef) -> None:
         new_bases = tuple(
             base for base in node.bases if not m.matches(base.value, m.Name("object"))
         )
```

### Comparing `fixit-0.1.4/fixit/rules/no_namedtuple.py` & `fixit-2.0.0a1/src/fixit/rules/no_namedtuple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import List, Optional, Sequence, Tuple
 
 import libcst as cst
-from libcst import MaybeSentinel, ensure_type, parse_expression
+from libcst import ensure_type, MaybeSentinel, parse_expression
 from libcst.metadata import QualifiedName, QualifiedNameProvider, QualifiedNameSource
 
 from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
 
 
 class NoNamedTupleRule(CstLintRule):
     """
```

### Comparing `fixit-0.1.4/fixit/rules/no_redundant_arguments_super.py` & `fixit-2.0.0a1/src/fixit/rules/no_redundant_arguments_super.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import List, Union
 
 import libcst as cst
 import libcst.matchers as m
 
-from fixit import (
-    CstContext,
-    CstLintRule,
-    InvalidTestCase as Invalid,
-    ValidTestCase as Valid,
-)
+from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
 
 
 class NoRedundantArgumentsSuperRule(CstLintRule):
     """
     Remove redundant arguments when using super for readability.
     """
 
@@ -116,16 +111,16 @@
                     class InnerInnerFoo(Bar):
                         def foo(self, bar):
                             super().foo(bar)
             """,
         ),
     ]
 
-    def __init__(self, context: CstContext) -> None:
-        super().__init__(context)
+    def __init__(self) -> None:
+        super().__init__()
         self.current_classes: List[str] = []
 
     def visit_ClassDef(self, node: cst.ClassDef) -> None:
         self.current_classes.append(node.name.value)
 
     def leave_ClassDef(self, original_node: cst.ClassDef) -> None:
         self.current_classes.pop()
@@ -140,15 +135,15 @@
                     m.Arg(),
                 ],
             ),
         ):
             self.report(original_node, replacement=original_node.with_changes(args=()))
 
     def _build_arg_class_matcher(self) -> Union[m.Attribute, m.Name]:
-        matcher = m.Name(value=self.current_classes[0])
+        matcher: Union[m.Name, m.Attribute] = m.Name(value=self.current_classes[0])
 
         # For nested classes, we need to match attributes, so we can target
         # `super(Foo.InnerFoo, self)` for example.
         if len(self.current_classes) > 1:
             for class_name in self.current_classes[1:]:
                 matcher = m.Attribute(value=matcher, attr=m.Name(value=class_name))
```

### Comparing `fixit-0.1.4/fixit/rules/no_redundant_fstring.py` & `fixit-2.0.0a1/src/fixit/rules/no_redundant_fstring.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import libcst as cst
 import libcst.matchers as m
 
-from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
+from fixit import (
+    CodePosition,
+    CodeRange,
+    CstLintRule,
+    InvalidTestCase as Invalid,
+    ValidTestCase as Valid,
+)
 
 
 class NoRedundantFStringRule(CstLintRule):
     """
     Remove redundant f-string without placeholders.
     """
 
@@ -25,31 +31,31 @@
         Valid('good = "good" % ()'),
         Valid('good = rf"good\t+{bar}"'),
     ]
 
     INVALID = [
         Invalid(
             'bad: str = f"bad" + "bad"',
-            line=1,
             expected_replacement='bad: str = "bad" + "bad"',
+            range=CodeRange(start=CodePosition(1, 11), end=CodePosition(1, 17)),
         ),
         Invalid(
             "bad: str = f'bad'",
-            line=1,
             expected_replacement="bad: str = 'bad'",
+            range=CodeRange(start=CodePosition(1, 11), end=CodePosition(1, 17)),
         ),
         Invalid(
             "bad: str = rf'bad\t+'",
-            line=1,
             expected_replacement="bad: str = r'bad\t+'",
+            range=CodeRange(start=CodePosition(1, 11), end=CodePosition(1, 20)),
         ),
         Invalid(
             'bad: str = f"no args but messing up {{ braces }}"',
-            line=1,
             expected_replacement='bad: str = "no args but messing up { braces }"',
+            range=CodeRange(start=CodePosition(1, 11), end=CodePosition(1, 49)),
         ),
     ]
 
     def visit_FormattedString(self, node: cst.FormattedString) -> None:
         if not m.matches(node, m.FormattedString(parts=(m.FormattedStringText(),))):
             return
```

### Comparing `fixit-0.1.4/fixit/rules/no_redundant_lambda.py` & `fixit-2.0.0a1/src/fixit/rules/no_redundant_lambda.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import libcst as cst
 import libcst.matchers as m
 from libcst.helpers import get_full_name_for_node
 
 from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
 
 
 UNNECESSARY_LAMBDA: str = (
     "The lambda that is wrapping {function} is redundant. "
-    + "It can unwrapped safely and used purely."
+    "It can unwrapped safely and used purely."
 )
 
 
 class NoRedundantLambdaRule(CstLintRule):
-    """A lamba function which has a single objective of
+    """
+    A lamba function which has a single objective of
     passing all it is arguments to another callable can
-    be safely replaced by that callable."""
+    be safely replaced by that callable.
+    """
 
     VALID = [
         Valid("lambda x: foo(y)"),
         Valid("lambda x: foo(x, y)"),
         Valid("lambda x, y: foo(x)"),
         Valid("lambda *, x: foo(x)"),
         Valid("lambda x = y: foo(x)"),
```

### Comparing `fixit-0.1.4/fixit/rules/no_redundant_list_comprehension.py` & `fixit-2.0.0a1/src/fixit/rules/no_redundant_list_comprehension.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import libcst as cst
 import libcst.matchers as m
```

### Comparing `fixit-0.1.4/fixit/rules/no_static_if_condition.py` & `fixit-2.0.0a1/src/fixit/rules/no_static_if_condition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Optional
 
 import libcst as cst
```

### Comparing `fixit-0.1.4/fixit/rules/no_string_type_annotation.py` & `fixit-2.0.0a1/src/fixit/rules/no_string_type_annotation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Set
 
 import libcst as cst
 import libcst.matchers as m
 from libcst.metadata import QualifiedNameProvider
 
 from fixit import (
-    CstContext,
+    CodePosition,
+    CodeRange,
     CstLintRule,
     InvalidTestCase as Invalid,
     ValidTestCase as Valid,
 )
 
 
 class NoStringTypeAnnotationRule(CstLintRule):
@@ -98,154 +99,156 @@
             from __future__ import annotations
 
             from a.b import Class
 
             def foo() -> "Class":
                 return Class()
             """,
-            line=5,
             expected_replacement="""
             from __future__ import annotations
 
             from a.b import Class
 
             def foo() -> Class:
                 return Class()
             """,
+            range=CodeRange(start=CodePosition(5, 13), end=CodePosition(5, 20)),
         ),
         Invalid(
             """
             from __future__ import annotations
 
             from a.b import Class
 
             async def foo() -> "Class":
                 return await Class()
             """,
-            line=5,
             expected_replacement="""
             from __future__ import annotations
 
             from a.b import Class
 
             async def foo() -> Class:
                 return await Class()
             """,
+            range=CodeRange(start=CodePosition(5, 19), end=CodePosition(5, 26)),
         ),
         Invalid(
             """
             from __future__ import annotations
 
             import typing
             from a.b import Class
 
             def foo() -> typing.Type["Class"]:
                 return Class
             """,
-            line=6,
             expected_replacement="""
             from __future__ import annotations
 
             import typing
             from a.b import Class
 
             def foo() -> typing.Type[Class]:
                 return Class
             """,
+            range=CodeRange(start=CodePosition(6, 25), end=CodePosition(6, 32)),
         ),
         Invalid(
             """
             from __future__ import annotations
 
             import typing
             from a.b import Class
             from c import func
 
             def foo() -> Optional[typing.Type["Class"]]:
                 return Class if func() else None
             """,
-            line=7,
             expected_replacement="""
             from __future__ import annotations
 
             import typing
             from a.b import Class
             from c import func
 
             def foo() -> Optional[typing.Type[Class]]:
                 return Class if func() else None
             """,
+            range=CodeRange(start=CodePosition(7, 34), end=CodePosition(7, 41)),
         ),
         Invalid(
             """
             from __future__ import annotations
 
             from a.b import Class
 
             def foo(arg: "Class") -> None:
                 pass
 
             foo(Class())
             """,
-            line=5,
             expected_replacement="""
             from __future__ import annotations
 
             from a.b import Class
 
             def foo(arg: Class) -> None:
                 pass
 
             foo(Class())
             """,
+            range=CodeRange(start=CodePosition(5, 13), end=CodePosition(5, 20)),
         ),
         Invalid(
             """
             from __future__ import annotations
 
             from a.b import Class
 
             module_var: "Class" = Class()
             """,
-            line=5,
             expected_replacement="""
             from __future__ import annotations
 
             from a.b import Class
 
             module_var: Class = Class()
             """,
+            range=CodeRange(start=CodePosition(5, 12), end=CodePosition(5, 19)),
         ),
         Invalid(
             """
             from __future__ import annotations
 
             import typing
             from typing_extensions import Literal
             from a.b import Class
 
             def foo() -> typing.Tuple[Literal["a", "b"], "Class"]:
                 return Class()
             """,
-            line=7,
             expected_replacement="""
             from __future__ import annotations
 
             import typing
             from typing_extensions import Literal
             from a.b import Class
 
             def foo() -> typing.Tuple[Literal["a", "b"], Class]:
                 return Class()
             """,
+            range=CodeRange(start=CodePosition(7, 45), end=CodePosition(7, 52)),
         ),
     ]
 
-    def __init__(self, context: CstContext) -> None:
-        super().__init__(context)
+    METADATA_DEPENDENCIES = (QualifiedNameProvider,)
+
+    def __init__(self) -> None:
+        super().__init__()
         self.in_annotation: Set[cst.Annotation] = set()
         self.in_literal: Set[cst.Subscript] = set()
         self.has_future_annotations_import = False
 
     def visit_ImportFrom(self, node: cst.ImportFrom) -> None:
         if m.matches(
             node,
@@ -276,15 +279,15 @@
                     metadata=m.MatchMetadataIfTrue(
                         QualifiedNameProvider,
                         lambda qualnames: any(
                             n.name == "typing_extensions.Literal" for n in qualnames
                         ),
                     )
                 ),
-                metadata_resolver=self.context.wrapper,
+                metadata_resolver=self,
             ):
                 self.in_literal.add(node)
 
     def leave_Subscript(self, original_node: cst.Subscript) -> None:
         if not self.has_future_annotations_import:
             return
         if original_node in self.in_literal:
@@ -293,12 +296,9 @@
     def visit_SimpleString(self, node: cst.SimpleString) -> None:
         if not self.has_future_annotations_import:
             return
         if self.in_annotation and not self.in_literal:
             # This is not allowed past Python3.7 since it's no longer necessary.
             self.report(
                 node,
-                replacement=cst.parse_expression(
-                    node.evaluated_value,
-                    config=self.context.wrapper.module.config_for_parsing,
-                ),
+                replacement=cst.parse_expression(node.evaluated_value),
             )
```

### Comparing `fixit-0.1.4/fixit/rules/replace_union_with_optional.py` & `fixit-2.0.0a1/src/fixit/rules/replace_union_with_optional.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,16 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import libcst as cst
 import libcst.matchers as m
 
-from fixit import (
-    CstContext,
-    CstLintRule,
-    InvalidTestCase as Invalid,
-    ValidTestCase as Valid,
-)
+from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
 
 
 class ReplaceUnionWithOptionalRule(CstLintRule):
     """
     Enforces the use of ``Optional[T]`` over ``Union[T, None]`` and ``Union[None, T]``.
     See https://docs.python.org/3/library/typing.html#typing.Optional to learn more about Optionals.
     """
@@ -86,17 +81,14 @@
             from typing import Optional
             def func() -> Optional[Dict]:
                 pass
             """,
         ),
     ]
 
-    def __init__(self, context: CstContext) -> None:
-        super().__init__(context)
-
     def leave_Annotation(self, original_node: cst.Annotation) -> None:
         if self.contains_union_with_none(original_node):
             scope = self.get_metadata(cst.metadata.ScopeProvider, original_node, None)
             nones = 0
             indexes = []
             replacement = None
             if scope is not None and "Optional" in scope:
```

### Comparing `fixit-0.1.4/fixit/rules/rewrite_to_comprehension.py` & `fixit-2.0.0a1/src/fixit/rules/rewrite_to_comprehension.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+from typing import Optional, Union
+
 import libcst as cst
 import libcst.matchers as m
 
 from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
 
 
 UNNECESSARY_GENERATOR: str = (
@@ -100,22 +102,23 @@
             m.Call(
                 func=m.Name("list") | m.Name("set") | m.Name("dict"),
                 args=[m.Arg(value=m.GeneratorExp() | m.ListComp())],
             ),
         ):
             call_name = cst.ensure_type(node.func, cst.Name).value
 
+            exp: Union[cst.GeneratorExp, cst.ListComp]
             if m.matches(node.args[0].value, m.GeneratorExp()):
                 exp = cst.ensure_type(node.args[0].value, cst.GeneratorExp)
                 message_formatter = UNNECESSARY_GENERATOR
             else:
                 exp = cst.ensure_type(node.args[0].value, cst.ListComp)
                 message_formatter = UNNECESSARY_LIST_COMPREHENSION
 
-            replacement = None
+            replacement: Optional[Union[cst.Call, cst.BaseComp]] = None
             if call_name == "list":
                 replacement = node.deep_replace(
                     node, cst.ListComp(elt=exp.elt, for_in=exp.for_in)
                 )
             elif call_name == "set":
                 replacement = node.deep_replace(
                     node, cst.SetComp(elt=exp.elt, for_in=exp.for_in)
@@ -136,13 +139,13 @@
                     # Unrecoginized form
                     return
 
                 replacement = node.deep_replace(
                     node,
                     # pyre-fixme[6]: Expected `BaseAssignTargetExpression` for 1st
                     #  param but got `BaseExpression`.
-                    cst.DictComp(key=key, value=value, for_in=exp.for_in),
+                    cst.DictComp(key=key, value=value, for_in=exp.for_in),  # type: ignore
                 )
 
             self.report(
                 node, message_formatter.format(func=call_name), replacement=replacement
             )
```

### Comparing `fixit-0.1.4/fixit/rules/rewrite_to_literal.py` & `fixit-2.0.0a1/src/fixit/rules/rewrite_to_literal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+from typing import Sequence
+
 import libcst as cst
 import libcst.matchers as m
 
 from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
 
 
 UNNECESSARY_LITERAL: str = (
@@ -73,35 +75,39 @@
                 func=m.Name("tuple") | m.Name("list") | m.Name("set") | m.Name("dict"),
                 args=[m.Arg(value=m.List() | m.Tuple())],
             ),
         ) or m.matches(
             node,
             m.Call(func=m.Name("tuple") | m.Name("list") | m.Name("dict"), args=[]),
         ):
-
             pairs_matcher = m.ZeroOrMore(
                 m.Element(m.Tuple(elements=[m.DoNotCare(), m.DoNotCare()]))
                 | m.Element(m.List(elements=[m.DoNotCare(), m.DoNotCare()]))
             )
 
             exp = cst.ensure_type(node, cst.Call)
             call_name = cst.ensure_type(exp.func, cst.Name).value
 
             # If this is a empty call, it's an Unnecessary Call where we rewrite the call
             # to literal, except set().
+            elements: Sequence[cst.BaseElement]
             if not exp.args:
                 elements = []
                 message_formatter = UNNCESSARY_CALL
             else:
                 arg = exp.args[0].value
-                elements = cst.ensure_type(
-                    arg, cst.List if isinstance(arg, cst.List) else cst.Tuple
-                ).elements
+                if isinstance(arg, cst.List):
+                    elements = arg.elements
+                elif isinstance(arg, cst.Tuple):
+                    elements = arg.elements
+                else:
+                    raise ValueError(f"Unexpected {type(arg)}")
                 message_formatter = UNNECESSARY_LITERAL
 
+            new_node: cst.CSTNode
             if call_name == "tuple":
                 new_node = cst.Tuple(elements=elements)
             elif call_name == "list":
                 new_node = cst.List(elements=elements)
             elif call_name == "set":
                 # set() doesn't have an equivelant literal call. If it was
                 # matched here, it's an unnecessary literal suggestion.
@@ -119,20 +125,20 @@
                 exp.args[0].value,
                 m.Tuple(elements=[pairs_matcher]) | m.List(elements=[pairs_matcher]),
             ):
                 new_node = cst.Dict(
                     elements=[
                         (
                             lambda val: cst.DictElement(
-                                val.elements[0].value, val.elements[1].value
+                                val.elements[0].value, val.elements[1].value  # type: ignore
                             )
                         )(
                             cst.ensure_type(
                                 ele.value,
-                                cst.Tuple
+                                cst.Tuple  # type: ignore
                                 if isinstance(ele.value, cst.Tuple)
                                 else cst.List,
                             )
                         )
                         for ele in elements
                     ]
                 )
```

### Comparing `fixit-0.1.4/fixit/rules/sorted_attributes_rule.py` & `fixit-2.0.0a1/src/fixit/rules/sorted_attributes_rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import List, Union
 
 import libcst as cst
@@ -97,15 +97,15 @@
                 found_any_assign = True
                 assign_lines.append(line)
             else:
                 _add_unmatched_line(line)
                 continue
 
         sorted_assign_lines = sorted(
-            assign_lines, key=lambda line: line.body[0].targets[0].target.value
+            assign_lines, key=lambda line: line.body[0].targets[0].target.value  # type: ignore
         )
         if sorted_assign_lines == assign_lines:
             return
         self.report(
             node,
             replacement=node.with_changes(
                 body=node.body.with_changes(
```

### Comparing `fixit-0.1.4/fixit/rules/use_assert_in.py` & `fixit-2.0.0a1/src/fixit/rules/use_assert_in.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import libcst as cst
 import libcst.matchers as m
 from libcst.helpers import ensure_type
```

### Comparing `fixit-0.1.4/fixit/rules/use_assert_is_not_none.py` & `fixit-2.0.0a1/src/fixit/rules/use_assert_is_not_none.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Sequence
 
 import libcst as cst
 import libcst.matchers as m
 from libcst.helpers import ensure_type
 
-from fixit.common.base import CstLintRule
-from fixit.common.utils import InvalidTestCase as Invalid, ValidTestCase as Valid
+from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
 
 
 class UseAssertIsNotNoneRule(CstLintRule):
     """
     Discourages use of ``assertTrue(x is not None)`` and ``assertFalse(x is not None)`` as it is deprecated (https://docs.python.org/3.8/library/unittest.html#deprecated-aliases).
     Use ``assertIsNotNone(x)`` and ``assertIsNone(x)``) instead.
```

### Comparing `fixit-0.1.4/fixit/rules/use_classname_as_code.py` & `fixit-2.0.0a1/src/fixit/rules/use_classname_as_code.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import re
 from typing import cast
 
 import libcst as cst
 import libcst.matchers as m
 
-from fixit import (
-    CstContext,
-    CstLintRule,
-    InvalidTestCase as Invalid,
-    ValidTestCase as Valid,
-)
+from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
 
 
 class UseClassNameAsCodeRule(CstLintRule):
     """
     Meta lint rule which checks that codes of lint rules are migrated to new format in lint rule class definitions.
     """
 
@@ -76,16 +71,16 @@
                         code="",
                         )
                 ]
             """,
         ),
     ]
 
-    def __init__(self, context: CstContext) -> None:
-        super().__init__(context)
+    def __init__(self) -> None:
+        super().__init__()
         self.inside_invalid_call: bool = False
 
     def visit_SimpleString(self, node: cst.SimpleString) -> None:
         matched = re.match(r"^(\'|\")(?P<igcode>IG\d+ )\S", node.value)
 
         if matched is not None:
             replacement_string = node.value.replace(matched.group("igcode"), "", 1)
```

### Comparing `fixit-0.1.4/fixit/rules/use_fstring.py` & `fixit-2.0.0a1/src/fixit/rules/use_fstring.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import re
-from typing import Callable, cast
+from typing import Callable, cast, List, Optional
 
 import libcst as cst
 import libcst.matchers as m
 
 from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
 
 
 USE_FSTRING_SIMPLE_EXPRESSION_MAX_LENGTH = 30
 
 
-def _match_simple_string(node: cst.CSTNode) -> bool:
+def _match_simple_string(node: cst.BaseExpression) -> bool:
     if isinstance(node, cst.SimpleString) and "b" not in node.prefix.lower():
         # SimpleString can be a bytes and fstring don't support bytes
         # This helper is for autofixer and it only handles %s simple cases for now.
         # for the other types like %f %d, it require more processing on the format.
         # Convert a %d to fstring will change the exception type. We may get help
         # from TypeInferenceProvider to confirm the type before codedmod.
         # We leave it as future work.
         return re.fullmatch("[^%]*(%s[^%]*)+", node.raw_value) is not None
     return False
 
 
-def _gen_match_simple_expression(module: cst.Module) -> Callable[[cst.CSTNode], bool]:
-    def _match_simple_expression(node: cst.CSTNode) -> bool:
+def _gen_match_simple_expression(
+    codegen: Callable[[cst.CSTNode], str],
+) -> Callable[[cst.BaseExpression], bool]:
+    def _match_simple_expression(node: cst.BaseExpression) -> bool:
         # either each element in Tuple is simple expression or the entire expression is simple.
         if (
             isinstance(node, cst.Tuple)
             and all(
-                len(module.code_for_node(elm.value))
-                < USE_FSTRING_SIMPLE_EXPRESSION_MAX_LENGTH
+                len(codegen(elm.value)) < USE_FSTRING_SIMPLE_EXPRESSION_MAX_LENGTH
                 for elm in node.elements
             )
-        ) or len(module.code_for_node(node)) < USE_FSTRING_SIMPLE_EXPRESSION_MAX_LENGTH:
+        ) or len(codegen(node)) < USE_FSTRING_SIMPLE_EXPRESSION_MAX_LENGTH:
             return True
         return False
 
     return _match_simple_expression
 
 
 class EscapeStringQuote(cst.CSTTransformer):
@@ -80,18 +81,18 @@
         For example:
 
         1: this is the answer: %d" % (a_long_function_call() + b_another_long_function_call())
         2: f"this is the answer: {a_long_function_call() + b_another_long_function_call()}"
         3: result = a_long_function_call() + b_another_long_function_call()
         f"this is the answer: {result}"
 
-        Line 1 is more readable than line 2. Ideally, we’d like developers to manually fix this case to line 3
+        Line 1 is more readable than line 2. Ideally, we'd like developers to manually fix this case to line 3
 
     2. only %s placeholders are linted against for now. We leave it as future work to support other placeholders.
-        For example, %d raises TypeError for non-numeric objects, whereas f“{x:d}” raises ValueError.
+        For example, %d raises TypeError for non-numeric objects, whereas f"{x:d}" raises ValueError.
         This discrepancy in the type of exception raised could potentially break the logic in the code where the exception is handled
     """
 
     MESSAGE: str = (
         "Do not use printf style formatting or .format(). "
         + "Use f-string instead to be more readable and efficient. "
         + "See https://www.python.org/dev/peps/pep-0498/"
@@ -139,42 +140,50 @@
         ),
         Invalid(
             '"a list: %s" % " ".join(var)',
             expected_replacement='''f"a list: {' '.join(var)}"''',
         ),
     ]
 
+    _codegen: Optional[Callable[[cst.CSTNode], str]]
+
+    def visit_Module(self, node: cst.Module) -> Optional[bool]:
+        self._codegen = node.code_for_node
+        return super().visit_Module(node)
+
     def visit_Call(self, node: cst.Call) -> None:
         if m.matches(
             node,
             m.Call(
                 func=m.Attribute(value=m.SimpleString(), attr=m.Name(value="format"))
             ),
         ):
             self.report(node)
 
     def visit_BinaryOperation(self, node: cst.BinaryOperation) -> None:
+        codegen = self._codegen
+        if not codegen:
+            raise ValueError("No codegen found. Have we visited a Module?")
+
         expr_key = "expr"
         extracts = m.extract(
             node,
             m.BinaryOperation(
                 left=m.MatchIfTrue(_match_simple_string),
                 operator=m.Modulo(),
                 right=m.SaveMatchedNode(
-                    m.MatchIfTrue(
-                        _gen_match_simple_expression(self.context.wrapper.module)
-                    ),
+                    m.MatchIfTrue(_gen_match_simple_expression(codegen)),
                     expr_key,
                 ),
             ),
         )
 
         if extracts:
-            expr = extracts[expr_key]
-            parts = []
+            expr = cast(cst.BaseExpression, extracts[expr_key])
+            parts: List[cst.BaseFormattedStringContent] = []
             simple_string = cst.ensure_type(node.left, cst.SimpleString)
             innards = simple_string.raw_value.replace("{", "{{").replace("}", "}}")
             tokens = innards.split("%s")
             token = tokens[0]
             if len(token) > 0:
                 parts.append(cst.FormattedStringText(value=token))
             expressions = (
@@ -190,14 +199,15 @@
                     self.report(node)
                     return
                 try:
                     parts.append(
                         cst.FormattedStringExpression(
                             expression=cast(
                                 cst.BaseExpression,
+                                # pyre-fixme[16]: `Sequence` has no attribute `visit`.
                                 expressions[i - 1].visit(escape_transformer),
                             )
                         )
                     )
                 except Exception:
                     self.report(node)
                     return
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `fixit-0.1.4/fixit/rules/use_lint_fixme_comment.py` & `fixit-2.0.0a1/src/fixit/rules/use_lint_fixme_comment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 import libcst as cst
 
 from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
```

### Comparing `fixit-0.1.4/fixit/rules/use_types_from_typing.py` & `fixit-2.0.0a1/src/fixit/rules/use_types_from_typing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,18 @@
-# Copyright (c) Facebook, Inc. and its affiliates.
+# Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from typing import Set
 
 import libcst
 from libcst.metadata import QualifiedNameProvider, ScopeProvider
 
-from fixit import (
-    CstContext,
-    CstLintRule,
-    InvalidTestCase as Invalid,
-    ValidTestCase as Valid,
-)
+from fixit import CstLintRule, InvalidTestCase as Invalid, ValidTestCase as Valid
 
 
 REPLACE_BUILTIN_TYPE_ANNOTATION: str = (
     "You are using builtins.{builtin_type} as a type annotation "
     + "but the type system doesn't recognize it as a valid type."
     + " You should use typing.{correct_type} instead."
 )
@@ -113,16 +108,16 @@
             from typing import Dict
             def func() -> None:
                 thing: Dict[str, str] = {}
             """,
         ),
     ]
 
-    def __init__(self, context: CstContext) -> None:
-        super().__init__(context)
+    def __init__(self) -> None:
+        super().__init__()
         self.annotation_counter: int = 0
 
     def visit_Annotation(self, node: libcst.Annotation) -> None:
         self.annotation_counter += 1
 
     def leave_Annotation(self, original_node: libcst.Annotation) -> None:
         self.annotation_counter -= 1
```

