# Comparing `tmp/django-insights-0.1.7.tar.gz` & `tmp/django-insights-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-insights-0.1.7.tar", last modified: Wed Apr  5 21:50:01 2023, max compression
+gzip compressed data, was "django-insights-0.1.8.tar", last modified: Sat Apr  8 18:04:21 2023, max compression
```

## Comparing `django-insights-0.1.7.tar` & `django-insights-0.1.8.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0       56 2023-02-26 21:15:55.562658 django-insights-0.1.7/.flake8
--rw-r--r--   0        0        0      244 2023-03-28 21:32:35.215510 django-insights-0.1.7/.gitattributes
--rw-r--r--   0        0        0      891 2023-02-24 21:17:32.382096 django-insights-0.1.7/.github/workflows/main.yml
--rw-r--r--   0        0        0     3187 2023-04-05 21:13:27.224439 django-insights-0.1.7/.gitignore
--rw-r--r--   0        0        0      264 2023-02-26 20:52:10.152584 django-insights-0.1.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1109 2023-02-25 13:18:46.605352 django-insights-0.1.7/LICENSE
--rw-r--r--   0        0        0      623 2023-03-28 20:21:57.901560 django-insights-0.1.7/Makefile
--rw-r--r--   0        0        0     7966 2023-03-30 07:31:33.216404 django-insights-0.1.7/README.md
--rw-r--r--   0        0        0       46 2023-04-05 21:47:44.469414 django-insights-0.1.7/django_insights/__init__.py
--rw-r--r--   0        0        0      215 2023-02-26 11:01:11.047792 django-insights-0.1.7/django_insights/apps.py
--rw-r--r--   0        0        0     4149 2023-04-05 21:31:11.247613 django-insights-0.1.7/django_insights/charts.py
--rw-r--r--   0        0        0      259 2023-03-12 14:18:47.495430 django-insights-0.1.7/django_insights/choices.py
--rw-r--r--   0        0        0      884 2023-02-23 21:13:48.665974 django-insights-0.1.7/django_insights/database.py
--rw-r--r--   0        0        0        0 2023-02-23 21:13:48.666862 django-insights-0.1.7/django_insights/management/__init__.py
--rw-r--r--   0        0        0        0 2023-02-23 21:13:48.668039 django-insights-0.1.7/django_insights/management/commands/__init__.py
--rw-r--r--   0        0        0      462 2023-02-24 23:42:13.381163 django-insights-0.1.7/django_insights/management/commands/collect_insights.py
--rw-r--r--   0        0        0      871 2023-03-10 08:56:52.661518 django-insights-0.1.7/django_insights/managers.py
--rw-r--r--   0        0        0     8676 2023-03-28 13:24:36.228388 django-insights-0.1.7/django_insights/metrics.py
--rw-r--r--   0        0        0      725 2023-03-12 12:52:11.383735 django-insights-0.1.7/django_insights/metrics_types.py
--rw-r--r--   0        0        0     7904 2023-03-28 13:25:20.560193 django-insights-0.1.7/django_insights/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-03-28 07:45:20.815997 django-insights-0.1.7/django_insights/migrations/__init__.py
--rw-r--r--   0        0        0     4818 2023-03-28 20:23:30.873379 django-insights-0.1.7/django_insights/models.py
--rw-r--r--   0        0        0      383 2023-03-07 12:33:11.768638 django-insights-0.1.7/django_insights/packages/package.json
--rw-r--r--   0        0        0    15745 2023-03-07 12:33:11.768750 django-insights-0.1.7/django_insights/packages/pnpm-lock.yaml
--rw-r--r--   0        0        0        0 2023-02-23 21:13:48.678161 django-insights-0.1.7/django_insights/packages/src/index.js
--rw-r--r--   0        0        0       58 2023-02-23 21:13:48.678382 django-insights-0.1.7/django_insights/packages/src/input.css
--rw-r--r--   0        0        0     1680 2023-03-08 21:48:39.256071 django-insights-0.1.7/django_insights/packages/tailwind.config.js
--rw-r--r--   0        0        0     1002 2023-03-28 13:24:36.228540 django-insights-0.1.7/django_insights/registry.py
--rw-r--r--   0        0        0      646 2023-04-05 21:42:25.867540 django-insights-0.1.7/django_insights/settings.py
--rw-r--r--   0        0        0   529814 2023-03-08 22:12:02.091816 django-insights-0.1.7/django_insights/static/insights/css/insights.css
--rw-r--r--   0        0        0   353824 2015-07-10 13:05:30.000000 django-insights-0.1.7/django_insights/static/insights/fonts/ubuntu.ttf
--rw-r--r--   0        0        0    59706 2023-02-23 21:13:48.682069 django-insights-0.1.7/django_insights/static/insights/js/preline.js
--rw-r--r--   0        0        0    15501 2023-03-13 09:03:26.927652 django-insights-0.1.7/django_insights/templates/insights/app.html
--rw-r--r--   0        0        0     6902 2023-03-28 13:24:36.228639 django-insights-0.1.7/django_insights/templates/insights/base.html
--rw-r--r--   0        0        0     6380 2023-03-12 13:27:51.016392 django-insights-0.1.7/django_insights/templates/insights/dashboard.html
--rw-r--r--   0        0        0        0 2023-02-23 21:13:48.683405 django-insights-0.1.7/django_insights/templatetags/__init__.py
--rw-r--r--   0        0        0      494 2023-03-12 14:33:43.288031 django-insights-0.1.7/django_insights/templatetags/insight_chart.py
--rw-r--r--   0        0        0      147 2023-02-24 19:40:28.249653 django-insights-0.1.7/django_insights/templatetags/remove_substr.py
--rw-r--r--   0        0        0      459 2023-03-12 14:20:57.093944 django-insights-0.1.7/django_insights/urls.py
--rw-r--r--   0        0        0     2917 2023-04-05 21:42:56.386970 django-insights-0.1.7/django_insights/views.py
--rw-r--r--   0        0        0       15 2023-02-26 21:29:19.397018 django-insights-0.1.7/docs/alternatives.md
--rw-r--r--   0        0        0   104686 2023-03-08 20:52:29.374163 django-insights-0.1.7/docs/assets/images/banner.png
--rw-r--r--   0        0        0    76251 2023-03-30 07:08:50.901329 django-insights-0.1.7/docs/assets/images/screen_1.png
--rw-r--r--   0        0        0   220288 2023-03-30 07:09:17.833607 django-insights-0.1.7/docs/assets/images/screen_2.png
--rw-r--r--   0        0        0       29 2023-04-05 08:22:13.827431 django-insights-0.1.7/docs/index.md
--rw-r--r--   0        0        0       15 2023-02-26 10:44:14.900040 django-insights-0.1.7/docs/installation.md
--rw-r--r--   0        0        0     1125 2023-02-25 13:27:48.753743 django-insights-0.1.7/docs/license.md
--rw-r--r--   0        0        0      141 2023-04-05 08:33:05.969826 django-insights-0.1.7/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      147 2023-02-26 22:07:38.873478 django-insights-0.1.7/docs/types.md
--rwxr-xr-x   0        0        0      305 2023-02-27 21:15:11.665286 django-insights-0.1.7/manage.py
--rw-r--r--   0        0        0      745 2023-04-05 08:38:12.582792 django-insights-0.1.7/mkdocs.yml
--rw-r--r--   0        0        0        0 2023-02-23 23:09:34.899629 django-insights-0.1.7/project/__init__.py
--rw-r--r--   0        0        0        0 2023-02-27 21:13:14.042679 django-insights-0.1.7/project/settings/__init__.py
--rw-r--r--   0        0        0     2365 2023-04-05 21:10:10.757630 django-insights-0.1.7/project/settings/base.py
--rw-r--r--   0        0        0       44 2023-02-27 21:17:52.522054 django-insights-0.1.7/project/settings/dev.py
--rw-r--r--   0        0        0      216 2023-02-27 21:17:56.995963 django-insights-0.1.7/project/settings/test.py
--rw-r--r--   0        0        0        0 2023-02-23 22:04:55.674675 django-insights-0.1.7/project/testapp/__init__.py
--rw-r--r--   0        0        0      199 2023-03-27 15:07:38.129565 django-insights-0.1.7/project/testapp/apps.py
--rw-r--r--   0        0        0     4083 2023-03-28 09:51:28.154540 django-insights-0.1.7/project/testapp/insights.py
--rw-r--r--   0        0        0        0 2023-02-27 22:02:09.838142 django-insights-0.1.7/project/testapp/management/__init__.py
--rw-r--r--   0        0        0        0 2023-02-27 22:02:09.839797 django-insights-0.1.7/project/testapp/management/commands/__init__.py
--rw-r--r--   0        0        0     1589 2023-03-28 20:49:22.754952 django-insights-0.1.7/project/testapp/management/commands/seed_db.py
--rw-r--r--   0        0        0     2035 2023-03-28 13:22:15.312678 django-insights-0.1.7/project/testapp/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-03-28 07:45:20.309342 django-insights-0.1.7/project/testapp/migrations/__init__.py
--rw-r--r--   0        0        0      590 2023-03-27 19:21:14.518601 django-insights-0.1.7/project/testapp/models.py
--rw-r--r--   0        0        0        0 2023-03-27 15:07:00.152163 django-insights-0.1.7/project/testapp/users/__init__.py
--rw-r--r--   0        0        0      128 2023-03-27 19:24:32.782266 django-insights-0.1.7/project/testapp/users/apps.py
--rw-r--r--   0        0        0      322 2023-03-28 12:33:39.507403 django-insights-0.1.7/project/testapp/users/insights.py
--rw-r--r--   0        0        0     2812 2023-03-28 13:22:15.312746 django-insights-0.1.7/project/testapp/users/migrations/0001_initial.py
--rw-r--r--   0        0        0      406 2023-03-27 19:29:06.702145 django-insights-0.1.7/project/testapp/users/migrations/0002_alter_appuser_created.py
--rw-r--r--   0        0        0        0 2023-03-27 19:26:48.098800 django-insights-0.1.7/project/testapp/users/migrations/__init__.py
--rw-r--r--   0        0        0      589 2023-03-27 19:29:04.098220 django-insights-0.1.7/project/testapp/users/models.py
--rw-r--r--   0        0        0      391 2023-04-05 21:09:49.280598 django-insights-0.1.7/project/urls.py
--rw-r--r--   0        0        0     1858 2023-03-28 20:07:46.011067 django-insights-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3963 2023-02-24 21:17:19.425307 django-insights-0.1.7/requirements/compile.py
--rw-r--r--   0        0        0    27230 2023-03-08 20:34:30.812867 django-insights-0.1.7/requirements/py310-django32.txt
--rw-r--r--   0        0        0    27028 2023-03-08 20:34:32.608775 django-insights-0.1.7/requirements/py310-django40.txt
--rw-r--r--   0        0        0    27027 2023-03-08 20:34:34.407786 django-insights-0.1.7/requirements/py310-django41.txt
--rw-r--r--   0        0        0    27027 2023-03-08 20:34:36.255245 django-insights-0.1.7/requirements/py310-django42.txt
--rw-r--r--   0        0        0    26618 2023-03-08 20:34:39.816942 django-insights-0.1.7/requirements/py311-django41.txt
--rw-r--r--   0        0        0    26618 2023-03-08 20:34:41.452206 django-insights-0.1.7/requirements/py311-django42.txt
--rw-r--r--   0        0        0    27661 2023-03-08 20:34:11.169086 django-insights-0.1.7/requirements/py38-django32.txt
--rw-r--r--   0        0        0    28862 2023-03-08 20:34:13.341844 django-insights-0.1.7/requirements/py38-django40.txt
--rw-r--r--   0        0        0    28861 2023-03-08 20:34:15.479204 django-insights-0.1.7/requirements/py38-django41.txt
--rw-r--r--   0        0        0    28861 2023-03-08 20:34:17.666389 django-insights-0.1.7/requirements/py38-django42.txt
--rw-r--r--   0        0        0    27661 2023-03-08 20:34:22.041756 django-insights-0.1.7/requirements/py39-django32.txt
--rw-r--r--   0        0        0    27459 2023-03-08 20:34:24.070919 django-insights-0.1.7/requirements/py39-django40.txt
--rw-r--r--   0        0        0    27458 2023-03-08 20:34:26.018066 django-insights-0.1.7/requirements/py39-django41.txt
--rw-r--r--   0        0        0    27458 2023-03-08 20:34:28.097400 django-insights-0.1.7/requirements/py39-django42.txt
--rw-r--r--   0        0        0       49 2023-03-08 20:32:58.867282 django-insights-0.1.7/requirements/requirements.in
--rw-r--r--   0        0        0        0 2023-02-23 22:29:47.164960 django-insights-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0     1337 2023-03-28 13:31:30.803421 django-insights-0.1.7/tests/test_api.py
--rw-r--r--   0        0        0      232 2023-02-26 20:39:42.248922 django-insights-0.1.7/tests/utils.py
--rw-r--r--   0        0        0      365 2023-02-24 21:17:25.741397 django-insights-0.1.7/tox.ini
--rw-r--r--   0        0        0     9449 1970-01-01 00:00:00.000000 django-insights-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       56 2023-02-26 21:15:55.562658 django-insights-0.1.8/.flake8
+-rw-r--r--   0        0        0      244 2023-03-28 21:32:35.215510 django-insights-0.1.8/.gitattributes
+-rw-r--r--   0        0        0      891 2023-02-24 21:17:32.382096 django-insights-0.1.8/.github/workflows/main.yml
+-rw-r--r--   0        0        0     3187 2023-04-05 21:13:27.224439 django-insights-0.1.8/.gitignore
+-rw-r--r--   0        0        0      264 2023-02-26 20:52:10.152584 django-insights-0.1.8/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1109 2023-02-25 13:18:46.605352 django-insights-0.1.8/LICENSE
+-rw-r--r--   0        0        0      623 2023-03-28 20:21:57.901560 django-insights-0.1.8/Makefile
+-rw-r--r--   0        0        0     7984 2023-04-06 20:47:21.522352 django-insights-0.1.8/README.md
+-rw-r--r--   0        0        0       46 2023-04-08 17:59:45.396893 django-insights-0.1.8/django_insights/__init__.py
+-rw-r--r--   0        0        0      215 2023-02-26 11:01:11.047792 django-insights-0.1.8/django_insights/apps.py
+-rw-r--r--   0        0        0     4149 2023-04-05 21:31:11.247613 django-insights-0.1.8/django_insights/charts.py
+-rw-r--r--   0        0        0      259 2023-03-12 14:18:47.495430 django-insights-0.1.8/django_insights/choices.py
+-rw-r--r--   0        0        0      884 2023-02-23 21:13:48.665974 django-insights-0.1.8/django_insights/database.py
+-rw-r--r--   0        0        0        0 2023-02-23 21:13:48.666862 django-insights-0.1.8/django_insights/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-23 21:13:48.668039 django-insights-0.1.8/django_insights/management/commands/__init__.py
+-rw-r--r--   0        0        0      462 2023-02-24 23:42:13.381163 django-insights-0.1.8/django_insights/management/commands/collect_insights.py
+-rw-r--r--   0        0        0      871 2023-03-10 08:56:52.661518 django-insights-0.1.8/django_insights/managers.py
+-rw-r--r--   0        0        0     8766 2023-04-08 10:39:49.464770 django-insights-0.1.8/django_insights/metrics.py
+-rw-r--r--   0        0        0      725 2023-03-12 12:52:11.383735 django-insights-0.1.8/django_insights/metrics_types.py
+-rw-r--r--   0        0        0     7904 2023-03-28 13:25:20.560193 django-insights-0.1.8/django_insights/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-03-28 07:45:20.815997 django-insights-0.1.8/django_insights/migrations/__init__.py
+-rw-r--r--   0        0        0     4818 2023-03-28 20:23:30.873379 django-insights-0.1.8/django_insights/models.py
+-rw-r--r--   0        0        0      482 2023-04-08 17:35:49.087873 django-insights-0.1.8/django_insights/packages/package.json
+-rw-r--r--   0        0        0    22652 2023-04-08 17:29:02.239158 django-insights-0.1.8/django_insights/packages/pnpm-lock.yaml
+-rw-r--r--   0        0        0     1094 2023-04-08 17:33:41.969030 django-insights-0.1.8/django_insights/packages/src/index.js
+-rw-r--r--   0        0        0       58 2023-02-23 21:13:48.678382 django-insights-0.1.8/django_insights/packages/src/input.css
+-rw-r--r--   0        0        0     1658 2023-04-08 10:52:26.468020 django-insights-0.1.8/django_insights/packages/tailwind.config.js
+-rw-r--r--   0        0        0     1002 2023-03-28 13:24:36.228540 django-insights-0.1.8/django_insights/registry.py
+-rw-r--r--   0        0        0      646 2023-04-05 21:42:25.867540 django-insights-0.1.8/django_insights/settings.py
+-rw-r--r--   0        0        0    22995 2023-04-08 17:44:48.234018 django-insights-0.1.8/django_insights/static/insights/css/insights.css
+-rw-r--r--   0        0        0   353824 2015-07-10 13:05:30.000000 django-insights-0.1.8/django_insights/static/insights/fonts/ubuntu.ttf
+-rw-r--r--   0        0        0    61038 2023-04-08 17:35:51.682751 django-insights-0.1.8/django_insights/static/insights/js/insights.js
+-rw-r--r--   0        0        0    15501 2023-04-08 17:40:29.590099 django-insights-0.1.8/django_insights/templates/insights/app.html
+-rw-r--r--   0        0        0     6535 2023-04-08 17:48:58.492016 django-insights-0.1.8/django_insights/templates/insights/base.html
+-rw-r--r--   0        0        0     6359 2023-04-08 17:45:27.323555 django-insights-0.1.8/django_insights/templates/insights/dashboard.html
+-rw-r--r--   0        0        0        0 2023-02-23 21:13:48.683405 django-insights-0.1.8/django_insights/templatetags/__init__.py
+-rw-r--r--   0        0        0      494 2023-03-12 14:33:43.288031 django-insights-0.1.8/django_insights/templatetags/insight_chart.py
+-rw-r--r--   0        0        0      147 2023-02-24 19:40:28.249653 django-insights-0.1.8/django_insights/templatetags/remove_substr.py
+-rw-r--r--   0        0        0      459 2023-03-12 14:20:57.093944 django-insights-0.1.8/django_insights/urls.py
+-rw-r--r--   0        0        0     2949 2023-04-08 17:56:42.113914 django-insights-0.1.8/django_insights/views.py
+-rw-r--r--   0        0        0       15 2023-02-26 21:29:19.397018 django-insights-0.1.8/docs/alternatives.md
+-rw-r--r--   0        0        0   104686 2023-03-08 20:52:29.374163 django-insights-0.1.8/docs/assets/images/banner.png
+-rw-r--r--   0        0        0    76251 2023-03-30 07:08:50.901329 django-insights-0.1.8/docs/assets/images/screen_1.png
+-rw-r--r--   0        0        0   220288 2023-03-30 07:09:17.833607 django-insights-0.1.8/docs/assets/images/screen_2.png
+-rw-r--r--   0        0        0      742 2023-04-06 21:00:21.424436 django-insights-0.1.8/docs/index.md
+-rw-r--r--   0        0        0     1733 2023-04-06 21:03:35.460205 django-insights-0.1.8/docs/installation.md
+-rw-r--r--   0        0        0     1125 2023-02-25 13:27:48.753743 django-insights-0.1.8/docs/license.md
+-rw-r--r--   0        0        0       51 2023-04-08 10:38:49.029564 django-insights-0.1.8/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      147 2023-02-26 22:07:38.873478 django-insights-0.1.8/docs/types.md
+-rwxr-xr-x   0        0        0      305 2023-02-27 21:15:11.665286 django-insights-0.1.8/manage.py
+-rw-r--r--   0        0        0      828 2023-04-08 10:42:02.031696 django-insights-0.1.8/mkdocs.yml
+-rw-r--r--   0        0        0        0 2023-02-23 23:09:34.899629 django-insights-0.1.8/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-27 21:13:14.042679 django-insights-0.1.8/project/settings/__init__.py
+-rw-r--r--   0        0        0     2362 2023-04-08 17:45:53.136019 django-insights-0.1.8/project/settings/base.py
+-rw-r--r--   0        0        0       44 2023-02-27 21:17:52.522054 django-insights-0.1.8/project/settings/dev.py
+-rw-r--r--   0        0        0      216 2023-02-27 21:17:56.995963 django-insights-0.1.8/project/settings/test.py
+-rw-r--r--   0        0        0        0 2023-02-23 22:04:55.674675 django-insights-0.1.8/project/testapp/__init__.py
+-rw-r--r--   0        0        0      199 2023-03-27 15:07:38.129565 django-insights-0.1.8/project/testapp/apps.py
+-rw-r--r--   0        0        0     4083 2023-03-28 09:51:28.154540 django-insights-0.1.8/project/testapp/insights.py
+-rw-r--r--   0        0        0        0 2023-02-27 22:02:09.838142 django-insights-0.1.8/project/testapp/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-27 22:02:09.839797 django-insights-0.1.8/project/testapp/management/commands/__init__.py
+-rw-r--r--   0        0        0     1589 2023-03-28 20:49:22.754952 django-insights-0.1.8/project/testapp/management/commands/seed_db.py
+-rw-r--r--   0        0        0     2035 2023-03-28 13:22:15.312678 django-insights-0.1.8/project/testapp/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-03-28 07:45:20.309342 django-insights-0.1.8/project/testapp/migrations/__init__.py
+-rw-r--r--   0        0        0      590 2023-03-27 19:21:14.518601 django-insights-0.1.8/project/testapp/models.py
+-rw-r--r--   0        0        0        0 2023-03-27 15:07:00.152163 django-insights-0.1.8/project/testapp/users/__init__.py
+-rw-r--r--   0        0        0      128 2023-03-27 19:24:32.782266 django-insights-0.1.8/project/testapp/users/apps.py
+-rw-r--r--   0        0        0      322 2023-03-28 12:33:39.507403 django-insights-0.1.8/project/testapp/users/insights.py
+-rw-r--r--   0        0        0     2812 2023-03-28 13:22:15.312746 django-insights-0.1.8/project/testapp/users/migrations/0001_initial.py
+-rw-r--r--   0        0        0      406 2023-03-27 19:29:06.702145 django-insights-0.1.8/project/testapp/users/migrations/0002_alter_appuser_created.py
+-rw-r--r--   0        0        0        0 2023-03-27 19:26:48.098800 django-insights-0.1.8/project/testapp/users/migrations/__init__.py
+-rw-r--r--   0        0        0      589 2023-03-27 19:29:04.098220 django-insights-0.1.8/project/testapp/users/models.py
+-rw-r--r--   0        0        0      391 2023-04-05 21:09:49.280598 django-insights-0.1.8/project/urls.py
+-rw-r--r--   0        0        0     1858 2023-03-28 20:07:46.011067 django-insights-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3963 2023-02-24 21:17:19.425307 django-insights-0.1.8/requirements/compile.py
+-rw-r--r--   0        0        0    27230 2023-03-08 20:34:30.812867 django-insights-0.1.8/requirements/py310-django32.txt
+-rw-r--r--   0        0        0    27028 2023-03-08 20:34:32.608775 django-insights-0.1.8/requirements/py310-django40.txt
+-rw-r--r--   0        0        0    27027 2023-03-08 20:34:34.407786 django-insights-0.1.8/requirements/py310-django41.txt
+-rw-r--r--   0        0        0    27027 2023-03-08 20:34:36.255245 django-insights-0.1.8/requirements/py310-django42.txt
+-rw-r--r--   0        0        0    26618 2023-03-08 20:34:39.816942 django-insights-0.1.8/requirements/py311-django41.txt
+-rw-r--r--   0        0        0    26618 2023-03-08 20:34:41.452206 django-insights-0.1.8/requirements/py311-django42.txt
+-rw-r--r--   0        0        0    27661 2023-03-08 20:34:11.169086 django-insights-0.1.8/requirements/py38-django32.txt
+-rw-r--r--   0        0        0    28862 2023-03-08 20:34:13.341844 django-insights-0.1.8/requirements/py38-django40.txt
+-rw-r--r--   0        0        0    28861 2023-03-08 20:34:15.479204 django-insights-0.1.8/requirements/py38-django41.txt
+-rw-r--r--   0        0        0    28861 2023-03-08 20:34:17.666389 django-insights-0.1.8/requirements/py38-django42.txt
+-rw-r--r--   0        0        0    27661 2023-03-08 20:34:22.041756 django-insights-0.1.8/requirements/py39-django32.txt
+-rw-r--r--   0        0        0    27459 2023-03-08 20:34:24.070919 django-insights-0.1.8/requirements/py39-django40.txt
+-rw-r--r--   0        0        0    27458 2023-03-08 20:34:26.018066 django-insights-0.1.8/requirements/py39-django41.txt
+-rw-r--r--   0        0        0    27458 2023-03-08 20:34:28.097400 django-insights-0.1.8/requirements/py39-django42.txt
+-rw-r--r--   0        0        0       49 2023-03-08 20:32:58.867282 django-insights-0.1.8/requirements/requirements.in
+-rw-r--r--   0        0        0        0 2023-02-23 22:29:47.164960 django-insights-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0     1337 2023-03-28 13:31:30.803421 django-insights-0.1.8/tests/test_api.py
+-rw-r--r--   0        0        0      232 2023-02-26 20:39:42.248922 django-insights-0.1.8/tests/utils.py
+-rw-r--r--   0        0        0      365 2023-02-24 21:17:25.741397 django-insights-0.1.8/tox.ini
+-rw-r--r--   0        0        0     9467 1970-01-01 00:00:00.000000 django-insights-0.1.8/PKG-INFO
```

### Comparing `django-insights-0.1.7/.github/workflows/main.yml` & `django-insights-0.1.8/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/.gitignore` & `django-insights-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/LICENSE` & `django-insights-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/Makefile` & `django-insights-0.1.8/Makefile`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/README.md` & `django-insights-0.1.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 ## Features
 
 Create insights for your app, store them in a SQLite database for further processing, these insights are written right next to your application logic.
 
 ### Note:
 
-Still working on some small things, extending tests and improve docs.
+Still working on some small things, extending tests and improving the documentation.
+
 For now focus is on:
 
 - Django 3.2 (LTS), 4.0,4.1 and 4.2;
 - Python ≥ 3.8
 
 ## Installation
 
@@ -107,15 +108,15 @@
         include('django_insights.urls', namespace='insights'),
     ),
 ]
 ```
 
 !["Dashboard - App"](https://raw.githubusercontent.com/terminalkitten/django-insights/main/docs/assets/images/screen_2.png)
 
-Now you can visit https://localhost:8000/insights to inspect your Django Insights database
+Now you can visit https://localhost:8000/insights to inspect your Django Insights database.
 
 ## Metrics
 
 Django insights contains 5 types of metrics it can collect:
 
 - `@metrics.counter`
 - `@metrics.gauge`
@@ -260,15 +261,15 @@
 INSIGHTS_CHART_LIGHT_PRIMARY_COLOR = "#2563EB"
 INSIGHTS_CHART_DARK_PRIMARY_COLOR = "#BFDBFE"
 
 ```
 
 ## Use-cases
 
-Insights are gathered from your current application state, Django Insights is not intentend to be used as a realtime, incremementing datasource. You should be able to re-gather these insights from your actual data at any moment in time.
+Insights are gathered from your current application state, Django Insights is not intentend to be used as a realtime, incremementing data-source. You should be able to re-gather these insights from your actual data at any moment in time.
 
 Yes:
 
 - How many users, how many users invited a year
 - How many reports a day, how many messages send on Wednesday's
 
 No:
```

### Comparing `django-insights-0.1.7/django_insights/charts.py` & `django-insights-0.1.8/django_insights/charts.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/django_insights/database.py` & `django-insights-0.1.8/django_insights/database.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/django_insights/managers.py` & `django-insights-0.1.8/django_insights/managers.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/django_insights/metrics.py` & `django-insights-0.1.8/django_insights/metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,23 +15,26 @@
     TimeSeriesType,
 )
 from django_insights.models import App, Bucket, BucketValue, Counter, Gauge
 from django_insights.registry import registry
 
 
 class InsightMetrics:
-    """Auto-generate metrics from mulitple apps at once"""
+    """Auto-generate metrics from multiple apps at once"""
 
-    create_counters: list[Counter] = []
-    create_gauges: list[Gauge] = []
-    create_bucket_values: list[BucketValue] = []
+    create_counters: list[Counter]
+    create_gauges: list[Gauge]
+    create_bucket_values: list[BucketValue]
 
     apps: dict[str, App] = {}
 
     def __init__(self, reset=True) -> None:
+        self.create_counters = []
+        self.create_gauges = []
+        self.create_bucket_values = []
         self.delete_metrics() if reset else None
 
     def delete_metrics(self) -> None:
         """Reset current dataset if metrics are generated"""
         Counter.objects.all().delete()
         Gauge.objects.all().delete()
         Bucket.objects.all().delete()
```

### Comparing `django-insights-0.1.7/django_insights/metrics_types.py` & `django-insights-0.1.8/django_insights/metrics_types.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/django_insights/migrations/0001_initial.py` & `django-insights-0.1.8/django_insights/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/django_insights/models.py` & `django-insights-0.1.8/django_insights/models.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/django_insights/packages/tailwind.config.js` & `django-insights-0.1.8/django_insights/packages/tailwind.config.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,42 +1,42 @@
 /** @type {import('tailwindcss').Config} */
 module.exports = {
-    content: ["../templates/**/*.{html,js}", "node_modules/preline/dist/*.js"],
-    darkMode: "class",
+    content: ['../templates/**/*.{html,js}', 'node_modules/preline/dist/*.js'],
+    darkMode: 'class',
     theme: {
         fontFamily: {
-            sans: ["Ubuntu", "sans-serif"],
+            sans: ['Ubuntu', 'sans-serif'],
         },
         extend: {
             colors: {
-                background: "#f0f3f6",
-                foreground: "#0d1117",
+                background: '#f0f3f6',
+                foreground: '#0d1117',
                 gray: {
-                    50: "#f6f8fa",
-                    100: "#eaeef2",
-                    200: "#d0d7de",
-                    300: "#afb8c1",
-                    400: "#8c959f",
-                    500: "#6e7781",
-                    600: "#57606a",
-                    700: "#424a53",
-                    800: "#32383f",
-                    900: "#24292f",
+                    50: '#f6f8fa',
+                    100: '#eaeef2',
+                    200: '#d0d7de',
+                    300: '#afb8c1',
+                    400: '#8c959f',
+                    500: '#6e7781',
+                    600: '#57606a',
+                    700: '#424a53',
+                    800: '#32383f',
+                    900: '#24292f',
                 },
                 slate: {
-                    50: "#f6f8fa",
-                    100: "#eaeef2",
-                    200: "#d0d7de",
-                    300: "#afb8c1",
-                    400: "#8c959f",
-                    500: "#6e7781",
-                    600: "#57606a",
-                    700: "#424a53",
-                    800: "#32383f",
-                    900: "#24292f",
+                    50: '#f6f8fa',
+                    100: '#eaeef2',
+                    200: '#d0d7de',
+                    300: '#afb8c1',
+                    400: '#8c959f',
+                    500: '#6e7781',
+                    600: '#57606a',
+                    700: '#424a53',
+                    800: '#32383f',
+                    900: '#24292f',
                 },
             },
 
             //   neutral: {
             //     50: "#f9fafb",
             //     100: "#f4f4f5",
             //     200: "#e6e6e6",
@@ -60,9 +60,9 @@
             //     700: "#355bb6",
             //     800: "#2746a0",
             //     900: "#1e3a8a",
             //   },
             // },
         },
     },
-    plugins: [require("preline/plugin"), require("nightwind")],
+    plugins: [require('preline/plugin')],
 };
```

### Comparing `django-insights-0.1.7/django_insights/registry.py` & `django-insights-0.1.8/django_insights/registry.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/django_insights/settings.py` & `django-insights-0.1.8/django_insights/settings.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/django_insights/static/insights/fonts/ubuntu.ttf` & `django-insights-0.1.8/django_insights/static/insights/fonts/ubuntu.ttf`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/django_insights/static/insights/js/preline.js` & `django-insights-0.1.8/django_insights/static/insights/js/insights.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -1,2600 +1,2654 @@
-/*! For license information please see preline.js.LICENSE.txt */ ! function(e, t) {
-    if ("object" == typeof exports && "object" == typeof module) module.exports = t();
-    else if ("function" == typeof define && define.amd) define([], t);
-    else {
-        var o = t();
-        for (var n in o)("object" == typeof exports ? exports : e)[n] = o[n]
-    }
-}(self, (function() {
-    return (() => {
-        "use strict";
-        var e = {
-                661: (e, t, o) => {
-                    function n(e) {
-                        return n = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-                            return typeof e
-                        } : function(e) {
-                            return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                        }, n(e)
-                    }
-
-                    function r(e, t) {
-                        for (var o = 0; o < t.length; o++) {
-                            var n = t[o];
-                            n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
-                        }
-                    }
+(() => {
+    var Ce = Object.create;
+    var we = Object.defineProperty;
+    var Te = Object.getOwnPropertyDescriptor;
+    var Re = Object.getOwnPropertyNames;
+    var qe = Object.getPrototypeOf,
+        De = Object.prototype.hasOwnProperty;
+    var He = (F, Q) => () => (Q || F((Q = {
+        exports: {}
+    }).exports, Q), Q.exports);
+    var Be = (F, Q, Y, mt) => {
+        if (Q && typeof Q == "object" || typeof Q == "function")
+            for (let G of Re(Q)) !De.call(F, G) && G !== Y && we(F, G, {
+                get: () => Q[G],
+                enumerable: !(mt = Te(Q, G)) || mt.enumerable
+            });
+        return F
+    };
+    var Ie = (F, Q, Y) => (Y = F != null ? Ce(qe(F)) : {}, Be(Q || !F || !F.__esModule ? we(Y, "default", {
+        value: F,
+        enumerable: !0
+    }) : Y, F));
+    var Oe = He((Ft, ee) => {
+        (function(F, Q) {
+            if (typeof Ft == "object" && typeof ee == "object") ee.exports = Q();
+            else if (typeof define == "function" && define.amd) define([], Q);
+            else {
+                var Y = Q();
+                for (var mt in Y)(typeof Ft == "object" ? Ft : F)[mt] = Y[mt]
+            }
+        })(self, function() {
+            return (() => {
+                "use strict";
+                var F = {
+                        661: (G, it, N) => {
+                            function R(O) {
+                                return R = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(c) {
+                                    return typeof c
+                                } : function(c) {
+                                    return c && typeof Symbol == "function" && c.constructor === Symbol && c !== Symbol.prototype ? "symbol" : typeof c
+                                }, R(O)
+                            }
+
+                            function B(O, c) {
+                                for (var a = 0; a < c.length; a++) {
+                                    var o = c[a];
+                                    o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(O, o.key, o)
+                                }
+                            }
+
+                            function C(O, c) {
+                                return C = Object.setPrototypeOf || function(a, o) {
+                                    return a.__proto__ = o, a
+                                }, C(O, c)
+                            }
+
+                            function $(O, c) {
+                                if (c && (R(c) === "object" || typeof c == "function")) return c;
+                                if (c !== void 0) throw new TypeError("Derived constructors may only return object or undefined");
+                                return function(a) {
+                                    if (a === void 0) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                                    return a
+                                }(O)
+                            }
+
+                            function P(O) {
+                                return P = Object.setPrototypeOf ? Object.getPrototypeOf : function(c) {
+                                    return c.__proto__ || Object.getPrototypeOf(c)
+                                }, P(O)
+                            }
+                            var x = function(O) {
+                                (function(u, t) {
+                                    if (typeof t != "function" && t !== null) throw new TypeError("Super expression must either be null or a function");
+                                    u.prototype = Object.create(t && t.prototype, {
+                                        constructor: {
+                                            value: u,
+                                            writable: !0,
+                                            configurable: !0
+                                        }
+                                    }), Object.defineProperty(u, "prototype", {
+                                        writable: !1
+                                    }), t && C(u, t)
+                                })(h, O);
+                                var c, a, o, y, m = (o = h, y = function() {
+                                    if (typeof Reflect > "u" || !Reflect.construct || Reflect.construct.sham) return !1;
+                                    if (typeof Proxy == "function") return !0;
+                                    try {
+                                        return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
+                                    } catch {
+                                        return !1
+                                    }
+                                }(), function() {
+                                    var u, t = P(o);
+                                    if (y) {
+                                        var e = P(this).constructor;
+                                        u = Reflect.construct(t, arguments, e)
+                                    } else u = t.apply(this, arguments);
+                                    return $(this, u)
+                                });
+
+                                function h() {
+                                    return function(u, t) {
+                                        if (!(u instanceof t)) throw new TypeError("Cannot call a class as a function")
+                                    }(this, h), m.call(this, ".hs-accordion")
+                                }
+                                return c = h, (a = [{
+                                    key: "init",
+                                    value: function() {
+                                        var u = this;
+                                        document.addEventListener("click", function(t) {
+                                            var e = t.target,
+                                                s = e.closest(u.selector),
+                                                d = e.closest(".hs-accordion-toggle"),
+                                                l = e.closest(".hs-accordion-group");
+                                            s && l && d && (u._hideAll(s), u.show(s))
+                                        })
+                                    }
+                                }, {
+                                    key: "show",
+                                    value: function(u) {
+                                        var t = this;
+                                        if (u.classList.contains("active")) return this.hide(u);
+                                        u.classList.add("active");
+                                        var e = u.querySelector(".hs-accordion-content");
+                                        e.style.display = "block", e.style.height = 0, setTimeout(function() {
+                                            e.style.height = "".concat(e.scrollHeight, "px")
+                                        }), this.afterTransition(e, function() {
+                                            u.classList.contains("active") && (e.style.height = "", t._fireEvent("open", u), t._dispatch("open.hs.accordion", u, u))
+                                        })
+                                    }
+                                }, {
+                                    key: "hide",
+                                    value: function(u) {
+                                        var t = this,
+                                            e = u.querySelector(".hs-accordion-content");
+                                        e.style.height = "".concat(e.scrollHeight, "px"), setTimeout(function() {
+                                            e.style.height = 0
+                                        }), this.afterTransition(e, function() {
+                                            u.classList.contains("active") || (e.style.display = "", t._fireEvent("hide", u), t._dispatch("hide.hs.accordion", u, u))
+                                        }), u.classList.remove("active")
+                                    }
+                                }, {
+                                    key: "_hideAll",
+                                    value: function(u) {
+                                        var t = this,
+                                            e = u.closest(".hs-accordion-group");
+                                        e.hasAttribute("data-hs-accordion-always-open") || e.querySelectorAll(this.selector).forEach(function(s) {
+                                            u !== s && t.hide(s)
+                                        })
+                                    }
+                                }]) && B(c.prototype, a), Object.defineProperty(c, "prototype", {
+                                    writable: !1
+                                }), h
+                            }(N(765).Z);
+                            window.HSAccordion = new x, document.addEventListener("load", window.HSAccordion.init())
+                        },
+                        795: (G, it, N) => {
+                            function R(c) {
+                                return R = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(a) {
+                                    return typeof a
+                                } : function(a) {
+                                    return a && typeof Symbol == "function" && a.constructor === Symbol && a !== Symbol.prototype ? "symbol" : typeof a
+                                }, R(c)
+                            }
+
+                            function B(c, a) {
+                                (a == null || a > c.length) && (a = c.length);
+                                for (var o = 0, y = new Array(a); o < a; o++) y[o] = c[o];
+                                return y
+                            }
+
+                            function C(c, a) {
+                                for (var o = 0; o < a.length; o++) {
+                                    var y = a[o];
+                                    y.enumerable = y.enumerable || !1, y.configurable = !0, "value" in y && (y.writable = !0), Object.defineProperty(c, y.key, y)
+                                }
+                            }
 
-                    function i(e, t) {
-                        return i = Object.setPrototypeOf || function(e, t) {
-                            return e.__proto__ = t, e
-                        }, i(e, t)
-                    }
-
-                    function a(e, t) {
-                        if (t && ("object" === n(t) || "function" == typeof t)) return t;
-                        if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                        return function(e) {
-                            if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-                            return e
-                        }(e)
-                    }
-
-                    function s(e) {
-                        return s = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
-                            return e.__proto__ || Object.getPrototypeOf(e)
-                        }, s(e)
-                    }
-                    var c = function(e) {
-                        ! function(e, t) {
-                            if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
-                            e.prototype = Object.create(t && t.prototype, {
-                                constructor: {
-                                    value: e,
-                                    writable: !0,
-                                    configurable: !0
-                                }
-                            }), Object.defineProperty(e, "prototype", {
-                                writable: !1
-                            }), t && i(e, t)
-                        }(u, e);
-                        var t, o, n, c, l = (n = u, c = function() {
-                            if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
-                            if (Reflect.construct.sham) return !1;
-                            if ("function" == typeof Proxy) return !0;
-                            try {
-                                return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
-                            } catch (e) {
-                                return !1
+                            function $(c, a) {
+                                return $ = Object.setPrototypeOf || function(o, y) {
+                                    return o.__proto__ = y, o
+                                }, $(c, a)
+                            }
+
+                            function P(c, a) {
+                                if (a && (R(a) === "object" || typeof a == "function")) return a;
+                                if (a !== void 0) throw new TypeError("Derived constructors may only return object or undefined");
+                                return function(o) {
+                                    if (o === void 0) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                                    return o
+                                }(c)
+                            }
+
+                            function x(c) {
+                                return x = Object.setPrototypeOf ? Object.getPrototypeOf : function(a) {
+                                    return a.__proto__ || Object.getPrototypeOf(a)
+                                }, x(c)
+                            }
+                            var O = function(c) {
+                                (function(t, e) {
+                                    if (typeof e != "function" && e !== null) throw new TypeError("Super expression must either be null or a function");
+                                    t.prototype = Object.create(e && e.prototype, {
+                                        constructor: {
+                                            value: t,
+                                            writable: !0,
+                                            configurable: !0
+                                        }
+                                    }), Object.defineProperty(t, "prototype", {
+                                        writable: !1
+                                    }), e && $(t, e)
+                                })(u, c);
+                                var a, o, y, m, h = (y = u, m = function() {
+                                    if (typeof Reflect > "u" || !Reflect.construct || Reflect.construct.sham) return !1;
+                                    if (typeof Proxy == "function") return !0;
+                                    try {
+                                        return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
+                                    } catch {
+                                        return !1
+                                    }
+                                }(), function() {
+                                    var t, e = x(y);
+                                    if (m) {
+                                        var s = x(this).constructor;
+                                        t = Reflect.construct(e, arguments, s)
+                                    } else t = e.apply(this, arguments);
+                                    return P(this, t)
+                                });
+
+                                function u() {
+                                    return function(t, e) {
+                                        if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
+                                    }(this, u), h.call(this, "[data-hs-collapse]")
+                                }
+                                return a = u, (o = [{
+                                    key: "init",
+                                    value: function() {
+                                        var t = this;
+                                        document.addEventListener("click", function(e) {
+                                            var s = e.target.closest(t.selector);
+                                            if (s) {
+                                                var d = document.querySelectorAll(s.getAttribute("data-hs-collapse"));
+                                                t.toggle(d)
+                                            }
+                                        })
+                                    }
+                                }, {
+                                    key: "toggle",
+                                    value: function(t) {
+                                        var e, s = this;
+                                        t.length && (e = t, function(d) {
+                                            if (Array.isArray(d)) return B(d)
+                                        }(e) || function(d) {
+                                            if (typeof Symbol < "u" && d[Symbol.iterator] != null || d["@@iterator"] != null) return Array.from(d)
+                                        }(e) || function(d, l) {
+                                            if (d) {
+                                                if (typeof d == "string") return B(d, l);
+                                                var p = Object.prototype.toString.call(d).slice(8, -1);
+                                                return p === "Object" && d.constructor && (p = d.constructor.name), p === "Map" || p === "Set" ? Array.from(d) : p === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(p) ? B(d, l) : void 0
+                                            }
+                                        }(e) || function() {
+                                            throw new TypeError(`Invalid attempt to spread non-iterable instance.
+In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
+                                        }()).forEach(function(d) {
+                                            d.classList.contains("hidden") ? s.show(d) : s.hide(d)
+                                        })
+                                    }
+                                }, {
+                                    key: "show",
+                                    value: function(t) {
+                                        var e = this;
+                                        t.classList.add("open"), t.classList.remove("hidden"), t.style.height = 0, document.querySelectorAll(this.selector).forEach(function(s) {
+                                            t.closest(s.getAttribute("data-hs-collapse")) && s.classList.add("open")
+                                        }), t.style.height = "".concat(t.scrollHeight, "px"), this.afterTransition(t, function() {
+                                            t.classList.contains("open") && (t.style.height = "", e._fireEvent("open", t), e._dispatch("open.hs.collapse", t, t))
+                                        })
+                                    }
+                                }, {
+                                    key: "hide",
+                                    value: function(t) {
+                                        var e = this;
+                                        t.style.height = "".concat(t.scrollHeight, "px"), setTimeout(function() {
+                                            t.style.height = 0
+                                        }), t.classList.remove("open"), this.afterTransition(t, function() {
+                                            t.classList.contains("open") || (t.classList.add("hidden"), t.style.height = null, e._fireEvent("hide", t), e._dispatch("hide.hs.collapse", t, t), t.querySelectorAll(".hs-mega-menu-content.block").forEach(function(s) {
+                                                s.classList.remove("block"), s.classList.add("hidden")
+                                            }))
+                                        }), document.querySelectorAll(this.selector).forEach(function(s) {
+                                            t.closest(s.getAttribute("data-hs-collapse")) && s.classList.remove("open")
+                                        })
+                                    }
+                                }]) && C(a.prototype, o), Object.defineProperty(a, "prototype", {
+                                    writable: !1
+                                }), u
+                            }(N(765).Z);
+                            window.HSCollapse = new O, document.addEventListener("load", window.HSCollapse.init())
+                        },
+                        682: (G, it, N) => {
+                            var R = N(714),
+                                B = N(765);
+                            let C = {
+                                historyIndex: -1,
+                                addHistory: function(m) {
+                                    this.historyIndex = m
+                                },
+                                existsInHistory: function(m) {
+                                    return m > this.historyIndex
+                                },
+                                clearHistory: function() {
+                                    this.historyIndex = -1
+                                }
+                            };
+
+                            function $(m) {
+                                return $ = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(h) {
+                                    return typeof h
+                                } : function(h) {
+                                    return h && typeof Symbol == "function" && h.constructor === Symbol && h !== Symbol.prototype ? "symbol" : typeof h
+                                }, $(m)
+                            }
+
+                            function P(m) {
+                                return function(h) {
+                                    if (Array.isArray(h)) return x(h)
+                                }(m) || function(h) {
+                                    if (typeof Symbol < "u" && h[Symbol.iterator] != null || h["@@iterator"] != null) return Array.from(h)
+                                }(m) || function(h, u) {
+                                    if (h) {
+                                        if (typeof h == "string") return x(h, u);
+                                        var t = Object.prototype.toString.call(h).slice(8, -1);
+                                        return t === "Object" && h.constructor && (t = h.constructor.name), t === "Map" || t === "Set" ? Array.from(h) : t === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(t) ? x(h, u) : void 0
+                                    }
+                                }(m) || function() {
+                                    throw new TypeError(`Invalid attempt to spread non-iterable instance.
+In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
+                                }()
                             }
-                        }(), function() {
-                            var e, t = s(n);
-                            if (c) {
-                                var o = s(this).constructor;
-                                e = Reflect.construct(t, arguments, o)
-                            } else e = t.apply(this, arguments);
-                            return a(this, e)
-                        });
-
-                        function u() {
-                            return function(e, t) {
-                                if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                            }(this, u), l.call(this, ".hs-accordion")
-                        }
-                        return t = u, (o = [{
-                            key: "init",
-                            value: function() {
-                                var e = this;
-                                document.addEventListener("click", (function(t) {
-                                    var o = t.target,
-                                        n = o.closest(e.selector),
-                                        r = o.closest(".hs-accordion-toggle"),
-                                        i = o.closest(".hs-accordion-group");
-                                    n && i && r && (e._hideAll(n), e.show(n))
-                                }))
-                            }
-                        }, {
-                            key: "show",
-                            value: function(e) {
-                                var t = this;
-                                if (e.classList.contains("active")) return this.hide(e);
-                                e.classList.add("active");
-                                var o = e.querySelector(".hs-accordion-content");
-                                o.style.display = "block", o.style.height = 0, setTimeout((function() {
-                                    o.style.height = "".concat(o.scrollHeight, "px")
-                                })), this.afterTransition(o, (function() {
-                                    e.classList.contains("active") && (o.style.height = "", t._fireEvent("open", e), t._dispatch("open.hs.accordion", e, e))
-                                }))
-                            }
-                        }, {
-                            key: "hide",
-                            value: function(e) {
-                                var t = this,
-                                    o = e.querySelector(".hs-accordion-content");
-                                o.style.height = "".concat(o.scrollHeight, "px"), setTimeout((function() {
-                                    o.style.height = 0
-                                })), this.afterTransition(o, (function() {
-                                    e.classList.contains("active") || (o.style.display = "", t._fireEvent("hide", e), t._dispatch("hide.hs.accordion", e, e))
-                                })), e.classList.remove("active")
-                            }
-                        }, {
-                            key: "_hideAll",
-                            value: function(e) {
-                                var t = this,
-                                    o = e.closest(".hs-accordion-group");
-                                o.hasAttribute("data-hs-accordion-always-open") || o.querySelectorAll(this.selector).forEach((function(o) {
-                                    e !== o && t.hide(o)
-                                }))
-                            }
-                        }]) && r(t.prototype, o), Object.defineProperty(t, "prototype", {
-                            writable: !1
-                        }), u
-                    }(o(765).Z);
-                    window.HSAccordion = new c, document.addEventListener("load", window.HSAccordion.init())
-                },
-                795: (e, t, o) => {
-                    function n(e) {
-                        return n = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-                            return typeof e
-                        } : function(e) {
-                            return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                        }, n(e)
-                    }
-
-                    function r(e, t) {
-                        (null == t || t > e.length) && (t = e.length);
-                        for (var o = 0, n = new Array(t); o < t; o++) n[o] = e[o];
-                        return n
-                    }
-
-                    function i(e, t) {
-                        for (var o = 0; o < t.length; o++) {
-                            var n = t[o];
-                            n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
-                        }
-                    }
 
-                    function a(e, t) {
-                        return a = Object.setPrototypeOf || function(e, t) {
-                            return e.__proto__ = t, e
-                        }, a(e, t)
-                    }
-
-                    function s(e, t) {
-                        if (t && ("object" === n(t) || "function" == typeof t)) return t;
-                        if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                        return function(e) {
-                            if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-                            return e
-                        }(e)
-                    }
-
-                    function c(e) {
-                        return c = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
-                            return e.__proto__ || Object.getPrototypeOf(e)
-                        }, c(e)
-                    }
-                    var l = function(e) {
-                        ! function(e, t) {
-                            if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
-                            e.prototype = Object.create(t && t.prototype, {
-                                constructor: {
-                                    value: e,
-                                    writable: !0,
-                                    configurable: !0
-                                }
-                            }), Object.defineProperty(e, "prototype", {
-                                writable: !1
-                            }), t && a(e, t)
-                        }(f, e);
-                        var t, o, n, l, u = (n = f, l = function() {
-                            if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
-                            if (Reflect.construct.sham) return !1;
-                            if ("function" == typeof Proxy) return !0;
-                            try {
-                                return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
-                            } catch (e) {
-                                return !1
+                            function x(m, h) {
+                                (h == null || h > m.length) && (h = m.length);
+                                for (var u = 0, t = new Array(h); u < h; u++) t[u] = m[u];
+                                return t
                             }
-                        }(), function() {
-                            var e, t = c(n);
-                            if (l) {
-                                var o = c(this).constructor;
-                                e = Reflect.construct(t, arguments, o)
-                            } else e = t.apply(this, arguments);
-                            return s(this, e)
-                        });
-
-                        function f() {
-                            return function(e, t) {
-                                if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                            }(this, f), u.call(this, "[data-hs-collapse]")
-                        }
-                        return t = f, (o = [{
-                            key: "init",
-                            value: function() {
-                                var e = this;
-                                document.addEventListener("click", (function(t) {
-                                    var o = t.target.closest(e.selector);
-                                    if (o) {
-                                        var n = document.querySelectorAll(o.getAttribute("data-hs-collapse"));
-                                        e.toggle(n)
-                                    }
-                                }))
+
+                            function O(m, h) {
+                                for (var u = 0; u < h.length; u++) {
+                                    var t = h[u];
+                                    t.enumerable = t.enumerable || !1, t.configurable = !0, "value" in t && (t.writable = !0), Object.defineProperty(m, t.key, t)
+                                }
                             }
-                        }, {
-                            key: "toggle",
-                            value: function(e) {
-                                var t, o = this;
-                                e.length && (t = e, function(e) {
-                                    if (Array.isArray(e)) return r(e)
-                                }(t) || function(e) {
-                                    if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
-                                }(t) || function(e, t) {
-                                    if (e) {
-                                        if ("string" == typeof e) return r(e, t);
-                                        var o = Object.prototype.toString.call(e).slice(8, -1);
-                                        return "Object" === o && e.constructor && (o = e.constructor.name), "Map" === o || "Set" === o ? Array.from(e) : "Arguments" === o || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(o) ? r(e, t) : void 0
-                                    }
-                                }(t) || function() {
-                                    throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
-                                }()).forEach((function(e) {
-                                    e.classList.contains("hidden") ? o.show(e) : o.hide(e)
-                                }))
-                            }
-                        }, {
-                            key: "show",
-                            value: function(e) {
-                                var t = this;
-                                e.classList.add("open"), e.classList.remove("hidden"), e.style.height = 0, document.querySelectorAll(this.selector).forEach((function(t) {
-                                    e.closest(t.getAttribute("data-hs-collapse")) && t.classList.add("open")
-                                })), e.style.height = "".concat(e.scrollHeight, "px"), this.afterTransition(e, (function() {
-                                    e.classList.contains("open") && (e.style.height = "", t._fireEvent("open", e), t._dispatch("open.hs.collapse", e, e))
-                                }))
-                            }
-                        }, {
-                            key: "hide",
-                            value: function(e) {
-                                var t = this;
-                                e.style.height = "".concat(e.scrollHeight, "px"), setTimeout((function() {
-                                    e.style.height = 0
-                                })), e.classList.remove("open"), this.afterTransition(e, (function() {
-                                    e.classList.contains("open") || (e.classList.add("hidden"), e.style.height = null, t._fireEvent("hide", e), t._dispatch("hide.hs.collapse", e, e), e.querySelectorAll(".hs-mega-menu-content.block").forEach((function(e) {
-                                        e.classList.remove("block"), e.classList.add("hidden")
-                                    })))
-                                })), document.querySelectorAll(this.selector).forEach((function(t) {
-                                    e.closest(t.getAttribute("data-hs-collapse")) && t.classList.remove("open")
-                                }))
-                            }
-                        }]) && i(t.prototype, o), Object.defineProperty(t, "prototype", {
-                            writable: !1
-                        }), f
-                    }(o(765).Z);
-                    window.HSCollapse = new l, document.addEventListener("load", window.HSCollapse.init())
-                },
-                682: (e, t, o) => {
-                    var n = o(714),
-                        r = o(765);
-                    const i = {
-                        historyIndex: -1,
-                        addHistory: function(e) {
-                            this.historyIndex = e
-                        },
-                        existsInHistory: function(e) {
-                            return e > this.historyIndex
-                        },
-                        clearHistory: function() {
-                            this.historyIndex = -1
-                        }
-                    };
 
-                    function a(e) {
-                        return a = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-                            return typeof e
-                        } : function(e) {
-                            return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                        }, a(e)
-                    }
-
-                    function s(e) {
-                        return function(e) {
-                            if (Array.isArray(e)) return c(e)
-                        }(e) || function(e) {
-                            if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
-                        }(e) || function(e, t) {
-                            if (e) {
-                                if ("string" == typeof e) return c(e, t);
-                                var o = Object.prototype.toString.call(e).slice(8, -1);
-                                return "Object" === o && e.constructor && (o = e.constructor.name), "Map" === o || "Set" === o ? Array.from(e) : "Arguments" === o || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(o) ? c(e, t) : void 0
-                            }
-                        }(e) || function() {
-                            throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
-                        }()
-                    }
-
-                    function c(e, t) {
-                        (null == t || t > e.length) && (t = e.length);
-                        for (var o = 0, n = new Array(t); o < t; o++) n[o] = e[o];
-                        return n
-                    }
-
-                    function l(e, t) {
-                        for (var o = 0; o < t.length; o++) {
-                            var n = t[o];
-                            n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
-                        }
-                    }
+                            function c(m, h) {
+                                return c = Object.setPrototypeOf || function(u, t) {
+                                    return u.__proto__ = t, u
+                                }, c(m, h)
+                            }
 
-                    function u(e, t) {
-                        return u = Object.setPrototypeOf || function(e, t) {
-                            return e.__proto__ = t, e
-                        }, u(e, t)
-                    }
-
-                    function f(e, t) {
-                        if (t && ("object" === a(t) || "function" == typeof t)) return t;
-                        if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                        return function(e) {
-                            if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-                            return e
-                        }(e)
-                    }
-
-                    function p(e) {
-                        return p = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
-                            return e.__proto__ || Object.getPrototypeOf(e)
-                        }, p(e)
-                    }
-                    var d = function(e) {
-                        ! function(e, t) {
-                            if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
-                            e.prototype = Object.create(t && t.prototype, {
-                                constructor: {
-                                    value: e,
-                                    writable: !0,
-                                    configurable: !0
-                                }
-                            }), Object.defineProperty(e, "prototype", {
-                                writable: !1
-                            }), t && u(e, t)
-                        }(d, e);
-                        var t, o, r, a, c = (r = d, a = function() {
-                            if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
-                            if (Reflect.construct.sham) return !1;
-                            if ("function" == typeof Proxy) return !0;
-                            try {
-                                return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
-                            } catch (e) {
-                                return !1
+                            function a(m, h) {
+                                if (h && ($(h) === "object" || typeof h == "function")) return h;
+                                if (h !== void 0) throw new TypeError("Derived constructors may only return object or undefined");
+                                return function(u) {
+                                    if (u === void 0) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                                    return u
+                                }(m)
                             }
-                        }(), function() {
-                            var e, t = p(r);
-                            if (a) {
-                                var o = p(this).constructor;
-                                e = Reflect.construct(t, arguments, o)
-                            } else e = t.apply(this, arguments);
-                            return f(this, e)
-                        });
-
-                        function d() {
-                            var e;
-                            return function(e, t) {
-                                if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                            }(this, d), (e = c.call(this, ".hs-dropdown")).positions = {
-                                top: "top",
-                                "top-left": "top-start",
-                                "top-right": "top-end",
-                                bottom: "bottom",
-                                "bottom-left": "bottom-start",
-                                "bottom-right": "bottom-end",
-                                right: "right",
-                                "right-top": "right-start",
-                                "right-bottom": "right-end",
-                                left: "left",
-                                "left-top": "left-start",
-                                "left-bottom": "left-end"
-                            }, e.absoluteStrategyModifiers = function(e) {
-                                return [{
-                                    name: "applyStyles",
-                                    fn: function(t) {
-                                        var o = (window.getComputedStyle(e).getPropertyValue("--strategy") || "absolute").replace(" ", ""),
-                                            n = (window.getComputedStyle(e).getPropertyValue("--adaptive") || "adaptive").replace(" ", "");
-                                        t.state.elements.popper.style.position = o, t.state.elements.popper.style.transform = "adaptive" === n ? t.state.styles.popper.transform : null, t.state.elements.popper.style.top = null, t.state.elements.popper.style.bottom = null, t.state.elements.popper.style.left = null, t.state.elements.popper.style.right = null, t.state.elements.popper.style.margin = 0
-                                    }
-                                }, {
-                                    name: "computeStyles",
-                                    options: {
-                                        adaptive: !1
+
+                            function o(m) {
+                                return o = Object.setPrototypeOf ? Object.getPrototypeOf : function(h) {
+                                    return h.__proto__ || Object.getPrototypeOf(h)
+                                }, o(m)
+                            }
+                            var y = function(m) {
+                                (function(l, p) {
+                                    if (typeof p != "function" && p !== null) throw new TypeError("Super expression must either be null or a function");
+                                    l.prototype = Object.create(p && p.prototype, {
+                                        constructor: {
+                                            value: l,
+                                            writable: !0,
+                                            configurable: !0
+                                        }
+                                    }), Object.defineProperty(l, "prototype", {
+                                        writable: !1
+                                    }), p && c(l, p)
+                                })(d, m);
+                                var h, u, t, e, s = (t = d, e = function() {
+                                    if (typeof Reflect > "u" || !Reflect.construct || Reflect.construct.sham) return !1;
+                                    if (typeof Proxy == "function") return !0;
+                                    try {
+                                        return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
+                                    } catch {
+                                        return !1
                                     }
-                                }]
-                            }, e._history = i, e
-                        }
-                        return t = d, o = [{
-                            key: "init",
-                            value: function() {
-                                var e = this;
-                                document.addEventListener("click", (function(t) {
-                                    var o = t.target,
-                                        n = o.closest(e.selector),
-                                        r = o.closest(".hs-dropdown-menu");
-                                    if (n && n.classList.contains("open") || e._closeOthers(n), r) {
-                                        var i = (window.getComputedStyle(n).getPropertyValue("--auto-close") || "").replace(" ", "");
-                                        if (("false" == i || "inside" == i) && !n.parentElement.closest(e.selector)) return
-                                    }
-                                    n && (n.classList.contains("open") ? e.close(n) : e.open(n))
-                                })), document.addEventListener("mousemove", (function(t) {
-                                    var o = t.target,
-                                        n = o.closest(e.selector);
-                                    if (o.closest(".hs-dropdown-menu"), n) {
-                                        var r = (window.getComputedStyle(n).getPropertyValue("--trigger") || "click").replace(" ", "");
-                                        if ("hover" !== r) return;
-                                        n && n.classList.contains("open") || e._closeOthers(n), "hover" !== r || n.classList.contains("open") || /iPad|iPhone|iPod/.test(navigator.platform) || navigator.maxTouchPoints && navigator.maxTouchPoints > 2 && /MacIntel/.test(navigator.platform) || navigator.maxTouchPoints && navigator.maxTouchPoints > 2 && /MacIntel/.test(navigator.platform) || e._hover(o)
-                                    }
-                                })), document.addEventListener("keydown", this._keyboardSupport.bind(this)), window.addEventListener("resize", (function() {
-                                    document.querySelectorAll(".hs-dropdown.open").forEach((function(t) {
-                                        e.close(t, !0)
-                                    }))
-                                }))
-                            }
-                        }, {
-                            key: "_closeOthers",
-                            value: function() {
-                                var e = this,
-                                    t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null,
-                                    o = document.querySelectorAll("".concat(this.selector, ".open"));
-                                o.forEach((function(o) {
-                                    if (!t || t.closest(".hs-dropdown.open") !== o) {
-                                        var n = (window.getComputedStyle(o).getPropertyValue("--auto-close") || "").replace(" ", "");
-                                        "false" != n && "outside" != n && e.close(o)
-                                    }
-                                }))
-                            }
-                        }, {
-                            key: "_hover",
-                            value: function(e) {
-                                var t = this,
-                                    o = e.closest(this.selector);
-                                this.open(o), document.addEventListener("mousemove", (function e(n) {
-                                    n.target.closest(t.selector) && n.target.closest(t.selector) !== o.parentElement.closest(t.selector) || (t.close(o), document.removeEventListener("mousemove", e, !0))
-                                }), !0)
-                            }
-                        }, {
-                            key: "close",
-                            value: function(e) {
-                                var t = this,
-                                    o = arguments.length > 1 && void 0 !== arguments[1] && arguments[1],
-                                    n = e.querySelector(".hs-dropdown-menu"),
-                                    r = function() {
-                                        e.classList.contains("open") || (n.classList.remove("block"), n.classList.add("hidden"), n.style.inset = null, n.style.position = null, e._popper && e._popper.destroy())
-                                    };
-                                o || this.afterTransition(e.querySelector("[data-hs-dropdown-transition]") || n, (function() {
-                                    r()
-                                })), n.style.margin = null, e.classList.remove("open"), o && r(), this._fireEvent("close", e), this._dispatch("close.hs.dropdown", e, e);
-                                var i = n.querySelectorAll(".hs-dropdown.open");
-                                i.forEach((function(e) {
-                                    t.close(e, !0)
-                                }))
-                            }
-                        }, {
-                            key: "open",
-                            value: function(e) {
-                                var t = e.querySelector(".hs-dropdown-menu"),
-                                    o = (window.getComputedStyle(e).getPropertyValue("--placement") || "").replace(" ", ""),
-                                    r = (window.getComputedStyle(e).getPropertyValue("--strategy") || "fixed").replace(" ", ""),
-                                    i = ((window.getComputedStyle(e).getPropertyValue("--adaptive") || "adaptive").replace(" ", ""), parseInt((window.getComputedStyle(e).getPropertyValue("--offset") || "10").replace(" ", "")));
-                                if ("static" !== r) {
-                                    e._popper && e._popper.destroy();
-                                    var a = (0, n.fi)(e, t, {
-                                        placement: this.positions[o] || "bottom-start",
-                                        strategy: r,
-                                        modifiers: [].concat(s("fixed" !== r ? this.absoluteStrategyModifiers(e) : []), [{
-                                            name: "offset",
+                                }(), function() {
+                                    var l, p = o(t);
+                                    if (e) {
+                                        var v = o(this).constructor;
+                                        l = Reflect.construct(p, arguments, v)
+                                    } else l = p.apply(this, arguments);
+                                    return a(this, l)
+                                });
+
+                                function d() {
+                                    var l;
+                                    return function(p, v) {
+                                        if (!(p instanceof v)) throw new TypeError("Cannot call a class as a function")
+                                    }(this, d), (l = s.call(this, ".hs-dropdown")).positions = {
+                                        top: "top",
+                                        "top-left": "top-start",
+                                        "top-right": "top-end",
+                                        bottom: "bottom",
+                                        "bottom-left": "bottom-start",
+                                        "bottom-right": "bottom-end",
+                                        right: "right",
+                                        "right-top": "right-start",
+                                        "right-bottom": "right-end",
+                                        left: "left",
+                                        "left-top": "left-start",
+                                        "left-bottom": "left-end"
+                                    }, l.absoluteStrategyModifiers = function(p) {
+                                        return [{
+                                            name: "applyStyles",
+                                            fn: function(v) {
+                                                var S = (window.getComputedStyle(p).getPropertyValue("--strategy") || "absolute").replace(" ", ""),
+                                                    E = (window.getComputedStyle(p).getPropertyValue("--adaptive") || "adaptive").replace(" ", "");
+                                                v.state.elements.popper.style.position = S, v.state.elements.popper.style.transform = E === "adaptive" ? v.state.styles.popper.transform : null, v.state.elements.popper.style.top = null, v.state.elements.popper.style.bottom = null, v.state.elements.popper.style.left = null, v.state.elements.popper.style.right = null, v.state.elements.popper.style.margin = 0
+                                            }
+                                        }, {
+                                            name: "computeStyles",
                                             options: {
-                                                offset: [0, i]
+                                                adaptive: !1
                                             }
-                                        }])
-                                    });
-                                    e._popper = a
-                                }
-                                t.style.margin = null, t.classList.add("block"), t.classList.remove("hidden"), setTimeout((function() {
-                                    e.classList.add("open")
-                                })), this._fireEvent("open", e), this._dispatch("open.hs.dropdown", e, e)
-                            }
-                        }, {
-                            key: "_keyboardSupport",
-                            value: function(e) {
-                                var t = document.querySelector(".hs-dropdown.open");
-                                if (t) return 27 === e.keyCode ? (e.preventDefault(), this._esc(t)) : 40 === e.keyCode ? (e.preventDefault(), this._down(t)) : 38 === e.keyCode ? (e.preventDefault(), this._up(t)) : 36 === e.keyCode ? (e.preventDefault(), this._start(t)) : 35 === e.keyCode ? (e.preventDefault(), this._end(t)) : void this._byChar(t, e.key)
-                            }
-                        }, {
-                            key: "_esc",
-                            value: function(e) {
-                                this.close(e)
-                            }
-                        }, {
-                            key: "_up",
-                            value: function(e) {
-                                var t = e.querySelector(".hs-dropdown-menu"),
-                                    o = s(t.querySelectorAll("a")).reverse().filter((function(e) {
-                                        return !e.disabled
-                                    })),
-                                    n = t.querySelector("a:focus"),
-                                    r = o.findIndex((function(e) {
-                                        return e === n
-                                    }));
-                                r + 1 < o.length && r++, o[r].focus()
-                            }
-                        }, {
-                            key: "_down",
-                            value: function(e) {
-                                var t = e.querySelector(".hs-dropdown-menu"),
-                                    o = s(t.querySelectorAll("a")).filter((function(e) {
-                                        return !e.disabled
-                                    })),
-                                    n = t.querySelector("a:focus"),
-                                    r = o.findIndex((function(e) {
-                                        return e === n
-                                    }));
-                                r + 1 < o.length && r++, o[r].focus()
-                            }
-                        }, {
-                            key: "_start",
-                            value: function(e) {
-                                var t = s(e.querySelector(".hs-dropdown-menu").querySelectorAll("a")).filter((function(e) {
-                                    return !e.disabled
-                                }));
-                                t.length && t[0].focus()
-                            }
-                        }, {
-                            key: "_end",
-                            value: function(e) {
-                                var t = s(e.querySelector(".hs-dropdown-menu").querySelectorAll("a")).reverse().filter((function(e) {
-                                    return !e.disabled
-                                }));
-                                t.length && t[0].focus()
-                            }
-                        }, {
-                            key: "_byChar",
-                            value: function(e, t) {
-                                var o = this,
-                                    n = s(e.querySelector(".hs-dropdown-menu").querySelectorAll("a")),
-                                    r = function() {
-                                        return n.findIndex((function(e, n) {
-                                            return e.innerText.toLowerCase().charAt(0) === t.toLowerCase() && o._history.existsInHistory(n)
-                                        }))
-                                    },
-                                    i = r(); - 1 === i && (this._history.clearHistory(), i = r()), -1 !== i && (n[i].focus(), this._history.addHistory(i))
+                                        }]
+                                    }, l._history = C, l
+                                }
+                                return h = d, u = [{
+                                    key: "init",
+                                    value: function() {
+                                        var l = this;
+                                        document.addEventListener("click", function(p) {
+                                            var v = p.target,
+                                                S = v.closest(l.selector),
+                                                E = v.closest(".hs-dropdown-menu");
+                                            if (S && S.classList.contains("open") || l._closeOthers(S), E) {
+                                                var _ = (window.getComputedStyle(S).getPropertyValue("--auto-close") || "").replace(" ", "");
+                                                if ((_ == "false" || _ == "inside") && !S.parentElement.closest(l.selector)) return
+                                            }
+                                            S && (S.classList.contains("open") ? l.close(S) : l.open(S))
+                                        }), document.addEventListener("mousemove", function(p) {
+                                            var v = p.target,
+                                                S = v.closest(l.selector);
+                                            if (v.closest(".hs-dropdown-menu"), S) {
+                                                var E = (window.getComputedStyle(S).getPropertyValue("--trigger") || "click").replace(" ", "");
+                                                if (E !== "hover") return;
+                                                S && S.classList.contains("open") || l._closeOthers(S), E !== "hover" || S.classList.contains("open") || /iPad|iPhone|iPod/.test(navigator.platform) || navigator.maxTouchPoints && navigator.maxTouchPoints > 2 && /MacIntel/.test(navigator.platform) || navigator.maxTouchPoints && navigator.maxTouchPoints > 2 && /MacIntel/.test(navigator.platform) || l._hover(v)
+                                            }
+                                        }), document.addEventListener("keydown", this._keyboardSupport.bind(this)), window.addEventListener("resize", function() {
+                                            document.querySelectorAll(".hs-dropdown.open").forEach(function(p) {
+                                                l.close(p, !0)
+                                            })
+                                        })
+                                    }
+                                }, {
+                                    key: "_closeOthers",
+                                    value: function() {
+                                        var l = this,
+                                            p = arguments.length > 0 && arguments[0] !== void 0 ? arguments[0] : null,
+                                            v = document.querySelectorAll("".concat(this.selector, ".open"));
+                                        v.forEach(function(S) {
+                                            if (!p || p.closest(".hs-dropdown.open") !== S) {
+                                                var E = (window.getComputedStyle(S).getPropertyValue("--auto-close") || "").replace(" ", "");
+                                                E != "false" && E != "outside" && l.close(S)
+                                            }
+                                        })
+                                    }
+                                }, {
+                                    key: "_hover",
+                                    value: function(l) {
+                                        var p = this,
+                                            v = l.closest(this.selector);
+                                        this.open(v), document.addEventListener("mousemove", function S(E) {
+                                            E.target.closest(p.selector) && E.target.closest(p.selector) !== v.parentElement.closest(p.selector) || (p.close(v), document.removeEventListener("mousemove", S, !0))
+                                        }, !0)
+                                    }
+                                }, {
+                                    key: "close",
+                                    value: function(l) {
+                                        var p = this,
+                                            v = arguments.length > 1 && arguments[1] !== void 0 && arguments[1],
+                                            S = l.querySelector(".hs-dropdown-menu"),
+                                            E = function() {
+                                                l.classList.contains("open") || (S.classList.remove("block"), S.classList.add("hidden"), S.style.inset = null, S.style.position = null, l._popper && l._popper.destroy())
+                                            };
+                                        v || this.afterTransition(l.querySelector("[data-hs-dropdown-transition]") || S, function() {
+                                            E()
+                                        }), S.style.margin = null, l.classList.remove("open"), v && E(), this._fireEvent("close", l), this._dispatch("close.hs.dropdown", l, l);
+                                        var _ = S.querySelectorAll(".hs-dropdown.open");
+                                        _.forEach(function(et) {
+                                            p.close(et, !0)
+                                        })
+                                    }
+                                }, {
+                                    key: "open",
+                                    value: function(l) {
+                                        var p = l.querySelector(".hs-dropdown-menu"),
+                                            v = (window.getComputedStyle(l).getPropertyValue("--placement") || "").replace(" ", ""),
+                                            S = (window.getComputedStyle(l).getPropertyValue("--strategy") || "fixed").replace(" ", ""),
+                                            E = ((window.getComputedStyle(l).getPropertyValue("--adaptive") || "adaptive").replace(" ", ""), parseInt((window.getComputedStyle(l).getPropertyValue("--offset") || "10").replace(" ", "")));
+                                        if (S !== "static") {
+                                            l._popper && l._popper.destroy();
+                                            var _ = (0, R.fi)(l, p, {
+                                                placement: this.positions[v] || "bottom-start",
+                                                strategy: S,
+                                                modifiers: [].concat(P(S !== "fixed" ? this.absoluteStrategyModifiers(l) : []), [{
+                                                    name: "offset",
+                                                    options: {
+                                                        offset: [0, E]
+                                                    }
+                                                }])
+                                            });
+                                            l._popper = _
+                                        }
+                                        p.style.margin = null, p.classList.add("block"), p.classList.remove("hidden"), setTimeout(function() {
+                                            l.classList.add("open")
+                                        }), this._fireEvent("open", l), this._dispatch("open.hs.dropdown", l, l)
+                                    }
+                                }, {
+                                    key: "_keyboardSupport",
+                                    value: function(l) {
+                                        var p = document.querySelector(".hs-dropdown.open");
+                                        if (p) return l.keyCode === 27 ? (l.preventDefault(), this._esc(p)) : l.keyCode === 40 ? (l.preventDefault(), this._down(p)) : l.keyCode === 38 ? (l.preventDefault(), this._up(p)) : l.keyCode === 36 ? (l.preventDefault(), this._start(p)) : l.keyCode === 35 ? (l.preventDefault(), this._end(p)) : void this._byChar(p, l.key)
+                                    }
+                                }, {
+                                    key: "_esc",
+                                    value: function(l) {
+                                        this.close(l)
+                                    }
+                                }, {
+                                    key: "_up",
+                                    value: function(l) {
+                                        var p = l.querySelector(".hs-dropdown-menu"),
+                                            v = P(p.querySelectorAll("a")).reverse().filter(function(_) {
+                                                return !_.disabled
+                                            }),
+                                            S = p.querySelector("a:focus"),
+                                            E = v.findIndex(function(_) {
+                                                return _ === S
+                                            });
+                                        E + 1 < v.length && E++, v[E].focus()
+                                    }
+                                }, {
+                                    key: "_down",
+                                    value: function(l) {
+                                        var p = l.querySelector(".hs-dropdown-menu"),
+                                            v = P(p.querySelectorAll("a")).filter(function(_) {
+                                                return !_.disabled
+                                            }),
+                                            S = p.querySelector("a:focus"),
+                                            E = v.findIndex(function(_) {
+                                                return _ === S
+                                            });
+                                        E + 1 < v.length && E++, v[E].focus()
+                                    }
+                                }, {
+                                    key: "_start",
+                                    value: function(l) {
+                                        var p = P(l.querySelector(".hs-dropdown-menu").querySelectorAll("a")).filter(function(v) {
+                                            return !v.disabled
+                                        });
+                                        p.length && p[0].focus()
+                                    }
+                                }, {
+                                    key: "_end",
+                                    value: function(l) {
+                                        var p = P(l.querySelector(".hs-dropdown-menu").querySelectorAll("a")).reverse().filter(function(v) {
+                                            return !v.disabled
+                                        });
+                                        p.length && p[0].focus()
+                                    }
+                                }, {
+                                    key: "_byChar",
+                                    value: function(l, p) {
+                                        var v = this,
+                                            S = P(l.querySelector(".hs-dropdown-menu").querySelectorAll("a")),
+                                            E = function() {
+                                                return S.findIndex(function(et, U) {
+                                                    return et.innerText.toLowerCase().charAt(0) === p.toLowerCase() && v._history.existsInHistory(U)
+                                                })
+                                            },
+                                            _ = E();
+                                        _ === -1 && (this._history.clearHistory(), _ = E()), _ !== -1 && (S[_].focus(), this._history.addHistory(_))
+                                    }
+                                }, {
+                                    key: "toggle",
+                                    value: function(l) {
+                                        l.classList.contains("open") ? this.close(l) : this.open(l)
+                                    }
+                                }], u && O(h.prototype, u), Object.defineProperty(h, "prototype", {
+                                    writable: !1
+                                }), d
+                            }(B.Z);
+                            window.HSDropdown = new y, document.addEventListener("load", window.HSDropdown.init())
+                        },
+                        284: (G, it, N) => {
+                            function R(c) {
+                                return R = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(a) {
+                                    return typeof a
+                                } : function(a) {
+                                    return a && typeof Symbol == "function" && a.constructor === Symbol && a !== Symbol.prototype ? "symbol" : typeof a
+                                }, R(c)
+                            }
+
+                            function B(c, a) {
+                                (a == null || a > c.length) && (a = c.length);
+                                for (var o = 0, y = new Array(a); o < a; o++) y[o] = c[o];
+                                return y
+                            }
+
+                            function C(c, a) {
+                                for (var o = 0; o < a.length; o++) {
+                                    var y = a[o];
+                                    y.enumerable = y.enumerable || !1, y.configurable = !0, "value" in y && (y.writable = !0), Object.defineProperty(c, y.key, y)
+                                }
                             }
-                        }, {
-                            key: "toggle",
-                            value: function(e) {
-                                e.classList.contains("open") ? this.close(e) : this.open(e)
-                            }
-                        }], o && l(t.prototype, o), Object.defineProperty(t, "prototype", {
-                            writable: !1
-                        }), d
-                    }(r.Z);
-                    window.HSDropdown = new d, document.addEventListener("load", window.HSDropdown.init())
-                },
-                284: (e, t, o) => {
-                    function n(e) {
-                        return n = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-                            return typeof e
-                        } : function(e) {
-                            return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                        }, n(e)
-                    }
-
-                    function r(e, t) {
-                        (null == t || t > e.length) && (t = e.length);
-                        for (var o = 0, n = new Array(t); o < t; o++) n[o] = e[o];
-                        return n
-                    }
-
-                    function i(e, t) {
-                        for (var o = 0; o < t.length; o++) {
-                            var n = t[o];
-                            n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
-                        }
-                    }
 
-                    function a(e, t) {
-                        return a = Object.setPrototypeOf || function(e, t) {
-                            return e.__proto__ = t, e
-                        }, a(e, t)
-                    }
-
-                    function s(e, t) {
-                        if (t && ("object" === n(t) || "function" == typeof t)) return t;
-                        if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                        return function(e) {
-                            if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-                            return e
-                        }(e)
-                    }
-
-                    function c(e) {
-                        return c = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
-                            return e.__proto__ || Object.getPrototypeOf(e)
-                        }, c(e)
-                    }
-                    var l = function(e) {
-                        ! function(e, t) {
-                            if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
-                            e.prototype = Object.create(t && t.prototype, {
-                                constructor: {
-                                    value: e,
-                                    writable: !0,
-                                    configurable: !0
-                                }
-                            }), Object.defineProperty(e, "prototype", {
-                                writable: !1
-                            }), t && a(e, t)
-                        }(f, e);
-                        var t, o, n, l, u = (n = f, l = function() {
-                            if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
-                            if (Reflect.construct.sham) return !1;
-                            if ("function" == typeof Proxy) return !0;
-                            try {
-                                return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
-                            } catch (e) {
-                                return !1
-                            }
-                        }(), function() {
-                            var e, t = c(n);
-                            if (l) {
-                                var o = c(this).constructor;
-                                e = Reflect.construct(t, arguments, o)
-                            } else e = t.apply(this, arguments);
-                            return s(this, e)
-                        });
-
-                        function f() {
-                            var e;
-                            return function(e, t) {
-                                if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                            }(this, f), (e = u.call(this, "[data-hs-overlay]")).openNextOverlay = !1, e
-                        }
-                        return t = f, (o = [{
-                            key: "init",
-                            value: function() {
-                                var e = this;
-                                document.addEventListener("click", (function(t) {
-                                    var o = t.target.closest(e.selector),
-                                        n = t.target.closest("[data-hs-overlay-close]"),
-                                        r = "true" === t.target.getAttribute("aria-overlay");
-                                    return n ? e.close(n.closest(".hs-overlay.open")) : o ? e.toggle(document.querySelector(o.getAttribute("data-hs-overlay"))) : void(r && e._onBackdropClick(t.target))
-                                })), document.addEventListener("keydown", (function(t) {
-                                    if (27 === t.keyCode) {
-                                        var o = document.querySelector(".hs-overlay.open");
-                                        if (!o) return;
-                                        setTimeout((function() {
-                                            "false" !== o.getAttribute("data-hs-overlay-keyboard") && e.close(o)
-                                        }))
+                            function $(c, a) {
+                                return $ = Object.setPrototypeOf || function(o, y) {
+                                    return o.__proto__ = y, o
+                                }, $(c, a)
+                            }
+
+                            function P(c, a) {
+                                if (a && (R(a) === "object" || typeof a == "function")) return a;
+                                if (a !== void 0) throw new TypeError("Derived constructors may only return object or undefined");
+                                return function(o) {
+                                    if (o === void 0) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                                    return o
+                                }(c)
+                            }
+
+                            function x(c) {
+                                return x = Object.setPrototypeOf ? Object.getPrototypeOf : function(a) {
+                                    return a.__proto__ || Object.getPrototypeOf(a)
+                                }, x(c)
+                            }
+                            var O = function(c) {
+                                (function(t, e) {
+                                    if (typeof e != "function" && e !== null) throw new TypeError("Super expression must either be null or a function");
+                                    t.prototype = Object.create(e && e.prototype, {
+                                        constructor: {
+                                            value: t,
+                                            writable: !0,
+                                            configurable: !0
+                                        }
+                                    }), Object.defineProperty(t, "prototype", {
+                                        writable: !1
+                                    }), e && $(t, e)
+                                })(u, c);
+                                var a, o, y, m, h = (y = u, m = function() {
+                                    if (typeof Reflect > "u" || !Reflect.construct || Reflect.construct.sham) return !1;
+                                    if (typeof Proxy == "function") return !0;
+                                    try {
+                                        return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
+                                    } catch {
+                                        return !1
                                     }
-                                }))
-                            }
-                        }, {
-                            key: "toggle",
-                            value: function(e) {
-                                e && (e.classList.contains("hidden") ? this.open(e) : this.close(e))
-                            }
-                        }, {
-                            key: "open",
-                            value: function(e) {
-                                var t = this;
-                                if (e) {
-                                    var o = document.querySelector(".hs-overlay.open"),
-                                        n = "true" !== this.getClassProperty(e, "--body-scroll", "false");
-                                    if (o) return this.openNextOverlay = !0, this.close(o).then((function() {
-                                        t.open(e), t.openNextOverlay = !1
-                                    }));
-                                    n && (document.body.style.overflow = "hidden"), this._buildBackdrop(e), this._checkTimer(e), this._autoHide(e), e.classList.remove("hidden"), e.setAttribute("aria-overlay", "true"), e.setAttribute("tabindex", "-1"), setTimeout((function() {
-                                        e.classList.contains("hidden") || (e.classList.add("open"), t._fireEvent("open", e), t._dispatch("open.hs.overlay", e, e), t._focusInput(e))
-                                    }), 50)
-                                }
-                            }
-                        }, {
-                            key: "close",
-                            value: function(e) {
-                                var t = this;
-                                return new Promise((function(o) {
-                                    e && (e.classList.remove("open"), e.removeAttribute("aria-overlay"), e.removeAttribute("tabindex", "-1"), t.afterTransition(e, (function() {
-                                        e.classList.contains("open") || (e.classList.add("hidden"), t._destroyBackdrop(), t._fireEvent("close", e), t._dispatch("close.hs.overlay", e, e), document.body.style.overflow = "", o(e))
-                                    })))
-                                }))
-                            }
-                        }, {
-                            key: "_autoHide",
-                            value: function(e) {
-                                var t = this,
-                                    o = parseInt(this.getClassProperty(e, "--auto-hide", "0"));
-                                o && (e.autoHide = setTimeout((function() {
-                                    t.close(e)
-                                }), o))
-                            }
-                        }, {
-                            key: "_checkTimer",
-                            value: function(e) {
-                                e.autoHide && (clearTimeout(e.autoHide), delete e.autoHide)
-                            }
-                        }, {
-                            key: "_onBackdropClick",
-                            value: function(e) {
-                                "static" !== this.getClassProperty(e, "--overlay-backdrop", "true") && this.close(e)
-                            }
-                        }, {
-                            key: "_buildBackdrop",
-                            value: function(e) {
-                                var t, o = this,
-                                    n = e.getAttribute("data-hs-overlay-backdrop-container") || !1,
-                                    i = document.createElement("div"),
-                                    a = "transition duration fixed inset-0 z-50 bg-gray-900 bg-opacity-50 dark:bg-opacity-80 hs-overlay-backdrop",
-                                    s = function(e, t) {
-                                        var o = "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
-                                        if (!o) {
-                                            if (Array.isArray(e) || (o = function(e, t) {
-                                                    if (e) {
-                                                        if ("string" == typeof e) return r(e, t);
-                                                        var o = Object.prototype.toString.call(e).slice(8, -1);
-                                                        return "Object" === o && e.constructor && (o = e.constructor.name), "Map" === o || "Set" === o ? Array.from(e) : "Arguments" === o || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(o) ? r(e, t) : void 0
+                                }(), function() {
+                                    var t, e = x(y);
+                                    if (m) {
+                                        var s = x(this).constructor;
+                                        t = Reflect.construct(e, arguments, s)
+                                    } else t = e.apply(this, arguments);
+                                    return P(this, t)
+                                });
+
+                                function u() {
+                                    var t;
+                                    return function(e, s) {
+                                        if (!(e instanceof s)) throw new TypeError("Cannot call a class as a function")
+                                    }(this, u), (t = h.call(this, "[data-hs-overlay]")).openNextOverlay = !1, t
+                                }
+                                return a = u, (o = [{
+                                    key: "init",
+                                    value: function() {
+                                        var t = this;
+                                        document.addEventListener("click", function(e) {
+                                            var s = e.target.closest(t.selector),
+                                                d = e.target.closest("[data-hs-overlay-close]"),
+                                                l = e.target.getAttribute("aria-overlay") === "true";
+                                            return d ? t.close(d.closest(".hs-overlay.open")) : s ? t.toggle(document.querySelector(s.getAttribute("data-hs-overlay"))) : void(l && t._onBackdropClick(e.target))
+                                        }), document.addEventListener("keydown", function(e) {
+                                            if (e.keyCode === 27) {
+                                                var s = document.querySelector(".hs-overlay.open");
+                                                if (!s) return;
+                                                setTimeout(function() {
+                                                    s.getAttribute("data-hs-overlay-keyboard") !== "false" && t.close(s)
+                                                })
+                                            }
+                                        })
+                                    }
+                                }, {
+                                    key: "toggle",
+                                    value: function(t) {
+                                        t && (t.classList.contains("hidden") ? this.open(t) : this.close(t))
+                                    }
+                                }, {
+                                    key: "open",
+                                    value: function(t) {
+                                        var e = this;
+                                        if (t) {
+                                            var s = document.querySelector(".hs-overlay.open"),
+                                                d = this.getClassProperty(t, "--body-scroll", "false") !== "true";
+                                            if (s) return this.openNextOverlay = !0, this.close(s).then(function() {
+                                                e.open(t), e.openNextOverlay = !1
+                                            });
+                                            d && (document.body.style.overflow = "hidden"), this._buildBackdrop(t), this._checkTimer(t), this._autoHide(t), t.classList.remove("hidden"), t.setAttribute("aria-overlay", "true"), t.setAttribute("tabindex", "-1"), setTimeout(function() {
+                                                t.classList.contains("hidden") || (t.classList.add("open"), e._fireEvent("open", t), e._dispatch("open.hs.overlay", t, t), e._focusInput(t))
+                                            }, 50)
+                                        }
+                                    }
+                                }, {
+                                    key: "close",
+                                    value: function(t) {
+                                        var e = this;
+                                        return new Promise(function(s) {
+                                            t && (t.classList.remove("open"), t.removeAttribute("aria-overlay"), t.removeAttribute("tabindex", "-1"), e.afterTransition(t, function() {
+                                                t.classList.contains("open") || (t.classList.add("hidden"), e._destroyBackdrop(), e._fireEvent("close", t), e._dispatch("close.hs.overlay", t, t), document.body.style.overflow = "", s(t))
+                                            }))
+                                        })
+                                    }
+                                }, {
+                                    key: "_autoHide",
+                                    value: function(t) {
+                                        var e = this,
+                                            s = parseInt(this.getClassProperty(t, "--auto-hide", "0"));
+                                        s && (t.autoHide = setTimeout(function() {
+                                            e.close(t)
+                                        }, s))
+                                    }
+                                }, {
+                                    key: "_checkTimer",
+                                    value: function(t) {
+                                        t.autoHide && (clearTimeout(t.autoHide), delete t.autoHide)
+                                    }
+                                }, {
+                                    key: "_onBackdropClick",
+                                    value: function(t) {
+                                        this.getClassProperty(t, "--overlay-backdrop", "true") !== "static" && this.close(t)
+                                    }
+                                }, {
+                                    key: "_buildBackdrop",
+                                    value: function(t) {
+                                        var e, s = this,
+                                            d = t.getAttribute("data-hs-overlay-backdrop-container") || !1,
+                                            l = document.createElement("div"),
+                                            p = "transition duration fixed inset-0 z-50 bg-gray-900 bg-opacity-50 dark:bg-opacity-80 hs-overlay-backdrop",
+                                            v = function(_, et) {
+                                                var U = typeof Symbol < "u" && _[Symbol.iterator] || _["@@iterator"];
+                                                if (!U) {
+                                                    if (Array.isArray(_) || (U = function(rt, Bt) {
+                                                            if (rt) {
+                                                                if (typeof rt == "string") return B(rt, Bt);
+                                                                var Ot = Object.prototype.toString.call(rt).slice(8, -1);
+                                                                return Ot === "Object" && rt.constructor && (Ot = rt.constructor.name), Ot === "Map" || Ot === "Set" ? Array.from(rt) : Ot === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(Ot) ? B(rt, Bt) : void 0
+                                                            }
+                                                        }(_)) || et && _ && typeof _.length == "number") {
+                                                        U && (_ = U);
+                                                        var kt = 0,
+                                                            Et = function() {};
+                                                        return {
+                                                            s: Et,
+                                                            n: function() {
+                                                                return kt >= _.length ? {
+                                                                    done: !0
+                                                                } : {
+                                                                    done: !1,
+                                                                    value: _[kt++]
+                                                                }
+                                                            },
+                                                            e: function(rt) {
+                                                                throw rt
+                                                            },
+                                                            f: Et
+                                                        }
                                                     }
-                                                }(e)) || t && e && "number" == typeof e.length) {
-                                                o && (e = o);
-                                                var n = 0,
-                                                    i = function() {};
+                                                    throw new TypeError(`Invalid attempt to iterate non-iterable instance.
+In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
+                                                }
+                                                var wt, xt = !0,
+                                                    Ht = !1;
                                                 return {
-                                                    s: i,
+                                                    s: function() {
+                                                        U = U.call(_)
+                                                    },
                                                     n: function() {
-                                                        return n >= e.length ? {
-                                                            done: !0
-                                                        } : {
-                                                            done: !1,
-                                                            value: e[n++]
-                                                        }
+                                                        var rt = U.next();
+                                                        return xt = rt.done, rt
                                                     },
-                                                    e: function(e) {
-                                                        throw e
+                                                    e: function(rt) {
+                                                        Ht = !0, wt = rt
                                                     },
-                                                    f: i
+                                                    f: function() {
+                                                        try {
+                                                            xt || U.return == null || U.return()
+                                                        } finally {
+                                                            if (Ht) throw wt
+                                                        }
+                                                    }
                                                 }
+                                            }(t.classList.values());
+                                        try {
+                                            for (v.s(); !(e = v.n()).done;) {
+                                                var S = e.value;
+                                                S.startsWith("hs-overlay-backdrop-open:") && (p += " ".concat(S))
                                             }
-                                            throw new TypeError("Invalid attempt to iterate non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
+                                        } catch (_) {
+                                            v.e(_)
+                                        } finally {
+                                            v.f()
                                         }
-                                        var a, s = !0,
-                                            c = !1;
-                                        return {
-                                            s: function() {
-                                                o = o.call(e)
-                                            },
-                                            n: function() {
-                                                var e = o.next();
-                                                return s = e.done, e
-                                            },
-                                            e: function(e) {
-                                                c = !0, a = e
-                                            },
-                                            f: function() {
-                                                try {
-                                                    s || null == o.return || o.return()
-                                                } finally {
-                                                    if (c) throw a
+                                        var E = this.getClassProperty(t, "--overlay-backdrop", "true") !== "static";
+                                        this.getClassProperty(t, "--overlay-backdrop", "true") === "false" || (d && ((l = document.querySelector(d).cloneNode(!0)).classList.remove("hidden"), p = l.classList, l.classList = ""), E && l.addEventListener("click", function() {
+                                            return s.close(t)
+                                        }, !0), l.setAttribute("data-hs-overlay-backdrop-template", ""), document.body.appendChild(l), setTimeout(function() {
+                                            l.classList = p
+                                        }))
+                                    }
+                                }, {
+                                    key: "_destroyBackdrop",
+                                    value: function() {
+                                        var t = document.querySelector("[data-hs-overlay-backdrop-template]");
+                                        t && (this.openNextOverlay && (t.style.transitionDuration = "".concat(1.8 * parseFloat(window.getComputedStyle(t).transitionDuration.replace(/[^\d.-]/g, "")), "s")), t.classList.add("opacity-0"), this.afterTransition(t, function() {
+                                            t.remove()
+                                        }))
+                                    }
+                                }, {
+                                    key: "_focusInput",
+                                    value: function(t) {
+                                        var e = t.querySelector("[autofocus]");
+                                        e && e.focus()
+                                    }
+                                }]) && C(a.prototype, o), Object.defineProperty(a, "prototype", {
+                                    writable: !1
+                                }), u
+                            }(N(765).Z);
+                            window.HSOverlay = new O, document.addEventListener("load", window.HSOverlay.init())
+                        },
+                        181: (G, it, N) => {
+                            function R(O) {
+                                return R = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(c) {
+                                    return typeof c
+                                } : function(c) {
+                                    return c && typeof Symbol == "function" && c.constructor === Symbol && c !== Symbol.prototype ? "symbol" : typeof c
+                                }, R(O)
+                            }
+
+                            function B(O, c) {
+                                for (var a = 0; a < c.length; a++) {
+                                    var o = c[a];
+                                    o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(O, o.key, o)
+                                }
+                            }
+
+                            function C(O, c) {
+                                return C = Object.setPrototypeOf || function(a, o) {
+                                    return a.__proto__ = o, a
+                                }, C(O, c)
+                            }
+
+                            function $(O, c) {
+                                if (c && (R(c) === "object" || typeof c == "function")) return c;
+                                if (c !== void 0) throw new TypeError("Derived constructors may only return object or undefined");
+                                return function(a) {
+                                    if (a === void 0) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                                    return a
+                                }(O)
+                            }
+
+                            function P(O) {
+                                return P = Object.setPrototypeOf ? Object.getPrototypeOf : function(c) {
+                                    return c.__proto__ || Object.getPrototypeOf(c)
+                                }, P(O)
+                            }
+                            var x = function(O) {
+                                (function(u, t) {
+                                    if (typeof t != "function" && t !== null) throw new TypeError("Super expression must either be null or a function");
+                                    u.prototype = Object.create(t && t.prototype, {
+                                        constructor: {
+                                            value: u,
+                                            writable: !0,
+                                            configurable: !0
+                                        }
+                                    }), Object.defineProperty(u, "prototype", {
+                                        writable: !1
+                                    }), t && C(u, t)
+                                })(h, O);
+                                var c, a, o, y, m = (o = h, y = function() {
+                                    if (typeof Reflect > "u" || !Reflect.construct || Reflect.construct.sham) return !1;
+                                    if (typeof Proxy == "function") return !0;
+                                    try {
+                                        return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
+                                    } catch {
+                                        return !1
+                                    }
+                                }(), function() {
+                                    var u, t = P(o);
+                                    if (y) {
+                                        var e = P(this).constructor;
+                                        u = Reflect.construct(t, arguments, e)
+                                    } else u = t.apply(this, arguments);
+                                    return $(this, u)
+                                });
+
+                                function h() {
+                                    return function(u, t) {
+                                        if (!(u instanceof t)) throw new TypeError("Cannot call a class as a function")
+                                    }(this, h), m.call(this, "[data-hs-remove-element]")
+                                }
+                                return c = h, (a = [{
+                                    key: "init",
+                                    value: function() {
+                                        var u = this;
+                                        document.addEventListener("click", function(t) {
+                                            var e = t.target.closest(u.selector);
+                                            if (e) {
+                                                var s = document.querySelector(e.getAttribute("data-hs-remove-element"));
+                                                s && (s.classList.add("hs-removing"), u.afterTransition(s, function() {
+                                                    s.remove()
+                                                }))
+                                            }
+                                        })
+                                    }
+                                }]) && B(c.prototype, a), Object.defineProperty(c, "prototype", {
+                                    writable: !1
+                                }), h
+                            }(N(765).Z);
+                            window.HSRemoveElement = new x, document.addEventListener("load", window.HSRemoveElement.init())
+                        },
+                        778: (G, it, N) => {
+                            function R(O) {
+                                return R = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(c) {
+                                    return typeof c
+                                } : function(c) {
+                                    return c && typeof Symbol == "function" && c.constructor === Symbol && c !== Symbol.prototype ? "symbol" : typeof c
+                                }, R(O)
+                            }
+
+                            function B(O, c) {
+                                for (var a = 0; a < c.length; a++) {
+                                    var o = c[a];
+                                    o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(O, o.key, o)
+                                }
+                            }
+
+                            function C(O, c) {
+                                return C = Object.setPrototypeOf || function(a, o) {
+                                    return a.__proto__ = o, a
+                                }, C(O, c)
+                            }
+
+                            function $(O, c) {
+                                if (c && (R(c) === "object" || typeof c == "function")) return c;
+                                if (c !== void 0) throw new TypeError("Derived constructors may only return object or undefined");
+                                return function(a) {
+                                    if (a === void 0) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                                    return a
+                                }(O)
+                            }
+
+                            function P(O) {
+                                return P = Object.setPrototypeOf ? Object.getPrototypeOf : function(c) {
+                                    return c.__proto__ || Object.getPrototypeOf(c)
+                                }, P(O)
+                            }
+                            var x = function(O) {
+                                (function(u, t) {
+                                    if (typeof t != "function" && t !== null) throw new TypeError("Super expression must either be null or a function");
+                                    u.prototype = Object.create(t && t.prototype, {
+                                        constructor: {
+                                            value: u,
+                                            writable: !0,
+                                            configurable: !0
+                                        }
+                                    }), Object.defineProperty(u, "prototype", {
+                                        writable: !1
+                                    }), t && C(u, t)
+                                })(h, O);
+                                var c, a, o, y, m = (o = h, y = function() {
+                                    if (typeof Reflect > "u" || !Reflect.construct || Reflect.construct.sham) return !1;
+                                    if (typeof Proxy == "function") return !0;
+                                    try {
+                                        return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
+                                    } catch {
+                                        return !1
+                                    }
+                                }(), function() {
+                                    var u, t = P(o);
+                                    if (y) {
+                                        var e = P(this).constructor;
+                                        u = Reflect.construct(t, arguments, e)
+                                    } else u = t.apply(this, arguments);
+                                    return $(this, u)
+                                });
+
+                                function h() {
+                                    var u;
+                                    return function(t, e) {
+                                        if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
+                                    }(this, h), (u = m.call(this, "[data-hs-scrollspy] ")).activeSection = null, u
+                                }
+                                return c = h, (a = [{
+                                    key: "init",
+                                    value: function() {
+                                        var u = this;
+                                        document.querySelectorAll(this.selector).forEach(function(t) {
+                                            var e = document.querySelector(t.getAttribute("data-hs-scrollspy")),
+                                                s = t.querySelectorAll("[href]"),
+                                                d = e.children,
+                                                l = t.getAttribute("data-hs-scrollspy-scrollable-parent") ? document.querySelector(t.getAttribute("data-hs-scrollspy-scrollable-parent")) : document;
+                                            Array.from(d).forEach(function(p) {
+                                                p.getAttribute("id") && l.addEventListener("scroll", function(v) {
+                                                    return u._update({
+                                                        $scrollspyEl: t,
+                                                        $scrollspyContentEl: e,
+                                                        links: s,
+                                                        $sectionEl: p,
+                                                        sections: d,
+                                                        ev: v
+                                                    })
+                                                })
+                                            }), s.forEach(function(p) {
+                                                p.addEventListener("click", function(v) {
+                                                    v.preventDefault(), p.getAttribute("href") !== "javascript:;" && u._scrollTo({
+                                                        $scrollspyEl: t,
+                                                        $scrollableEl: l,
+                                                        $link: p
+                                                    })
+                                                })
+                                            })
+                                        })
+                                    }
+                                }, {
+                                    key: "_update",
+                                    value: function(u) {
+                                        var t = u.ev,
+                                            e = u.$scrollspyEl,
+                                            s = (u.sections, u.links),
+                                            d = u.$sectionEl,
+                                            l = parseInt(this.getClassProperty(e, "--scrollspy-offset", "0")),
+                                            p = this.getClassProperty(d, "--scrollspy-offset") || l,
+                                            v = t.target === document ? 0 : parseInt(t.target.getBoundingClientRect().top),
+                                            S = parseInt(d.getBoundingClientRect().top) - p - v,
+                                            E = d.offsetHeight;
+                                        if (S <= 0 && S + E > 0) {
+                                            if (this.activeSection === d) return;
+                                            s.forEach(function(kt) {
+                                                kt.classList.remove("active")
+                                            });
+                                            var _ = e.querySelector('[href="#'.concat(d.getAttribute("id"), '"]'));
+                                            if (_) {
+                                                _.classList.add("active");
+                                                var et = _.closest("[data-hs-scrollspy-group]");
+                                                if (et) {
+                                                    var U = et.querySelector("[href]");
+                                                    U && U.classList.add("active")
                                                 }
                                             }
+                                            this.activeSection = d
                                         }
-                                    }(e.classList.values());
-                                try {
-                                    for (s.s(); !(t = s.n()).done;) {
-                                        var c = t.value;
-                                        c.startsWith("hs-overlay-backdrop-open:") && (a += " ".concat(c))
-                                    }
-                                } catch (e) {
-                                    s.e(e)
-                                } finally {
-                                    s.f()
-                                }
-                                var l = "static" !== this.getClassProperty(e, "--overlay-backdrop", "true");
-                                "false" === this.getClassProperty(e, "--overlay-backdrop", "true") || (n && ((i = document.querySelector(n).cloneNode(!0)).classList.remove("hidden"), a = i.classList, i.classList = ""), l && i.addEventListener("click", (function() {
-                                    return o.close(e)
-                                }), !0), i.setAttribute("data-hs-overlay-backdrop-template", ""), document.body.appendChild(i), setTimeout((function() {
-                                    i.classList = a
-                                })))
-                            }
-                        }, {
-                            key: "_destroyBackdrop",
-                            value: function() {
-                                var e = document.querySelector("[data-hs-overlay-backdrop-template]");
-                                e && (this.openNextOverlay && (e.style.transitionDuration = "".concat(1.8 * parseFloat(window.getComputedStyle(e).transitionDuration.replace(/[^\d.-]/g, "")), "s")), e.classList.add("opacity-0"), this.afterTransition(e, (function() {
-                                    e.remove()
-                                })))
-                            }
-                        }, {
-                            key: "_focusInput",
-                            value: function(e) {
-                                var t = e.querySelector("[autofocus]");
-                                t && t.focus()
-                            }
-                        }]) && i(t.prototype, o), Object.defineProperty(t, "prototype", {
-                            writable: !1
-                        }), f
-                    }(o(765).Z);
-                    window.HSOverlay = new l, document.addEventListener("load", window.HSOverlay.init())
-                },
-                181: (e, t, o) => {
-                    function n(e) {
-                        return n = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-                            return typeof e
-                        } : function(e) {
-                            return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                        }, n(e)
-                    }
-
-                    function r(e, t) {
-                        for (var o = 0; o < t.length; o++) {
-                            var n = t[o];
-                            n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
-                        }
-                    }
-
-                    function i(e, t) {
-                        return i = Object.setPrototypeOf || function(e, t) {
-                            return e.__proto__ = t, e
-                        }, i(e, t)
-                    }
-
-                    function a(e, t) {
-                        if (t && ("object" === n(t) || "function" == typeof t)) return t;
-                        if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                        return function(e) {
-                            if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-                            return e
-                        }(e)
-                    }
-
-                    function s(e) {
-                        return s = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
-                            return e.__proto__ || Object.getPrototypeOf(e)
-                        }, s(e)
-                    }
-                    var c = function(e) {
-                        ! function(e, t) {
-                            if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
-                            e.prototype = Object.create(t && t.prototype, {
-                                constructor: {
-                                    value: e,
-                                    writable: !0,
-                                    configurable: !0
-                                }
-                            }), Object.defineProperty(e, "prototype", {
-                                writable: !1
-                            }), t && i(e, t)
-                        }(u, e);
-                        var t, o, n, c, l = (n = u, c = function() {
-                            if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
-                            if (Reflect.construct.sham) return !1;
-                            if ("function" == typeof Proxy) return !0;
-                            try {
-                                return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
-                            } catch (e) {
-                                return !1
+                                    }
+                                }, {
+                                    key: "_scrollTo",
+                                    value: function(u) {
+                                        var t = u.$scrollspyEl,
+                                            e = u.$scrollableEl,
+                                            s = u.$link,
+                                            d = document.querySelector(s.getAttribute("href")),
+                                            l = parseInt(this.getClassProperty(t, "--scrollspy-offset", "0")),
+                                            p = this.getClassProperty(d, "--scrollspy-offset") || l,
+                                            v = e === document ? 0 : e.offsetTop,
+                                            S = d.offsetTop - p - v,
+                                            E = e === document ? window : e;
+                                        this._fireEvent("scroll", t), this._dispatch("scroll.hs.scrollspy", t, t), window.history.replaceState(null, null, s.getAttribute("href")), E.scrollTo({
+                                            top: S,
+                                            left: 0,
+                                            behavior: "smooth"
+                                        })
+                                    }
+                                }]) && B(c.prototype, a), Object.defineProperty(c, "prototype", {
+                                    writable: !1
+                                }), h
+                            }(N(765).Z);
+                            window.HSScrollspy = new x, document.addEventListener("load", window.HSScrollspy.init())
+                        },
+                        51: (G, it, N) => {
+                            function R(a) {
+                                return R = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(o) {
+                                    return typeof o
+                                } : function(o) {
+                                    return o && typeof Symbol == "function" && o.constructor === Symbol && o !== Symbol.prototype ? "symbol" : typeof o
+                                }, R(a)
                             }
-                        }(), function() {
-                            var e, t = s(n);
-                            if (c) {
-                                var o = s(this).constructor;
-                                e = Reflect.construct(t, arguments, o)
-                            } else e = t.apply(this, arguments);
-                            return a(this, e)
-                        });
-
-                        function u() {
-                            return function(e, t) {
-                                if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                            }(this, u), l.call(this, "[data-hs-remove-element]")
-                        }
-                        return t = u, (o = [{
-                            key: "init",
-                            value: function() {
-                                var e = this;
-                                document.addEventListener("click", (function(t) {
-                                    var o = t.target.closest(e.selector);
+
+                            function B(a) {
+                                return function(o) {
+                                    if (Array.isArray(o)) return C(o)
+                                }(a) || function(o) {
+                                    if (typeof Symbol < "u" && o[Symbol.iterator] != null || o["@@iterator"] != null) return Array.from(o)
+                                }(a) || function(o, y) {
                                     if (o) {
-                                        var n = document.querySelector(o.getAttribute("data-hs-remove-element"));
-                                        n && (n.classList.add("hs-removing"), e.afterTransition(n, (function() {
-                                            n.remove()
-                                        })))
-                                    }
-                                }))
-                            }
-                        }]) && r(t.prototype, o), Object.defineProperty(t, "prototype", {
-                            writable: !1
-                        }), u
-                    }(o(765).Z);
-                    window.HSRemoveElement = new c, document.addEventListener("load", window.HSRemoveElement.init())
-                },
-                778: (e, t, o) => {
-                    function n(e) {
-                        return n = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-                            return typeof e
-                        } : function(e) {
-                            return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                        }, n(e)
-                    }
-
-                    function r(e, t) {
-                        for (var o = 0; o < t.length; o++) {
-                            var n = t[o];
-                            n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
-                        }
-                    }
+                                        if (typeof o == "string") return C(o, y);
+                                        var m = Object.prototype.toString.call(o).slice(8, -1);
+                                        return m === "Object" && o.constructor && (m = o.constructor.name), m === "Map" || m === "Set" ? Array.from(o) : m === "Arguments" || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(m) ? C(o, y) : void 0
+                                    }
+                                }(a) || function() {
+                                    throw new TypeError(`Invalid attempt to spread non-iterable instance.
+In order to be iterable, non-array objects must have a [Symbol.iterator]() method.`)
+                                }()
+                            }
 
-                    function i(e, t) {
-                        return i = Object.setPrototypeOf || function(e, t) {
-                            return e.__proto__ = t, e
-                        }, i(e, t)
-                    }
-
-                    function a(e, t) {
-                        if (t && ("object" === n(t) || "function" == typeof t)) return t;
-                        if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                        return function(e) {
-                            if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-                            return e
-                        }(e)
-                    }
-
-                    function s(e) {
-                        return s = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
-                            return e.__proto__ || Object.getPrototypeOf(e)
-                        }, s(e)
-                    }
-                    var c = function(e) {
-                        ! function(e, t) {
-                            if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
-                            e.prototype = Object.create(t && t.prototype, {
-                                constructor: {
-                                    value: e,
-                                    writable: !0,
-                                    configurable: !0
-                                }
-                            }), Object.defineProperty(e, "prototype", {
-                                writable: !1
-                            }), t && i(e, t)
-                        }(u, e);
-                        var t, o, n, c, l = (n = u, c = function() {
-                            if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
-                            if (Reflect.construct.sham) return !1;
-                            if ("function" == typeof Proxy) return !0;
-                            try {
-                                return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
-                            } catch (e) {
-                                return !1
+                            function C(a, o) {
+                                (o == null || o > a.length) && (o = a.length);
+                                for (var y = 0, m = new Array(o); y < o; y++) m[y] = a[y];
+                                return m
                             }
-                        }(), function() {
-                            var e, t = s(n);
-                            if (c) {
-                                var o = s(this).constructor;
-                                e = Reflect.construct(t, arguments, o)
-                            } else e = t.apply(this, arguments);
-                            return a(this, e)
-                        });
-
-                        function u() {
-                            var e;
-                            return function(e, t) {
-                                if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                            }(this, u), (e = l.call(this, "[data-hs-scrollspy] ")).activeSection = null, e
-                        }
-                        return t = u, (o = [{
-                            key: "init",
-                            value: function() {
-                                var e = this;
-                                document.querySelectorAll(this.selector).forEach((function(t) {
-                                    var o = document.querySelector(t.getAttribute("data-hs-scrollspy")),
-                                        n = t.querySelectorAll("[href]"),
-                                        r = o.children,
-                                        i = t.getAttribute("data-hs-scrollspy-scrollable-parent") ? document.querySelector(t.getAttribute("data-hs-scrollspy-scrollable-parent")) : document;
-                                    Array.from(r).forEach((function(a) {
-                                        a.getAttribute("id") && i.addEventListener("scroll", (function(i) {
-                                            return e._update({
-                                                $scrollspyEl: t,
-                                                $scrollspyContentEl: o,
-                                                links: n,
-                                                $sectionEl: a,
-                                                sections: r,
-                                                ev: i
-                                            })
-                                        }))
-                                    })), n.forEach((function(o) {
-                                        o.addEventListener("click", (function(n) {
-                                            n.preventDefault(), "javascript:;" !== o.getAttribute("href") && e._scrollTo({
-                                                $scrollspyEl: t,
-                                                $scrollableEl: i,
-                                                $link: o
+
+                            function $(a, o) {
+                                for (var y = 0; y < o.length; y++) {
+                                    var m = o[y];
+                                    m.enumerable = m.enumerable || !1, m.configurable = !0, "value" in m && (m.writable = !0), Object.defineProperty(a, m.key, m)
+                                }
+                            }
+
+                            function P(a, o) {
+                                return P = Object.setPrototypeOf || function(y, m) {
+                                    return y.__proto__ = m, y
+                                }, P(a, o)
+                            }
+
+                            function x(a, o) {
+                                if (o && (R(o) === "object" || typeof o == "function")) return o;
+                                if (o !== void 0) throw new TypeError("Derived constructors may only return object or undefined");
+                                return function(y) {
+                                    if (y === void 0) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                                    return y
+                                }(a)
+                            }
+
+                            function O(a) {
+                                return O = Object.setPrototypeOf ? Object.getPrototypeOf : function(o) {
+                                    return o.__proto__ || Object.getPrototypeOf(o)
+                                }, O(a)
+                            }
+                            var c = function(a) {
+                                (function(e, s) {
+                                    if (typeof s != "function" && s !== null) throw new TypeError("Super expression must either be null or a function");
+                                    e.prototype = Object.create(s && s.prototype, {
+                                        constructor: {
+                                            value: e,
+                                            writable: !0,
+                                            configurable: !0
+                                        }
+                                    }), Object.defineProperty(e, "prototype", {
+                                        writable: !1
+                                    }), s && P(e, s)
+                                })(t, a);
+                                var o, y, m, h, u = (m = t, h = function() {
+                                    if (typeof Reflect > "u" || !Reflect.construct || Reflect.construct.sham) return !1;
+                                    if (typeof Proxy == "function") return !0;
+                                    try {
+                                        return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
+                                    } catch {
+                                        return !1
+                                    }
+                                }(), function() {
+                                    var e, s = O(m);
+                                    if (h) {
+                                        var d = O(this).constructor;
+                                        e = Reflect.construct(s, arguments, d)
+                                    } else e = s.apply(this, arguments);
+                                    return x(this, e)
+                                });
+
+                                function t() {
+                                    return function(e, s) {
+                                        if (!(e instanceof s)) throw new TypeError("Cannot call a class as a function")
+                                    }(this, t), u.call(this, "[data-hs-tab]")
+                                }
+                                return o = t, (y = [{
+                                    key: "init",
+                                    value: function() {
+                                        var e = this;
+                                        document.addEventListener("keydown", this._keyboardSupport.bind(this)), document.addEventListener("click", function(s) {
+                                            var d = s.target.closest(e.selector);
+                                            d && e.open(d)
+                                        }), document.querySelectorAll("[hs-data-tab-select]").forEach(function(s) {
+                                            var d = document.querySelector(s.getAttribute("hs-data-tab-select"));
+                                            d && d.addEventListener("change", function(l) {
+                                                var p = document.querySelector('[data-hs-tab="'.concat(l.target.value, '"]'));
+                                                p && e.open(p)
                                             })
-                                        }))
-                                    }))
-                                }))
+                                        })
+                                    }
+                                }, {
+                                    key: "open",
+                                    value: function(e) {
+                                        var s = document.querySelector(e.getAttribute("data-hs-tab")),
+                                            d = B(e.parentElement.children),
+                                            l = B(s.parentElement.children),
+                                            p = e.closest("[hs-data-tab-select]"),
+                                            v = p ? document.querySelector(p.getAttribute("data-hs-tab")) : null;
+                                        d.forEach(function(S) {
+                                            return S.classList.remove("active")
+                                        }), l.forEach(function(S) {
+                                            return S.classList.add("hidden")
+                                        }), e.classList.add("active"), s.classList.remove("hidden"), this._fireEvent("change", e), this._dispatch("change.hs.tab", e, e), v && (v.value = e.getAttribute("data-hs-tab"))
+                                    }
+                                }, {
+                                    key: "_keyboardSupport",
+                                    value: function(e) {
+                                        var s = e.target.closest(this.selector);
+                                        if (s) {
+                                            var d = s.closest('[role="tablist"]').getAttribute("data-hs-tabs-vertical") === "true";
+                                            return (d ? e.keyCode === 38 : e.keyCode === 37) ? (e.preventDefault(), this._left(s)) : (d ? e.keyCode === 40 : e.keyCode === 39) ? (e.preventDefault(), this._right(s)) : e.keyCode === 36 ? (e.preventDefault(), this._start(s)) : e.keyCode === 35 ? (e.preventDefault(), this._end(s)) : void 0
+                                        }
+                                    }
+                                }, {
+                                    key: "_right",
+                                    value: function(e) {
+                                        var s = e.closest('[role="tablist"]');
+                                        if (s) {
+                                            var d = B(s.querySelectorAll(this.selector)).filter(function(v) {
+                                                    return !v.disabled
+                                                }),
+                                                l = s.querySelector("button:focus"),
+                                                p = d.findIndex(function(v) {
+                                                    return v === l
+                                                });
+                                            p + 1 < d.length ? p++ : p = 0, d[p].focus(), this.open(d[p])
+                                        }
+                                    }
+                                }, {
+                                    key: "_left",
+                                    value: function(e) {
+                                        var s = e.closest('[role="tablist"]');
+                                        if (s) {
+                                            var d = B(s.querySelectorAll(this.selector)).filter(function(v) {
+                                                    return !v.disabled
+                                                }).reverse(),
+                                                l = s.querySelector("button:focus"),
+                                                p = d.findIndex(function(v) {
+                                                    return v === l
+                                                });
+                                            p + 1 < d.length ? p++ : p = 0, d[p].focus(), this.open(d[p])
+                                        }
+                                    }
+                                }, {
+                                    key: "_start",
+                                    value: function(e) {
+                                        var s = e.closest('[role="tablist"]');
+                                        if (s) {
+                                            var d = B(s.querySelectorAll(this.selector)).filter(function(l) {
+                                                return !l.disabled
+                                            });
+                                            d.length && (d[0].focus(), this.open(d[0]))
+                                        }
+                                    }
+                                }, {
+                                    key: "_end",
+                                    value: function(e) {
+                                        var s = e.closest('[role="tablist"]');
+                                        if (s) {
+                                            var d = B(s.querySelectorAll(this.selector)).reverse().filter(function(l) {
+                                                return !l.disabled
+                                            });
+                                            d.length && (d[0].focus(), this.open(d[0]))
+                                        }
+                                    }
+                                }]) && $(o.prototype, y), Object.defineProperty(o, "prototype", {
+                                    writable: !1
+                                }), t
+                            }(N(765).Z);
+                            window.HSTabs = new c, document.addEventListener("load", window.HSTabs.init())
+                        },
+                        185: (G, it, N) => {
+                            var R = N(765),
+                                B = N(714);
+
+                            function C(a) {
+                                return C = typeof Symbol == "function" && typeof Symbol.iterator == "symbol" ? function(o) {
+                                    return typeof o
+                                } : function(o) {
+                                    return o && typeof Symbol == "function" && o.constructor === Symbol && o !== Symbol.prototype ? "symbol" : typeof o
+                                }, C(a)
+                            }
+
+                            function $(a, o) {
+                                for (var y = 0; y < o.length; y++) {
+                                    var m = o[y];
+                                    m.enumerable = m.enumerable || !1, m.configurable = !0, "value" in m && (m.writable = !0), Object.defineProperty(a, m.key, m)
+                                }
                             }
-                        }, {
-                            key: "_update",
-                            value: function(e) {
-                                var t = e.ev,
-                                    o = e.$scrollspyEl,
-                                    n = (e.sections, e.links),
-                                    r = e.$sectionEl,
-                                    i = parseInt(this.getClassProperty(o, "--scrollspy-offset", "0")),
-                                    a = this.getClassProperty(r, "--scrollspy-offset") || i,
-                                    s = t.target === document ? 0 : parseInt(t.target.getBoundingClientRect().top),
-                                    c = parseInt(r.getBoundingClientRect().top) - a - s,
-                                    l = r.offsetHeight;
-                                if (c <= 0 && c + l > 0) {
-                                    if (this.activeSection === r) return;
-                                    n.forEach((function(e) {
-                                        e.classList.remove("active")
-                                    }));
-                                    var u = o.querySelector('[href="#'.concat(r.getAttribute("id"), '"]'));
-                                    if (u) {
-                                        u.classList.add("active");
-                                        var f = u.closest("[data-hs-scrollspy-group]");
-                                        if (f) {
-                                            var p = f.querySelector("[href]");
-                                            p && p.classList.add("active")
-                                        }
-                                    }
-                                    this.activeSection = r
-                                }
-                            }
-                        }, {
-                            key: "_scrollTo",
-                            value: function(e) {
-                                var t = e.$scrollspyEl,
-                                    o = e.$scrollableEl,
-                                    n = e.$link,
-                                    r = document.querySelector(n.getAttribute("href")),
-                                    i = parseInt(this.getClassProperty(t, "--scrollspy-offset", "0")),
-                                    a = this.getClassProperty(r, "--scrollspy-offset") || i,
-                                    s = o === document ? 0 : o.offsetTop,
-                                    c = r.offsetTop - a - s,
-                                    l = o === document ? window : o;
-                                this._fireEvent("scroll", t), this._dispatch("scroll.hs.scrollspy", t, t), window.history.replaceState(null, null, n.getAttribute("href")), l.scrollTo({
-                                    top: c,
-                                    left: 0,
-                                    behavior: "smooth"
-                                })
+
+                            function P(a, o) {
+                                return P = Object.setPrototypeOf || function(y, m) {
+                                    return y.__proto__ = m, y
+                                }, P(a, o)
+                            }
+
+                            function x(a, o) {
+                                if (o && (C(o) === "object" || typeof o == "function")) return o;
+                                if (o !== void 0) throw new TypeError("Derived constructors may only return object or undefined");
+                                return function(y) {
+                                    if (y === void 0) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                                    return y
+                                }(a)
+                            }
+
+                            function O(a) {
+                                return O = Object.setPrototypeOf ? Object.getPrototypeOf : function(o) {
+                                    return o.__proto__ || Object.getPrototypeOf(o)
+                                }, O(a)
+                            }
+                            var c = function(a) {
+                                (function(e, s) {
+                                    if (typeof s != "function" && s !== null) throw new TypeError("Super expression must either be null or a function");
+                                    e.prototype = Object.create(s && s.prototype, {
+                                        constructor: {
+                                            value: e,
+                                            writable: !0,
+                                            configurable: !0
+                                        }
+                                    }), Object.defineProperty(e, "prototype", {
+                                        writable: !1
+                                    }), s && P(e, s)
+                                })(t, a);
+                                var o, y, m, h, u = (m = t, h = function() {
+                                    if (typeof Reflect > "u" || !Reflect.construct || Reflect.construct.sham) return !1;
+                                    if (typeof Proxy == "function") return !0;
+                                    try {
+                                        return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], function() {})), !0
+                                    } catch {
+                                        return !1
+                                    }
+                                }(), function() {
+                                    var e, s = O(m);
+                                    if (h) {
+                                        var d = O(this).constructor;
+                                        e = Reflect.construct(s, arguments, d)
+                                    } else e = s.apply(this, arguments);
+                                    return x(this, e)
+                                });
+
+                                function t() {
+                                    return function(e, s) {
+                                        if (!(e instanceof s)) throw new TypeError("Cannot call a class as a function")
+                                    }(this, t), u.call(this, ".hs-tooltip")
+                                }
+                                return o = t, (y = [{
+                                    key: "init",
+                                    value: function() {
+                                        var e = this;
+                                        document.addEventListener("click", function(s) {
+                                            var d = s.target.closest(e.selector);
+                                            d && e.getClassProperty(d, "--trigger") === "focus" && e._focus(d), d && e.getClassProperty(d, "--trigger") === "click" && e._click(d)
+                                        }), document.addEventListener("mousemove", function(s) {
+                                            var d = s.target.closest(e.selector);
+                                            d && e.getClassProperty(d, "--trigger") !== "focus" && e.getClassProperty(d, "--trigger") !== "click" && e._hover(d)
+                                        })
+                                    }
+                                }, {
+                                    key: "_hover",
+                                    value: function(e) {
+                                        var s = this;
+                                        if (!e.classList.contains("show")) {
+                                            var d = e.querySelector(".hs-tooltip-toggle"),
+                                                l = e.querySelector(".hs-tooltip-content"),
+                                                p = this.getClassProperty(e, "--placement");
+                                            (0, B.fi)(d, l, {
+                                                placement: p || "top",
+                                                strategy: "fixed",
+                                                modifiers: [{
+                                                    name: "offset",
+                                                    options: {
+                                                        offset: [0, 5]
+                                                    }
+                                                }]
+                                            }), this.show(e), e.addEventListener("mouseleave", function v(S) {
+                                                S.toElement.closest(s.selector) && S.toElement.closest(s.selector) == e || (s.hide(e), e.removeEventListener("mouseleave", v, !0))
+                                            }, !0)
+                                        }
+                                    }
+                                }, {
+                                    key: "_focus",
+                                    value: function(e) {
+                                        var s = this,
+                                            d = e.querySelector(".hs-tooltip-toggle"),
+                                            l = e.querySelector(".hs-tooltip-content"),
+                                            p = this.getClassProperty(e, "--placement"),
+                                            v = this.getClassProperty(e, "--strategy");
+                                        (0, B.fi)(d, l, {
+                                            placement: p || "top",
+                                            strategy: v || "fixed",
+                                            modifiers: [{
+                                                name: "offset",
+                                                options: {
+                                                    offset: [0, 5]
+                                                }
+                                            }]
+                                        }), this.show(e), e.addEventListener("blur", function S() {
+                                            s.hide(e), e.removeEventListener("blur", S, !0)
+                                        }, !0)
+                                    }
+                                }, {
+                                    key: "_click",
+                                    value: function(e) {
+                                        var s = this;
+                                        if (!e.classList.contains("show")) {
+                                            var d = e.querySelector(".hs-tooltip-toggle"),
+                                                l = e.querySelector(".hs-tooltip-content"),
+                                                p = this.getClassProperty(e, "--placement"),
+                                                v = this.getClassProperty(e, "--strategy");
+                                            (0, B.fi)(d, l, {
+                                                placement: p || "top",
+                                                strategy: v || "fixed",
+                                                modifiers: [{
+                                                    name: "offset",
+                                                    options: {
+                                                        offset: [0, 5]
+                                                    }
+                                                }]
+                                            }), this.show(e);
+                                            var S = function E(_) {
+                                                setTimeout(function() {
+                                                    s.hide(e), e.removeEventListener("click", E, !0), e.removeEventListener("blur", E, !0)
+                                                })
+                                            };
+                                            e.addEventListener("blur", S, !0), e.addEventListener("click", S, !0)
+                                        }
+                                    }
+                                }, {
+                                    key: "show",
+                                    value: function(e) {
+                                        var s = this;
+                                        e.querySelector(".hs-tooltip-content").classList.remove("hidden"), setTimeout(function() {
+                                            e.classList.add("show"), s._fireEvent("show", e), s._dispatch("show.hs.tooltip", e, e)
+                                        })
+                                    }
+                                }, {
+                                    key: "hide",
+                                    value: function(e) {
+                                        var s = e.querySelector(".hs-tooltip-content");
+                                        e.classList.remove("show"), this._fireEvent("hide", e), this._dispatch("hide.hs.tooltip", e, e), this.afterTransition(s, function() {
+                                            e.classList.contains("show") || s.classList.add("hidden")
+                                        })
+                                    }
+                                }]) && $(o.prototype, y), Object.defineProperty(o, "prototype", {
+                                    writable: !1
+                                }), t
+                            }(R.Z);
+                            window.HSTooltip = new c, document.addEventListener("load", window.HSTooltip.init())
+                        },
+                        765: (G, it, N) => {
+                            function R(C, $) {
+                                for (var P = 0; P < $.length; P++) {
+                                    var x = $[P];
+                                    x.enumerable = x.enumerable || !1, x.configurable = !0, "value" in x && (x.writable = !0), Object.defineProperty(C, x.key, x)
+                                }
+                            }
+                            N.d(it, {
+                                Z: () => B
+                            });
+                            var B = function() {
+                                function C(x, O) {
+                                    (function(c, a) {
+                                        if (!(c instanceof a)) throw new TypeError("Cannot call a class as a function")
+                                    })(this, C), this.$collection = [], this.selector = x, this.config = O, this.events = {}
+                                }
+                                var $, P;
+                                return $ = C, P = [{
+                                    key: "_fireEvent",
+                                    value: function(x) {
+                                        var O = arguments.length > 1 && arguments[1] !== void 0 ? arguments[1] : null;
+                                        this.events.hasOwnProperty(x) && this.events[x](O)
+                                    }
+                                }, {
+                                    key: "_dispatch",
+                                    value: function(x, O) {
+                                        var c = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : null,
+                                            a = new CustomEvent(x, {
+                                                detail: {
+                                                    payload: c
+                                                },
+                                                bubbles: !0,
+                                                cancelable: !0,
+                                                composed: !1
+                                            });
+                                        O.dispatchEvent(a)
+                                    }
+                                }, {
+                                    key: "on",
+                                    value: function(x, O) {
+                                        this.events[x] = O
+                                    }
+                                }, {
+                                    key: "afterTransition",
+                                    value: function(x, O) {
+                                        window.getComputedStyle(x, null).getPropertyValue("transition") !== "all 0s ease 0s" ? x.addEventListener("transitionend", function c() {
+                                            O(), x.removeEventListener("transitionend", c, !0)
+                                        }, !0) : O()
+                                    }
+                                }, {
+                                    key: "getClassProperty",
+                                    value: function(x, O) {
+                                        var c = arguments.length > 2 && arguments[2] !== void 0 ? arguments[2] : "",
+                                            a = (window.getComputedStyle(x).getPropertyValue(O) || c).replace(" ", "");
+                                        return a
+                                    }
+                                }], P && R($.prototype, P), Object.defineProperty($, "prototype", {
+                                    writable: !1
+                                }), C
+                            }()
+                        },
+                        714: (G, it, N) => {
+                            function R(n) {
+                                if (n == null) return window;
+                                if (n.toString() !== "[object Window]") {
+                                    var r = n.ownerDocument;
+                                    return r && r.defaultView || window
+                                }
+                                return n
                             }
-                        }]) && r(t.prototype, o), Object.defineProperty(t, "prototype", {
-                            writable: !1
-                        }), u
-                    }(o(765).Z);
-                    window.HSScrollspy = new c, document.addEventListener("load", window.HSScrollspy.init())
-                },
-                51: (e, t, o) => {
-                    function n(e) {
-                        return n = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-                            return typeof e
-                        } : function(e) {
-                            return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                        }, n(e)
-                    }
-
-                    function r(e) {
-                        return function(e) {
-                            if (Array.isArray(e)) return i(e)
-                        }(e) || function(e) {
-                            if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
-                        }(e) || function(e, t) {
-                            if (e) {
-                                if ("string" == typeof e) return i(e, t);
-                                var o = Object.prototype.toString.call(e).slice(8, -1);
-                                return "Object" === o && e.constructor && (o = e.constructor.name), "Map" === o || "Set" === o ? Array.from(e) : "Arguments" === o || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(o) ? i(e, t) : void 0
-                            }
-                        }(e) || function() {
-                            throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
-                        }()
-                    }
-
-                    function i(e, t) {
-                        (null == t || t > e.length) && (t = e.length);
-                        for (var o = 0, n = new Array(t); o < t; o++) n[o] = e[o];
-                        return n
-                    }
-
-                    function a(e, t) {
-                        for (var o = 0; o < t.length; o++) {
-                            var n = t[o];
-                            n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
-                        }
-                    }
 
-                    function s(e, t) {
-                        return s = Object.setPrototypeOf || function(e, t) {
-                            return e.__proto__ = t, e
-                        }, s(e, t)
-                    }
-
-                    function c(e, t) {
-                        if (t && ("object" === n(t) || "function" == typeof t)) return t;
-                        if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                        return function(e) {
-                            if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-                            return e
-                        }(e)
-                    }
-
-                    function l(e) {
-                        return l = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
-                            return e.__proto__ || Object.getPrototypeOf(e)
-                        }, l(e)
-                    }
-                    var u = function(e) {
-                        ! function(e, t) {
-                            if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
-                            e.prototype = Object.create(t && t.prototype, {
-                                constructor: {
-                                    value: e,
-                                    writable: !0,
-                                    configurable: !0
-                                }
-                            }), Object.defineProperty(e, "prototype", {
-                                writable: !1
-                            }), t && s(e, t)
-                        }(f, e);
-                        var t, o, n, i, u = (n = f, i = function() {
-                            if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
-                            if (Reflect.construct.sham) return !1;
-                            if ("function" == typeof Proxy) return !0;
-                            try {
-                                return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
-                            } catch (e) {
-                                return !1
+                            function B(n) {
+                                return n instanceof R(n).Element || n instanceof Element
                             }
-                        }(), function() {
-                            var e, t = l(n);
-                            if (i) {
-                                var o = l(this).constructor;
-                                e = Reflect.construct(t, arguments, o)
-                            } else e = t.apply(this, arguments);
-                            return c(this, e)
-                        });
-
-                        function f() {
-                            return function(e, t) {
-                                if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                            }(this, f), u.call(this, "[data-hs-tab]")
-                        }
-                        return t = f, (o = [{
-                            key: "init",
-                            value: function() {
-                                var e = this;
-                                document.addEventListener("keydown", this._keyboardSupport.bind(this)), document.addEventListener("click", (function(t) {
-                                    var o = t.target.closest(e.selector);
-                                    o && e.open(o)
-                                })), document.querySelectorAll("[hs-data-tab-select]").forEach((function(t) {
-                                    var o = document.querySelector(t.getAttribute("hs-data-tab-select"));
-                                    o && o.addEventListener("change", (function(t) {
-                                        var o = document.querySelector('[data-hs-tab="'.concat(t.target.value, '"]'));
-                                        o && e.open(o)
-                                    }))
-                                }))
-                            }
-                        }, {
-                            key: "open",
-                            value: function(e) {
-                                var t = document.querySelector(e.getAttribute("data-hs-tab")),
-                                    o = r(e.parentElement.children),
-                                    n = r(t.parentElement.children),
-                                    i = e.closest("[hs-data-tab-select]"),
-                                    a = i ? document.querySelector(i.getAttribute("data-hs-tab")) : null;
-                                o.forEach((function(e) {
-                                    return e.classList.remove("active")
-                                })), n.forEach((function(e) {
-                                    return e.classList.add("hidden")
-                                })), e.classList.add("active"), t.classList.remove("hidden"), this._fireEvent("change", e), this._dispatch("change.hs.tab", e, e), a && (a.value = e.getAttribute("data-hs-tab"))
-                            }
-                        }, {
-                            key: "_keyboardSupport",
-                            value: function(e) {
-                                var t = e.target.closest(this.selector);
-                                if (t) {
-                                    var o = "true" === t.closest('[role="tablist"]').getAttribute("data-hs-tabs-vertical");
-                                    return (o ? 38 === e.keyCode : 37 === e.keyCode) ? (e.preventDefault(), this._left(t)) : (o ? 40 === e.keyCode : 39 === e.keyCode) ? (e.preventDefault(), this._right(t)) : 36 === e.keyCode ? (e.preventDefault(), this._start(t)) : 35 === e.keyCode ? (e.preventDefault(), this._end(t)) : void 0
-                                }
-                            }
-                        }, {
-                            key: "_right",
-                            value: function(e) {
-                                var t = e.closest('[role="tablist"]');
-                                if (t) {
-                                    var o = r(t.querySelectorAll(this.selector)).filter((function(e) {
-                                            return !e.disabled
-                                        })),
-                                        n = t.querySelector("button:focus"),
-                                        i = o.findIndex((function(e) {
-                                            return e === n
-                                        }));
-                                    i + 1 < o.length ? i++ : i = 0, o[i].focus(), this.open(o[i])
-                                }
-                            }
-                        }, {
-                            key: "_left",
-                            value: function(e) {
-                                var t = e.closest('[role="tablist"]');
-                                if (t) {
-                                    var o = r(t.querySelectorAll(this.selector)).filter((function(e) {
-                                            return !e.disabled
-                                        })).reverse(),
-                                        n = t.querySelector("button:focus"),
-                                        i = o.findIndex((function(e) {
-                                            return e === n
-                                        }));
-                                    i + 1 < o.length ? i++ : i = 0, o[i].focus(), this.open(o[i])
-                                }
-                            }
-                        }, {
-                            key: "_start",
-                            value: function(e) {
-                                var t = e.closest('[role="tablist"]');
-                                if (t) {
-                                    var o = r(t.querySelectorAll(this.selector)).filter((function(e) {
-                                        return !e.disabled
-                                    }));
-                                    o.length && (o[0].focus(), this.open(o[0]))
-                                }
-                            }
-                        }, {
-                            key: "_end",
-                            value: function(e) {
-                                var t = e.closest('[role="tablist"]');
-                                if (t) {
-                                    var o = r(t.querySelectorAll(this.selector)).reverse().filter((function(e) {
-                                        return !e.disabled
-                                    }));
-                                    o.length && (o[0].focus(), this.open(o[0]))
-                                }
-                            }
-                        }]) && a(t.prototype, o), Object.defineProperty(t, "prototype", {
-                            writable: !1
-                        }), f
-                    }(o(765).Z);
-                    window.HSTabs = new u, document.addEventListener("load", window.HSTabs.init())
-                },
-                185: (e, t, o) => {
-                    var n = o(765),
-                        r = o(714);
-
-                    function i(e) {
-                        return i = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
-                            return typeof e
-                        } : function(e) {
-                            return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                        }, i(e)
-                    }
-
-                    function a(e, t) {
-                        for (var o = 0; o < t.length; o++) {
-                            var n = t[o];
-                            n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
-                        }
-                    }
 
-                    function s(e, t) {
-                        return s = Object.setPrototypeOf || function(e, t) {
-                            return e.__proto__ = t, e
-                        }, s(e, t)
-                    }
-
-                    function c(e, t) {
-                        if (t && ("object" === i(t) || "function" == typeof t)) return t;
-                        if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                        return function(e) {
-                            if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-                            return e
-                        }(e)
-                    }
-
-                    function l(e) {
-                        return l = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
-                            return e.__proto__ || Object.getPrototypeOf(e)
-                        }, l(e)
-                    }
-                    var u = function(e) {
-                        ! function(e, t) {
-                            if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
-                            e.prototype = Object.create(t && t.prototype, {
-                                constructor: {
-                                    value: e,
-                                    writable: !0,
-                                    configurable: !0
-                                }
-                            }), Object.defineProperty(e, "prototype", {
-                                writable: !1
-                            }), t && s(e, t)
-                        }(f, e);
-                        var t, o, n, i, u = (n = f, i = function() {
-                            if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
-                            if (Reflect.construct.sham) return !1;
-                            if ("function" == typeof Proxy) return !0;
-                            try {
-                                return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
-                            } catch (e) {
-                                return !1
+                            function C(n) {
+                                return n instanceof R(n).HTMLElement || n instanceof HTMLElement
                             }
-                        }(), function() {
-                            var e, t = l(n);
-                            if (i) {
-                                var o = l(this).constructor;
-                                e = Reflect.construct(t, arguments, o)
-                            } else e = t.apply(this, arguments);
-                            return c(this, e)
-                        });
-
-                        function f() {
-                            return function(e, t) {
-                                if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                            }(this, f), u.call(this, ".hs-tooltip")
-                        }
-                        return t = f, (o = [{
-                            key: "init",
-                            value: function() {
-                                var e = this;
-                                document.addEventListener("click", (function(t) {
-                                    var o = t.target.closest(e.selector);
-                                    o && "focus" === e.getClassProperty(o, "--trigger") && e._focus(o), o && "click" === e.getClassProperty(o, "--trigger") && e._click(o)
-                                })), document.addEventListener("mousemove", (function(t) {
-                                    var o = t.target.closest(e.selector);
-                                    o && "focus" !== e.getClassProperty(o, "--trigger") && "click" !== e.getClassProperty(o, "--trigger") && e._hover(o)
-                                }))
-                            }
-                        }, {
-                            key: "_hover",
-                            value: function(e) {
-                                var t = this;
-                                if (!e.classList.contains("show")) {
-                                    var o = e.querySelector(".hs-tooltip-toggle"),
-                                        n = e.querySelector(".hs-tooltip-content"),
-                                        i = this.getClassProperty(e, "--placement");
-                                    (0, r.fi)(o, n, {
-                                        placement: i || "top",
-                                        strategy: "fixed",
-                                        modifiers: [{
-                                            name: "offset",
-                                            options: {
-                                                offset: [0, 5]
-                                            }
-                                        }]
-                                    }), this.show(e), e.addEventListener("mouseleave", (function o(n) {
-                                        n.toElement.closest(t.selector) && n.toElement.closest(t.selector) == e || (t.hide(e), e.removeEventListener("mouseleave", o, !0))
-                                    }), !0)
-                                }
-                            }
-                        }, {
-                            key: "_focus",
-                            value: function(e) {
-                                var t = this,
-                                    o = e.querySelector(".hs-tooltip-toggle"),
-                                    n = e.querySelector(".hs-tooltip-content"),
-                                    i = this.getClassProperty(e, "--placement"),
-                                    a = this.getClassProperty(e, "--strategy");
-                                (0, r.fi)(o, n, {
-                                    placement: i || "top",
-                                    strategy: a || "fixed",
-                                    modifiers: [{
-                                        name: "offset",
-                                        options: {
-                                            offset: [0, 5]
-                                        }
-                                    }]
-                                }), this.show(e), e.addEventListener("blur", (function o() {
-                                    t.hide(e), e.removeEventListener("blur", o, !0)
-                                }), !0)
-                            }
-                        }, {
-                            key: "_click",
-                            value: function(e) {
-                                var t = this;
-                                if (!e.classList.contains("show")) {
-                                    var o = e.querySelector(".hs-tooltip-toggle"),
-                                        n = e.querySelector(".hs-tooltip-content"),
-                                        i = this.getClassProperty(e, "--placement"),
-                                        a = this.getClassProperty(e, "--strategy");
-                                    (0, r.fi)(o, n, {
-                                        placement: i || "top",
-                                        strategy: a || "fixed",
-                                        modifiers: [{
-                                            name: "offset",
-                                            options: {
-                                                offset: [0, 5]
-                                            }
-                                        }]
-                                    }), this.show(e);
-                                    var s = function o(n) {
-                                        setTimeout((function() {
-                                            t.hide(e), e.removeEventListener("click", o, !0), e.removeEventListener("blur", o, !0)
-                                        }))
+
+                            function $(n) {
+                                return typeof ShadowRoot < "u" && (n instanceof R(n).ShadowRoot || n instanceof ShadowRoot)
+                            }
+                            N.d(it, {
+                                fi: () => Pe
+                            });
+                            var P = Math.max,
+                                x = Math.min,
+                                O = Math.round;
+
+                            function c(n, r) {
+                                r === void 0 && (r = !1);
+                                var i = n.getBoundingClientRect(),
+                                    f = 1,
+                                    w = 1;
+                                if (C(n) && r) {
+                                    var b = n.offsetHeight,
+                                        g = n.offsetWidth;
+                                    g > 0 && (f = O(i.width) / g || 1), b > 0 && (w = O(i.height) / b || 1)
+                                }
+                                return {
+                                    width: i.width / f,
+                                    height: i.height / w,
+                                    top: i.top / w,
+                                    right: i.right / f,
+                                    bottom: i.bottom / w,
+                                    left: i.left / f,
+                                    x: i.left / f,
+                                    y: i.top / w
+                                }
+                            }
+
+                            function a(n) {
+                                var r = R(n);
+                                return {
+                                    scrollLeft: r.pageXOffset,
+                                    scrollTop: r.pageYOffset
+                                }
+                            }
+
+                            function o(n) {
+                                return n ? (n.nodeName || "").toLowerCase() : null
+                            }
+
+                            function y(n) {
+                                return ((B(n) ? n.ownerDocument : n.document) || window.document).documentElement
+                            }
+
+                            function m(n) {
+                                return c(y(n)).left + a(n).scrollLeft
+                            }
+
+                            function h(n) {
+                                return R(n).getComputedStyle(n)
+                            }
+
+                            function u(n) {
+                                var r = h(n),
+                                    i = r.overflow,
+                                    f = r.overflowX,
+                                    w = r.overflowY;
+                                return /auto|scroll|overlay|hidden/.test(i + w + f)
+                            }
+
+                            function t(n, r, i) {
+                                i === void 0 && (i = !1);
+                                var f, w, b = C(r),
+                                    g = C(r) && function(L) {
+                                        var nt = L.getBoundingClientRect(),
+                                            D = O(nt.width) / L.offsetWidth || 1,
+                                            z = O(nt.height) / L.offsetHeight || 1;
+                                        return D !== 1 || z !== 1
+                                    }(r),
+                                    k = y(r),
+                                    j = c(n, g),
+                                    A = {
+                                        scrollLeft: 0,
+                                        scrollTop: 0
+                                    },
+                                    T = {
+                                        x: 0,
+                                        y: 0
                                     };
-                                    e.addEventListener("blur", s, !0), e.addEventListener("click", s, !0)
+                                return (b || !b && !i) && ((o(r) !== "body" || u(k)) && (A = (f = r) !== R(f) && C(f) ? {
+                                    scrollLeft: (w = f).scrollLeft,
+                                    scrollTop: w.scrollTop
+                                } : a(f)), C(r) ? ((T = c(r, !0)).x += r.clientLeft, T.y += r.clientTop) : k && (T.x = m(k))), {
+                                    x: j.left + A.scrollLeft - T.x,
+                                    y: j.top + A.scrollTop - T.y,
+                                    width: j.width,
+                                    height: j.height
                                 }
                             }
-                        }, {
-                            key: "show",
-                            value: function(e) {
-                                var t = this;
-                                e.querySelector(".hs-tooltip-content").classList.remove("hidden"), setTimeout((function() {
-                                    e.classList.add("show"), t._fireEvent("show", e), t._dispatch("show.hs.tooltip", e, e)
-                                }))
-                            }
-                        }, {
-                            key: "hide",
-                            value: function(e) {
-                                var t = e.querySelector(".hs-tooltip-content");
-                                e.classList.remove("show"), this._fireEvent("hide", e), this._dispatch("hide.hs.tooltip", e, e), this.afterTransition(t, (function() {
-                                    e.classList.contains("show") || t.classList.add("hidden")
-                                }))
-                            }
-                        }]) && a(t.prototype, o), Object.defineProperty(t, "prototype", {
-                            writable: !1
-                        }), f
-                    }(n.Z);
-                    window.HSTooltip = new u, document.addEventListener("load", window.HSTooltip.init())
-                },
-                765: (e, t, o) => {
-                    function n(e, t) {
-                        for (var o = 0; o < t.length; o++) {
-                            var n = t[o];
-                            n.enumerable = n.enumerable || !1, n.configurable = !0, "value" in n && (n.writable = !0), Object.defineProperty(e, n.key, n)
-                        }
-                    }
-                    o.d(t, {
-                        Z: () => r
-                    });
-                    var r = function() {
-                        function e(t, o) {
-                            ! function(e, t) {
-                                if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                            }(this, e), this.$collection = [], this.selector = t, this.config = o, this.events = {}
-                        }
-                        var t, o;
-                        return t = e, o = [{
-                            key: "_fireEvent",
-                            value: function(e) {
-                                var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null;
-                                this.events.hasOwnProperty(e) && this.events[e](t)
-                            }
-                        }, {
-                            key: "_dispatch",
-                            value: function(e, t) {
-                                var o = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : null,
-                                    n = new CustomEvent(e, {
-                                        detail: {
-                                            payload: o
-                                        },
-                                        bubbles: !0,
-                                        cancelable: !0,
-                                        composed: !1
-                                    });
-                                t.dispatchEvent(n)
-                            }
-                        }, {
-                            key: "on",
-                            value: function(e, t) {
-                                this.events[e] = t
-                            }
-                        }, {
-                            key: "afterTransition",
-                            value: function(e, t) {
-                                "all 0s ease 0s" !== window.getComputedStyle(e, null).getPropertyValue("transition") ? e.addEventListener("transitionend", (function o() {
-                                    t(), e.removeEventListener("transitionend", o, !0)
-                                }), !0) : t()
-                            }
-                        }, {
-                            key: "getClassProperty",
-                            value: function(e, t) {
-                                var o = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "",
-                                    n = (window.getComputedStyle(e).getPropertyValue(t) || o).replace(" ", "");
-                                return n
+
+                            function e(n) {
+                                var r = c(n),
+                                    i = n.offsetWidth,
+                                    f = n.offsetHeight;
+                                return Math.abs(r.width - i) <= 1 && (i = r.width), Math.abs(r.height - f) <= 1 && (f = r.height), {
+                                    x: n.offsetLeft,
+                                    y: n.offsetTop,
+                                    width: i,
+                                    height: f
+                                }
                             }
-                        }], o && n(t.prototype, o), Object.defineProperty(t, "prototype", {
-                            writable: !1
-                        }), e
-                    }()
-                },
-                714: (e, t, o) => {
-                    function n(e) {
-                        if (null == e) return window;
-                        if ("[object Window]" !== e.toString()) {
-                            var t = e.ownerDocument;
-                            return t && t.defaultView || window
-                        }
-                        return e
-                    }
 
-                    function r(e) {
-                        return e instanceof n(e).Element || e instanceof Element
-                    }
-
-                    function i(e) {
-                        return e instanceof n(e).HTMLElement || e instanceof HTMLElement
-                    }
-
-                    function a(e) {
-                        return "undefined" != typeof ShadowRoot && (e instanceof n(e).ShadowRoot || e instanceof ShadowRoot)
-                    }
-                    o.d(t, {
-                        fi: () => ce
-                    });
-                    var s = Math.max,
-                        c = Math.min,
-                        l = Math.round;
-
-                    function u(e, t) {
-                        void 0 === t && (t = !1);
-                        var o = e.getBoundingClientRect(),
-                            n = 1,
-                            r = 1;
-                        if (i(e) && t) {
-                            var a = e.offsetHeight,
-                                s = e.offsetWidth;
-                            s > 0 && (n = l(o.width) / s || 1), a > 0 && (r = l(o.height) / a || 1)
-                        }
-                        return {
-                            width: o.width / n,
-                            height: o.height / r,
-                            top: o.top / r,
-                            right: o.right / n,
-                            bottom: o.bottom / r,
-                            left: o.left / n,
-                            x: o.left / n,
-                            y: o.top / r
-                        }
-                    }
+                            function s(n) {
+                                return o(n) === "html" ? n : n.assignedSlot || n.parentNode || ($(n) ? n.host : null) || y(n)
+                            }
 
-                    function f(e) {
-                        var t = n(e);
-                        return {
-                            scrollLeft: t.pageXOffset,
-                            scrollTop: t.pageYOffset
-                        }
-                    }
+                            function d(n) {
+                                return ["html", "body", "#document"].indexOf(o(n)) >= 0 ? n.ownerDocument.body : C(n) && u(n) ? n : d(s(n))
+                            }
 
-                    function p(e) {
-                        return e ? (e.nodeName || "").toLowerCase() : null
-                    }
-
-                    function d(e) {
-                        return ((r(e) ? e.ownerDocument : e.document) || window.document).documentElement
-                    }
-
-                    function y(e) {
-                        return u(d(e)).left + f(e).scrollLeft
-                    }
-
-                    function h(e) {
-                        return n(e).getComputedStyle(e)
-                    }
-
-                    function v(e) {
-                        var t = h(e),
-                            o = t.overflow,
-                            n = t.overflowX,
-                            r = t.overflowY;
-                        return /auto|scroll|overlay|hidden/.test(o + r + n)
-                    }
-
-                    function m(e, t, o) {
-                        void 0 === o && (o = !1);
-                        var r, a, s = i(t),
-                            c = i(t) && function(e) {
-                                var t = e.getBoundingClientRect(),
-                                    o = l(t.width) / e.offsetWidth || 1,
-                                    n = l(t.height) / e.offsetHeight || 1;
-                                return 1 !== o || 1 !== n
-                            }(t),
-                            h = d(t),
-                            m = u(e, c),
-                            b = {
-                                scrollLeft: 0,
-                                scrollTop: 0
-                            },
-                            g = {
-                                x: 0,
-                                y: 0
-                            };
-                        return (s || !s && !o) && (("body" !== p(t) || v(h)) && (b = (r = t) !== n(r) && i(r) ? {
-                            scrollLeft: (a = r).scrollLeft,
-                            scrollTop: a.scrollTop
-                        } : f(r)), i(t) ? ((g = u(t, !0)).x += t.clientLeft, g.y += t.clientTop) : h && (g.x = y(h))), {
-                            x: m.left + b.scrollLeft - g.x,
-                            y: m.top + b.scrollTop - g.y,
-                            width: m.width,
-                            height: m.height
-                        }
-                    }
+                            function l(n, r) {
+                                var i;
+                                r === void 0 && (r = []);
+                                var f = d(n),
+                                    w = f === ((i = n.ownerDocument) == null ? void 0 : i.body),
+                                    b = R(f),
+                                    g = w ? [b].concat(b.visualViewport || [], u(f) ? f : []) : f,
+                                    k = r.concat(g);
+                                return w ? k : k.concat(l(s(g)))
+                            }
 
-                    function b(e) {
-                        var t = u(e),
-                            o = e.offsetWidth,
-                            n = e.offsetHeight;
-                        return Math.abs(t.width - o) <= 1 && (o = t.width), Math.abs(t.height - n) <= 1 && (n = t.height), {
-                            x: e.offsetLeft,
-                            y: e.offsetTop,
-                            width: o,
-                            height: n
-                        }
-                    }
+                            function p(n) {
+                                return ["table", "td", "th"].indexOf(o(n)) >= 0
+                            }
+
+                            function v(n) {
+                                return C(n) && h(n).position !== "fixed" ? n.offsetParent : null
+                            }
 
-                    function g(e) {
-                        return "html" === p(e) ? e : e.assignedSlot || e.parentNode || (a(e) ? e.host : null) || d(e)
-                    }
-
-                    function w(e) {
-                        return ["html", "body", "#document"].indexOf(p(e)) >= 0 ? e.ownerDocument.body : i(e) && v(e) ? e : w(g(e))
-                    }
-
-                    function O(e, t) {
-                        var o;
-                        void 0 === t && (t = []);
-                        var r = w(e),
-                            i = r === (null == (o = e.ownerDocument) ? void 0 : o.body),
-                            a = n(r),
-                            s = i ? [a].concat(a.visualViewport || [], v(r) ? r : []) : r,
-                            c = t.concat(s);
-                        return i ? c : c.concat(O(g(s)))
-                    }
-
-                    function S(e) {
-                        return ["table", "td", "th"].indexOf(p(e)) >= 0
-                    }
-
-                    function x(e) {
-                        return i(e) && "fixed" !== h(e).position ? e.offsetParent : null
-                    }
-
-                    function _(e) {
-                        for (var t = n(e), o = x(e); o && S(o) && "static" === h(o).position;) o = x(o);
-                        return o && ("html" === p(o) || "body" === p(o) && "static" === h(o).position) ? t : o || function(e) {
-                            var t = -1 !== navigator.userAgent.toLowerCase().indexOf("firefox");
-                            if (-1 !== navigator.userAgent.indexOf("Trident") && i(e) && "fixed" === h(e).position) return null;
-                            for (var o = g(e); i(o) && ["html", "body"].indexOf(p(o)) < 0;) {
-                                var n = h(o);
-                                if ("none" !== n.transform || "none" !== n.perspective || "paint" === n.contain || -1 !== ["transform", "perspective"].indexOf(n.willChange) || t && "filter" === n.willChange || t && n.filter && "none" !== n.filter) return o;
-                                o = o.parentNode
-                            }
-                            return null
-                        }(e) || t
-                    }
-                    var E = "top",
-                        k = "bottom",
-                        j = "right",
-                        P = "left",
-                        L = "auto",
-                        A = [E, k, j, P],
-                        T = "start",
-                        C = "end",
-                        q = "viewport",
-                        R = "popper",
-                        D = A.reduce((function(e, t) {
-                            return e.concat([t + "-" + T, t + "-" + C])
-                        }), []),
-                        H = [].concat(A, [L]).reduce((function(e, t) {
-                            return e.concat([t, t + "-" + T, t + "-" + C])
-                        }), []),
-                        B = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
-
-                    function I(e) {
-                        var t = new Map,
-                            o = new Set,
-                            n = [];
-
-                        function r(e) {
-                            o.add(e.name), [].concat(e.requires || [], e.requiresIfExists || []).forEach((function(e) {
-                                if (!o.has(e)) {
-                                    var n = t.get(e);
-                                    n && r(n)
+                            function S(n) {
+                                for (var r = R(n), i = v(n); i && p(i) && h(i).position === "static";) i = v(i);
+                                return i && (o(i) === "html" || o(i) === "body" && h(i).position === "static") ? r : i || function(f) {
+                                    var w = navigator.userAgent.toLowerCase().indexOf("firefox") !== -1;
+                                    if (navigator.userAgent.indexOf("Trident") !== -1 && C(f) && h(f).position === "fixed") return null;
+                                    for (var b = s(f); C(b) && ["html", "body"].indexOf(o(b)) < 0;) {
+                                        var g = h(b);
+                                        if (g.transform !== "none" || g.perspective !== "none" || g.contain === "paint" || ["transform", "perspective"].indexOf(g.willChange) !== -1 || w && g.willChange === "filter" || w && g.filter && g.filter !== "none") return b;
+                                        b = b.parentNode
+                                    }
+                                    return null
+                                }(n) || r
+                            }
+                            var E = "top",
+                                _ = "bottom",
+                                et = "right",
+                                U = "left",
+                                kt = "auto",
+                                Et = [E, _, et, U],
+                                wt = "start",
+                                xt = "end",
+                                Ht = "viewport",
+                                rt = "popper",
+                                Bt = Et.reduce(function(n, r) {
+                                    return n.concat([r + "-" + wt, r + "-" + xt])
+                                }, []),
+                                Ot = [].concat(Et, [kt]).reduce(function(n, r) {
+                                    return n.concat([r, r + "-" + wt, r + "-" + xt])
+                                }, []),
+                                Se = ["beforeRead", "read", "afterRead", "beforeMain", "main", "afterMain", "beforeWrite", "write", "afterWrite"];
+
+                            function ke(n) {
+                                var r = new Map,
+                                    i = new Set,
+                                    f = [];
+
+                                function w(b) {
+                                    i.add(b.name), [].concat(b.requires || [], b.requiresIfExists || []).forEach(function(g) {
+                                        if (!i.has(g)) {
+                                            var k = r.get(g);
+                                            k && w(k)
+                                        }
+                                    }), f.push(b)
                                 }
-                            })), n.push(e)
-                        }
-                        return e.forEach((function(e) {
-                            t.set(e.name, e)
-                        })), e.forEach((function(e) {
-                            o.has(e.name) || r(e)
-                        })), n
-                    }
-                    var M = {
-                        placement: "bottom",
-                        modifiers: [],
-                        strategy: "absolute"
-                    };
+                                return n.forEach(function(b) {
+                                    r.set(b.name, b)
+                                }), n.forEach(function(b) {
+                                    i.has(b.name) || w(b)
+                                }), f
+                            }
+                            var re = {
+                                placement: "bottom",
+                                modifiers: [],
+                                strategy: "absolute"
+                            };
 
-                    function V() {
-                        for (var e = arguments.length, t = new Array(e), o = 0; o < e; o++) t[o] = arguments[o];
-                        return !t.some((function(e) {
-                            return !(e && "function" == typeof e.getBoundingClientRect)
-                        }))
-                    }
-
-                    function W(e) {
-                        void 0 === e && (e = {});
-                        var t = e,
-                            o = t.defaultModifiers,
-                            n = void 0 === o ? [] : o,
-                            i = t.defaultOptions,
-                            a = void 0 === i ? M : i;
-                        return function(e, t, o) {
-                            void 0 === o && (o = a);
-                            var i, s, c = {
-                                    placement: "bottom",
-                                    orderedModifiers: [],
-                                    options: Object.assign({}, M, a),
-                                    modifiersData: {},
-                                    elements: {
-                                        reference: e,
-                                        popper: t
-                                    },
-                                    attributes: {},
-                                    styles: {}
-                                },
-                                l = [],
-                                u = !1,
-                                f = {
-                                    state: c,
-                                    setOptions: function(o) {
-                                        var i = "function" == typeof o ? o(c.options) : o;
-                                        p(), c.options = Object.assign({}, a, c.options, i), c.scrollParents = {
-                                            reference: r(e) ? O(e) : e.contextElement ? O(e.contextElement) : [],
-                                            popper: O(t)
-                                        };
-                                        var s, u, d = function(e) {
-                                            var t = I(e);
-                                            return B.reduce((function(e, o) {
-                                                return e.concat(t.filter((function(e) {
-                                                    return e.phase === o
-                                                })))
-                                            }), [])
-                                        }((s = [].concat(n, c.options.modifiers), u = s.reduce((function(e, t) {
-                                            var o = e[t.name];
-                                            return e[t.name] = o ? Object.assign({}, o, t, {
-                                                options: Object.assign({}, o.options, t.options),
-                                                data: Object.assign({}, o.data, t.data)
-                                            }) : t, e
-                                        }), {}), Object.keys(u).map((function(e) {
-                                            return u[e]
-                                        }))));
-                                        return c.orderedModifiers = d.filter((function(e) {
-                                            return e.enabled
-                                        })), c.orderedModifiers.forEach((function(e) {
-                                            var t = e.name,
-                                                o = e.options,
-                                                n = void 0 === o ? {} : o,
-                                                r = e.effect;
-                                            if ("function" == typeof r) {
-                                                var i = r({
-                                                    state: c,
-                                                    name: t,
-                                                    instance: f,
-                                                    options: n
-                                                });
-                                                l.push(i || function() {})
-                                            }
-                                        })), f.update()
-                                    },
-                                    forceUpdate: function() {
-                                        if (!u) {
-                                            var e = c.elements,
-                                                t = e.reference,
-                                                o = e.popper;
-                                            if (V(t, o)) {
-                                                c.rects = {
-                                                    reference: m(t, _(o), "fixed" === c.options.strategy),
-                                                    popper: b(o)
-                                                }, c.reset = !1, c.placement = c.options.placement, c.orderedModifiers.forEach((function(e) {
-                                                    return c.modifiersData[e.name] = Object.assign({}, e.data)
-                                                }));
-                                                for (var n = 0; n < c.orderedModifiers.length; n++)
-                                                    if (!0 !== c.reset) {
-                                                        var r = c.orderedModifiers[n],
-                                                            i = r.fn,
-                                                            a = r.options,
-                                                            s = void 0 === a ? {} : a,
-                                                            l = r.name;
-                                                        "function" == typeof i && (c = i({
-                                                            state: c,
-                                                            options: s,
-                                                            name: l,
-                                                            instance: f
-                                                        }) || c)
-                                                    } else c.reset = !1, n = -1
+                            function ne() {
+                                for (var n = arguments.length, r = new Array(n), i = 0; i < n; i++) r[i] = arguments[i];
+                                return !r.some(function(f) {
+                                    return !(f && typeof f.getBoundingClientRect == "function")
+                                })
+                            }
+
+                            function Ee(n) {
+                                n === void 0 && (n = {});
+                                var r = n,
+                                    i = r.defaultModifiers,
+                                    f = i === void 0 ? [] : i,
+                                    w = r.defaultOptions,
+                                    b = w === void 0 ? re : w;
+                                return function(g, k, j) {
+                                    j === void 0 && (j = b);
+                                    var A, T, L = {
+                                            placement: "bottom",
+                                            orderedModifiers: [],
+                                            options: Object.assign({}, re, b),
+                                            modifiersData: {},
+                                            elements: {
+                                                reference: g,
+                                                popper: k
+                                            },
+                                            attributes: {},
+                                            styles: {}
+                                        },
+                                        nt = [],
+                                        D = !1,
+                                        z = {
+                                            state: L,
+                                            setOptions: function(q) {
+                                                var ot = typeof q == "function" ? q(L.options) : q;
+                                                W(), L.options = Object.assign({}, b, L.options, ot), L.scrollParents = {
+                                                    reference: B(g) ? l(g) : g.contextElement ? l(g.contextElement) : [],
+                                                    popper: l(k)
+                                                };
+                                                var J, M, X = function(H) {
+                                                    var I = ke(H);
+                                                    return Se.reduce(function(V, Z) {
+                                                        return V.concat(I.filter(function(K) {
+                                                            return K.phase === Z
+                                                        }))
+                                                    }, [])
+                                                }((J = [].concat(f, L.options.modifiers), M = J.reduce(function(H, I) {
+                                                    var V = H[I.name];
+                                                    return H[I.name] = V ? Object.assign({}, V, I, {
+                                                        options: Object.assign({}, V.options, I.options),
+                                                        data: Object.assign({}, V.data, I.data)
+                                                    }) : I, H
+                                                }, {}), Object.keys(M).map(function(H) {
+                                                    return M[H]
+                                                })));
+                                                return L.orderedModifiers = X.filter(function(H) {
+                                                    return H.enabled
+                                                }), L.orderedModifiers.forEach(function(H) {
+                                                    var I = H.name,
+                                                        V = H.options,
+                                                        Z = V === void 0 ? {} : V,
+                                                        K = H.effect;
+                                                    if (typeof K == "function") {
+                                                        var st = K({
+                                                            state: L,
+                                                            name: I,
+                                                            instance: z,
+                                                            options: Z
+                                                        });
+                                                        nt.push(st || function() {})
+                                                    }
+                                                }), z.update()
+                                            },
+                                            forceUpdate: function() {
+                                                if (!D) {
+                                                    var q = L.elements,
+                                                        ot = q.reference,
+                                                        J = q.popper;
+                                                    if (ne(ot, J)) {
+                                                        L.rects = {
+                                                            reference: t(ot, S(J), L.options.strategy === "fixed"),
+                                                            popper: e(J)
+                                                        }, L.reset = !1, L.placement = L.options.placement, L.orderedModifiers.forEach(function(K) {
+                                                            return L.modifiersData[K.name] = Object.assign({}, K.data)
+                                                        });
+                                                        for (var M = 0; M < L.orderedModifiers.length; M++)
+                                                            if (L.reset !== !0) {
+                                                                var X = L.orderedModifiers[M],
+                                                                    H = X.fn,
+                                                                    I = X.options,
+                                                                    V = I === void 0 ? {} : I,
+                                                                    Z = X.name;
+                                                                typeof H == "function" && (L = H({
+                                                                    state: L,
+                                                                    options: V,
+                                                                    name: Z,
+                                                                    instance: z
+                                                                }) || L)
+                                                            } else L.reset = !1, M = -1
+                                                    }
+                                                }
+                                            },
+                                            update: (A = function() {
+                                                return new Promise(function(q) {
+                                                    z.forceUpdate(), q(L)
+                                                })
+                                            }, function() {
+                                                return T || (T = new Promise(function(q) {
+                                                    Promise.resolve().then(function() {
+                                                        T = void 0, q(A())
+                                                    })
+                                                })), T
+                                            }),
+                                            destroy: function() {
+                                                W(), D = !0
                                             }
-                                        }
-                                    },
-                                    update: (i = function() {
-                                        return new Promise((function(e) {
-                                            f.forceUpdate(), e(c)
-                                        }))
-                                    }, function() {
-                                        return s || (s = new Promise((function(e) {
-                                            Promise.resolve().then((function() {
-                                                s = void 0, e(i())
-                                            }))
-                                        }))), s
-                                    }),
-                                    destroy: function() {
-                                        p(), u = !0
+                                        };
+                                    if (!ne(g, k)) return z;
+
+                                    function W() {
+                                        nt.forEach(function(q) {
+                                            return q()
+                                        }), nt = []
                                     }
-                                };
-                            if (!V(e, t)) return f;
+                                    return z.setOptions(j).then(function(q) {
+                                        !D && j.onFirstUpdate && j.onFirstUpdate(q)
+                                    }), z
+                                }
+                            }
+                            var $t = {
+                                passive: !0
+                            };
 
-                            function p() {
-                                l.forEach((function(e) {
-                                    return e()
-                                })), l = []
-                            }
-                            return f.setOptions(o).then((function(e) {
-                                !u && o.onFirstUpdate && o.onFirstUpdate(e)
-                            })), f
-                        }
-                    }
-                    var $ = {
-                        passive: !0
-                    };
+                            function bt(n) {
+                                return n.split("-")[0]
+                            }
 
-                    function N(e) {
-                        return e.split("-")[0]
-                    }
-
-                    function Z(e) {
-                        return e.split("-")[1]
-                    }
-
-                    function U(e) {
-                        return ["top", "bottom"].indexOf(e) >= 0 ? "x" : "y"
-                    }
-
-                    function z(e) {
-                        var t, o = e.reference,
-                            n = e.element,
-                            r = e.placement,
-                            i = r ? N(r) : null,
-                            a = r ? Z(r) : null,
-                            s = o.x + o.width / 2 - n.width / 2,
-                            c = o.y + o.height / 2 - n.height / 2;
-                        switch (i) {
-                            case E:
-                                t = {
-                                    x: s,
-                                    y: o.y - n.height
-                                };
-                                break;
-                            case k:
-                                t = {
-                                    x: s,
-                                    y: o.y + o.height
-                                };
-                                break;
-                            case j:
-                                t = {
-                                    x: o.x + o.width,
-                                    y: c
-                                };
-                                break;
-                            case P:
-                                t = {
-                                    x: o.x - n.width,
-                                    y: c
-                                };
-                                break;
-                            default:
-                                t = {
-                                    x: o.x,
-                                    y: o.y
-                                }
-                        }
-                        var l = i ? U(i) : null;
-                        if (null != l) {
-                            var u = "y" === l ? "height" : "width";
-                            switch (a) {
-                                case T:
-                                    t[l] = t[l] - (o[u] / 2 - n[u] / 2);
-                                    break;
-                                case C:
-                                    t[l] = t[l] + (o[u] / 2 - n[u] / 2)
+                            function At(n) {
+                                return n.split("-")[1]
                             }
-                        }
-                        return t
-                    }
-                    var F = {
-                        top: "auto",
-                        right: "auto",
-                        bottom: "auto",
-                        left: "auto"
-                    };
 
-                    function X(e) {
-                        var t, o = e.popper,
-                            r = e.popperRect,
-                            i = e.placement,
-                            a = e.variation,
-                            s = e.offsets,
-                            c = e.position,
-                            u = e.gpuAcceleration,
-                            f = e.adaptive,
-                            p = e.roundOffsets,
-                            y = e.isFixed,
-                            v = s.x,
-                            m = void 0 === v ? 0 : v,
-                            b = s.y,
-                            g = void 0 === b ? 0 : b,
-                            w = "function" == typeof p ? p({
-                                x: m,
-                                y: g
-                            }) : {
-                                x: m,
-                                y: g
-                            };
-                        m = w.x, g = w.y;
-                        var O = s.hasOwnProperty("x"),
-                            S = s.hasOwnProperty("y"),
-                            x = P,
-                            L = E,
-                            A = window;
-                        if (f) {
-                            var T = _(o),
-                                q = "clientHeight",
-                                R = "clientWidth";
-                            T === n(o) && "static" !== h(T = d(o)).position && "absolute" === c && (q = "scrollHeight", R = "scrollWidth"), T = T, (i === E || (i === P || i === j) && a === C) && (L = k, g -= (y && A.visualViewport ? A.visualViewport.height : T[q]) - r.height, g *= u ? 1 : -1), i !== P && (i !== E && i !== k || a !== C) || (x = j, m -= (y && A.visualViewport ? A.visualViewport.width : T[R]) - r.width, m *= u ? 1 : -1)
-                        }
-                        var D, H = Object.assign({
-                                position: c
-                            }, f && F),
-                            B = !0 === p ? function(e) {
-                                var t = e.x,
-                                    o = e.y,
-                                    n = window.devicePixelRatio || 1;
-                                return {
-                                    x: l(t * n) / n || 0,
-                                    y: l(o * n) / n || 0
+                            function Yt(n) {
+                                return ["top", "bottom"].indexOf(n) >= 0 ? "x" : "y"
+                            }
+
+                            function oe(n) {
+                                var r, i = n.reference,
+                                    f = n.element,
+                                    w = n.placement,
+                                    b = w ? bt(w) : null,
+                                    g = w ? At(w) : null,
+                                    k = i.x + i.width / 2 - f.width / 2,
+                                    j = i.y + i.height / 2 - f.height / 2;
+                                switch (b) {
+                                    case E:
+                                        r = {
+                                            x: k,
+                                            y: i.y - f.height
+                                        };
+                                        break;
+                                    case _:
+                                        r = {
+                                            x: k,
+                                            y: i.y + i.height
+                                        };
+                                        break;
+                                    case et:
+                                        r = {
+                                            x: i.x + i.width,
+                                            y: j
+                                        };
+                                        break;
+                                    case U:
+                                        r = {
+                                            x: i.x - f.width,
+                                            y: j
+                                        };
+                                        break;
+                                    default:
+                                        r = {
+                                            x: i.x,
+                                            y: i.y
+                                        }
+                                }
+                                var A = b ? Yt(b) : null;
+                                if (A != null) {
+                                    var T = A === "y" ? "height" : "width";
+                                    switch (g) {
+                                        case wt:
+                                            r[A] = r[A] - (i[T] / 2 - f[T] / 2);
+                                            break;
+                                        case xt:
+                                            r[A] = r[A] + (i[T] / 2 - f[T] / 2)
+                                    }
                                 }
-                            }({
-                                x: m,
-                                y: g
-                            }) : {
-                                x: m,
-                                y: g
+                                return r
+                            }
+                            var xe = {
+                                top: "auto",
+                                right: "auto",
+                                bottom: "auto",
+                                left: "auto"
                             };
-                        return m = B.x, g = B.y, u ? Object.assign({}, H, ((D = {})[L] = S ? "0" : "", D[x] = O ? "0" : "", D.transform = (A.devicePixelRatio || 1) <= 1 ? "translate(" + m + "px, " + g + "px)" : "translate3d(" + m + "px, " + g + "px, 0)", D)) : Object.assign({}, H, ((t = {})[L] = S ? g + "px" : "", t[x] = O ? m + "px" : "", t.transform = "", t))
-                    }
-                    var Y = {
-                        left: "right",
-                        right: "left",
-                        bottom: "top",
-                        top: "bottom"
-                    };
 
-                    function G(e) {
-                        return e.replace(/left|right|bottom|top/g, (function(e) {
-                            return Y[e]
-                        }))
-                    }
-                    var J = {
-                        start: "end",
-                        end: "start"
-                    };
+                            function ie(n) {
+                                var r, i = n.popper,
+                                    f = n.popperRect,
+                                    w = n.placement,
+                                    b = n.variation,
+                                    g = n.offsets,
+                                    k = n.position,
+                                    j = n.gpuAcceleration,
+                                    A = n.adaptive,
+                                    T = n.roundOffsets,
+                                    L = n.isFixed,
+                                    nt = g.x,
+                                    D = nt === void 0 ? 0 : nt,
+                                    z = g.y,
+                                    W = z === void 0 ? 0 : z,
+                                    q = typeof T == "function" ? T({
+                                        x: D,
+                                        y: W
+                                    }) : {
+                                        x: D,
+                                        y: W
+                                    };
+                                D = q.x, W = q.y;
+                                var ot = g.hasOwnProperty("x"),
+                                    J = g.hasOwnProperty("y"),
+                                    M = U,
+                                    X = E,
+                                    H = window;
+                                if (A) {
+                                    var I = S(i),
+                                        V = "clientHeight",
+                                        Z = "clientWidth";
+                                    I === R(i) && h(I = y(i)).position !== "static" && k === "absolute" && (V = "scrollHeight", Z = "scrollWidth"), I = I, (w === E || (w === U || w === et) && b === xt) && (X = _, W -= (L && H.visualViewport ? H.visualViewport.height : I[V]) - f.height, W *= j ? 1 : -1), w !== U && (w !== E && w !== _ || b !== xt) || (M = et, D -= (L && H.visualViewport ? H.visualViewport.width : I[Z]) - f.width, D *= j ? 1 : -1)
+                                }
+                                var K, st = Object.assign({
+                                        position: k
+                                    }, A && xe),
+                                    ct = T === !0 ? function(ft) {
+                                        var yt = ft.x,
+                                            St = ft.y,
+                                            pt = window.devicePixelRatio || 1;
+                                        return {
+                                            x: O(yt * pt) / pt || 0,
+                                            y: O(St * pt) / pt || 0
+                                        }
+                                    }({
+                                        x: D,
+                                        y: W
+                                    }) : {
+                                        x: D,
+                                        y: W
+                                    };
+                                return D = ct.x, W = ct.y, j ? Object.assign({}, st, ((K = {})[X] = J ? "0" : "", K[M] = ot ? "0" : "", K.transform = (H.devicePixelRatio || 1) <= 1 ? "translate(" + D + "px, " + W + "px)" : "translate3d(" + D + "px, " + W + "px, 0)", K)) : Object.assign({}, st, ((r = {})[X] = J ? W + "px" : "", r[M] = ot ? D + "px" : "", r.transform = "", r))
+                            }
+                            var _e = {
+                                left: "right",
+                                right: "left",
+                                bottom: "top",
+                                top: "bottom"
+                            };
 
-                    function K(e) {
-                        return e.replace(/start|end/g, (function(e) {
-                            return J[e]
-                        }))
-                    }
-
-                    function Q(e, t) {
-                        var o = t.getRootNode && t.getRootNode();
-                        if (e.contains(t)) return !0;
-                        if (o && a(o)) {
-                            var n = t;
-                            do {
-                                if (n && e.isSameNode(n)) return !0;
-                                n = n.parentNode || n.host
-                            } while (n)
-                        }
-                        return !1
-                    }
+                            function Nt(n) {
+                                return n.replace(/left|right|bottom|top/g, function(r) {
+                                    return _e[r]
+                                })
+                            }
+                            var je = {
+                                start: "end",
+                                end: "start"
+                            };
 
-                    function ee(e) {
-                        return Object.assign({}, e, {
-                            left: e.x,
-                            top: e.y,
-                            right: e.x + e.width,
-                            bottom: e.y + e.height
-                        })
-                    }
-
-                    function te(e, t) {
-                        return t === q ? ee(function(e) {
-                            var t = n(e),
-                                o = d(e),
-                                r = t.visualViewport,
-                                i = o.clientWidth,
-                                a = o.clientHeight,
-                                s = 0,
-                                c = 0;
-                            return r && (i = r.width, a = r.height, /^((?!chrome|android).)*safari/i.test(navigator.userAgent) || (s = r.offsetLeft, c = r.offsetTop)), {
-                                width: i,
-                                height: a,
-                                x: s + y(e),
-                                y: c
-                            }
-                        }(e)) : r(t) ? function(e) {
-                            var t = u(e);
-                            return t.top = t.top + e.clientTop, t.left = t.left + e.clientLeft, t.bottom = t.top + e.clientHeight, t.right = t.left + e.clientWidth, t.width = e.clientWidth, t.height = e.clientHeight, t.x = t.left, t.y = t.top, t
-                        }(t) : ee(function(e) {
-                            var t, o = d(e),
-                                n = f(e),
-                                r = null == (t = e.ownerDocument) ? void 0 : t.body,
-                                i = s(o.scrollWidth, o.clientWidth, r ? r.scrollWidth : 0, r ? r.clientWidth : 0),
-                                a = s(o.scrollHeight, o.clientHeight, r ? r.scrollHeight : 0, r ? r.clientHeight : 0),
-                                c = -n.scrollLeft + y(e),
-                                l = -n.scrollTop;
-                            return "rtl" === h(r || o).direction && (c += s(o.clientWidth, r ? r.clientWidth : 0) - i), {
-                                width: i,
-                                height: a,
-                                x: c,
-                                y: l
-                            }
-                        }(d(e)))
-                    }
-
-                    function oe(e) {
-                        return Object.assign({}, {
-                            top: 0,
-                            right: 0,
-                            bottom: 0,
-                            left: 0
-                        }, e)
-                    }
-
-                    function ne(e, t) {
-                        return t.reduce((function(t, o) {
-                            return t[o] = e, t
-                        }), {})
-                    }
-
-                    function re(e, t) {
-                        void 0 === t && (t = {});
-                        var o = t,
-                            n = o.placement,
-                            a = void 0 === n ? e.placement : n,
-                            l = o.boundary,
-                            f = void 0 === l ? "clippingParents" : l,
-                            y = o.rootBoundary,
-                            v = void 0 === y ? q : y,
-                            m = o.elementContext,
-                            b = void 0 === m ? R : m,
-                            w = o.altBoundary,
-                            S = void 0 !== w && w,
-                            x = o.padding,
-                            P = void 0 === x ? 0 : x,
-                            L = oe("number" != typeof P ? P : ne(P, A)),
-                            T = b === R ? "reference" : R,
-                            C = e.rects.popper,
-                            D = e.elements[S ? T : b],
-                            H = function(e, t, o) {
-                                var n = "clippingParents" === t ? function(e) {
-                                        var t = O(g(e)),
-                                            o = ["absolute", "fixed"].indexOf(h(e).position) >= 0 && i(e) ? _(e) : e;
-                                        return r(o) ? t.filter((function(e) {
-                                            return r(e) && Q(e, o) && "body" !== p(e)
-                                        })) : []
-                                    }(e) : [].concat(t),
-                                    a = [].concat(n, [o]),
-                                    l = a[0],
-                                    u = a.reduce((function(t, o) {
-                                        var n = te(e, o);
-                                        return t.top = s(n.top, t.top), t.right = c(n.right, t.right), t.bottom = c(n.bottom, t.bottom), t.left = s(n.left, t.left), t
-                                    }), te(e, l));
-                                return u.width = u.right - u.left, u.height = u.bottom - u.top, u.x = u.left, u.y = u.top, u
-                            }(r(D) ? D : D.contextElement || d(e.elements.popper), f, v),
-                            B = u(e.elements.reference),
-                            I = z({
-                                reference: B,
-                                element: C,
-                                strategy: "absolute",
-                                placement: a
-                            }),
-                            M = ee(Object.assign({}, C, I)),
-                            V = b === R ? M : B,
-                            W = {
-                                top: H.top - V.top + L.top,
-                                bottom: V.bottom - H.bottom + L.bottom,
-                                left: H.left - V.left + L.left,
-                                right: V.right - H.right + L.right
-                            },
-                            $ = e.modifiersData.offset;
-                        if (b === R && $) {
-                            var N = $[a];
-                            Object.keys(W).forEach((function(e) {
-                                var t = [j, k].indexOf(e) >= 0 ? 1 : -1,
-                                    o = [E, k].indexOf(e) >= 0 ? "y" : "x";
-                                W[e] += N[o] * t
-                            }))
-                        }
-                        return W
-                    }
+                            function ae(n) {
+                                return n.replace(/start|end/g, function(r) {
+                                    return je[r]
+                                })
+                            }
 
-                    function ie(e, t, o) {
-                        return s(e, c(t, o))
-                    }
-
-                    function ae(e, t, o) {
-                        return void 0 === o && (o = {
-                            x: 0,
-                            y: 0
-                        }), {
-                            top: e.top - t.height - o.y,
-                            right: e.right - t.width + o.x,
-                            bottom: e.bottom - t.height + o.y,
-                            left: e.left - t.width - o.x
-                        }
-                    }
+                            function se(n, r) {
+                                var i = r.getRootNode && r.getRootNode();
+                                if (n.contains(r)) return !0;
+                                if (i && $(i)) {
+                                    var f = r;
+                                    do {
+                                        if (f && n.isSameNode(f)) return !0;
+                                        f = f.parentNode || f.host
+                                    } while (f)
+                                }
+                                return !1
+                            }
 
-                    function se(e) {
-                        return [E, j, k, P].some((function(t) {
-                            return e[t] >= 0
-                        }))
-                    }
-                    var ce = W({
-                        defaultModifiers: [{
-                            name: "eventListeners",
-                            enabled: !0,
-                            phase: "write",
-                            fn: function() {},
-                            effect: function(e) {
-                                var t = e.state,
-                                    o = e.instance,
-                                    r = e.options,
-                                    i = r.scroll,
-                                    a = void 0 === i || i,
-                                    s = r.resize,
-                                    c = void 0 === s || s,
-                                    l = n(t.elements.popper),
-                                    u = [].concat(t.scrollParents.reference, t.scrollParents.popper);
-                                return a && u.forEach((function(e) {
-                                        e.addEventListener("scroll", o.update, $)
-                                    })), c && l.addEventListener("resize", o.update, $),
-                                    function() {
-                                        a && u.forEach((function(e) {
-                                            e.removeEventListener("scroll", o.update, $)
-                                        })), c && l.removeEventListener("resize", o.update, $)
-                                    }
-                            },
-                            data: {}
-                        }, {
-                            name: "popperOffsets",
-                            enabled: !0,
-                            phase: "read",
-                            fn: function(e) {
-                                var t = e.state,
-                                    o = e.name;
-                                t.modifiersData[o] = z({
-                                    reference: t.rects.reference,
-                                    element: t.rects.popper,
-                                    strategy: "absolute",
-                                    placement: t.placement
+                            function Xt(n) {
+                                return Object.assign({}, n, {
+                                    left: n.x,
+                                    top: n.y,
+                                    right: n.x + n.width,
+                                    bottom: n.y + n.height
                                 })
-                            },
-                            data: {}
-                        }, {
-                            name: "computeStyles",
-                            enabled: !0,
-                            phase: "beforeWrite",
-                            fn: function(e) {
-                                var t = e.state,
-                                    o = e.options,
-                                    n = o.gpuAcceleration,
-                                    r = void 0 === n || n,
-                                    i = o.adaptive,
-                                    a = void 0 === i || i,
-                                    s = o.roundOffsets,
-                                    c = void 0 === s || s,
-                                    l = {
-                                        placement: N(t.placement),
-                                        variation: Z(t.placement),
-                                        popper: t.elements.popper,
-                                        popperRect: t.rects.popper,
-                                        gpuAcceleration: r,
-                                        isFixed: "fixed" === t.options.strategy
-                                    };
-                                null != t.modifiersData.popperOffsets && (t.styles.popper = Object.assign({}, t.styles.popper, X(Object.assign({}, l, {
-                                    offsets: t.modifiersData.popperOffsets,
-                                    position: t.options.strategy,
-                                    adaptive: a,
-                                    roundOffsets: c
-                                })))), null != t.modifiersData.arrow && (t.styles.arrow = Object.assign({}, t.styles.arrow, X(Object.assign({}, l, {
-                                    offsets: t.modifiersData.arrow,
-                                    position: "absolute",
-                                    adaptive: !1,
-                                    roundOffsets: c
-                                })))), t.attributes.popper = Object.assign({}, t.attributes.popper, {
-                                    "data-popper-placement": t.placement
-                                })
-                            },
-                            data: {}
-                        }, {
-                            name: "applyStyles",
-                            enabled: !0,
-                            phase: "write",
-                            fn: function(e) {
-                                var t = e.state;
-                                Object.keys(t.elements).forEach((function(e) {
-                                    var o = t.styles[e] || {},
-                                        n = t.attributes[e] || {},
-                                        r = t.elements[e];
-                                    i(r) && p(r) && (Object.assign(r.style, o), Object.keys(n).forEach((function(e) {
-                                        var t = n[e];
-                                        !1 === t ? r.removeAttribute(e) : r.setAttribute(e, !0 === t ? "" : t)
-                                    })))
-                                }))
-                            },
-                            effect: function(e) {
-                                var t = e.state,
-                                    o = {
-                                        popper: {
-                                            position: t.options.strategy,
-                                            left: "0",
-                                            top: "0",
-                                            margin: "0"
-                                        },
-                                        arrow: {
-                                            position: "absolute"
-                                        },
-                                        reference: {}
-                                    };
-                                return Object.assign(t.elements.popper.style, o.popper), t.styles = o, t.elements.arrow && Object.assign(t.elements.arrow.style, o.arrow),
-                                    function() {
-                                        Object.keys(t.elements).forEach((function(e) {
-                                            var n = t.elements[e],
-                                                r = t.attributes[e] || {},
-                                                a = Object.keys(t.styles.hasOwnProperty(e) ? t.styles[e] : o[e]).reduce((function(e, t) {
-                                                    return e[t] = "", e
-                                                }), {});
-                                            i(n) && p(n) && (Object.assign(n.style, a), Object.keys(r).forEach((function(e) {
-                                                n.removeAttribute(e)
-                                            })))
-                                        }))
+                            }
+
+                            function ce(n, r) {
+                                return r === Ht ? Xt(function(i) {
+                                    var f = R(i),
+                                        w = y(i),
+                                        b = f.visualViewport,
+                                        g = w.clientWidth,
+                                        k = w.clientHeight,
+                                        j = 0,
+                                        A = 0;
+                                    return b && (g = b.width, k = b.height, /^((?!chrome|android).)*safari/i.test(navigator.userAgent) || (j = b.offsetLeft, A = b.offsetTop)), {
+                                        width: g,
+                                        height: k,
+                                        x: j + m(i),
+                                        y: A
                                     }
-                            },
-                            requires: ["computeStyles"]
-                        }, {
-                            name: "offset",
-                            enabled: !0,
-                            phase: "main",
-                            requires: ["popperOffsets"],
-                            fn: function(e) {
-                                var t = e.state,
-                                    o = e.options,
-                                    n = e.name,
-                                    r = o.offset,
-                                    i = void 0 === r ? [0, 0] : r,
-                                    a = H.reduce((function(e, o) {
-                                        return e[o] = function(e, t, o) {
-                                            var n = N(e),
-                                                r = [P, E].indexOf(n) >= 0 ? -1 : 1,
-                                                i = "function" == typeof o ? o(Object.assign({}, t, {
-                                                    placement: e
-                                                })) : o,
-                                                a = i[0],
-                                                s = i[1];
-                                            return a = a || 0, s = (s || 0) * r, [P, j].indexOf(n) >= 0 ? {
-                                                x: s,
-                                                y: a
-                                            } : {
-                                                x: a,
-                                                y: s
-                                            }
-                                        }(o, t.rects, i), e
-                                    }), {}),
-                                    s = a[t.placement],
-                                    c = s.x,
-                                    l = s.y;
-                                null != t.modifiersData.popperOffsets && (t.modifiersData.popperOffsets.x += c, t.modifiersData.popperOffsets.y += l), t.modifiersData[n] = a
-                            }
-                        }, {
-                            name: "flip",
-                            enabled: !0,
-                            phase: "main",
-                            fn: function(e) {
-                                var t = e.state,
-                                    o = e.options,
-                                    n = e.name;
-                                if (!t.modifiersData[n]._skip) {
-                                    for (var r = o.mainAxis, i = void 0 === r || r, a = o.altAxis, s = void 0 === a || a, c = o.fallbackPlacements, l = o.padding, u = o.boundary, f = o.rootBoundary, p = o.altBoundary, d = o.flipVariations, y = void 0 === d || d, h = o.allowedAutoPlacements, v = t.options.placement, m = N(v), b = c || (m !== v && y ? function(e) {
-                                            if (N(e) === L) return [];
-                                            var t = G(e);
-                                            return [K(e), t, K(t)]
-                                        }(v) : [G(v)]), g = [v].concat(b).reduce((function(e, o) {
-                                            return e.concat(N(o) === L ? function(e, t) {
-                                                void 0 === t && (t = {});
-                                                var o = t,
-                                                    n = o.placement,
-                                                    r = o.boundary,
-                                                    i = o.rootBoundary,
-                                                    a = o.padding,
-                                                    s = o.flipVariations,
-                                                    c = o.allowedAutoPlacements,
-                                                    l = void 0 === c ? H : c,
-                                                    u = Z(n),
-                                                    f = u ? s ? D : D.filter((function(e) {
-                                                        return Z(e) === u
-                                                    })) : A,
-                                                    p = f.filter((function(e) {
-                                                        return l.indexOf(e) >= 0
-                                                    }));
-                                                0 === p.length && (p = f);
-                                                var d = p.reduce((function(t, o) {
-                                                    return t[o] = re(e, {
-                                                        placement: o,
-                                                        boundary: r,
-                                                        rootBoundary: i,
-                                                        padding: a
-                                                    })[N(o)], t
-                                                }), {});
-                                                return Object.keys(d).sort((function(e, t) {
-                                                    return d[e] - d[t]
-                                                }))
-                                            }(t, {
-                                                placement: o,
-                                                boundary: u,
-                                                rootBoundary: f,
-                                                padding: l,
-                                                flipVariations: y,
-                                                allowedAutoPlacements: h
-                                            }) : o)
-                                        }), []), w = t.rects.reference, O = t.rects.popper, S = new Map, x = !0, _ = g[0], C = 0; C < g.length; C++) {
-                                        var q = g[C],
-                                            R = N(q),
-                                            B = Z(q) === T,
-                                            I = [E, k].indexOf(R) >= 0,
-                                            M = I ? "width" : "height",
-                                            V = re(t, {
-                                                placement: q,
-                                                boundary: u,
-                                                rootBoundary: f,
-                                                altBoundary: p,
-                                                padding: l
-                                            }),
-                                            W = I ? B ? j : P : B ? k : E;
-                                        w[M] > O[M] && (W = G(W));
-                                        var $ = G(W),
-                                            U = [];
-                                        if (i && U.push(V[R] <= 0), s && U.push(V[W] <= 0, V[$] <= 0), U.every((function(e) {
-                                                return e
-                                            }))) {
-                                            _ = q, x = !1;
-                                            break
-                                        }
-                                        S.set(q, U)
-                                    }
-                                    if (x)
-                                        for (var z = function(e) {
-                                                var t = g.find((function(t) {
-                                                    var o = S.get(t);
-                                                    if (o) return o.slice(0, e).every((function(e) {
-                                                        return e
-                                                    }))
-                                                }));
-                                                if (t) return _ = t, "break"
-                                            }, F = y ? 3 : 1; F > 0 && "break" !== z(F); F--);
-                                    t.placement !== _ && (t.modifiersData[n]._skip = !0, t.placement = _, t.reset = !0)
-                                }
-                            },
-                            requiresIfExists: ["offset"],
-                            data: {
-                                _skip: !1
-                            }
-                        }, {
-                            name: "preventOverflow",
-                            enabled: !0,
-                            phase: "main",
-                            fn: function(e) {
-                                var t = e.state,
-                                    o = e.options,
-                                    n = e.name,
-                                    r = o.mainAxis,
-                                    i = void 0 === r || r,
-                                    a = o.altAxis,
-                                    l = void 0 !== a && a,
-                                    u = o.boundary,
-                                    f = o.rootBoundary,
-                                    p = o.altBoundary,
-                                    d = o.padding,
-                                    y = o.tether,
-                                    h = void 0 === y || y,
-                                    v = o.tetherOffset,
-                                    m = void 0 === v ? 0 : v,
-                                    g = re(t, {
-                                        boundary: u,
-                                        rootBoundary: f,
-                                        padding: d,
-                                        altBoundary: p
-                                    }),
-                                    w = N(t.placement),
-                                    O = Z(t.placement),
-                                    S = !O,
-                                    x = U(w),
-                                    L = "x" === x ? "y" : "x",
-                                    A = t.modifiersData.popperOffsets,
-                                    C = t.rects.reference,
-                                    q = t.rects.popper,
-                                    R = "function" == typeof m ? m(Object.assign({}, t.rects, {
-                                        placement: t.placement
-                                    })) : m,
-                                    D = "number" == typeof R ? {
-                                        mainAxis: R,
-                                        altAxis: R
-                                    } : Object.assign({
-                                        mainAxis: 0,
-                                        altAxis: 0
-                                    }, R),
-                                    H = t.modifiersData.offset ? t.modifiersData.offset[t.placement] : null,
-                                    B = {
-                                        x: 0,
-                                        y: 0
-                                    };
-                                if (A) {
-                                    if (i) {
-                                        var I, M = "y" === x ? E : P,
-                                            V = "y" === x ? k : j,
-                                            W = "y" === x ? "height" : "width",
-                                            $ = A[x],
-                                            z = $ + g[M],
-                                            F = $ - g[V],
-                                            X = h ? -q[W] / 2 : 0,
-                                            Y = O === T ? C[W] : q[W],
-                                            G = O === T ? -q[W] : -C[W],
-                                            J = t.elements.arrow,
-                                            K = h && J ? b(J) : {
-                                                width: 0,
-                                                height: 0
-                                            },
-                                            Q = t.modifiersData["arrow#persistent"] ? t.modifiersData["arrow#persistent"].padding : {
-                                                top: 0,
-                                                right: 0,
-                                                bottom: 0,
-                                                left: 0
-                                            },
-                                            ee = Q[M],
-                                            te = Q[V],
-                                            oe = ie(0, C[W], K[W]),
-                                            ne = S ? C[W] / 2 - X - oe - ee - D.mainAxis : Y - oe - ee - D.mainAxis,
-                                            ae = S ? -C[W] / 2 + X + oe + te + D.mainAxis : G + oe + te + D.mainAxis,
-                                            se = t.elements.arrow && _(t.elements.arrow),
-                                            ce = se ? "y" === x ? se.clientTop || 0 : se.clientLeft || 0 : 0,
-                                            le = null != (I = null == H ? void 0 : H[x]) ? I : 0,
-                                            ue = $ + ae - le,
-                                            fe = ie(h ? c(z, $ + ne - le - ce) : z, $, h ? s(F, ue) : F);
-                                        A[x] = fe, B[x] = fe - $
-                                    }
-                                    if (l) {
-                                        var pe, de = "x" === x ? E : P,
-                                            ye = "x" === x ? k : j,
-                                            he = A[L],
-                                            ve = "y" === L ? "height" : "width",
-                                            me = he + g[de],
-                                            be = he - g[ye],
-                                            ge = -1 !== [E, P].indexOf(w),
-                                            we = null != (pe = null == H ? void 0 : H[L]) ? pe : 0,
-                                            Oe = ge ? me : he - C[ve] - q[ve] - we + D.altAxis,
-                                            Se = ge ? he + C[ve] + q[ve] - we - D.altAxis : be,
-                                            xe = h && ge ? function(e, t, o) {
-                                                var n = ie(e, t, o);
-                                                return n > o ? o : n
-                                            }(Oe, he, Se) : ie(h ? Oe : me, he, h ? Se : be);
-                                        A[L] = xe, B[L] = xe - he
-                                    }
-                                    t.modifiersData[n] = B
-                                }
-                            },
-                            requiresIfExists: ["offset"]
-                        }, {
-                            name: "arrow",
-                            enabled: !0,
-                            phase: "main",
-                            fn: function(e) {
-                                var t, o = e.state,
-                                    n = e.name,
-                                    r = e.options,
-                                    i = o.elements.arrow,
-                                    a = o.modifiersData.popperOffsets,
-                                    s = N(o.placement),
-                                    c = U(s),
-                                    l = [P, j].indexOf(s) >= 0 ? "height" : "width";
-                                if (i && a) {
-                                    var u = function(e, t) {
-                                            return oe("number" != typeof(e = "function" == typeof e ? e(Object.assign({}, t.rects, {
-                                                placement: t.placement
-                                            })) : e) ? e : ne(e, A))
-                                        }(r.padding, o),
-                                        f = b(i),
-                                        p = "y" === c ? E : P,
-                                        d = "y" === c ? k : j,
-                                        y = o.rects.reference[l] + o.rects.reference[c] - a[c] - o.rects.popper[l],
-                                        h = a[c] - o.rects.reference[c],
-                                        v = _(i),
-                                        m = v ? "y" === c ? v.clientHeight || 0 : v.clientWidth || 0 : 0,
-                                        g = y / 2 - h / 2,
-                                        w = u[p],
-                                        O = m - f[l] - u[d],
-                                        S = m / 2 - f[l] / 2 + g,
-                                        x = ie(w, S, O),
-                                        L = c;
-                                    o.modifiersData[n] = ((t = {})[L] = x, t.centerOffset = x - S, t)
-                                }
-                            },
-                            effect: function(e) {
-                                var t = e.state,
-                                    o = e.options.element,
-                                    n = void 0 === o ? "[data-popper-arrow]" : o;
-                                null != n && ("string" != typeof n || (n = t.elements.popper.querySelector(n))) && Q(t.elements.popper, n) && (t.elements.arrow = n)
-                            },
-                            requires: ["popperOffsets"],
-                            requiresIfExists: ["preventOverflow"]
-                        }, {
-                            name: "hide",
-                            enabled: !0,
-                            phase: "main",
-                            requiresIfExists: ["preventOverflow"],
-                            fn: function(e) {
-                                var t = e.state,
-                                    o = e.name,
-                                    n = t.rects.reference,
-                                    r = t.rects.popper,
-                                    i = t.modifiersData.preventOverflow,
-                                    a = re(t, {
-                                        elementContext: "reference"
-                                    }),
-                                    s = re(t, {
-                                        altBoundary: !0
+                                }(n)) : B(r) ? function(i) {
+                                    var f = c(i);
+                                    return f.top = f.top + i.clientTop, f.left = f.left + i.clientLeft, f.bottom = f.top + i.clientHeight, f.right = f.left + i.clientWidth, f.width = i.clientWidth, f.height = i.clientHeight, f.x = f.left, f.y = f.top, f
+                                }(r) : Xt(function(i) {
+                                    var f, w = y(i),
+                                        b = a(i),
+                                        g = (f = i.ownerDocument) == null ? void 0 : f.body,
+                                        k = P(w.scrollWidth, w.clientWidth, g ? g.scrollWidth : 0, g ? g.clientWidth : 0),
+                                        j = P(w.scrollHeight, w.clientHeight, g ? g.scrollHeight : 0, g ? g.clientHeight : 0),
+                                        A = -b.scrollLeft + m(i),
+                                        T = -b.scrollTop;
+                                    return h(g || w).direction === "rtl" && (A += P(w.clientWidth, g ? g.clientWidth : 0) - k), {
+                                        width: k,
+                                        height: j,
+                                        x: A,
+                                        y: T
+                                    }
+                                }(y(n)))
+                            }
+
+                            function le(n) {
+                                return Object.assign({}, {
+                                    top: 0,
+                                    right: 0,
+                                    bottom: 0,
+                                    left: 0
+                                }, n)
+                            }
+
+                            function ue(n, r) {
+                                return r.reduce(function(i, f) {
+                                    return i[f] = n, i
+                                }, {})
+                            }
+
+                            function It(n, r) {
+                                r === void 0 && (r = {});
+                                var i = r,
+                                    f = i.placement,
+                                    w = f === void 0 ? n.placement : f,
+                                    b = i.boundary,
+                                    g = b === void 0 ? "clippingParents" : b,
+                                    k = i.rootBoundary,
+                                    j = k === void 0 ? Ht : k,
+                                    A = i.elementContext,
+                                    T = A === void 0 ? rt : A,
+                                    L = i.altBoundary,
+                                    nt = L !== void 0 && L,
+                                    D = i.padding,
+                                    z = D === void 0 ? 0 : D,
+                                    W = le(typeof z != "number" ? z : ue(z, Et)),
+                                    q = T === rt ? "reference" : rt,
+                                    ot = n.rects.popper,
+                                    J = n.elements[nt ? q : T],
+                                    M = function(ct, ft, yt) {
+                                        var St = ft === "clippingParents" ? function(tt) {
+                                                var _t = l(s(tt)),
+                                                    dt = ["absolute", "fixed"].indexOf(h(tt).position) >= 0 && C(tt) ? S(tt) : tt;
+                                                return B(dt) ? _t.filter(function(ut) {
+                                                    return B(ut) && se(ut, dt) && o(ut) !== "body"
+                                                }) : []
+                                            }(ct) : [].concat(ft),
+                                            pt = [].concat(St, [yt]),
+                                            lt = pt[0],
+                                            at = pt.reduce(function(tt, _t) {
+                                                var dt = ce(ct, _t);
+                                                return tt.top = P(dt.top, tt.top), tt.right = x(dt.right, tt.right), tt.bottom = x(dt.bottom, tt.bottom), tt.left = P(dt.left, tt.left), tt
+                                            }, ce(ct, lt));
+                                        return at.width = at.right - at.left, at.height = at.bottom - at.top, at.x = at.left, at.y = at.top, at
+                                    }(B(J) ? J : J.contextElement || y(n.elements.popper), g, j),
+                                    X = c(n.elements.reference),
+                                    H = oe({
+                                        reference: X,
+                                        element: ot,
+                                        strategy: "absolute",
+                                        placement: w
                                     }),
-                                    c = ae(a, n),
-                                    l = ae(s, r, i),
-                                    u = se(c),
-                                    f = se(l);
-                                t.modifiersData[o] = {
-                                    referenceClippingOffsets: c,
-                                    popperEscapeOffsets: l,
-                                    isReferenceHidden: u,
-                                    hasPopperEscaped: f
-                                }, t.attributes.popper = Object.assign({}, t.attributes.popper, {
-                                    "data-popper-reference-hidden": u,
-                                    "data-popper-escaped": f
+                                    I = Xt(Object.assign({}, ot, H)),
+                                    V = T === rt ? I : X,
+                                    Z = {
+                                        top: M.top - V.top + W.top,
+                                        bottom: V.bottom - M.bottom + W.bottom,
+                                        left: M.left - V.left + W.left,
+                                        right: V.right - M.right + W.right
+                                    },
+                                    K = n.modifiersData.offset;
+                                if (T === rt && K) {
+                                    var st = K[w];
+                                    Object.keys(Z).forEach(function(ct) {
+                                        var ft = [et, _].indexOf(ct) >= 0 ? 1 : -1,
+                                            yt = [E, _].indexOf(ct) >= 0 ? "y" : "x";
+                                        Z[ct] += st[yt] * ft
+                                    })
+                                }
+                                return Z
+                            }
+
+                            function Mt(n, r, i) {
+                                return P(n, x(r, i))
+                            }
+
+                            function fe(n, r, i) {
+                                return i === void 0 && (i = {
+                                    x: 0,
+                                    y: 0
+                                }), {
+                                    top: n.top - r.height - i.y,
+                                    right: n.right - r.width + i.x,
+                                    bottom: n.bottom - r.height + i.y,
+                                    left: n.left - r.width - i.x
+                                }
+                            }
+
+                            function pe(n) {
+                                return [E, et, _, U].some(function(r) {
+                                    return n[r] >= 0
                                 })
                             }
-                        }]
-                    })
+                            var Pe = Ee({
+                                defaultModifiers: [{
+                                    name: "eventListeners",
+                                    enabled: !0,
+                                    phase: "write",
+                                    fn: function() {},
+                                    effect: function(n) {
+                                        var r = n.state,
+                                            i = n.instance,
+                                            f = n.options,
+                                            w = f.scroll,
+                                            b = w === void 0 || w,
+                                            g = f.resize,
+                                            k = g === void 0 || g,
+                                            j = R(r.elements.popper),
+                                            A = [].concat(r.scrollParents.reference, r.scrollParents.popper);
+                                        return b && A.forEach(function(T) {
+                                                T.addEventListener("scroll", i.update, $t)
+                                            }), k && j.addEventListener("resize", i.update, $t),
+                                            function() {
+                                                b && A.forEach(function(T) {
+                                                    T.removeEventListener("scroll", i.update, $t)
+                                                }), k && j.removeEventListener("resize", i.update, $t)
+                                            }
+                                    },
+                                    data: {}
+                                }, {
+                                    name: "popperOffsets",
+                                    enabled: !0,
+                                    phase: "read",
+                                    fn: function(n) {
+                                        var r = n.state,
+                                            i = n.name;
+                                        r.modifiersData[i] = oe({
+                                            reference: r.rects.reference,
+                                            element: r.rects.popper,
+                                            strategy: "absolute",
+                                            placement: r.placement
+                                        })
+                                    },
+                                    data: {}
+                                }, {
+                                    name: "computeStyles",
+                                    enabled: !0,
+                                    phase: "beforeWrite",
+                                    fn: function(n) {
+                                        var r = n.state,
+                                            i = n.options,
+                                            f = i.gpuAcceleration,
+                                            w = f === void 0 || f,
+                                            b = i.adaptive,
+                                            g = b === void 0 || b,
+                                            k = i.roundOffsets,
+                                            j = k === void 0 || k,
+                                            A = {
+                                                placement: bt(r.placement),
+                                                variation: At(r.placement),
+                                                popper: r.elements.popper,
+                                                popperRect: r.rects.popper,
+                                                gpuAcceleration: w,
+                                                isFixed: r.options.strategy === "fixed"
+                                            };
+                                        r.modifiersData.popperOffsets != null && (r.styles.popper = Object.assign({}, r.styles.popper, ie(Object.assign({}, A, {
+                                            offsets: r.modifiersData.popperOffsets,
+                                            position: r.options.strategy,
+                                            adaptive: g,
+                                            roundOffsets: j
+                                        })))), r.modifiersData.arrow != null && (r.styles.arrow = Object.assign({}, r.styles.arrow, ie(Object.assign({}, A, {
+                                            offsets: r.modifiersData.arrow,
+                                            position: "absolute",
+                                            adaptive: !1,
+                                            roundOffsets: j
+                                        })))), r.attributes.popper = Object.assign({}, r.attributes.popper, {
+                                            "data-popper-placement": r.placement
+                                        })
+                                    },
+                                    data: {}
+                                }, {
+                                    name: "applyStyles",
+                                    enabled: !0,
+                                    phase: "write",
+                                    fn: function(n) {
+                                        var r = n.state;
+                                        Object.keys(r.elements).forEach(function(i) {
+                                            var f = r.styles[i] || {},
+                                                w = r.attributes[i] || {},
+                                                b = r.elements[i];
+                                            C(b) && o(b) && (Object.assign(b.style, f), Object.keys(w).forEach(function(g) {
+                                                var k = w[g];
+                                                k === !1 ? b.removeAttribute(g) : b.setAttribute(g, k === !0 ? "" : k)
+                                            }))
+                                        })
+                                    },
+                                    effect: function(n) {
+                                        var r = n.state,
+                                            i = {
+                                                popper: {
+                                                    position: r.options.strategy,
+                                                    left: "0",
+                                                    top: "0",
+                                                    margin: "0"
+                                                },
+                                                arrow: {
+                                                    position: "absolute"
+                                                },
+                                                reference: {}
+                                            };
+                                        return Object.assign(r.elements.popper.style, i.popper), r.styles = i, r.elements.arrow && Object.assign(r.elements.arrow.style, i.arrow),
+                                            function() {
+                                                Object.keys(r.elements).forEach(function(f) {
+                                                    var w = r.elements[f],
+                                                        b = r.attributes[f] || {},
+                                                        g = Object.keys(r.styles.hasOwnProperty(f) ? r.styles[f] : i[f]).reduce(function(k, j) {
+                                                            return k[j] = "", k
+                                                        }, {});
+                                                    C(w) && o(w) && (Object.assign(w.style, g), Object.keys(b).forEach(function(k) {
+                                                        w.removeAttribute(k)
+                                                    }))
+                                                })
+                                            }
+                                    },
+                                    requires: ["computeStyles"]
+                                }, {
+                                    name: "offset",
+                                    enabled: !0,
+                                    phase: "main",
+                                    requires: ["popperOffsets"],
+                                    fn: function(n) {
+                                        var r = n.state,
+                                            i = n.options,
+                                            f = n.name,
+                                            w = i.offset,
+                                            b = w === void 0 ? [0, 0] : w,
+                                            g = Ot.reduce(function(T, L) {
+                                                return T[L] = function(nt, D, z) {
+                                                    var W = bt(nt),
+                                                        q = [U, E].indexOf(W) >= 0 ? -1 : 1,
+                                                        ot = typeof z == "function" ? z(Object.assign({}, D, {
+                                                            placement: nt
+                                                        })) : z,
+                                                        J = ot[0],
+                                                        M = ot[1];
+                                                    return J = J || 0, M = (M || 0) * q, [U, et].indexOf(W) >= 0 ? {
+                                                        x: M,
+                                                        y: J
+                                                    } : {
+                                                        x: J,
+                                                        y: M
+                                                    }
+                                                }(L, r.rects, b), T
+                                            }, {}),
+                                            k = g[r.placement],
+                                            j = k.x,
+                                            A = k.y;
+                                        r.modifiersData.popperOffsets != null && (r.modifiersData.popperOffsets.x += j, r.modifiersData.popperOffsets.y += A), r.modifiersData[f] = g
+                                    }
+                                }, {
+                                    name: "flip",
+                                    enabled: !0,
+                                    phase: "main",
+                                    fn: function(n) {
+                                        var r = n.state,
+                                            i = n.options,
+                                            f = n.name;
+                                        if (!r.modifiersData[f]._skip) {
+                                            for (var w = i.mainAxis, b = w === void 0 || w, g = i.altAxis, k = g === void 0 || g, j = i.fallbackPlacements, A = i.padding, T = i.boundary, L = i.rootBoundary, nt = i.altBoundary, D = i.flipVariations, z = D === void 0 || D, W = i.allowedAutoPlacements, q = r.options.placement, ot = bt(q), J = j || (ot !== q && z ? function(ut) {
+                                                    if (bt(ut) === kt) return [];
+                                                    var ht = Nt(ut);
+                                                    return [ae(ut), ht, ae(ht)]
+                                                }(q) : [Nt(q)]), M = [q].concat(J).reduce(function(ut, ht) {
+                                                    return ut.concat(bt(ht) === kt ? function(Ct, jt) {
+                                                        jt === void 0 && (jt = {});
+                                                        var vt = jt,
+                                                            Wt = vt.placement,
+                                                            Zt = vt.boundary,
+                                                            Tt = vt.rootBoundary,
+                                                            Gt = vt.padding,
+                                                            Kt = vt.flipVariations,
+                                                            Rt = vt.allowedAutoPlacements,
+                                                            Jt = Rt === void 0 ? Ot : Rt,
+                                                            Vt = At(Wt),
+                                                            Ut = Vt ? Kt ? Bt : Bt.filter(function(gt) {
+                                                                return At(gt) === Vt
+                                                            }) : Et,
+                                                            qt = Ut.filter(function(gt) {
+                                                                return Jt.indexOf(gt) >= 0
+                                                            });
+                                                        qt.length === 0 && (qt = Ut);
+                                                        var Dt = qt.reduce(function(gt, Pt) {
+                                                            return gt[Pt] = It(Ct, {
+                                                                placement: Pt,
+                                                                boundary: Zt,
+                                                                rootBoundary: Tt,
+                                                                padding: Gt
+                                                            })[bt(Pt)], gt
+                                                        }, {});
+                                                        return Object.keys(Dt).sort(function(gt, Pt) {
+                                                            return Dt[gt] - Dt[Pt]
+                                                        })
+                                                    }(r, {
+                                                        placement: ht,
+                                                        boundary: T,
+                                                        rootBoundary: L,
+                                                        padding: A,
+                                                        flipVariations: z,
+                                                        allowedAutoPlacements: W
+                                                    }) : ht)
+                                                }, []), X = r.rects.reference, H = r.rects.popper, I = new Map, V = !0, Z = M[0], K = 0; K < M.length; K++) {
+                                                var st = M[K],
+                                                    ct = bt(st),
+                                                    ft = At(st) === wt,
+                                                    yt = [E, _].indexOf(ct) >= 0,
+                                                    St = yt ? "width" : "height",
+                                                    pt = It(r, {
+                                                        placement: st,
+                                                        boundary: T,
+                                                        rootBoundary: L,
+                                                        altBoundary: nt,
+                                                        padding: A
+                                                    }),
+                                                    lt = yt ? ft ? et : U : ft ? _ : E;
+                                                X[St] > H[St] && (lt = Nt(lt));
+                                                var at = Nt(lt),
+                                                    tt = [];
+                                                if (b && tt.push(pt[ct] <= 0), k && tt.push(pt[lt] <= 0, pt[at] <= 0), tt.every(function(ut) {
+                                                        return ut
+                                                    })) {
+                                                    Z = st, V = !1;
+                                                    break
+                                                }
+                                                I.set(st, tt)
+                                            }
+                                            if (V)
+                                                for (var _t = function(ut) {
+                                                        var ht = M.find(function(Ct) {
+                                                            var jt = I.get(Ct);
+                                                            if (jt) return jt.slice(0, ut).every(function(vt) {
+                                                                return vt
+                                                            })
+                                                        });
+                                                        if (ht) return Z = ht, "break"
+                                                    }, dt = z ? 3 : 1; dt > 0 && _t(dt) !== "break"; dt--);
+                                            r.placement !== Z && (r.modifiersData[f]._skip = !0, r.placement = Z, r.reset = !0)
+                                        }
+                                    },
+                                    requiresIfExists: ["offset"],
+                                    data: {
+                                        _skip: !1
+                                    }
+                                }, {
+                                    name: "preventOverflow",
+                                    enabled: !0,
+                                    phase: "main",
+                                    fn: function(n) {
+                                        var r = n.state,
+                                            i = n.options,
+                                            f = n.name,
+                                            w = i.mainAxis,
+                                            b = w === void 0 || w,
+                                            g = i.altAxis,
+                                            k = g !== void 0 && g,
+                                            j = i.boundary,
+                                            A = i.rootBoundary,
+                                            T = i.altBoundary,
+                                            L = i.padding,
+                                            nt = i.tether,
+                                            D = nt === void 0 || nt,
+                                            z = i.tetherOffset,
+                                            W = z === void 0 ? 0 : z,
+                                            q = It(r, {
+                                                boundary: j,
+                                                rootBoundary: A,
+                                                padding: L,
+                                                altBoundary: T
+                                            }),
+                                            ot = bt(r.placement),
+                                            J = At(r.placement),
+                                            M = !J,
+                                            X = Yt(ot),
+                                            H = X === "x" ? "y" : "x",
+                                            I = r.modifiersData.popperOffsets,
+                                            V = r.rects.reference,
+                                            Z = r.rects.popper,
+                                            K = typeof W == "function" ? W(Object.assign({}, r.rects, {
+                                                placement: r.placement
+                                            })) : W,
+                                            st = typeof K == "number" ? {
+                                                mainAxis: K,
+                                                altAxis: K
+                                            } : Object.assign({
+                                                mainAxis: 0,
+                                                altAxis: 0
+                                            }, K),
+                                            ct = r.modifiersData.offset ? r.modifiersData.offset[r.placement] : null,
+                                            ft = {
+                                                x: 0,
+                                                y: 0
+                                            };
+                                        if (I) {
+                                            if (b) {
+                                                var yt, St = X === "y" ? E : U,
+                                                    pt = X === "y" ? _ : et,
+                                                    lt = X === "y" ? "height" : "width",
+                                                    at = I[X],
+                                                    tt = at + q[St],
+                                                    _t = at - q[pt],
+                                                    dt = D ? -Z[lt] / 2 : 0,
+                                                    ut = J === wt ? V[lt] : Z[lt],
+                                                    ht = J === wt ? -Z[lt] : -V[lt],
+                                                    Ct = r.elements.arrow,
+                                                    jt = D && Ct ? e(Ct) : {
+                                                        width: 0,
+                                                        height: 0
+                                                    },
+                                                    vt = r.modifiersData["arrow#persistent"] ? r.modifiersData["arrow#persistent"].padding : {
+                                                        top: 0,
+                                                        right: 0,
+                                                        bottom: 0,
+                                                        left: 0
+                                                    },
+                                                    Wt = vt[St],
+                                                    Zt = vt[pt],
+                                                    Tt = Mt(0, V[lt], jt[lt]),
+                                                    Gt = M ? V[lt] / 2 - dt - Tt - Wt - st.mainAxis : ut - Tt - Wt - st.mainAxis,
+                                                    Kt = M ? -V[lt] / 2 + dt + Tt + Zt + st.mainAxis : ht + Tt + Zt + st.mainAxis,
+                                                    Rt = r.elements.arrow && S(r.elements.arrow),
+                                                    Jt = Rt ? X === "y" ? Rt.clientTop || 0 : Rt.clientLeft || 0 : 0,
+                                                    Vt = (yt = ct?.[X]) != null ? yt : 0,
+                                                    Ut = at + Kt - Vt,
+                                                    qt = Mt(D ? x(tt, at + Gt - Vt - Jt) : tt, at, D ? P(_t, Ut) : _t);
+                                                I[X] = qt, ft[X] = qt - at
+                                            }
+                                            if (k) {
+                                                var Dt, gt = X === "x" ? E : U,
+                                                    Pt = X === "x" ? _ : et,
+                                                    Lt = I[H],
+                                                    zt = H === "y" ? "height" : "width",
+                                                    de = Lt + q[gt],
+                                                    ye = Lt - q[Pt],
+                                                    Qt = [E, U].indexOf(ot) !== -1,
+                                                    he = (Dt = ct?.[H]) != null ? Dt : 0,
+                                                    ve = Qt ? de : Lt - V[zt] - Z[zt] - he + st.altAxis,
+                                                    me = Qt ? Lt + V[zt] + Z[zt] - he - st.altAxis : ye,
+                                                    be = D && Qt ? function(Le, Ae, te) {
+                                                        var ge = Mt(Le, Ae, te);
+                                                        return ge > te ? te : ge
+                                                    }(ve, Lt, me) : Mt(D ? ve : de, Lt, D ? me : ye);
+                                                I[H] = be, ft[H] = be - Lt
+                                            }
+                                            r.modifiersData[f] = ft
+                                        }
+                                    },
+                                    requiresIfExists: ["offset"]
+                                }, {
+                                    name: "arrow",
+                                    enabled: !0,
+                                    phase: "main",
+                                    fn: function(n) {
+                                        var r, i = n.state,
+                                            f = n.name,
+                                            w = n.options,
+                                            b = i.elements.arrow,
+                                            g = i.modifiersData.popperOffsets,
+                                            k = bt(i.placement),
+                                            j = Yt(k),
+                                            A = [U, et].indexOf(k) >= 0 ? "height" : "width";
+                                        if (b && g) {
+                                            var T = function(Z, K) {
+                                                    return le(typeof(Z = typeof Z == "function" ? Z(Object.assign({}, K.rects, {
+                                                        placement: K.placement
+                                                    })) : Z) != "number" ? Z : ue(Z, Et))
+                                                }(w.padding, i),
+                                                L = e(b),
+                                                nt = j === "y" ? E : U,
+                                                D = j === "y" ? _ : et,
+                                                z = i.rects.reference[A] + i.rects.reference[j] - g[j] - i.rects.popper[A],
+                                                W = g[j] - i.rects.reference[j],
+                                                q = S(b),
+                                                ot = q ? j === "y" ? q.clientHeight || 0 : q.clientWidth || 0 : 0,
+                                                J = z / 2 - W / 2,
+                                                M = T[nt],
+                                                X = ot - L[A] - T[D],
+                                                H = ot / 2 - L[A] / 2 + J,
+                                                I = Mt(M, H, X),
+                                                V = j;
+                                            i.modifiersData[f] = ((r = {})[V] = I, r.centerOffset = I - H, r)
+                                        }
+                                    },
+                                    effect: function(n) {
+                                        var r = n.state,
+                                            i = n.options.element,
+                                            f = i === void 0 ? "[data-popper-arrow]" : i;
+                                        f != null && (typeof f != "string" || (f = r.elements.popper.querySelector(f))) && se(r.elements.popper, f) && (r.elements.arrow = f)
+                                    },
+                                    requires: ["popperOffsets"],
+                                    requiresIfExists: ["preventOverflow"]
+                                }, {
+                                    name: "hide",
+                                    enabled: !0,
+                                    phase: "main",
+                                    requiresIfExists: ["preventOverflow"],
+                                    fn: function(n) {
+                                        var r = n.state,
+                                            i = n.name,
+                                            f = r.rects.reference,
+                                            w = r.rects.popper,
+                                            b = r.modifiersData.preventOverflow,
+                                            g = It(r, {
+                                                elementContext: "reference"
+                                            }),
+                                            k = It(r, {
+                                                altBoundary: !0
+                                            }),
+                                            j = fe(g, f),
+                                            A = fe(k, w, b),
+                                            T = pe(j),
+                                            L = pe(A);
+                                        r.modifiersData[i] = {
+                                            referenceClippingOffsets: j,
+                                            popperEscapeOffsets: A,
+                                            isReferenceHidden: T,
+                                            hasPopperEscaped: L
+                                        }, r.attributes.popper = Object.assign({}, r.attributes.popper, {
+                                            "data-popper-reference-hidden": T,
+                                            "data-popper-escaped": L
+                                        })
+                                    }
+                                }]
+                            })
+                        }
+                    },
+                    Q = {};
+
+                function Y(G) {
+                    var it = Q[G];
+                    if (it !== void 0) return it.exports;
+                    var N = Q[G] = {
+                        exports: {}
+                    };
+                    return F[G](N, N.exports, Y), N.exports
                 }
-            },
-            t = {};
+                Y.d = (G, it) => {
+                    for (var N in it) Y.o(it, N) && !Y.o(G, N) && Object.defineProperty(G, N, {
+                        enumerable: !0,
+                        get: it[N]
+                    })
+                }, Y.o = (G, it) => Object.prototype.hasOwnProperty.call(G, it), Y.r = G => {
+                    typeof Symbol < "u" && Symbol.toStringTag && Object.defineProperty(G, Symbol.toStringTag, {
+                        value: "Module"
+                    }), Object.defineProperty(G, "__esModule", {
+                        value: !0
+                    })
+                };
+                var mt = {};
+                return Y.r(mt), Y(661), Y(795), Y(682), Y(284), Y(181), Y(778), Y(51), Y(185), mt
+            })()
+        })
+    });
+    var Ze = Ie(Oe());
 
-        function o(n) {
-            var r = t[n];
-            if (void 0 !== r) return r.exports;
-            var i = t[n] = {
-                exports: {}
-            };
-            return e[n](i, i.exports, o), i.exports
-        }
-        o.d = (e, t) => {
-            for (var n in t) o.o(t, n) && !o.o(e, n) && Object.defineProperty(e, n, {
-                enumerable: !0,
-                get: t[n]
-            })
-        }, o.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), o.r = e => {
-            "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
-                value: "Module"
-            }), Object.defineProperty(e, "__esModule", {
-                value: !0
-            })
-        };
-        var n = {};
-        return o.r(n), o(661), o(795), o(682), o(284), o(181), o(778), o(51), o(185), n
-    })()
-}));
+    function Me(F) {
+        document.cookie = `theme=${F}; path=/; max-age=${60*60*24*14};`
+    }
+
+    function Ve(F) {
+        let Y = `; ${document.cookie}`.split(`; ${F}=`);
+        if (Y.length === 2) return Y.pop().split(";").shift()
+    }
+
+    function $e(F) {
+        let Q = document.getElementById("html-root");
+        F == "light" ? Q.classList.remove("dark") : Q.classList.add("dark")
+    }
+
+    function Ne() {
+        let F = document.getElementById("html-root");
+        return F.classList.contains("dark") ? (F.classList.remove("dark"), "light") : (F.classList.add("dark"), "dark")
+    }
+    document.addEventListener("DOMContentLoaded", function() {
+        let F = Ve("theme");
+        $e(F), document.getElementById("mode-toggle").addEventListener("click", Y => {
+            let mt = Ne();
+            Me(mt), window.location.reload()
+        })
+    });
+})();
+/*! Bundled license information:
+
+preline/dist/preline.js:
+  (*! For license information please see preline.js.LICENSE.txt *)
+*/
```

### Comparing `django-insights-0.1.7/django_insights/templates/insights/app.html` & `django-insights-0.1.8/django_insights/templates/insights/app.html`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/django_insights/templates/insights/base.html` & `django-insights-0.1.8/django_insights/templates/insights/base.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,130 +1,112 @@
 {% load static %}
 {% url 'insights:insight_dashboard' as dashboard_url %}
 <!doctype html>
-<html id="html-root" lang="en" class="">
+<html id="html-root" lang="en">
     <title>{{ app_name }} - Insights</title>
     <head>
         <meta charset="UTF-8" />
         <meta lang="en" />
         <meta keywords="{{ app_name }}, insights" />
         <meta description="{{ app_name }} - Insights" />
         <meta charset="UTF-8"/>
         <meta name="viewport" content="width=device-width, initial-scale=1.0" />
         <link rel="preconnect" href="https://fonts.bunny.net" />
         <link href="https://fonts.bunny.net/css?family=ubuntu:300,300i,400,400i,500,500i,700,700i"
               rel="stylesheet"/>
         <link rel="stylesheet" href="{% static 'insights/css/insights.css' %}" />
-        <script src="{% static 'insights/js/preline.js' %}"></script>
-        <script>
-            function setCookie(theme) {
-                document.cookie = `theme=${theme}; path=/; max-age=${60 * 60 * 24 * 14};`;
-            }
-
-            function getCookie (name) {
-                let value = `; ${document.cookie}`;
-                let parts = value.split(`; ${name}=`);
-                if (parts.length === 2) return parts.pop().split(';').shift();
-            }
-
-            function darkMode(theme) {
-                const element = document.getElementById('html-root')
-                if(theme == 'light') {
-                    element.classList.remove('dark')
-                } else {
-                    element.classList.add('dark')
-                }
-            }
-            
-            function toggleDarkMode() {
-                const element = document.getElementById('html-root')
-                if (element.classList.contains('dark')) {
-                    element.classList.remove('dark');
-                    return "light"
-                } else {
-                    element.classList.add('dark')
-                    return "dark"
-                }
-            }
-
-            const theme = getCookie('theme')
-            darkMode(theme);
-            
-            document.addEventListener('DOMContentLoaded', function() {
-
-
-                const button = document.querySelector("button");
-                
-                button.addEventListener("click", (event) => {
-                    const theme = toggleDarkMode()
-                    setCookie(theme)
-                    window.location.reload()
-                });
-            });
-        </script>
+        <script src="{% static 'insights/js/insights.js' %}" defer></script>
     </head>
     <body class="bg-background text-foreground dark:bg-foreground dark:text-background">
-        <header class="z-50 flex flex-wrap w-full py-2 text-sm sm:justify-start sm:flex-nowrap">
-            <nav class="w-full px-4 mx-auto sm:flex sm:items-center sm:justify-between">
-                <button class="p-2 rounded-sm hover:bg-gray-100">
+        <div class="sticky inset-x-0 top-0 z-20 px-4 bg-white drop-shadow-sm sm:px-6 md:px-8 dark:bg-foreground">
+            <div class="flex items-center py-1">
+                <!-- Navigation Toggle -->
+                <button type="button"
+                        class="text-gray-500 hover:text-gray-600"
+                        data-hs-overlay="#application-sidebar"
+                        aria-controls="application-sidebar"
+                        aria-label="Toggle navigation">
+                    <span class="sr-only">Toggle Navigation</span>
+                    <svg class="w-5 h-5"
+                         width="16"
+                         height="16"
+                         fill="currentColor"
+                         viewBox="0 0 16 16">
+                        <path fill-rule="evenodd" d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5zm0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5zm0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5z"/>
+                    </svg>
+                </button>
+                <!-- End Navigation Toggle -->
+                <!-- Breadcrumb -->
+                <ol class="flex items-center flex-grow min-w-0 ml-3 whitespace-nowrap"
+                    aria-label="Breadcrumb">
+                    <li class="flex items-center text-sm text-gray-800 dark:text-gray-400">
+                        {{ app_name }}
+                        <svg class="flex-shrink-0 mx-3 overflow-visible h-2.5 w-2.5 text-gray-400 dark:text-gray-600"
+                             width="16"
+                             height="16"
+                             viewBox="0 0 16 16"
+                             fill="none"
+                             xmlns="http://www.w3.org/2000/svg">
+                            <path d="M5 1L10.6869 7.16086C10.8637 7.35239 10.8637 7.64761 10.6869 7.83914L5 14" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
+                        </svg>
+                    </li>
+                    <li class="text-sm font-semibold text-gray-800 truncate dark:text-gray-400"
+                        aria-current="page">Dashboard</li>
+                </ol>
+                <button id="mode-toggle"
+                        class="p-2 rounded-sm hover:bg-gray-100 dark:hover:bg-gray-900">
                     <svg xmlns="http://www.w3.org/2000/svg"
                          fill="none"
                          viewBox="0 0 24 24"
                          stroke-width="1.5"
                          stroke="currentColor"
                          class="w-4 h-4">
                         <path stroke-linecap="round" stroke-linejoin="round" d="M12 3v2.25m6.364.386l-1.591 1.591M21 12h-2.25m-.386 6.364l-1.591-1.591M12 18.75V21m-4.773-4.227l-1.591 1.591M5.25 12H3m4.227-4.773L5.636 5.636M15.75 12a3.75 3.75 0 11-7.5 0 3.75 3.75 0 017.5 0z" />
                     </svg>
                 </button>
-            </nav>
-        </header>
-        <header class="z-50 flex flex-wrap w-full py-4 text-sm sm:justify-start sm:flex-nowrap">
-            <nav class="max-w-[85rem] w-full mx-auto px-4 sm:flex sm:items-center sm:justify-between"
-                 aria-label="Home">
-                <div class="flex items-center justify-between">
-                    <a class="flex-none" href="{{ dashboard_url }}">
-                        <span class="text-xl font-semibold text-primary-500">{{ app_name }}</span>
-                        <span class="inline-block align-top dark:text-white">Insights</span>
-                    </a>
-                    <div class="sm:hidden">
-                        <button type="button"
-                                class="inline-flex items-center justify-center gap-2 p-2 text-sm font-medium text-gray-700 align-middle transition-all bg-white border rounded-md shadow-sm hs-collapse-toggle hover:bg-gray-50 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-offset-white focus:ring-blue-600"
-                                data-hs-collapse="#navbar-collapse-with-animation"
-                                aria-controls="navbar-collapse-with-animation"
-                                aria-label="Toggle navigation">
-                            <svg class="w-4 h-4 hs-collapse-open:hidden"
-                                 width="16"
-                                 height="16"
-                                 fill="currentColor"
-                                 viewBox="0 0 16 16">
-                                <path fill-rule="evenodd" d="M2.5 12a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5zm0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5zm0-4a.5.5 0 0 1 .5-.5h10a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5z"/>
-                            </svg>
-                            <svg class="hidden w-4 h-4 hs-collapse-open:block"
+                <!-- End Breadcrumb -->
+            </div>
+        </div>
+        <!-- Sidebar -->
+        <div id="application-sidebar"
+             class="hs-overlay hs-overlay-open:translate-x-0 -translate-x-full transition-all duration-300 transform hidden fixed top-0 left-0 bottom-0 z-[60] w-64 bg-white border-r border-gray-200 pt-7 pb-10 overflow-y-auto scrollbar-y dark:scrollbar-y dark:bg-foreground dark:border-foreground">
+            <div class="px-6">
+                <a class="flex-none" href="{{ dashboard_url }}">
+                    <span class="text-xl font-semibold text-primary-500">{{ app_name }}</span>
+                    <span class="inline-block align-top dark:text-white">Insights</span>
+                </a>
+            </div>
+            <nav class="flex flex-col flex-wrap w-full p-6">
+                <ul class="space-y-1.5">
+                    <li>
+                        <a class="flex items-center gap-x-3.5 py-2 px-2.5 bg-gray-100 text-sm text-slate-700 rounded-md hover:bg-gray-100 dark:bg-gray-900 dark:text-white"
+                           href="{{ dashboard_url }}">
+                            <svg class="w-3.5 h-3.5"
+                                 xmlns="http://www.w3.org/2000/svg"
                                  width="16"
                                  height="16"
                                  fill="currentColor"
                                  viewBox="0 0 16 16">
-                                <path d="M4.646 4.646a.5.5 0 0 1 .708 0L8 7.293l2.646-2.647a.5.5 0 0 1 .708.708L8.707 8l2.647 2.646a.5.5 0 0 1-.708.708L8 8.707l-2.646 2.647a.5.5 0 0 1-.708-.708L7.293 8 4.646 5.354a.5.5 0 0 1 0-.708z"/>
+                                <path fill-rule="evenodd" d="M2 13.5V7h1v6.5a.5.5 0 0 0 .5.5h9a.5.5 0 0 0 .5-.5V7h1v6.5a1.5 1.5 0 0 1-1.5 1.5h-9A1.5 1.5 0 0 1 2 13.5zm11-11V6l-2-2V2.5a.5.5 0 0 1 .5-.5h1a.5.5 0 0 1 .5.5z"/>
+                                <path fill-rule="evenodd" d="M7.293 1.5a1 1 0 0 1 1.414 0l6.647 6.646a.5.5 0 0 1-.708.708L8 2.207 1.354 8.854a.5.5 0 1 1-.708-.708L7.293 1.5z"/>
                             </svg>
-                        </button>
-                    </div>
-                </div>
-                <div id="navbar-collapse-with-animation"
-                     class="hidden overflow-hidden transition-all duration-300 hs-collapse basis-full grow sm:block">
-                    <div class="flex flex-col gap-5 mt-5 shrink sm:flex-row sm:items-center sm:justify-end sm:mt-0 sm:pl-5">
-                        <a class="font-medium text-gray-600 hover:text-gray-400 dark:text-background dark:hover:text-gray-500"
-                           href="{{ dashboard_url }}">Dashboard</a>
-                        {% for app in apps %}
-                            {% url 'insights:insight_app' app_uuid=app.uuid as app_url %}
-                            <a class="font-medium text-gray-600 hover:text-gray-400 dark:text-background dark:hover:text-gray-500"
-                               href="{{ app_url }}">{{ app.name }}</a>
-                        {% endfor %}
-                    </div>
-                </div>
+                            Dashboard
+                        </a>
+                    </li>
+                    {% for app in apps %}
+                        {% url 'insights:insight_app' app_uuid=app.uuid as app_url %}
+                        <li>
+                            <a class="flex items-center gap-x-3.5 py-2 px-2.5 text-sm text-slate-700 rounded-md hover:bg-gray-100 dark:hover:bg-gray-900 dark:text-slate-400 dark:hover:text-slate-300"
+                               href="{{ app_url }}">
+                                {{ app.name }}
+                            </a>
+                        </li>
+                    {% endfor %}
+                </ul>
             </nav>
-        </header>
-        <div>
+        </div>
+        <div class="w-full px-4 pt-4 sm:px-6 md:px-8">
             {% block content %}
             {% endblock content %}
         </div>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -3,14 +3,18 @@
 
 
 
 
 
 
 
+  Toggle Navigation
+   1. {{ app_name }}
+   2. Dashboard
 
 {{_app_name_}}_Insights
-
-Dashboard {% for app in apps %} {% url 'insights:insight_app' app_uuid=app.uuid
-as app_url %} {{_app.name_}} {% endfor %}
-
+    * ____Dashboard
+    * {% for app in apps %} {% url 'insights:insight_app' app_uuid=app.uuid as
+      app_url %}
+    * {{_app.name_}}
+    * {% endfor %}
 {% block content %} {% endblock content %}
```

### Comparing `django-insights-0.1.7/django_insights/templates/insights/dashboard.html` & `django-insights-0.1.8/django_insights/templates/insights/dashboard.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% extends "insights/base.html" %}
 {% block content %}
     <!-- Card Section -->
-    <div class="max-w-[85rem] py-4 lg:py-6 mx-auto">
+    <div class="max-w-[85rem]">
         <!-- Grid -->
         <div class="grid gap-4 sm:grid-cols-2 lg:grid-cols-4 sm:gap-6">
             {% for counter in counter_list %}
                 <div class="flex flex-col border shadow-sm border-slate-200 dark:border-slate-900 bg-background text-foreground dark:bg-foreground dark:text-background rounded-xl">
                     <div class="p-4 md:p-5">
                         <div class="flex items-center gap-x-2">
                             <p class="text-xs tracking-wide text-gray-500 uppercase">{{ counter.question }}</p>
```

### Comparing `django-insights-0.1.7/django_insights/views.py` & `django-insights-0.1.8/django_insights/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,17 @@
         view._is_coroutine = asyncio.coroutines._is_coroutine
         return view
 
     async def get(self, request, bucket_id):
         theme = self.request.COOKIES.get('theme') or settings.INSIGHTS_DEFAULT_THEME
         bucket: Bucket = await get_bucket(bucket_id)
 
-        filename: str = f"{settings.MEDIA_ROOT}insights/{bucket.type}-{bucket.pk}.png"
+        filename: str = (
+            f"{settings.MEDIA_ROOT}insights/{bucket.type}-{bucket.pk}-{theme}.png"
+        )
 
         if os.path.exists(filename) and settings.INSIGHT_CHARTS_USE_MEDIA_CACHE:
             with open(filename, 'rb') as cached_image:
                 buffer = cached_image.read()
 
             return HttpResponse(buffer, content_type='image/png')
```

### Comparing `django-insights-0.1.7/docs/assets/images/banner.png` & `django-insights-0.1.8/docs/assets/images/banner.png`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/docs/assets/images/screen_1.png` & `django-insights-0.1.8/docs/assets/images/screen_1.png`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/docs/assets/images/screen_2.png` & `django-insights-0.1.8/docs/assets/images/screen_2.png`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/docs/license.md` & `django-insights-0.1.8/docs/license.md`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/project/settings/base.py` & `django-insights-0.1.8/project/settings/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
 USE_TZ = True
 
 
 # Django Insights settings
 
 # Custom app name
-INSIGHTS_APP_NAME = "Bezamon"
+INSIGHTS_APP_NAME = "Finq"
 
 # Quality of chart images
 INSIGHTS_CHART_DPI = 180
 
 # Change primary color
 INSIGHTS_CHART_LIGHT_PRIMARY_COLOR = "#2563EB"
 INSIGHTS_CHART_DARK_PRIMARY_COLOR = "#BFDBFE"
```

### Comparing `django-insights-0.1.7/project/testapp/insights.py` & `django-insights-0.1.8/project/testapp/insights.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/project/testapp/management/commands/seed_db.py` & `django-insights-0.1.8/project/testapp/management/commands/seed_db.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/project/testapp/migrations/0001_initial.py` & `django-insights-0.1.8/project/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/project/testapp/models.py` & `django-insights-0.1.8/project/testapp/models.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/project/testapp/users/migrations/0001_initial.py` & `django-insights-0.1.8/project/testapp/users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/project/testapp/users/models.py` & `django-insights-0.1.8/project/testapp/users/models.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/pyproject.toml` & `django-insights-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/compile.py` & `django-insights-0.1.8/requirements/compile.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/py310-django32.txt` & `django-insights-0.1.8/requirements/py310-django32.txt`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/py310-django40.txt` & `django-insights-0.1.8/requirements/py310-django40.txt`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/py310-django41.txt` & `django-insights-0.1.8/requirements/py310-django41.txt`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/py310-django42.txt` & `django-insights-0.1.8/requirements/py310-django42.txt`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/py311-django41.txt` & `django-insights-0.1.8/requirements/py311-django41.txt`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/py311-django42.txt` & `django-insights-0.1.8/requirements/py311-django42.txt`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/py38-django32.txt` & `django-insights-0.1.8/requirements/py38-django32.txt`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/py38-django40.txt` & `django-insights-0.1.8/requirements/py38-django40.txt`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/py38-django41.txt` & `django-insights-0.1.8/requirements/py38-django41.txt`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/py38-django42.txt` & `django-insights-0.1.8/requirements/py38-django42.txt`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/py39-django32.txt` & `django-insights-0.1.8/requirements/py39-django32.txt`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/py39-django40.txt` & `django-insights-0.1.8/requirements/py39-django40.txt`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/py39-django41.txt` & `django-insights-0.1.8/requirements/py39-django41.txt`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/requirements/py39-django42.txt` & `django-insights-0.1.8/requirements/py39-django42.txt`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/tests/test_api.py` & `django-insights-0.1.8/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-insights-0.1.7/PKG-INFO` & `django-insights-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-insights
-Version: 0.1.7
+Version: 0.1.8
 Summary: Django Insights 
 Author-email: DK <dk@terminalkitten.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -44,15 +44,16 @@
 
 ## Features
 
 Create insights for your app, store them in a SQLite database for further processing, these insights are written right next to your application logic.
 
 ### Note:
 
-Still working on some small things, extending tests and improve docs.
+Still working on some small things, extending tests and improving the documentation.
+
 For now focus is on:
 
 - Django 3.2 (LTS), 4.0,4.1 and 4.2;
 - Python ≥ 3.8
 
 ## Installation
 
@@ -147,15 +148,15 @@
         include('django_insights.urls', namespace='insights'),
     ),
 ]
 ```
 
 !["Dashboard - App"](https://raw.githubusercontent.com/terminalkitten/django-insights/main/docs/assets/images/screen_2.png)
 
-Now you can visit https://localhost:8000/insights to inspect your Django Insights database
+Now you can visit https://localhost:8000/insights to inspect your Django Insights database.
 
 ## Metrics
 
 Django insights contains 5 types of metrics it can collect:
 
 - `@metrics.counter`
 - `@metrics.gauge`
@@ -300,15 +301,15 @@
 INSIGHTS_CHART_LIGHT_PRIMARY_COLOR = "#2563EB"
 INSIGHTS_CHART_DARK_PRIMARY_COLOR = "#BFDBFE"
 
 ```
 
 ## Use-cases
 
-Insights are gathered from your current application state, Django Insights is not intentend to be used as a realtime, incremementing datasource. You should be able to re-gather these insights from your actual data at any moment in time.
+Insights are gathered from your current application state, Django Insights is not intentend to be used as a realtime, incremementing data-source. You should be able to re-gather these insights from your actual data at any moment in time.
 
 Yes:
 
 - How many users, how many users invited a year
 - How many reports a day, how many messages send on Wednesday's
 
 No:
```

