# Comparing `tmp/powermanim-0.0.5.tar.gz` & `tmp/powermanim-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powermanim-0.0.5.tar", last modified: Sun Mar 26 09:13:34 2023, max compression
+gzip compressed data, was "powermanim-0.0.6.tar", last modified: Fri Apr  7 23:26:19 2023, max compression
```

## Comparing `powermanim-0.0.5.tar` & `powermanim-0.0.6.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.387432 powermanim-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)      314 2023-03-26 09:10:33.000000 powermanim-0.0.5/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-03-26 09:10:33.000000 powermanim-0.0.5/.env.template
--rw-r--r--   0 runner    (1001) docker     (122)      154 2023-03-26 09:10:33.000000 powermanim-0.0.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.371431 powermanim-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.379432 powermanim-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-03-26 09:10:33.000000 powermanim-0.0.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)     4773 2023-03-26 09:10:33.000000 powermanim-0.0.5/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3749 2023-03-26 09:10:33.000000 powermanim-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-03-26 09:10:33.000000 powermanim-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-03-26 09:10:33.000000 powermanim-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1939 2023-03-26 09:13:34.387432 powermanim-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-03-26 09:10:33.000000 powermanim-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.379432 powermanim-0.0.5/data/
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-03-26 09:10:33.000000 powermanim-0.0.5/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.379432 powermanim-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      298 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/.hugo_build.lock
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.371431 powermanim-0.0.5/docs/assets/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.379432 powermanim-0.0.5/docs/assets/media/
--rw-r--r--   0 runner    (1001) docker     (122)    39583 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/assets/media/banner.png
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/assets/media/book.svg
--rw-r--r--   0 runner    (1001) docker     (122)    15329 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/assets/media/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.379432 powermanim-0.0.5/docs/assets/media/icons/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/assets/media/icons/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.379432 powermanim-0.0.5/docs/assets/scss/
--rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/assets/scss/custom.scss
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.371431 powermanim-0.0.5/docs/config/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.379432 powermanim-0.0.5/docs/config/_default/
--rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/config/_default/config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/config/_default/languages.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      358 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/config/_default/menus.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1921 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/config/_default/params.yaml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.375431 powermanim-0.0.5/docs/content/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.371431 powermanim-0.0.5/docs/content/authors/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.379432 powermanim-0.0.5/docs/content/authors/admin/
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/content/authors/admin/_index.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.379432 powermanim-0.0.5/docs/content/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/content/docs/_index.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.379432 powermanim-0.0.5/docs/content/docs/chapter1/
--rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/content/docs/chapter1/_index.md
--rw-r--r--   0 runner    (1001) docker     (122)     6549 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/content/docs/chapter1/reading-list.md
--rw-r--r--   0 runner    (1001) docker     (122)     6498 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/content/docs/chapter1/syllabus.md
--rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/content/docs/chapter1/takeaways.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.383432 powermanim-0.0.5/docs/content/docs/chapter2/
--rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/content/docs/chapter2/_index.md
--rw-r--r--   0 runner    (1001) docker     (122)     6549 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/content/docs/chapter2/reading-list.md
--rw-r--r--   0 runner    (1001) docker     (122)     6498 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/content/docs/chapter2/syllabus.md
--rw-r--r--   0 runner    (1001) docker     (122)     3350 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/content/docs/chapter2/takeaways.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.383432 powermanim-0.0.5/docs/content/home/
--rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/content/home/animations.md
--rw-r--r--   0 runner    (1001) docker     (122)      411 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/content/home/features.md
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/content/home/index.md
--rw-r--r--   0 runner    (1001) docker     (122)      507 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/go.mod
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.375431 powermanim-0.0.5/docs/layouts/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.375431 powermanim-0.0.5/docs/layouts/partials/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.383432 powermanim-0.0.5/docs/layouts/partials/views/
--rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/layouts/partials/views/masonry.html
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/netlify.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.375431 powermanim-0.0.5/docs/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.383432 powermanim-0.0.5/docs/static/uploads/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-26 09:10:33.000000 powermanim-0.0.5/docs/static/uploads/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-03-26 09:13:25.000000 powermanim-0.0.5/env.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      982 2023-03-26 09:10:33.000000 powermanim-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-26 09:13:34.387432 powermanim-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-03-26 09:10:33.000000 powermanim-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.375431 powermanim-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.383432 powermanim-0.0.5/src/powermanim/
--rw-r--r--   0 runner    (1001) docker     (122)      282 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-03-26 09:13:34.000000 powermanim-0.0.5/src/powermanim/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.383432 powermanim-0.0.5/src/powermanim/components/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2271 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/components/_powermanim.py
--rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/components/chartbars.py
--rw-r--r--   0 runner    (1001) docker     (122)     1119 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/components/numberslider.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/components/vgrouphighlight.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.383432 powermanim-0.0.5/src/powermanim/layouts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4244 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/layouts/arrangedbullets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.383432 powermanim-0.0.5/src/powermanim/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (122)     2152 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/scripts/build_anims
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.383432 powermanim-0.0.5/src/powermanim/showcase/
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/showcase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.383432 powermanim-0.0.5/src/powermanim/showcase/components/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/showcase/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/showcase/components/chartbars.py
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/showcase/components/numberslider.py
--rw-r--r--   0 runner    (1001) docker     (122)      997 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/showcase/components/vgroupghighlight.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.387432 powermanim-0.0.5/src/powermanim/showcase/layouts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/showcase/layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/showcase/layouts/arrangedbullets.py
--rw-r--r--   0 runner    (1001) docker     (122)      707 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/showcase/showcasescene.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.387432 powermanim-0.0.5/src/powermanim/showcase/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/showcase/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/showcase/templates/bulletlist.py
--rw-r--r--   0 runner    (1001) docker     (122)      378 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/showcase/templates/sectiontitle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.387432 powermanim-0.0.5/src/powermanim/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2699 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/templates/bulletlist.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-03-26 09:10:33.000000 powermanim-0.0.5/src/powermanim/templates/sectiontitle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.383432 powermanim-0.0.5/src/powermanim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1939 2023-03-26 09:13:34.000000 powermanim-0.0.5/src/powermanim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2396 2023-03-26 09:13:34.000000 powermanim-0.0.5/src/powermanim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-26 09:13:34.000000 powermanim-0.0.5/src/powermanim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-26 09:11:51.000000 powermanim-0.0.5/src/powermanim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      152 2023-03-26 09:13:34.000000 powermanim-0.0.5/src/powermanim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-03-26 09:13:34.000000 powermanim-0.0.5/src/powermanim.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.387432 powermanim-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-26 09:10:33.000000 powermanim-0.0.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-26 09:13:34.387432 powermanim-0.0.5/tests/showcase/
--rw-r--r--   0 runner    (1001) docker     (122)      467 2023-03-26 09:10:33.000000 powermanim-0.0.5/tests/showcase/test_showcasing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (122)      314 2023-04-07 23:23:00.000000 powermanim-0.0.6/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-04-07 23:23:00.000000 powermanim-0.0.6/.env.template
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-04-07 23:23:00.000000 powermanim-0.0.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     6429 2023-04-07 23:23:00.000000 powermanim-0.0.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4773 2023-04-07 23:23:00.000000 powermanim-0.0.6/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3749 2023-04-07 23:23:00.000000 powermanim-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     3933 2023-04-07 23:23:00.000000 powermanim-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-04-07 23:23:00.000000 powermanim-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     1939 2023-04-07 23:26:19.965717 powermanim-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1480 2023-04-07 23:23:00.000000 powermanim-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/data/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-04-07 23:23:00.000000 powermanim-0.0.6/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      298 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/.hugo_build.lock
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/docs/assets/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/assets/media/
+-rw-r--r--   0 runner    (1001) docker     (122)    39583 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/assets/media/banner.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/assets/media/book.svg
+-rw-r--r--   0 runner    (1001) docker     (122)    15329 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/assets/media/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/assets/media/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/assets/media/icons/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/assets/scss/
+-rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/assets/scss/custom.scss
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/docs/config/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/config/_default/
+-rw-r--r--   0 runner    (1001) docker     (122)     2083 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/config/_default/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      596 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/config/_default/languages.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/config/_default/menus.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     1921 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/config/_default/params.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/docs/content/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/docs/content/authors/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/content/authors/admin/
+-rw-r--r--   0 runner    (1001) docker     (122)      209 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/authors/admin/_index.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/content/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/_index.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/content/docs/chapter1/
+-rw-r--r--   0 runner    (1001) docker     (122)     1752 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter1/_index.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6549 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter1/reading-list.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6498 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter1/syllabus.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter1/takeaways.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/content/docs/chapter2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1737 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter2/_index.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6549 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter2/reading-list.md
+-rw-r--r--   0 runner    (1001) docker     (122)     6498 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter2/syllabus.md
+-rw-r--r--   0 runner    (1001) docker     (122)     3350 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/docs/chapter2/takeaways.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/content/home/
+-rw-r--r--   0 runner    (1001) docker     (122)     1601 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/home/animations.md
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/home/features.md
+-rw-r--r--   0 runner    (1001) docker     (122)      107 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/content/home/index.md
+-rw-r--r--   0 runner    (1001) docker     (122)      507 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/go.mod
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/docs/layouts/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/docs/layouts/partials/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.961717 powermanim-0.0.6/docs/layouts/partials/views/
+-rw-r--r--   0 runner    (1001) docker     (122)     1686 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/layouts/partials/views/masonry.html
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/netlify.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/docs/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/docs/static/uploads/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/docs/static/uploads/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (122)      138 2023-04-07 23:26:12.000000 powermanim-0.0.6/env.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      982 2023-04-07 23:23:00.000000 powermanim-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-04-07 23:26:19.969717 powermanim-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-04-07 23:23:00.000000 powermanim-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.957717 powermanim-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/
+-rw-r--r--   0 runner    (1001) docker     (122)      282 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-07 23:26:19.000000 powermanim-0.0.6/src/powermanim/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/components/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2632 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/components/chartbars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1119 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/components/numberslider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2517 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/components/powermanim.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3048 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/components/vgrouphighlight.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/layouts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/layouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4897 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/layouts/arrangedbullets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2152 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/scripts/build_anims
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/showcase/
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/showcase/components/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/components/chartbars.py
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/components/numberslider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/components/vgroupghighlight.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/showcase/layouts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/layouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/layouts/arrangedbullets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/showcasescene.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/showcase/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1394 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/templates/bulletlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/showcase/templates/sectiontitle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/templates/bulletlist.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-04-07 23:23:00.000000 powermanim-0.0.6/src/powermanim/templates/sectiontitle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/src/powermanim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1939 2023-04-07 23:26:19.000000 powermanim-0.0.6/src/powermanim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2395 2023-04-07 23:26:19.000000 powermanim-0.0.6/src/powermanim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 23:26:19.000000 powermanim-0.0.6/src/powermanim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-07 23:24:14.000000 powermanim-0.0.6/src/powermanim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      152 2023-04-07 23:26:19.000000 powermanim-0.0.6/src/powermanim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-04-07 23:26:19.000000 powermanim-0.0.6/src/powermanim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-07 23:23:00.000000 powermanim-0.0.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-07 23:26:19.965717 powermanim-0.0.6/tests/showcase/
+-rw-r--r--   0 runner    (1001) docker     (122)      467 2023-04-07 23:23:00.000000 powermanim-0.0.6/tests/showcase/test_showcasing.py
```

### Comparing `powermanim-0.0.5/.github/workflows/publish.yml` & `powermanim-0.0.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/.github/workflows/tests.yml` & `powermanim-0.0.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/.gitignore` & `powermanim-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/.pre-commit-config.yaml` & `powermanim-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/LICENSE` & `powermanim-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/PKG-INFO` & `powermanim-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powermanim
-Version: 0.0.5
+Version: 0.0.6
 Summary: Manim extension with custom components, layouts and slide templates aimed to ease the development of live presentations.
 Home-page: https://github.com/lucmos/powermanim
 Author: Luca Moschella
 Author-email: luca.moschella94@gmail.com
 License: MIT Licence
 Keywords: python
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powermanim Version: 0.0.5 Summary: Manim extension
+Metadata-Version: 2.1 Name: powermanim Version: 0.0.6 Summary: Manim extension
 with custom components, layouts and slide templates aimed to ease the
 development of live presentations. Home-page: https://github.com/lucmos/
 powermanim Author: Luca Moschella Author-email: luca.moschella94@gmail.com
 License: MIT Licence Keywords: python Description-Content-Type: text/markdown
 Provides-Extra: docs Provides-Extra: test Provides-Extra: dev License-File:
 LICENSE [![](docs/assets/media/banner.png)](https://lucmos.github.io/
 powermanim)
```

### Comparing `powermanim-0.0.5/README.md` & `powermanim-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/assets/media/banner.png` & `powermanim-0.0.6/docs/assets/media/banner.png`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/assets/media/book.svg` & `powermanim-0.0.6/docs/assets/media/book.svg`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/assets/media/icon.png` & `powermanim-0.0.6/docs/assets/media/icon.png`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/assets/scss/custom.scss` & `powermanim-0.0.6/docs/assets/scss/custom.scss`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/config/_default/config.yaml` & `powermanim-0.0.6/docs/config/_default/config.yaml`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/config/_default/languages.yaml` & `powermanim-0.0.6/docs/config/_default/languages.yaml`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/config/_default/params.yaml` & `powermanim-0.0.6/docs/config/_default/params.yaml`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/content/docs/chapter1/_index.md` & `powermanim-0.0.6/docs/content/docs/chapter1/_index.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/content/docs/chapter1/reading-list.md` & `powermanim-0.0.6/docs/content/docs/chapter1/reading-list.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/content/docs/chapter1/syllabus.md` & `powermanim-0.0.6/docs/content/docs/chapter1/syllabus.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/content/docs/chapter1/takeaways.md` & `powermanim-0.0.6/docs/content/docs/chapter1/takeaways.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/content/docs/chapter2/_index.md` & `powermanim-0.0.6/docs/content/docs/chapter2/_index.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/content/docs/chapter2/reading-list.md` & `powermanim-0.0.6/docs/content/docs/chapter2/reading-list.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/content/docs/chapter2/syllabus.md` & `powermanim-0.0.6/docs/content/docs/chapter2/syllabus.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/content/docs/chapter2/takeaways.md` & `powermanim-0.0.6/docs/content/docs/chapter2/takeaways.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/content/home/animations.md` & `powermanim-0.0.6/docs/content/home/animations.md`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/docs/layouts/partials/views/masonry.html` & `powermanim-0.0.6/docs/layouts/partials/views/masonry.html`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/pyproject.toml` & `powermanim-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/setup.cfg` & `powermanim-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/src/powermanim/components/_powermanim.py` & `powermanim-0.0.6/src/powermanim/components/powermanim.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,45 +11,54 @@
 
 
 class PowerManim(VGroup):
     def build_shapes(self):
         logo_green = "#87c2a5"
         logo_blue = "#525893"
         logo_red = "#e07a5f"
+
         circle = Circle(color=logo_green, fill_opacity=1).shift(LEFT)
-        square = Difference(Square().shift(UP), circle, color=logo_blue, fill_opacity=1).shift(UR * 0.2)
-        triangle = Difference(Triangle().shift(RIGHT), square, color=logo_red, fill_opacity=1).shift(DR * 0.2)
+
+        square = Square(color=logo_blue, fill_opacity=1).shift(UP)
+        triangle = Triangle(color=logo_red, fill_opacity=1).shift(RIGHT)
+
+        square = Difference(square, circle, color=logo_blue, fill_opacity=1)
+        triangle = Difference(triangle, square, color=logo_red, fill_opacity=1)
+
+        circle.shift(DL * self.gap)
+        triangle.shift(DR * self.gap)
+
         return VGroup(circle, square, triangle)
 
     def build_text(self):
-        logo_black = "#343434"
-        ds_m = MathTex(r"\mathbb{PM}", fill_color=logo_black).scale(5)
+        ds_m = MathTex(r"\mathbb{PM}", fill_color=self.logo_black).scale(5)
         ds_m.shift(4.25 * LEFT + 1.5 * UP)
         return ds_m
 
     def build_banner(self):
         shapes = self.build_shapes()
 
-        font_color = "#343434"
-        logo_black = "#343434"
-
-        ds_p = MathTex(r"\mathbb{P}", fill_color=logo_black).scale(2)
+        ds_p = MathTex(r"\mathbb{P}", fill_color=self.logo_black).scale(2)
         ower = Tex("ower", tex_template=TexFontTemplates.gnu_freeserif_freesans).scale(2)
-        ower.next_to(ds_p, RIGHT, buff=SMALL_BUFF).align_to(ds_p, DOWN).set_color(font_color)
+        ower.next_to(ds_p, RIGHT, buff=SMALL_BUFF).align_to(ds_p, DOWN).set_color(self.font_color)
         power = VGroup(ds_p, ower)
 
-        ds_m = MathTex(r"\mathbb{M}", fill_color=logo_black).scale(2)
+        ds_m = MathTex(r"\mathbb{M}", fill_color=self.logo_black).scale(2)
         anim = Tex("anim", tex_template=TexFontTemplates.gnu_freeserif_freesans).scale(2)
-        anim.next_to(ds_m, RIGHT, buff=SMALL_BUFF).align_to(ds_m, DOWN).set_color(font_color)
+        anim.next_to(ds_m, RIGHT, buff=SMALL_BUFF).align_to(ds_m, DOWN).set_color(self.font_color)
         tmanim = VGroup(ds_m, anim)
 
         banner = VGroup(power, tmanim).arrange(RIGHT, buff=MED_SMALL_BUFF).move_to(ORIGIN).scale(1.5)
-        banner.shift(UP * 0.5 + LEFT * 0.5)
-        shapes.next_to(banner.get_critical_point(DR), DR, buff=-1)
+        banner.next_to(shapes[1], LEFT)
+        banner.align_to(shapes[0].get_critical_point(UP) + self.gap, DOWN)
 
         return VGroup(shapes, banner).move_to(ORIGIN)
 
-    def __init__(self):
+    def __init__(self, font_color="#343434", logo_black="#343434", gap=0.4):
+        self.font_color = font_color
+        self.logo_black = logo_black
+        self.gap = gap
+
         shapes = self.build_shapes()
         ds_m = self.build_text()
         super().__init__(*shapes, ds_m)
         self.move_to(ORIGIN)
```

### Comparing `powermanim-0.0.5/src/powermanim/components/chartbars.py` & `powermanim-0.0.6/src/powermanim/components/chartbars.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/src/powermanim/components/numberslider.py` & `powermanim-0.0.6/src/powermanim/components/numberslider.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/src/powermanim/components/vgrouphighlight.py` & `powermanim-0.0.6/src/powermanim/components/vgrouphighlight.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self.active_opacity = active_opacity
         self.scale_active = scale_active
         self.scale_about_point = scale_about_point
         self.scale_about_edge = scale_about_edge
 
         self.previously_active_idxs = []
 
-    def highlight(self, scene: Scene, indices: T.Union[int, T.Sequence[int]]) -> None:
+    def highlight(self, indices: T.Union[int, T.Sequence[int]]) -> AnimationGroup:
         """Highlights the submobjects in the given indices in the scene.
 
         Args:
             scene:
                 The scene in which the animation is played.
 
             indices:
@@ -73,11 +73,8 @@
                 if previously_active_idx not in indices:
                     anims.append(
                         self.submobjects[previously_active_idx].animate.restore(),
                     )
 
         self.previously_active_idxs = indices
 
-        scene.play(
-            AnimationGroup(*anims, lag_ratio=self.anim_lag_ratio),
-            run_time=self.anim_run_time,
-        )
+        return AnimationGroup(*anims, lag_ratio=self.anim_lag_ratio)
```

### Comparing `powermanim-0.0.5/src/powermanim/layouts/arrangedbullets.py` & `powermanim-0.0.6/src/powermanim/layouts/arrangedbullets.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 import typing as T
 from collections import defaultdict
 
 from manim import *
 
 
-class Bullet(VGroup):
+class MathBullet(MathTex):
     def __init__(
         self,
-        *text: T.Union[Tex, Text, MathTex],
+        *text: str,
         level: int = 0,
         group: T.Optional[int] = None,
         adjustment: float = 0.0,
-        symbol: T.Optional[str] = r"$\bullet$",
-        buff: float = DEFAULT_MOBJECT_TO_MOBJECT_BUFFER,
-        text_components_buff: float = DEFAULT_MOBJECT_TO_MOBJECT_BUFFER,
+        symbol: T.Optional[str] = r"\bullet",
+        autoplace: bool = True,
+        **kwargs,
     ):
         """A class to represent a bullet point.
 
         Args:
             text: The text to be displayed.
             level: The indent level of the bullet point.
             group: The group the bullet point belongs to, controls the animations.
             adjustment: The adjustment of the bullet.
             symbol: The symbol to be displayed as the bullet.
-            buff: The spacing between the bullet and the text.
-            text_components_buff: The spacing between the text components.
+            autoplace: Whether to automatically place the bullet point.
         """
         self.level = level
         self.adjustment = adjustment
         self.group = group
+        self.symbol = symbol
+        self.autoplace = autoplace
 
-        self.text = VGroup(*text).arrange(RIGHT, buff=text_components_buff)
-        self.bullet = symbol
-
+        first_text, *rest_text = text
         if symbol is not None:
-            self.bullet = Tex(symbol)
-            self.bullet.next_to(self.text, LEFT, buff=buff)
-        super().__init__(VGroup(self.bullet, self.text) if self.bullet is not None else self.text)
+            first_text = rf"{symbol}~{first_text}"
+
+        super().__init__(first_text, *rest_text, **kwargs)
 
     def indent(self, indent_buff: float = MED_LARGE_BUFF * 1.5):
         """Indent the bullet point.
 
         Args:
             indent_buff: The spacing between the bullet and the text.
         """
@@ -61,18 +60,61 @@
             adjustment: The shift of the bullet.
         """
         if adjustment is None:
             adjustment = self.adjustment
         self.shift(self.adjustment)
 
 
+class Bullet(MathBullet):
+    def __init__(
+        self,
+        *text: str,
+        level: int = 0,
+        group: T.Optional[int] = None,
+        adjustment: float = 0.0,
+        symbol: T.Optional[str] = r"$\bullet$",
+        force_inline: bool = False,
+        arg_separator="",
+        tex_environment="center",
+        **kwargs,
+    ):
+        first_text, *rest_text = text
+        if force_inline:
+            first_text = r"\mbox{" + first_text
+            rest_text = *rest_text, r"}"
+
+        super().__init__(
+            first_text,
+            *rest_text,
+            level=level,
+            group=group,
+            adjustment=adjustment,
+            symbol=symbol,
+            arg_separator=arg_separator,
+            tex_environment=tex_environment,
+            **kwargs,
+        )
+
+
 class ArrangedBullets(VGroup):
+    def arrage_rows(self, rows: T.Iterable[T.Union[MathBullet, Bullet, MathTex, Tex, Text]]):
+        bullet_rows: T.Iterable[MathBullet] = (
+            VGroup(*rows)
+            .arrange(DOWN, aligned_edge=LEFT, buff=self.line_spacing)
+            .to_edge(LEFT, buff=self.left_buff)
+            .shift(self.global_shift)
+        )
+
+        for row in bullet_rows:
+            row.indent(indent_buff=self.indent_buff)
+            row.adjust()
+
     def __init__(
         self,
-        *rows: T.Union[Bullet, MathTex, Tex, Text],
+        *rows: T.Union[MathBullet, Bullet, MathTex, Tex, Text],
         line_spacing: float = MED_LARGE_BUFF * 1.5,
         indent_buff: float = MED_LARGE_BUFF * 1.5,
         left_buff: float = MED_LARGE_BUFF * 1.5,
         global_shift: float = 0.0,
     ):
         """A VGroup that arranges the rows in a list of bullet points.
 
@@ -84,37 +126,26 @@
             global_shift: The global_shift of the rows.
         """
         self.line_spacing = line_spacing
         self.indent_buff = indent_buff
         self.left_buff = left_buff
         self.global_shift = global_shift
 
-        rows = [(row if isinstance(row, Bullet) else Bullet(row)) for row in rows]
-        bullet_rows: T.Iterable[Bullet] = (
-            VGroup(*rows)
-            .arrange(DOWN, aligned_edge=LEFT, buff=line_spacing)
-            .to_edge(LEFT, buff=left_buff)
-            .shift(global_shift)
-        )
+        rows = [(row if isinstance(row, MathBullet) else Bullet(row)) for row in rows]
 
-        for row in bullet_rows:
-            row.indent(indent_buff=indent_buff)
-            row.adjust()
+        self.arrage_rows((row for row in rows if row.autoplace))
 
-        groups = [row.group for row in bullet_rows]
+        groups = [row.group for row in rows]
 
         # If there is a None and aso something else
         if (None in groups) and len(set(groups)) != 1:
             raise ValueError("The groups must be specified for all or no bullets at all.")
 
-        if None in groups:
-            groups = list(range(len(bullet_rows)))
-
         group2bullet = defaultdict(list)
-        for i, row in enumerate(bullet_rows):
+        for i, row in enumerate(rows):
             group = row.group
             if group is None:
                 group = i
             group2bullet[group].append(row)
 
         group_rows = []
         for _, bullets in group2bullet.items():
```

### Comparing `powermanim-0.0.5/src/powermanim/scripts/build_anims` & `powermanim-0.0.6/src/powermanim/scripts/build_anims`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/src/powermanim/showcase/__init__.py` & `powermanim-0.0.6/src/powermanim/showcase/__init__.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/src/powermanim/showcase/components/chartbars.py` & `powermanim-0.0.6/src/powermanim/showcase/components/chartbars.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/src/powermanim/showcase/components/numberslider.py` & `powermanim-0.0.6/src/powermanim/showcase/components/numberslider.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/src/powermanim/showcase/layouts/arrangedbullets.py` & `powermanim-0.0.6/src/powermanim/showcase/layouts/arrangedbullets.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 class ArrangedBulletsShowcase(ShowcaseScene):
     def showcasing():
         return ArrangedBullets
 
     def construct(self):
         rows = [
-            Bullet(Text("First row")),
-            Bullet(Text("Second row")),
-            Bullet(Text("Elements:")),
-            Bullet(Text("First element"), level=1, symbol="(1)"),
-            Bullet(Text("Second element"), level=1, symbol="(2)"),
-            Bullet(Text("Third element"), level=1, symbol="(3)"),
+            Bullet("First row"),
+            Bullet("Second row"),
+            Bullet("Elements:"),
+            Bullet("First element", level=1, symbol="(1)"),
+            Bullet("Second element", level=1, symbol="(2)"),
+            Bullet("Third element", level=1, symbol="(3)"),
         ]
         g_rows = VGroup(*rows).set_opacity(0.25).scale(0.9)
         g_rows.target = ArrangedBullets(
             *g_rows.copy(),
             line_spacing=MED_LARGE_BUFF * 1.25,
             left_buff=MED_LARGE_BUFF * 3,
         ).set_opacity(1)
```

### Comparing `powermanim-0.0.5/src/powermanim/showcase/showcasescene.py` & `powermanim-0.0.6/src/powermanim/showcase/showcasescene.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/src/powermanim/templates/bulletlist.py` & `powermanim-0.0.6/src/powermanim/templates/bulletlist.py`

 * *Files 20% similar despite different names*

```diff
@@ -44,32 +44,33 @@
             scale_active=scale_active,
             scale_about_edge=LEFT,
         )
         super().__init__(self.rows)
 
         self.highlighted = 0
 
-    def also_next(self, scene: Scene) -> None:
+    def also_next(self) -> Animation:
         """Highlights also the next item in the list."""
         self.highlighted += 1
 
         if self.highlighted > self.arranged_list.ngroups:
             raise StopIteration("No more elements to highlight.")
 
-        self.rows.highlight(scene=scene, indices=list(range(self.highlighted)))
+        return self.rows.highlight(indices=list(range(self.highlighted)))
 
-    def only_next(self, scene: Scene) -> None:
+    def only_next(self) -> Animation:
         """Highlights only the next item in the list."""
         if self.highlighted > self.arranged_list.ngroups:
             raise StopIteration("No more elements to highlight.")
-
-        self.rows.highlight(scene=scene, indices=self.highlighted)
+        anims = self.rows.highlight(indices=self.highlighted)
         self.highlighted += 1
+        return anims
 
-    def clear(self, scene: Scene) -> None:
+    def clear(self) -> Animation:
         """Clears the list hightlighting."""
-        self.rows.highlight(scene=scene, indices=[])
+        anims = self.rows.highlight(indices=[])
         self.highlighted = 0
+        return anims
 
-    def all(self, scene: Scene) -> None:
+    def all(self) -> Animation:
         """Highlights all the list."""
-        self.rows.highlight(scene=scene, indices=list(range(len(self.rows))))
+        return self.rows.highlight(indices=list(range(len(self.rows))))
```

### Comparing `powermanim-0.0.5/src/powermanim/templates/sectiontitle.py` & `powermanim-0.0.6/src/powermanim/templates/sectiontitle.py`

 * *Files identical despite different names*

### Comparing `powermanim-0.0.5/src/powermanim.egg-info/PKG-INFO` & `powermanim-0.0.6/src/powermanim.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powermanim
-Version: 0.0.5
+Version: 0.0.6
 Summary: Manim extension with custom components, layouts and slide templates aimed to ease the development of live presentations.
 Home-page: https://github.com/lucmos/powermanim
 Author: Luca Moschella
 Author-email: luca.moschella94@gmail.com
 License: MIT Licence
 Keywords: python
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: powermanim Version: 0.0.5 Summary: Manim extension
+Metadata-Version: 2.1 Name: powermanim Version: 0.0.6 Summary: Manim extension
 with custom components, layouts and slide templates aimed to ease the
 development of live presentations. Home-page: https://github.com/lucmos/
 powermanim Author: Luca Moschella Author-email: luca.moschella94@gmail.com
 License: MIT Licence Keywords: python Description-Content-Type: text/markdown
 Provides-Extra: docs Provides-Extra: test Provides-Extra: dev License-File:
 LICENSE [![](docs/assets/media/banner.png)](https://lucmos.github.io/
 powermanim)
```

### Comparing `powermanim-0.0.5/src/powermanim.egg-info/SOURCES.txt` & `powermanim-0.0.6/src/powermanim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 src/powermanim.egg-info/PKG-INFO
 src/powermanim.egg-info/SOURCES.txt
 src/powermanim.egg-info/dependency_links.txt
 src/powermanim.egg-info/not-zip-safe
 src/powermanim.egg-info/requires.txt
 src/powermanim.egg-info/top_level.txt
 src/powermanim/components/__init__.py
-src/powermanim/components/_powermanim.py
 src/powermanim/components/chartbars.py
 src/powermanim/components/numberslider.py
+src/powermanim/components/powermanim.py
 src/powermanim/components/vgrouphighlight.py
 src/powermanim/layouts/__init__.py
 src/powermanim/layouts/arrangedbullets.py
 src/powermanim/scripts/build_anims
 src/powermanim/showcase/__init__.py
 src/powermanim/showcase/showcasescene.py
 src/powermanim/showcase/components/__init__.py
```

