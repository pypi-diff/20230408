# Comparing `tmp/ytmusicapi-0.9.2.tar.gz` & `tmp/ytmusicapi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ytmusicapi-0.9.2.tar", last modified: Thu Aug 27 11:24:54 2020, max compression
+gzip compressed data, was "ytmusicapi-1.0.0.tar", last modified: Sat Apr  8 18:29:21 2023, max compression
```

## Comparing `ytmusicapi-0.9.2.tar` & `ytmusicapi-1.0.0.tar`

### file list

```diff
@@ -1,54 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.754874 ytmusicapi-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (116)      119 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3573 2020-08-27 11:24:54.754874 ytmusicapi-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2645 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-08-27 11:24:54.754874 ytmusicapi-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      913 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.746874 ytmusicapi-0.9.2/ytmusicapi/
--rw-r--r--   0 runner    (1001) docker     (116)      170 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       22 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/_version.py
--rw-r--r--   0 runner    (1001) docker     (116)     1155 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/context.json
--rw-r--r--   0 runner    (1001) docker     (116)      338 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/headers.json
--rw-r--r--   0 runner    (1001) docker     (116)     1558 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.742874 ytmusicapi-0.9.2/ytmusicapi/locales/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.742874 ytmusicapi-0.9.2/ytmusicapi/locales/de/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.750874 ytmusicapi-0.9.2/ytmusicapi/locales/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)      667 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/locales/de/LC_MESSAGES/base.mo
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.742874 ytmusicapi-0.9.2/ytmusicapi/locales/en/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.750874 ytmusicapi-0.9.2/ytmusicapi/locales/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)      378 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/locales/en/LC_MESSAGES/base.mo
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.742874 ytmusicapi-0.9.2/ytmusicapi/locales/es/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.750874 ytmusicapi-0.9.2/ytmusicapi/locales/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)      703 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/locales/es/LC_MESSAGES/base.mo
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.742874 ytmusicapi-0.9.2/ytmusicapi/locales/fr/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.750874 ytmusicapi-0.9.2/ytmusicapi/locales/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)      668 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.742874 ytmusicapi-0.9.2/ytmusicapi/locales/it/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.750874 ytmusicapi-0.9.2/ytmusicapi/locales/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)      663 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/locales/it/LC_MESSAGES/base.mo
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.746874 ytmusicapi-0.9.2/ytmusicapi/locales/ja/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.750874 ytmusicapi-0.9.2/ytmusicapi/locales/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (116)      706 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.754874 ytmusicapi-0.9.2/ytmusicapi/mixins/
--rw-r--r--   0 runner    (1001) docker     (116)    21278 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/mixins/browsing.py
--rw-r--r--   0 runner    (1001) docker     (116)     9547 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/mixins/library.py
--rw-r--r--   0 runner    (1001) docker     (116)    11023 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/mixins/playlists.py
--rw-r--r--   0 runner    (1001) docker     (116)    10156 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/mixins/uploads.py
--rw-r--r--   0 runner    (1001) docker     (116)     3151 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/mixins/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.754874 ytmusicapi-0.9.2/ytmusicapi/parsers/
--rw-r--r--   0 runner    (1001) docker     (116)     1469 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5443 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/parsers/browsing.py
--rw-r--r--   0 runner    (1001) docker     (116)     2624 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/parsers/library.py
--rw-r--r--   0 runner    (1001) docker     (116)     2753 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/parsers/playlists.py
--rw-r--r--   0 runner    (1001) docker     (116)     1248 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/parsers/uploads.py
--rw-r--r--   0 runner    (1001) docker     (116)     2901 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/parsers/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      700 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/parsers/watch.py
--rw-r--r--   0 runner    (1001) docker     (116)     1790 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)     5914 2020-08-27 11:24:46.000000 ytmusicapi-0.9.2/ytmusicapi/ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-08-27 11:24:54.750874 ytmusicapi-0.9.2/ytmusicapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3573 2020-08-27 11:24:54.000000 ytmusicapi-0.9.2/ytmusicapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      999 2020-08-27 11:24:54.000000 ytmusicapi-0.9.2/ytmusicapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-27 11:24:54.000000 ytmusicapi-0.9.2/ytmusicapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-08-27 11:24:54.000000 ytmusicapi-0.9.2/ytmusicapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       78 2020-08-27 11:24:54.000000 ytmusicapi-0.9.2/ytmusicapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       11 2020-08-27 11:24:54.000000 ytmusicapi-0.9.2/ytmusicapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.367682 ytmusicapi-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.github/workflows/docsbuild.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-08 18:29:21.367682 ytmusicapi-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/docs/source/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/setup/browser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/setup/headers_auth.json.example
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/setup/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/setup/oauth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 18:29:21.367682 ytmusicapi-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/tests/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/tests/test.cfg.example
+-rw-r--r--   0 runner    (1001) docker     (123)    22657 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/ytmusicapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/ytmusicapi/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/auth/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/auth/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/auth/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/continuations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ar/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ar/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/base.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/de/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/de/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/en/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/en/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/es/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/es/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/fr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/fr/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/hi/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/hi/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/hi/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/it/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/it/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/ja/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ja/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ja/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/ko/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ko/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ko/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/pt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/pt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/pt/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/pt/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ru/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ru/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/tr/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/tr/LC_MESSAGES/base.po
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/update_mo.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/update_po.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/ur/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/ur/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ur/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/ur/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/zh_CN/LC_MESSAGES/base.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.355682 ytmusicapi-1.0.0/ytmusicapi/locales/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.363682 ytmusicapi-1.0.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.367682 ytmusicapi-1.0.0/ytmusicapi/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35118 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10479 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/mixins/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.367682 ytmusicapi-1.0.0/ytmusicapi/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/albums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/browsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/playlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/songs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/uploads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/parsers/watch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6782 2023-04-08 18:29:08.000000 ytmusicapi-1.0.0/ytmusicapi/ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 18:29:21.359682 ytmusicapi-1.0.0/ytmusicapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-04-08 18:29:21.000000 ytmusicapi-1.0.0/ytmusicapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-04-08 18:29:21.000000 ytmusicapi-1.0.0/ytmusicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 18:29:21.000000 ytmusicapi-1.0.0/ytmusicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-08 18:29:21.000000 ytmusicapi-1.0.0/ytmusicapi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-08 18:29:21.000000 ytmusicapi-1.0.0/ytmusicapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-08 18:29:21.000000 ytmusicapi-1.0.0/ytmusicapi.egg-info/top_level.txt
```

### Comparing `ytmusicapi-0.9.2/PKG-INFO` & `ytmusicapi-1.0.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,98 @@
-Metadata-Version: 2.1
-Name: ytmusicapi
-Version: 0.9.2
-Summary: Unofficial API for YouTube Music
-Home-page: https://github.com/sigma67/ytmusicapi
-Author: sigma67
-Author-email: 
-License: MIT
-Description: ytmusicapi: Unofficial API for YouTube Music
-        ############################################
-        
-        .. image:: https://img.shields.io/pypi/dm/ytmusicapi?style=flat-square
-            :alt: PyPI Downloads
-            :target: https://pypi.org/project/ytmusicapi/
-        
-        .. image:: https://img.shields.io/codecov/c/github/sigma67/ytmusicapi?style=flat-square
-            :alt: Code coverage
-            :target: https://codecov.io/gh/sigma67/ytmusicapi
-        
-        .. image:: https://img.shields.io/github/v/release/sigma67/ytmusicapi?style=flat-square
-            :alt: Latest release
-            :target: https://github.com/sigma67/ytmusicapi/releases/latest
-        
-        .. image:: https://img.shields.io/github/commits-since/sigma67/ytmusicapi/latest?style=flat-square
-            :alt: Commits since latest release
-            :target: https://github.com/sigma67/ytmusicapi/commits
-        
-        
-        A work-in-progress API that emulates web requests from the YouTube Music web client.
-        
-        Currently you need to extract your authentication data from your web browser and provide it through a file for it to work.
-        
-        .. features
-        
-        Features
-        --------
-        | **Browsing**:
-        
-        * search (including all filters)
-        * get artist information and releases (songs, videos, albums, singles)
-        * get user information (videos, playlists)
-        * get albums
-        * get song metadata
-        * get watch playlists (playlist that appears when you press play in YouTube Music)
-        
-        | **Library management**:
-        
-        * get library contents: playlists, songs, artists, albums and subscriptions
-        * add/remove library content: rate songs, albums and playlists, subscribe/unsubscribe artists
-        
-        | **Playlists**:
-        
-        * create and delete playlists
-        * modify playlists: edit metadata, add/move/remove tracks
-        * get playlist contents
-        
-        | **Uploads**:
-        
-        * Upload songs and remove them again
-        * List uploaded songs, artists and albums
-        
-        
-        Usage
-        ------
-        .. code-block:: python
-        
-            from ytmusicapi import YTMusic
-        
-            ytmusic = YTMusic('headers_auth.json')
-            playlistId = ytmusic.create_playlist("test", "test description")
-            search_results = ytmusic.search("Oasis Wonderwall")
-            ytmusic.add_playlist_items(playlistId, [search_results[0]['videoId']])
-        
-        The `tests <https://github.com/sigma67/ytmusicapi/blob/master/tests/test.py>`_ are also a great source of usage examples.
-        
-        .. end-features
-        
-        Requirements
-        ==============
-        
-        - Python 3.5 or higher - https://www.python.org
-        
-        Setup and Usage
-        ===============
-        
-        See the `Documentation <https://ytmusicapi.readthedocs.io/en/latest/usage.html>`_ for detailed instructions
-        
-        Contributing
-        ==============
-        
-        Pull requests are welcome. There are still some features that are not yet implemented.
-        Please, refer to `CONTRIBUTING.rst <https://github.com/sigma67/ytmusicapi/blob/master/CONTRIBUTING.rst>`_ for guidance.
-Platform: UNKNOWN
-Requires-Python: >=3.5
-Provides-Extra: dev
+ytmusicapi: Unofficial API for YouTube Music
+############################################
+
+.. image:: https://img.shields.io/pypi/dm/ytmusicapi?style=flat-square
+    :alt: PyPI Downloads
+    :target: https://pypi.org/project/ytmusicapi/
+
+.. image:: https://badges.gitter.im/sigma67/ytmusicapi.svg
+   :alt: Ask questions at https://gitter.im/sigma67/ytmusicapi
+   :target: https://gitter.im/sigma67/ytmusicapi
+
+.. image:: https://img.shields.io/codecov/c/github/sigma67/ytmusicapi?style=flat-square
+    :alt: Code coverage
+    :target: https://codecov.io/gh/sigma67/ytmusicapi
+
+.. image:: https://img.shields.io/github/v/release/sigma67/ytmusicapi?style=flat-square
+    :alt: Latest release
+    :target: https://github.com/sigma67/ytmusicapi/releases/latest
+
+.. image:: https://img.shields.io/github/commits-since/sigma67/ytmusicapi/latest?style=flat-square
+    :alt: Commits since latest release
+    :target: https://github.com/sigma67/ytmusicapi/commits
+
+
+ytmusicapi is a Python 3 library to send requests to the YouTube Music API.
+It emulates YouTube Music web client requests using the user's cookie data for authentication.
+
+.. features
+
+Features
+--------
+At this point ytmusicapi supports nearly all content interactions in the YouTube Music web app.
+If you find something missing or broken, feel free to create an `issue <https://github.com/sigma67/ytmusicapi/issues/new>`_
+
+| **Browsing**:
+
+* search (including all filters) and suggestions
+* get artist information and releases (songs, videos, albums, singles, related artists)
+* get user information (videos, playlists)
+* get albums
+* get song metadata
+* get watch playlists (next songs when you press play/radio/shuffle in YouTube Music)
+* get song lyrics
+
+| **Exploring music**:
+
+* get moods and genres playlists
+* get latest charts (globally and per country)
+
+| **Library management**:
+
+* get library contents: playlists, songs, artists, albums and subscriptions
+* add/remove library content: rate songs, albums and playlists, subscribe/unsubscribe artists
+* get and modify play history
+
+| **Playlists**:
+
+* create and delete playlists
+* modify playlists: edit metadata, add/move/remove tracks
+* get playlist contents
+* get playlist suggestions
+
+| **Uploads**:
+
+* upload songs and remove them again
+* list uploaded songs, artists and albums
+
+
+Usage
+------
+.. code-block:: python
+
+    from ytmusicapi import YTMusic
+
+    yt = YTMusic('oauth.json')
+    playlistId = yt.create_playlist('test', 'test description')
+    search_results = yt.search('Oasis Wonderwall')
+    yt.add_playlist_items(playlistId, [search_results[0]['videoId']])
+
+The `tests <https://github.com/sigma67/ytmusicapi/blob/master/tests/test.py>`_ are also a great source of usage examples.
+
+.. end-features
+
+Requirements
+==============
+
+- Python 3.8 or higher - https://www.python.org
+
+Setup and Usage
+===============
+
+See the `Documentation <https://ytmusicapi.readthedocs.io/en/latest/usage.html>`_ for detailed instructions
+
+Contributing
+==============
+
+Pull requests are welcome. There are still some features that are not yet implemented.
+Please, refer to `CONTRIBUTING.rst <https://github.com/sigma67/ytmusicapi/blob/master/CONTRIBUTING.rst>`_ for guidance.
```

### Comparing `ytmusicapi-0.9.2/ytmusicapi/locales/de/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.0/ytmusicapi/locales/fr/LC_MESSAGES/base.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,36 +1,32 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-07-21 09:15+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-msgid "albums"
-msgstr "alben"
-
 msgid "artist"
-msgstr "künstler"
+msgstr "artiste"
 
 msgid "playlist"
 msgstr "playlist"
 
-msgid "playlists"
-msgstr "playlists"
-
-msgid "singles"
-msgstr "singles"
+msgid "related"
+msgstr "vous aimerez peut-être aussi"
 
 msgid "song"
-msgstr "titel"
+msgstr "titre"
+
+msgid "station"
+msgstr "radio"
 
 msgid "video"
-msgstr "video"
+msgstr "vidéo"
 
 msgid "videos"
-msgstr "videos"
+msgstr "vidéos"
```

### Comparing `ytmusicapi-0.9.2/ytmusicapi/locales/es/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.0/ytmusicapi/locales/es/LC_MESSAGES/base.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,11 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-07-21 09:15+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -19,18 +18,24 @@
 
 msgid "playlist"
 msgstr "lista de reproducción"
 
 msgid "playlists"
 msgstr "listas de reproducción"
 
+msgid "related"
+msgstr "puede que también te guste"
+
 msgid "singles"
 msgstr "sencillos"
 
 msgid "song"
 msgstr "canción"
 
+msgid "station"
+msgstr "emisora"
+
 msgid "video"
 msgstr "vídeo"
 
 msgid "videos"
 msgstr "vídeos"
```

### Comparing `ytmusicapi-0.9.2/ytmusicapi/locales/fr/LC_MESSAGES/base.mo` & `ytmusicapi-1.0.0/ytmusicapi/locales/zh_TW/LC_MESSAGES/base.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,36 +1,41 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2020-07-21 09:15+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 msgid "albums"
-msgstr "albums"
+msgstr "專輯"
 
 msgid "artist"
-msgstr "artiste"
+msgstr "藝人"
 
 msgid "playlist"
-msgstr "playlist"
+msgstr "播放清單"
 
 msgid "playlists"
-msgstr "playlists"
+msgstr "精選收錄"
+
+msgid "related"
+msgstr "粉絲可能也會喜歡"
 
 msgid "singles"
-msgstr "singles"
+msgstr "單曲"
 
 msgid "song"
-msgstr "titre"
+msgstr "歌曲"
+
+msgid "station"
+msgstr "電台"
 
 msgid "video"
-msgstr "vidéo"
+msgstr "影片"
 
 msgid "videos"
-msgstr "vidéos"
+msgstr "影片"
```

### Comparing `ytmusicapi-0.9.2/ytmusicapi/mixins/library.py` & `ytmusicapi-1.0.0/ytmusicapi/mixins/library.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-from ytmusicapi.helpers import *
+from random import randint
+from ytmusicapi.continuations import *
+from ._utils import *
 from ytmusicapi.parsers.browsing import *
 from ytmusicapi.parsers.library import *
-from ytmusicapi.parsers.playlists import *
+from typing import List, Dict
 
 
 class LibraryMixin:
+
     def get_library_playlists(self, limit: int = 25) -> List[Dict]:
         """
         Retrieves the playlists in the user's library.
 
-        :param limit: Number of playlists to retrieve
+        :param limit: Number of playlists to retrieve. `None` retrieves them all.
         :return: List of owned playlists.
 
         Each item is in the following format::
 
             {
                 'playlistId': 'PLQwVIlKxHM6rz0fDJVv_0UlXGEWf-bFys',
                 'title': 'Playlist title',
@@ -22,122 +25,163 @@
             }
         """
         self._check_auth()
         body = {'browseId': 'FEmusic_liked_playlists'}
         endpoint = 'browse'
         response = self._send_request(endpoint, body)
 
-        results = find_object_by_key(nav(response, SINGLE_COLUMN_TAB + SECTION_LIST),
-                                     'itemSectionRenderer')
-        results = nav(results, ITEM_SECTION)['gridRenderer']
+        results = get_library_contents(response, GRID)
         playlists = parse_content_list(results['items'][1:], parse_playlist)
 
         if 'continuations' in results:
             request_func = lambda additionalParams: self._send_request(
                 endpoint, body, additionalParams)
             parse_func = lambda contents: parse_content_list(contents, parse_playlist)
+            remaining_limit = None if limit is None else (limit - len(playlists))
             playlists.extend(
-                get_continuations(results, 'gridContinuation', limit - len(playlists),
-                                  request_func, parse_func))
+                get_continuations(results, 'gridContinuation', remaining_limit, request_func,
+                                  parse_func))
 
         return playlists
 
-    def get_library_songs(self, limit: int = 25) -> List[Dict]:
+    def get_library_songs(self,
+                          limit: int = 25,
+                          validate_responses: bool = False,
+                          order: str = None) -> List[Dict]:
         """
         Gets the songs in the user's library (liked videos are not included).
         To get liked songs and videos, use :py:func:`get_liked_songs`
 
         :param limit: Number of songs to retrieve
+        :param validate_responses: Flag indicating if responses from YTM should be validated and retried in case
+            when some songs are missing. Default: False
+        :param order: Order of songs to return. Allowed values: 'a_to_z', 'z_to_a', 'recently_added'. Default: Default order.
         :return: List of songs. Same format as :py:func:`get_playlist`
         """
         self._check_auth()
         body = {'browseId': 'FEmusic_liked_videos'}
+        validate_order_parameter(order)
+        if order is not None:
+            body["params"] = prepare_order_params(order)
         endpoint = 'browse'
-        response = self._send_request(endpoint, body)
-        results = find_object_by_key(nav(response, SINGLE_COLUMN_TAB + SECTION_LIST),
-                                     'itemSectionRenderer')
-        results = nav(results, ITEM_SECTION)
-        if 'musicShelfRenderer' not in results:
+        per_page = 25
+
+        request_func = lambda additionalParams: self._send_request(endpoint, body)
+        parse_func = lambda raw_response: parse_library_songs(raw_response)
+
+        if validate_responses and limit is None:
+            raise Exception("Validation is not supported without a limit parameter.")
+
+        if validate_responses:
+            validate_func = lambda parsed: validate_response(parsed, per_page, limit, 0)
+            response = resend_request_until_parsed_response_is_valid(request_func, None,
+                                                                     parse_func, validate_func, 3)
+        else:
+            response = parse_func(request_func(None))
+
+        results = response['results']
+        songs = response['parsed']
+        if songs is None:
             return []
-        results = results['musicShelfRenderer']
-        songs = parse_playlist_items(results['contents'][1:])
 
         if 'continuations' in results:
-            request_func = lambda additionalParams: self._send_request(
+            request_continuations_func = lambda additionalParams: self._send_request(
                 endpoint, body, additionalParams)
-            parse_func = lambda contents: parse_playlist_items(contents)
-            songs.extend(
-                get_continuations(results, 'musicShelfContinuation', limit - len(songs),
-                                  request_func, parse_func))
+            parse_continuations_func = lambda contents: parse_playlist_items(contents)
+
+            if validate_responses:
+                songs.extend(
+                    get_validated_continuations(results, 'musicShelfContinuation',
+                                                limit - len(songs), per_page,
+                                                request_continuations_func,
+                                                parse_continuations_func))
+            else:
+                remaining_limit = None if limit is None else (limit - len(songs))
+                songs.extend(
+                    get_continuations(results, 'musicShelfContinuation', remaining_limit,
+                                      request_continuations_func, parse_continuations_func))
 
         return songs
 
-    def get_library_albums(self, limit: int = 25) -> List[Dict]:
+    def get_library_albums(self, limit: int = 25, order: str = None) -> List[Dict]:
         """
         Gets the albums in the user's library.
 
         :param limit: Number of albums to return
-        :return: List of albums
+        :param order: Order of albums to return. Allowed values: 'a_to_z', 'z_to_a', 'recently_added'. Default: Default order.
+        :return: List of albums.
+
+        Each item is in the following format::
+
+            {
+              "browseId": "MPREb_G8AiyN7RvFg",
+              "playlistId": "OLAK5uy_lKgoGvlrWhX0EIPavQUXxyPed8Cj38AWc",
+              "title": "Beautiful",
+              "type": "Album",
+              "thumbnails": [...],
+              "artists": [{
+                "name": "Project 46",
+                "id": "UCXFv36m62USAN5rnVct9B4g"
+              }],
+              "year": "2015"
+            }
         """
         self._check_auth()
         body = {'browseId': 'FEmusic_liked_albums'}
+        validate_order_parameter(order)
+        if order is not None:
+            body["params"] = prepare_order_params(order)
 
         endpoint = 'browse'
         response = self._send_request(endpoint, body)
-        results = find_object_by_key(nav(response, SINGLE_COLUMN_TAB + SECTION_LIST),
-                                     'itemSectionRenderer')
-        results = nav(results, ITEM_SECTION)
-        if 'gridRenderer' not in results:
-            return []
-        results = results['gridRenderer']
-        albums = parse_albums(results['items'], False)
-
-        if 'continuations' in results:
-            request_func = lambda additionalParams: self._send_request(
-                endpoint, body, additionalParams)
-            parse_func = lambda contents: parse_albums(contents, False)
-            albums.extend(
-                get_continuations(results, 'gridContinuation', limit - len(albums), request_func,
-                                  parse_func))
-
-        return albums
+        return parse_library_albums(
+            response,
+            lambda additionalParams: self._send_request(endpoint, body, additionalParams), limit)
 
-    def get_library_artists(self, limit: int = 25) -> List[Dict]:
+    def get_library_artists(self, limit: int = 25, order: str = None) -> List[Dict]:
         """
         Gets the artists of the songs in the user's library.
 
         :param limit: Number of artists to return
+        :param order: Order of artists to return. Allowed values: 'a_to_z', 'z_to_a', 'recently_added'. Default: Default order.
         :return: List of artists.
 
         Each item is in the following format::
 
             {
               "browseId": "UCxEqaQWosMHaTih-tgzDqug",
               "artist": "WildVibes",
               "subscribers": "2.91K",
               "thumbnails": [...]
             }
         """
         self._check_auth()
         body = {'browseId': 'FEmusic_library_corpus_track_artists'}
+        validate_order_parameter(order)
+        if order is not None:
+            body["params"] = prepare_order_params(order)
         endpoint = 'browse'
         response = self._send_request(endpoint, body)
         return parse_library_artists(
             response,
             lambda additionalParams: self._send_request(endpoint, body, additionalParams), limit)
 
-    def get_library_subscriptions(self, limit: int = 25) -> List[Dict]:
+    def get_library_subscriptions(self, limit: int = 25, order: str = None) -> List[Dict]:
         """
         Gets the artists the user has subscribed to.
 
         :param limit: Number of artists to return
+        :param order: Order of artists to return. Allowed values: 'a_to_z', 'z_to_a', 'recently_added'. Default: Default order.
         :return: List of artists. Same format as :py:func:`get_library_artists`
         """
         self._check_auth()
         body = {'browseId': 'FEmusic_library_corpus_artists'}
+        validate_order_parameter(order)
+        if order is not None:
+            body["params"] = prepare_order_params(order)
         endpoint = 'browse'
         response = self._send_request(endpoint, body)
         return parse_library_artists(
             response,
             lambda additionalParams: self._send_request(endpoint, body, additionalParams), limit)
 
     def get_liked_songs(self, limit: int = 100) -> Dict:
@@ -160,23 +204,40 @@
         self._check_auth()
         body = {'browseId': 'FEmusic_history'}
         endpoint = 'browse'
         response = self._send_request(endpoint, body)
         results = nav(response, SINGLE_COLUMN_TAB + SECTION_LIST)
         songs = []
         for content in results:
-            data = content['musicShelfRenderer']['contents']
-            menu_entries = [[-1] + MENU_SERVICE + ['feedbackEndpoint', 'feedbackToken']]
+            data = nav(content, MUSIC_SHELF + ['contents'], True)
+            if not data:
+                error = nav(content, ['musicNotifierShelfRenderer'] + TITLE, True)
+                raise Exception(error)
+            menu_entries = [[-1] + MENU_SERVICE + FEEDBACK_TOKEN]
             songlist = parse_playlist_items(data, menu_entries)
             for song in songlist:
                 song['played'] = nav(content['musicShelfRenderer'], TITLE_TEXT)
             songs.extend(songlist)
 
         return songs
 
+    def add_history_item(self, song):
+        """
+        Add an item to the account's history using the playbackTracking URI
+        obtained from :py:func:`get_song`.
+
+        :param song: Dictionary as returned by :py:func:`get_song`
+        :return: Full response. response.status_code is 204 if successful
+        """
+        url = song["playbackTracking"]["videostatsPlaybackUrl"]["baseUrl"]
+        CPNA = ("abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789-_")
+        cpn = "".join((CPNA[randint(0, 256) & 63] for _ in range(0, 16)))
+        params = {"ver": 2, "c": "WEB_REMIX", "cpn": cpn}
+        return self._send_get_request(url, params)
+
     def remove_history_items(self, feedbackTokens: List[str]) -> Dict:  # pragma: no cover
         """
         Remove an item from the account's history. This method does currently not work with brand accounts
 
         :param feedbackTokens: Token to identify the item to remove, obtained from :py:func:`get_history`
         :return: Full response
         """
@@ -202,14 +263,27 @@
         body = {'target': {'videoId': videoId}}
         endpoint = prepare_like_endpoint(rating)
         if endpoint is None:
             return
 
         return self._send_request(endpoint, body)
 
+    def edit_song_library_status(self, feedbackTokens: List[str] = None) -> Dict:
+        """
+        Adds or removes a song from your library depending on the token provided.
+
+        :param feedbackTokens: List of feedbackTokens obtained from authenticated requests
+            to endpoints that return songs (i.e. :py:func:`get_album`)
+        :return: Full response
+        """
+        self._check_auth()
+        body = {'feedbackTokens': feedbackTokens}
+        endpoint = 'feedback'
+        return endpoint if not endpoint else self._send_request(endpoint, body)
+
     def rate_playlist(self, playlistId: str, rating: str = 'INDIFFERENT') -> Dict:
         """
         Rates a playlist/album ("Add to library"/"Remove from library" interactions on YouTube Music)
         You can also dislike a playlist/album, which has an effect on your recommendations
 
         :param playlistId: Playlist id
         :param rating: One of 'LIKE', 'DISLIKE', 'INDIFFERENT'
```

### Comparing `ytmusicapi-0.9.2/ytmusicapi/mixins/uploads.py` & `ytmusicapi-1.0.0/ytmusicapi/mixins/uploads.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,224 +1,220 @@
 import requests
 import ntpath
 import os
 from typing import List, Dict, Union
+
+from ._utils import validate_order_parameter, prepare_order_params
 from ytmusicapi.helpers import *
-from ytmusicapi.parsers.library import *
-from ytmusicapi.parsers.uploads import *
+from ytmusicapi.navigation import *
+from ytmusicapi.continuations import get_continuations
+from ytmusicapi.parsers.library import parse_library_albums, parse_library_artists, get_library_contents
+from ytmusicapi.parsers.albums import parse_album_header
+from ytmusicapi.parsers.uploads import parse_uploaded_items
 
 
 class UploadsMixin:
-    def get_library_upload_songs(self, limit: int = 25) -> List[Dict]:
+    def get_library_upload_songs(self, limit: int = 25, order: str = None) -> List[Dict]:
         """
         Returns a list of uploaded songs
 
-        :param limit: How many songs to return. Default: 25
+        :param limit: How many songs to return. `None` retrieves them all. Default: 25
+        :param order: Order of songs to return. Allowed values: 'a_to_z', 'z_to_a', 'recently_added'. Default: Default order.
         :return: List of uploaded songs.
 
         Each item is in the following format::
 
             {
               "entityId": "t_po_CICr2crg7OWpchDpjPjrBA",
               "videoId": "Uise6RPKoek",
-              "artist": "Coldplay",
+              "artists": [{
+                'name': 'Coldplay',
+                'id': 'FEmusic_library_privately_owned_artist_detaila_po_CICr2crg7OWpchIIY29sZHBsYXk',
+              }],
               "title": "A Sky Full Of Stars",
               "album": "Ghost Stories",
               "likeStatus": "LIKE",
               "thumbnails": [...]
             }
         """
         self._check_auth()
         endpoint = 'browse'
         body = {"browseId": "FEmusic_library_privately_owned_tracks"}
+        validate_order_parameter(order)
+        if order is not None:
+            body["params"] = prepare_order_params(order)
         response = self._send_request(endpoint, body)
-        results = find_object_by_key(nav(response, SINGLE_COLUMN_TAB + SECTION_LIST),
-                                     'itemSectionRenderer')
-        results = nav(results, ITEM_SECTION)['musicShelfRenderer']
-        songs = []
-
-        songs.extend(parse_uploaded_items(results['contents'][1:]))
+        results = get_library_contents(response, MUSIC_SHELF)
+        if results is None:
+            return []
+        songs = parse_uploaded_items(results['contents'][1:])
 
         if 'continuations' in results:
             request_func = lambda additionalParams: self._send_request(
                 endpoint, body, additionalParams)
+            remaining_limit = None if limit is None else (limit - len(songs))
             songs.extend(
-                get_continuations(results, 'musicShelfContinuation', limit - len(songs),
-                                  request_func, parse_uploaded_items))
+                get_continuations(results, 'musicShelfContinuation', remaining_limit, request_func,
+                                  parse_uploaded_items))
 
         return songs
 
-    def get_library_upload_albums(self, limit: int = 25) -> List[Dict]:
+    def get_library_upload_albums(self, limit: int = 25, order: str = None) -> List[Dict]:
         """
         Gets the albums of uploaded songs in the user's library.
 
-        :param limit: Number of albums to return. Default: 25
+        :param limit: Number of albums to return. `None` retrives them all. Default: 25
+        :param order: Order of albums to return. Allowed values: 'a_to_z', 'z_to_a', 'recently_added'. Default: Default order.
         :return: List of albums as returned by :py:func:`get_library_albums`
         """
         self._check_auth()
         body = {'browseId': 'FEmusic_library_privately_owned_releases'}
+        validate_order_parameter(order)
+        if order is not None:
+            body["params"] = prepare_order_params(order)
         endpoint = 'browse'
         response = self._send_request(endpoint, body)
-        results = find_object_by_key(nav(response, SINGLE_COLUMN_TAB + SECTION_LIST),
-                                     'itemSectionRenderer')
-        results = nav(results, ITEM_SECTION)
-        if 'gridRenderer' not in results:
-            return []
-        else:
-            results = results['gridRenderer']
-        albums = parse_albums(results['items'])
+        return parse_library_albums(
+            response,
+            lambda additionalParams: self._send_request(endpoint, body, additionalParams), limit)
 
-        if 'continuations' in results:
-            request_func = lambda additionalParams: self._send_request(
-                endpoint, body, additionalParams)
-            parse_func = lambda contents: parse_albums(contents)
-            albums.extend(
-                get_continuations(results, 'gridContinuation', limit - len(albums), request_func,
-                                  parse_func))
-
-        return albums
-
-    def get_library_upload_artists(self, limit: int = 25) -> List[Dict]:
+    def get_library_upload_artists(self, limit: int = 25, order: str = None) -> List[Dict]:
         """
         Gets the artists of uploaded songs in the user's library.
 
-        :param limit: Number of artists to return. Default: 25
+        :param limit: Number of artists to return. `None` retrieves them all. Default: 25
+        :param order: Order of artists to return. Allowed values: 'a_to_z', 'z_to_a', 'recently_added'. Default: Default order.
         :return: List of artists as returned by :py:func:`get_library_artists`
         """
         self._check_auth()
         body = {'browseId': 'FEmusic_library_privately_owned_artists'}
+        validate_order_parameter(order)
+        if order is not None:
+            body["params"] = prepare_order_params(order)
         endpoint = 'browse'
         response = self._send_request(endpoint, body)
-        results = find_object_by_key(nav(response, SINGLE_COLUMN_TAB + SECTION_LIST),
-                                     'itemSectionRenderer')
-        results = nav(results, ITEM_SECTION)['musicShelfRenderer']
-        artists = parse_artists(results['contents'], True)
-
-        if 'continuations' in results:
-            request_func = lambda additionalParams: self._send_request(
-                endpoint, body, additionalParams)
-            parse_func = lambda contents: parse_artists(contents, True)
-            artists.extend(
-                get_continuations(results, 'musicShelfContinuation', limit - len(artists),
-                                  request_func, parse_func))
-
-        return artists
+        return parse_library_artists(
+            response,
+            lambda additionalParams: self._send_request(endpoint, body, additionalParams), limit)
 
-    def get_library_upload_artist(self, browseId: str) -> List[Dict]:
+    def get_library_upload_artist(self, browseId: str, limit: int = 25) -> List[Dict]:
         """
         Returns a list of uploaded tracks for the artist.
 
         :param browseId: Browse id of the upload artist, i.e. from :py:func:`get_library_upload_songs`
+        :param limit: Number of songs to return (increments of 25).
         :return: List of uploaded songs.
 
         Example List::
 
             [
               {
                 "entityId": "t_po_CICr2crg7OWpchDKwoakAQ",
                 "videoId": "Dtffhy8WJgw",
                 "title": "Hold Me (Original Mix)",
-                "artist": [
+                "artists": [
                   {
                     "name": "Jakko",
                     "id": "FEmusic_library_privately_owned_artist_detaila_po_CICr2crg7OWpchIFamFra28"
                   }
                 ],
                 "album": null,
                 "likeStatus": "LIKE",
                 "thumbnails": [...]
               }
             ]
         """
         self._check_auth()
-        body = prepare_browse_endpoint("ARTIST", browseId)
+        body = {'browseId': browseId}
         endpoint = 'browse'
         response = self._send_request(endpoint, body)
-        results = nav(response, SINGLE_COLUMN_TAB + SECTION_LIST + MUSIC_SHELF)
+        results = nav(response, SINGLE_COLUMN_TAB + SECTION_LIST_ITEM + MUSIC_SHELF)
         if len(results['contents']) > 1:
             results['contents'].pop(0)
 
-        return parse_uploaded_items(results['contents'])
+        items = parse_uploaded_items(results['contents'])
+
+        if 'continuations' in results:
+            request_func = lambda additionalParams: self._send_request(
+                endpoint, body, additionalParams)
+            parse_func = lambda contents: parse_uploaded_items(contents)
+            remaining_limit = None if limit is None else (limit - len(items))
+            items.extend(
+                get_continuations(results, 'musicShelfContinuation', remaining_limit, request_func,
+                                  parse_func))
+
+        return items
 
     def get_library_upload_album(self, browseId: str) -> Dict:
         """
         Get information and tracks of an album associated with uploaded tracks
 
         :param browseId: Browse id of the upload album, i.e. from i.e. from :py:func:`get_library_upload_songs`
         :return: Dictionary with title, description, artist and tracks.
 
         Example album::
 
             {
-              "title": "Hard To Stop - Single",
-              "thumbnails": [...]
-              "year": "2013",
-              "trackCount": 1,
-              "duration": "4 minutes, 2 seconds",
+              "title": "18 Months",
+              "type": "Album",
+              "thumbnails": [...],
+              "trackCount": 7,
+              "duration": "24 minutes",
+              "audioPlaylistId": "MLPRb_po_55chars",
               "tracks": [
                 {
-                  "entityId": "t_po_CICr2crg7OWpchDN6tnYBw",
-                  "videoId": "VBQVcjJM7ak",
-                  "title": "Hard To Stop (Vicetone x Ne-Yo x Daft Punk)",
-                  "likeStatus": "LIKE"
-                }
-              ]
-            }
+                  "entityId": "t_po_22chars",
+                  "videoId": "FVo-UZoPygI",
+                  "title": "Feel So Close",
+                  "duration": "4:15",
+                  "duration_seconds": 255,
+                  "artists": None,
+                  "album": {
+                    "name": "18 Months",
+                    "id": "FEmusic_library_privately_owned_release_detailb_po_55chars"
+                  },
+                  "likeStatus": "INDIFFERENT",
+                  "thumbnails": None
+                },
         """
         self._check_auth()
-        body = prepare_browse_endpoint("ALBUM", browseId)
+        body = {'browseId': browseId}
         endpoint = 'browse'
         response = self._send_request(endpoint, body)
-        header = response['header']['musicDetailHeaderRenderer']
-        album = {'title': nav(header, TITLE_TEXT)}
-        album['thumbnails'] = nav(header, THUMBNAIL_CROPPED)
-        if "description" in header:
-            album["description"] = header["description"]["runs"][0]["text"]
-        run_count = len(header['subtitle']['runs'])
-        if run_count == 3:
-            album['year'] = nav(header, SUBTITLE2)
-
-        if run_count == 5:
-            album['artist'] = {
-                'name': nav(header, SUBTITLE2),
-                'id': nav(header, ['subtitle', 'runs', 2] + NAVIGATION_BROWSE_ID)
-            }
-            album['year'] = nav(header, SUBTITLE3)
-
-        if len(header['secondSubtitle']['runs']) > 1:
-            album['trackCount'] = to_int(header['secondSubtitle']['runs'][0]['text'])
-            album['duration'] = header['secondSubtitle']['runs'][2]['text']
-        else:
-            album['duration'] = header['secondSubtitle']['runs'][0]['text']
-
-        results = nav(response, SINGLE_COLUMN_TAB + SECTION_LIST + MUSIC_SHELF)
+        album = parse_album_header(response)
+        results = nav(response, SINGLE_COLUMN_TAB + SECTION_LIST_ITEM + MUSIC_SHELF)
         album['tracks'] = parse_uploaded_items(results['contents'])
+        album['duration_seconds'] = sum_total_duration(album)
         return album
 
     def upload_song(self, filepath: str) -> Union[str, requests.Response]:
         """
         Uploads a song to YouTube Music
 
         :param filepath: Path to the music file (mp3, m4a, wma, flac or ogg)
         :return: Status String or full response
         """
         self._check_auth()
+        if not self.is_browser_auth:
+            raise Exception("Please provide authentication before using this function")
         if not os.path.isfile(filepath):
             raise Exception("The provided file does not exist.")
 
         supported_filetypes = ["mp3", "m4a", "wma", "flac", "ogg"]
         if os.path.splitext(filepath)[1][1:] not in supported_filetypes:
             raise Exception(
                 "The provided file type is not supported by YouTube Music. Supported file types are "
                 + ', '.join(supported_filetypes))
 
-        headers = self.headers
-        upload_url = "https://upload.youtube.com/upload/usermusic/http?authuser=0"
+        headers = self.headers.copy()
+        upload_url = "https://upload.youtube.com/upload/usermusic/http?authuser=%s" % headers[
+            'x-goog-authuser']
         filesize = os.path.getsize(filepath)
         body = ("filename=" + ntpath.basename(filepath)).encode('utf-8')
+        headers.pop('content-encoding', None)
         headers['content-type'] = 'application/x-www-form-urlencoded;charset=utf-8'
         headers['X-Goog-Upload-Command'] = 'start'
         headers['X-Goog-Upload-Header-Content-Length'] = str(filesize)
         headers['X-Goog-Upload-Protocol'] = 'resumable'
         response = requests.post(upload_url, data=body, headers=headers, proxies=self.proxies)
         headers['X-Goog-Upload-Command'] = 'upload, finalize'
         headers['X-Goog-Upload-Offset'] = '0'
```

### Comparing `ytmusicapi-0.9.2/ytmusicapi/parsers/playlists.py` & `ytmusicapi-1.0.0/ytmusicapi/parsers/playlists.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,78 +1,101 @@
-from .utils import *
 from typing import List
+from .songs import *
+from ._utils import *
 
 
 def parse_playlist_items(results, menu_entries: List[List] = None):
     songs = []
     count = 1
     for result in results:
         count += 1
-        if 'musicResponsiveListItemRenderer' not in result:
+        if MRLIR not in result:
             continue
-        data = result['musicResponsiveListItemRenderer']
+        data = result[MRLIR]
 
-        try:
-            # if playlist is not owned, the playlist item can't be interacted with
-            videoId = setVideoId = None
-            like = None
+        videoId = setVideoId = None
+        like = None
+        feedback_tokens = None
+
+        # if the item has a menu, find its setVideoId
+        if 'menu' in data:
+            for item in nav(data, MENU_ITEMS):
+                if 'menuServiceItemRenderer' in item:
+                    menu_service = nav(item, MENU_SERVICE)
+                    if 'playlistEditEndpoint' in menu_service:
+                        setVideoId = menu_service['playlistEditEndpoint']['actions'][0][
+                            'setVideoId']
+                        videoId = menu_service['playlistEditEndpoint']['actions'][0][
+                            'removedVideoId']
 
-            # if item is not playable, there is no videoId
+                if TOGGLE_MENU in item:
+                    feedback_tokens = parse_song_menu_tokens(item)
+
+        # if item is not playable, the videoId was retrieved above
+        if nav(data, PLAY_BUTTON, none_if_absent=True) is not None:
             if 'playNavigationEndpoint' in nav(data, PLAY_BUTTON):
                 videoId = nav(data,
                               PLAY_BUTTON)['playNavigationEndpoint']['watchEndpoint']['videoId']
 
-                for item in nav(data, MENU_ITEMS):
-                    if 'menuServiceItemRenderer' in item and 'playlistEditEndpoint' in nav(
-                            item, MENU_SERVICE):
-                        setVideoId = nav(
-                            item, MENU_SERVICE)['playlistEditEndpoint']['actions'][0]['setVideoId']
-                        break
-
                 if 'menu' in data:
                     like = nav(data, MENU_LIKE_STATUS, True)
 
-            title = get_item_text(data, 0)
-            if title == 'Song deleted':
-                continue
-
-            artists = parse_song_artists(data, 1)
-
-            album = parse_song_album(data, 2)
-
-            duration = None
-            if 'fixedColumns' in data:
-                if 'simpleText' in data['fixedColumns'][0][
-                        'musicResponsiveListItemFixedColumnRenderer']['text']:
-                    duration = data['fixedColumns'][0][
-                        'musicResponsiveListItemFixedColumnRenderer']['text']['simpleText']
-                else:
-                    duration = data['fixedColumns'][0][
-                        'musicResponsiveListItemFixedColumnRenderer']['text']['runs'][0]['text']
-
-            thumbnails = None
-            if 'thumbnail' in data:
-                thumbnails = nav(data, THUMBNAILS)
-
-            song = {
-                'videoId': videoId,
-                'title': title,
-                'artists': artists,
-                'album': album,
-                'likeStatus': like,
-                'thumbnails': thumbnails
-            }
-            if duration:
-                song['duration'] = duration
-            if setVideoId:
-                song['setVideoId'] = setVideoId
-
-            if menu_entries:
-                for menu_entry in menu_entries:
-                    song[menu_entry[-1]] = nav(data, MENU_ITEMS + menu_entry)
+        title = get_item_text(data, 0)
+        if title == 'Song deleted':
+            continue
+
+        artists = parse_song_artists(data, 1)
 
-            songs.append(song)
+        album = parse_song_album(data, 2)
 
-        except Exception as e:
-            print("Item " + str(count) + ": " + str(e))
+        duration = None
+        if 'fixedColumns' in data:
+            if 'simpleText' in get_fixed_column_item(data, 0)['text']:
+                duration = get_fixed_column_item(data, 0)['text']['simpleText']
+            else:
+                duration = get_fixed_column_item(data, 0)['text']['runs'][0]['text']
+
+        thumbnails = None
+        if 'thumbnail' in data:
+            thumbnails = nav(data, THUMBNAILS)
+
+        isAvailable = True
+        if 'musicItemRendererDisplayPolicy' in data:
+            isAvailable = data[
+                'musicItemRendererDisplayPolicy'] != 'MUSIC_ITEM_RENDERER_DISPLAY_POLICY_GREY_OUT'
+
+        isExplicit = nav(data, BADGE_LABEL, True) is not None
+
+        videoType = nav(
+            data, MENU_ITEMS + [0, 'menuNavigationItemRenderer', 'navigationEndpoint']
+            + NAVIGATION_VIDEO_TYPE, True)
+
+        song = {
+            'videoId': videoId,
+            'title': title,
+            'artists': artists,
+            'album': album,
+            'likeStatus': like,
+            'thumbnails': thumbnails,
+            'isAvailable': isAvailable,
+            'isExplicit': isExplicit,
+            'videoType': videoType
+        }
+        if duration:
+            song['duration'] = duration
+            song['duration_seconds'] = parse_duration(duration)
+        if setVideoId:
+            song['setVideoId'] = setVideoId
+        if feedback_tokens:
+            song['feedbackTokens'] = feedback_tokens
+
+        if menu_entries:
+            for menu_entry in menu_entries:
+                song[menu_entry[-1]] = nav(data, MENU_ITEMS + menu_entry)
+
+        songs.append(song)
 
     return songs
+
+
+def validate_playlist_id(playlistId):
+    return playlistId if not playlistId.startswith("VL") else playlistId[2:]
```

### Comparing `ytmusicapi-0.9.2/ytmusicapi/parsers/uploads.py` & `ytmusicapi-1.0.0/ytmusicapi/parsers/uploads.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-from ytmusicapi.parsers.utils import *
+from ._utils import *
+from .songs import parse_song_artists, parse_song_album
 
 
 def parse_uploaded_items(results):
     songs = []
     for result in results:
-        data = result['musicResponsiveListItemRenderer']
+        data = result[MRLIR]
         if 'menu' not in data:
             continue
         entityId = nav(data, MENU_ITEMS)[-1]['menuNavigationItemRenderer']['navigationEndpoint'][
             'confirmDialogEndpoint']['content']['confirmDialogRenderer']['confirmButton'][
                 'buttonRenderer']['command']['musicDeletePrivatelyOwnedEntityCommand']['entityId']
 
         videoId = nav(data, MENU_ITEMS + [0]
                       + MENU_SERVICE)['queueAddEndpoint']['queueTarget']['videoId']
 
         title = get_item_text(data, 0)
         like = nav(data, MENU_LIKE_STATUS)
         thumbnails = nav(data, THUMBNAILS) if 'thumbnail' in data else None
+        duration = get_fixed_column_item(data, 0)['text']['runs'][0]['text']
         song = {
             'entityId': entityId,
             'videoId': videoId,
             'title': title,
-            'artist': None,
-            'album': None,
+            'duration': duration,
+            'duration_seconds': parse_duration(duration),
+            'artists': parse_song_artists(data, 1),
+            'album': parse_song_album(data, 2),
             'likeStatus': like,
             'thumbnails': thumbnails
         }
-        if get_flex_column_item(data, 1):
-            song['artist'] = parse_song_artists(data, 1)
-            song['album'] = parse_song_album(data, 2)
 
         songs.append(song)
 
     return songs
```

### Comparing `ytmusicapi-0.9.2/ytmusicapi/setup.py` & `ytmusicapi-1.0.0/ytmusicapi/auth/browser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-import pkg_resources
-import json
 import os
 import platform
+from ytmusicapi.helpers import *
 
 path = os.path.dirname(os.path.realpath(__file__)) + os.sep
 
 
-def setup(filepath=None, headers_raw=None):
+def setup_browser(filepath=None, headers_raw=None):
     contents = []
     if not headers_raw:
         eof = "Ctrl-D" if platform.system() != "Windows" else "'Enter, Ctrl-Z, Enter'"
         print("Please paste the request headers from Firefox and press " + eof + " to continue:")
         while True:
             try:
                 line = input()
             except EOFError:
                 break
             contents.append(line)
     else:
         contents = headers_raw.split('\n')
 
-    required_headers = ["Cookie"]
-    required_headers_lower = {v.lower(): v for v in required_headers }
     try:
-        headers = {}
+        user_headers = {}
         for content in contents:
             header = content.split(': ')
-            key = header[0].lower()
-            if key in required_headers_lower:
-                headers[required_headers_lower[key]] = ': '.join(header[1:])
+            if len(header) == 1 or header[0].startswith(
+                    ":"):  # nothing was split or chromium headers
+                continue
+            user_headers[header[0].lower()] = ': '.join(header[1:])
 
     except Exception as e:
         raise Exception("Error parsing your input, please try again. Full error: " + str(e))
 
-    if len(headers) != len(required_headers):
-        missing = set(required_headers) - set(headers)
+    missing_headers = {"cookie", "x-goog-authuser"} - set(k.lower() for k in user_headers.keys())
+    if missing_headers:
         raise Exception(
-            "The following entries are missing in your headers: " + ", ".join(missing)
+            "The following entries are missing in your headers: " + ", ".join(missing_headers)
             + ". Please try a different request (such as /browse) and make sure you are logged in."
         )
 
-    with open(pkg_resources.resource_filename('ytmusicapi', 'headers.json')) as json_file:
-        default_headers = json.load(json_file)
+    ignore_headers = {"host", "content-length", "accept-encoding"}
+    for key in user_headers.copy().keys():
+        if key.startswith("sec") or key in ignore_headers:
+            user_headers.pop(key, None)
+
+    init_headers = initialize_headers()
+    user_headers.update(init_headers)
+    headers = user_headers
 
-    default_headers.update(headers)
     if filepath is not None:
         with open(filepath, 'w') as file:
-            json.dump(default_headers, file, ensure_ascii=True, indent=4, sort_keys=True)
+            json.dump(headers, file, ensure_ascii=True, indent=4, sort_keys=True)
 
-    return json.dumps(default_headers)
+    return json.dumps(headers)
```

### Comparing `ytmusicapi-0.9.2/ytmusicapi/ytmusic.py` & `ytmusicapi-1.0.0/ytmusicapi/ytmusic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,129 +1,151 @@
 import requests
-import json
 import gettext
-import pkg_resources
 import os
+from functools import partial
 from contextlib import suppress
 from typing import Dict
+
+from ytmusicapi.auth.headers import prepare_headers
+from ytmusicapi.parsers.i18n import Parser
 from ytmusicapi.helpers import *
-from ytmusicapi.parsers import browsing
-from ytmusicapi.setup import setup
 from ytmusicapi.mixins.browsing import BrowsingMixin
+from ytmusicapi.mixins.search import SearchMixin
 from ytmusicapi.mixins.watch import WatchMixin
+from ytmusicapi.mixins.explore import ExploreMixin
 from ytmusicapi.mixins.library import LibraryMixin
 from ytmusicapi.mixins.playlists import PlaylistsMixin
 from ytmusicapi.mixins.uploads import UploadsMixin
 
-params = '?alt=json&key=AIzaSyC9XL3ZjWddXya6X74dJoCTL-WEYFDNX30'
-base_url = 'https://music.youtube.com/youtubei/v1/'
-
 
-class YTMusic(BrowsingMixin, WatchMixin, LibraryMixin, PlaylistsMixin, UploadsMixin):
+class YTMusic(BrowsingMixin, SearchMixin, WatchMixin, ExploreMixin, LibraryMixin, PlaylistsMixin,
+              UploadsMixin):
     """
     Allows automated interactions with YouTube Music by emulating the YouTube web client's requests.
     Permits both authenticated and non-authenticated requests.
     Authentication header data must be provided on initialization.
     """
+
     def __init__(self,
                  auth: str = None,
                  user: str = None,
+                 requests_session=True,
                  proxies: dict = None,
                  language: str = 'en'):
         """
         Create a new instance to interact with YouTube Music.
 
         :param auth: Optional. Provide a string or path to file.
           Authentication credentials are needed to manage your library.
-          Should be an adjusted version of `headers_auth.json.example` in the project root.
           See :py:func:`setup` for how to fill in the correct credentials.
           Default: A default header is used without authentication.
         :param user: Optional. Specify a user ID string to use in requests.
           This is needed if you want to send requests on behalf of a brand account.
           Otherwise the default account is used. You can retrieve the user ID
-          by going to https://myaccount.google.com and selecting your brand account.
+          by going to https://myaccount.google.com/brandaccounts and selecting your brand account.
           The user ID will be in the URL: https://myaccount.google.com/b/user_id/
+        :param requests_session: A Requests session object or a truthy value to create one.
+          Default sessions have a request timeout of 30s, which produces a requests.exceptions.ReadTimeout.
+          The timeout can be changed by passing your own Session object::
+
+            s = requests.Session()
+            s.request = functools.partial(s.request, timeout=3)
+            ytm = YTMusic(session=s)
+
+          A falsy value disables sessions.
+          It is generally a good idea to keep sessions enabled for
+          performance reasons (connection pooling).
         :param proxies: Optional. Proxy configuration in requests_ format_.
 
             .. _requests: https://requests.readthedocs.io/
             .. _format: https://requests.readthedocs.io/en/master/user/advanced/#proxies
 
         :param language: Optional. Can be used to change the language of returned data.
             English will be used by default. Available languages can be checked in
             the ytmusicapi/locales directory.
         """
         self.auth = auth
+
+        if isinstance(requests_session, requests.Session):
+            self._session = requests_session
+        else:
+            if requests_session:  # Build a new session.
+                self._session = requests.Session()
+                self._session.request = partial(self._session.request, timeout=30)
+            else:  # Use the Requests API module as a "session".
+                self._session = requests.api
+
         self.proxies = proxies
+        self.cookies = {'CONSENT': 'YES+1'}
 
+        self.headers = prepare_headers(self._session, proxies, auth)
+
+        if 'x-goog-visitor-id' not in self.headers:
+            self.headers.update(get_visitor_id(self._send_get_request))
+
+        # prepare context
+        self.context = initialize_context()
+        self.context['context']['client']['hl'] = language
+        locale_dir = os.path.abspath(os.path.dirname(__file__)) + os.sep + 'locales'
+        supported_languages = [f for f in next(os.walk(locale_dir))[1]]
+        if language not in supported_languages:
+            raise Exception("Language not supported. Supported languages are "
+                            + (', '.join(supported_languages)) + ".")
+        self.language = language
         try:
-            if auth is None or os.path.isfile(auth):
-                file = auth if auth else pkg_resources.resource_filename(
-                    'ytmusicapi', 'headers.json')
-                with open(file) as json_file:
-                    self.headers = json.load(json_file)
-            else:
-                self.headers = json.loads(auth)
-        except Exception as e:
-            print(
-                "Failed loading provided credentials. Make sure to provide a string or a file path. "
-                "Reason: " + str(e))
-
-        with open(pkg_resources.resource_filename('ytmusicapi', 'context.json')) as json_file:
-            self.context = json.load(json_file)
-            self.context['context']['client']['hl'] = language
-            supported_languages = [
-                f for f in pkg_resources.resource_listdir('ytmusicapi', 'locales')
-            ]
-            if language not in supported_languages:
-                raise Exception("Language not supported. Supported languages are "
-                                ', '.join(supported_languages))
-            self.language = language
+            locale.setlocale(locale.LC_ALL, self.language)
+        except locale.Error:
+            with suppress(locale.Error):
+                locale.setlocale(locale.LC_ALL, 'en_US.UTF-8')
+        self.lang = gettext.translation('base', localedir=locale_dir, languages=[language])
+        self.parser = Parser(self.lang)
+
+        if user:
+            self.context['context']['user']['onBehalfOfUser'] = user
+
+        auth_header = self.headers.get("authorization")
+        self.is_browser_auth = auth_header and "SAPISIDHASH" in auth_header
+        if self.is_browser_auth:
             try:
-                locale.setlocale(locale.LC_ALL, language)
-            except locale.Error:
-                with suppress(locale.Error):
-                    locale.setlocale(locale.LC_ALL, 'en_US.UTF-8')
-            self.lang = gettext.translation('base',
-                                            localedir=pkg_resources.resource_filename(
-                                                'ytmusicapi', 'locales'),
-                                            languages=[language])
-            self.parser = browsing.Parser(self.lang)
-
-            if user:
-                self.context['context']['user']['onBehalfOfUser'] = user
-
-        # verify authentication credentials work
-        if auth:
-            self.sapisid = sapisid_from_cookie(self.headers['Cookie'])
-            response = self._send_request('guide', {})
-            if 'error' in response:
-                raise Exception(
-                    "The provided credentials are invalid. Reason given by the server: "
-                    + response['error']['status'])
+                cookie = self.headers.get('cookie')
+                self.sapisid = sapisid_from_cookie(cookie)
+            except KeyError:
+                raise Exception("Your cookie is missing the required value __Secure-3PAPISID")
 
     def _send_request(self, endpoint: str, body: Dict, additionalParams: str = "") -> Dict:
         body.update(self.context)
-        if self.auth:
-            self.headers["Authorization"] = get_authorization(self.sapisid + ' '
-                                                              + self.headers['x-origin'])
-        response = requests.post(base_url + endpoint + params + additionalParams,
-                                 json=body,
-                                 headers=self.headers,
-                                 proxies=self.proxies)
-        return json.loads(response.text)
+        params = YTM_PARAMS
+        if self.is_browser_auth:
+            origin = self.headers.get('origin', self.headers.get('x-origin'))
+            self.headers["authorization"] = get_authorization(self.sapisid + ' ' + origin)
+            params += YTM_PARAMS_KEY
+
+        response = self._session.post(YTM_BASE_API + endpoint + params + additionalParams,
+                                      json=body,
+                                      headers=self.headers,
+                                      proxies=self.proxies,
+                                      cookies=self.cookies)
+        response_text = json.loads(response.text)
+        if response.status_code >= 400:
+            message = "Server returned HTTP " + str(
+                response.status_code) + ": " + response.reason + ".\n"
+            error = response_text.get('error', {}).get('message')
+            raise Exception(message + error)
+        return response_text
+
+    def _send_get_request(self, url: str, params: Dict = None):
+        response = self._session.get(url,
+                                     params=params,
+                                     headers=self.headers,
+                                     proxies=self.proxies,
+                                     cookies=self.cookies)
+        return response
 
     def _check_auth(self):
-        if self.auth == "":
+        if not self.auth:
             raise Exception("Please provide authentication before using this function")
 
-    @classmethod
-    def setup(cls, filepath: str = None, headers_raw: str = None) -> Dict:
-        """
-        Requests browser headers from the user via command line
-        and returns a string that can be passed to YTMusic()
+    def __enter__(self):
+        return self
 
-        :param filepath: Optional filepath to store headers to.
-        :param headers_raw: Optional request headers copied from browser.
-            Otherwise requested from terminal
-        :return: configuration headers string
-        """
-        return setup(filepath, headers_raw)
+    def __exit__(self, execType=None, execValue=None, trackback=None):
+        pass
```

