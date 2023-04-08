# Comparing `tmp/vws-python-mock-2023.3.5.tar.gz` & `tmp/vws-python-mock-2023.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vws-python-mock-2023.3.5.tar", last modified: Sun Mar  5 22:31:17 2023, max compression
+gzip compressed data, was "vws-python-mock-2023.4.8.tar", last modified: Sat Apr  8 18:21:20 2023, max compression
```

## Comparing `vws-python-mock-2023.3.5.tar` & `vws-python-mock-2023.4.8.tar`

### file list

```diff
@@ -1,162 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.608524 vws-python-mock-2023.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.596524 vws-python-mock-2023.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.596524 vws-python-mock-2023.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/.github/workflows/docker-build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/.github/workflows/windows-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-05 22:30:59.000000 vws-python-mock-2023.3.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-03-05 22:31:17.608524 vws-python-mock-2023.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.596524 vws-python-mock-2023.3.5/ci/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/ci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/ci/custom_linters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/ci/decrypt_secret.sh
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/ci/set_secrets_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/codecov.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.596524 vws-python-mock-2023.3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.600524 vws-python-mock-2023.3.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/source/basic-example.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/source/ci-setup.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2508 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/source/differences-to-vws.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4557 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/source/docker.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/source/getting-started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/source/mock-api-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/source/release-process.rst
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/docs/source/versioning-and-api-stability.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/lint.mk
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.600524 vws-python-mock-2023.3.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/requirements/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/requirements/setup-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/secrets.tar.gpg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-05 22:31:17.608524 vws-python-mock-2023.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/spelling_private_dict.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.592524 vws-python-mock-2023.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.600524 vws-python-mock-2023.3.5/src/mock_vws/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_base64_decoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    25347 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_cgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_database_matchers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.600524 vws-python-mock-2023.3.5/src/mock_vws/_flask_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_flask_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.592524 vws-python-mock-2023.3.5/src/mock_vws/_flask_server/dockerfiles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.600524 vws-python-mock-2023.3.5/src/mock_vws/_flask_server/dockerfiles/target_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_flask_server/dockerfiles/target_manager/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.600524 vws-python-mock-2023.3.5/src/mock_vws/_flask_server/dockerfiles/vwq/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_flask_server/dockerfiles/vwq/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.600524 vws-python-mock-2023.3.5/src/mock_vws/_flask_server/dockerfiles/vws/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_flask_server/dockerfiles/vws/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_flask_server/target_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_flask_server/vwq.py
--rw-r--r--   0 runner    (1001) docker     (123)    17769 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_flask_server/vws.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_mock_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_query_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.604524 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/accept_header_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/auth_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/content_length_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/content_type_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/date_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    24458 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/fields_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/image_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/include_target_data_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/num_results_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/project_state_validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.604524 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_query_validators/resources/query_out_of_bounds_response.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.604524 vws-python-mock-2023.3.5/src/mock_vws/_requests_mock_server/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_requests_mock_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5261 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_requests_mock_server/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_requests_mock_server/mock_web_query_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23736 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_requests_mock_server/mock_web_services_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.604524 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/active_flag_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/auth_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/content_length_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/content_type_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/date_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)    16098 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/image_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/json_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/key_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/metadata_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/name_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/project_state_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/target_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/_services_validators/width_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/database.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.604524 vws-python-mock-2023.3.5/src/mock_vws/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/resources/deleted_target_matched_response.html
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/resources/oops_error_occurred_response.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/src/mock_vws/target_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.604524 vws-python-mock-2023.3.5/src/vws_python_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-03-05 22:31:17.000000 vws-python-mock-2023.3.5/src/vws_python_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-03-05 22:31:17.000000 vws-python-mock-2023.3.5/src/vws_python_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 22:31:17.000000 vws-python-mock-2023.3.5/src/vws_python_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 22:31:17.000000 vws-python-mock-2023.3.5/src/vws_python_mock.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-03-05 22:31:17.000000 vws-python-mock-2023.3.5/src/vws_python_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-05 22:31:17.000000 vws-python-mock-2023.3.5/src/vws_python_mock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.604524 vws-python-mock-2023.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.608524 vws-python-mock-2023.3.5/tests/mock_vws/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.608524 vws-python-mock-2023.3.5/tests/mock_vws/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/fixtures/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/fixtures/prepared_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/fixtures/vuforia_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/jetty_error_array_out_of_bounds.html
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/jetty_error_array_out_of_bounds_2.html
--rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/jetty_error_array_out_of_bounds_3.html
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/jetty_error_deletion_not_complete.html
--rw-r--r--   0 runner    (1001) docker     (123)    32319 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_add_target.py
--rw-r--r--   0 runner    (1001) docker     (123)    11980 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_authorization_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_content_length.py
--rw-r--r--   0 runner    (1001) docker     (123)    13009 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_database_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    10104 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_date_header.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_delete_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11816 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_flask_app_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_get_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_get_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_invalid_given_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_invalid_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    66643 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_requests_mock_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_target_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_target_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_unexpected_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/test_update_target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:31:17.608524 vws-python-mock-2023.3.5/tests/mock_vws/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/utils/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/tests/mock_vws/utils/usage_test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-03-05 22:30:57.000000 vws-python-mock-2023.3.5/vuforia_secrets.env.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.432574 vws-python-mock-2023.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.408573 vws-python-mock-2023.4.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.408573 vws-python-mock-2023.4.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.github/workflows/docker-build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.github/workflows/windows-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.408573 vws-python-mock-2023.4.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-08 18:21:02.000000 vws-python-mock-2023.4.8/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-08 18:21:20.432574 vws-python-mock-2023.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.408573 vws-python-mock-2023.4.8/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/ci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/ci/custom_linters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/ci/decrypt_secret.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/ci/set_secrets_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/doc8.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.408573 vws-python-mock-2023.4.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.412573 vws-python-mock-2023.4.8/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/basic-example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/ci-setup.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2569 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/differences-to-vws.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/getting-started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/mock-api-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/release-process.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/docs/source/versioning-and-api-stability.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/lint.mk
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12335 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/secrets.tar.gpg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 18:21:20.432574 vws-python-mock-2023.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/spelling_private_dict.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.404573 vws-python-mock-2023.4.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.416574 vws-python-mock-2023.4.8/src/mock_vws/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_base64_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_database_matchers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.416574 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.404573 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/dockerfiles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.416574 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/dockerfiles/target_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/dockerfiles/target_manager/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.416574 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/dockerfiles/vwq/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/dockerfiles/vwq/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.416574 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/dockerfiles/vws/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/dockerfiles/vws/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     8802 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/target_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/vwq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20085 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_flask_server/vws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_mock_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.420574 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/accept_header_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/auth_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/content_length_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/content_type_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/date_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23346 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/fields_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/image_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/include_target_data_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/num_results_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_query_validators/project_state_validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.420574 vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/mock_web_query_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25025 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/mock_web_services_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.424574 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/active_flag_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/auth_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/content_length_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/content_type_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/date_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17325 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/image_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/json_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/key_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/metadata_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/name_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/project_state_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/target_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/_services_validators/width_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/image_matchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.424574 vws-python-mock-2023.4.8/src/mock_vws/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/resources/deleted_target_matched_response.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/resources/oops_error_occurred_response.html
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7135 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/target_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/src/mock_vws/target_raters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.424574 vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-08 18:21:20.000000 vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-04-08 18:21:20.000000 vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:21:20.000000 vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:21:19.000000 vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-04-08 18:21:20.000000 vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-08 18:21:20.000000 vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.424574 vws-python-mock-2023.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.428574 vws-python-mock-2023.4.8/tests/mock_vws/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.428574 vws-python-mock-2023.4.8/tests/mock_vws/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/fixtures/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/fixtures/prepared_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/fixtures/vuforia_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/jetty_error_deletion_not_complete.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32560 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_add_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_authorization_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_content_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13101 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_database_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10196 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_date_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_delete_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20015 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_flask_app_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8193 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_get_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_get_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_invalid_given_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_invalid_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69389 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28210 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_requests_mock_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_target_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_target_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_unexpected_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29397 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/test_update_target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:21:20.432574 vws-python-mock-2023.4.8/tests/mock_vws/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8889 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/utils/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4746 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/tests/mock_vws/utils/usage_test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-08 18:21:00.000000 vws-python-mock-2023.4.8/vuforia_secrets.env.example
```

### Comparing `vws-python-mock-2023.3.5/.github/workflows/ci.yml` & `vws-python-mock-2023.4.8/.github/workflows/ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -9,114 +9,105 @@
     branches: [master]
   schedule:
     # * is a special character in YAML so you have to quote this string
     # Run at 1:00 every day
     - cron: '0 1 * * *'
   workflow_dispatch: {}
 
+# We share Vuforia credentials and therefore Vuforia databases across
+# workflows.
+# We therefore want to run only one workflow at a time.
+concurrency: vuforia_credentials
+
 jobs:
   build:
 
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.11"]
         ci_pattern:
-          - test_query.py::TestContentType
-          - test_query.py::TestSuccess
-          - test_query.py::TestIncorrectFields
-          - test_query.py::TestMaxNumResults
-          - test_query.py::TestIncludeTargetData
-          - test_query.py::TestAcceptHeader
-          - test_query.py::TestActiveFlag
-          - test_query.py::TestBadImage
-          - test_query.py::TestMaximumImageFileSize
-          - test_query.py::TestMaximumImageDimensions
-          - test_query.py::TestImageFormats
-          - test_query.py::TestProcessing
-          - test_query.py::TestUpdate
-          - test_query.py::TestDeleted
-          - test_query.py::TestTargetStatusFailed
-          - test_query.py::TestDateFormats
-          - test_query.py::TestInactiveProject
-          - test_add_target.py
-          - test_authorization_header.py::TestAuthorizationHeader
-          - test_authorization_header.py::TestMalformed::test_one_part_no_space
-          - test_authorization_header.py::TestMalformed::test_one_part_with_space
-          - test_authorization_header.py::TestMalformed::test_missing_signature
-          - test_authorization_header.py::TestBadKey
-          - test_content_length.py::TestIncorrect::test_not_integer
-          - test_content_length.py::TestIncorrect::test_too_large
-          - test_content_length.py::TestIncorrect::test_too_small
-          - test_database_summary.py
-          - test_date_header.py::TestFormat
-          - test_date_header.py::TestMissing
-          - test_date_header.py::TestSkewedTime::test_date_out_of_range
-          - test_date_header.py::TestSkewedTime::test_date_in_range
-          - test_delete_target.py
-          - test_get_duplicates.py
-          - test_get_target.py
-          - test_invalid_given_id.py
-          - test_invalid_json.py
-          - test_target_list.py
-          - test_target_summary.py
-          - test_unexpected_json.py
-          - test_update_target.py::TestActiveFlag
-          - test_update_target.py::TestApplicationMetadata
-          - test_update_target.py::TestImage::test_image_valid
-          - test_update_target.py::TestImage::test_bad_image_format_or_color_space
-          - test_update_target.py::TestImage::test_corrupted
-          - test_update_target.py::TestImage::test_image_too_large
-          - test_update_target.py::TestImage::test_not_base64_encoded_processable
-          - test_update_target.py::TestImage::test_not_base64_encoded_not_processable
-          - test_update_target.py::TestImage::test_not_image
-          - test_update_target.py::TestImage::test_invalid_type
-          - test_update_target.py::TestImage::test_rating_can_change
-          - test_update_target.py::TestTargetName
-          - test_update_target.py::TestUnexpectedData
-          - test_update_target.py::TestUpdate
-          - test_update_target.py::TestWidth
-          - test_update_target.py::TestInactiveProject
-          - test_requests_mock_usage.py
-          - test_flask_app_usage.py
-          - test_docker.py
+          - tests/mock_vws/test_query.py::TestContentType
+          - tests/mock_vws/test_query.py::TestSuccess
+          - tests/mock_vws/test_query.py::TestIncorrectFields
+          - tests/mock_vws/test_query.py::TestMaxNumResults
+          - tests/mock_vws/test_query.py::TestIncludeTargetData
+          - tests/mock_vws/test_query.py::TestAcceptHeader
+          - tests/mock_vws/test_query.py::TestActiveFlag
+          - tests/mock_vws/test_query.py::TestBadImage
+          - tests/mock_vws/test_query.py::TestMaximumImageFileSize
+          - tests/mock_vws/test_query.py::TestMaximumImageDimensions
+          - tests/mock_vws/test_query.py::TestImageFormats
+          - tests/mock_vws/test_query.py::TestProcessing
+          - tests/mock_vws/test_query.py::TestUpdate
+          - tests/mock_vws/test_query.py::TestDeleted
+          - tests/mock_vws/test_query.py::TestTargetStatusFailed
+          - tests/mock_vws/test_query.py::TestDateFormats
+          - tests/mock_vws/test_query.py::TestInactiveProject
+          - tests/mock_vws/test_add_target.py
+          - tests/mock_vws/test_authorization_header.py::TestAuthorizationHeader
+          - tests/mock_vws/test_authorization_header.py::TestMalformed::test_one_part_no_space
+          - tests/mock_vws/test_authorization_header.py::TestMalformed::test_one_part_with_space
+          - tests/mock_vws/test_authorization_header.py::TestMalformed::test_missing_signature
+          - tests/mock_vws/test_authorization_header.py::TestBadKey
+          - tests/mock_vws/test_content_length.py::TestIncorrect::test_not_integer
+          - tests/mock_vws/test_content_length.py::TestIncorrect::test_too_large
+          - tests/mock_vws/test_content_length.py::TestIncorrect::test_too_small
+          - tests/mock_vws/test_database_summary.py
+          - tests/mock_vws/test_date_header.py::TestFormat
+          - tests/mock_vws/test_date_header.py::TestMissing
+          - tests/mock_vws/test_date_header.py::TestSkewedTime::test_date_out_of_range
+          - tests/mock_vws/test_date_header.py::TestSkewedTime::test_date_in_range
+          - tests/mock_vws/test_delete_target.py
+          - tests/mock_vws/test_get_duplicates.py
+          - tests/mock_vws/test_get_target.py
+          - tests/mock_vws/test_invalid_given_id.py
+          - tests/mock_vws/test_invalid_json.py
+          - tests/mock_vws/test_target_list.py
+          - tests/mock_vws/test_target_summary.py
+          - tests/mock_vws/test_unexpected_json.py
+          - tests/mock_vws/test_update_target.py::TestActiveFlag
+          - tests/mock_vws/test_update_target.py::TestApplicationMetadata
+          - tests/mock_vws/test_update_target.py::TestImage::test_image_valid
+          - tests/mock_vws/test_update_target.py::TestImage::test_bad_image_format_or_color_space
+          - tests/mock_vws/test_update_target.py::TestImage::test_corrupted
+          - tests/mock_vws/test_update_target.py::TestImage::test_image_too_large
+          - tests/mock_vws/test_update_target.py::TestImage::test_not_base64_encoded_processable
+          - tests/mock_vws/test_update_target.py::TestImage::test_not_base64_encoded_not_processable
+          - tests/mock_vws/test_update_target.py::TestImage::test_not_image
+          - tests/mock_vws/test_update_target.py::TestImage::test_invalid_type
+          - tests/mock_vws/test_update_target.py::TestImage::test_rating_can_change
+          - tests/mock_vws/test_update_target.py::TestTargetName
+          - tests/mock_vws/test_update_target.py::TestUnexpectedData
+          - tests/mock_vws/test_update_target.py::TestUpdate
+          - tests/mock_vws/test_update_target.py::TestWidth
+          - tests/mock_vws/test_update_target.py::TestInactiveProject
+          - tests/mock_vws/test_requests_mock_usage.py
+          - tests/mock_vws/test_flask_app_usage.py
+          - tests/mock_vws/test_docker.py
+          - README.rst
+          - docs/source/basic-example.rst
 
     steps:
-      # We share Vuforia credentials and therefore Vuforia databases across
-      # workflows.
-      # We therefore want to run only one workflow at a time.
-      - name: Wait for other GitHub Workflows to finish
-        uses: softprops/turnstyle@v1
-        with:
-          same-branch-only: false
-          # By default this is 60.
-          # We have a lot of jobs so this is set higher - we hit API timeouts.
-          poll-interval-seconds: 300
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-
       - uses: actions/checkout@v3
         with:
           # See https://github.com/codecov/codecov-action/issues/190.
           fetch-depth: 2
 
       - name: "Set up Python"
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - uses: actions/cache@v3
         with:
           path: ~/.cache/pip
-          # This is like the example but we use ``*requirements.txt`` rather
-          # than ``requirements.txt`` because we have multiple requirements
-          # files.
-          key: ${{ runner.os }}-pip-${{ hashFiles('**/*requirements.txt') }}
+          key: ${{ runner.os }}-pip-${{ hashFiles('pyproject.toml') }}
           restore-keys: |
             ${{ runner.os }}-pip-
 
       - name: "Install dependencies"
         run: |
           python -m pip install --upgrade pip setuptools wheel
           # We use '--ignore-installed' to avoid GitHub's cache which can cause
@@ -141,15 +132,15 @@
             -s \
             -vvv \
             --showlocals \
             --exitfirst \
             --cov=src/ \
             --cov=tests \
             --cov-report=xml \
-            tests/mock_vws/${{ matrix.ci_pattern }}
+            ${{ matrix.ci_pattern }}
 
       - name: "Show coverage file"
         run: |
           # Sometimes we have been sure that we have 100% coverage, but codecov
           # says otherwise.
           #
           # We show the coverage file here to help with debugging.
@@ -168,8 +159,9 @@
         run: |
           echo ${{ github.event_name }}
 
       - name: "Upload coverage to Codecov"
         uses: "codecov/codecov-action@v3"
         with:
           fail_ci_if_error: true
+          token: ${{ secrets.CODECOV_TOKEN }}
         if: ${{ github.event_name == 'pull_request' || github.event_name == 'push' }}
```

### Comparing `vws-python-mock-2023.3.5/.github/workflows/docker-build.yml` & `vws-python-mock-2023.4.8/.github/workflows/docker-build.yml`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.3.5/.github/workflows/lint.yml` & `vws-python-mock-2023.4.8/.github/workflows/lint.yml`

 * *Files 21% similar despite different names*

```diff
@@ -27,18 +27,15 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - uses: actions/cache@v3
         with:
           path: ~/.cache/pip
-          # This is like the example but we use ``*requirements.txt`` rather
-          # than ``requirements.txt`` because we have multiple requirements
-          # files.
-          key: ${{ runner.os }}-pip-${{ hashFiles('**/*requirements.txt') }}
+          key: ${{ runner.os }}-pip-${{ hashFiles('pyproject.toml') }}
           restore-keys: |
             ${{ runner.os }}-pip-
 
       - name: "Install dependencies"
         run: |
           python -m pip install --upgrade pip setuptools wheel
           # We use '--ignore-installed' to avoid GitHub's cache which can cause
```

### Comparing `vws-python-mock-2023.3.5/.github/workflows/release.yml` & `vws-python-mock-2023.4.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.3.5/.github/workflows/windows-ci.yml` & `vws-python-mock-2023.4.8/.github/workflows/windows-ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -33,18 +33,15 @@
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - uses: actions/cache@v3
         with:
           path: ~/.cache/pip
-          # This is like the example but we use ``*requirements.txt`` rather
-          # than ``requirements.txt`` because we have multiple requirements
-          # files.
-          key: ${{ runner.os }}-pip-${{ hashFiles('**/*requirements.txt') }}
+          key: ${{ runner.os }}-pip-${{ hashFiles('pyproject.toml') }}
           restore-keys: |
             ${{ runner.os }}-pip-
 
       - name: "Install dependencies"
         run: |
           python -m pip install --upgrade pip setuptools wheel
           # We use '--ignore-installed' to avoid GitHub's cache which can cause
@@ -81,8 +78,11 @@
         run: |
           echo ${{ github.event_name }}
 
       - name: "Upload coverage to Codecov"
         uses: "codecov/codecov-action@v3"
         with:
           fail_ci_if_error: true
+          # See https://community.codecov.com/t/upload-issues-unable-to-locate-build-via-github-actions-api/3954
+          # which tells us to use the token to avoid errors.
+          token: ${{ secrets.CODECOV_TOKEN }}
         if: ${{ github.event_name == 'pull_request' || github.event_name == 'push' }}
```

### Comparing `vws-python-mock-2023.3.5/.gitignore` & `vws-python-mock-2023.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.3.5/CHANGELOG.rst` & `vws-python-mock-2023.4.8/CHANGELOG.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 =========
 
 Next
 ----
 
+2023.04.08
+------------
+
+2023.03.26
+------------
+
 2023.03.05
 ------------
 
 2021.12.27.3
 ------------
 
 2021.12.27.2
```

### Comparing `vws-python-mock-2023.3.5/CODE_OF_CONDUCT.rst` & `vws-python-mock-2023.4.8/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.3.5/LICENSE` & `vws-python-mock-2023.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.3.5/Makefile` & `vws-python-mock-2023.4.8/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     black \
     check-manifest \
     doc8 \
     linkcheck \
     mypy \
     pip-extra-reqs \
     pip-missing-reqs \
+    pyright \
     pyroma \
     ruff \
     spelling \
     vulture \
     pylint \
     custom-linters
```

### Comparing `vws-python-mock-2023.3.5/PKG-INFO` & `vws-python-mock-2023.4.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vws-python-mock
-Version: 2023.3.5
+Version: 2023.4.8
 Summary: A mock for the Vuforia Web Services (VWS) API.
 Author-email: Adam Dangoor <adamdangoor@gmail.com>
 License: The MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -55,18 +55,19 @@
 
 This requires Python 3.11+.
 
 .. code:: sh
 
     pip install vws-python-mock
 
-.. code:: python
+.. code-block:: python
 
     import requests
-    from mock_vws import MockVWS, VuforiaDatabase
+    from mock_vws import MockVWS
+    from mock_vws.database import VuforiaDatabase
 
     with MockVWS() as mock:
         database = VuforiaDatabase()
         mock.add_database(database=database)
         # This will use the Vuforia mock.
         requests.get('https://vws.vuforia.com/summary')
```

### Comparing `vws-python-mock-2023.3.5/README.rst` & `vws-python-mock-2023.4.8/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,19 @@
 
 This requires Python 3.11+.
 
 .. code:: sh
 
     pip install vws-python-mock
 
-.. code:: python
+.. code-block:: python
 
     import requests
-    from mock_vws import MockVWS, VuforiaDatabase
+    from mock_vws import MockVWS
+    from mock_vws.database import VuforiaDatabase
 
     with MockVWS() as mock:
         database = VuforiaDatabase()
         mock.add_database(database=database)
         # This will use the Vuforia mock.
         requests.get('https://vws.vuforia.com/summary')
```

### Comparing `vws-python-mock-2023.3.5/ci/custom_linters.py` & `vws-python-mock-2023.4.8/ci/custom_linters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 Custom lint tests.
 """
 
-import subprocess
 from pathlib import Path
 
 import pytest
 import yaml
 
 
 def _ci_patterns() -> set[str]:
@@ -19,63 +18,71 @@
     matrix = github_workflow_config["jobs"]["build"]["strategy"]["matrix"]
     ci_pattern_list = matrix["ci_pattern"]
     ci_patterns = set(ci_pattern_list)
     assert len(ci_pattern_list) == len(ci_patterns)
     return ci_patterns
 
 
-def _tests_from_pattern(ci_pattern: str) -> set[str]:
+def _tests_from_pattern(
+    ci_pattern: str,
+    capsys: pytest.CaptureFixture[str],
+) -> set[str]:
     """
     From a CI pattern, get all tests ``pytest`` would collect.
     """
+    # Clear the captured output.
+    capsys.readouterr()
     tests: set[str] = set()
-    args = ["pytest", "-q", "--collect-only", ci_pattern]
-    result = subprocess.run(args=args, stdout=subprocess.PIPE, check=True)
-    for line in result.stdout.decode().splitlines():
+    pytest.main(args=["-q", "--collect-only", ci_pattern])
+    data = capsys.readouterr().out
+    for line in data.splitlines():
+        # We filter empty lines and lines which look like
+        # "9 tests collected in 0.01s".
         if line and "collected in" not in line:
             tests.add(line)
     return tests
 
 
 def test_ci_patterns_valid() -> None:
     """
     All of the CI patterns in the CI configuration match at least one test in
     the test suite.
     """
     ci_patterns = _ci_patterns()
 
     for ci_pattern in ci_patterns:
-        pattern = "tests/mock_vws/" + ci_pattern
-        collect_only_result = pytest.main(["--collect-only", pattern])
+        collect_only_result = pytest.main(["--collect-only", ci_pattern])
 
         message = f'"{ci_pattern}" does not match any tests.'
         assert collect_only_result == 0, message
 
 
-def test_tests_collected_once() -> None:
+def test_tests_collected_once(
+    capsys: pytest.CaptureFixture[str],
+) -> None:
     """
     Each test in the test suite is collected exactly once.
 
     This does not necessarily mean that they are run - they may be skipped.
     """
     ci_patterns = _ci_patterns()
     tests_to_patterns: dict[str, set[str]] = {}
+
     for pattern in ci_patterns:
-        pattern_in_dir = "tests/mock_vws/" + pattern
-        tests = _tests_from_pattern(ci_pattern=pattern_in_dir)
+        tests = _tests_from_pattern(ci_pattern=pattern, capsys=capsys)
         for test in tests:
             if test in tests_to_patterns:
-                tests_to_patterns[test].add(pattern_in_dir)
+                tests_to_patterns[test].add(pattern)
             else:
-                tests_to_patterns[test] = {pattern_in_dir}
+                tests_to_patterns[test] = {pattern}
 
     for test_name, patterns in tests_to_patterns.items():
         message = (
             f'Test "{test_name}" will be run once for each pattern in '
             f"{patterns}. "
             "Each test should be run only once."
         )
         assert len(patterns) == 1, message
 
-    all_tests = _tests_from_pattern(ci_pattern="tests/")
+    all_tests = _tests_from_pattern(ci_pattern=".", capsys=capsys)
     assert tests_to_patterns.keys() - all_tests == set()
     assert all_tests - tests_to_patterns.keys() == set()
```

### Comparing `vws-python-mock-2023.3.5/ci/set_secrets_file.py` & `vws-python-mock-2023.4.8/ci/set_secrets_file.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.3.5/docs/Makefile` & `vws-python-mock-2023.4.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.3.5/docs/source/basic-example.rst` & `vws-python-mock-2023.4.8/docs/source/basic-example.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Using the mock redirects requests to Vuforia made with `requests`_ to an in-memory implementation.
 
-.. code:: python
+.. code-block:: python
 
     import requests
-    from mock_vws import MockVWS, VuforiaDatabase
+    from mock_vws import MockVWS
+    from mock_vws.database import VuforiaDatabase
 
     with MockVWS() as mock:
         database = VuforiaDatabase()
         mock.add_database(database=database)
         # This will use the Vuforia mock.
         requests.get('https://vws.vuforia.com/summary')
```

### Comparing `vws-python-mock-2023.3.5/docs/source/ci-setup.rst` & `vws-python-mock-2023.4.8/docs/source/ci-setup.rst`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 CI is set up with secrets for connecting to Vuforia.
 These variables include those from :file:`vuforia_secrets.env.example`.
 
 To avoid hitting request quotas and to avoid conflicts when running multiple tests in parallel, we use multiple target databases.
 
 CI builds use a different credentials file depending on the build configuration.
 Within a workflow, this avoids conflicts.
-However, there may be conflicts across workflows, as currently there is no way to prevent workflows from running in parallel.
-See https://github.community/t5/GitHub-Actions/Prevent-parallel-workflows/td-p/32889.
-
 
 How to set GitHub Actions secrets
 ---------------------------------
 
 Create environment variable files for secrets:
 
 .. prompt:: bash
```

### Comparing `vws-python-mock-2023.3.5/docs/source/conf.py` & `vws-python-mock-2023.4.8/docs/source/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,46 +2,47 @@
 """
 Configuration for Sphinx.
 """
 
 # pylint: disable=invalid-name
 
 import datetime
-
-from pkg_resources import get_distribution
+import importlib.metadata
 
 project = "VWS-Python-Mock"
 author = "Adam Dangoor"
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx_autodoc_typehints",
     "sphinx_paramlinks",
     "sphinx-prompt",
     "sphinx_substitution_extensions",
     "sphinxcontrib.spelling",
     "sphinxcontrib.autohttp.flask",
+    "sphinx_toolbox.more_autodoc.autoprotocol",
+    "enum_tools.autoenum",
 ]
 
 templates_path = ["_templates"]
 source_suffix = ".rst"
 master_doc = "index"
 
 year = datetime.datetime.now(tz=datetime.UTC).year
 project_copyright = f"{year}, {author}"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
-# Use ``pkg_resources`` as per
+# Use ``importlib.metadata.version`` as per
 # https://github.com/pypa/setuptools_scm#usage-from-sphinx.
-version = get_distribution(project).version
+version = importlib.metadata.version(distribution_name=project)
 _month, _day, _year, *_ = version.split(".")
 release = f"{_month}.{_day}.{_year}"
 
 language = "en"
 
 # The name of the syntax highlighting style to use.
 pygments_style = "sphinx"
@@ -58,15 +59,14 @@
     ),
     "docker": ("https://docker-py.readthedocs.io/en/stable", None),
 }
 nitpicky = True
 warning_is_error = True
 nitpick_ignore = [
     ("py:exc", "requests.exceptions.MissingSchema"),
-    ("http:obj", "string"),
 ]
 
 html_theme = "furo"
 html_title = project
 html_show_copyright = False
 html_show_sphinx = False
 html_show_sourcelink = False
@@ -77,15 +77,15 @@
 # Don't check anchors because many websites use #! for AJAX magic
 # http://sphinx-doc.org/config.html#confval-linkcheck_anchors
 linkcheck_anchors = False
 # Retry link checking to avoid transient network errors.
 linkcheck_retries = 5
 linkcheck_ignore = [
     # Requires login.
-    r"https://developer.vuforia.com/targetmanager",
+    "https://developer.vuforia.com/targetmanager",
 ]
 
 spelling_word_list_filename = "../../spelling_private_dict.txt"
 
 autodoc_member_order = "bysource"
 
 rst_prolog = f"""
```

### Comparing `vws-python-mock-2023.3.5/docs/source/contributing.rst` & `vws-python-mock-2023.4.8/docs/source/contributing.rst`

 * *Files 11% similar despite different names*

```diff
@@ -139,39 +139,39 @@
 
 The ``tracking_rating`` returned by ``GET /targets/<target_id>`` can be -1.
 
 The database summary from ``GET /summary`` has multiple undocumented return fields.
 
 The database summary from ``GET /summary`` is not immediately accurate.
 
-The documentation page `How To Perform an Image Recognition Query`_ states that the ``Content-Type`` header must be set to ``multipart/form-data``.
+The documentation page `Vuforia Query Web API`_ states that the ``Content-Type`` header must be set to ``multipart/form-data``.
 However, it must be set to ``multipart/form-data; boundary=<BOUNDARY>`` where ``<BOUNDARY>`` is the boundary used when encoding the form data.
 
-The documentation page `How To Perform an Image Recognition Query`_ states that ``Content-Type`` will be the only response header.
+The documentation page `Vuforia Query Web API`_ states that ``Content-Type`` will be the only response header.
 This is not the case.
 
-The documentation page `How To Perform an Image Recognition Query`_ states that 10 is the maximum allowed value of ``max_num_results``.
+The documentation page `Vuforia Query Web API`_ states that 10 is the maximum allowed value of ``max_num_results``.
 However, the maximum allowed value is 50.
 
 A response to an invalid query may have an ``application/json`` content type but include text (not JSON) data.
 
 After deleting a target, for up to approximately 30 seconds, matching it with a query returns a 500 response.
 
 A target with the name ``\uffff`` gets stuck in processing.
 
-The documentation page `How To Perform an Image Recognition Query`_ states that "The API accepts requests with unknown data fields, and ignore the unknown fields.".
+The documentation page `Vuforia Query Web API`_ states that "The API accepts requests with unknown data fields, and ignore the unknown fields.".
 This is not the case.
 
-The documentation page `How To Perform an Image Recognition Query`_ states "Maximum image size: 2.1 MPixel. 512 KiB for JPEG, 2MiB for PNG".
+The documentation page `Vuforia Query Web API`_ states "Maximum image size: 2.1 MPixel. 512 KiB for JPEG, 2MiB for PNG".
 However, JPEG images up to 2MiB are accepted.
 
 The ``request_count`` in a database summary is always ``0``.
 
 The documentation for the target summary report says "Note: tracking_rating and ``reco_rating`` are provided only when status = success.".
 However, ``reco_rating`` is never provided and ``tracking_rating`` is provided even when the status is "failed".
 
-.. _How To Perform an Image Recognition Query: https://library.vuforia.com/articles/Solution/How-To-Perform-an-Image-Recognition-Query
+.. _Vuforia Query Web API: https://library.vuforia.com/web-api/vuforia-query-web-api
 
 Release Process
 ---------------
 
 See :doc:`release-process`.
```

### Comparing `vws-python-mock-2023.3.5/docs/source/differences-to-vws.rst` & `vws-python-mock-2023.4.8/docs/source/differences-to-vws.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Differences between the mock and the real Vuforia Web Services
 ==============================================================
 
 The mock attempts to be realistic, but it was built without access to the source code of the original API.
 Please report any issues `here <https://github.com/VWS-Python/vws-python-mock/issues>`__.
-There is no attempt to make the image matching realistic.
+
+Image matching
+--------------
+
+Vuforia's image matching is proprietary and we do not intend to accurately copy it.
+Instead, we aim for simple algorithms which are fast and are good enough for testing purposes.
+The image matcher is configurable, using :paramref:`~mock_vws.MockVWS.match_checker`.
 
 Speed and summary accuracy
 --------------------------
 
 The mock responds much more quickly than the real Vuforia Web Services.
 
 Targets in the mock are set to 'processing' for half a second by default.
@@ -19,24 +25,22 @@
 The mock is accurate immediately with regards to images.
 The mock does not count recognitions.
 
 Image quality and ratings
 -------------------------
 
 Targets are assigned a rating between 0 and 5 of how good they are for tracking purposes.
-In the mock this is a random number between 0 and 5.
+In the mock this is calculated from the image quality, differently to how Vuforia does this.
+This is customizable with the :paramref:`~mock_vws.MockVWS.target_tracking_rater` parameter.
 
 Image targets which are not suited to detection are given 'failed' statuses.
 The criteria for these images is not defined by the Vuforia documentation.
 The mock is more forgiving than the real Vuforia Web Services.
 Therefore, an image given a 'success' status by the mock may not be given a 'success' status by the real Vuforia Web Services.
 
-When updating an image for a target on the real Vuforia Web Services, the rating may stay the same.
-The mock changes the rating for a target to a different random number when the image is changed.
-
 Matching targets in the processing state
 ----------------------------------------
 
 Matching a target which is in the processing state sometimes returns a successful response with no results.
 Sometimes a 500 (``INTERNAL SERVER ERROR``) response is given.
 The mock always gives a 500 response.
 
@@ -87,15 +91,15 @@
 This has error handling which is not duplicated in the mock.
 For example, Vuforia returns a 400 (``BAD REQUEST``) response if a header or cookie is given which is larger than 8 KiB.
 
 Result codes
 ------------
 
 Result codes are returned by requests to Vuforia to help with debugging.
-See `How To Interpret VWS API Result Codes <https://library.vuforia.com/articles/Solution/How-To-Use-the-Vuforia-Web-Services-API#How-To-Interperete-VWS-API-Result-Codes>`_ for details of the available result codes.
+See `VWS API Result Codes <https://library.vuforia.com/web-api/cloud-targets-web-services-api#result-codes>`_ for details of the available result codes.
 There are some result codes which the mock cannot return.
 
 These are:
 
 * ``RequestQuotaReached``
 * ``DateRangeError``
 * ``TargetQuotaReached``
```

### Comparing `vws-python-mock-2023.3.5/docs/source/docker.rst` & `vws-python-mock-2023.4.8/docs/source/docker.rst`

 * *Files 18% similar despite different names*

```diff
@@ -96,39 +96,76 @@
 
    This is required by the VWS mock and the VWQ mock containers.
    This is the route to the target manager container from the other containers.
 
 Optional configuration
 ^^^^^^^^^^^^^^^^^^^^^^
 
+Target manager container
+~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. envvar:: TARGET_RATER
+
+   The rater to use for target tracking ratings.
+
+   Options include:
+
+   * ``brisque``: The rating is derived using the BRISQUE algorithm.
+   * ``perfect``: The rating is always 5.
+   * ``random``: The rating is random.
+
+   Default: ``brisque``
+
 Query container
 ~~~~~~~~~~~~~~~
 
 .. envvar:: DELETION_PROCESSING_SECONDS
 
    The number of seconds after a target deletion is recognized that the
    query endpoint will return a 500 response on a match.
 
-   Default 3.0
+   Default: 3.0
 
 .. envvar:: DELETION_RECOGNITION_SECONDS
 
    The number of seconds after a target has been deleted that the query
    endpoint will still recognize the target for.
 
-   Default 0.2
+   Default: 2.0
+
+.. envvar:: QUERY_IMAGE_MATCHER
+
+   The matcher to use for the query endpoint.
+
+   Options include:
+
+   * ``exact``: The images must be exactly the same to match.
+   * ``average_hash``: The images must have a similar average hash to match.
+
+   Default: ``average_hash``
 
 VWS container
 ~~~~~~~~~~~~~
 
 .. envvar:: PROCESSING_TIME_SECONDS
 
    The number of seconds to process each image for.
 
-   Default 0.5
+   Default 2
+
+.. envvar:: DUPLICATES_IMAGE_MATCHER
+
+   The matcher to use for the duplicates endpoint.
+
+   Options include:
+
+   * ``exact``: The images must be exactly the same to be duplicates.
+   * ``average_hash``: The images must have a similar average hash to be duplicates.
+
+   Default: ``average_hash``
 
 Building images from source
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. prompt:: bash
 
    export REPOSITORY_ROOT=$PWD
```

### Comparing `vws-python-mock-2023.3.5/docs/source/index.rst` & `vws-python-mock-2023.4.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.3.5/lint.mk` & `vws-python-mock-2023.4.8/lint.mk`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Make commands for linting
 
 SHELL := /bin/bash -euxo pipefail
 
 .PHONY: custom-linters
 custom-linters:
-	# Running pytest needs this file
-	touch vuforia_secrets.env
 	pytest ci/custom_linters.py
 
 .PHONY: black
 black:
 	black --check .
 
 .PHONY: fix-black
@@ -34,28 +32,32 @@
 
 .PHONY: fix-ruff
 fix-ruff:
 	ruff --fix .
 
 .PHONY: pip-extra-reqs
 pip-extra-reqs:
-	pip-extra-reqs --skip-incompatible --requirements-file=requirements/requirements.txt src/
+	pip-extra-reqs --skip-incompatible --requirements-file=<(pdm export --pyproject) src/
 
 .PHONY: pip-missing-reqs
 pip-missing-reqs:
-	pip-missing-reqs --requirements-file=requirements/requirements.txt src/
+	pip-missing-reqs --requirements-file=<(pdm export --pyproject) src/
 
 .PHONY: pylint
 pylint:
 	pylint *.py src/ tests/ docs/ ci/
 
 .PHONY: pyroma
 pyroma:
 	pyroma --min 10 .
 
+.PHONY: pyright
+pyright:
+	pyright .
+
 .PHONY: vulture
 vulture:
 	vulture --min-confidence 100 --exclude _vendor --exclude .eggs .
 
 .PHONY: linkcheck
 linkcheck:
 	$(MAKE) -C docs/ linkcheck SPHINXOPTS=$(SPHINXOPTS)
```

### Comparing `vws-python-mock-2023.3.5/pyproject.toml` & `vws-python-mock-2023.4.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -88,23 +88,21 @@
 [tool.black]
 
 line-length = 79
 
 [tool.coverage.run]
 
 branch = true
-omit = [
-  "src/mock_vws/_cgi.py",
-]
 
 [tool.pytest.ini_options]
 
 xfail_strict = true
 log_cli = true
-env_files = ["./vuforia_secrets.env"]
+addopts = ["--strict-markers"]
+markers = ["requires_docker_build"]
 
 [tool.check-manifest]
 
 ignore = [
   "*.enc",
   "readthedocs.yaml",
   "CHANGELOG.rst",
@@ -117,41 +115,48 @@
   "codecov.yaml",
   "doc8.ini",
   "docs",
   "docs/**",
   ".git_archival.txt",
   "spelling_private_dict.txt",
   "tests",
-  "tests-pylintrc",
   "tests/**",
   "vuforia_secrets.env.example",
   "lint.mk",
   "src/mock_vws/_flask_server/dockerfiles/*/Dockerfile",
   "secrets.tar.gpg",
 ]
 
 [tool.mypy]
 
 strict = true
+plugins = ["pydantic.mypy"]
 
-[[tool.mypy.overrides]]
-module = [
-    "mock_vws/_cgi",
-]
-ignore_errors = true
+[tool.pydantic-mypy]
+init_forbid_extra = true
+init_typed = true
+warn_required_dynamic_aliases = true
+warn_untyped_fields = true
 
 [[tool.mypy.overrides]]
 
 module = [
+    "brisque",
+    "cv2",
     "docker",
+    "docker.errors",
     "docker.models.networks",
+    "multipart",
+    "sybil",
+    "sybil.parsers.rest",
 ]
 
 ignore_missing_imports = true
 
+# This is ignored until we can bump doc8.
 [tool.doc8]
 
 max_line_length = 2000
 ignore_path = [
     "./.eggs",
     "./docs/build",
     "./docs/build/spelling/output.txt",
@@ -166,67 +171,68 @@
 # https://github.com/pypa/setuptools_scm/issues/77 so that we do not
 # error in the Docker build stage of the release pipeline.
 #
 # This must be a PEP 440 compliant version.
 fallback_version = "0.0.0"
 
 [build-system]
-requires = ["setuptools", "pip", "wheel"]
+requires = [
+     "pip",
+     "setuptools",
+     "setuptools-scm-git-archive==1.4",
+     "setuptools_scm[toml]==7.1.0",
+     "wheel",
+ ]
 build-backend = "setuptools.build_meta"
 
 [tool.ruff]
 select = ["ALL"]
 
 ignore = [
     # We do not annotate the type of 'self', or 'cls'.
     "ANN101",
     "ANN102",
-    "ANN401",
-    # We are happy to manage our own "complexity".
-    "C901",
     # Allow our chosen docstring line-style - no one-line summary.
     "D200",
     "D203",
     "D205",
     "D212",
     "D213",
     "D400",
     "D415",
-    # Allow backslashes in a docstring.
-    # See https://click.palletsprojects.com/en/8.0.x/documentation/#preventing-rewrapping.
-    "D301",
     # It is too much work to make every docstring imperative.
     "D401",
     # We ignore some docstyle errors which do not apply to Google style
     # docstrings.
     "D406",
     "D407",
     # We have an existing interface to support and so we do not want to change
     # exception names.
     "N818",
     # Ignore "too-many-*" errors as they seem to get in the way more than
     # helping.
-    "PLR0912",
     "PLR0913",
-    "PLR0915",
-    # Allow 'assert' as we use it for tests.
+    # Allow 'assert' in tests as it is the standard for pytest.
+    # Also, allow 'assert' in other code as it is the standard for Python type hint
+    # narrowing - see
+    # https://mypy.readthedocs.io/en/stable/type_narrowing.html#type-narrowing-expressions.
     "S101",
-    # Allow imports which are only used for type checking to be outside type
-    # checking blocks.
-    "TCH001",
-    "TCH002",
-    "TCH003",
+    # Allow `random` as we are not implementing something which needs cryptographic safety.
+    "S311",
 ]
 
+# Do not automatically remove commented out code.
+# We comment out code during development, and with VSCode auto-save, this code
+# is sometimes annoyingly removed.
+unfixable = ["ERA001"]
+
 line-length = 79
 target-version = "py311"
 
 [tool.ruff.per-file-ignores]
-# Ignore copy of old stdlib cgi module.
-"src/mock_vws/_cgi.py" = ["ALL"]
 "tests/**" = [
     # Allow possible hardcoded passwords in tests.
     "S105",
     "S106",
 ]
 
 [tool.distutils.bdist_wheel]
@@ -245,21 +251,81 @@
 description = "A mock for the Vuforia Web Services (VWS) API."
 dynamic = ["version"]
 keywords = ["vuforia", "vws", "mock", "fake", "client"]
 license = { file = "LICENSE" }
 name = "vws-python-mock"
 readme = { file = "README.rst", content-type = "text/x-rst"}
 requires-python = ">=3.10"
+dependencies = [
+    "ImageHash",
+    "Pillow",
+    "brisque",
+    "flask",
+    "multipart",
+    "numpy",
+    "opencv-python",
+    "pydantic",
+    "requests",
+    "requests-mock",
+    "tzdata; sys_platform == 'win32'",
+    "vws-auth-tools",
+    "werkzeug",
+]
+
+[project.optional-dependencies]
+dev = [
+    "PyYAML==6.0",
+    "Sphinx-Substitution-Extensions==2022.2.16",
+    "Sphinx==6.1.3",
+    "VWS-Test-Fixtures==2023.3.5",
+    "black==23.3.0",
+    "check-manifest==0.49",
+    "dirty-equals==0.5.0",
+    # We pin to an old doc8 to avoid version conflicts with sphinx_toolbox.
+    # When we bump this, we can remove doc8.ini.
+    "doc8==0.11.2",
+    "docker==6.0.1",
+    "dodgy==0.2.1",
+    "enum-tools[sphinx]==0.9.0.post1",
+    "freezegun==1.2.2",
+    "furo==2023.3.27",
+    "mypy==1.2.0",
+    "pdm==2.4.9",
+    "pip_check_reqs==2.4.4",
+    "pydocstyle==6.3.0",
+    "pyenchant==3.2.2",
+    "pylint==2.17.2",
+    "pyright==1.1.302",
+    "pyroma==4.2",
+    "pytest-cov==4.0.0",
+    "pytest==7.2.2",
+    "requests-mock-flask==2023.3.5.1",
+    "ruff==0.0.261",
+    "sphinx-autodoc-typehints==1.22",
+    "sphinx-prompt==1.5.0",
+    "sphinx_paramlinks==0.5.4",
+    "sphinxcontrib-httpdomain==1.8.1",
+    "sphinxcontrib-spelling==8.0.0",
+    "sphinx-toolbox==3.4.0",
+    "sybil==5.0.0",
+    "types-PyYAML==6.0.12.9",
+    "types-Pillow==9.4.0.19",
+    "types-requests==2.28.11.17",
+    "types-urllib3==1.26.25.10",
+    "vulture==2.7",
+    "vws-python==2023.3.25",
+]
 
 [project.urls]
 Source = "https://github.com/VWS-Python/vws-python-mock"
 Documentation = "https://vws-python-mock.readthedocs.io"
 
 [tool.setuptools]
 zip-safe = false
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
 mock_vws = ["py.typed"]
 
+[tool.pyright]
```

### Comparing `vws-python-mock-2023.3.5/secrets.tar.gpg` & `vws-python-mock-2023.4.8/secrets.tar.gpg`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.3.5/spelling_private_dict.txt` & `vws-python-mock-2023.4.8/spelling_private_dict.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 KiB
 MPixel
 MiB
 MissingSchema
 Ubuntu
 admin
+another's
 api
 args
 ascii
 auth
 backend
 backends
 binascii
@@ -31,14 +32,15 @@
 exc
 filename
 foo
 formdata
 github
 greyscale
 gzip
+hardcoded
 hexdigits
 hmac
 html
 http
 https
 iff
 io
@@ -49,14 +51,16 @@
 kib
 kwargs
 learnings
 linters
 linting
 login
 macOS
+matcher
+matchers
 mb
 metadata
 mib
 mockvws
 multipart
 mypy
 nat
@@ -64,14 +68,15 @@
 outerboundary
 overridable
 pdict
 plugins
 png
 pragma
 processable
+pyright
 pytest
 readme
 readthedocs
 recognitions
 refactoring
 regex
 reimplementation
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_base64_decoding.py` & `vws-python-mock-2023.4.8/src/mock_vws/_base64_decoding.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 def decode_base64(encoded_data: str) -> bytes:
     """
     Decode base64 somewhat like Vuforia does.
 
     Raises:
         binascii.Error: Vuforia would consider this encoded data as an
-        "UNPROCESSABLE_ENTITY".
+          "UNPROCESSABLE_ENTITY".
 
     Returns:
         The given data, decoded as base64.
     """
     acceptable_characters = string.ascii_letters + string.digits + "+/="
     for character in encoded_data:
         if character not in acceptable_characters:
             raise binascii.Error
 
-    mod_4_result_to_modified_encoded_data = {
+    mod_four_result_to_modified_encoded_data = {
         0: encoded_data,
         1: encoded_data[:-1],
-        2: encoded_data + "==",
-        3: encoded_data + "=",
+        2: f"{encoded_data}==",
+        3: f"{encoded_data}=",
     }
-    modified_encoded_data = mod_4_result_to_modified_encoded_data[
+    modified_encoded_data = mod_four_result_to_modified_encoded_data[
         len(encoded_data) % 4
     ]
     return base64.b64decode(modified_encoded_data)
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_constants.py` & `vws-python-mock-2023.4.8/src/mock_vws/_constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 class ResultCodes(Enum):
     """
     Constants representing various VWS result codes.
 
     See
-    https://library.vuforia.com/articles/Solution/How-To-Use-the-Vuforia-Web-Services-API.html#How-To-Interperete-VWS-API-Result-Codes
+    https://library.vuforia.com/web-api/cloud-targets-web-services-api#result-codes.
 
     Some codes here are not documented in the above link.
     """
 
     SUCCESS = "Success"
     TARGET_CREATED = "TargetCreated"
     AUTHENTICATION_FAILURE = "AuthenticationFailure"
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_database_matchers.py` & `vws-python-mock-2023.4.8/src/mock_vws/_database_matchers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Helpers for getting databases which match keys given in requests.
 """
 
 from __future__ import annotations
 
-from collections.abc import Iterable
+from typing import TYPE_CHECKING
 
 from vws_auth_tools import authorization_header
 
-from mock_vws.database import VuforiaDatabase
+if TYPE_CHECKING:
+    from collections.abc import Iterable
+
+    from mock_vws.database import VuforiaDatabase
 
 
 def get_database_matching_client_keys(
     request_headers: dict[str, str],
     request_body: bytes | None,
     request_method: str,
     request_path: str,
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_flask_server/target_manager.py` & `vws-python-mock-2023.4.8/src/mock_vws/_flask_server/target_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,100 @@
 """
 Storage layer for the mock Vuforia Flask application.
 """
 
 import base64
 import dataclasses
 import datetime
-import os
-import random
+import json
+from enum import StrEnum, auto
 from http import HTTPStatus
 from zoneinfo import ZoneInfo
 
-from flask import Flask, jsonify, request
+from flask import Flask, Response, request
+from pydantic import BaseSettings
 
 from mock_vws.database import VuforiaDatabase
 from mock_vws.states import States
 from mock_vws.target import Target
 from mock_vws.target_manager import TargetManager
+from mock_vws.target_raters import (
+    BrisqueTargetTrackingRater,
+    HardcodedTargetTrackingRater,
+    RandomTargetTrackingRater,
+    TargetTrackingRater,
+)
 
 TARGET_MANAGER_FLASK_APP = Flask(__name__)
 
 TARGET_MANAGER = TargetManager()
 
 
+class _TargetRaterChoice(StrEnum):
+    """Target rater choices."""
+
+    BRISQUE = auto()
+    PERFECT = auto()
+    RANDOM = auto()
+
+    def to_target_rater(self) -> TargetTrackingRater:
+        """Get the target rater."""
+        rater = {
+            _TargetRaterChoice.BRISQUE: BrisqueTargetTrackingRater(),
+            _TargetRaterChoice.PERFECT: HardcodedTargetTrackingRater(rating=5),
+            _TargetRaterChoice.RANDOM: RandomTargetTrackingRater(),
+        }[self]
+        assert isinstance(rater, TargetTrackingRater)
+        return rater
+
+
+class TargetManagerSettings(BaseSettings):
+    """Settings for the Target Manager Flask app."""
+
+    target_manager_host: str = ""
+    target_rater: _TargetRaterChoice = _TargetRaterChoice.BRISQUE
+
+
 @TARGET_MANAGER_FLASK_APP.route(
     "/databases/<string:database_name>",
     methods=["DELETE"],
 )
-def delete_database(database_name: str) -> tuple[str, int]:
+def delete_database(database_name: str) -> Response:
     """
     Delete a database.
 
     :status 200: The database has been deleted.
     """
     try:
         (matching_database,) = {
             database
             for database in TARGET_MANAGER.databases
             if database_name == database.database_name
         }
     except ValueError:
-        return "", HTTPStatus.NOT_FOUND
+        return Response(response="", status=HTTPStatus.NOT_FOUND)
 
     TARGET_MANAGER.remove_database(database=matching_database)
-    return "", HTTPStatus.OK
+    return Response(response="", status=HTTPStatus.OK)
 
 
 @TARGET_MANAGER_FLASK_APP.route("/databases", methods=["GET"])
-def get_databases() -> tuple[str, int]:
+def get_databases() -> Response:
     """
     Return a list of all databases.
     """
     databases = [database.to_dict() for database in TARGET_MANAGER.databases]
-    return jsonify(databases), HTTPStatus.OK
+    return Response(
+        response=json.dumps(obj=databases),
+        status=HTTPStatus.OK,
+    )
 
 
 @TARGET_MANAGER_FLASK_APP.route("/databases", methods=["POST"])
-def create_database() -> tuple[str, int]:
+def create_database() -> Response:
     """
     Create a new database.
 
     :reqheader Content-Type: application/json
     :resheader Content-Type: application/json
 
     :reqjson string client_access_key: (Optional) The client access key for the
@@ -82,35 +117,36 @@
     :resjson string state_name: The database state. This will be "WORKING" or
       "PROJECT_INACTIVE".
     :reqjsonarr targets: The targets in the database.
 
     :status 201: The database has been successfully created.
     """
     random_database = VuforiaDatabase()
-    server_access_key = request.json.get(
+    request_json = json.loads(request.data)
+    server_access_key = request_json.get(
         "server_access_key",
         random_database.server_access_key,
     )
-    server_secret_key = request.json.get(
+    server_secret_key = request_json.get(
         "server_secret_key",
         random_database.server_secret_key,
     )
-    client_access_key = request.json.get(
+    client_access_key = request_json.get(
         "client_access_key",
         random_database.client_access_key,
     )
-    client_secret_key = request.json.get(
+    client_secret_key = request_json.get(
         "client_secret_key",
         random_database.client_secret_key,
     )
-    database_name = request.json.get(
+    database_name = request_json.get(
         "database_name",
         random_database.database_name,
     )
-    state_name = request.json.get(
+    state_name = request_json.get(
         "state_name",
         random_database.state.name,
     )
 
     state = States[state_name]
 
     database = VuforiaDatabase(
@@ -120,120 +156,133 @@
         client_secret_key=client_secret_key,
         database_name=database_name,
         state=state,
     )
     try:
         TARGET_MANAGER.add_database(database=database)
     except ValueError as exc:
-        return str(exc), HTTPStatus.CONFLICT
-
-    return jsonify(database.to_dict()), HTTPStatus.CREATED
+        return Response(
+            response=str(exc),
+            status=HTTPStatus.CONFLICT,
+        )
+
+    return Response(
+        response=json.dumps(database.to_dict()),
+        status=HTTPStatus.CREATED,
+    )
 
 
 @TARGET_MANAGER_FLASK_APP.route(
     "/databases/<string:database_name>/targets",
     methods=["POST"],
 )
-def create_target(database_name: str) -> tuple[str, int]:
+def create_target(database_name: str) -> Response:
     """
     Create a new target in a given database.
     """
-    [database] = [
+    (database,) = (
         database
         for database in TARGET_MANAGER.databases
         if database.database_name == database_name
-    ]
-    image_base64 = request.json["image_base64"]
-    image_bytes = base64.b64decode(image_base64)
+    )
+    request_json = json.loads(request.data)
+    image_base64 = request_json["image_base64"]
+    image_bytes = base64.b64decode(s=image_base64)
+    settings = TargetManagerSettings.parse_obj(obj={})
+    target_tracking_rater = settings.target_rater.to_target_rater()
+
     target = Target(
-        name=request.json["name"],
-        width=request.json["width"],
+        name=request_json["name"],
+        width=request_json["width"],
         image_value=image_bytes,
-        active_flag=request.json["active_flag"],
-        processing_time_seconds=request.json["processing_time_seconds"],
-        application_metadata=request.json["application_metadata"],
-        target_id=request.json["target_id"],
+        active_flag=request_json["active_flag"],
+        processing_time_seconds=request_json["processing_time_seconds"],
+        application_metadata=request_json["application_metadata"],
+        target_id=request_json["target_id"],
+        target_tracking_rater=target_tracking_rater,
     )
     database.targets.add(target)
 
-    return jsonify(target.to_dict()), HTTPStatus.CREATED
+    return Response(
+        response=json.dumps(target.to_dict()),
+        status=HTTPStatus.CREATED,
+    )
 
 
 @TARGET_MANAGER_FLASK_APP.route(
     "/databases/<string:database_name>/targets/<string:target_id>",
     methods=["DELETE"],
 )
-def delete_target(database_name: str, target_id: str) -> tuple[str, int]:
+def delete_target(database_name: str, target_id: str) -> Response:
     """
     Delete a target.
     """
-    [database] = [
+    (database,) = (
         database
         for database in TARGET_MANAGER.databases
         if database.database_name == database_name
-    ]
+    )
     target = database.get_target(target_id=target_id)
     now = datetime.datetime.now(tz=target.upload_date.tzinfo)
     new_target = dataclasses.replace(target, delete_date=now)
     database.targets.remove(target)
     database.targets.add(new_target)
-    return jsonify(new_target.to_dict()), HTTPStatus.OK
+    return Response(
+        response=json.dumps(new_target.to_dict()),
+        status=HTTPStatus.OK,
+    )
 
 
 @TARGET_MANAGER_FLASK_APP.route(
     "/databases/<string:database_name>/targets/<string:target_id>",
     methods=["PUT"],
 )
-def update_target(database_name: str, target_id: str) -> tuple[str, int]:
+def update_target(database_name: str, target_id: str) -> Response:
     """
     Update a target.
     """
-    [database] = [
+    (database,) = (
         database
         for database in TARGET_MANAGER.databases
         if database.database_name == database_name
-    ]
+    )
     target = database.get_target(target_id=target_id)
 
-    width = request.json.get("width", target.width)
-    name = request.json.get("name", target.name)
-    active_flag = request.json.get("active_flag", target.active_flag)
-    application_metadata = request.json.get(
+    request_json = json.loads(request.data)
+    width = request_json.get("width", target.width)
+    name = request_json.get("name", target.name)
+    active_flag = request_json.get("active_flag", target.active_flag)
+    application_metadata = request_json.get(
         "application_metadata",
         target.application_metadata,
     )
 
     image_value = target.image_value
-    if "image" in request.json:
-        image_value = base64.b64decode(request.json["image"])
-
-    # In the real implementation, the tracking rating can stay the same.
-    # However, for demonstration purposes, the tracking rating changes but
-    # when the target is updated.
-    available_values = list(set(range(6)) - {target.tracking_rating})
-    processed_tracking_rating = random.choice(available_values)
+    request_json = json.loads(request.data)
+    if "image" in request_json:
+        image_value = base64.b64decode(s=request_json["image"])
 
     gmt = ZoneInfo("GMT")
     last_modified_date = datetime.datetime.now(tz=gmt)
 
     new_target = dataclasses.replace(
         target,
         name=name,
         width=width,
         active_flag=active_flag,
         application_metadata=application_metadata,
         image_value=image_value,
-        processed_tracking_rating=processed_tracking_rating,
         last_modified_date=last_modified_date,
     )
 
     database.targets.remove(target)
     database.targets.add(new_target)
 
-    return jsonify(new_target.to_dict()), HTTPStatus.OK
+    return Response(
+        response=json.dumps(new_target.to_dict()),
+        status=HTTPStatus.OK,
+    )
 
 
 if __name__ == "__main__":  # pragma: no cover
-    TARGET_MANAGER_FLASK_APP.run(
-        debug=True,
-        host=os.environ["TARGET_MANAGER_HOST"],
-    )
+    SETTINGS = TargetManagerSettings.parse_obj(obj={})
+    TARGET_MANAGER_FLASK_APP.run(host=SETTINGS.target_manager_host)
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_flask_server/vwq.py` & `vws-python-mock-2023.4.8/src/mock_vws/_flask_server/vwq.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,76 @@
 """
 A fake implementation of the Vuforia Web Query API using Flask.
 
 See
-https://library.vuforia.com/articles/Solution/How-To-Perform-an-Image-Recognition-Query
+https://library.vuforia.com/web-api/vuforia-query-web-api
 """
 
 import email.utils
-import os
+from enum import StrEnum, auto
 from http import HTTPStatus
 
 import requests
 from flask import Flask, Response, request
+from pydantic import BaseSettings
+from werkzeug.datastructures import Headers
 
 from mock_vws._query_tools import (
     ActiveMatchingTargetsDeleteProcessing,
     get_query_match_response_text,
 )
 from mock_vws._query_validators import run_query_validators
 from mock_vws._query_validators.exceptions import (
     DeletedTargetMatched,
     ValidatorException,
 )
 from mock_vws.database import VuforiaDatabase
+from mock_vws.image_matchers import (
+    AverageHashMatcher,
+    ExactMatcher,
+    ImageMatcher,
+)
 
 CLOUDRECO_FLASK_APP = Flask(import_name=__name__)
 CLOUDRECO_FLASK_APP.config["PROPAGATE_EXCEPTIONS"] = True
 
 
+class _ImageMatcherChoice(StrEnum):
+    """Image matcher choices."""
+
+    EXACT = auto()
+    AVERAGE_HASH = auto()
+
+    def to_image_matcher(self) -> ImageMatcher:
+        """Get the image matcher."""
+        matcher = {
+            _ImageMatcherChoice.EXACT: ExactMatcher(),
+            _ImageMatcherChoice.AVERAGE_HASH: AverageHashMatcher(threshold=10),
+        }[self]
+        assert isinstance(matcher, ImageMatcher)
+        return matcher
+
+
+class VWQSettings(BaseSettings):
+    """Settings for the VWQ Flask app."""
+
+    vwq_host: str = ""
+    target_manager_base_url: str
+    deletion_processing_seconds: float = 3.0
+    deletion_recognition_seconds: float = 2.0
+    query_image_matcher: _ImageMatcherChoice = _ImageMatcherChoice.AVERAGE_HASH
+
+
 def get_all_databases() -> set[VuforiaDatabase]:
     """
     Get all database objects from the target manager back-end.
     """
-    target_manager_base_url = os.environ["TARGET_MANAGER_BASE_URL"]
+    settings = VWQSettings.parse_obj(obj={})
     response = requests.get(
-        url=f"{target_manager_base_url}/databases",
+        url=f"{settings.target_manager_base_url}/databases",
         timeout=30,
     )
     return {
         VuforiaDatabase.from_dict(database_dict=database_dict)
         for database_dict in response.json()
     }
 
@@ -60,51 +93,36 @@
     terminate_wsgi_input = CLOUDRECO_FLASK_APP.config.get(
         "TERMINATE_WSGI_INPUT",
         False,
     )
     request.environ["wsgi.input_terminated"] = terminate_wsgi_input
 
 
-class ResponseNoContentTypeAdded(Response):
-    """
-    A custom response type.
-
-    Without this, a content type is added to all responses.
-    Some of our responses need to not have a "Content-Type" header.
-    """
-
-    default_mimetype = None
-
-
-CLOUDRECO_FLASK_APP.response_class = ResponseNoContentTypeAdded
-
-
 @CLOUDRECO_FLASK_APP.errorhandler(ValidatorException)
 def handle_exceptions(exc: ValidatorException) -> Response:
     """
     Return the error response associated with the given exception.
     """
-    return ResponseNoContentTypeAdded(
+    response = Response(
         status=exc.status_code.value,
         response=exc.response_text,
         headers=exc.headers,
     )
 
+    response.headers = Headers(exc.headers)
+    return response
+
 
 @CLOUDRECO_FLASK_APP.route("/v1/query", methods=["POST"])
 def query() -> Response:
     """
     Perform an image recognition query.
     """
-    query_processes_deletion_seconds = float(
-        os.environ.get("DELETION_PROCESSING_SECONDS", "3.0"),
-    )
-    query_recognizes_deletion_seconds = float(
-        os.environ.get("DELETION_RECOGNITION_SECONDS", "0.2"),
-    )
+    settings = VWQSettings.parse_obj(obj={})
+    query_match_checker = settings.query_image_matcher.to_image_matcher()
 
     databases = get_all_databases()
     request_body = request.stream.read()
     run_query_validators(
         request_headers=dict(request.headers),
         request_body=request_body,
         request_method=request.method,
@@ -116,18 +134,19 @@
     try:
         response_text = get_query_match_response_text(
             request_headers=dict(request.headers),
             request_body=request_body,
             request_method=request.method,
             request_path=request.path,
             databases=databases,
-            query_processes_deletion_seconds=query_processes_deletion_seconds,
+            query_processes_deletion_seconds=settings.deletion_processing_seconds,
             query_recognizes_deletion_seconds=(
-                query_recognizes_deletion_seconds
+                settings.deletion_recognition_seconds
             ),
+            query_match_checker=query_match_checker,
         )
     except ActiveMatchingTargetsDeleteProcessing as exc:
         raise DeletedTargetMatched from exc
 
     headers = {
         "Content-Type": "application/json",
         "Date": date,
@@ -138,8 +157,9 @@
         status=HTTPStatus.OK,
         response=response_text,
         headers=headers,
     )
 
 
 if __name__ == "__main__":  # pragma: no cover
-    CLOUDRECO_FLASK_APP.run(debug=True, host=os.environ["VWQ_HOST"])
+    SETTINGS = VWQSettings.parse_obj(obj={})
+    CLOUDRECO_FLASK_APP.run(host=SETTINGS.vwq_host)
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_flask_server/vws.py` & `vws-python-mock-2023.4.8/src/mock_vws/_flask_server/vws.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,67 +4,95 @@
 See
 https://library.vuforia.com/articles/Solution/How-To-Use-the-Vuforia-Web-Services-API
 """
 
 import base64
 import email.utils
 import json
-import os
+import logging
 import uuid
+from enum import StrEnum, auto
 from http import HTTPStatus
 
 import requests
 from flask import Flask, Response, request
+from pydantic import BaseSettings
+from werkzeug.datastructures import Headers
 
 from mock_vws._constants import ResultCodes, TargetStatuses
 from mock_vws._database_matchers import get_database_matching_server_keys
 from mock_vws._mock_common import json_dump
 from mock_vws._services_validators import run_services_validators
 from mock_vws._services_validators.exceptions import (
     Fail,
     TargetStatusNotSuccess,
     TargetStatusProcessing,
     ValidatorException,
 )
 from mock_vws.database import VuforiaDatabase
+from mock_vws.image_matchers import (
+    AverageHashMatcher,
+    ExactMatcher,
+    ImageMatcher,
+)
 from mock_vws.target import Target
+from mock_vws.target_raters import (
+    HardcodedTargetTrackingRater,
+)
 
 VWS_FLASK_APP = Flask(import_name=__name__)
 VWS_FLASK_APP.config["PROPAGATE_EXCEPTIONS"] = True
 
 
+_LOGGER = logging.getLogger(__name__)
+
+
+class _ImageMatcherChoice(StrEnum):
+    """Image matcher choices."""
+
+    EXACT = auto()
+    AVERAGE_HASH = auto()
+
+    def to_image_matcher(self) -> ImageMatcher:
+        """Get the image matcher."""
+        matcher = {
+            _ImageMatcherChoice.EXACT: ExactMatcher(),
+            _ImageMatcherChoice.AVERAGE_HASH: AverageHashMatcher(threshold=10),
+        }[self]
+        assert isinstance(matcher, ImageMatcher)
+        return matcher
+
+
+class VWSSettings(BaseSettings):
+    """Settings for the VWS Flask app."""
+
+    target_manager_base_url: str
+    processing_time_seconds: float = 2
+    vws_host: str = ""
+    duplicates_image_matcher: _ImageMatcherChoice = (
+        _ImageMatcherChoice.AVERAGE_HASH
+    )
+
+
 def get_all_databases() -> set[VuforiaDatabase]:
     """
     Get all database objects from the task manager back-end.
     """
-    target_manager_base_url = os.environ["TARGET_MANAGER_BASE_URL"]
+    settings = VWSSettings.parse_obj(obj={})
+    timeout_seconds = 30
     response = requests.get(
-        url=f"{target_manager_base_url}/databases",
-        timeout=30,
+        url=f"{settings.target_manager_base_url}/databases",
+        timeout=timeout_seconds,
     )
     return {
         VuforiaDatabase.from_dict(database_dict=database_dict)
         for database_dict in response.json()
     }
 
 
-class ResponseNoContentTypeAdded(Response):
-    """
-    A custom response type.
-
-    Without this, a content type is added to all responses.
-    Some of our responses need to not have a "Content-Type" header.
-    """
-
-    default_mimetype = None
-
-
-VWS_FLASK_APP.response_class = ResponseNoContentTypeAdded
-
-
 @VWS_FLASK_APP.before_request
 def set_terminate_wsgi_input() -> None:
     """
     We set ``wsgi.input_terminated`` to ``True`` when going through
     ``requests``, so that requests have the given ``Content-Length`` headers
     and the given data in ``request.headers`` and ``request.data``.
 
@@ -99,32 +127,33 @@
 
 
 @VWS_FLASK_APP.errorhandler(ValidatorException)
 def handle_exceptions(exc: ValidatorException) -> Response:
     """
     Return the error response associated with the given exception.
     """
-    return ResponseNoContentTypeAdded(
+    response = Response(
         status=exc.status_code.value,
         response=exc.response_text,
         headers=exc.headers,
     )
 
+    response.headers = Headers(exc.headers)
+    return response
+
 
 @VWS_FLASK_APP.route("/targets", methods=["POST"])
 def add_target() -> Response:
     """
     Add a target.
 
     Fake implementation of
     https://library.vuforia.com/articles/Solution/How-To-Use-the-Vuforia-Web-Services-API.html#How-To-Add-a-Target
     """
-    processing_time_seconds = float(
-        os.environ.get("PROCESSING_TIME_SECONDS", "0.5"),
-    )
+    settings = VWSSettings.parse_obj(obj={})
     databases = get_all_databases()
     database = get_database_matching_server_keys(
         request_headers=dict(request.headers),
         request_body=request.data,
         request_method=request.method,
         request_path=request.path,
         databases=databases,
@@ -136,38 +165,44 @@
     # when the content type is given as ``application/json``.
     request_json = json.loads(request.data)
     name = request_json["name"]
     active_flag = request_json.get("active_flag")
     if active_flag is None:
         active_flag = True
 
+    # This rater is not used.
+    target_tracking_rater = HardcodedTargetTrackingRater(rating=1)
+
     new_target = Target(
         name=name,
         width=request_json["width"],
         image_value=base64.b64decode(request_json["image"]),
         active_flag=active_flag,
-        processing_time_seconds=processing_time_seconds,
+        processing_time_seconds=settings.processing_time_seconds,
         application_metadata=request_json.get("application_metadata"),
+        target_tracking_rater=target_tracking_rater,
     )
 
-    target_manager_base_url = os.environ["TARGET_MANAGER_BASE_URL"]
-    databases_url = f"{target_manager_base_url}/databases"
+    databases_url = f"{settings.target_manager_base_url}/databases"
+    timeout_seconds = 30
     requests.post(
         url=f"{databases_url}/{database.database_name}/targets",
         json=new_target.to_dict(),
-        timeout=30,
+        timeout=timeout_seconds,
     )
 
     date = email.utils.formatdate(None, localtime=False, usegmt=True)
     headers = {
         "content-type": "application/json",
         "server": "envoy",
         "date": date,
-        "x-aws-region": "us-west-2, eu-west-1",
         "x-envoy-upstream-service-time": "5",
+        "strict-transport-security": "max-age=31536000",
+        "x-aws-region": "us-east-2, us-west-2",
+        "x-content-type-options": "nosniff",
     }
 
     body = {
         "transaction_id": uuid.uuid4().hex,
         "result_code": ResultCodes.TARGET_CREATED.value,
         "target_id": new_target.target_id,
     }
@@ -193,17 +228,17 @@
         request_body=request.data,
         request_method=request.method,
         request_path=request.path,
         databases=databases,
     )
 
     assert isinstance(database, VuforiaDatabase)
-    [target] = [
+    (target,) = (
         target for target in database.targets if target.target_id == target_id
-    ]
+    )
 
     target_record = {
         "target_id": target.target_id,
         "active_flag": target.active_flag,
         "name": target.name,
         "width": target.width,
         "tracking_rating": target.tracking_rating,
@@ -211,16 +246,18 @@
     }
 
     date = email.utils.formatdate(None, localtime=False, usegmt=True)
     headers = {
         "content-type": "application/json",
         "server": "envoy",
         "date": date,
-        "x-aws-region": "us-west-2, eu-west-1",
         "x-envoy-upstream-service-time": "5",
+        "strict-transport-security": "max-age=31536000",
+        "x-aws-region": "us-east-2, us-west-2",
+        "x-content-type-options": "nosniff",
     }
     body = {
         "result_code": ResultCodes.SUCCESS.value,
         "transaction_id": uuid.uuid4().hex,
         "target_record": target_record,
         "status": target.status,
     }
@@ -235,49 +272,51 @@
 def delete_target(target_id: str) -> Response:
     """
     Delete a target.
 
     Fake implementation of
     https://library.vuforia.com/articles/Solution/How-To-Use-the-Vuforia-Web-Services-API.html#How-To-Delete-a-Target
     """
+    settings = VWSSettings.parse_obj(obj={})
     databases = get_all_databases()
     database = get_database_matching_server_keys(
         request_headers=dict(request.headers),
         request_body=request.data,
         request_method=request.method,
         request_path=request.path,
         databases=databases,
     )
 
     assert isinstance(database, VuforiaDatabase)
-    [target] = [
+    (target,) = (
         target for target in database.targets if target.target_id == target_id
-    ]
+    )
 
     if target.status == TargetStatuses.PROCESSING.value:
         raise TargetStatusProcessing
 
-    target_manager_base_url = os.environ["TARGET_MANAGER_BASE_URL"]
-    databases_url = f"{target_manager_base_url}/databases"
+    databases_url = f"{settings.target_manager_base_url}/databases"
     requests.delete(
         url=f"{databases_url}/{database.database_name}/targets/{target_id}",
         timeout=30,
     )
 
     body = {
         "transaction_id": uuid.uuid4().hex,
         "result_code": ResultCodes.SUCCESS.value,
     }
     date = email.utils.formatdate(None, localtime=False, usegmt=True)
     headers = {
         "content-type": "application/json",
         "server": "envoy",
         "date": date,
-        "x-aws-region": "us-west-2, eu-west-1",
         "x-envoy-upstream-service-time": "5",
+        "strict-transport-security": "max-age=31536000",
+        "x-aws-region": "us-east-2, us-west-2",
+        "x-content-type-options": "nosniff",
     }
     return Response(
         status=HTTPStatus.OK,
         response=json_dump(body),
         headers=headers,
     )
 
@@ -319,16 +358,18 @@
         "request_usage": 0,
     }
     date = email.utils.formatdate(None, localtime=False, usegmt=True)
     headers = {
         "content-type": "application/json",
         "server": "envoy",
         "date": date,
-        "x-aws-region": "us-west-2, eu-west-1",
         "x-envoy-upstream-service-time": "5",
+        "strict-transport-security": "max-age=31536000",
+        "x-aws-region": "us-east-2, us-west-2",
+        "x-content-type-options": "nosniff",
     }
     return Response(
         status=HTTPStatus.OK,
         response=json_dump(body),
         headers=headers,
     )
 
@@ -347,17 +388,17 @@
         request_body=request.data,
         request_method=request.method,
         request_path=request.path,
         databases=databases,
     )
 
     assert isinstance(database, VuforiaDatabase)
-    [target] = [
+    (target,) = (
         target for target in database.targets if target.target_id == target_id
-    ]
+    )
     body = {
         "status": target.status,
         "transaction_id": uuid.uuid4().hex,
         "result_code": ResultCodes.SUCCESS.value,
         "database_name": database.database_name,
         "target_name": target.name,
         "upload_date": target.upload_date.strftime("%Y-%m-%d"),
@@ -368,16 +409,18 @@
         "previous_month_recos": target.previous_month_recos,
     }
     date = email.utils.formatdate(None, localtime=False, usegmt=True)
     headers = {
         "content-type": "application/json",
         "server": "envoy",
         "date": date,
-        "x-aws-region": "us-west-2, eu-west-1",
         "x-envoy-upstream-service-time": "5",
+        "strict-transport-security": "max-age=31536000",
+        "x-aws-region": "us-east-2, us-west-2",
+        "x-content-type-options": "nosniff",
     }
     return Response(
         status=HTTPStatus.OK,
         response=json_dump(body),
         headers=headers,
     )
 
@@ -387,33 +430,38 @@
     """
     Get targets which may be considered duplicates of a given target.
 
     Fake implementation of
     https://library.vuforia.com/articles/Solution/How-To-Use-the-Vuforia-Web-Services-API.html#How-To-Check-for-Duplicate-Targets
     """
     databases = get_all_databases()
+    settings = VWSSettings.parse_obj(obj={})
     database = get_database_matching_server_keys(
         request_headers=dict(request.headers),
         request_body=request.data,
         request_method=request.method,
         request_path=request.path,
         databases=databases,
     )
+    image_match_checker = settings.duplicates_image_matcher.to_image_matcher()
 
     assert isinstance(database, VuforiaDatabase)
-    [target] = [
+    (target,) = (
         target for target in database.targets if target.target_id == target_id
-    ]
-    other_targets = set(database.targets) - {target}
+    )
+    other_targets = database.targets - {target}
 
     similar_targets: list[str] = [
         other.target_id
         for other in other_targets
-        if other.image_value == target.image_value
-        and TargetStatuses.FAILED.value not in (target.status, other.status)
+        if image_match_checker(
+            first_image_content=target.image_value,
+            second_image_content=other.image_value,
+        )
+        and TargetStatuses.FAILED.value not in {target.status, other.status}
         and TargetStatuses.PROCESSING.value != other.status
         and other.active_flag
     ]
 
     body = {
         "transaction_id": uuid.uuid4().hex,
         "result_code": ResultCodes.SUCCESS.value,
@@ -421,16 +469,18 @@
     }
 
     date = email.utils.formatdate(None, localtime=False, usegmt=True)
     headers = {
         "content-type": "application/json",
         "server": "envoy",
         "date": date,
-        "x-aws-region": "us-west-2, eu-west-1",
         "x-envoy-upstream-service-time": "5",
+        "strict-transport-security": "max-age=31536000",
+        "x-aws-region": "us-east-2, us-west-2",
+        "x-content-type-options": "nosniff",
     }
     return Response(
         status=HTTPStatus.OK,
         response=json_dump(body),
         headers=headers,
     )
 
@@ -460,16 +510,18 @@
         "results": results,
     }
     date = email.utils.formatdate(None, localtime=False, usegmt=True)
     headers = {
         "content-type": "application/json",
         "server": "envoy",
         "date": date,
-        "x-aws-region": "us-west-2, eu-west-1",
         "x-envoy-upstream-service-time": "5",
+        "strict-transport-security": "max-age=31536000",
+        "x-aws-region": "us-east-2, us-west-2",
+        "x-content-type-options": "nosniff",
     }
     return Response(
         status=HTTPStatus.OK,
         response=json_dump(body),
         headers=headers,
     )
 
@@ -478,79 +530,94 @@
 def update_target(target_id: str) -> Response:
     """
     Update a target.
 
     Fake implementation of
     https://library.vuforia.com/articles/Solution/How-To-Use-the-Vuforia-Web-Services-API.html#How-To-Update-a-Target
     """
+    settings = VWSSettings.parse_obj(obj={})
     # We do not use ``request.get_json(force=True)`` because this only works
     # when the content type is given as ``application/json``.
     request_json = json.loads(request.data)
     databases = get_all_databases()
     database = get_database_matching_server_keys(
         request_headers=dict(request.headers),
         request_body=request.data,
         request_method=request.method,
         request_path=request.path,
         databases=databases,
     )
 
     assert isinstance(database, VuforiaDatabase)
-    [target] = [
+    (target,) = (
         target for target in database.targets if target.target_id == target_id
-    ]
+    )
 
     if target.status != TargetStatuses.SUCCESS.value:
         raise TargetStatusNotSuccess
 
     update_values = {}
     if "width" in request_json:
         update_values["width"] = request_json["width"]
 
     if "active_flag" in request_json:
         active_flag = request_json["active_flag"]
         if active_flag is None:
+            _LOGGER.warning(
+                msg=(
+                    'The value of "active_flag" was None. '
+                    "This is not allowed. "
+                ),
+            )
             raise Fail(status_code=HTTPStatus.BAD_REQUEST)
         update_values["active_flag"] = active_flag
 
     if "application_metadata" in request_json:
         application_metadata = request_json["application_metadata"]
         if application_metadata is None:
+            _LOGGER.warning(
+                msg=(
+                    'The value of "application_metadata" was None. '
+                    "This is not allowed."
+                ),
+            )
             raise Fail(status_code=HTTPStatus.BAD_REQUEST)
         update_values["application_metadata"] = application_metadata
 
     if "name" in request_json:
         name = request_json["name"]
         update_values["name"] = name
 
     if "image" in request_json:
         image = request_json["image"]
         update_values["image"] = image
 
-    target_manager_base_url = os.environ["TARGET_MANAGER_BASE_URL"]
     put_url = (
-        f"{target_manager_base_url}/databases/{database.database_name}/"
-        f"targets/{target_id}"
+        f"{settings.target_manager_base_url}/databases/"
+        f"{database.database_name}/targets/{target_id}"
     )
     requests.put(url=put_url, json=update_values, timeout=30)
 
     date = email.utils.formatdate(None, localtime=False, usegmt=True)
     headers = {
         "content-type": "application/json",
         "server": "envoy",
         "date": date,
-        "x-aws-region": "us-west-2, eu-west-1",
         "x-envoy-upstream-service-time": "5",
+        "strict-transport-security": "max-age=31536000",
+        "x-aws-region": "us-east-2, us-west-2",
+        "x-content-type-options": "nosniff",
     }
     body = {
         "result_code": ResultCodes.SUCCESS.value,
         "transaction_id": uuid.uuid4().hex,
     }
     return Response(
         status=HTTPStatus.OK,
         response=json_dump(body),
         headers=headers,
     )
 
 
 if __name__ == "__main__":  # pragma: no cover
-    VWS_FLASK_APP.run(debug=True, host=os.environ["VWS_HOST"])
+    SETTINGS = VWSSettings.parse_obj(obj={})
+    VWS_FLASK_APP.run(host=SETTINGS.vws_host)
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_mock_common.py` & `vws-python-mock-2023.4.8/src/mock_vws/_mock_common.py`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_query_tools.py` & `vws-python-mock-2023.4.8/src/mock_vws/_query_tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,24 +5,28 @@
 from __future__ import annotations
 
 import base64
 import datetime
 import io
 import uuid
 from email.message import EmailMessage
-from typing import Any
+from typing import TYPE_CHECKING, Any
 from zoneinfo import ZoneInfo
 
-import mock_vws._cgi as cgi
+import multipart
+
 from mock_vws._base64_decoding import decode_base64
 from mock_vws._constants import ResultCodes, TargetStatuses
 from mock_vws._database_matchers import get_database_matching_client_keys
 from mock_vws._mock_common import json_dump
 from mock_vws.database import VuforiaDatabase
 
+if TYPE_CHECKING:
+    from mock_vws.image_matchers import ImageMatcher
+
 
 class ActiveMatchingTargetsDeleteProcessing(Exception):
     """
     There is at least one active target which matches and was recently deleted.
     """
 
 
@@ -30,50 +34,61 @@
     request_headers: dict[str, str],
     request_body: bytes,
     request_method: str,
     request_path: str,
     databases: set[VuforiaDatabase],
     query_processes_deletion_seconds: int | float,
     query_recognizes_deletion_seconds: int | float,
+    query_match_checker: ImageMatcher,
 ) -> str:
     """
     Args:
         request_path: The path of the request.
         request_headers: The headers sent with the request.
         request_body: The body of the request.
         request_method: The HTTP method of the request.
         databases: All Vuforia databases.
         query_recognizes_deletion_seconds: The number of seconds after a target
             has been deleted that the query endpoint will still recognize the
             target for.
         query_processes_deletion_seconds: The number of seconds after a target
             deletion is recognized that the query endpoint will return a 500
             response on a match.
+        query_match_checker: A callable which takes two image values and
+            returns whether they match.
 
     Returns:
         The response text for a query endpoint request.
 
     Raises:
         ActiveMatchingTargetsDeleteProcessing: There is at least one active
             target which matches and was recently deleted.
     """
     body_file = io.BytesIO(request_body)
 
     email_message = EmailMessage()
     email_message["content-type"] = request_headers["Content-Type"]
-    boundary = email_message.get_boundary().encode()
-    parsed = cgi.parse_multipart(fp=body_file, pdict={"boundary": boundary})
+    boundary = email_message.get_boundary()
+    assert isinstance(boundary, str)
 
-    [max_num_results] = parsed.get("max_num_results", ["1"])
+    parsed = multipart.MultipartParser(stream=body_file, boundary=boundary)
 
-    [include_target_data] = parsed.get("include_target_data", ["top"])
-    include_target_data = include_target_data.lower()
+    parsed_max_num_results = parsed.get("max_num_results")
+    if parsed_max_num_results is None:
+        max_num_results = "1"
+    else:
+        max_num_results = parsed_max_num_results.value
+
+    parsed_include_target_data = parsed.get("include_target_data")
+    if parsed_include_target_data is None:
+        include_target_data = "top"
+    else:
+        include_target_data = parsed_include_target_data.value.lower()
 
-    [image_value] = parsed["image"]
-    assert isinstance(image_value, bytes)
+    image_value = parsed.get("image").raw
     gmt = ZoneInfo("GMT")
     now = datetime.datetime.now(tz=gmt)
 
     processing_timedelta = datetime.timedelta(
         seconds=query_processes_deletion_seconds,
     )
 
@@ -90,15 +105,18 @@
     )
 
     assert isinstance(database, VuforiaDatabase)
 
     matching_targets = [
         target
         for target in database.targets
-        if target.image_value == image_value
+        if query_match_checker(
+            first_image_content=target.image_value,
+            second_image_content=image_value,
+        )
     ]
 
     not_deleted_matches = [
         target
         for target in matching_targets
         if target.active_flag
         and not target.delete_date
@@ -122,15 +140,21 @@
         < (recognition_timedelta + processing_timedelta)
         and target not in deletion_not_recognized_matches
     ]
 
     if active_matching_targets_delete_processing:
         raise ActiveMatchingTargetsDeleteProcessing
 
-    matches = not_deleted_matches + deletion_not_recognized_matches
+    all_quality_matches = not_deleted_matches + deletion_not_recognized_matches
+    minimum_rating = 0
+    matches = [
+        match
+        for match in all_quality_matches
+        if match.tracking_rating > minimum_rating
+    ]
 
     results: list[dict[str, Any]] = []
     for target in matches:
         target_timestamp = target.last_modified_date.timestamp()
         if target.application_metadata is None:
             application_metadata = None
         else:
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_query_validators/__init__.py` & `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Input validators to use in the mock query API.
 """
+from __future__ import annotations
 
-
-from mock_vws.database import VuforiaDatabase
+from typing import TYPE_CHECKING
 
 from .accept_header_validators import validate_accept_header
 from .auth_validators import (
     validate_auth_header_exists,
     validate_auth_header_has_signature,
     validate_auth_header_number_of_parts,
     validate_authorization,
@@ -32,14 +32,17 @@
     validate_image_format,
     validate_image_is_image,
 )
 from .include_target_data_validators import validate_include_target_data
 from .num_results_validators import validate_max_num_results
 from .project_state_validators import validate_project_state
 
+if TYPE_CHECKING:
+    from mock_vws.database import VuforiaDatabase
+
 
 def run_query_validators(
     request_path: str,
     request_headers: dict[str, str],
     request_body: bytes,
     request_method: str,
     databases: set[VuforiaDatabase],
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_query_validators/auth_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/auth_validators.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """
 Authorization validators to use in the mock query API.
 """
+from __future__ import annotations
 
+import logging
+from typing import TYPE_CHECKING
 
 from mock_vws._database_matchers import get_database_matching_client_keys
 from mock_vws._query_validators.exceptions import (
     AuthenticationFailure,
     AuthHeaderMissing,
     MalformedAuthHeader,
-    QueryOutOfBounds,
 )
-from mock_vws.database import VuforiaDatabase
+
+_LOGGER = logging.getLogger(__name__)
+
+if TYPE_CHECKING:
+    from mock_vws.database import VuforiaDatabase
 
 
 def validate_auth_header_exists(request_headers: dict[str, str]) -> None:
     """
     Validate that there is an authorization header given to the query endpoint.
 
     Args:
@@ -22,14 +28,15 @@
 
     Raises:
         AuthHeaderMissing: There is no "Authorization" header.
     """
     if "Authorization" in request_headers:
         return
 
+    _LOGGER.warning(msg="There is no authorization header.")
     raise AuthHeaderMissing
 
 
 def validate_auth_header_number_of_parts(
     request_headers: dict[str, str],
 ) -> None:
     """
@@ -43,14 +50,15 @@
     """
     header = request_headers["Authorization"]
     parts = header.split(" ")
     expected_number_of_parts = 2
     if len(parts) == expected_number_of_parts and parts[1]:
         return
 
+    _LOGGER.warning(msg="The authorization header is malformed.")
     raise MalformedAuthHeader
 
 
 def validate_client_key_exists(
     request_headers: dict[str, str],
     databases: set[VuforiaDatabase],
 ) -> None:
@@ -67,34 +75,36 @@
     header = request_headers["Authorization"]
     first_part, _ = header.split(":")
     _, access_key = first_part.split(" ")
     for database in databases:
         if access_key == database.client_access_key:
             return
 
+    _LOGGER.warning(msg="The client key is unknown.")
     raise AuthenticationFailure
 
 
 def validate_auth_header_has_signature(
     request_headers: dict[str, str],
 ) -> None:
     """
     Validate the authorization header includes a signature.
 
     Args:
         request_headers: The headers sent with the request.
 
     Raises:
-        QueryOutOfBounds: The "Authorization" header has no signature.
+        MalformedAuthHeader: The "Authorization" header has no signature.
     """
     header = request_headers["Authorization"]
     if header.count(":") == 1 and header.split(":")[1]:
         return
 
-    raise QueryOutOfBounds
+    _LOGGER.warning(msg="The authorization header has no signature.")
+    raise MalformedAuthHeader
 
 
 def validate_authorization(
     request_path: str,
     request_headers: dict[str, str],
     request_body: bytes,
     request_method: str,
@@ -120,8 +130,11 @@
         request_path=request_path,
         databases=databases,
     )
 
     if database is not None:
         return
 
+    _LOGGER.warning(
+        msg="The authorization header does not match any databases.",
+    )
     raise AuthenticationFailure
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_query_validators/content_length_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/content_length_validators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """
 Content-Length header validators to use in the mock.
 """
 
 
+import logging
+
 from mock_vws._query_validators.exceptions import (
     AuthenticationFailureGoodFormatting,
     ContentLengthHeaderNotInt,
     ContentLengthHeaderTooLarge,
 )
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_content_length_header_is_int(
     request_headers: dict[str, str],
 ) -> None:
     """
     Validate the ``Content-Length`` header is an integer.
 
@@ -23,14 +27,15 @@
         ContentLengthHeaderNotInt: ``Content-Length`` header is not an integer.
     """
     given_content_length = request_headers["Content-Length"]
 
     try:
         int(given_content_length)
     except ValueError as exc:
+        _LOGGER.warning(msg="The Content-Length header is not an integer.")
         raise ContentLengthHeaderNotInt from exc
 
 
 def validate_content_length_header_not_too_large(
     request_headers: dict[str, str],
     request_body: bytes,
 ) -> None:
@@ -47,14 +52,15 @@
     """
     given_content_length = request_headers["Content-Length"]
 
     body_length = len(request_body if request_body else b"")
     given_content_length_value = int(given_content_length)
     # We skip coverage here as running a test to cover this is very slow.
     if given_content_length_value > body_length:  # pragma: no cover
+        _LOGGER.warning(msg="The Content-Length header is too large.")
         raise ContentLengthHeaderTooLarge
 
 
 def validate_content_length_header_not_too_small(
     request_headers: dict[str, str],
     request_body: bytes,
 ) -> None:
@@ -71,8 +77,9 @@
     """
     given_content_length = request_headers["Content-Length"]
 
     body_length = len(request_body if request_body else b"")
     given_content_length_value = int(given_content_length)
 
     if given_content_length_value < body_length:
+        _LOGGER.warning(msg="The Content-Length header is too small.")
         raise AuthenticationFailureGoodFormatting
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_query_validators/content_type_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/content_type_validators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """
 Validators for the ``Content-Type`` header.
 """
 
 
-import mock_vws._cgi as cgi
+import logging
+from email.message import EmailMessage
+
 from mock_vws._query_validators.exceptions import (
     ImageNotGiven,
     NoBoundaryFound,
     NoContentType,
     UnsupportedMediaType,
 )
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_content_type_header(
     request_headers: dict[str, str],
     request_body: bytes,
 ) -> None:
     """
     Validate the ``Content-Type`` header.
@@ -28,19 +32,31 @@
             'multipart/form-data'.
         NoBoundaryFound: The ``Content-Type`` header does not contain a
             boundary.
         ImageNotGiven: The boundary is not in the request body.
         NoContentType: The content type header is either empty or not given.
     """
     content_type_header = request_headers.get("Content-Type", "")
-    main_value, pdict = cgi.parse_header(content_type_header)
-    if content_type_header == "":
+    if not content_type_header:
+        _LOGGER.warning(msg="The content type header is empty.")
         raise NoContentType
 
-    if main_value not in ("multipart/form-data", "*/*"):
+    email_message = EmailMessage()
+    email_message["content-type"] = request_headers["Content-Type"]
+    if email_message.get_content_type() not in {"multipart/form-data", "*/*"}:
+        _LOGGER.warning(
+            msg=(
+                "The content type header main part is not multipart/form-data."
+            ),
+        )
         raise UnsupportedMediaType
 
-    if "boundary" not in pdict:
+    boundary = email_message.get_boundary()
+    if boundary is None:
+        _LOGGER.warning(
+            msg="The content type header does not contain a boundary.",
+        )
         raise NoBoundaryFound
 
-    if pdict["boundary"].encode() not in request_body:
+    if boundary.encode() not in request_body:
+        _LOGGER.warning(msg="The boundary is not in the request body.")
         raise ImageNotGiven
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_query_validators/date_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/date_validators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 """
 Validators of the date header to use in the mock query API.
 """
 
 import contextlib
 import datetime
+import logging
 from zoneinfo import ZoneInfo
 
 from mock_vws._query_validators.exceptions import (
     DateFormatNotValid,
     DateHeaderNotGiven,
     RequestTimeTooSkewed,
 )
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_date_header_given(request_headers: dict[str, str]) -> None:
     """
     Validate the date header is given to the query endpoint.
 
     Args:
         request_headers: The headers sent with the request.
 
     Raises:
         DateHeaderNotGiven: The date is not given.
     """
     if "Date" in request_headers:
         return
 
+    _LOGGER.warning(msg="The date header is not given.")
     raise DateHeaderNotGiven
 
 
 def _accepted_date_formats() -> set[str]:
     """
     Return all known accepted date formats.
 
@@ -39,20 +43,18 @@
     known_accepted_formats = {
         "%a, %b %d %H:%M:%S %Y",
         "%a %b %d %H:%M:%S %Y",
         "%a, %d %b %Y %H:%M:%S",
         "%a %d %b %Y %H:%M:%S",
     }
 
-    known_accepted_formats = known_accepted_formats.union(
-        {date_format + " GMT" for date_format in known_accepted_formats},
+    return known_accepted_formats.union(
+        {f"{date_format} GMT" for date_format in known_accepted_formats},
     )
 
-    return known_accepted_formats
-
 
 def validate_date_format(request_headers: dict[str, str]) -> None:
     """
     Validate the format of the date header given to the query endpoint.
 
     Args:
         request_headers: The headers sent with the request.
@@ -63,14 +65,15 @@
     date_header = request_headers["Date"]
 
     for date_format in _accepted_date_formats():
         with contextlib.suppress(ValueError):
             datetime.datetime.strptime(date_header, date_format).astimezone()
             return
 
+    _LOGGER.warning(msg="The date header is in the wrong format.")
     raise DateFormatNotValid
 
 
 def validate_date_in_range(request_headers: dict[str, str]) -> None:
     """
     Validate date in the date header given to the query endpoint.
 
@@ -78,25 +81,28 @@
         request_headers: The headers sent with the request.
 
     Raises:
         RequestTimeTooSkewed: The date is out of range.
     """
     date_header = request_headers["Date"]
 
+    date = None
     for date_format in _accepted_date_formats():
         with contextlib.suppress(ValueError):
             date = datetime.datetime.strptime(
                 date_header,
                 date_format,
             ).astimezone()
 
+    assert isinstance(date, datetime.datetime)
     gmt = ZoneInfo("GMT")
     now = datetime.datetime.now(tz=gmt)
     date_from_header = date.replace(tzinfo=gmt)
     time_difference = now - date_from_header
 
     maximum_time_difference = datetime.timedelta(minutes=65)
 
     if abs(time_difference) < maximum_time_difference:
         return
 
+    _LOGGER.warning(msg="The date header is out of range.")
     raise RequestTimeTooSkewed
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_query_validators/exceptions.py` & `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self.response_text = "Malformed date header."
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "Content-Type": "text/plain;charset=iso-8859-1",
             "Connection": "keep-alive",
             "Server": "nginx",
             "Date": date,
-            "WWW-Authenticate": "VWS",
+            "WWW-Authenticate": "KWS",
             "Content-Length": str(len(self.response_text)),
         }
 
 
 class RequestTimeTooSkewed(ValidatorException):
     """
     Exception raised when Vuforia returns a response with a result code
@@ -262,15 +262,15 @@
 
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "Content-Type": "text/plain;charset=iso-8859-1",
             "Connection": "keep-alive",
             "Server": "nginx",
             "Date": date,
-            "WWW-Authenticate": "VWS",
+            "WWW-Authenticate": "KWS",
             "Content-Length": str(len(self.response_text)),
         }
 
 
 class MalformedAuthHeader(ValidatorException):
     """
     Exception raised when an auth header is not given.
@@ -279,26 +279,27 @@
     def __init__(self) -> None:
         """
         Attributes:
             status_code: The status code to use in a response if this is
                 raised.
             response_text: The response text to use in a response if this is
                 raised.
+            www_authenticate: The WWW-Authenticate header value.
         """
         super().__init__()
         self.status_code = HTTPStatus.UNAUTHORIZED
         self.response_text = "Malformed authorization header."
 
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "Content-Type": "text/plain;charset=iso-8859-1",
             "Connection": "keep-alive",
             "Server": "nginx",
             "Date": date,
-            "WWW-Authenticate": "VWS",
+            "WWW-Authenticate": "KWS",
             "Content-Length": str(len(self.response_text)),
         }
 
 
 class UnknownParameters(ValidatorException):
     """
     Exception raised when unknown parameters are given.
@@ -539,47 +540,14 @@
             "Connection": "keep-alive",
             "Server": "nginx",
             "Date": date,
             "Content-Length": str(len(self.response_text)),
         }
 
 
-class QueryOutOfBounds(ValidatorException):
-    """
-    Exception raised when VWS returns an HTML page which says that there is a
-    particular out of bounds error.
-    """
-
-    def __init__(self) -> None:
-        """
-        Attributes:
-            status_code: The status code to use in a response if this is
-                raised.
-            response_text: The response text to use in a response if this is
-                raised.
-        """
-        super().__init__()
-        self.status_code = HTTPStatus.INTERNAL_SERVER_ERROR
-        resources_dir = Path(__file__).parent / "resources"
-        filename = "query_out_of_bounds_response.html"
-        oops_resp_file = resources_dir / filename
-        text = str(oops_resp_file.read_text())
-        self.response_text = text
-
-        date = email.utils.formatdate(None, localtime=False, usegmt=True)
-        self.headers = {
-            "Content-Type": "text/html;charset=iso-8859-1",
-            "Connection": "keep-alive",
-            "Server": "nginx",
-            "Date": date,
-            "Cache-Control": "must-revalidate,no-cache,no-store",
-            "Content-Length": str(len(self.response_text)),
-        }
-
-
 class ContentLengthHeaderTooLarge(ValidatorException):
     """
     Exception raised when the given content length header is too large.
     """
 
     # We skip coverage here as running a test to cover this is very slow.
     def __init__(self) -> None:  # pragma: no cover
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_query_validators/image_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/image_validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """
 Input validators for the image field use in the mock query API.
 """
 
 import io
+import logging
 from email.message import EmailMessage
 
+import multipart
 from PIL import Image
 
-import mock_vws._cgi as cgi
 from mock_vws._query_validators.exceptions import (
     BadImage,
     ImageNotGiven,
     RequestEntityTooLarge,
 )
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_image_field_given(
     request_headers: dict[str, str],
     request_body: bytes,
 ) -> None:
     """
     Validate that the image field is given.
@@ -29,20 +32,21 @@
     Raises:
         ImageNotGiven: The image field is not given.
     """
     body_file = io.BytesIO(request_body)
 
     email_message = EmailMessage()
     email_message["content-type"] = request_headers["Content-Type"]
-    boundary = email_message.get_boundary().encode()
-    parsed = cgi.parse_multipart(fp=body_file, pdict={"boundary": boundary})
-
-    if "image" in parsed:
+    boundary = email_message.get_boundary()
+    assert isinstance(boundary, str)
+    parsed = multipart.MultipartParser(stream=body_file, boundary=boundary)
+    if parsed.get("image") is not None:
         return
 
+    _LOGGER.warning(msg="The image field is not given.")
     raise ImageNotGiven
 
 
 def validate_image_file_size(
     request_headers: dict[str, str],
     request_body: bytes,
 ) -> None:
@@ -56,28 +60,29 @@
     Raises:
         RequestEntityTooLarge: The image file size is too large.
     """
     body_file = io.BytesIO(request_body)
 
     email_message = EmailMessage()
     email_message["content-type"] = request_headers["Content-Type"]
-    boundary = email_message.get_boundary().encode()
-    parsed = cgi.parse_multipart(fp=body_file, pdict={"boundary": boundary})
-
-    [image] = parsed["image"]
+    boundary = email_message.get_boundary()
+    assert isinstance(boundary, str)
+    parsed = multipart.MultipartParser(stream=body_file, boundary=boundary)
+    image = parsed.get("image").raw
 
     # This is the documented maximum size of a PNG as per.
-    # https://library.vuforia.com/articles/Solution/How-To-Perform-an-Image-Recognition-Query.
+    # https://library.vuforia.com/web-api/vuforia-query-web-api.
     # However, the tests show that this maximum size also applies to JPEG
     # files.
     max_bytes = 2 * 1024 * 1024
     # Ignore coverage on this as there is a bug in urllib3 which means that we
     # do not trigger this exception.
     # See https://github.com/urllib3/urllib3/issues/2733.
     if len(image) > max_bytes:  # pragma: no cover
+        _LOGGER.warning(msg="The image file size is too large.")
         raise RequestEntityTooLarge
 
 
 def validate_image_dimensions(
     request_headers: dict[str, str],
     request_body: bytes,
 ) -> None:
@@ -92,26 +97,26 @@
         BadImage: The image is given and is not within the maximum width and
             height limits.
     """
     body_file = io.BytesIO(request_body)
 
     email_message = EmailMessage()
     email_message["content-type"] = request_headers["Content-Type"]
-    boundary = email_message.get_boundary().encode()
-    parsed = cgi.parse_multipart(fp=body_file, pdict={"boundary": boundary})
-
-    [image] = parsed["image"]
-    assert isinstance(image, bytes)
+    boundary = email_message.get_boundary()
+    assert isinstance(boundary, str)
+    parsed = multipart.MultipartParser(stream=body_file, boundary=boundary)
+    image = parsed.get("image").raw
     image_file = io.BytesIO(image)
     pil_image = Image.open(image_file)
     max_width = 30000
     max_height = 30000
     if pil_image.height <= max_height and pil_image.width <= max_width:
         return
 
+    _LOGGER.warning(msg="The image dimensions are too large.")
     raise BadImage
 
 
 def validate_image_format(
     request_headers: dict[str, str],
     request_body: bytes,
 ) -> None:
@@ -125,26 +130,26 @@
     Raises:
         BadImage: The image is given and is not either a PNG or a JPEG.
     """
     body_file = io.BytesIO(request_body)
 
     email_message = EmailMessage()
     email_message["content-type"] = request_headers["Content-Type"]
-    boundary = email_message.get_boundary().encode()
-    parsed = cgi.parse_multipart(fp=body_file, pdict={"boundary": boundary})
-
-    [image] = parsed["image"]
+    boundary = email_message.get_boundary()
+    assert isinstance(boundary, str)
+    parsed = multipart.MultipartParser(stream=body_file, boundary=boundary)
+    image = parsed.get("image").raw
 
-    assert isinstance(image, bytes)
     image_file = io.BytesIO(image)
     pil_image = Image.open(image_file)
 
-    if pil_image.format in ("PNG", "JPEG"):
+    if pil_image.format in {"PNG", "JPEG"}:
         return
 
+    _LOGGER.warning(msg="The image format is not PNG or JPEG.")
     raise BadImage
 
 
 def validate_image_is_image(
     request_headers: dict[str, str],
     request_body: bytes,
 ) -> None:
@@ -158,19 +163,19 @@
     Raises:
         BadImage: Image data is given and it is not an image file.
     """
     body_file = io.BytesIO(request_body)
 
     email_message = EmailMessage()
     email_message["content-type"] = request_headers["Content-Type"]
-    boundary = email_message.get_boundary().encode()
-    parsed = cgi.parse_multipart(fp=body_file, pdict={"boundary": boundary})
-
-    [image] = parsed["image"]
+    boundary = email_message.get_boundary()
+    assert isinstance(boundary, str)
+    parsed = multipart.MultipartParser(stream=body_file, boundary=boundary)
+    image = parsed.get("image").raw
 
-    assert isinstance(image, bytes)
     image_file = io.BytesIO(image)
 
     try:
         Image.open(image_file)
     except OSError as exc:
+        _LOGGER.warning(msg="The image is not an image file.")
         raise BadImage from exc
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_query_validators/include_target_data_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/include_target_data_validators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """
 Validators for the ``include_target_data`` field.
 """
 
 import io
+import logging
 from email.message import EmailMessage
 
-import mock_vws._cgi as cgi
+import multipart
+
 from mock_vws._query_validators.exceptions import InvalidIncludeTargetData
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_include_target_data(
     request_headers: dict[str, str],
     request_body: bytes,
 ) -> None:
     """
     Validate the ``include_target_data`` field is either an accepted value or
@@ -25,18 +29,26 @@
         InvalidIncludeTargetData: The ``include_target_data`` field is not an
             accepted value.
     """
     body_file = io.BytesIO(request_body)
 
     email_message = EmailMessage()
     email_message["content-type"] = request_headers["Content-Type"]
-    boundary = email_message.get_boundary().encode()
-    parsed = cgi.parse_multipart(fp=body_file, pdict={"boundary": boundary})
+    boundary = email_message.get_boundary()
+    assert isinstance(boundary, str)
+    parsed = multipart.MultipartParser(stream=body_file, boundary=boundary)
+
+    parsed_include_target_data = parsed.get("include_target_data")
+    if parsed_include_target_data is None:
+        include_target_data = "top"
+    else:
+        include_target_data = parsed_include_target_data.value
 
-    [include_target_data] = parsed.get("include_target_data", ["top"])
-    lower_include_target_data = include_target_data.lower()
     allowed_included_target_data = {"top", "all", "none"}
-    if lower_include_target_data in allowed_included_target_data:
+    if include_target_data.lower() in allowed_included_target_data:
         return
 
     assert isinstance(include_target_data, str)
+    _LOGGER.warning(
+        msg="The include_target_data field is not an accepted value.",
+    )
     raise InvalidIncludeTargetData(given_value=include_target_data)
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_query_validators/num_results_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/num_results_validators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """
 Validators for the ``max_num_results`` fields.
 """
 
 import io
+import logging
 from email.message import EmailMessage
 
-import mock_vws._cgi as cgi
+import multipart
+
 from mock_vws._query_validators.exceptions import (
     InvalidMaxNumResults,
     MaxNumResultsOutOfRange,
 )
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_max_num_results(
     request_headers: dict[str, str],
     request_body: bytes,
 ) -> None:
     """
     Validate the ``max_num_results`` field is either an integer within range or
@@ -29,25 +33,32 @@
             less than or equal to the max integer in Java.
         MaxNumResultsOutOfRange: The ``max_num_results`` given is not in range.
     """
     body_file = io.BytesIO(request_body)
 
     email_message = EmailMessage()
     email_message["content-type"] = request_headers["Content-Type"]
-    boundary = email_message.get_boundary().encode()
-    parsed = cgi.parse_multipart(fp=body_file, pdict={"boundary": boundary})
-
-    [max_num_results] = parsed.get("max_num_results", ["1"])
-    assert isinstance(max_num_results, str)
+    boundary = email_message.get_boundary()
+    assert isinstance(boundary, str)
+    parsed = multipart.MultipartParser(stream=body_file, boundary=boundary)
+
+    parsed_max_num_results = parsed.get("max_num_results")
+    if parsed_max_num_results is None:
+        max_num_results = "1"
+    else:
+        max_num_results = parsed_max_num_results.value
 
     try:
         max_num_results_int = int(max_num_results)
     except ValueError as exc:
+        _LOGGER.warning(msg="The max_num_results field is not an integer.")
         raise InvalidMaxNumResults(given_value=max_num_results) from exc
 
     java_max_int = 2147483647
     if max_num_results_int > java_max_int:
+        _LOGGER.warning(msg="The max_num_results field is too large.")
         raise InvalidMaxNumResults(given_value=max_num_results)
 
     max_allowed_results = 50
     if max_num_results_int < 1 or max_num_results_int > max_allowed_results:
+        _LOGGER.warning(msg="The max_num_results field is out of range.")
         raise MaxNumResultsOutOfRange(given_value=max_num_results)
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_query_validators/project_state_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_query_validators/project_state_validators.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """
 Validators for the project state.
 """
 
 
+import logging
+
 from mock_vws._database_matchers import get_database_matching_client_keys
 from mock_vws._query_validators.exceptions import InactiveProject
 from mock_vws.database import VuforiaDatabase
 from mock_vws.states import States
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_project_state(
     request_path: str,
     request_headers: dict[str, str],
     request_body: bytes,
     request_method: str,
     databases: set[VuforiaDatabase],
@@ -37,8 +41,9 @@
         databases=databases,
     )
 
     assert isinstance(database, VuforiaDatabase)
     if database.state != States.PROJECT_INACTIVE:
         return
 
+    _LOGGER.warning(msg="The project is inactive.")
     raise InactiveProject
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_requests_mock_server/decorators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,61 +2,81 @@
 Decorators for using the mock.
 """
 
 from __future__ import annotations
 
 import re
 from contextlib import ContextDecorator
-from typing import Literal
+from typing import TYPE_CHECKING, Literal
 from urllib.parse import urljoin, urlparse
 
 import requests
 from requests_mock.mocker import Mocker
 
-from mock_vws.database import VuforiaDatabase
+from mock_vws.image_matchers import (
+    AverageHashMatcher,
+    ImageMatcher,
+)
 from mock_vws.target_manager import TargetManager
+from mock_vws.target_raters import BrisqueTargetTrackingRater
 
 from .mock_web_query_api import MockVuforiaWebQueryAPI
 from .mock_web_services_api import MockVuforiaWebServicesAPI
 
+if TYPE_CHECKING:
+    from mock_vws.database import VuforiaDatabase
+    from mock_vws.target_raters import TargetTrackingRater
+
+
+_AVERAGE_HASH_MATCHER = AverageHashMatcher(threshold=10)
+_BRISQUE_TRACKING_RATER = BrisqueTargetTrackingRater()
+
 
 class MockVWS(ContextDecorator):
     """
     Route requests to Vuforia's Web Service APIs to fakes of those APIs.
     """
 
     def __init__(
         self,
         base_vws_url: str = "https://vws.vuforia.com",
         base_vwq_url: str = "https://cloudreco.vuforia.com",
-        processing_time_seconds: int | float = 0.5,
-        query_recognizes_deletion_seconds: int | float = 0.2,
+        duplicate_match_checker: ImageMatcher = _AVERAGE_HASH_MATCHER,
+        query_match_checker: ImageMatcher = _AVERAGE_HASH_MATCHER,
+        processing_time_seconds: int | float = 2,
+        query_recognizes_deletion_seconds: int | float = 2,
         query_processes_deletion_seconds: int | float = 3,
+        target_tracking_rater: TargetTrackingRater = _BRISQUE_TRACKING_RATER,
         *,
         real_http: bool = False,
     ) -> None:
         """
         Route requests to Vuforia's Web Service APIs to fakes of those APIs.
 
         Args:
             real_http: Whether or not to forward requests to the real
                 server if they are not handled by the mock.
                 See
                 https://requests-mock.readthedocs.io/en/latest/mocker.html#real-http-requests.
-            processing_time_seconds: The number of seconds
-                to process each image for.
+            processing_time_seconds: The number of seconds to process each
+                image for.
                 In the real Vuforia Web Services, this is not deterministic.
             base_vwq_url: The base URL for the VWQ API.
             base_vws_url: The base URL for the VWS API.
             query_recognizes_deletion_seconds: The number
                 of seconds after a target has been deleted that the query
                 endpoint will still recognize the target for.
             query_processes_deletion_seconds: The number of
                 seconds after a target deletion is recognized that the query
                 endpoint will return a 500 response on a match.
+            query_match_checker: A callable which takes two image values and
+                returns whether they will match in a query request.
+            duplicate_match_checker: A callable which takes two image values
+                and returns whether they are duplicates.
+            target_tracking_rater: A callable for rating targets for tracking.
 
         Raises:
             requests.exceptions.MissingSchema: There is no schema in a given
                 URL.
         """
         super().__init__()
         self._real_http = real_http
@@ -66,32 +86,35 @@
         self._base_vws_url = base_vws_url
         self._base_vwq_url = base_vwq_url
         missing_scheme_error = (
             'Invalid URL "{url}": No scheme supplied. '
             'Perhaps you meant "https://{url}".'
         )
         for url in (base_vwq_url, base_vws_url):
-            result = urlparse(url)
-            if not result.scheme:
+            parse_result = urlparse(url=url)
+            if not parse_result.scheme:
                 error = missing_scheme_error.format(url=url)
                 raise requests.exceptions.MissingSchema(error)
 
         self._mock_vws_api = MockVuforiaWebServicesAPI(
             target_manager=self._target_manager,
             processing_time_seconds=processing_time_seconds,
+            duplicate_match_checker=duplicate_match_checker,
+            target_tracking_rater=target_tracking_rater,
         )
 
         self._mock_vwq_api = MockVuforiaWebQueryAPI(
             target_manager=self._target_manager,
             query_processes_deletion_seconds=(
                 query_processes_deletion_seconds
             ),
             query_recognizes_deletion_seconds=(
                 query_recognizes_deletion_seconds
             ),
+            query_match_checker=query_match_checker,
         )
 
     def add_database(self, database: VuforiaDatabase) -> None:
         """
         Add a cloud database.
 
         Args:
@@ -107,38 +130,38 @@
         """
         Start an instance of a Vuforia mock.
 
         Returns:
             ``self``.
         """
         with Mocker(real_http=self._real_http) as mock:
-            for route in self._mock_vws_api.routes:
+            for vws_route in self._mock_vws_api.routes:
                 url_pattern = urljoin(
                     base=self._base_vws_url,
-                    url=route.path_pattern + "$",
+                    url=f"{vws_route.path_pattern}$",
                 )
 
-                for http_method in route.http_methods:
+                for vws_http_method in vws_route.http_methods:
                     mock.register_uri(
-                        method=http_method,
+                        method=vws_http_method,
                         url=re.compile(url_pattern),
-                        text=getattr(self._mock_vws_api, route.route_name),
+                        text=getattr(self._mock_vws_api, vws_route.route_name),
                     )
 
-            for route in self._mock_vwq_api.routes:
+            for vwq_route in self._mock_vwq_api.routes:
                 url_pattern = urljoin(
                     base=self._base_vwq_url,
-                    url=route.path_pattern + "$",
+                    url=f"{vwq_route.path_pattern}$",
                 )
 
-                for http_method in route.http_methods:
+                for vwq_http_method in vwq_route.http_methods:
                     mock.register_uri(
-                        method=http_method,
+                        method=vwq_http_method,
                         url=re.compile(url_pattern),
-                        text=getattr(self._mock_vwq_api, route.route_name),
+                        text=getattr(self._mock_vwq_api, vwq_route.route_name),
                     )
 
         self._mock = mock
         self._mock.start()
 
         return self
 
@@ -147,12 +170,11 @@
         Stop the Vuforia mock.
 
         Returns:
             False
         """
         # __exit__ needs this to be passed in but vulture thinks that it is
         # unused, so we "use" it here.
-        for _ in (exc,):
-            pass
+        assert isinstance(exc, tuple)
 
         self._mock.stop()
         return False
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_requests_mock_server/mock_web_query_api.py` & `vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/mock_web_query_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 """
 A fake implementation of the Vuforia Web Query API.
 
 See
-https://library.vuforia.com/articles/Solution/How-To-Perform-an-Image-Recognition-Query
+https://library.vuforia.com/web-api/vuforia-query-web-api
 """
 
 from __future__ import annotations
 
 import email.utils
-from collections.abc import Callable
+from typing import TYPE_CHECKING
 
 from requests_mock import POST
-from requests_mock.request import _RequestObjectProxy
-from requests_mock.response import _Context
 
 from mock_vws._mock_common import Route
 from mock_vws._query_tools import (
     ActiveMatchingTargetsDeleteProcessing,
     get_query_match_response_text,
 )
 from mock_vws._query_validators import run_query_validators
 from mock_vws._query_validators.exceptions import (
     DeletedTargetMatched,
     ValidatorException,
 )
-from mock_vws.target_manager import TargetManager
+
+if TYPE_CHECKING:
+    from collections.abc import Callable
+
+    from requests_mock.request import _RequestObjectProxy
+    from requests_mock.response import _Context
+
+    from mock_vws.image_matchers import ImageMatcher
+    from mock_vws.target_manager import TargetManager
 
 _ROUTES: set[Route] = set()
 
 
 def route(
     path_pattern: str,
     http_methods: set[str],
@@ -74,36 +80,40 @@
     """
 
     def __init__(
         self,
         target_manager: TargetManager,
         query_recognizes_deletion_seconds: int | float,
         query_processes_deletion_seconds: int | float,
+        query_match_checker: ImageMatcher,
     ) -> None:
         """
         Args:
             target_manager: The target manager which holds all databases.
             query_recognizes_deletion_seconds: The number of seconds after a
                 target has been deleted that the query endpoint will still
                 recognize the target for.
             query_processes_deletion_seconds: The number of seconds after a
                 target deletion is recognized that the query endpoint will
                 return a 500 response on a match.
+            query_match_checker: A callable which takes two image values and
+                returns whether they match.
 
         Attributes:
             routes: The `Route`s to be used in the mock.
         """
         self.routes: set[Route] = _ROUTES
         self._target_manager = target_manager
         self._query_processes_deletion_seconds = (
             query_processes_deletion_seconds
         )
         self._query_recognizes_deletion_seconds = (
             query_recognizes_deletion_seconds
         )
+        self._query_match_checker = query_match_checker
 
     @route(path_pattern="/v1/query", http_methods={POST})
     def query(
         self,
         request: _RequestObjectProxy,
         context: _Context,
     ) -> str:
@@ -132,14 +142,15 @@
                 databases=self._target_manager.databases,
                 query_processes_deletion_seconds=(
                     self._query_processes_deletion_seconds
                 ),
                 query_recognizes_deletion_seconds=(
                     self._query_recognizes_deletion_seconds
                 ),
+                query_match_checker=self._query_match_checker,
             )
         except ActiveMatchingTargetsDeleteProcessing:
             deleted_target_matched_exception = DeletedTargetMatched()
             context.headers = deleted_target_matched_exception.headers
             context.status_code = deleted_target_matched_exception.status_code
             return deleted_target_matched_exception.response_text
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_requests_mock_server/mock_web_services_api.py` & `vws-python-mock-2023.4.8/src/mock_vws/_requests_mock_server/mock_web_services_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,37 +7,43 @@
 
 from __future__ import annotations
 
 import base64
 import dataclasses
 import datetime
 import email.utils
-import random
 import uuid
-from collections.abc import Callable
 from http import HTTPStatus
+from typing import TYPE_CHECKING
 from zoneinfo import ZoneInfo
 
 from requests_mock import DELETE, GET, POST, PUT
-from requests_mock.request import _RequestObjectProxy
-from requests_mock.response import _Context
 
 from mock_vws._constants import ResultCodes, TargetStatuses
 from mock_vws._database_matchers import get_database_matching_server_keys
 from mock_vws._mock_common import Route, json_dump
 from mock_vws._services_validators import run_services_validators
 from mock_vws._services_validators.exceptions import (
     Fail,
     TargetStatusNotSuccess,
     TargetStatusProcessing,
     ValidatorException,
 )
 from mock_vws.database import VuforiaDatabase
 from mock_vws.target import Target
-from mock_vws.target_manager import TargetManager
+
+if TYPE_CHECKING:
+    from collections.abc import Callable
+
+    from requests_mock.request import _RequestObjectProxy
+    from requests_mock.response import _Context
+
+    from mock_vws.image_matchers import ImageMatcher
+    from mock_vws.target_manager import TargetManager
+    from mock_vws.target_raters import TargetTrackingRater
 
 _TARGET_ID_PATTERN = "[A-Za-z0-9]+"
 
 
 _ROUTES: set[Route] = set()
 
 
@@ -46,15 +52,15 @@
     http_methods: set[str],
 ) -> Callable[[Callable[..., str]], Callable[..., str]]:
     """
     Register a decorated method so that it can be recognized as a route.
 
     Args:
         path_pattern: The end part of a URL pattern. E.g. `/targets` or
-            `/targets/.+`.
+          `/targets/.+`.
         http_methods: HTTP methods that map to the route function.
 
     Returns:
         A decorator which takes methods and makes them recognizable as routes.
     """
 
     def decorator(method: Callable[..., str]) -> Callable[..., str]:
@@ -85,28 +91,35 @@
     This implementation is tied to the implementation of `requests_mock`.
     """
 
     def __init__(
         self,
         target_manager: TargetManager,
         processing_time_seconds: int | float,
+        duplicate_match_checker: ImageMatcher,
+        target_tracking_rater: TargetTrackingRater,
     ) -> None:
         """
         Args:
             target_manager: Target Manager which stores databases.
             processing_time_seconds: The number of seconds to process each
-                image for. In the real Vuforia Web Services, this is not
-                deterministic.
+              image for. In the real Vuforia Web Services, this is not
+              deterministic.
+            duplicate_match_checker: A callable which takes two image values
+              and returns whether they are duplicates.
+            target_tracking_rater: A callable for rating targets for tracking.
 
         Attributes:
             routes: The `Route`s to be used in the mock.
         """
         self._target_manager = target_manager
         self.routes: set[Route] = _ROUTES
         self._processing_time_seconds = processing_time_seconds
+        self._duplicate_match_checker = duplicate_match_checker
+        self._target_tracking_rater = target_tracking_rater
 
     @route(
         path_pattern="/targets",
         http_methods={POST},
     )
     def add_target(
         self,
@@ -154,14 +167,15 @@
         new_target = Target(
             name=request.json()["name"],
             width=request.json()["width"],
             image_value=base64.b64decode(request.json()["image"]),
             active_flag=active_flag,
             processing_time_seconds=self._processing_time_seconds,
             application_metadata=application_metadata,
+            target_tracking_rater=self._target_tracking_rater,
         )
         database.targets.add(new_target)
 
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         context.status_code = HTTPStatus.CREATED
         body = {
             "transaction_id": uuid.uuid4().hex,
@@ -170,16 +184,18 @@
         }
         body_json = json_dump(body)
         context.headers = {
             "content-type": "application/json",
             "server": "envoy",
             "date": date,
             "content-length": str(len(body_json)),
-            "x-aws-region": "us-west-2, eu-west-1",
             "x-envoy-upstream-service-time": "5",
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
         return body_json
 
     @route(
         path_pattern=f"/targets/{_TARGET_ID_PATTERN}",
         http_methods={DELETE},
     )
@@ -238,16 +254,18 @@
         }
         body_json = json_dump(body)
         context.headers = {
             "content-length": str(len(body_json)),
             "content-type": "application/json",
             "date": date,
             "server": "envoy",
-            "x-aws-region": "us-west-2, eu-west-1",
             "x-envoy-upstream-service-time": "5",
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
         return body_json
 
     @route(path_pattern="/summary", http_methods={GET})
     def database_summary(
         self,
         request: _RequestObjectProxy,
@@ -302,16 +320,18 @@
         }
         body_json = json_dump(body)
         context.headers = {
             "content-length": str(len(body_json)),
             "content-type": "application/json",
             "date": date,
             "server": "envoy",
-            "x-aws-region": "us-west-2, eu-west-1",
             "x-envoy-upstream-service-time": "5",
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
         return body_json
 
     @route(path_pattern="/targets", http_methods={GET})
     def target_list(
         self,
         request: _RequestObjectProxy,
@@ -343,28 +363,32 @@
             request_path=request.path,
             databases=self._target_manager.databases,
         )
 
         assert isinstance(database, VuforiaDatabase)
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
 
-        results = [target.target_id for target in database.not_deleted_targets]
+        response_results = [
+            target.target_id for target in database.not_deleted_targets
+        ]
         body: dict[str, str | list[str]] = {
             "transaction_id": uuid.uuid4().hex,
             "result_code": ResultCodes.SUCCESS.value,
-            "results": results,
+            "results": response_results,
         }
         body_json = json_dump(body)
         context.headers = {
             "content-length": str(len(body_json)),
             "content-type": "application/json",
             "date": date,
             "server": "envoy",
-            "x-aws-region": "us-west-2, eu-west-1",
             "x-envoy-upstream-service-time": "5",
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
         return body_json
 
     @route(path_pattern=f"/targets/{_TARGET_ID_PATTERN}", http_methods={GET})
     def get_target(
         self,
         request: _RequestObjectProxy,
@@ -418,16 +442,18 @@
         }
         body_json = json_dump(body)
         context.headers = {
             "content-length": str(len(body_json)),
             "content-type": "application/json",
             "date": date,
             "server": "envoy",
-            "x-aws-region": "us-west-2, eu-west-1",
             "x-envoy-upstream-service-time": "5",
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
         return body_json
 
     @route(
         path_pattern=f"/duplicates/{_TARGET_ID_PATTERN}",
         http_methods={GET},
     )
@@ -462,22 +488,25 @@
             request_path=request.path,
             databases=self._target_manager.databases,
         )
         assert isinstance(database, VuforiaDatabase)
         target_id = request.path.split("/")[-1]
         target = database.get_target(target_id=target_id)
 
-        other_targets = set(database.targets) - {target}
+        other_targets = database.targets - {target}
 
         similar_targets: list[str] = [
             other.target_id
             for other in other_targets
-            if other.image_value == target.image_value
+            if self._duplicate_match_checker(
+                first_image_content=target.image_value,
+                second_image_content=other.image_value,
+            )
             and TargetStatuses.FAILED.value
-            not in (target.status, other.status)
+            not in {target.status, other.status}
             and TargetStatuses.PROCESSING.value != other.status
             and other.active_flag
         ]
 
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         body = {
             "transaction_id": uuid.uuid4().hex,
@@ -486,16 +515,18 @@
         }
         body_json = json_dump(body)
         context.headers = {
             "content-length": str(len(body_json)),
             "content-type": "application/json",
             "date": date,
             "server": "envoy",
-            "x-aws-region": "us-west-2, eu-west-1",
             "x-envoy-upstream-service-time": "5",
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
 
         return body_json
 
     @route(
         path_pattern=f"/targets/{_TARGET_ID_PATTERN}",
         http_methods={PUT},
@@ -569,31 +600,24 @@
             and application_metadata is None
         ):
             fail_exception = Fail(status_code=HTTPStatus.BAD_REQUEST)
             context.headers = fail_exception.headers
             context.status_code = fail_exception.status_code
             return fail_exception.response_text
 
-        # In the real implementation, the tracking rating can stay the same.
-        # However, for demonstration purposes, the tracking rating changes but
-        # when the target is updated.
-        available_values = list(set(range(6)) - {target.tracking_rating})
-        processed_tracking_rating = random.choice(available_values)
-
         gmt = ZoneInfo("GMT")
         last_modified_date = datetime.datetime.now(tz=gmt)
 
         new_target = dataclasses.replace(
             target,
             name=name,
             width=width,
             active_flag=active_flag,
             application_metadata=application_metadata,
             image_value=image_value,
-            processed_tracking_rating=processed_tracking_rating,
             last_modified_date=last_modified_date,
         )
 
         database.targets.remove(target)
         database.targets.add(new_target)
 
         body = {
@@ -602,16 +626,18 @@
         }
         body_json = json_dump(body)
         context.headers = {
             "content-type": "application/json",
             "server": "envoy",
             "date": date,
             "content-length": str(len(body_json)),
-            "x-aws-region": "us-west-2, eu-west-1",
             "x-envoy-upstream-service-time": "5",
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
         return body_json
 
     @route(path_pattern=f"/summary/{_TARGET_ID_PATTERN}", http_methods={GET})
     def target_summary(
         self,
         request: _RequestObjectProxy,
@@ -664,12 +690,14 @@
         }
         body_json = json_dump(body)
         context.headers = {
             "content-length": str(len(body_json)),
             "content-type": "application/json",
             "date": date,
             "server": "envoy",
-            "x-aws-region": "us-west-2, eu-west-1",
             "x-envoy-upstream-service-time": "5",
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
 
         return body_json
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_services_validators/__init__.py` & `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Input validators to use in the mock.
 """
 
+from __future__ import annotations
 
-from mock_vws.database import VuforiaDatabase
+from typing import TYPE_CHECKING
 
 from .active_flag_validators import validate_active_flag
 from .auth_validators import (
     validate_access_key_exists,
     validate_auth_header_exists,
     validate_auth_header_has_signature,
     validate_authorization,
@@ -27,15 +28,15 @@
     validate_image_color_space,
     validate_image_data_type,
     validate_image_encoding,
     validate_image_format,
     validate_image_is_image,
     validate_image_size,
 )
-from .json_validators import validate_json
+from .json_validators import validate_body_given, validate_json
 from .key_validators import validate_keys
 from .metadata_validators import (
     validate_metadata_encoding,
     validate_metadata_size,
     validate_metadata_type,
 )
 from .name_validators import (
@@ -45,14 +46,17 @@
     validate_name_length,
     validate_name_type,
 )
 from .project_state_validators import validate_project_state
 from .target_validators import validate_target_id_exists
 from .width_validators import validate_width
 
+if TYPE_CHECKING:
+    from mock_vws.database import VuforiaDatabase
+
 
 def run_services_validators(
     request_path: str,
     request_headers: dict[str, str],
     request_body: bytes,
     request_method: str,
     databases: set[VuforiaDatabase],
@@ -90,18 +94,26 @@
     validate_target_id_exists(
         request_headers=request_headers,
         request_body=request_body,
         request_method=request_method,
         request_path=request_path,
         databases=databases,
     )
-    validate_json(
+
+    validate_body_given(
         request_body=request_body,
         request_method=request_method,
     )
+
+    validate_date_header_given(request_headers=request_headers)
+    validate_date_format(request_headers=request_headers)
+    validate_date_in_range(request_headers=request_headers)
+
+    validate_json(request_body=request_body)
+
     validate_keys(
         request_body=request_body,
         request_path=request_path,
         request_method=request_method,
     )
     validate_metadata_type(request_body=request_body)
     validate_metadata_encoding(request_body=request_body)
@@ -139,19 +151,14 @@
 
     validate_width(request_body=request_body)
     validate_content_type_header_given(
         request_headers=request_headers,
         request_method=request_method,
     )
 
-    validate_date_header_given(request_headers=request_headers)
-
-    validate_date_format(request_headers=request_headers)
-    validate_date_in_range(request_headers=request_headers)
-
     validate_content_length_header_is_int(
         request_headers=request_headers,
         request_body=request_body,
     )
     validate_content_length_header_not_too_large(
         request_headers=request_headers,
         request_body=request_body,
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_services_validators/auth_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/auth_validators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 """
 Authorization header validators to use in the mock.
 """
+from __future__ import annotations
 
+import logging
 from http import HTTPStatus
+from typing import TYPE_CHECKING
 
 from mock_vws._database_matchers import get_database_matching_server_keys
 from mock_vws._services_validators.exceptions import (
     AuthenticationFailure,
     Fail,
 )
-from mock_vws.database import VuforiaDatabase
+
+if TYPE_CHECKING:
+    from mock_vws.database import VuforiaDatabase
+
+
+_LOGGER = logging.getLogger(__name__)
 
 
 def validate_auth_header_exists(request_headers: dict[str, str]) -> None:
     """
     Validate that there is an authorization header given to a VWS endpoint.
 
     Args:
         request_headers: The headers sent with the request.
 
     Raises:
         AuthenticationFailure: There is no "Authorization" header.
     """
     if "Authorization" not in request_headers:
+        _LOGGER.warning(msg="There is no authorization header.")
         raise AuthenticationFailure
 
 
 def validate_access_key_exists(
     request_headers: dict[str, str],
     databases: set[VuforiaDatabase],
 ) -> None:
@@ -43,14 +52,18 @@
     header = request_headers["Authorization"]
     first_part, _ = header.split(":")
     _, access_key = first_part.split(" ")
     for database in databases:
         if access_key == database.server_access_key:
             return
 
+    _LOGGER.warning(
+        'The access key "%s" does not match a known database.',
+        access_key,
+    )
     raise Fail(status_code=HTTPStatus.BAD_REQUEST)
 
 
 def validate_auth_header_has_signature(
     request_headers: dict[str, str],
 ) -> None:
     """
@@ -62,14 +75,17 @@
     Raises:
         Fail: The "Authorization" header does not include a signature.
     """
     header = request_headers["Authorization"]
     if header.count(":") == 1 and header.split(":")[1]:
         return
 
+    _LOGGER.warning(
+        msg="The authorization header does not include a signature.",
+    )
     raise Fail(status_code=HTTPStatus.BAD_REQUEST)
 
 
 def validate_authorization(
     request_path: str,
     request_headers: dict[str, str],
     request_body: bytes,
@@ -95,8 +111,11 @@
         request_body=request_body,
         request_method=request_method,
         request_path=request_path,
         databases=databases,
     )
 
     if database is None:
+        _LOGGER.warning(
+            msg="No database matches the given authorization header.",
+        )
         raise AuthenticationFailure
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_services_validators/content_length_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/content_length_validators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """
 Content-Length header validators to use in the mock.
 """
 
 
+import logging
+
 from mock_vws._services_validators.exceptions import (
     AuthenticationFailure,
     ContentLengthHeaderNotInt,
     ContentLengthHeaderTooLarge,
 )
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_content_length_header_is_int(
     request_headers: dict[str, str],
     request_body: bytes,
 ) -> None:
     """
     Validate the ``Content-Length`` header is an integer.
@@ -27,14 +31,15 @@
     """
     body_length = len(request_body if request_body else b"")
     given_content_length = request_headers.get("Content-Length", body_length)
 
     try:
         int(given_content_length)
     except ValueError as exc:
+        _LOGGER.warning(msg="The Content-Length header is not an integer.")
         raise ContentLengthHeaderNotInt from exc
 
 
 def validate_content_length_header_not_too_large(
     request_headers: dict[str, str],
     request_body: bytes,
 ) -> None:
@@ -50,14 +55,15 @@
             that the content length is greater than the body length.
     """
     body_length = len(request_body if request_body else b"")
     given_content_length = request_headers.get("Content-Length", body_length)
     given_content_length_value = int(given_content_length)
     # We skip coverage here as running a test to cover this is very slow.
     if given_content_length_value > body_length:  # pragma: no cover
+        _LOGGER.warning(msg="The Content-Length header is too large.")
         raise ContentLengthHeaderTooLarge
 
 
 def validate_content_length_header_not_too_small(
     request_headers: dict[str, str],
     request_body: bytes,
 ) -> None:
@@ -73,8 +79,9 @@
             the content length is smaller than the body length.
     """
     body_length = len(request_body if request_body else b"")
     given_content_length = request_headers.get("Content-Length", body_length)
     given_content_length_value = int(given_content_length)
 
     if given_content_length_value < body_length:
+        _LOGGER.warning(msg="The Content-Length header is too small.")
         raise AuthenticationFailure
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_services_validators/content_type_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/content_type_validators.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """
 Content-Type header validators to use in the mock.
 """
 
 
+import logging
+
 from requests_mock import POST, PUT
 
 from mock_vws._services_validators.exceptions import AuthenticationFailure
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_content_type_header_given(
     request_headers: dict[str, str],
     request_method: str,
 ) -> None:
     """
     Validate that there is a non-empty content type header given if required.
@@ -19,12 +23,13 @@
         request_headers: The headers sent with the request.
         request_method: The HTTP method of the request.
 
     Raises:
         AuthenticationFailure: No ``Content-Type`` header is given and the
             request requires one.
     """
-    request_needs_content_type = bool(request_method in (POST, PUT))
+    request_needs_content_type = bool(request_method in {POST, PUT})
     if request_headers.get("Content-Type") or not request_needs_content_type:
         return
 
+    _LOGGER.warning(msg="No Content-Type header is given.")
     raise AuthenticationFailure
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_services_validators/date_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/date_validators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 """
 Validators of the date header to use in the mock services API.
 """
 
 import datetime
+import logging
 from http import HTTPStatus
 from zoneinfo import ZoneInfo
 
 from mock_vws._services_validators.exceptions import Fail, RequestTimeTooSkewed
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_date_header_given(request_headers: dict[str, str]) -> None:
     """
     Validate the date header is given to a VWS endpoint.
 
     Args:
         request_headers: The headers sent with the request.
 
     Raises:
         Fail: The date is not given.
     """
     if "Date" in request_headers:
         return
 
+    _LOGGER.warning(msg="The date header is not given.")
     raise Fail(status_code=HTTPStatus.BAD_REQUEST)
 
 
 def validate_date_format(request_headers: dict[str, str]) -> None:
     """
     Validate the format of the date header given to a VWS endpoint.
 
@@ -36,14 +40,15 @@
         Fail: The date is in the wrong format.
     """
     date_header = request_headers["Date"]
     date_format = "%a, %d %b %Y %H:%M:%S GMT"
     try:
         datetime.datetime.strptime(date_header, date_format).astimezone()
     except ValueError as exc:
+        _LOGGER.warning(msg="The date header is in the wrong format.")
         raise Fail(status_code=HTTPStatus.BAD_REQUEST) from exc
 
 
 def validate_date_in_range(request_headers: dict[str, str]) -> None:
     """
     Validate the date header given to a VWS endpoint is in range.
 
@@ -61,8 +66,9 @@
 
     now = datetime.datetime.now(tz=gmt)
     time_difference = now - date_from_header
 
     maximum_time_difference = datetime.timedelta(minutes=5)
 
     if abs(time_difference) >= maximum_time_difference:
+        _LOGGER.warning(msg="The date header is out of range.")
         raise RequestTimeTooSkewed
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_services_validators/exceptions.py` & `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -44,16 +44,18 @@
         self.response_text = json_dump(body)
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "content-type": "application/json",
             "server": "envoy",
             "date": date,
             "x-envoy-upstream-service-time": "5",
-            "x-aws-region": "us-west-2, eu-west-1",
             "content-length": str(len(self.response_text)),
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
 
 
 class ProjectInactive(ValidatorException):
     """
     Exception raised when Vuforia returns a response with a result code
     'ProjectInactive'.
@@ -76,16 +78,18 @@
         self.response_text = json_dump(body)
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "content-type": "application/json",
             "server": "envoy",
             "date": date,
             "x-envoy-upstream-service-time": "5",
-            "x-aws-region": "us-west-2, eu-west-1",
             "content-length": str(len(self.response_text)),
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
 
 
 class AuthenticationFailure(ValidatorException):
     """
     Exception raised when Vuforia returns a response with a result code
     'AuthenticationFailure'.
@@ -108,16 +112,18 @@
         self.response_text = json_dump(body)
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "content-type": "application/json",
             "server": "envoy",
             "date": date,
             "x-envoy-upstream-service-time": "5",
-            "x-aws-region": "us-west-2, eu-west-1",
             "content-length": str(len(self.response_text)),
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
 
 
 class Fail(ValidatorException):
     """
     Exception raised when Vuforia returns a response with a result code 'Fail'.
     """
@@ -139,16 +145,18 @@
         self.response_text = json_dump(body)
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "content-type": "application/json",
             "server": "envoy",
             "date": date,
             "x-envoy-upstream-service-time": "5",
-            "x-aws-region": "us-west-2, eu-west-1",
             "content-length": str(len(self.response_text)),
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
 
 
 class MetadataTooLarge(ValidatorException):
     """
     Exception raised when Vuforia returns a response with a result code
     'MetadataTooLarge'.
@@ -171,16 +179,18 @@
         self.response_text = json_dump(body)
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "content-type": "application/json",
             "server": "envoy",
             "date": date,
             "x-envoy-upstream-service-time": "5",
-            "x-aws-region": "us-west-2, eu-west-1",
             "content-length": str(len(self.response_text)),
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
 
 
 class TargetNameExist(ValidatorException):
     """
     Exception raised when Vuforia returns a response with a result code
     'TargetNameExist'.
@@ -203,16 +213,18 @@
         self.response_text = json_dump(body)
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "content-type": "application/json",
             "server": "envoy",
             "date": date,
             "x-envoy-upstream-service-time": "5",
-            "x-aws-region": "us-west-2, eu-west-1",
             "content-length": str(len(self.response_text)),
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
 
 
 class OopsErrorOccurredResponse(ValidatorException):
     """
     Exception raised when VWS returns an HTML page which says "Oops, an error
     occurred".
@@ -237,16 +249,18 @@
         self.response_text = text
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "content-type": "text/html; charset=UTF-8",
             "server": "envoy",
             "date": date,
             "x-envoy-upstream-service-time": "5",
-            "x-aws-region": "us-west-2, eu-west-1",
             "content-length": str(len(self.response_text)),
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
 
 
 class BadImage(ValidatorException):
     """
     Exception raised when Vuforia returns a response with a result code
     'BadImage'.
@@ -269,16 +283,18 @@
         self.response_text = json_dump(body)
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "content-type": "application/json",
             "server": "envoy",
             "date": date,
             "x-envoy-upstream-service-time": "5",
-            "x-aws-region": "us-west-2, eu-west-1",
             "content-length": str(len(self.response_text)),
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
 
 
 class ImageTooLarge(ValidatorException):
     """
     Exception raised when Vuforia returns a response with a result code
     'ImageTooLarge'.
@@ -301,16 +317,18 @@
         self.response_text = json_dump(body)
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "content-type": "application/json",
             "server": "envoy",
             "date": date,
             "x-envoy-upstream-service-time": "5",
-            "x-aws-region": "us-west-2, eu-west-1",
             "content-length": str(len(self.response_text)),
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
 
 
 class RequestTimeTooSkewed(ValidatorException):
     """
     Exception raised when Vuforia returns a response with a result code
     'RequestTimeTooSkewed'.
@@ -333,16 +351,18 @@
         self.response_text = json_dump(body)
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "content-type": "application/json",
             "server": "envoy",
             "date": date,
             "x-envoy-upstream-service-time": "5",
-            "x-aws-region": "us-west-2, eu-west-1",
             "content-length": str(len(self.response_text)),
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
 
 
 class ContentLengthHeaderTooLarge(ValidatorException):
     """
     Exception raised when the given content length header is too large.
     """
@@ -362,15 +382,14 @@
         self.response_text = "stream timeout"
         self.headers = {
             "content-length": str(len(self.response_text)),
             "date": date,
             "server": "envoy",
             "content-type": "text/plain",
             "connection": "close",
-            "x-aws-region": "eu-west-1",
         }
 
 
 class ContentLengthHeaderNotInt(ValidatorException):
     """
     Exception raised when the given content length header is not an integer.
     """
@@ -413,15 +432,14 @@
         self.status_code = HTTPStatus.BAD_REQUEST
         self.response_text = ""
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "server": "envoy",
             "date": date,
             "x-envoy-upstream-service-time": "5",
-            "x-aws-region": "us-west-2, eu-west-1",
             "content-length": str(len(self.response_text)),
         }
 
 
 class TargetStatusNotSuccess(ValidatorException):
     """
     Exception raised when trying to update a target that does not have a
@@ -445,16 +463,18 @@
         self.response_text = json_dump(body)
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "content-type": "application/json",
             "server": "envoy",
             "date": date,
             "x-envoy-upstream-service-time": "5",
-            "x-aws-region": "us-west-2, eu-west-1",
             "content-length": str(len(self.response_text)),
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
 
 
 class TargetStatusProcessing(ValidatorException):
     """
     Exception raised when trying to delete a target which is processing.
     """
@@ -476,10 +496,12 @@
         self.response_text = json_dump(body)
         date = email.utils.formatdate(None, localtime=False, usegmt=True)
         self.headers = {
             "content-type": "application/json",
             "server": "envoy",
             "date": date,
             "x-envoy-upstream-service-time": "5",
-            "x-aws-region": "us-west-2, eu-west-1",
             "content-length": str(len(self.response_text)),
+            "strict-transport-security": "max-age=31536000",
+            "x-aws-region": "us-east-2, us-west-2",
+            "x-content-type-options": "nosniff",
         }
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_services_validators/image_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/image_validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """
 Image validators to use in the mock.
 """
 
 import binascii
 import io
 import json
+import logging
 from http import HTTPStatus
 
 from PIL import Image
 
 from mock_vws._base64_decoding import decode_base64
 from mock_vws._services_validators.exceptions import (
     BadImage,
     Fail,
     ImageTooLarge,
 )
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_image_format(request_body: bytes) -> None:
     """
     Validate the format of the image given to a VWS endpoint.
 
     Args:
         request_body: The body of the request.
@@ -36,17 +39,18 @@
     if image is None:
         return
 
     decoded = decode_base64(encoded_data=image)
     image_file = io.BytesIO(decoded)
     pil_image = Image.open(image_file)
 
-    if pil_image.format in ("PNG", "JPEG"):
+    if pil_image.format in {"PNG", "JPEG"}:
         return
 
+    _LOGGER.warning(msg="The image is not a PNG or JPEG.")
     raise BadImage
 
 
 def validate_image_color_space(request_body: bytes) -> None:
     """
     Validate the color space of the image given to a VWS endpoint.
 
@@ -66,17 +70,20 @@
     if image is None:
         return
 
     decoded = decode_base64(encoded_data=image)
     image_file = io.BytesIO(decoded)
     pil_image = Image.open(image_file)
 
-    if pil_image.mode in ("L", "RGB"):
+    if pil_image.mode in {"L", "RGB"}:
         return
 
+    _LOGGER.warning(
+        msg="The image is not in the RGB or greyscale color space.",
+    )
     raise BadImage
 
 
 def validate_image_size(request_body: bytes) -> None:
     """
     Validate the file size of the image given to a VWS endpoint.
 
@@ -98,14 +105,15 @@
 
     decoded = decode_base64(encoded_data=image)
 
     max_allowed_size = 2_359_293
     if len(decoded) <= max_allowed_size:
         return
 
+    _LOGGER.warning(msg="The image is too large.")
     raise ImageTooLarge
 
 
 def validate_image_is_image(request_body: bytes) -> None:
     """
     Validate that the given image data is actually an image file.
 
@@ -151,14 +159,15 @@
         return
 
     image = json.loads(request_text).get("image")
 
     try:
         decode_base64(encoded_data=image)
     except binascii.Error as exc:
+        _LOGGER.warning(msg=('Image data cannot be base64 decoded: "%s"', exc))
         raise Fail(status_code=HTTPStatus.UNPROCESSABLE_ENTITY) from exc
 
 
 def validate_image_data_type(request_body: bytes) -> None:
     """
     Validate that the given image data is a string.
 
@@ -176,8 +185,9 @@
         return
 
     image = json.loads(request_text).get("image")
 
     if isinstance(image, str):
         return
 
+    _LOGGER.warning(msg=('Image data is not a string: "%s"', image))
     raise Fail(status_code=HTTPStatus.BAD_REQUEST)
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_services_validators/json_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/json_validators.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,64 @@
 """
 Validators for given JSON.
 """
 
 import json
+import logging
 from http import HTTPStatus
 from json.decoder import JSONDecodeError
 
 from requests_mock import POST, PUT
 
 from mock_vws._services_validators.exceptions import (
     Fail,
     UnnecessaryRequestBody,
 )
 
+_LOGGER = logging.getLogger(__name__)
 
-def validate_json(
-    request_body: bytes,
-    request_method: str,
-) -> None:
+
+def validate_body_given(request_body: bytes, request_method: str) -> None:
     """
-    Validate that there is either no JSON given or the JSON given is valid.
+    Validate that no JSON is given for requests other than ``POST`` and ``PUT``
+    requests.
 
     Args:
         request_body: The body of the request.
         request_method: The HTTP method of the request.
 
     Raises:
         UnnecessaryRequestBody: A request body was given for an endpoint which
             does not require one.
         Fail: The request body includes invalid JSON.
     """
     if not request_body:
         return
 
-    if request_method not in (POST, PUT):
+    if request_method not in {POST, PUT}:
+        _LOGGER.warning(
+            msg=(
+                "A request body was given for an endpoint which does not "
+                "require one."
+            ),
+        )
         raise UnnecessaryRequestBody
 
+
+def validate_json(request_body: bytes) -> None:
+    """
+    Validate that any given body is valid JSON.
+
+    Args:
+        request_body: The body of the request.
+
+    Raises:
+        Fail: The request body includes invalid JSON.
+    """
+    if not request_body:
+        return
+
     try:
         json.loads(request_body.decode())
     except JSONDecodeError as exc:
+        _LOGGER.warning(msg="The request body is not valid JSON.")
         raise Fail(status_code=HTTPStatus.BAD_REQUEST) from exc
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_services_validators/key_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/key_validators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """
 Validators for JSON keys.
 """
 
 import json
+import logging
 import re
 from dataclasses import dataclass
 from http import HTTPStatus
 
 from requests_mock import DELETE, GET, POST, PUT
 
 from .exceptions import Fail
 
+_LOGGER = logging.getLogger(__name__)
+
 
 @dataclass
 class _Route:
     """
     A representation of a VWS route.
 
     Args:
@@ -126,20 +129,20 @@
         target_list,
         get_target,
         get_duplicates,
         update_target,
         target_summary,
     )
 
-    [matching_route] = [
+    (matching_route,) = (
         route
         for route in routes
-        if re.match(re.compile(route.path_pattern + "$"), request_path)
+        if re.match(re.compile(f"{route.path_pattern}$"), request_path)
         and request_method in route.http_methods
-    ]
+    )
 
     mandatory_keys = matching_route.mandatory_keys
     optional_keys = matching_route.optional_keys
     allowed_keys = mandatory_keys.union(optional_keys)
 
     if not request_body and not allowed_keys:
         return
@@ -149,8 +152,9 @@
     given_keys = set(request_json.keys())
     all_given_keys_allowed = given_keys.issubset(allowed_keys)
     all_mandatory_keys_given = mandatory_keys.issubset(given_keys)
 
     if all_given_keys_allowed and all_mandatory_keys_given:
         return
 
+    _LOGGER.warning(msg="Invalid keys given to endpoint.")
     raise Fail(status_code=HTTPStatus.BAD_REQUEST)
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_services_validators/metadata_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/metadata_validators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Validators for application metadata.
 """
 
 import binascii
 import json
+import logging
 from http import HTTPStatus
 
 from mock_vws._base64_decoding import decode_base64
 from mock_vws._services_validators.exceptions import Fail, MetadataTooLarge
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_metadata_size(request_body: bytes) -> None:
     """
     Validate that the given application metadata is a string or 1024 * 1024
     bytes or fewer.
 
     Args:
@@ -31,14 +34,15 @@
         return
     decoded = decode_base64(encoded_data=application_metadata)
 
     max_metadata_bytes = 1024 * 1024 - 1
     if len(decoded) <= max_metadata_bytes:
         return
 
+    _LOGGER.warning(msg="The application metadata is too large.")
     raise MetadataTooLarge
 
 
 def validate_metadata_encoding(request_body: bytes) -> None:
     """
     Validate that the given application metadata can be base64 decoded.
 
@@ -61,14 +65,15 @@
 
     if application_metadata is None:
         return
 
     try:
         decode_base64(encoded_data=application_metadata)
     except binascii.Error as exc:
+        _LOGGER.warning(msg="The application metadata is not base64 encoded.")
         raise Fail(status_code=HTTPStatus.UNPROCESSABLE_ENTITY) from exc
 
 
 def validate_metadata_type(request_body: bytes) -> None:
     """
     Validate that the given application metadata is a string or NULL.
 
@@ -87,8 +92,9 @@
         return
 
     application_metadata = request_json.get("application_metadata")
 
     if application_metadata is None or isinstance(application_metadata, str):
         return
 
+    _LOGGER.warning(msg="The application metadata is not a string or NULL.")
     raise Fail(status_code=HTTPStatus.BAD_REQUEST)
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_services_validators/name_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/name_validators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 Validators for target names.
 """
 
 import json
+import logging
 from http import HTTPStatus
 
 from mock_vws._database_matchers import get_database_matching_server_keys
 from mock_vws._services_validators.exceptions import (
     Fail,
     OopsErrorOccurredResponse,
     TargetNameExist,
 )
 from mock_vws.database import VuforiaDatabase
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_name_characters_in_range(
     request_body: bytes,
     request_method: str,
     request_path: str,
 ) -> None:
     """
@@ -43,16 +46,18 @@
     name = json.loads(request_text)["name"]
 
     max_character_ord = 65535
     if all(ord(character) <= max_character_ord for character in name):
         return
 
     if (request_method, request_path) == ("POST", "/targets"):
+        _LOGGER.warning(msg="Characters are out of range.")
         raise OopsErrorOccurredResponse
 
+    _LOGGER.warning(msg="Characters are out of range.")
     raise TargetNameExist
 
 
 def validate_name_type(request_body: bytes) -> None:
     """
     Validate the type of the name argument given to a VWS endpoint.
 
@@ -70,14 +75,15 @@
         return
 
     name = json.loads(request_text)["name"]
 
     if isinstance(name, str):
         return
 
+    _LOGGER.warning(msg="Name is not a string.")
     raise Fail(status_code=HTTPStatus.BAD_REQUEST)
 
 
 def validate_name_length(request_body: bytes) -> None:
     """
     Validate the length of the name argument given to a VWS endpoint.
 
@@ -97,14 +103,15 @@
 
     name = json.loads(request_text)["name"]
 
     max_length = 64
     if name and len(name) <= max_length:
         return
 
+    _LOGGER.warning(msg="Name is not between 1 and 64 characters in length.")
     raise Fail(status_code=HTTPStatus.BAD_REQUEST)
 
 
 def validate_name_does_not_exist_new_target(
     databases: set[VuforiaDatabase],
     request_body: bytes,
     request_headers: dict[str, str],
@@ -152,14 +159,15 @@
         for target in database.not_deleted_targets
         if target.name == name
     ]
 
     if not matching_name_targets:
         return
 
+    _LOGGER.warning(msg="Target name already exists.")
     raise TargetNameExist
 
 
 def validate_name_does_not_exist_existing_target(
     request_headers: dict[str, str],
     request_body: bytes,
     request_method: str,
@@ -210,12 +218,13 @@
         for target in database.not_deleted_targets
         if target.name == name
     ]
 
     if not matching_name_targets:
         return
 
-    [matching_name_target] = matching_name_targets
+    (matching_name_target,) = matching_name_targets
     if matching_name_target.target_id == target_id:
         return
 
+    _LOGGER.warning(msg="Name already exists for another target.")
     raise TargetNameExist
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_services_validators/project_state_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/project_state_validators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """
 Validators for the project state.
 """
 
 
+import logging
+
 from mock_vws._database_matchers import get_database_matching_server_keys
 from mock_vws._services_validators.exceptions import ProjectInactive
 from mock_vws.database import VuforiaDatabase
 from mock_vws.states import States
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_project_state(
     request_path: str,
     request_headers: dict[str, str],
     request_body: bytes,
     request_method: str,
     databases: set[VuforiaDatabase],
@@ -41,8 +45,9 @@
     assert isinstance(database, VuforiaDatabase)
     if database.state != States.PROJECT_INACTIVE:
         return
 
     if request_method == "GET" and "duplicates" not in request_path:
         return
 
+    _LOGGER.warning(msg="The project is inactive.")
     raise ProjectInactive
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_services_validators/target_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/target_validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 """
 Validators for given target IDs.
 """
 
+import logging
+
 from mock_vws._database_matchers import get_database_matching_server_keys
 from mock_vws._services_validators.exceptions import UnknownTarget
 from mock_vws.database import VuforiaDatabase
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_target_id_exists(
     request_path: str,
     request_headers: dict[str, str],
     request_body: bytes,
     request_method: str,
     databases: set[VuforiaDatabase],
@@ -42,14 +46,15 @@
         request_path=request_path,
         databases=databases,
     )
 
     assert isinstance(database, VuforiaDatabase)
 
     try:
-        [_] = [
+        (_,) = (
             target
             for target in database.not_deleted_targets
             if target.target_id == target_id
-        ]
+        )
     except ValueError as exc:
+        _LOGGER.warning('The target ID "%s" does not exist.', target_id)
         raise UnknownTarget from exc
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/_services_validators/width_validators.py` & `vws-python-mock-2023.4.8/src/mock_vws/_services_validators/width_validators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 Validators for the width field.
 """
 
 import json
-import numbers
+import logging
 from http import HTTPStatus
 
 from mock_vws._services_validators.exceptions import Fail
 
+_LOGGER = logging.getLogger(__name__)
+
 
 def validate_width(request_body: bytes) -> None:
     """
     Validate the width argument given to a VWS endpoint.
 
     Args:
         request_body: The body of the request.
@@ -24,12 +26,13 @@
 
     request_text = request_body.decode()
     if "width" not in json.loads(request_text):
         return
 
     width = json.loads(request_text).get("width")
 
-    width_is_number = isinstance(width, numbers.Number)
+    width_is_number = isinstance(width, int | float)
     width_positive = width_is_number and width > 0
 
     if not width_positive:
+        _LOGGER.warning(msg="Width is not a positive number.")
         raise Fail(status_code=HTTPStatus.BAD_REQUEST)
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/database.py` & `vws-python-mock-2023.4.8/src/mock_vws/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,20 +63,20 @@
     # We have ``targets`` as ``hash=False`` so that we can have the class as
     # ``frozen=True`` while still being able to keep the interface we want.
     # In particular, we might want to inspect the ``database`` object's targets
     # as they change via API requests.
     targets: set[Target] = field(default_factory=set, hash=False)
     state: States = States.WORKING
 
-    request_quota = 100000
-    reco_threshold = 1000
-    current_month_recos = 0
-    previous_month_recos = 0
-    total_recos = 0
-    target_quota = 1000
+    request_quota: int = 100000
+    reco_threshold: int = 1000
+    current_month_recos: int = 0
+    previous_month_recos: int = 0
+    total_recos: int = 0
+    target_quota: int = 1000
 
     def to_dict(self) -> DatabaseDict:
         """
         Dump a target to a dictionary which can be loaded as JSON.
         """
         targets = [target.to_dict() for target in self.targets]
         return {
@@ -89,17 +89,17 @@
             "targets": targets,
         }
 
     def get_target(self, target_id: str) -> Target:
         """
         Return a target from the database with the given ID.
         """
-        [target] = [
+        (target,) = (
             target for target in self.targets if target.target_id == target_id
-        ]
+        )
         return target
 
     @classmethod
     def from_dict(cls, database_dict: DatabaseDict) -> VuforiaDatabase:
         """
         Load a database from a dictionary.
         """
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/resources/deleted_target_matched_response.html` & `vws-python-mock-2023.4.8/src/mock_vws/resources/deleted_target_matched_response.html`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/resources/oops_error_occurred_response.html` & `vws-python-mock-2023.4.8/src/mock_vws/resources/oops_error_occurred_response.html`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/target.py` & `vws-python-mock-2023.4.8/src/mock_vws/target.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,42 +2,45 @@
 A fake implementation of a target for the Vuforia Web Services API.
 """
 from __future__ import annotations
 
 import base64
 import datetime
 import io
-import random
 import statistics
 import uuid
 from dataclasses import dataclass, field
-from typing import TypedDict
+from typing import TYPE_CHECKING, TypedDict
 from zoneinfo import ZoneInfo
 
 from PIL import Image, ImageStat
 
 from mock_vws._constants import TargetStatuses
+from mock_vws.target_raters import HardcodedTargetTrackingRater
+
+if TYPE_CHECKING:
+    from mock_vws.target_raters import TargetTrackingRater
 
 
 class TargetDict(TypedDict):
     """
     A dictionary type which represents a target.
     """
 
     name: str
     width: float
     image_base64: str
     active_flag: bool
     processing_time_seconds: int | float
-    processed_tracking_rating: int
     application_metadata: str | None
     target_id: str
     last_modified_date: str
     delete_date_optional: str | None
     upload_date: str
+    tracking_rating: int
 
 
 def _random_hex() -> str:
     """
     Return a random hex value.
     """
     return uuid.uuid4().hex
@@ -47,41 +50,32 @@
     """
     Return the current time in the GMT time zone.
     """
     gmt = ZoneInfo("GMT")
     return datetime.datetime.now(tz=gmt)
 
 
-def _random_tracking_rating() -> int:
-    """
-    Return a random tracking rating.
-    """
-    return random.randint(0, 5)
-
-
 @dataclass(frozen=True, eq=True)
 class Target:
     """
     A Vuforia Target as managed in
     https://developer.vuforia.com/target-manager.
     """
 
     active_flag: bool
     application_metadata: str | None
     image_value: bytes
     name: str
     processing_time_seconds: float
     width: float
+    target_tracking_rater: TargetTrackingRater = field(compare=False)
     current_month_recos: int = 0
     delete_date: datetime.datetime | None = None
     last_modified_date: datetime.datetime = field(default_factory=_time_now)
     previous_month_recos: int = 0
-    processed_tracking_rating: int = field(
-        default_factory=_random_tracking_rating,
-    )
     reco_rating: str = ""
     target_id: str = field(default_factory=_random_hex)
     total_recos: int = 0
     upload_date: datetime.datetime = field(default_factory=_time_now)
 
     @property
     def _post_processing_status(self) -> TargetStatuses:
@@ -128,56 +122,51 @@
 
         if time_since_change <= processing_time:
             return str(TargetStatuses.PROCESSING.value)
 
         return str(self._post_processing_status.value)
 
     @property
+    def _post_processing_target_rating(self) -> int:
+        return self.target_tracking_rater(image_content=self.image_value)
+
+    @property
     def tracking_rating(self) -> int:
         """
         Return the tracking rating of the target recognition image.
-
-        In this implementation that is just a random integer between 0 and 5
-        if the target status is 'success'.
-        The rating is 0 if the target status is 'failed'.
-        The rating is -1 for a short time while the target is being processed.
-        The real VWS seems to give -1 for a short time while processing, then
-        the real rating, even while it is still processing.
         """
         pre_rating_time = datetime.timedelta(
             # That this is half of the total processing time is unrealistic.
             # In VWS it is not a constant percentage.
             seconds=self.processing_time_seconds
             / 2,
         )
 
         timezone = self.upload_date.tzinfo
         now = datetime.datetime.now(tz=timezone)
         time_since_upload = now - self.upload_date
 
+        # The real VWS seems to give -1 for a short time while processing, then
+        # the real rating, even while it is still processing.
         if time_since_upload <= pre_rating_time:
             return -1
 
-        if self._post_processing_status == TargetStatuses.SUCCESS:
-            return self.processed_tracking_rating
-
-        return 0
+        return self._post_processing_target_rating
 
     @classmethod
     def from_dict(cls, target_dict: TargetDict) -> Target:
         """
         Load a target from a dictionary.
         """
         timezone = ZoneInfo("GMT")
         name = target_dict["name"]
         active_flag = target_dict["active_flag"]
         width = target_dict["width"]
         image_base64 = target_dict["image_base64"]
         image_value = base64.b64decode(image_base64)
-        processed_tracking_rating = target_dict["processed_tracking_rating"]
         processing_time_seconds = target_dict["processing_time_seconds"]
         application_metadata = target_dict["application_metadata"]
         target_id = target_dict["target_id"]
         delete_date_optional = target_dict["delete_date_optional"]
         if delete_date_optional is None:
             delete_date = None
         else:
@@ -187,26 +176,29 @@
         last_modified_date = datetime.datetime.fromisoformat(
             target_dict["last_modified_date"],
         ).replace(tzinfo=timezone)
         upload_date = datetime.datetime.fromisoformat(
             target_dict["upload_date"],
         ).replace(tzinfo=timezone)
 
+        target_tracking_rater = HardcodedTargetTrackingRater(
+            rating=target_dict["tracking_rating"],
+        )
         return Target(
             target_id=target_id,
             name=name,
             active_flag=active_flag,
             width=width,
             image_value=image_value,
             processing_time_seconds=processing_time_seconds,
             application_metadata=application_metadata,
             delete_date=delete_date,
             last_modified_date=last_modified_date,
             upload_date=upload_date,
-            processed_tracking_rating=processed_tracking_rating,
+            target_tracking_rater=target_tracking_rater,
         )
 
     def to_dict(self) -> TargetDict:
         """
         Dump a target to a dictionary which can be loaded as JSON.
         """
         delete_date: str | None = None
@@ -217,14 +209,14 @@
 
         return {
             "name": self.name,
             "width": self.width,
             "image_base64": image_base64,
             "active_flag": self.active_flag,
             "processing_time_seconds": self.processing_time_seconds,
-            "processed_tracking_rating": self.processed_tracking_rating,
             "application_metadata": self.application_metadata,
             "target_id": self.target_id,
             "last_modified_date": self.last_modified_date.isoformat(),
             "delete_date_optional": delete_date,
             "upload_date": self.upload_date.isoformat(),
+            "tracking_rating": self.tracking_rating,
         }
```

### Comparing `vws-python-mock-2023.3.5/src/mock_vws/target_manager.py` & `vws-python-mock-2023.4.8/src/mock_vws/target_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """
 A fake implementation of a Vuforia target manager.
 """
+from __future__ import annotations
 
+from typing import TYPE_CHECKING
 
-from mock_vws.database import VuforiaDatabase
+if TYPE_CHECKING:
+    from mock_vws.database import VuforiaDatabase
 
 
 class TargetManager:
     """
     A target manager as per https://developer.vuforia.com/target-manager.
     """
```

### Comparing `vws-python-mock-2023.3.5/src/vws_python_mock.egg-info/PKG-INFO` & `vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vws-python-mock
-Version: 2023.3.5
+Version: 2023.4.8
 Summary: A mock for the Vuforia Web Services (VWS) API.
 Author-email: Adam Dangoor <adamdangoor@gmail.com>
 License: The MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -55,18 +55,19 @@
 
 This requires Python 3.11+.
 
 .. code:: sh
 
     pip install vws-python-mock
 
-.. code:: python
+.. code-block:: python
 
     import requests
-    from mock_vws import MockVWS, VuforiaDatabase
+    from mock_vws import MockVWS
+    from mock_vws.database import VuforiaDatabase
 
     with MockVWS() as mock:
         database = VuforiaDatabase()
         mock.add_database(database=database)
         # This will use the Vuforia mock.
         requests.get('https://vws.vuforia.com/summary')
```

### Comparing `vws-python-mock-2023.3.5/src/vws_python_mock.egg-info/SOURCES.txt` & `vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,30 @@
 CHANGELOG.rst
 CODE_OF_CONDUCT.rst
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
 codecov.yaml
+conftest.py
+doc8.ini
 lint.mk
 pyproject.toml
 readthedocs.yaml
 secrets.tar.gpg
-setup.py
 spelling_private_dict.txt
 vuforia_secrets.env.example
 .github/dependabot.yml
 .github/workflows/ci.yml
 .github/workflows/docker-build.yml
 .github/workflows/lint.yml
 .github/workflows/release.yml
 .github/workflows/windows-ci.yml
+.vscode/extensions.json
+.vscode/settings.json
 ci/__init__.py
 ci/custom_linters.py
 ci/decrypt_secret.sh
 ci/set_secrets_file.py
 docs/Makefile
 docs/source/__init__.py
 docs/source/basic-example.rst
@@ -36,29 +39,27 @@
 docs/source/docker.rst
 docs/source/getting-started.rst
 docs/source/index.rst
 docs/source/installation.rst
 docs/source/mock-api-reference.rst
 docs/source/release-process.rst
 docs/source/versioning-and-api-stability.rst
-requirements/dev-requirements.txt
-requirements/requirements.txt
-requirements/setup-requirements.txt
 src/mock_vws/__init__.py
 src/mock_vws/_base64_decoding.py
-src/mock_vws/_cgi.py
 src/mock_vws/_constants.py
 src/mock_vws/_database_matchers.py
 src/mock_vws/_mock_common.py
 src/mock_vws/_query_tools.py
 src/mock_vws/database.py
+src/mock_vws/image_matchers.py
 src/mock_vws/py.typed
 src/mock_vws/states.py
 src/mock_vws/target.py
 src/mock_vws/target_manager.py
+src/mock_vws/target_raters.py
 src/mock_vws/_flask_server/__init__.py
 src/mock_vws/_flask_server/target_manager.py
 src/mock_vws/_flask_server/vwq.py
 src/mock_vws/_flask_server/vws.py
 src/mock_vws/_flask_server/dockerfiles/target_manager/Dockerfile
 src/mock_vws/_flask_server/dockerfiles/vwq/Dockerfile
 src/mock_vws/_flask_server/dockerfiles/vws/Dockerfile
@@ -70,15 +71,14 @@
 src/mock_vws/_query_validators/date_validators.py
 src/mock_vws/_query_validators/exceptions.py
 src/mock_vws/_query_validators/fields_validators.py
 src/mock_vws/_query_validators/image_validators.py
 src/mock_vws/_query_validators/include_target_data_validators.py
 src/mock_vws/_query_validators/num_results_validators.py
 src/mock_vws/_query_validators/project_state_validators.py
-src/mock_vws/_query_validators/resources/query_out_of_bounds_response.html
 src/mock_vws/_requests_mock_server/__init__.py
 src/mock_vws/_requests_mock_server/decorators.py
 src/mock_vws/_requests_mock_server/mock_web_query_api.py
 src/mock_vws/_requests_mock_server/mock_web_services_api.py
 src/mock_vws/_services_validators/__init__.py
 src/mock_vws/_services_validators/active_flag_validators.py
 src/mock_vws/_services_validators/auth_validators.py
@@ -101,17 +101,14 @@
 src/vws_python_mock.egg-info/dependency_links.txt
 src/vws_python_mock.egg-info/not-zip-safe
 src/vws_python_mock.egg-info/requires.txt
 src/vws_python_mock.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/mock_vws/__init__.py
-tests/mock_vws/jetty_error_array_out_of_bounds.html
-tests/mock_vws/jetty_error_array_out_of_bounds_2.html
-tests/mock_vws/jetty_error_array_out_of_bounds_3.html
 tests/mock_vws/jetty_error_deletion_not_complete.html
 tests/mock_vws/test_add_target.py
 tests/mock_vws/test_authorization_header.py
 tests/mock_vws/test_content_length.py
 tests/mock_vws/test_database_summary.py
 tests/mock_vws/test_date_header.py
 tests/mock_vws/test_delete_target.py
```

### Comparing `vws-python-mock-2023.3.5/src/vws_python_mock.egg-info/requires.txt` & `vws-python-mock-2023.4.8/src/vws_python_mock.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,55 @@
+ImageHash
 Pillow
-VWS-Auth-Tools
+brisque
 flask
-requests-mock
+multipart
+numpy
+opencv-python
+pydantic
 requests
+requests-mock
+vws-auth-tools
+werkzeug
 
 [:sys_platform == "win32"]
 tzdata
 
 [dev]
 PyYAML==6.0
 Sphinx-Substitution-Extensions==2022.2.16
 Sphinx==6.1.3
-VWS-Test-Fixtures==2022.1.3
-black==23.1.0
+VWS-Test-Fixtures==2023.3.5
+black==23.3.0
 check-manifest==0.49
 dirty-equals==0.5.0
-doc8==1.1.1
+doc8==0.11.2
 docker==6.0.1
 dodgy==0.2.1
+enum-tools[sphinx]==0.9.0.post1
 freezegun==1.2.2
-furo==2022.12.7
-keyring==23.13.1
-mypy==1.0.1
+furo==2023.3.27
+mypy==1.2.0
+pdm==2.4.9
 pip_check_reqs==2.4.4
 pydocstyle==6.3.0
 pyenchant==3.2.2
-pylint==2.16.2
+pylint==2.17.2
+pyright==1.1.302
 pyroma==4.2
 pytest-cov==4.0.0
-pytest-envfiles==0.1.0
-pytest==7.2.1
-requests-mock-flask==2022.4.3
-ruff==0.0.253
+pytest==7.2.2
+requests-mock-flask==2023.3.5.1
+ruff==0.0.261
 sphinx-autodoc-typehints==1.22
 sphinx-prompt==1.5.0
 sphinx_paramlinks==0.5.4
 sphinxcontrib-httpdomain==1.8.1
 sphinxcontrib-spelling==8.0.0
-types-Flask==1.1.6
-types-freezegun==1.1.10
-types-PyYAML==6.0.12.8
-types-Pillow==9.4.0.17
-types-requests==2.28.11.15
-types-setuptools==67.4.0.3
-types-urllib3==1.26.25.8
+sphinx-toolbox==3.4.0
+sybil==5.0.0
+types-PyYAML==6.0.12.9
+types-Pillow==9.4.0.19
+types-requests==2.28.11.17
+types-urllib3==1.26.25.10
 vulture==2.7
-vws-python==2021.3.28.2
+vws-python==2023.3.25
```

### Comparing `vws-python-mock-2023.3.5/tests/conftest.py` & `vws-python-mock-2023.4.8/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 """
 Configuration, plugins and fixtures for `pytest`.
 """
+from __future__ import annotations
 
 import base64
 import binascii
-import io
 import uuid
+from typing import TYPE_CHECKING
 
 import pytest
-from _pytest.fixtures import SubRequest
-from mock_vws.database import VuforiaDatabase
 from vws import VWS, CloudRecoService
 
-from tests.mock_vws.utils import Endpoint
+if TYPE_CHECKING:
+    import io
+
+    from _pytest.fixtures import SubRequest
+    from mock_vws.database import VuforiaDatabase
+
+    from tests.mock_vws.utils import Endpoint
 
 pytest_plugins = [
     "tests.mock_vws.fixtures.prepared_requests",
     "tests.mock_vws.fixtures.credentials",
     "tests.mock_vws.fixtures.vuforia_backends",
 ]
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/fixtures/prepared_requests.py` & `vws-python-mock-2023.4.8/tests/mock_vws/fixtures/prepared_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """
 Fixtures which prepare requests.
 """
+from __future__ import annotations
 
 import base64
-import io
 import json
 from http import HTTPStatus
-from typing import Any
+from typing import TYPE_CHECKING, Any
 from urllib.parse import urljoin
 
 import pytest
 import requests
 from mock_vws._constants import ResultCodes
-from mock_vws.database import VuforiaDatabase
 from requests_mock import DELETE, GET, POST, PUT
 from urllib3.filepost import encode_multipart_formdata
-from vws import VWS
 from vws_auth_tools import authorization_header, rfc_1123_date
 
 from tests.mock_vws.utils import Endpoint
 
+if TYPE_CHECKING:
+    import io
+
+    from mock_vws.database import VuforiaDatabase
+    from vws import VWS
+
 VWS_HOST = "https://vws.vuforia.com"
 VWQ_HOST = "https://cloudreco.vuforia.com"
 
 
 @pytest.fixture()
 def add_target(
     vuforia_database: VuforiaDatabase,
@@ -441,17 +445,15 @@
     """
     image_content = high_quality_image.read()
     date = rfc_1123_date()
     request_path = "/v1/query"
     files = {"image": ("image.jpeg", image_content, "image/jpeg")}
     method = POST
 
-    content, content_type_header = encode_multipart_formdata(
-        fields=files,
-    )  # type: ignore[no-untyped-call]
+    content, content_type_header = encode_multipart_formdata(fields=files)
 
     access_key = vuforia_database.client_access_key
     secret_key = vuforia_database.client_secret_key
     authorization_string = authorization_header(
         access_key=access_key,
         secret_key=secret_key,
         method=method,
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/fixtures/vuforia_backends.py` & `vws-python-mock-2023.4.8/tests/mock_vws/fixtures/vuforia_backends.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 """
 Choose which backends to use for the tests.
 """
+from __future__ import annotations
 
 import contextlib
 import logging
-from collections.abc import Generator
 from enum import Enum
+from typing import TYPE_CHECKING
 
 import pytest
 import requests
 import requests_mock
-from _pytest.config.argparsing import Parser
-from _pytest.fixtures import SubRequest
 from mock_vws import MockVWS
 from mock_vws._flask_server.target_manager import TARGET_MANAGER_FLASK_APP
 from mock_vws._flask_server.vwq import CLOUDRECO_FLASK_APP
 from mock_vws._flask_server.vws import VWS_FLASK_APP
 from mock_vws.database import VuforiaDatabase
 from mock_vws.states import States
 from requests_mock_flask import add_flask_app_to_mock
 from vws import VWS
 from vws.exceptions.vws_exceptions import TargetStatusNotSuccess
 
+if TYPE_CHECKING:
+    from collections.abc import Generator
+
+    from _pytest.config.argparsing import Parser
+    from _pytest.fixtures import SubRequest
+
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.DEBUG)
 
 
 def _delete_all_targets(database_keys: VuforiaDatabase) -> None:
     """
     Delete all targets.
@@ -81,15 +86,15 @@
         database_name=inactive_database.database_name,
         server_access_key=inactive_database.server_access_key,
         server_secret_key=inactive_database.server_secret_key,
         client_access_key=inactive_database.client_access_key,
         client_secret_key=inactive_database.client_secret_key,
     )
 
-    with MockVWS(processing_time_seconds=0.2) as mock:
+    with MockVWS() as mock:
         mock.add_database(database=working_database)
         mock.add_database(database=inactive_database)
         yield
 
 
 def _enable_use_docker_in_memory(
     working_database: VuforiaDatabase,
@@ -181,14 +186,38 @@
         parser.addoption(
             f"--skip-{backend.name.lower()}",
             action="store_true",
             default=False,
             help=f"Skip tests for {backend.value}",
         )
 
+    parser.addoption(
+        "--skip-docker_build_tests",
+        action="store_true",
+        default=False,
+    )
+
+
+def pytest_collection_modifyitems(
+    config: pytest.Config,
+    items: list[pytest.Function],
+) -> None:
+    """Skip Docker tests if requested."""
+    skip_docker_build_tests_option = "--skip-docker_build_tests"
+    skip_docker_build_tests_marker = pytest.mark.skip(
+        reason=(
+            "Skipping docker build tests because "
+            f"{skip_docker_build_tests_option} was set"
+        ),
+    )
+    if config.getoption(skip_docker_build_tests_option):
+        for item in items:
+            if "requires_docker_build" in item.keywords:
+                item.add_marker(skip_docker_build_tests_marker)
+
 
 @pytest.fixture(
     params=list(VuforiaBackend),
     ids=[backend.value for backend in list(VuforiaBackend)],
 )
 def verify_mock_vuforia(
     request: SubRequest,
@@ -197,17 +226,20 @@
     monkeypatch: pytest.MonkeyPatch,
 ) -> Generator[None, None, None]:
     """
     Test functions which use this fixture are run multiple times. Once with the
     real Vuforia, and once with each mock.
 
     This is useful for verifying the mocks.
+
+    Yields:
+        ``None``.
     """
     backend = request.param
-    should_skip = request.config.getvalue(f"--skip-{backend.name.lower()}")
+    should_skip = request.config.getoption(f"--skip-{backend.name.lower()}")
     if should_skip:  # pragma: no cover
         pytest.skip()
 
     enable_function = {
         VuforiaBackend.REAL: _enable_use_real_vuforia,
         VuforiaBackend.MOCK: _enable_use_mock_vuforia,
         VuforiaBackend.DOCKER_IN_MEMORY: _enable_use_docker_in_memory,
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/jetty_error_deletion_not_complete.html` & `vws-python-mock-2023.4.8/tests/mock_vws/jetty_error_deletion_not_complete.html`

 * *Files identical despite different names*

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_add_target.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_add_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 """
 Tests for the mock of the add target endpoint.
 """
 
 from __future__ import annotations
 
 import base64
-import io
 import json
 from http import HTTPStatus
 from string import hexdigits
-from typing import Any, Final
+from typing import TYPE_CHECKING, Any, Final
 from urllib.parse import urljoin
 
 import pytest
 import requests
 from dirty_equals import IsInstance
 from mock_vws._constants import ResultCodes
-from mock_vws.database import VuforiaDatabase
-from requests import Response
+from requests.structures import CaseInsensitiveDict
 from requests_mock import POST
-from vws import VWS
 from vws_auth_tools import authorization_header, rfc_1123_date
 
 from tests.mock_vws.utils import make_image_file
 from tests.mock_vws.utils.assertions import (
     assert_valid_date_header,
     assert_vws_failure,
     assert_vws_response,
 )
 
+if TYPE_CHECKING:
+    import io
+
+    from mock_vws.database import VuforiaDatabase
+    from vws import VWS
+
 _MAX_METADATA_BYTES: Final[int] = 1024 * 1024 - 1
 
 
 def add_target_to_vws(
     vuforia_database: VuforiaDatabase,
     data: dict[str, Any],
     content_type: str = "application/json",
-) -> Response:
+) -> requests.Response:
     """
     Return a response from a request to the endpoint to add a target.
 
     Args:
         vuforia_database: The credentials to use to connect to Vuforia.
         data: The data to send, in JSON format, to the endpoint.
         content_type: The `Content-Type` header to use.
@@ -74,40 +77,42 @@
         url=urljoin(base="https://vws.vuforia.com/", url=request_path),
         headers=headers,
         data=content,
         timeout=30,
     )
 
 
-def _assert_oops_response(response: Response) -> None:
+def _assert_oops_response(response: requests.Response) -> None:
     """
     Assert that the response is in the format of Vuforia's "Oops, an error
     occurred" HTML response.
 
     Raises:
         AssertionError: The given response is not expected format.
     """
     assert_valid_date_header(response=response)
     assert "Oops, an error occurred" in response.text
     assert "This exception has been logged with id" in response.text
 
-    expected_headers = requests.structures.CaseInsensitiveDict(
+    expected_headers = CaseInsensitiveDict(
         data={
             "content-type": "text/html; charset=UTF-8",
             "date": response.headers["date"],
             "server": "envoy",
             "content-length": "1190",
             "x-envoy-upstream-service-time": IsInstance(expected_type=str),
+            "strict-transport-security": "max-age=31536000",
             "x-aws-region": IsInstance(expected_type=str),
+            "x-content-type-options": "nosniff",
         },
     )
     assert response.headers == expected_headers
 
 
-def assert_success(response: Response) -> None:
+def assert_success(response: requests.Response) -> None:
     """
     Assert that the given response is a success response for adding a
     target.
 
     Raises:
         AssertionError: The given response is not a valid success response
             for adding a target.
@@ -250,15 +255,15 @@
         "width",
         [-1, "10", None, 0],
         ids=["Negative", "Wrong Type", "None", "Zero"],
     )
     def test_width_invalid(
         vuforia_database: VuforiaDatabase,
         image_file_failed_state: io.BytesIO,
-        width: Any,
+        width: int | str | None,
     ) -> None:
         """
         The width must be a number greater than zero.
         """
         image_data = image_file_failed_state.read()
         image_data_encoded = base64.b64encode(image_data).decode("ascii")
 
@@ -350,16 +355,16 @@
             content_type="application/json",
         )
 
         assert_success(response=response)
 
     @staticmethod
     @pytest.mark.parametrize(
-        ("name", "status_code"),
-        [
+        argnames=("name", "status_code"),
+        argvalues=[
             (1, HTTPStatus.BAD_REQUEST),
             ("", HTTPStatus.BAD_REQUEST),
             ("a" * (_MAX_NAME_LENGTH + 1), HTTPStatus.BAD_REQUEST),
             (None, HTTPStatus.BAD_REQUEST),
             (chr(_MAX_CHAR_VALUE + 1), HTTPStatus.INTERNAL_SERVER_ERROR),
             (
                 chr(_MAX_CHAR_VALUE + 1) * (_MAX_NAME_LENGTH + 1),
@@ -729,15 +734,15 @@
             status_code=HTTPStatus.UNPROCESSABLE_ENTITY,
             result_code=ResultCodes.BAD_IMAGE,
         )
 
     @staticmethod
     @pytest.mark.parametrize("invalid_type_image", [1, None])
     def test_invalid_type(
-        invalid_type_image: Any,
+        invalid_type_image: int | None,
         vuforia_database: VuforiaDatabase,
     ) -> None:
         """
         If the given image is not a string, a `Fail` result is returned.
         """
         data = {
             "name": "example_name",
@@ -964,24 +969,24 @@
     ) -> None:
         """
         NULL is valid application metadata.
         """
         image_data = image_file_failed_state.read()
         image_data_encoded = base64.b64encode(image_data).decode("ascii")
 
-        data = {
+        request_data = {
             "name": "example_name",
             "width": 1,
             "image": image_data_encoded,
             "application_metadata": None,
         }
 
         response = add_target_to_vws(
             vuforia_database=vuforia_database,
-            data=data,
+            data=request_data,
         )
 
         assert_success(response=response)
 
     @staticmethod
     def test_invalid_type(
         vuforia_database: VuforiaDatabase,
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_authorization_header.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_authorization_header.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 """
 Tests for the `Authorization` header.
 """
+from __future__ import annotations
 
-import io
 import uuid
 from http import HTTPStatus
-from pathlib import Path
+from typing import TYPE_CHECKING
 from urllib.parse import urlparse
 
 import pytest
 import requests
 from mock_vws._constants import ResultCodes
-from mock_vws.database import VuforiaDatabase
 from requests.structures import CaseInsensitiveDict
 from vws import VWS, CloudRecoService
 from vws.exceptions import cloud_reco_exceptions
 from vws.exceptions.vws_exceptions import AuthenticationFailure, Fail
 from vws_auth_tools import rfc_1123_date
 
-from tests.mock_vws.utils import Endpoint
 from tests.mock_vws.utils.assertions import (
     assert_valid_date_header,
     assert_valid_transaction_id,
     assert_vwq_failure,
     assert_vws_failure,
 )
 
+if TYPE_CHECKING:
+    import io
+
+    from mock_vws.database import VuforiaDatabase
+
+    from tests.mock_vws.utils import Endpoint
+
 
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestAuthorizationHeader:
     """
     Tests for what happens when the `Authorization` header is not as expected.
     """
 
@@ -57,15 +62,15 @@
         netloc = urlparse(url).netloc
         if netloc == "cloudreco.vuforia.com":
             assert_vwq_failure(
                 response=response,
                 status_code=HTTPStatus.UNAUTHORIZED,
                 content_type="text/plain;charset=iso-8859-1",
                 cache_control=None,
-                www_authenticate="VWS",
+                www_authenticate="KWS",
                 connection="keep-alive",
             )
             assert response.text == "Authorization header missing."
             return
 
         assert_vws_failure(
             response=response,
@@ -110,15 +115,15 @@
         netloc = urlparse(url).netloc
         if netloc == "cloudreco.vuforia.com":
             assert_vwq_failure(
                 response=response,
                 status_code=HTTPStatus.UNAUTHORIZED,
                 content_type="text/plain;charset=iso-8859-1",
                 cache_control=None,
-                www_authenticate="VWS",
+                www_authenticate="KWS",
                 connection="keep-alive",
             )
             assert response.text == "Malformed authorization header."
             return
 
         assert_vws_failure(
             response=response,
@@ -150,15 +155,15 @@
         netloc = urlparse(url).netloc
         if netloc == "cloudreco.vuforia.com":
             assert_vwq_failure(
                 response=response,
                 status_code=HTTPStatus.UNAUTHORIZED,
                 content_type="text/plain;charset=iso-8859-1",
                 cache_control=None,
-                www_authenticate="VWS",
+                www_authenticate="KWS",
                 connection="keep-alive",
             )
             assert response.text == "Malformed authorization header."
             return
 
         assert_vws_failure(
             response=response,
@@ -195,37 +200,21 @@
         response = session.send(request=endpoint.prepared_request)
 
         url = str(endpoint.prepared_request.url)
         netloc = urlparse(url).netloc
         if netloc == "cloudreco.vuforia.com":
             assert_vwq_failure(
                 response=response,
-                status_code=HTTPStatus.INTERNAL_SERVER_ERROR,
-                content_type="text/html;charset=iso-8859-1",
-                cache_control="must-revalidate,no-cache,no-store",
-                www_authenticate=None,
+                status_code=HTTPStatus.UNAUTHORIZED,
+                content_type="text/plain;charset=iso-8859-1",
+                cache_control=None,
+                www_authenticate="KWS",
                 connection="keep-alive",
             )
-            content_filename = "jetty_error_array_out_of_bounds.html"
-            content_filename_2 = "jetty_error_array_out_of_bounds_2.html"
-            content_filename_3 = "jetty_error_array_out_of_bounds_3.html"
-            content_path = Path(__file__).parent / content_filename
-            content_path_2 = Path(__file__).parent / content_filename_2
-            content_path_3 = Path(__file__).parent / content_filename_3
-            content_text = content_path.read_text()
-            content_2_text = content_path_2.read_text()
-            content_3_text = content_path_3.read_text()
-            # We make a new variable for response text so that it is printed
-            # with ``pytest --showlocals``.
-            response_text = response.text
-            assert response_text in (
-                content_text,
-                content_2_text,
-                content_3_text,
-            )
+            assert response.text == "Malformed authorization header."
             return
 
         assert_vws_failure(
             response=response,
             status_code=HTTPStatus.BAD_REQUEST,
             result_code=ResultCodes.FAIL,
         )
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_content_length.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_content_length.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """
 Tests for the ``Content-Length`` header.
 """
+from __future__ import annotations
 
 from http import HTTPStatus
+from typing import TYPE_CHECKING
 from urllib.parse import urlparse
 
 import pytest
 import requests
-from dirty_equals import IsInstance
 from mock_vws._constants import ResultCodes
 from requests.structures import CaseInsensitiveDict
 
-from tests.mock_vws.utils import Endpoint
 from tests.mock_vws.utils.assertions import (
     assert_valid_date_header,
     assert_vwq_failure,
     assert_vws_failure,
 )
 
+if TYPE_CHECKING:
+    from tests.mock_vws.utils import Endpoint
+
 
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestIncorrect:
     """
     Tests for the ``Content-Length`` header set incorrectly.
 
     We cannot test what happens if ``Content-Length`` is removed from a
@@ -45,15 +48,15 @@
         session = requests.Session()
         response = session.send(request=endpoint.prepared_request)
         assert response.status_code == HTTPStatus.BAD_REQUEST
 
         url = str(endpoint.prepared_request.url)
         netloc = urlparse(url).netloc
         if netloc == "cloudreco.vuforia.com":
-            assert response.text == ""
+            assert not response.text
             assert response.headers == CaseInsensitiveDict(
                 data={
                     "Content-Length": str(len(response.text)),
                     "Connection": "Close",
                 },
             )
             return
@@ -87,33 +90,32 @@
         headers = {**endpoint_headers, "Content-Length": content_length}
 
         endpoint.prepared_request.headers = CaseInsensitiveDict(data=headers)
         session = requests.Session()
         response = session.send(request=endpoint.prepared_request)
         if netloc == "cloudreco.vuforia.com":
             assert response.status_code == HTTPStatus.GATEWAY_TIMEOUT
-            assert response.text == ""
+            assert not response.text
             assert response.headers == CaseInsensitiveDict(
                 data={
                     "Content-Length": str(len(response.text)),
                     "Connection": "keep-alive",
                 },
             )
             return
 
         assert_valid_date_header(response=response)
         # We have seen both of these response texts.
-        assert response.text in ("stream timeout", "")
+        assert response.text in {"stream timeout", ""}
         expected_headers = {
             "content-length": str(len(response.text)),
             "connection": "close",
             "content-type": "text/plain",
             "server": "envoy",
             "date": response.headers["date"],
-            "x-aws-region": IsInstance(expected_type=str),
         }
         assert response.headers == CaseInsensitiveDict(
             data=expected_headers,
         )
         assert response.status_code == HTTPStatus.REQUEST_TIMEOUT
 
     @staticmethod
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_database_summary.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_database_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 """
 Tests for the mock of the database summary endpoint.
 """
+from __future__ import annotations
 
-import io
 import logging
 import time
 import uuid
 from http import HTTPStatus
+from typing import TYPE_CHECKING
 
 import pytest
 from mock_vws import MockVWS
 from mock_vws.database import VuforiaDatabase
 from vws import VWS, CloudRecoService
 from vws.exceptions.vws_exceptions import Fail
 
+if TYPE_CHECKING:
+    import io
+
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.DEBUG)
 
 
 def _wait_for_image_numbers(
     vws_client: VWS,
     active_images: int,
@@ -40,15 +44,15 @@
         vws_client: The client to use to connect to Vuforia.
         active_images: The expected number of active images.
         inactive_images: The expected number of inactive images.
         failed_images: The expected number of failed images.
         processing_images: The expected number of processing images.
 
     Raises:
-        Exception: The numbers of images in various categories do not match
+        ValueError: The numbers of images in various categories do not match
             within the time limit.
     """
     requirements = {
         "active_images": active_images,
         "inactive_images": inactive_images,
         "failed_images": failed_images,
         "processing_images": processing_images,
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_date_header.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_date_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 """
 Tests for the `Date` header.
 """
 
+from __future__ import annotations
+
 from datetime import datetime, timedelta
 from http import HTTPStatus
+from typing import TYPE_CHECKING
 from urllib.parse import urlparse
 from zoneinfo import ZoneInfo
 
 import pytest
 import requests
 from freezegun import freeze_time
 from mock_vws._constants import ResultCodes
 from requests.structures import CaseInsensitiveDict
 from vws_auth_tools import authorization_header, rfc_1123_date
 
-from tests.mock_vws.utils import Endpoint
 from tests.mock_vws.utils.assertions import (
     assert_query_success,
     assert_valid_transaction_id,
     assert_vwq_failure,
     assert_vws_failure,
     assert_vws_response,
 )
 
+if TYPE_CHECKING:
+    from tests.mock_vws.utils import Endpoint
+
 _VWS_MAX_TIME_SKEW = timedelta(minutes=5)
 _VWQ_MAX_TIME_SKEW = timedelta(minutes=65)
 _LEEWAY = timedelta(seconds=10)
 
 
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestMissing:
@@ -133,15 +138,15 @@
         if netloc == "cloudreco.vuforia.com":
             assert response.text == "Malformed date header."
             assert_vwq_failure(
                 response=response,
                 status_code=HTTPStatus.UNAUTHORIZED,
                 content_type="text/plain;charset=iso-8859-1",
                 cache_control=None,
-                www_authenticate="VWS",
+                www_authenticate="KWS",
                 connection="keep-alive",
             )
             return
 
         assert_vws_failure(
             response=response,
             status_code=HTTPStatus.BAD_REQUEST,
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_delete_target.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_delete_target.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """
 Tests for deleting targets.
 """
+from __future__ import annotations
 
 from http import HTTPStatus
+from typing import TYPE_CHECKING
 
 import pytest
 from mock_vws._constants import ResultCodes
-from vws import VWS
 from vws.exceptions.vws_exceptions import (
     ProjectInactive,
     TargetStatusProcessing,
     UnknownTarget,
 )
 
 from tests.mock_vws.utils.assertions import assert_vws_failure
 
+if TYPE_CHECKING:
+    from vws import VWS
+
 
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestDelete:
     """
     Tests for deleting targets.
     """
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_get_duplicates.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_get_duplicates.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 """
 Tests for the mock of the get duplicates endpoint.
 """
+from __future__ import annotations
 
+import copy
 import io
 import uuid
+from typing import TYPE_CHECKING
 
 import pytest
-from vws import VWS
+from PIL import Image
 from vws.exceptions.vws_exceptions import ProjectInactive
 from vws.reports import TargetStatuses
 
+if TYPE_CHECKING:
+    from vws import VWS
+
 
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestDuplicates:
     """
     Tests for the mock of the target duplicates endpoint.
     """
 
     @staticmethod
     def test_duplicates(
         high_quality_image: io.BytesIO,
         image_file_success_state_low_rating: io.BytesIO,
         vws_client: VWS,
     ) -> None:
         """
-        Target IDs of similar targets are returned.
-
-        In the mock, "similar" means that the images are exactly the same.
+        Target IDs of the exact same targets are returned.
         """
         image_data = high_quality_image
         different_image_data = image_file_success_state_low_rating
 
         original_target_id = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
@@ -62,14 +66,55 @@
         duplicates = vws_client.get_duplicate_targets(
             target_id=original_target_id,
         )
 
         assert duplicates == [similar_target_id]
 
     @staticmethod
+    def test_duplicates_not_same(
+        high_quality_image: io.BytesIO,
+        vws_client: VWS,
+    ) -> None:
+        """
+        Target IDs of similar targets are returned.
+        """
+        image_data = high_quality_image
+        similar_image_data = copy.copy(image_data)
+        similar_image_buffer = io.BytesIO()
+        pil_similar_image = Image.open(similar_image_data)
+        # Re-save means similar but not identical.
+        pil_similar_image.save(similar_image_buffer, format="JPEG")
+        assert similar_image_buffer.getvalue() != image_data.getvalue()
+
+        original_target_id = vws_client.add_target(
+            name=uuid.uuid4().hex,
+            width=1,
+            image=image_data,
+            active_flag=True,
+            application_metadata=None,
+        )
+
+        similar_target_id = vws_client.add_target(
+            name=uuid.uuid4().hex,
+            width=1,
+            image=similar_image_buffer,
+            active_flag=True,
+            application_metadata=None,
+        )
+
+        vws_client.wait_for_target_processed(target_id=original_target_id)
+        vws_client.wait_for_target_processed(target_id=similar_target_id)
+
+        duplicates = vws_client.get_duplicate_targets(
+            target_id=original_target_id,
+        )
+
+        assert duplicates == [similar_target_id]
+
+    @staticmethod
     def test_status(
         image_file_failed_state: io.BytesIO,
         vws_client: VWS,
     ) -> None:
         """
         Targets are not duplicates if the status is not 'success'.
         """
@@ -201,14 +246,17 @@
             target_id=processing_target_id,
         )
 
         target_details = vws_client.get_target_record(
             target_id=processing_target_id,
         )
 
+        # There is a race condition here.
+        # If getting the target details and getting the duplicates takes longer
+        # than the processing time, the target will be in the success state.
         assert target_details.status == TargetStatuses.PROCESSING
         assert duplicates == [processed_target_id]
 
 
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestInactiveProject:
     """
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_get_target.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_get_target.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """
 Tests for getting a target record.
 
 https://library.vuforia.com/articles/Solution/How-To-Use-the-Vuforia-Web-Services-API.html#How-To-Retrieve-a-Target-Record
 """
+from __future__ import annotations
 
-import io
 import uuid
+from typing import TYPE_CHECKING
 
 import pytest
-from vws import VWS
 from vws.exceptions.vws_exceptions import UnknownTarget
 from vws.reports import TargetRecord, TargetStatuses
 
+if TYPE_CHECKING:
+    import io
+
+    from vws import VWS
+
 
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestGetRecord:
     """
     Tests for getting a target record.
     """
 
@@ -110,14 +115,70 @@
 
         # The tracking rating stays stable across requests
         target_details = vws_client.get_target_record(target_id=target_id)
         new_tracking_rating = target_details.target_record.tracking_rating
         assert new_tracking_rating == tracking_rating
 
 
+def _get_target_tracking_rating(
+    vws_client: VWS,
+    image_file: io.BytesIO,
+) -> int:
+    """
+    Get the tracking rating of a target.
+    """
+    target_id = vws_client.add_target(
+        name=f"example_{uuid.uuid4().hex}",
+        width=1,
+        image=image_file,
+        active_flag=True,
+        application_metadata=None,
+    )
+
+    vws_client.wait_for_target_processed(target_id=target_id)
+    target_details = vws_client.get_target_record(target_id=target_id)
+    return target_details.target_record.tracking_rating
+
+
+@pytest.mark.usefixtures("verify_mock_vuforia")
+class TestTargetTrackingRating:
+    """
+    Tests which exercise the target tracking_rating, and check the image
+    fixtures we use.
+    """
+
+    @staticmethod
+    def test_target_quality(
+        vws_client: VWS,
+        high_quality_image: io.BytesIO,
+        image_file_success_state_low_rating: io.BytesIO,
+        corrupted_image_file: io.BytesIO,
+    ) -> None:
+        """
+        The target tracking rating is as expected.
+        """
+        high_quality_image_tracking_rating = _get_target_tracking_rating(
+            vws_client=vws_client,
+            image_file=high_quality_image,
+        )
+        low_quality_image_tracking_rating = _get_target_tracking_rating(
+            vws_client=vws_client,
+            image_file=image_file_success_state_low_rating,
+        )
+        corrupted_image_file_tracking_rating = _get_target_tracking_rating(
+            vws_client=vws_client,
+            image_file=corrupted_image_file,
+        )
+        assert (
+            high_quality_image_tracking_rating
+            > low_quality_image_tracking_rating
+            >= corrupted_image_file_tracking_rating
+        )
+
+
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestInactiveProject:
     """
     Tests for inactive projects.
     """
 
     @staticmethod
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_invalid_json.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_invalid_json.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 """
 Tests for giving invalid JSON to endpoints.
 """
 
+from __future__ import annotations
+
 from datetime import datetime, timedelta
 from http import HTTPStatus
+from typing import TYPE_CHECKING
 from urllib.parse import urlparse
 from zoneinfo import ZoneInfo
 
 import pytest
 import requests
 from freezegun import freeze_time
 from mock_vws._constants import ResultCodes
 from requests.structures import CaseInsensitiveDict
 from vws_auth_tools import authorization_header, rfc_1123_date
 
-from tests.mock_vws.utils import Endpoint
 from tests.mock_vws.utils.assertions import (
     assert_valid_date_header,
     assert_vwq_failure,
     assert_vws_failure,
 )
 
+if TYPE_CHECKING:
+    from tests.mock_vws.utils import Endpoint
+
 
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestInvalidJSON:
     """
     Tests for giving invalid JSON to endpoints.
     """
 
@@ -71,18 +76,19 @@
         takes_json_data = (
             endpoint.auth_header_content_type == "application/json"
         )
 
         assert_valid_date_header(response=response)
 
         if date_is_skewed and takes_json_data:
-            # On the real implementation, we get `HTTPStatus.FORBIDDEN` and
-            # `REQUEST_TIME_TOO_SKEWED`.
-            # See https://github.com/VWS-Python/vws-python-mock/issues/4 for
-            # implementing this on them mock.
+            assert_vws_failure(
+                response=response,
+                status_code=HTTPStatus.FORBIDDEN,
+                result_code=ResultCodes.REQUEST_TIME_TOO_SKEWED,
+            )
             return
 
         if not date_is_skewed and takes_json_data:
             assert_vws_failure(
                 response=response,
                 status_code=HTTPStatus.BAD_REQUEST,
                 result_code=ResultCodes.FAIL,
@@ -101,9 +107,9 @@
                 www_authenticate=None,
                 connection="keep-alive",
             )
             expected_text = "No image."
             assert response.text == expected_text
             return
 
-        assert response.text == ""
+        assert not response.text
         assert "Content-Type" not in response.headers
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_query.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 """
 Tests for the mock of the query endpoint.
 
-https://library.vuforia.com/articles/Solution/How-To-Perform-an-Image-Recognition-Query.
+https://library.vuforia.com/web-api/vuforia-query-web-api.
 """
 
 from __future__ import annotations
 
 import base64
 import calendar
+import copy
 import datetime
 import io
 import sys
 import textwrap
 import time
 import uuid
 from http import HTTPStatus
 from pathlib import Path
-from typing import Any
+from typing import TYPE_CHECKING, Any
 from urllib.parse import urljoin
 from zoneinfo import ZoneInfo
 
 import pytest
 import requests
 from mock_vws._constants import ResultCodes
-from mock_vws.database import VuforiaDatabase
 from PIL import Image
-from requests import Response
 from requests_mock import POST
 from urllib3.filepost import encode_multipart_formdata
-from vws import VWS, CloudRecoService
 from vws.reports import TargetStatuses
 from vws_auth_tools import authorization_header, rfc_1123_date
 
 from tests.mock_vws.utils import make_image_file
 from tests.mock_vws.utils.assertions import (
     assert_query_success,
     assert_valid_date_header,
     assert_valid_transaction_id,
     assert_vwq_failure,
 )
 
+if TYPE_CHECKING:
+    from mock_vws.database import VuforiaDatabase
+    from vws import VWS, CloudRecoService
+
 VWQ_HOST = "https://cloudreco.vuforia.com"
 
 _JETTY_CONTENT_TYPE_ERROR = textwrap.dedent(
     """\
     <html>
     <head>
     <meta http-equiv="Content-Type" content="text/html;charset=utf-8"/>
@@ -82,31 +84,29 @@
     _JETTY_ERROR_DELETION_NOT_COMPLETE_START_PATH.read_text()
 )
 
 
 def query(
     vuforia_database: VuforiaDatabase,
     body: dict[str, Any],
-) -> Response:
+) -> requests.Response:
     """
     Make a request to the endpoint to make an image recognition query.
 
     Args:
         vuforia_database: The credentials to use to connect to
             Vuforia.
         body: The request body to send in ``multipart/formdata`` format.
 
     Returns:
         The response returned by the API.
     """
     date = rfc_1123_date()
     request_path = "/v1/query"
-    content, content_type_header = encode_multipart_formdata(
-        fields=body,
-    )  # type: ignore[no-untyped-call]
+    content, content_type_header = encode_multipart_formdata(fields=body)
     method = POST
 
     access_key = vuforia_database.client_access_key
     secret_key = vuforia_database.client_secret_key
     authorization_string = authorization_header(
         access_key=access_key,
         secret_key=secret_key,
@@ -138,22 +138,22 @@
 class TestContentType:
     """
     Tests for the Content-Type header.
     """
 
     @staticmethod
     @pytest.mark.parametrize(
-        (
+        argnames=(
             "content_type",
             "resp_status_code",
             "resp_content_type",
             "resp_cache_control",
             "resp_text",
         ),
-        [
+        argvalues=[
             (
                 "text/html",
                 HTTPStatus.UNSUPPORTED_MEDIA_TYPE,
                 None,
                 None,
                 "",
             ),
@@ -202,17 +202,15 @@
         """
         With bad Content-Type headers we get a variety of results.
         """
         image_content = high_quality_image.getvalue()
         date = rfc_1123_date()
         request_path = "/v1/query"
         body = {"image": ("image.jpeg", image_content, "image/jpeg")}
-        content, _ = encode_multipart_formdata(
-            fields=body,
-        )  # type: ignore[no-untyped-call]
+        content, _ = encode_multipart_formdata(fields=body)
         method = POST
 
         access_key = vuforia_database.client_access_key
         secret_key = vuforia_database.client_secret_key
         authorization_string = authorization_header(
             access_key=access_key,
             secret_key=secret_key,
@@ -257,17 +255,15 @@
         with the correct boundary, an ``UNSUPPORTED_MEDIA_TYPE`` response is
         given.
         """
         image_content = high_quality_image.getvalue()
         date = rfc_1123_date()
         request_path = "/v1/query"
         body = {"image": ("image.jpeg", image_content, "image/jpeg")}
-        content, content_type_header = encode_multipart_formdata(
-            fields=body,
-        )  # type: ignore[no-untyped-call]
+        content, content_type_header = encode_multipart_formdata(fields=body)
         method = POST
 
         content_type = "text/html"
 
         access_key = vuforia_database.client_access_key
         secret_key = vuforia_database.client_secret_key
         authorization_string = authorization_header(
@@ -293,15 +289,15 @@
             method=method,
             url=urljoin(base=VWQ_HOST, url=request_path),
             headers=headers,
             data=content,
             timeout=30,
         )
 
-        assert response.text == ""
+        assert not response.text
         assert_vwq_failure(
             response=response,
             status_code=HTTPStatus.UNSUPPORTED_MEDIA_TYPE,
             content_type=None,
             cache_control=None,
             www_authenticate=None,
             connection="keep-alive",
@@ -324,17 +320,15 @@
         """
         If no boundary is given, a ``BAD_REQUEST`` is returned.
         """
         image_content = high_quality_image.getvalue()
         date = rfc_1123_date()
         request_path = "/v1/query"
         body = {"image": ("image.jpeg", image_content, "image/jpeg")}
-        content, _ = encode_multipart_formdata(
-            fields=body,
-        )  # type: ignore[no-untyped-call]
+        content, _ = encode_multipart_formdata(fields=body)
         method = POST
 
         access_key = vuforia_database.client_access_key
         secret_key = vuforia_database.client_secret_key
         authorization_string = authorization_header(
             access_key=access_key,
             secret_key=secret_key,
@@ -382,17 +376,15 @@
         """
         If a bogus boundary is given, a ``BAD_REQUEST`` is returned.
         """
         image_content = high_quality_image.getvalue()
         date = rfc_1123_date()
         request_path = "/v1/query"
         body = {"image": ("image.jpeg", image_content, "image/jpeg")}
-        content, _ = encode_multipart_formdata(
-            fields=body,
-        )  # type: ignore[no-untyped-call]
+        content, _ = encode_multipart_formdata(fields=body)
         method = POST
 
         access_key = vuforia_database.client_access_key
         secret_key = vuforia_database.client_secret_key
         authorization_string = authorization_header(
             access_key=access_key,
             secret_key=secret_key,
@@ -438,17 +430,15 @@
         If sections that are not the boundary section are given in the header,
         that is fine.
         """
         image_content = high_quality_image.getvalue()
         date = rfc_1123_date()
         request_path = "/v1/query"
         body = {"image": ("image.jpeg", image_content, "image/jpeg")}
-        content, content_type_header = encode_multipart_formdata(
-            fields=body,
-        )  # type: ignore[no-untyped-call]
+        content, content_type_header = encode_multipart_formdata(fields=body)
         method = POST
 
         access_key = vuforia_database.client_access_key
         secret_key = vuforia_database.client_secret_key
         authorization_string = authorization_header(
             access_key=access_key,
             secret_key=secret_key,
@@ -498,44 +488,46 @@
 
         response = query(vuforia_database=vuforia_database, body=body)
 
         assert_query_success(response=response)
         assert response.json()["results"] == []
 
     @staticmethod
-    def test_match(
+    def test_match_exact(
         high_quality_image: io.BytesIO,
         vuforia_database: VuforiaDatabase,
         vws_client: VWS,
     ) -> None:
         """
-        If the exact image that was added is queried for, target data is shown.
+        If the exact high quality image that was added is queried for, target
+        data is shown.
         """
-        image_content = high_quality_image.getvalue()
+        image_file = high_quality_image
+        image_content = image_file.getvalue()
         metadata_encoded = base64.b64encode(b"example").decode("ascii")
         name = "example_name"
 
         target_id = vws_client.add_target(
             name=name,
             width=1,
-            image=high_quality_image,
+            image=image_file,
             active_flag=True,
             application_metadata=metadata_encoded,
         )
 
         approximate_target_created = calendar.timegm(time.gmtime())
 
         vws_client.wait_for_target_processed(target_id=target_id)
 
         body = {"image": ("image.jpeg", image_content, "image/jpeg")}
 
         response = query(vuforia_database=vuforia_database, body=body)
 
         assert_query_success(response=response)
-        [result] = response.json()["results"]
+        (result,) = response.json()["results"]
         assert result.keys() == {"target_id", "target_data"}
         assert result["target_id"] == target_id
         target_data = result["target_data"]
         assert target_data.keys() == {
             "application_metadata",
             "name",
             "target_timestamp",
@@ -545,14 +537,87 @@
         target_timestamp = target_data["target_timestamp"]
         assert isinstance(target_timestamp, int)
         time_difference = abs(approximate_target_created - target_timestamp)
         max_time_difference = 5
         assert time_difference < max_time_difference
 
     @staticmethod
+    def test_low_quality_image(
+        image_file_success_state_low_rating: io.BytesIO,
+        cloud_reco_client: CloudRecoService,
+        vws_client: VWS,
+    ) -> None:
+        """
+        If the exact low quality image that was added is queried for, no
+        results are returned.
+        """
+        image_file = image_file_success_state_low_rating
+        metadata_encoded = base64.b64encode(b"example").decode("ascii")
+        name = "example_name"
+
+        target_id = vws_client.add_target(
+            name=name,
+            width=1,
+            image=image_file,
+            active_flag=True,
+            application_metadata=metadata_encoded,
+        )
+
+        vws_client.wait_for_target_processed(target_id=target_id)
+        matching_targets = cloud_reco_client.query(image=image_file)
+        assert not matching_targets
+
+    @staticmethod
+    def test_match_similar(
+        high_quality_image: io.BytesIO,
+        different_high_quality_image: io.BytesIO,
+        vws_client: VWS,
+        cloud_reco_client: CloudRecoService,
+    ) -> None:
+        """
+        If a similar image to one that was added is queried for, target data is
+        shown.
+        """
+        metadata_encoded = base64.b64encode(b"example").decode("ascii")
+        name_matching = "example_name_matching"
+        name_not_matching = "example_name_not_matching"
+
+        target_id_matching = vws_client.add_target(
+            name=name_matching,
+            width=1,
+            image=high_quality_image,
+            active_flag=True,
+            application_metadata=metadata_encoded,
+        )
+
+        target_id_not_matching = vws_client.add_target(
+            name=name_not_matching,
+            width=1,
+            image=different_high_quality_image,
+            active_flag=True,
+            application_metadata=metadata_encoded,
+        )
+
+        vws_client.wait_for_target_processed(target_id=target_id_matching)
+        vws_client.wait_for_target_processed(target_id=target_id_not_matching)
+
+        similar_image_buffer = io.BytesIO()
+        similar_image_data = copy.copy(high_quality_image)
+        pil_similar_image = Image.open(similar_image_data)
+        # Re-save means similar but not identical.
+        pil_similar_image.save(similar_image_buffer, format="JPEG")
+
+        (matching_target,) = cloud_reco_client.query(
+            image=similar_image_buffer,
+            max_num_results=5,
+        )
+
+        assert matching_target.target_id == target_id_matching
+
+    @staticmethod
     def test_not_base64_encoded_processable(
         high_quality_image: io.BytesIO,
         vuforia_database: VuforiaDatabase,
         vws_client: VWS,
         not_base64_encoded_processable: str,
     ) -> None:
         """
@@ -581,15 +646,15 @@
         vws_client.wait_for_target_processed(target_id=target_id)
 
         body = {"image": ("image.jpeg", image_content, "image/jpeg")}
 
         response = query(vuforia_database=vuforia_database, body=body)
 
         assert_query_success(response=response)
-        [result] = response.json()["results"]
+        (result,) = response.json()["results"]
         query_metadata = result["target_data"]["application_metadata"]
         mod_4_to_expected_metadata_original = {
             1: not_base64_encoded_processable[:-1],
             2: not_base64_encoded_processable + "==",
             3: not_base64_encoded_processable + "=",
         }
         expected_metadata_original = mod_4_to_expected_metadata_original[
@@ -732,15 +797,15 @@
 
         We assert that the response is a success, but not that the maximum
         number of results is enforced.
 
         This is because uploading 50 images would be very slow.
 
         The documentation at
-        https://library.vuforia.com/articles/Solution/How-To-Perform-an-Image-Recognition-Query
+        https://library.vuforia.com/web-api/vuforia-query-web-api
         states that this must be between 1 and 10, but in practice, 50 is the
         maximum.
         """
         image_content = high_quality_image.getvalue()
         body = {
             "image": ("image.jpeg", image_content, "image/jpeg"),
             "max_num_results": (None, num_results, "text/plain"),
@@ -786,15 +851,15 @@
         num_results: int,
     ) -> None:
         """
         An error is returned if ``max_num_results`` is given as an integer out
         of the range (1, 50).
 
         The documentation at
-        https://library.vuforia.com/articles/Solution/How-To-Perform-an-Image-Recognition-Query.
+        https://library.vuforia.com/web-api/vuforia-query-web-api.
         states that this must be between 1 and 10, but in practice, 50 is the
         maximum.
         """
         image_content = high_quality_image.getvalue()
         body = {
             "image": ("image.jpeg", image_content, "image/jpeg"),
             "max_num_results": (None, num_results, "text/plain"),
@@ -860,27 +925,27 @@
     image: io.BytesIO,
     vws_client: VWS,
     num_targets: int,
 ) -> None:
     """
     Add targets with the given image.
     """
-    target_ids = set()
+    target_ids: set[str] = set()
     for _ in range(num_targets):
         target_id = vws_client.add_target(
             name=uuid.uuid4().hex,
             width=1,
             image=image,
             active_flag=True,
             application_metadata=None,
         )
         target_ids.add(target_id)
 
-    for target_id in target_ids:
-        vws_client.wait_for_target_processed(target_id=target_id)
+    for created_target_id in target_ids:
+        vws_client.wait_for_target_processed(target_id=created_target_id)
 
 
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestIncludeTargetData:
     """
     Tests for the ``include_target_data`` parameter.
     """
@@ -1006,15 +1071,15 @@
         assert "target_data" in result_2
 
     @staticmethod
     @pytest.mark.parametrize("include_target_data", ["a", True, 0])
     def test_invalid_value(
         high_quality_image: io.BytesIO,
         vuforia_database: VuforiaDatabase,
-        include_target_data: Any,
+        include_target_data: str | bool | int,
     ) -> None:
         """
         A ``BAD_REQUEST`` error is given when a string that is not one of
         'none', 'top' or 'all' (case insensitive).
         """
         image_content = high_quality_image.getvalue()
         body = {
@@ -1064,17 +1129,15 @@
         """
         An ``Accept`` header can be given iff its value is "application/json".
         """
         image_content = high_quality_image.getvalue()
         date = rfc_1123_date()
         request_path = "/v1/query"
         body = {"image": ("image.jpeg", image_content, "image/jpeg")}
-        content, content_type_header = encode_multipart_formdata(
-            fields=body,
-        )  # type: ignore[no-untyped-call]
+        content, content_type_header = encode_multipart_formdata(fields=body)
         method = POST
 
         access_key = vuforia_database.client_access_key
         secret_key = vuforia_database.client_secret_key
         authorization_string = authorization_header(
             access_key=access_key,
             secret_key=secret_key,
@@ -1112,17 +1175,15 @@
         A NOT_ACCEPTABLE response is returned if an ``Accept`` header is given
         with a value which is not "application/json".
         """
         image_content = high_quality_image.getvalue()
         date = rfc_1123_date()
         request_path = "/v1/query"
         body = {"image": ("image.jpeg", image_content, "image/jpeg")}
-        content, content_type_header = encode_multipart_formdata(
-            fields=body,
-        )  # type: ignore[no-untyped-call]
+        content, content_type_header = encode_multipart_formdata(fields=body)
         method = POST
 
         access_key = vuforia_database.client_access_key
         secret_key = vuforia_database.client_secret_key
         authorization_string = authorization_header(
             access_key=access_key,
             secret_key=secret_key,
@@ -1265,15 +1326,15 @@
         ),
     )
     def test_png(
         vuforia_database: VuforiaDatabase,
     ) -> None:  # pragma: no cover
         """
         According to
-        https://library.vuforia.com/articles/Solution/How-To-Perform-an-Image-Recognition-Query.
+        https://library.vuforia.com/web-api/vuforia-query-web-api.
         the maximum file size is "2MiB for PNG".
 
         Above this limit, a ``REQUEST_ENTITY_TOO_LARGE`` response is returned.
         We do not test exactly at this limit, but that may be beneficial in the
         future.
         """
         max_bytes = 2 * 1024 * 1024
@@ -1346,15 +1407,15 @@
         ),
     )
     def test_jpeg(
         vuforia_database: VuforiaDatabase,
     ) -> None:  # pragma: no cover
         """
         According to
-        https://library.vuforia.com/articles/Solution/How-To-Perform-an-Image-Recognition-Query.
+        https://library.vuforia.com/web-api/vuforia-query-web-api.
         the maximum file size is "512 KiB for JPEG".
         However, this test shows that the maximum size for JPEG is 2 MiB.
 
         Above this limit, a ``REQUEST_ENTITY_TOO_LARGE`` response is returned.
         We do not test exactly at this limit, but that may be beneficial in the
         future.
         """
@@ -1542,14 +1603,37 @@
             '{"transaction_id": '
             f'"{transaction_id}",'
             f'"result_code":"{result_code}"'
             "}"
         )
         assert response.text == expected_text
 
+    @staticmethod
+    def test_max_pixels(vuforia_database: VuforiaDatabase) -> None:
+        """
+        No error is returned for an 835 x 835 image.
+        """
+        # If we make this 836 then we hit REQUEST_ENTITY_TOO_LARGE errors.
+        max_height = max_width = 835
+        png_not_too_wide = make_image_file(
+            file_format="PNG",
+            color_space="RGB",
+            width=max_width,
+            height=max_height,
+        )
+
+        image_content = png_not_too_wide.getvalue()
+
+        body = {"image": ("image.jpeg", image_content, "image/jpeg")}
+
+        response = query(vuforia_database=vuforia_database, body=body)
+
+        assert_query_success(response=response)
+        assert response.json()["results"] == []
+
 
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestImageFormats:
     """
     Tests for various image formats.
     """
 
@@ -1701,15 +1785,15 @@
 
         new_name = name + "2"
         new_metadata = metadata + b"2"
         new_metadata_encoded = base64.b64encode(new_metadata).decode("ascii")
 
         body = {"image": ("image.jpeg", image_content, "image/jpeg")}
         response = query(vuforia_database=vuforia_database, body=body)
-        [result] = response.json()["results"]
+        (result,) = response.json()["results"]
         target_data = result["target_data"]
         target_timestamp = target_data["target_timestamp"]
         original_target_timestamp = int(target_timestamp)
 
         vws_client.update_target(
             target_id=target_id,
             name=new_name,
@@ -1721,15 +1805,15 @@
 
         vws_client.wait_for_target_processed(target_id=target_id)
 
         body = {"image": ("image.jpeg", new_image_content, "image/jpeg")}
         response = query(vuforia_database=vuforia_database, body=body)
 
         assert_query_success(response=response)
-        [result] = response.json()["results"]
+        (result,) = response.json()["results"]
         assert result.keys() == {"target_id", "target_data"}
         assert result["target_id"] == target_id
         target_data = result["target_data"]
         assert target_data.keys() == {
             "application_metadata",
             "name",
             "target_timestamp",
@@ -1850,15 +1934,15 @@
                 assert response.text.startswith(
                     _JETTY_ERROR_DELETION_NOT_COMPLETE,
                 )
                 time.sleep(sleep_seconds)
                 total_waited += sleep_seconds
             else:
                 if response.json()["results"]:
-                    [result] = response.json()["results"]
+                    (result,) = response.json()["results"]
                     assert result["target_id"] == target_id
                     # We never see the target ID after having seen the server
                     # error.
                     assert not server_error_seen
                     time.sleep(sleep_seconds)
                     total_waited += sleep_seconds
                 else:
@@ -1977,17 +2061,15 @@
         if include_tz:
             datetime_format += " GMT"
 
         gmt = ZoneInfo("GMT")
         now = datetime.datetime.now(tz=gmt)
         date = now.strftime(datetime_format)
         request_path = "/v1/query"
-        content, content_type_header = encode_multipart_formdata(
-            fields=body,
-        )  # type: ignore[no-untyped-call]
+        content, content_type_header = encode_multipart_formdata(fields=body)
         method = POST
 
         access_key = vuforia_database.client_access_key
         secret_key = vuforia_database.client_secret_key
         authorization_string = authorization_header(
             access_key=access_key,
             secret_key=secret_key,
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_requests_mock_usage.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_flask_app_usage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,568 +1,571 @@
 """
-Tests for the usage of the mock for ``requests``.
+Tests for the usage of the mock Flask application.
 """
+from __future__ import annotations
 
-import datetime
-import email.utils
 import io
-import json
-import socket
+import uuid
+from http import HTTPStatus
+from typing import TYPE_CHECKING
 
 import pytest
 import requests
-from freezegun import freeze_time
-from mock_vws import MockVWS
+from mock_vws._flask_server.target_manager import TARGET_MANAGER_FLASK_APP
+from mock_vws._flask_server.vwq import CLOUDRECO_FLASK_APP
+from mock_vws._flask_server.vws import VWS_FLASK_APP
 from mock_vws.database import VuforiaDatabase
-from mock_vws.states import States
-from mock_vws.target import Target
-from requests.exceptions import MissingSchema
-from requests_mock.exceptions import NoMockAddress
-from vws import VWS
-from vws_auth_tools import rfc_1123_date
+from PIL import Image
+from requests_mock_flask import add_flask_app_to_mock
+from vws import VWS, CloudRecoService
 
 from tests.mock_vws.utils.usage_test_helpers import (
     process_deletion_seconds,
     processing_time_seconds,
     recognize_deletion_seconds,
 )
 
+if TYPE_CHECKING:
+    from requests_mock import Mocker
 
-def request_unmocked_address() -> None:
-    """
-    Make a request, using `requests` to an unmocked, free local address.
-
-    Raises:
-        requests.exceptions.ConnectionError: This is expected as there is
-            nothing to connect to.
-        requests_mock.exceptions.NoMockAddress: This request is being made in
-            the context of a `requests_mock` mock which does not mock local
-            addresses.
-    """
-    sock = socket.socket()
-    sock.bind(("", 0))
-    port = sock.getsockname()[1]
-    sock.close()
-    address = f"http://localhost:{port}"
-    requests.get(address, timeout=30)
-
-
-def request_mocked_address() -> None:
-    """
-    Make a request, using `requests` to an address that is mocked by `MockVWS`.
-    """
-    requests.get(
-        url="https://vws.vuforia.com/summary",
-        headers={
-            "Date": rfc_1123_date(),
-            "Authorization": "bad_auth_token",
-        },
-        data=b"",
-        timeout=30,
-    )
+_EXAMPLE_URL_FOR_TARGET_MANAGER = "http://" + uuid.uuid4().hex + ".com"
 
 
-class TestRealHTTP:
+@pytest.fixture(autouse=True)
+def _enable_requests_mock(
+    monkeypatch: pytest.MonkeyPatch,
+    requests_mock: Mocker,
+) -> None:
     """
-    Tests for making requests to mocked and unmocked addresses.
+    Enable a mock service backed by the Flask applications.
     """
+    add_flask_app_to_mock(
+        mock_obj=requests_mock,
+        flask_app=VWS_FLASK_APP,
+        base_url="https://vws.vuforia.com",
+    )
 
-    @staticmethod
-    def test_default() -> None:
-        """
-        By default, the mock stops any requests made with `requests` to
-        non-Vuforia addresses, but not to mocked Vuforia endpoints.
-        """
-        with MockVWS():
-            with pytest.raises(NoMockAddress):
-                request_unmocked_address()
-
-            # No exception is raised when making a request to a mocked
-            # endpoint.
-            request_mocked_address()
-
-        # The mocking stops when the context manager stops.
-        with pytest.raises(requests.exceptions.ConnectionError):
-            request_unmocked_address()
+    add_flask_app_to_mock(
+        mock_obj=requests_mock,
+        flask_app=CLOUDRECO_FLASK_APP,
+        base_url="https://cloudreco.vuforia.com",
+    )
 
-    @staticmethod
-    def test_real_http() -> None:
-        """
-        When the `real_http` parameter given to the context manager is set to
-        `True`, requests made to unmocked addresses are not stopped.
-        """
-        with (
-            MockVWS(real_http=True),
-            pytest.raises(requests.exceptions.ConnectionError),
-        ):
-            request_unmocked_address()
+    add_flask_app_to_mock(
+        mock_obj=requests_mock,
+        flask_app=TARGET_MANAGER_FLASK_APP,
+        base_url=_EXAMPLE_URL_FOR_TARGET_MANAGER,
+    )
+
+    monkeypatch.setenv(
+        name="TARGET_MANAGER_BASE_URL",
+        value=_EXAMPLE_URL_FOR_TARGET_MANAGER,
+    )
 
 
 class TestProcessingTime:
     """
     Tests for the time taken to process targets in the mock.
     """
 
     # There is a race condition in this test type - if tests start to
     # fail, consider increasing the leeway.
-    LEEWAY = 0.1
+    LEEWAY = 0.5
 
-    def test_default(self, image_file_failed_state: io.BytesIO) -> None:
+    def test_default(
+        self,
+        image_file_failed_state: io.BytesIO,
+    ) -> None:
         """
-        By default, targets in the mock take 0.5 seconds to be processed.
+        By default, targets in the mock takes 2 seconds to be processed.
         """
         database = VuforiaDatabase()
-        with MockVWS() as mock:
-            mock.add_database(database=database)
-            time_taken = processing_time_seconds(
-                vuforia_database=database,
-                image=image_file_failed_state,
-            )
+        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
+        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
 
-        expected = 0.5
-        assert abs(expected - time_taken) < self.LEEWAY
+        time_taken = processing_time_seconds(
+            vuforia_database=database,
+            image=image_file_failed_state,
+        )
+
+        expected = 2
+        assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
 
-    def test_custom(self, image_file_failed_state: io.BytesIO) -> None:
+    def test_custom(
+        self,
+        image_file_failed_state: io.BytesIO,
+        monkeypatch: pytest.MonkeyPatch,
+    ) -> None:
         """
         It is possible to set a custom processing time.
         """
+        seconds = 5
+        monkeypatch.setenv(
+            name="PROCESSING_TIME_SECONDS",
+            value=str(seconds),
+        )
         database = VuforiaDatabase()
-        with MockVWS(processing_time_seconds=0.1) as mock:
-            mock.add_database(database=database)
-            time_taken = processing_time_seconds(
-                vuforia_database=database,
-                image=image_file_failed_state,
-            )
-
-        expected = 0.1
-        assert abs(expected - time_taken) < self.LEEWAY
+        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
+        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
 
-
-class TestDatabaseName:
-    """
-    Tests for the database name.
-    """
-
-    @staticmethod
-    def test_default() -> None:
-        """
-        By default, the database has a random name.
-        """
-        database_details = VuforiaDatabase()
-        other_database_details = VuforiaDatabase()
-        assert (
-            database_details.database_name
-            != other_database_details.database_name
+        time_taken = processing_time_seconds(
+            vuforia_database=database,
+            image=image_file_failed_state,
         )
 
-    @staticmethod
-    def test_custom_name() -> None:
-        """
-        It is possible to set a custom database name.
-        """
-        database_details = VuforiaDatabase(database_name="foo")
-        assert database_details.database_name == "foo"
-
-
-class TestCustomBaseURLs:
-    """
-    Tests for using custom base URLs.
-    """
-
-    @staticmethod
-    def test_custom_base_vws_url() -> None:
-        """
-        It is possible to use a custom base VWS URL.
-        """
-        with MockVWS(
-            base_vws_url="https://vuforia.vws.example.com",
-            real_http=False,
-        ):
-            with pytest.raises(NoMockAddress):
-                requests.get(url="https://vws.vuforia.com/summary", timeout=30)
-
-            requests.get(
-                url="https://vuforia.vws.example.com/summary",
-                timeout=30,
-            )
-            requests.post(
-                url="https://cloudreco.vuforia.com/v1/query",
-                timeout=30,
-            )
-
-    @staticmethod
-    def test_custom_base_vwq_url() -> None:
-        """
-        It is possible to use a custom base cloud recognition URL.
-        """
-        with MockVWS(
-            base_vwq_url="https://vuforia.vwq.example.com",
-            real_http=False,
-        ):
-            with pytest.raises(NoMockAddress):
-                requests.post(
-                    url="https://cloudreco.vuforia.com/v1/query",
-                    timeout=30,
-                )
-
-            requests.post(
-                url="https://vuforia.vwq.example.com/v1/query",
-                timeout=30,
-            )
-            requests.get(
-                url="https://vws.vuforia.com/summary",
-                timeout=30,
-            )
-
-    @staticmethod
-    def test_no_scheme() -> None:
-        """
-        An error if raised if a URL is given with no scheme.
-        """
-        with pytest.raises(MissingSchema) as exc:
-            MockVWS(base_vws_url="vuforia.vws.example.com")
-
-        expected = (
-            'Invalid URL "vuforia.vws.example.com": No scheme supplied. '
-            'Perhaps you meant "https://vuforia.vws.example.com".'
-        )
-        assert str(exc.value) == expected
-        with pytest.raises(MissingSchema) as exc:
-            MockVWS(base_vwq_url="vuforia.vwq.example.com")
-        expected = (
-            'Invalid URL "vuforia.vwq.example.com": No scheme supplied. '
-            'Perhaps you meant "https://vuforia.vwq.example.com".'
-        )
-        assert str(exc.value) == expected
+        expected = seconds
+        assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
 
 
 class TestCustomQueryRecognizesDeletionSeconds:
     """
     Tests for setting the amount of time after a target has been deleted
     until it is not recognized by the query endpoint.
     """
 
-    LEEWAY = 0.15
+    LEEWAY = 0.5
 
     def test_default(
         self,
         high_quality_image: io.BytesIO,
+        monkeypatch: pytest.MonkeyPatch,
     ) -> None:
         """
-        By default it takes zero seconds for the Query API on the mock to
+        By default it takes 2 seconds for the Query API on the mock to
         recognize that a target has been deleted.
 
         The real Query API takes between zero and two seconds.
         See ``test_query`` for more information.
         """
         database = VuforiaDatabase()
-        with MockVWS() as mock:
-            mock.add_database(database=database)
-            time_taken = recognize_deletion_seconds(
-                high_quality_image=high_quality_image,
-                vuforia_database=database,
-            )
-
-        expected = 0.2
-        assert abs(expected - time_taken) < self.LEEWAY
-
-    def test_with_no_processing_time(
-        self,
-        high_quality_image: io.BytesIO,
-    ) -> None:
-        """
-        We test this because it exercises some otherwise untouched code.
-        """
-        database = VuforiaDatabase()
-        with MockVWS(query_processes_deletion_seconds=0) as mock:
-            mock.add_database(database=database)
-            time_taken = recognize_deletion_seconds(
-                high_quality_image=high_quality_image,
-                vuforia_database=database,
-            )
-
-        expected = 0.2
-        assert abs(expected - time_taken) < self.LEEWAY
-
+        # Use the "exact" matcher, as it is the fastest.
+        monkeypatch.setenv(name="QUERY_IMAGE_MATCHER", value="exact")
+        # Use the fastest tracking rater.
+        monkeypatch.setenv(name="TARGET_RATER", value="perfect")
+        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
+        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
+        time_taken = recognize_deletion_seconds(
+            high_quality_image=high_quality_image,
+            vuforia_database=database,
+        )
+
+        expected = 2
+        assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
+
+    @pytest.mark.parametrize(
+        argnames=["seconds"],
+        # We include 0 because it exercises some otherwise untouched code.
+        argvalues=[(0,), (5,)],
+    )
     def test_custom(
         self,
         high_quality_image: io.BytesIO,
+        monkeypatch: pytest.MonkeyPatch,
+        seconds: int | float,
     ) -> None:
         """
         It is possible to use set a custom amount of time that it takes for the
         Query API on the mock to recognize that a target has been deleted.
         """
-        # We choose a low time for a quick test.
-        query_recognizes_deletion = 0.5
         database = VuforiaDatabase()
-        with MockVWS(
-            query_recognizes_deletion_seconds=query_recognizes_deletion,
-        ) as mock:
-            mock.add_database(database=database)
-            time_taken = recognize_deletion_seconds(
-                high_quality_image=high_quality_image,
-                vuforia_database=database,
-            )
+        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
+        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
+        monkeypatch.setenv(
+            name="DELETION_RECOGNITION_SECONDS",
+            value=str(seconds),
+        )
+        # Use the "exact" matcher, as it is the fastest.
+        monkeypatch.setenv(name="QUERY_IMAGE_MATCHER", value="exact")
+        time_taken = recognize_deletion_seconds(
+            high_quality_image=high_quality_image,
+            vuforia_database=database,
+        )
 
-        expected = query_recognizes_deletion
-        assert abs(expected - time_taken) < self.LEEWAY
+        expected = seconds
+        assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
 
 
 class TestCustomQueryProcessDeletionSeconds:
     """
     Tests for setting the amount of time after a target has been deleted
     until it is not processed by the query endpoint.
     """
 
     # There is a race condition in this test type - if tests start to
     # fail, consider increasing the leeway.
-    LEEWAY = 0.2
+    LEEWAY = 0.5
 
     def test_default(
         self,
         high_quality_image: io.BytesIO,
+        monkeypatch: pytest.MonkeyPatch,
     ) -> None:
         """
         By default it takes three seconds for the Query API on the mock to
         process that a target has been deleted.
 
         The real Query API takes between seven and thirty seconds.
         See ``test_query`` for more information.
         """
+        # Use the "exact" matcher, as it is the fastest.
+        monkeypatch.setenv(name="QUERY_IMAGE_MATCHER", value="exact")
+        # Use the fastest tracking rater.
+        monkeypatch.setenv(name="TARGET_RATER", value="perfect")
         database = VuforiaDatabase()
-        with MockVWS() as mock:
-            mock.add_database(database=database)
-            time_taken = process_deletion_seconds(
-                high_quality_image=high_quality_image,
-                vuforia_database=database,
-            )
+        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
+        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
+        time_taken = process_deletion_seconds(
+            high_quality_image=high_quality_image,
+            vuforia_database=database,
+        )
 
         expected = 3
-        assert abs(expected - time_taken) < self.LEEWAY
+        # We minus the leeway because we might start the timer after the
+        # deletion processing has started.
+        assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
 
     def test_custom(
         self,
         high_quality_image: io.BytesIO,
+        monkeypatch: pytest.MonkeyPatch,
     ) -> None:
         """
         It is possible to use set a custom amount of time that it takes for the
         Query API on the mock to process that a target has been deleted.
         """
+        # Use the "exact" matcher, as it is the fastest.
+        monkeypatch.setenv(name="QUERY_IMAGE_MATCHER", value="exact")
+        # Use the fastest tracking rater.
+        monkeypatch.setenv(name="TARGET_RATER", value="perfect")
         # We choose a low time for a quick test.
-        query_processes_deletion = 0.1
+        query_processes_deletion = 5
         database = VuforiaDatabase()
-        with MockVWS(
-            query_processes_deletion_seconds=query_processes_deletion,
-        ) as mock:
-            mock.add_database(database=database)
-            time_taken = process_deletion_seconds(
-                high_quality_image=high_quality_image,
-                vuforia_database=database,
-            )
+        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
+        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
+        monkeypatch.setenv(
+            name="DELETION_PROCESSING_SECONDS",
+            value=str(query_processes_deletion),
+        )
+        time_taken = process_deletion_seconds(
+            high_quality_image=high_quality_image,
+            vuforia_database=database,
+        )
 
         expected = query_processes_deletion
-        assert abs(expected - time_taken) < self.LEEWAY
+        # We minus the leeway because we might start the timer after the
+        # deletion processing has started.
+        assert expected - self.LEEWAY < time_taken < expected + self.LEEWAY
 
 
-class TestStates:
+class TestAddDatabase:
     """
-    Tests for different mock states.
+    Tests for adding databases to the mock.
     """
 
     @staticmethod
-    def test_repr() -> None:
+    def test_duplicate_keys() -> None:
         """
-        The representation of a ``State`` shows the state.
+        It is not possible to have multiple databases with matching keys.
         """
-        assert repr(States.WORKING) == "<States.WORKING>"
+        database = VuforiaDatabase(
+            server_access_key="1",
+            server_secret_key="2",
+            client_access_key="3",
+            client_secret_key="4",
+            database_name="5",
+        )
 
+        bad_server_access_key_db = VuforiaDatabase(server_access_key="1")
+        bad_server_secret_key_db = VuforiaDatabase(server_secret_key="2")
+        bad_client_access_key_db = VuforiaDatabase(client_access_key="3")
+        bad_client_secret_key_db = VuforiaDatabase(client_secret_key="4")
+        bad_database_name_db = VuforiaDatabase(database_name="5")
 
-class TestTargets:
-    """
-    Tests for target representations.
-    """
+        server_access_key_conflict_error = (
+            "All server access keys must be unique. "
+            'There is already a database with the server access key "1".'
+        )
+        server_secret_key_conflict_error = (
+            "All server secret keys must be unique. "
+            'There is already a database with the server secret key "2".'
+        )
+        client_access_key_conflict_error = (
+            "All client access keys must be unique. "
+            'There is already a database with the client access key "3".'
+        )
+        client_secret_key_conflict_error = (
+            "All client secret keys must be unique. "
+            'There is already a database with the client secret key "4".'
+        )
+        database_name_conflict_error = (
+            "All names must be unique. "
+            'There is already a database with the name "5".'
+        )
+
+        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
+        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
+
+        for bad_database, expected_message in (
+            (bad_server_access_key_db, server_access_key_conflict_error),
+            (bad_server_secret_key_db, server_secret_key_conflict_error),
+            (bad_client_access_key_db, client_access_key_conflict_error),
+            (bad_client_secret_key_db, client_secret_key_conflict_error),
+            (bad_database_name_db, database_name_conflict_error),
+        ):
+            response = requests.post(
+                url=databases_url,
+                json=bad_database.to_dict(),
+                timeout=30,
+            )
+
+            assert response.status_code == HTTPStatus.CONFLICT
+            assert response.text == expected_message
 
     @staticmethod
-    def test_to_dict(high_quality_image: io.BytesIO) -> None:
+    def test_give_no_details(high_quality_image: io.BytesIO) -> None:
         """
-        It is possible to dump a target to a dictionary and load it back.
+        It is possible to create a database without giving any data.
         """
-        database = VuforiaDatabase()
+        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
+        response = requests.post(url=databases_url, json={}, timeout=30)
+        assert response.status_code == HTTPStatus.CREATED
+
+        data = response.json()
+
+        assert data["targets"] == []
+        assert data["state_name"] == "WORKING"
+        assert "database_name" in data
 
         vws_client = VWS(
-            server_access_key=database.server_access_key,
-            server_secret_key=database.server_secret_key,
+            server_access_key=data["server_access_key"],
+            server_secret_key=data["server_secret_key"],
         )
 
-        with MockVWS() as mock:
-            mock.add_database(database=database)
-            vws_client.add_target(
-                name="example",
-                width=1,
-                image=high_quality_image,
-                active_flag=True,
-                application_metadata=None,
-            )
+        cloud_reco_client = CloudRecoService(
+            client_access_key=data["client_access_key"],
+            client_secret_key=data["client_secret_key"],
+        )
 
-        (target,) = database.targets
-        target_dict = target.to_dict()
+        assert not vws_client.list_targets()
+        assert not cloud_reco_client.query(image=high_quality_image)
 
-        # The dictionary is JSON dump-able
-        assert json.dumps(target_dict)
 
-        new_target = Target.from_dict(target_dict=target_dict)
-        assert new_target == target
+class TestDeleteDatabase:
+    """
+    Tests for deleting databases from the mock.
+    """
 
     @staticmethod
-    def test_to_dict_deleted(high_quality_image: io.BytesIO) -> None:
+    def test_not_found() -> None:
         """
-        It is possible to dump a deleted target to a dictionary and load it
-        back.
+        A 404 error is returned when trying to delete a database which does not
+        exist.
         """
-        database = VuforiaDatabase()
+        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
+        delete_url = databases_url + "/" + "foobar"
+        response = requests.delete(url=delete_url, json={}, timeout=30)
+        assert response.status_code == HTTPStatus.NOT_FOUND
 
-        vws_client = VWS(
-            server_access_key=database.server_access_key,
-            server_secret_key=database.server_secret_key,
-        )
-
-        with MockVWS() as mock:
-            mock.add_database(database=database)
-            target_id = vws_client.add_target(
-                name="example",
-                width=1,
-                image=high_quality_image,
-                active_flag=True,
-                application_metadata=None,
-            )
-            vws_client.wait_for_target_processed(target_id=target_id)
-            vws_client.delete_target(target_id=target_id)
-
-        (target,) = database.targets
-        target_dict = target.to_dict()
+    @staticmethod
+    def test_delete_database() -> None:
+        """
+        It is possible to delete a database.
+        """
+        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
+        response = requests.post(url=databases_url, json={}, timeout=30)
+        assert response.status_code == HTTPStatus.CREATED
 
-        # The dictionary is JSON dump-able
-        assert json.dumps(target_dict)
+        data = response.json()
+        delete_url = databases_url + "/" + data["database_name"]
+        response = requests.delete(url=delete_url, json={}, timeout=30)
+        assert response.status_code == HTTPStatus.OK
 
-        new_target = Target.from_dict(target_dict=target_dict)
-        assert new_target.delete_date == target.delete_date
+        response = requests.delete(url=delete_url, json={}, timeout=30)
+        assert response.status_code == HTTPStatus.NOT_FOUND
 
 
-class TestDatabaseToDict:
-    """
-    Tests for dumping a database to a dictionary.
-    """
+class TestQueryImageMatchers:
+    """Tests for query image matchers."""
 
     @staticmethod
-    def test_to_dict(high_quality_image: io.BytesIO) -> None:
-        """
-        It is possible to dump a database to a dictionary and load it back.
-        """
+    def test_exact_match(
+        high_quality_image: io.BytesIO,
+        monkeypatch: pytest.MonkeyPatch,
+    ) -> None:
+        """The exact matcher matches only exactly the same images."""
+        monkeypatch.setenv(name="QUERY_IMAGE_MATCHER", value="exact")
+
         database = VuforiaDatabase()
+
         vws_client = VWS(
             server_access_key=database.server_access_key,
             server_secret_key=database.server_secret_key,
         )
+        cloud_reco_client = CloudRecoService(
+            client_access_key=database.client_access_key,
+            client_secret_key=database.client_secret_key,
+        )
 
-        # We test a database with a target added.
-        with MockVWS() as mock:
-            mock.add_database(database=database)
-            vws_client.add_target(
-                name="example",
-                width=1,
-                image=high_quality_image,
-                active_flag=True,
-                application_metadata=None,
-            )
+        pil_image = Image.open(fp=high_quality_image)
+        re_exported_image = io.BytesIO()
+        pil_image.save(re_exported_image, format="PNG")
 
-        database_dict = database.to_dict()
-        # The dictionary is JSON dump-able
-        assert json.dumps(database_dict)
+        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
+        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
 
-        new_database = VuforiaDatabase.from_dict(database_dict=database_dict)
-        assert new_database == database
+        target_id = vws_client.add_target(
+            name="example",
+            width=1,
+            image=high_quality_image,
+            application_metadata=None,
+            active_flag=True,
+        )
+        vws_client.wait_for_target_processed(target_id=target_id)
+        same_image_result = cloud_reco_client.query(
+            image=high_quality_image,
+        )
+        assert len(same_image_result) == 1
+        different_image_result = cloud_reco_client.query(
+            image=re_exported_image,
+        )
+        assert not different_image_result
 
+    @staticmethod
+    def test_average_hash_matcher(
+        high_quality_image: io.BytesIO,
+        different_high_quality_image: io.BytesIO,
+        monkeypatch: pytest.MonkeyPatch,
+    ) -> None:
+        """The average hash matcher matches similar images."""
+        monkeypatch.setenv(name="QUERY_IMAGE_MATCHER", value="average_hash")
+        database = VuforiaDatabase()
+        vws_client = VWS(
+            server_access_key=database.server_access_key,
+            server_secret_key=database.server_secret_key,
+        )
+        cloud_reco_client = CloudRecoService(
+            client_access_key=database.client_access_key,
+            client_secret_key=database.client_secret_key,
+        )
 
-class TestDateHeader:
-    """
-    Tests for the date header in responses from mock routes.
-    """
+        pil_image = Image.open(fp=high_quality_image)
+        re_exported_image = io.BytesIO()
+        pil_image.save(re_exported_image, format="PNG")
+        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
+        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
 
-    @staticmethod
-    def test_date_changes() -> None:
-        """
-        The date that the response is sent is in the response Date header.
-        """
-        new_year = 2012
-        new_time = datetime.datetime(new_year, 1, 1, tzinfo=datetime.UTC)
-        with MockVWS(), freeze_time(new_time):
-            response = requests.get(
-                url="https://vws.vuforia.com/summary",
-                timeout=30,
-            )
+        target_id = vws_client.add_target(
+            name="example",
+            width=1,
+            image=high_quality_image,
+            application_metadata=None,
+            active_flag=True,
+        )
+        vws_client.wait_for_target_processed(target_id=target_id)
+        same_image_result = cloud_reco_client.query(
+            image=high_quality_image,
+        )
+        assert len(same_image_result) == 1
+        similar_image_result = cloud_reco_client.query(
+            image=re_exported_image,
+        )
+        assert len(similar_image_result) == 1
 
-        date_response = response.headers["Date"]
-        date_from_response = email.utils.parsedate(date_response)
-        assert date_from_response is not None
-        year = date_from_response[0]
-        assert year == new_year
+        different_image_result = cloud_reco_client.query(
+            image=different_high_quality_image,
+        )
+        assert not different_image_result
 
 
-class TestAddDatabase:
-    """
-    Tests for adding databases to the mock.
-    """
+class TestDuplicatesImageMatchers:
+    """Tests for duplicates image matchers."""
 
     @staticmethod
-    def test_duplicate_keys() -> None:
-        """
-        It is not possible to have multiple databases with matching keys.
-        """
-        database = VuforiaDatabase(
-            server_access_key="1",
-            server_secret_key="2",
-            client_access_key="3",
-            client_secret_key="4",
-            database_name="5",
+    def test_exact_match(
+        high_quality_image: io.BytesIO,
+        monkeypatch: pytest.MonkeyPatch,
+    ) -> None:
+        """The exact matcher matches only exactly the same images."""
+        monkeypatch.setenv(name="DUPLICATES_IMAGE_MATCHER", value="exact")
+        database = VuforiaDatabase()
+        vws_client = VWS(
+            server_access_key=database.server_access_key,
+            server_secret_key=database.server_secret_key,
         )
 
-        bad_server_access_key_db = VuforiaDatabase(server_access_key="1")
-        bad_server_secret_key_db = VuforiaDatabase(server_secret_key="2")
-        bad_client_access_key_db = VuforiaDatabase(client_access_key="3")
-        bad_client_secret_key_db = VuforiaDatabase(client_secret_key="4")
-        bad_database_name_db = VuforiaDatabase(database_name="5")
-
-        server_access_key_conflict_error = (
-            "All server access keys must be unique. "
-            'There is already a database with the server access key "1".'
-        )
-        server_secret_key_conflict_error = (
-            "All server secret keys must be unique. "
-            'There is already a database with the server secret key "2".'
-        )
-        client_access_key_conflict_error = (
-            "All client access keys must be unique. "
-            'There is already a database with the client access key "3".'
+        pil_image = Image.open(fp=high_quality_image)
+        re_exported_image = io.BytesIO()
+        pil_image.save(re_exported_image, format="PNG")
+
+        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
+        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
+
+        target_id = vws_client.add_target(
+            name="example_0",
+            width=1,
+            image=high_quality_image,
+            application_metadata=None,
+            active_flag=True,
+        )
+        duplicate_target_id = vws_client.add_target(
+            name="example_1",
+            width=1,
+            image=high_quality_image,
+            application_metadata=None,
+            active_flag=True,
+        )
+        not_duplicate_target_id = vws_client.add_target(
+            name="example_2",
+            width=1,
+            image=re_exported_image,
+            application_metadata=None,
+            active_flag=True,
+        )
+        vws_client.wait_for_target_processed(target_id=target_id)
+        vws_client.wait_for_target_processed(target_id=duplicate_target_id)
+        vws_client.wait_for_target_processed(
+            target_id=not_duplicate_target_id,
         )
-        client_secret_key_conflict_error = (
-            "All client secret keys must be unique. "
-            'There is already a database with the client secret key "4".'
+        duplicates = vws_client.get_duplicate_targets(target_id=target_id)
+        assert duplicates == [duplicate_target_id]
+
+    @staticmethod
+    def test_average_hash_matcher(
+        high_quality_image: io.BytesIO,
+        monkeypatch: pytest.MonkeyPatch,
+    ) -> None:
+        """The average hash matcher matches similar images."""
+        monkeypatch.setenv(
+            name="DUPLICATES_IMAGE_MATCHER",
+            value="average_hash",
         )
-        database_name_conflict_error = (
-            "All names must be unique. "
-            'There is already a database with the name "5".'
+        database = VuforiaDatabase()
+        vws_client = VWS(
+            server_access_key=database.server_access_key,
+            server_secret_key=database.server_secret_key,
         )
 
-        with MockVWS() as mock:
-            mock.add_database(database=database)
-            for bad_database, expected_message in (
-                (bad_server_access_key_db, server_access_key_conflict_error),
-                (bad_server_secret_key_db, server_secret_key_conflict_error),
-                (bad_client_access_key_db, client_access_key_conflict_error),
-                (bad_client_secret_key_db, client_secret_key_conflict_error),
-                (bad_database_name_db, database_name_conflict_error),
-            ):
-                with pytest.raises(
-                    ValueError,
-                    match=expected_message + "$",
-                ):
-                    mock.add_database(database=bad_database)
+        pil_image = Image.open(fp=high_quality_image)
+        re_exported_image = io.BytesIO()
+        pil_image.save(re_exported_image, format="PNG")
+
+        databases_url = _EXAMPLE_URL_FOR_TARGET_MANAGER + "/databases"
+        requests.post(url=databases_url, json=database.to_dict(), timeout=30)
+
+        target_id = vws_client.add_target(
+            name="example",
+            width=1,
+            image=high_quality_image,
+            application_metadata=None,
+            active_flag=True,
+        )
+        duplicate_target_id = vws_client.add_target(
+            name="example_1",
+            width=1,
+            image=re_exported_image,
+            application_metadata=None,
+            active_flag=True,
+        )
+        vws_client.wait_for_target_processed(target_id=target_id)
+        vws_client.wait_for_target_processed(target_id=duplicate_target_id)
+        duplicates = vws_client.get_duplicate_targets(target_id=target_id)
+        assert duplicates == [duplicate_target_id]
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_target_list.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_target_list.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 """
 Tests for the mock of the target list endpoint.
 """
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
 
 import pytest
-from vws import VWS
+
+if TYPE_CHECKING:
+    from vws import VWS
 
 
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestTargetList:
     """
     Tests for the mock of the target list endpoint at `/targets`.
     """
@@ -28,15 +33,15 @@
         target_id: str,
     ) -> None:
         """
         Deleted targets are not returned in the list.
         """
         vws_client.wait_for_target_processed(target_id=target_id)
         vws_client.delete_target(target_id=target_id)
-        assert vws_client.list_targets() == []
+        assert not vws_client.list_targets()
 
 
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestInactiveProject:
     """
     Tests for inactive projects.
     """
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_target_summary.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_target_summary.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 """
 Tests for the mock of the target summary endpoint.
 """
 
+from __future__ import annotations
+
 import datetime
-import io
 import uuid
+from typing import TYPE_CHECKING
 from zoneinfo import ZoneInfo
 
 import pytest
-from _pytest.fixtures import SubRequest
-from mock_vws.database import VuforiaDatabase
-from vws import VWS, CloudRecoService
 from vws.exceptions.vws_exceptions import UnknownTarget
 from vws.reports import TargetStatuses
 
+if TYPE_CHECKING:
+    import io
+
+    from _pytest.fixtures import SubRequest
+    from mock_vws.database import VuforiaDatabase
+    from vws import VWS, CloudRecoService
+
 
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestTargetSummary:
     """
     Tests for the target summary endpoint.
     """
 
@@ -52,29 +58,29 @@
         assert report.database_name == vuforia_database.database_name
         assert report.target_name == name
         assert report.active_flag == active_flag
 
         # In case the date changes while adding a target
         # we allow the date before and after adding the target.
 
-        assert report.upload_date in (
+        assert report.upload_date in {
             date_before_add_target,
             date_after_add_target,
-        )
+        }
 
         # While processing the tracking rating is -1.
         assert report.tracking_rating == -1
         assert report.total_recos == 0
         assert report.current_month_recos == 0
         assert report.previous_month_recos == 0
 
     @staticmethod
     @pytest.mark.parametrize(
-        ("image_fixture_name", "expected_status"),
-        [
+        argnames=("image_fixture_name", "expected_status"),
+        argvalues=[
             ("high_quality_image", TargetStatuses.SUCCESS),
             ("image_file_failed_state", TargetStatuses.FAILED),
         ],
     )
     def test_after_processing(
         vws_client: VWS,
         request: SubRequest,
@@ -143,15 +149,15 @@
             active_flag=True,
             application_metadata=None,
         )
 
         vws_client.wait_for_target_processed(target_id=target_id)
 
         results = cloud_reco_client.query(image=high_quality_image)
-        [result] = results
+        (result,) = results
         assert result.target_id == target_id
 
         report = vws_client.get_target_summary_report(target_id=target_id)
         assert report.status == TargetStatuses.SUCCESS
         assert report.total_recos == 0
         assert report.current_month_recos == 0
         assert report.previous_month_recos == 0
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_unexpected_json.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_unexpected_json.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 """
 Tests for giving JSON data to endpoints which do not expect it.
 """
 
+from __future__ import annotations
+
 import json
 from http import HTTPStatus
+from typing import TYPE_CHECKING
 from urllib.parse import urlparse
 
 import pytest
 import requests
 from requests.structures import CaseInsensitiveDict
 from vws_auth_tools import authorization_header, rfc_1123_date
 
-from tests.mock_vws.utils import Endpoint
 from tests.mock_vws.utils.assertions import assert_vwq_failure
 
+if TYPE_CHECKING:
+    from tests.mock_vws.utils import Endpoint
+
 
 @pytest.mark.usefixtures("verify_mock_vuforia")
 class TestUnexpectedJSON:
     """
     Tests for giving JSON to endpoints which do not expect it.
     """
 
@@ -64,21 +69,21 @@
         response = session.send(request=endpoint.prepared_request)
 
         url = str(endpoint.prepared_request.url)
         netloc = urlparse(url).netloc
         if netloc == "cloudreco.vuforia.com":
             # The multipart/formdata boundary is no longer in the given
             # content.
-            assert response.text == ""
+            assert not response.text
             assert_vwq_failure(
                 response=response,
                 status_code=HTTPStatus.UNSUPPORTED_MEDIA_TYPE,
                 content_type=None,
                 cache_control=None,
                 www_authenticate=None,
                 connection="keep-alive",
             )
             return
 
         assert response.status_code == HTTPStatus.BAD_REQUEST
-        assert response.text == ""
+        assert not response.text
         assert "Content-Type" not in response.headers
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/test_update_target.py` & `vws-python-mock-2023.4.8/tests/mock_vws/test_update_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 """
 Tests for the mock of the update target endpoint.
 """
 
 from __future__ import annotations
 
 import base64
-import io
 import json
 import uuid
 from http import HTTPStatus
-from typing import Any, Final
+from typing import TYPE_CHECKING, Any, Final
 from urllib.parse import urljoin
 
 import pytest
 import requests
 from mock_vws._constants import ResultCodes
-from mock_vws.database import VuforiaDatabase
-from requests import Response
 from requests_mock import PUT
-from vws import VWS
 from vws.exceptions.vws_exceptions import BadImage, ProjectInactive
 from vws.reports import TargetStatuses
 from vws_auth_tools import authorization_header, rfc_1123_date
 
 from tests.mock_vws.utils import make_image_file
 from tests.mock_vws.utils.assertions import (
     assert_vws_failure,
     assert_vws_response,
 )
 
 _MAX_METADATA_BYTES: Final[int] = 1024 * 1024 - 1
 
+if TYPE_CHECKING:
+    import io
+
+    from mock_vws.database import VuforiaDatabase
+    from vws import VWS
+
 
 def update_target(
     vuforia_database: VuforiaDatabase,
     data: dict[str, Any],
     target_id: str,
     content_type: str = "application/json",
-) -> Response:
+) -> requests.Response:
     """
     Make a request to the endpoint to update a target.
 
     Args:
         vuforia_database: The credentials to use to connect to
             Vuforia.
         data: The data to send, in JSON format, to the endpoint.
@@ -237,15 +239,15 @@
         "width",
         [-1, "10", None, 0],
         ids=["Negative", "Wrong Type", "None", "Zero"],
     )
     def test_width_invalid(
         vuforia_database: VuforiaDatabase,
         vws_client: VWS,
-        width: Any,
+        width: int | str | None,
         target_id: str,
     ) -> None:
         """
         The width must be a number greater than zero.
         """
         vws_client.wait_for_target_processed(target_id=target_id)
 
@@ -510,16 +512,16 @@
         vws_client.wait_for_target_processed(target_id=target_id)
         vws_client.update_target(target_id=target_id, name=name)
         target_details = vws_client.get_target_record(target_id=target_id)
         assert target_details.target_record.name == name
 
     @staticmethod
     @pytest.mark.parametrize(
-        ("name", "status_code", "result_code"),
-        [
+        argnames=("name", "status_code", "result_code"),
+        argvalues=[
             (1, HTTPStatus.BAD_REQUEST, ResultCodes.FAIL),
             ("", HTTPStatus.BAD_REQUEST, ResultCodes.FAIL),
             (
                 "a" * (_MAX_NAME_LENGTH + 1),
                 HTTPStatus.BAD_REQUEST,
                 ResultCodes.FAIL,
             ),
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/utils/__init__.py` & `vws-python-mock-2023.4.8/tests/mock_vws/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     image = Image.new(color_space, (width, height))
     for row_index in range(height):
         for column_index in range(width):
             if color_space == "L":
                 grey = random.choice(seq=range(0, 255))
                 image.putpixel(xy=(column_index, row_index), value=grey)
             else:
-                assert color_space in ("CMYK", "RGB")
+                assert color_space in {"CMYK", "RGB"}
                 red = random.choice(seq=range(0, 255))
                 green = random.choice(seq=range(0, 255))
                 blue = random.choice(seq=range(0, 255))
                 image.putpixel(
                     xy=(column_index, row_index),
                     value=(red, green, blue),
                 )
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/utils/assertions.py` & `vws-python-mock-2023.4.8/tests/mock_vws/utils/assertions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 
 import copy
 import datetime
 import email.utils
 import json
 from http import HTTPStatus
 from string import hexdigits
+from typing import TYPE_CHECKING
 from zoneinfo import ZoneInfo
 
-from mock_vws._constants import ResultCodes
-from requests import Response
+if TYPE_CHECKING:
+    from mock_vws._constants import ResultCodes
+    from requests import Response
 
 
 def assert_vws_failure(
     response: Response,
     status_code: int,
     result_code: ResultCodes,
 ) -> None:
@@ -108,15 +110,15 @@
     response: Response,
     status_code: int,
     result_code: ResultCodes,
 ) -> None:
     """
     Assert that a VWS response is as expected, at least in part.
 
-    https://library.vuforia.com/articles/Solution/How-To-Use-the-Vuforia-Web-Services-API.html#How-To-Interperete-VWS-API-Result-Codes
+    https://library.vuforia.com/web-api/cloud-targets-web-services-api#result-codes
     implies that the expected status code can be worked out from the result
     code. However, this is not the case as the real results differ from the
     documentation.
 
     For example, it is possible to get a "Fail" result code and a 400 error.
 
     Args:
@@ -132,23 +134,26 @@
     response_result_code = response.json()["result_code"]
     assert response_result_code == result_code.value
     response_header_keys = {
         "content-length",
         "content-type",
         "date",
         "server",
+        "strict-transport-security",
         "x-aws-region",
+        "x-content-type-options",
         "x-envoy-upstream-service-time",
     }
     assert set(map(str.lower, response.headers.keys())) == response_header_keys
     assert response.headers["Content-Length"] == str(len(response.text))
     assert response.headers["Content-Type"] == "application/json"
     assert response.headers["Server"] == "envoy"
-    # The AWS region is not static so we just check that one exists.
-    assert response.headers["x-aws-region"]
+    assert response.headers["x-content-type-options"] == "nosniff"
+    assert "-" in response.headers["x-aws-region"]
+    assert response.headers["strict-transport-security"] == "max-age=31536000"
     assert int(response.headers["x-envoy-upstream-service-time"]) > 1
     assert_json_separators(response=response)
     assert_valid_transaction_id(response=response)
     assert_valid_date_header(response=response)
 
 
 def assert_query_success(response: Response) -> None:
@@ -173,15 +178,15 @@
     copied_response_headers = dict(copy.deepcopy(response.headers))
     copied_response_headers.pop("Date")
 
     # In the mock, all responses have the ``Content-Encoding`` ``gzip``.
     # In the real Vuforia, some do and some do not.
     # We are not sure why.
     content_encoding = copied_response_headers.pop("Content-Encoding", None)
-    assert content_encoding in (None, "gzip")
+    assert content_encoding in {None, "gzip"}
 
     expected_response_header_not_chunked = {
         "Connection": "keep-alive",
         "Content-Length": str(response.raw.tell()),
         "Content-Type": "application/json",
         "Server": "nginx",
     }
```

### Comparing `vws-python-mock-2023.3.5/tests/mock_vws/utils/usage_test_helpers.py` & `vws-python-mock-2023.4.8/tests/mock_vws/utils/usage_test_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """
 Helpers for testing the usage of the mocks.
 """
+from __future__ import annotations
+
 import datetime
-import io
+from typing import TYPE_CHECKING
 
-from mock_vws.database import VuforiaDatabase
 from vws import VWS, CloudRecoService
 from vws.exceptions.custom_exceptions import (
     ActiveMatchingTargetsDeleteProcessing,
 )
 from vws.reports import TargetStatuses
 
+if TYPE_CHECKING:
+    import io
+
+    from mock_vws.database import VuforiaDatabase
+
 
 def _add_and_delete_target(
     image: io.BytesIO,
     vuforia_database: VuforiaDatabase,
 ) -> None:
     """
     Add and delete a target with the given image.
```

### Comparing `vws-python-mock-2023.3.5/vuforia_secrets.env.example` & `vws-python-mock-2023.4.8/vuforia_secrets.env.example`

 * *Files identical despite different names*

