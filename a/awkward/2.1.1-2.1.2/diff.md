# Comparing `tmp/awkward-2.1.1.tar.gz` & `tmp/awkward-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Mar  7 19:33:13 2023, max compression
+gzip compressed data, last modified: Sat Apr  8 19:13:43 2023, max compression
```

## Comparing `awkward-2.1.1.tar` & `awkward-2.1.2.tar`

### file list

```diff
@@ -1,815 +1,829 @@
--rw-r--r--   0        0        0     1893 2023-03-07 19:33:13.000000 awkward-2.1.1/CITATION.cff
--rw-r--r--   0        0        0    13386 2023-03-07 19:33:13.000000 awkward-2.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    22299 2023-03-07 19:33:13.000000 awkward-2.1.1/README.md
--rw-r--r--   0        0        0      241 2023-03-07 19:33:13.000000 awkward-2.1.1/requirements-test.txt
--rw-r--r--   0        0        0     7833 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/_toc.yml
--rw-r--r--   0        0        0     7624 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/conf.py
--rw-r--r--   0        0        0      346 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/environment.yml.cog
--rw-r--r--   0        0        0     2603 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/index.md
--rw-r--r--   0        0        0    11642 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/prepare_docstrings.py
--rw-r--r--   0        0        0     4448 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/redirects-user-guide.json
--rw-r--r--   0        0        0    11436 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/redirects.json
--rw-r--r--   0        0        0      452 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/requirements.txt
--rw-r--r--   0        0        0      369 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/switcher.json
--rw-r--r--   0        0        0      930 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/_static/css/awkward.css
--rw-r--r--   0        0        0      354 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/_static/css/try-awkward-array.css
-lrwxr-xr-x   0        0        0        0 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
-lrwxr-xr-x   0        0        0        0 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0      469 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/_templates/funding.html
--rw-r--r--   0        0        0      474 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/_templates/redirect.html
--rw-r--r--   0        0        0     2877 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/getting-started/community-tutorials.md
--rw-r--r--   0        0        0     4654 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/getting-started/index.md
--rw-r--r--   0        0        0     3346 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/getting-started/papers-and-talks.md
--rw-r--r--   0        0        0       82 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/getting-started/try-awkward-array.md
-lrwxr-xr-x   0        0        0        0 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    12847 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/getting-started/demo/what-is-an-awkward-array.ipynb
-lrwxr-xr-x   0        0        0        0 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
-lrwxr-xr-x   0        0        0        0 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
-lrwxr-xr-x   0        0        0        0 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
-lrwxr-xr-x   0        0        0        0 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    17067 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/image/example-hierarchy.svg
-lrwxr-xr-x   0        0        0        0 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
-lrwxr-xr-x   0        0        0        0 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
-lrwxr-xr-x   0        0        0        0 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
-lrwxr-xr-x   0        0        0        0 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
-lrwxr-xr-x   0        0        0        0 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
-lrwxr-xr-x   0        0        0        0 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    25309 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/reference/ak.behavior.rst
--rw-r--r--   0        0        0     1430 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/reference/ak.builder.ArrayBuilder.rst
--rw-r--r--   0        0        0    64727 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/reference/awkwardforth.rst
--rw-r--r--   0        0        0      270 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/reference/index.md
--rw-r--r--   0        0        0     7252 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/reference/toctree.txt
--rw-r--r--   0        0        0     8320 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/10-minutes-to-awkward-array.md
--rw-r--r--   0        0        0      926 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-combinatorics-best-match.md
--rw-r--r--   0        0        0      930 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
--rw-r--r--   0        0        0      263 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-combinatorics.md
--rw-r--r--   0        0        0     8335 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-convert-arrow.md
--rw-r--r--   0        0        0     6392 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-convert-buffers.md
--rw-r--r--   0        0        0     2455 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-convert-json.md
--rw-r--r--   0        0        0    13475 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-convert-numpy.md
--rw-r--r--   0        0        0     7182 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-convert-pandas.md
--rw-r--r--   0        0        0    18830 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-convert-python.md
--rw-r--r--   0        0        0     3554 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-convert-rdataframe.md
--rw-r--r--   0        0        0      271 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-convert.md
--rw-r--r--   0        0        0    11973 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-create-arraybuilder.md
--rw-r--r--   0        0        0    36520 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-create-constructors.md
--rw-r--r--   0        0        0     7383 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-create-lists.md
--rw-r--r--   0        0        0     7456 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-create-missing.md
--rw-r--r--   0        0        0    11542 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-create-records.md
--rw-r--r--   0        0        0     4066 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-create-strings.md
--rw-r--r--   0        0        0      866 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-create-unflatten-group.md
--rw-r--r--   0        0        0      267 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-create.md
--rw-r--r--   0        0        0      834 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-examine-checking-validity.md
--rw-r--r--   0        0        0     2919 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-examine-list-fields.md
--rw-r--r--   0        0        0      848 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-examine-simple-slicing.md
--rw-r--r--   0        0        0      838 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-examine-single-item.md
--rw-r--r--   0        0        0     6778 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-examine-type.md
--rw-r--r--   0        0        0      269 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-examine.md
--rw-r--r--   0        0        0      844 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-filter-cut-mask.md
--rw-r--r--   0        0        0     3889 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-filter-masked.md
--rw-r--r--   0        0        0      840 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-filter-num.md
--rw-r--r--   0        0        0     7955 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-filter-ragged.md
--rw-r--r--   0        0        0      265 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-filter.md
--rw-r--r--   0        0        0      818 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-math-argminmax.md
--rw-r--r--   0        0        0      822 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-math-broadcasting.md
--rw-r--r--   0        0        0      828 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-math-gpu.md
--rw-r--r--   0        0        0      838 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-math-numpy.md
--rw-r--r--   0        0        0      846 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-math-reducing.md
--rw-r--r--   0        0        0      870 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-math-statistics.md
--rw-r--r--   0        0        0      265 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-math.md
--rw-r--r--   0        0        0     3411 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-restructure-add-fields.md
--rw-r--r--   0        0        0      842 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-restructure-concatenate.md
--rw-r--r--   0        0        0    19083 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-restructure-flatten.md
--rw-r--r--   0        0        0     7568 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-restructure-pad.md
--rw-r--r--   0        0        0      852 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-restructure-rename-records.md
--rw-r--r--   0        0        0      832 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-restructure-sort.md
--rw-r--r--   0        0        0     9624 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-restructure-zip-project.md
--rw-r--r--   0        0        0      273 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-restructure.md
--rw-r--r--   0        0        0     2599 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-specialize-differentiate-jax.md
--rw-r--r--   0        0        0      870 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-specialize-in-numba.md
--rw-r--r--   0        0        0      838 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-specialize-lorentz.md
--rw-r--r--   0        0        0      874 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-specialize-override-numpy.md
--rw-r--r--   0        0        0      870 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-specialize-subclass.md
--rw-r--r--   0        0        0      277 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-specialize.md
--rw-r--r--   0        0        0    11724 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-use-header-only-layoutbuilder.md
--rw-r--r--   0        0        0      900 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-use-in-numba-arraybuilder.md
--rw-r--r--   0        0        0     9973 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-use-in-numba-cuda.ipynb
--rw-r--r--   0        0        0      900 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-use-in-numba-features.md
--rw-r--r--   0        0        0      279 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/how-to-use-in-numba.md
--rw-r--r--   0        0        0      344 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/index.md
--rw-r--r--   0        0        0        0 2023-03-07 19:33:13.000000 awkward-2.1.1/docs/user-guide/requirements.txt
--rw-r--r--   0        0        0   367587 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/panel-data-analysts.png
--rw-r--r--   0        0        0   794465 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/panel-data-analysts.svg
--rw-r--r--   0        0        0   140700 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/panel-developers.png
--rw-r--r--   0        0        0   328307 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/panel-developers.svg
--rw-r--r--   0        0        0    73584 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/panel-doxygen.png
--rw-r--r--   0        0        0    58179 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/panel-sphinx.png
--rw-r--r--   0        0        0   127063 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/panel-tutorials-alternate.png
--rw-r--r--   0        0        0   173327 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/panel-tutorials.png
--rw-r--r--   0        0        0    12541 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/awkward-1-0-layers.pdf
--rw-r--r--   0        0        0    65246 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/awkward-1-0-layers.png
--rw-r--r--   0        0        0    41004 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/awkward-1-0-layers.svg
--rw-r--r--   0        0        0    14946 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/awkward-timeline.pdf
--rw-r--r--   0        0        0   125180 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/awkward-timeline.png
--rw-r--r--   0        0        0    70209 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/awkward-timeline.svg
--rw-r--r--   0        0        0   436595 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
--rw-r--r--   0        0        0   426911 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
--rw-r--r--   0        0        0   335955 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/awkward-uproot-timeline-pip.png
--rw-r--r--   0        0        0   325268 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/awkward-uproot-timeline-pip.svg
--rw-r--r--   0        0        0   129696 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/awkward-uproot-timeline.png
--rw-r--r--   0        0        0   120554 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/awkward-uproot-timeline.svg
--rw-r--r--   0        0        0     5208 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/cartoon-broadcasting.png
--rw-r--r--   0        0        0    25065 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/cartoon-broadcasting.svg
--rw-r--r--   0        0        0     5754 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/cartoon-cartesian.png
--rw-r--r--   0        0        0    32616 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/cartoon-cartesian.svg
--rw-r--r--   0        0        0     9584 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/cartoon-combinations.png
--rw-r--r--   0        0        0    39524 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/cartoon-combinations.svg
--rw-r--r--   0        0        0    10808 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/cartoon-schematic.png
--rw-r--r--   0        0        0    25779 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/cartoon-schematic.svg
--rw-r--r--   0        0        0    18178 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    36024 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/example-hierarchy.png
--rw-r--r--   0        0        0    17092 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/example-hierarchy.svg
--rw-r--r--   0        0        0    21120 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/example-reduction-sum-only.svg
--rw-r--r--   0        0        0    29325 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    55553 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/example-reduction.png
--rw-r--r--   0        0        0    21631 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/example-reduction.svg
--rw-r--r--   0        0        0    10978 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/git-strategy.pdf
--rw-r--r--   0        0        0    58904 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/git-strategy.png
--rw-r--r--   0        0        0    28990 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/git-strategy.svg
--rw-r--r--   0        0        0   113587 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/how-it-works-muons.png
--rw-r--r--   0        0        0    57471 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/how-it-works-muons.svg
--rw-r--r--   0        0        0    58475 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/how-it-works.svg
--rw-r--r--   0        0        0    63989 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/sorting-axis.svg
--rw-r--r--   0        0        0   124038 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/reducers/all.svg
--rw-r--r--   0        0        0   128558 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/reducers/any.svg
--rw-r--r--   0        0        0   134490 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/reducers/argmax.svg
--rw-r--r--   0        0        0   133192 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/reducers/argmin.svg
--rw-r--r--   0        0        0   106277 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/reducers/count.svg
--rw-r--r--   0        0        0   116417 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/reducers/count_nonzero.svg
--rw-r--r--   0        0        0   111789 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/reducers/max.svg
--rw-r--r--   0        0        0   109239 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/reducers/min.svg
--rw-r--r--   0        0        0   124702 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/reducers/product.svg
--rw-r--r--   0        0        0   108897 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/diagrams/reducers/sum.svg
--rw-r--r--   0        0        0     8347 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/logo/favicon.ico
--rw-r--r--   0        0        0     8984 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/logo/logo-300px-white.png
--rw-r--r--   0        0        0    11964 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    24707 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/logo/logo-600px.png
--rw-r--r--   0        0        0    18767 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/logo/logo.svg
--rw-r--r--   0        0        0    90413 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/photos/desire-path.jpg
--rw-r--r--   0        0        0    52113 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/plots/awkward-0-popularity.pdf
--rw-r--r--   0        0        0   146109 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/plots/awkward-0-popularity.png
--rw-r--r--   0        0        0   147576 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/plots/awkward-0-popularity.svg
--rw-r--r--   0        0        0    26938 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/plots/bikeroutes-scaling.svg
--rw-r--r--   0        0        0     8891 2023-03-07 19:33:13.000000 awkward-2.1.1/docs-img/screenshots/github-issues-documentation.png
--rw-r--r--   0        0        0     1280 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/__init__.py
--rw-r--r--   0        0        0     8273 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_backends.py
--rw-r--r--   0        0        0     5418 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_behavior.py
--rw-r--r--   0        0        0    40413 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_broadcasting.py
--rw-r--r--   0        0        0    15599 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_do.py
--rw-r--r--   0        0        0    11819 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_errors.py
--rw-r--r--   0        0        0     5175 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_kernels.py
--rw-r--r--   0        0        0     5938 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_layout.py
--rw-r--r--   0        0        0    10028 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_lookup.py
--rw-r--r--   0        0        0     9988 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_prettyprint.py
--rw-r--r--   0        0        0    24743 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_reducers.py
--rw-r--r--   0        0        0     2040 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_regularize.py
--rw-r--r--   0        0        0      419 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_singleton.py
--rw-r--r--   0        0        0    24637 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_slicing.py
--rw-r--r--   0        0        0      647 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_typetracer.py
--rw-r--r--   0        0        0     2438 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_util.py
--rw-r--r--   0        0        0      773 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_v2.py
--rw-r--r--   0        0        0      233 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/builder.py
--rw-r--r--   0        0        0      271 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forth.py
--rw-r--r--   0        0        0   102475 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/highlevel.py
--rw-r--r--   0        0        0     8079 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/index.py
--rw-r--r--   0        0        0     4189 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/jax.py
--rw-r--r--   0        0        0     2764 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/numba.py
--rw-r--r--   0        0        0     8232 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/record.py
--rw-r--r--   0        0        0      165 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/typetracer.py
--rw-r--r--   0        0        0     1005 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/typing.py
--rw-r--r--   0        0        0       88 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/__init__.py
--rw-r--r--   0        0        0    32693 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/avro.py
--rw-r--r--   0        0        0    53671 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cling.py
--rw-r--r--   0        0        0     1036 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/hist.py
--rw-r--r--   0        0        0     4549 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/numexpr.py
--rw-r--r--   0        0        0    10119 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/numpy.py
--rw-r--r--   0        0        0    38401 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/pyarrow.py
--rw-r--r--   0        0        0     7175 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/__init__.py
--rw-r--r--   0        0        0     2555 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
--rw-r--r--   0        0        0     4326 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
--rw-r--r--   0        0        0      987 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
--rw-r--r--   0        0        0     2542 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3034 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0      630 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
--rw-r--r--   0        0        0      830 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3196 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
--rw-r--r--   0        0        0     2668 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0      749 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
--rw-r--r--   0        0        0     2749 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
--rw-r--r--   0        0        0      552 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
--rw-r--r--   0        0        0      637 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
--rw-r--r--   0        0        0     2886 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
--rw-r--r--   0        0        0     2904 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     3416 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0     3531 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
--rw-r--r--   0        0        0      556 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
--rw-r--r--   0        0        0      695 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
--rw-r--r--   0        0        0     3036 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
--rw-r--r--   0        0        0      795 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
--rw-r--r--   0        0        0     2523 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0     2729 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
--rw-r--r--   0        0        0     1035 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
--rw-r--r--   0        0        0      961 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
--rw-r--r--   0        0        0     2593 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
--rw-r--r--   0        0        0     1536 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
--rw-r--r--   0        0        0     1710 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     2012 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1184 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
--rw-r--r--   0        0        0      755 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu
--rw-r--r--   0        0        0      806 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
--rw-r--r--   0        0        0      744 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
--rw-r--r--   0        0        0     1169 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0     1059 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
--rw-r--r--   0        0        0     3208 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
--rw-r--r--   0        0        0      575 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
--rw-r--r--   0        0        0      830 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
--rw-r--r--   0        0        0      650 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
--rw-r--r--   0        0        0     2610 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
--rw-r--r--   0        0        0     1126 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
--rw-r--r--   0        0        0      951 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      721 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
--rw-r--r--   0        0        0     1003 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
--rw-r--r--   0        0        0     1339 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
--rw-r--r--   0        0        0      835 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
--rw-r--r--   0        0        0      975 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
--rw-r--r--   0        0        0      802 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
--rw-r--r--   0        0        0     1123 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu
--rw-r--r--   0        0        0      623 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu
--rw-r--r--   0        0        0      789 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
--rw-r--r--   0        0        0     1040 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     1020 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1045 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      974 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
--rw-r--r--   0        0        0      946 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
--rw-r--r--   0        0        0      980 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
--rw-r--r--   0        0        0      663 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
--rw-r--r--   0        0        0      586 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
--rw-r--r--   0        0        0     2580 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
--rw-r--r--   0        0        0     1360 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
--rw-r--r--   0        0        0      461 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
--rw-r--r--   0        0        0      534 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
--rw-r--r--   0        0        0      529 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
--rw-r--r--   0        0        0      830 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
--rw-r--r--   0        0        0      636 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
--rw-r--r--   0        0        0      689 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0      457 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
--rw-r--r--   0        0        0      830 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
--rw-r--r--   0        0        0     2043 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
--rw-r--r--   0        0        0     2198 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
--rw-r--r--   0        0        0     2043 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
--rw-r--r--   0        0        0     2198 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
--rw-r--r--   0        0        0     3054 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
--rw-r--r--   0        0        0     3289 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
--rw-r--r--   0        0        0     2022 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
--rw-r--r--   0        0        0     2022 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
--rw-r--r--   0        0        0     3202 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
--rw-r--r--   0        0        0     3012 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
--rw-r--r--   0        0        0     3171 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
--rw-r--r--   0        0        0     3439 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
--rw-r--r--   0        0        0     3439 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
--rw-r--r--   0        0        0      865 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
--rw-r--r--   0        0        0      443 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
--rw-r--r--   0        0        0     3195 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
--rw-r--r--   0        0        0     1859 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/header-only/awkward/BuilderOptions.h
--rw-r--r--   0        0        0    19587 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
--rw-r--r--   0        0        0    89307 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
--rw-r--r--   0        0        0      298 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/header-only/awkward/demo_impl.h
--rw-r--r--   0        0        0     8025 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/header-only/awkward/utils.h
--rw-r--r--   0        0        0      239 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/jax/__init__.py
--rw-r--r--   0        0        0     6816 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/jax/reducers.py
--rw-r--r--   0        0        0     6050 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/jax/trees.py
--rw-r--r--   0        0        0       88 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/numba/__init__.py
--rw-r--r--   0        0        0    35824 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/numba/arrayview.py
--rw-r--r--   0        0        0     1225 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/numba/arrayview_cuda.py
--rw-r--r--   0        0        0    31514 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/numba/builder.py
--rw-r--r--   0        0        0    49185 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/numba/layout.py
--rw-r--r--   0        0        0       88 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/rdataframe/__init__.py
--rw-r--r--   0        0        0     9269 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/rdataframe/from_rdataframe.py
--rw-r--r--   0        0        0     9770 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/rdataframe/to_rdataframe.py
--rw-r--r--   0        0        0     1487 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
--rw-r--r--   0        0        0     3762 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_nplikes/__init__.py
--rw-r--r--   0        0        0    12319 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_nplikes/array_module.py
--rw-r--r--   0        0        0     4920 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_nplikes/cupy.py
--rw-r--r--   0        0        0     2149 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_nplikes/jax.py
--rw-r--r--   0        0        0     2736 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_nplikes/numpy.py
--rw-r--r--   0        0        0    13659 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_nplikes/numpylike.py
--rw-r--r--   0        0        0     2733 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_nplikes/shape.py
--rw-r--r--   0        0        0    42339 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_nplikes/typetracer.py
--rw-r--r--   0        0        0     2527 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/_nplikes/ufuncs.py
--rw-r--r--   0        0        0       88 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/behaviors/__init__.py
--rw-r--r--   0        0        0     3479 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/behaviors/categorical.py
--rw-r--r--   0        0        0     3951 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/behaviors/mixins.py
--rw-r--r--   0        0        0     8636 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/behaviors/string.py
--rw-r--r--   0        0        0      986 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/contents/__init__.py
--rw-r--r--   0        0        0    28420 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/contents/bitmaskedarray.py
--rw-r--r--   0        0        0    41499 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/contents/bytemaskedarray.py
--rw-r--r--   0        0        0    47375 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/contents/content.py
--rw-r--r--   0        0        0    13487 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/contents/emptyarray.py
--rw-r--r--   0        0        0    41196 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/contents/indexedarray.py
--rw-r--r--   0        0        0    64328 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/contents/indexedoptionarray.py
--rw-r--r--   0        0        0    60811 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/contents/listarray.py
--rw-r--r--   0        0        0    86211 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/contents/listoffsetarray.py
--rw-r--r--   0        0        0    50194 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/contents/numpyarray.py
--rw-r--r--   0        0        0    42278 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/contents/recordarray.py
--rw-r--r--   0        0        0    55394 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/contents/regulararray.py
--rw-r--r--   0        0        0    58737 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/contents/unionarray.py
--rw-r--r--   0        0        0    19172 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/contents/unmaskedarray.py
--rw-r--r--   0        0        0      951 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forms/__init__.py
--rw-r--r--   0        0        0     6327 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forms/bitmaskedform.py
--rw-r--r--   0        0        0     5545 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forms/bytemaskedform.py
--rw-r--r--   0        0        0     3368 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forms/emptyform.py
--rw-r--r--   0        0        0    18495 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forms/form.py
--rw-r--r--   0        0        0     5907 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forms/indexedform.py
--rw-r--r--   0        0        0     5276 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forms/indexedoptionform.py
--rw-r--r--   0        0        0     5798 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forms/listform.py
--rw-r--r--   0        0        0     4754 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forms/listoffsetform.py
--rw-r--r--   0        0        0     6043 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forms/numpyform.py
--rw-r--r--   0        0        0     8592 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forms/recordform.py
--rw-r--r--   0        0        0     5192 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forms/regularform.py
--rw-r--r--   0        0        0     8014 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forms/unionform.py
--rw-r--r--   0        0        0     4356 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/forms/unmaskedform.py
--rw-r--r--   0        0        0     4779 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/__init__.py
--rw-r--r--   0        0        0     4021 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_all.py
--rw-r--r--   0        0        0     5218 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_almost_equal.py
--rw-r--r--   0        0        0     4024 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_any.py
--rw-r--r--   0        0        0     5049 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_argcartesian.py
--rw-r--r--   0        0        0     3864 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_argcombinations.py
--rw-r--r--   0        0        0     6934 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_argmax.py
--rw-r--r--   0        0        0     6891 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_argmin.py
--rw-r--r--   0        0        0     3211 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_argsort.py
--rw-r--r--   0        0        0      915 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_backend.py
--rw-r--r--   0        0        0     9529 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_broadcast_arrays.py
--rw-r--r--   0        0        0     6637 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_broadcast_fields.py
--rw-r--r--   0        0        0    16525 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_cartesian.py
--rw-r--r--   0        0        0     1420 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_categories.py
--rw-r--r--   0        0        0     8118 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_combinations.py
--rw-r--r--   0        0        0    11580 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_concatenate.py
--rw-r--r--   0        0        0     2715 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_copy.py
--rw-r--r--   0        0        0     5840 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_corr.py
--rw-r--r--   0        0        0     5251 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_count.py
--rw-r--r--   0        0        0     4058 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_count_nonzero.py
--rw-r--r--   0        0        0     5193 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_covar.py
--rw-r--r--   0        0        0     4717 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_drop_none.py
--rw-r--r--   0        0        0     1106 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_fields.py
--rw-r--r--   0        0        0     5284 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_fill_none.py
--rw-r--r--   0        0        0     3546 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_firsts.py
--rw-r--r--   0        0        0     7802 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_flatten.py
--rw-r--r--   0        0        0     3154 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_from_arrow.py
--rw-r--r--   0        0        0      813 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_from_arrow_schema.py
--rw-r--r--   0        0        0     2795 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_from_avro_file.py
--rw-r--r--   0        0        0    14718 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_from_buffers.py
--rw-r--r--   0        0        0     1839 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_from_categorical.py
--rw-r--r--   0        0        0     1651 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_from_cupy.py
--rw-r--r--   0        0        0     3905 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_from_iter.py
--rw-r--r--   0        0        0     1716 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_from_jax.py
--rw-r--r--   0        0        0    30666 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_from_json.py
--rw-r--r--   0        0        0     2282 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_from_numpy.py
--rw-r--r--   0        0        0    12103 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_from_parquet.py
--rw-r--r--   0        0        0     3434 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_from_rdataframe.py
--rw-r--r--   0        0        0     3034 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_from_regular.py
--rw-r--r--   0        0        0     8859 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_full_like.py
--rw-r--r--   0        0        0      873 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_is_categorical.py
--rw-r--r--   0        0        0     2576 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_is_none.py
--rw-r--r--   0        0        0      705 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_is_tuple.py
--rw-r--r--   0        0        0      930 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_is_valid.py
--rw-r--r--   0        0        0     2568 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_isclose.py
--rw-r--r--   0        0        0     9122 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_linear_fit.py
--rw-r--r--   0        0        0     3258 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_local_index.py
--rw-r--r--   0        0        0     4818 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_mask.py
--rw-r--r--   0        0        0     7476 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_max.py
--rw-r--r--   0        0        0     9113 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_mean.py
--rw-r--r--   0        0        0     3585 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_merge_option_of_records.py
--rw-r--r--   0        0        0    12395 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_merge_union_of_records.py
--rw-r--r--   0        0        0     3217 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_metadata_from_parquet.py
--rw-r--r--   0        0        0     7428 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_min.py
--rw-r--r--   0        0        0     4931 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_moment.py
--rw-r--r--   0        0        0     2081 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_nan_to_none.py
--rw-r--r--   0        0        0     5103 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_nan_to_num.py
--rw-r--r--   0        0        0     3972 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_num.py
--rw-r--r--   0        0        0     1951 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_ones_like.py
--rw-r--r--   0        0        0     4362 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_pad_none.py
--rw-r--r--   0        0        0     1786 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_parameters.py
--rw-r--r--   0        0        0     6406 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_prod.py
--rw-r--r--   0        0        0     4733 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_ptp.py
--rw-r--r--   0        0        0     2275 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_ravel.py
--rw-r--r--   0        0        0     9734 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_run_lengths.py
--rw-r--r--   0        0        0     3126 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_singletons.py
--rw-r--r--   0        0        0     3362 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_softmax.py
--rw-r--r--   0        0        0     2723 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_sort.py
--rw-r--r--   0        0        0     8170 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_std.py
--rw-r--r--   0        0        0     3058 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_strings_astype.py
--rw-r--r--   0        0        0    11764 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_sum.py
--rw-r--r--   0        0        0     4931 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_arrow.py
--rw-r--r--   0        0        0     6725 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_arrow_table.py
--rw-r--r--   0        0        0     2325 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_backend.py
--rw-r--r--   0        0        0     6333 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_buffers.py
--rw-r--r--   0        0        0     6050 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_categorical.py
--rw-r--r--   0        0        0     1073 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_cupy.py
--rw-r--r--   0        0        0    13423 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_dataframe.py
--rw-r--r--   0        0        0     1074 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_jax.py
--rw-r--r--   0        0        0    11720 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_json.py
--rw-r--r--   0        0        0     4669 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_layout.py
--rw-r--r--   0        0        0     2612 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_list.py
--rw-r--r--   0        0        0     2088 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_numpy.py
--rw-r--r--   0        0        0     3354 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_packed.py
--rw-r--r--   0        0        0    16968 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_parquet.py
--rw-r--r--   0        0        0     2946 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_rdataframe.py
--rw-r--r--   0        0        0     3416 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_to_regular.py
--rw-r--r--   0        0        0    24129 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_transform.py
--rw-r--r--   0        0        0     4357 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_type.py
--rw-r--r--   0        0        0     9840 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_unflatten.py
--rw-r--r--   0        0        0     2611 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_unzip.py
--rw-r--r--   0        0        0     1161 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_validity_error.py
--rw-r--r--   0        0        0     2659 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_values_astype.py
--rw-r--r--   0        0        0     9398 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_var.py
--rw-r--r--   0        0        0     5604 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_where.py
--rw-r--r--   0        0        0     5175 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_with_field.py
--rw-r--r--   0        0        0     2610 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_with_name.py
--rw-r--r--   0        0        0     1848 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_with_parameter.py
--rw-r--r--   0        0        0     3809 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_without_field.py
--rw-r--r--   0        0        0     1509 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_without_parameters.py
--rw-r--r--   0        0        0     2134 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_zeros_like.py
--rw-r--r--   0        0        0     8952 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/operations/ak_zip.py
--rw-r--r--   0        0        0      707 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/types/__init__.py
--rw-r--r--   0        0        0   163323 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/types/_awkward_datashape_parser.py
--rw-r--r--   0        0        0     1905 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/types/arraytype.py
--rw-r--r--   0        0        0     2562 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/types/listtype.py
--rw-r--r--   0        0        0     5813 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/types/numpytype.py
--rw-r--r--   0        0        0     4193 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/types/optiontype.py
--rw-r--r--   0        0        0     7888 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/types/recordtype.py
--rw-r--r--   0        0        0     3283 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/types/regulartype.py
--rw-r--r--   0        0        0     1090 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/types/scalartype.py
--rw-r--r--   0        0        0     9367 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/types/type.py
--rw-r--r--   0        0        0     3605 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/types/uniontype.py
--rw-r--r--   0        0        0     1960 2023-03-07 19:33:13.000000 awkward-2.1.1/src/awkward/types/unknowntype.py
--rw-r--r--   0        0        0       88 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/__init__.py
--rw-r--r--   0        0        0     3358 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0002_minimal_listarray.py
--rw-r--r--   0        0        0      487 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0006_deep_iteration.py
--rw-r--r--   0        0        0     5565 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0008_slices_and_getitem.py
--rw-r--r--   0        0        0    13378 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0011_listarray.py
--rw-r--r--   0        0        0     4462 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0013_error_handling_struct.py
--rw-r--r--   0        0        0    17019 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0014_finish_up_getitem.py
--rw-r--r--   0        0        0     5169 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0018_fromiter_fillable.py
--rw-r--r--   0        0        0     8833 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0019_use_json_library.py
--rw-r--r--   0        0        0    13687 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0020_support_unsigned_indexes.py
--rw-r--r--   0        0        0     6966 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0021_emptyarray.py
--rw-r--r--   0        0        0    10743 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0023_regular_array.py
--rw-r--r--   0        0        0     4890 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0024_use_regular_array.py
--rw-r--r--   0        0        0    25581 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0025_record_array.py
--rw-r--r--   0        0        0     3436 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0028_add_dressed_types.py
--rw-r--r--   0        0        0     6361 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0032_replace_dressedtype.py
--rw-r--r--   0        0        0    12027 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0046_start_indexedarray.py
--rw-r--r--   0        0        0      898 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
--rw-r--r--   0        0        0    12231 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0057_introducing_forms.py
--rw-r--r--   0        0        0     5430 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0070_argmin_and_argmax.py
--rw-r--r--   0        0        0     5384 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0072_fillna_operation.py
--rw-r--r--   0        0        0    15655 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0074_argsort_and_sort.py
--rw-r--r--   0        0        0     2836 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0077_zip_operation.py
--rw-r--r--   0        0        0    11934 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0078_argcross_and_cross.py
--rw-r--r--   0        0        0    12124 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0079_argchoose_and_choose.py
--rw-r--r--   0        0        0     7071 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
--rw-r--r--   0        0        0     6579 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0084_start_unionarray.py
--rw-r--r--   0        0        0     6551 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0086_nep13_ufunc.py
--rw-r--r--   0        0        0    12540 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0089_numpy_functions.py
--rw-r--r--   0        0        0    46684 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0093_simplify_uniontypes_and_optiontypes.py
--rw-r--r--   0        0        0     6959 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0107_assign_fields_to_records.py
--rw-r--r--   0        0        0    46658 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0111_jagged_and_masked_getitem.py
--rw-r--r--   0        0        0    77224 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0115_generic_reducer_operation.py
--rw-r--r--   0        0        0    35084 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0118_numba_cpointers.py
--rw-r--r--   0        0        0     1091 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0119_numexpr_and_broadcast_arrays.py
--rw-r--r--   0        0        0     1106 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0124_strings_in_numba.py
--rw-r--r--   0        0        0    32114 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0127_tomask_operation.py
--rw-r--r--   0        0        0     3683 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0127b_tomask_operation_numba.py
--rw-r--r--   0        0        0      838 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0138_emptyarray_type.py
--rw-r--r--   0        0        0    17923 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0150_flatten.py
--rw-r--r--   0        0        0     3602 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0163_negative_axis_wrap.py
--rw-r--r--   0        0        0     9779 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0166_0167_0170_random_issues.py
--rw-r--r--   0        0        0     4552 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0173_astype_operation.py
--rw-r--r--   0        0        0    24034 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0184_concatenate_operation.py
--rw-r--r--   0        0        0     2063 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0193_is_none_axis_parameter.py
--rw-r--r--   0        0        0     3352 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0198_tutorial_documentation_1.py
--rw-r--r--   0        0        0     8998 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0222_count_with_axis0.py
--rw-r--r--   0        0        0    75605 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0224_arrow_to_awkward.py
--rw-r--r--   0        0        0      581 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0264_reduce_last_empty.py
--rw-r--r--   0        0        0     3251 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0273_path_for_with_field.py
--rw-r--r--   0        0        0      743 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0286_broadcast_single_value_with_field.py
--rw-r--r--   0        0        0     2205 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0290_bug_fixes_for_hats.py
--rw-r--r--   0        0        0     4806 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0315_integerindex.py
--rw-r--r--   0        0        0     5745 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0331_pandas_indexedarray.py
--rw-r--r--   0        0        0     1257 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0334_fully_broadcastable_where.py
--rw-r--r--   0        0        0      566 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0339_highlevel_sorting_function.py
--rw-r--r--   0        0        0     6757 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0348_form_keys.py
--rw-r--r--   0        0        0     4523 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0355_mixins.py
--rw-r--r--   0        0        0    10396 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0395_complex_type_arrays.py
--rw-r--r--   0        0        0     4934 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0395_fix_numba_indexedarray.py
--rw-r--r--   0        0        0     3077 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0397_arrays_as_constants_in_numba.py
--rw-r--r--   0        0        0    14529 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
--rw-r--r--   0        0        0    22467 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0404_array_validity_check.py
--rw-r--r--   0        0        0    14282 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0410_fix_argminmax_positions_for_missing_values.py
--rw-r--r--   0        0        0    17455 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0437_stream_of_many_json_files.py
--rw-r--r--   0        0        0    32921 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0447_preserve_regularness_in_reduce.py
--rw-r--r--   0        0        0    24075 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0449_merge_many_arrays_in_one_pass.py
--rw-r--r--   0        0        0     4059 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0493_zeros_ones_full_like.py
--rw-r--r--   0        0        0     1606 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0496_provide_local_index.py
--rw-r--r--   0        0        0     2059 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0499_getitem_indexedarray_bug.py
--rw-r--r--   0        0        0     1286 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0504_block_ufuncs_for_strings.py
--rw-r--r--   0        0        0     2926 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0511_copy_and_deepcopy.py
--rw-r--r--   0        0        0     9119 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
--rw-r--r--   0        0        0      365 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0546_fill_none_replacement_value_type.py
--rw-r--r--   0        0        0     1102 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0549_numba_array_asarray.py
--rw-r--r--   0        0        0     4268 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0557_min_max_initial_argument.py
--rw-r--r--   0        0        0      537 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0559_fix_booleans_in_numba.py
--rw-r--r--   0        0        0      636 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0572_numba_array_ndim.py
--rw-r--r--   0        0        0     4901 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0582_propagate_context_in_broadcast_and_apply.py
--rw-r--r--   0        0        0     1099 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0583_implement_unflatten_function.py
--rw-r--r--   0        0        0     3084 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0590_allow_regulararray_size_zero.py
--rw-r--r--   0        0        0     5957 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
--rw-r--r--   0        0        0      478 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0627_behavior_from_dict_of_arrays.py
--rw-r--r--   0        0        0     8205 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0652_tests_of_complex_numbers.py
--rw-r--r--   0        0        0     2338 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0674_categorical_validation.py
--rw-r--r--   0        0        0      750 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0713_getitem_field_should_simplify_optiontype.py
--rw-r--r--   0        0        0     1242 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
--rw-r--r--   0        0        0     1055 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0730_unflatten_axis_parameter.py
--rw-r--r--   0        0        0     2569 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0733_run_lengths.py
--rw-r--r--   0        0        0     2127 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0736_implement_argsort_for_strings.py
--rw-r--r--   0        0        0      330 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0758_ak_zip_scallars.py
--rw-r--r--   0        0        0     1122 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0766_prevent_combinations_of_characters.py
--rw-r--r--   0        0        0    26349 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0773_typeparser.py
--rw-r--r--   0        0        0      779 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
--rw-r--r--   0        0        0      871 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0794_ak_cartesian_on_empty_array.py
--rw-r--r--   0        0        0     1148 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0803_argsort_fix_type.py
--rw-r--r--   0        0        0     1364 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0806_empty_lists_cartesian_fix.py
--rw-r--r--   0        0        0     6311 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0813_full_like_dtype_arg.py
--rw-r--r--   0        0        0     1661 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0815_broadcast_union_types_to_all_possibilities.py
--rw-r--r--   0        0        0      488 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0819_issue.py
--rw-r--r--   0        0        0      682 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0828_arrow_datatype_null.py
--rw-r--r--   0        0        0    23609 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0835_datetime_type.py
--rw-r--r--   0        0        0      676 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0835_datetime_type_pandas.py
--rw-r--r--   0        0        0     4662 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0835_datetime_type_pyarrow.py
--rw-r--r--   0        0        0      680 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0850_argsort_mask_array.py
--rw-r--r--   0        0        0      449 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0863_is_none_numpy_array.py
--rw-r--r--   0        0        0     1029 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0866_getitem_field_and_flatten_unions.py
--rw-r--r--   0        0        0      929 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0875_arrow_null_type.py
--rw-r--r--   0        0        0      901 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0879_non_primitive_with_field.py
--rw-r--r--   0        0        0      563 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0884_index_and_identifier_refactoring.py
--rw-r--r--   0        0        0     1086 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0889_ptp.py
--rw-r--r--   0        0        0    53355 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0896_content_classes_refactoring.py
--rw-r--r--   0        0        0     1751 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0898_unzip_heterogeneous_records.py
--rw-r--r--   0        0        0      421 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
--rw-r--r--   0        0        0      530 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0905_leading_zeros_in_unflatten.py
--rw-r--r--   0        0        0     1048 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0906_arrow_fixed_size_list_type.py
--rw-r--r--   0        0        0      666 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0910_unflatten_counts_relation.py
--rw-r--r--   0        0        0     5261 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0912_packed.py
--rw-r--r--   0        0        0   115760 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0914_types_and_forms.py
--rw-r--r--   0        0        0     1877 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0916_datetime_values_astype.py
--rw-r--r--   0        0        0     5522 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0927_numpy_array_nbytes.py
--rw-r--r--   0        0        0      709 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0930_bug_in_unionarray_purelist_parameter.py
--rw-r--r--   0        0        0     1627 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0945_argsort_sort_nan_array.py
--rw-r--r--   0        0        0    28028 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0958_new_forms_must_accept_old_form_json.py
--rw-r--r--   0        0        0    28284 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0959__getitem_array_implementation.py
--rw-r--r--   0        0        0      651 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0975_mask_multidimensional_numpy_array.py
--rw-r--r--   0        0        0      644 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0979_where_multidimentional_numpy_array.py
--rw-r--r--   0        0        0     5803 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0982_missing_case_in_nonlocal_reducers.py
--rw-r--r--   0        0        0     1976 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0984_ravel.py
--rw-r--r--   0        0        0     1806 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_0992_correct_ptp_unmasking.py
--rw-r--r--   0        0        0     2100 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
--rw-r--r--   0        0        0      429 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1006_packed_regular_array_zero_size.py
--rw-r--r--   0        0        0      416 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1007_from_buffers_empty_ndarray.py
--rw-r--r--   0        0        0      551 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1017_numpyarray_broadcast.py
--rw-r--r--   0        0        0      785 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1030_mixin_class_name.py
--rw-r--r--   0        0        0    52114 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1031_start_getitem_next.py
--rw-r--r--   0        0        0    18007 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1031b_start_getitem_next_specialized.py
--rw-r--r--   0        0        0     1146 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1049_concatenate_single_array.py
--rw-r--r--   0        0        0     1559 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1055_fill_none_numpy_dimension.py
--rw-r--r--   0        0        0    42250 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1059_localindex.py
--rw-r--r--   0        0        0      551 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1066_to_numpy_masked_structured_array.py
--rw-r--r--   0        0        0      685 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1071_mask_identity_false_should_not_return_option_type.py
--rw-r--r--   0        0        0    27714 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1072_sort.py
--rw-r--r--   0        0        0    44140 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1074_combinations.py
--rw-r--r--   0        0        0     5181 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1075_validityerror.py
--rw-r--r--   0        0        0      273 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1106_argminmax_axis_None_missing_values.py
--rw-r--r--   0        0        0    25531 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1110_type_tracer_1.py
--rw-r--r--   0        0        0     1870 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1116_project_maskedarrays.py
--rw-r--r--   0        0        0    28234 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1125_to_arrow_from_arrow.py
--rw-r--r--   0        0        0     6276 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1132_utility_methods_for_highlevel_functions.py
--rw-r--r--   0        0        0    21098 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1134_from_buffers_to_buffers.py
--rw-r--r--   0        0        0    57322 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1135_rpad_operation.py
--rw-r--r--   0        0        0     4639 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1136_regulararray_zeros_in_shape.py
--rw-r--r--   0        0        0    10487 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1137_num.py
--rw-r--r--   0        0        0    10222 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1142_numbers_to_type.py
--rw-r--r--   0        0        0     2559 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1149_datetime_sort.py
--rw-r--r--   0        0        0      630 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1154_arrow_tables_should_preserve_parameters.py
--rw-r--r--   0        0        0    27983 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1162_ak_from_json_schema.py
--rw-r--r--   0        0        0      766 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1183_bugs_found_by_dask_project_2.py
--rw-r--r--   0        0        0     1286 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1189_fix_singletons_for_non_optional_data.py
--rw-r--r--   0        0        0      551 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1192_iterables_in___array_function__.py
--rw-r--r--   0        0        0      608 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1193_is_none_nested_option.py
--rw-r--r--   0        0        0     2601 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1233_ak_with_name.py
--rw-r--r--   0        0        0    26467 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1240_v2_implementation_of_numba_1.py
--rw-r--r--   0        0        0     1146 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1259_simplify_optiontype.py
--rw-r--r--   0        0        0     1560 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1260_simplify_masked_option_types.py
--rw-r--r--   0        0        0      681 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1271_fix_4D_reducers.py
--rw-r--r--   0        0        0    33003 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1294_to_and_from_parquet.py
--rw-r--r--   0        0        0     1945 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
--rw-r--r--   0        0        0    62340 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1300_awkward_to_cpp_converter_with_cling.py
--rw-r--r--   0        0        0    39474 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1300b_same_for_numba.py
--rw-r--r--   0        0        0      367 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1305_mixed_awkward_numpy_slicing.py
--rw-r--r--   0        0        0     1702 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1308_zip_after_option.py
--rw-r--r--   0        0        0     1703 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1318_array_function_types.py
--rw-r--r--   0        0        0     1730 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1320_mask_identity_defaults.py
--rw-r--r--   0        0        0      647 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1344_broadcast_arrays_depth_limit.py
--rw-r--r--   0        0        0     6621 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1345_avro_reader.py
--rw-r--r--   0        0        0     4562 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1351_is_tuple.py
--rw-r--r--   0        0        0     8362 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1374_to_rdataframe.py
--rw-r--r--   0        0        0     1755 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1377_ravel_string.py
--rw-r--r--   0        0        0     1468 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1379_reducers_with_axis_None_and_typetracers.py
--rw-r--r--   0        0        0     1384 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1399_from_jax.py
--rw-r--r--   0        0        0     1227 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1399_to_jax.py
--rw-r--r--   0        0        0      297 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1400_with_name_record.py
--rw-r--r--   0        0        0      449 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1403_from_numpy_strings.py
--rw-r--r--   0        0        0     3470 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1405_slicing_untested_cases.py
--rw-r--r--   0        0        0     6909 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1415_behaviour_forwarding.py
--rw-r--r--   0        0        0    18809 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1440_start_v2_to_parquet.py
--rw-r--r--   0        0        0    14402 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1447_jax_autodiff_slices_ufuncs.py
--rw-r--r--   0        0        0     8591 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1449_v2_to_json_from_json_functions.py
--rw-r--r--   0        0        0      692 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1453_write_single_records_to_parquet.py
--rw-r--r--   0        0        0     9828 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1473_from_rdataframe.py
--rw-r--r--   0        0        0    24648 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1477_generator_entry_type_as_rvec.py
--rw-r--r--   0        0        0     3579 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1490_jax_reducers_combinations.py
--rw-r--r--   0        0        0     3905 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1502_getitem_jagged_issue1406.py
--rw-r--r--   0        0        0     1733 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1504_typetracer_like.py
--rw-r--r--   0        0        0     4913 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1508_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     2186 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1511_set_attribute.py
--rw-r--r--   0        0        0      754 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1539_isnone_axis_check_issue1417.py
--rw-r--r--   0        0        0     1570 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1559_fix_ufuncs_records_1439.py
--rw-r--r--   0        0        0      990 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1565_axis_wrap_if_negative_record.py
--rw-r--r--   0        0        0     1080 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1567_fix_longlong_in_Index.py
--rw-r--r--   0        0        0     3022 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1568_fix_lengths_empty_regular_slices.py
--rw-r--r--   0        0        0      385 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1578_to_arrow_empty_recordarray.py
--rw-r--r--   0        0        0     5911 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1586_concatenate_should_preserve_regulararray.py
--rw-r--r--   0        0        0      216 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1593_empty_slice_list_record.py
--rw-r--r--   0        0        0     7260 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1604_preserve_form_in_concatenate.py
--rw-r--r--   0        0        0     3636 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1607_no_reducers_on_records.py
--rw-r--r--   0        0        0    10035 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1613_generator_tolayout_records.py
--rw-r--r--   0        0        0      727 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1619_from_parquet_empty_field.py
--rw-r--r--   0        0        0     6024 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1620_layout_builders.py
--rw-r--r--   0        0        0     8122 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1625_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0      770 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1642_from_iter_of_tuples.py
--rw-r--r--   0        0        0      389 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1644_concatenate_zeros_length.py
--rw-r--r--   0        0        0     4317 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1650_Record_to_list_should_listify_itself.py
--rw-r--r--   0        0        0      560 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1671_categorical_type.py
--rw-r--r--   0        0        0    11761 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1672_broadcast_parameters.py
--rw-r--r--   0        0        0     4453 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1677_array_builder_in_numba.py
--rw-r--r--   0        0        0      544 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1685_IndexedArray_project_parameters.py
--rw-r--r--   0        0        0      778 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1686_UnionArray_simplified_preserve_parameters.py
--rw-r--r--   0        0        0      936 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1688_pack_categorical.py
--rw-r--r--   0        0        0      525 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1703_fill_none_typetracer.py
--rw-r--r--   0        0        0     1743 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1707_broadcast_parameters_ufunc.py
--rw-r--r--   0        0        0      512 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1709_ak_array_constructor_behavior.py
--rw-r--r--   0        0        0      398 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1735_from_numpy_mask.py
--rw-r--r--   0        0        0      577 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1747_bytemaskedarray_mergemany.py
--rw-r--r--   0        0        0      824 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1753_indexedarray_merge_kernel.py
--rw-r--r--   0        0        0     1480 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1762_jax_behavior_support.py
--rw-r--r--   0        0        0      589 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1764_jax_jacobian.py
--rw-r--r--   0        0        0      962 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1765_add_ioanas_test_of_to_arraylib.py
--rw-r--r--   0        0        0     4790 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1766_record_form_fields.py
--rw-r--r--   0        0        0     2905 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1781_rdataframe_snapshot.py
--rw-r--r--   0        0        0      701 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1784_reduce_leading_sublist.py
--rw-r--r--   0        0        0      567 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1790_reduce_regulararray.py
--rw-r--r--   0        0        0     4191 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1791_reduce_trailing_sublist.py
--rw-r--r--   0        0        0     1027 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1794_run_lengths_empty_sublist.py
--rw-r--r--   0        0        0      407 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1823_fill_none_axis_none.py
--rw-r--r--   0        0        0      481 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1826_ravel_preserve_none.py
--rw-r--r--   0        0        0     1451 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1829_to_from_rdataframe_bool.py
--rw-r--r--   0        0        0      588 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
--rw-r--r--   0        0        0     1097 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1847_numpy_array_contiguous.py
--rw-r--r--   0        0        0      681 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
--rw-r--r--   0        0        0     1640 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1867_pass_behavior_through_combinations.py
--rw-r--r--   0        0        0    17239 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1904_drop_none.py
--rw-r--r--   0        0        0     3553 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1914_improved_axis_to_posaxis.py
--rw-r--r--   0        0        0     3444 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
--rw-r--r--   0        0        0      921 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1930_unflatten_counts_checks.py
--rw-r--r--   0        0        0      769 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1936_with_field_broadcasting.py
--rw-r--r--   0        0        0      551 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1940_ak_backend.py
--rw-r--r--   0        0        0     1457 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1943_regular_indexing.py
--rw-r--r--   0        0        0      188 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1944_to_numpy_empty_record_array.py
--rw-r--r--   0        0        0     1131 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1960_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     3286 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1961_ak_without_field.py
--rw-r--r--   0        0        0      280 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1978_akRecord_constructor_should_retain_type.py
--rw-r--r--   0        0        0      349 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
--rw-r--r--   0        0        0      371 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2008_ak_type_layout.py
--rw-r--r--   0        0        0    10222 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2020_reduce_axis_none.py
--rw-r--r--   0        0        0      803 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2021_check_TypeTracerArray_in_ak_where.py
--rw-r--r--   0        0        0      645 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2023_from_rdataframe.py
--rw-r--r--   0        0        0     2854 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
--rw-r--r--   0        0        0     1219 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2047_ak_transform_regular_to_jagged.py
--rw-r--r--   0        0        0      406 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2051_arraybuilder_behavior_propagation.py
--rw-r--r--   0        0        0     1275 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2055_array_builder_check.py
--rw-r--r--   0        0        0     1659 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2058_merge_numpy_array.py
--rw-r--r--   0        0        0      708 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2064_fill_none_record.py
--rw-r--r--   0        0        0      799 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2067_to_buffers_byteorder.py
--rw-r--r--   0        0        0      741 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2070_to_layout_string.py
--rw-r--r--   0        0        0     1172 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2071_unflatten_non_packed_counts.py
--rw-r--r--   0        0        0      291 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2076_ak_unzip_record.py
--rw-r--r--   0        0        0      545 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2078_array_function_wrap.py
--rw-r--r--   0        0        0      589 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2082_broadcast_zero_size.py
--rw-r--r--   0        0        0     2765 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2096_ak_scalar_type.py
--rw-r--r--   0        0        0      977 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2101_pickle_behavior_class.py
--rw-r--r--   0        0        0      519 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2104_numpy_merge_option.py
--rw-r--r--   0        0        0     2715 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2106_pickle_class.py
--rw-r--r--   0        0        0      722 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2108_fill_none_indexed.py
--rw-r--r--   0        0        0     2100 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2115_fix_up_typetracers.py
--rw-r--r--   0        0        0      487 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2120_missing_field_error.py
--rw-r--r--   0        0        0     1110 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2125_type_of_scalar.py
--rw-r--r--   0        0        0     1893 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2150_typetracer_high_level_ufunc.py
--rw-r--r--   0        0        0     1898 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2179_parameter_merging_rules.py
--rw-r--r--   0        0        0      510 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2181_with_name_len.py
--rw-r--r--   0        0        0     2957 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2185_merge_union_of_records.py
--rw-r--r--   0        0        0      528 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
--rw-r--r--   0        0        0     5548 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2198_almost_equal.py
--rw-r--r--   0        0        0     1252 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2202_filter_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0     1453 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2214_offset_bool_index.py
--rw-r--r--   0        0        0      334 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2219_flatten_empty.py
--rw-r--r--   0        0        0      663 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2226_slice_regulararray_typetracer.py
--rw-r--r--   0        0        0     1728 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2229_getitem_range_slice.py
--rw-r--r--   0        0        0     4003 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2234_from_rdataframe_keep_order.py
--rw-r--r--   0        0        0     3962 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2236_merge_union_of_records_option.py
--rw-r--r--   0        0        0      485 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2240_merge_union_parameters.py
--rw-r--r--   0        0        0     1338 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2240_simplify_merge_as_union.py
--rw-r--r--   0        0        0      512 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2246_slice_not_packed.py
--rw-r--r--   0        0        0      733 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2250_full_like_bool.py
--rw-r--r--   0        0        0     1835 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2258_from_rdataframe_with_arguments.py
--rw-r--r--   0        0        0      492 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2259_run_lengths_typetracer.py
--rw-r--r--   0        0        0      549 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2263_to_packed_list.py
--rw-r--r--   0        0        0      877 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2266_fix_nan_to_num.py
--rw-r--r--   0        0        0      909 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2267_broadcast_fields.py
--rw-r--r--   0        0        0     1336 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2293_unflatten_typetracer.py
--rw-r--r--   0        0        0      406 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2294_view_unknown_scalar.py
--rw-r--r--   0        0        0     2301 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2297_common_backend.py
--rw-r--r--   0        0        0      455 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2304_index_typetracer.py
--rw-r--r--   0        0        0     4386 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/test_2319_from_buffers_array.py
--rw-r--r--   0        0        0      128 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/__init__.py
--rw-r--r--   0        0        0      218 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/array_enum_test_data.avro
--rw-r--r--   0        0        0      176 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/array_string_test_data.avro
--rw-r--r--   0        0        0      152 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/array_test_data.avro
--rw-r--r--   0        0        0      115 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/bool_test_data.avro
--rw-r--r--   0        0        0      130 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/bytes_test_data.avro
--rw-r--r--   0        0        0      158 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/double_test_data.avro
--rw-r--r--   0        0        0      191 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/enum_null_test_data.avro
--rw-r--r--   0        0        0      180 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/enum_test_data.avro
--rw-r--r--   0        0        0      218 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/fixed_test_data.avro
--rw-r--r--   0        0        0      116 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/float_test_data.avro
--rw-r--r--   0        0        0      106 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/int_null_test_data.avro
--rw-r--r--   0        0        0      128 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/int_string_null_test_data.avro
--rw-r--r--   0        0        0       89 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/int_test_data.avro
--rw-r--r--   0        0        0     3035 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/list-depths-records-list.parquet
--rw-r--r--   0        0        0     2871 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/list-depths-records.parquet
--rw-r--r--   0        0        0      497 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/list-depths-simple.parquet
--rw-r--r--   0        0        0     1136 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/list-depths-strings.parquet
--rw-r--r--   0        0        0     1060 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/list-depths.parquet
--rw-r--r--   0        0        0      465 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/list-lengths.parquet
--rw-r--r--   0        0        0      116 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/long_test_data.avro
--rw-r--r--   0        0        0      681 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/nonnullable-depths.parquet
--rw-r--r--   0        0        0       75 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/null_test_data.avro
--rw-r--r--   0        0        0      719 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/nullable-depths.parquet
--rw-r--r--   0        0        0      635 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/nullable-levels.parquet
--rw-r--r--   0        0        0     3050 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/nullable-list-depths-records-list.parquet
--rw-r--r--   0        0        0     2926 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/nullable-list-depths-records.parquet
--rw-r--r--   0        0        0     1179 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/nullable-list-depths-strings.parquet
--rw-r--r--   0        0        0     1101 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/nullable-list-depths.parquet
--rw-r--r--   0        0        0      430 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/nullable-record-primitives-simple.parquet
--rw-r--r--   0        0        0     1181 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/nullable-record-primitives.parquet
--rw-r--r--   0        0        0     1193 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/record-primitives.parquet
--rw-r--r--   0        0        0      326 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/record_0_test_data.avro
--rw-r--r--   0        0        0      368 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/record_1_test_data.avro
--rw-r--r--   0        0        0      263 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/record_null_test_data.avro
--rw-r--r--   0        0        0      423 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/record_test_data.avro
--rw-r--r--   0        0        0      116 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/string_null_test_data.avro
--rw-r--r--   0        0        0      125 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/string_test_data.avro
--rw-r--r--   0        0        0      544 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/test-nan-inf.json
--rw-r--r--   0        0        0      155 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/test-record-array.json
--rw-r--r--   0        0        0      803 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/test-two-arrays.json
--rw-r--r--   0        0        0      535 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/test.json
--rw-r--r--   0        0        0      180 2023-03-07 19:33:13.000000 awkward-2.1.1/tests/samples/zero-record-batches.parquet
--rw-r--r--   0        0        0       88 2023-03-07 19:33:13.000000 awkward-2.1.1/tests-cuda/__init__.py
--rw-r--r--   0        0        0     7072 2023-03-07 19:33:13.000000 awkward-2.1.1/tests-cuda/test_1276_cuda_num.py
--rw-r--r--   0        0        0     9911 2023-03-07 19:33:13.000000 awkward-2.1.1/tests-cuda/test_1276_cuda_transfers.py
--rw-r--r--   0        0        0     1197 2023-03-07 19:33:13.000000 awkward-2.1.1/tests-cuda/test_1276_cupy_interop.py
--rw-r--r--   0        0        0     1782 2023-03-07 19:33:13.000000 awkward-2.1.1/tests-cuda/test_1276_from_cupy.py
--rw-r--r--   0        0        0    42786 2023-03-07 19:33:13.000000 awkward-2.1.1/tests-cuda/test_1300_same_for_numba_cuda.py
--rw-r--r--   0        0        0      834 2023-03-07 19:33:13.000000 awkward-2.1.1/tests-cuda/test_1381_check_errors.py
--rw-r--r--   0        0        0    11252 2023-03-07 19:33:13.000000 awkward-2.1.1/tests-cuda/test_1809_array_cuda_jit.py
--rw-r--r--   0        0        0     2212 2023-03-07 19:33:13.000000 awkward-2.1.1/.gitignore
--rw-r--r--   0        0        0     1520 2023-03-07 19:33:13.000000 awkward-2.1.1/LICENSE
--rw-r--r--   0        0        0     8408 2023-03-07 19:33:13.000000 awkward-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     6911 2023-03-07 19:33:13.000000 awkward-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1893 2023-04-08 19:13:43.000000 awkward-2.1.2/CITATION.cff
+-rw-r--r--   0        0        0    13386 2023-04-08 19:13:43.000000 awkward-2.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    22687 2023-04-08 19:13:43.000000 awkward-2.1.2/README.md
+-rw-r--r--   0        0        0      241 2023-04-08 19:13:43.000000 awkward-2.1.2/requirements-test.txt
+-rw-r--r--   0        0        0     7833 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/_toc.yml
+-rw-r--r--   0        0        0     7624 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/conf.py
+-rw-r--r--   0        0        0      346 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/environment.yml.cog
+-rw-r--r--   0        0        0     2603 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/index.md
+-rw-r--r--   0        0        0    11642 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/prepare_docstrings.py
+-rw-r--r--   0        0        0     4448 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/redirects-user-guide.json
+-rw-r--r--   0        0        0    11436 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/redirects.json
+-rw-r--r--   0        0        0      463 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/requirements.txt
+-rw-r--r--   0        0        0      369 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/switcher.json
+-rw-r--r--   0        0        0      930 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/_static/css/awkward.css
+-rw-r--r--   0        0        0      354 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/_static/css/try-awkward-array.css
+lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
+lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0      469 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/_templates/funding.html
+-rw-r--r--   0        0        0      474 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/_templates/redirect.html
+-rw-r--r--   0        0        0     2968 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/getting-started/community-tutorials.md
+-rw-r--r--   0        0        0     4654 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/getting-started/index.md
+-rw-r--r--   0        0        0     3346 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/getting-started/papers-and-talks.md
+-rw-r--r--   0        0        0       82 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/getting-started/try-awkward-array.md
+lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    12847 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/getting-started/demo/what-is-an-awkward-array.ipynb
+lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
+lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
+lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
+lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    17067 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/example-hierarchy.svg
+lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
+lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
+lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
+lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
+lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
+lrwxr-xr-x   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    25309 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/reference/ak.behavior.rst
+-rw-r--r--   0        0        0     1430 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/reference/ak.builder.ArrayBuilder.rst
+-rw-r--r--   0        0        0    64727 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/reference/awkwardforth.rst
+-rw-r--r--   0        0        0      270 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/reference/index.md
+-rw-r--r--   0        0        0     7252 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/reference/toctree.txt
+-rw-r--r--   0        0        0     8320 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/10-minutes-to-awkward-array.md
+-rw-r--r--   0        0        0      926 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-combinatorics-best-match.md
+-rw-r--r--   0        0        0      930 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
+-rw-r--r--   0        0        0      263 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-combinatorics.md
+-rw-r--r--   0        0        0     8335 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert-arrow.md
+-rw-r--r--   0        0        0     6392 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert-buffers.md
+-rw-r--r--   0        0        0     2455 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert-json.md
+-rw-r--r--   0        0        0    13475 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert-numpy.md
+-rw-r--r--   0        0        0     7182 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert-pandas.md
+-rw-r--r--   0        0        0    18830 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert-python.md
+-rw-r--r--   0        0        0     3554 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert-rdataframe.md
+-rw-r--r--   0        0        0      271 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-convert.md
+-rw-r--r--   0        0        0    11973 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create-arraybuilder.md
+-rw-r--r--   0        0        0    36520 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create-constructors.md
+-rw-r--r--   0        0        0     7383 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create-lists.md
+-rw-r--r--   0        0        0     7456 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create-missing.md
+-rw-r--r--   0        0        0    11542 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create-records.md
+-rw-r--r--   0        0        0     4066 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create-strings.md
+-rw-r--r--   0        0        0      866 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create-unflatten-group.md
+-rw-r--r--   0        0        0      267 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-create.md
+-rw-r--r--   0        0        0      834 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-examine-checking-validity.md
+-rw-r--r--   0        0        0     2919 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-examine-list-fields.md
+-rw-r--r--   0        0        0      848 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-examine-simple-slicing.md
+-rw-r--r--   0        0        0      838 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-examine-single-item.md
+-rw-r--r--   0        0        0     6778 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-examine-type.md
+-rw-r--r--   0        0        0      269 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-examine.md
+-rw-r--r--   0        0        0      844 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-filter-cut-mask.md
+-rw-r--r--   0        0        0     3889 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-filter-masked.md
+-rw-r--r--   0        0        0      840 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-filter-num.md
+-rw-r--r--   0        0        0     7955 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-filter-ragged.md
+-rw-r--r--   0        0        0      265 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-filter.md
+-rw-r--r--   0        0        0      818 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-math-argminmax.md
+-rw-r--r--   0        0        0      822 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-math-broadcasting.md
+-rw-r--r--   0        0        0      828 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-math-gpu.md
+-rw-r--r--   0        0        0      838 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-math-numpy.md
+-rw-r--r--   0        0        0      846 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-math-reducing.md
+-rw-r--r--   0        0        0      870 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-math-statistics.md
+-rw-r--r--   0        0        0      265 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-math.md
+-rw-r--r--   0        0        0     3411 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure-add-fields.md
+-rw-r--r--   0        0        0      842 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure-concatenate.md
+-rw-r--r--   0        0        0    19083 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure-flatten.md
+-rw-r--r--   0        0        0     7568 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure-pad.md
+-rw-r--r--   0        0        0      852 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure-rename-records.md
+-rw-r--r--   0        0        0      832 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure-sort.md
+-rw-r--r--   0        0        0     9624 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure-zip-project.md
+-rw-r--r--   0        0        0      273 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-restructure.md
+-rw-r--r--   0        0        0     2599 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-specialize-differentiate-jax.md
+-rw-r--r--   0        0        0      870 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-specialize-in-numba.md
+-rw-r--r--   0        0        0      838 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-specialize-lorentz.md
+-rw-r--r--   0        0        0      874 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-specialize-override-numpy.md
+-rw-r--r--   0        0        0      870 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-specialize-subclass.md
+-rw-r--r--   0        0        0      277 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-specialize.md
+-rw-r--r--   0        0        0    11724 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-use-header-only-layoutbuilder.md
+-rw-r--r--   0        0        0      900 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-use-in-numba-arraybuilder.md
+-rw-r--r--   0        0        0     9973 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-use-in-numba-cuda.ipynb
+-rw-r--r--   0        0        0      900 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-use-in-numba-features.md
+-rw-r--r--   0        0        0      279 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/how-to-use-in-numba.md
+-rw-r--r--   0        0        0      344 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/index.md
+-rw-r--r--   0        0        0        0 2023-04-08 19:13:43.000000 awkward-2.1.2/docs/user-guide/requirements.txt
+-rw-r--r--   0        0        0   367587 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-data-analysts.png
+-rw-r--r--   0        0        0   794465 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-data-analysts.svg
+-rw-r--r--   0        0        0   140700 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-developers.png
+-rw-r--r--   0        0        0   328307 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-developers.svg
+-rw-r--r--   0        0        0    73584 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-doxygen.png
+-rw-r--r--   0        0        0    58179 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-sphinx.png
+-rw-r--r--   0        0        0   127063 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-tutorials-alternate.png
+-rw-r--r--   0        0        0   173327 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/panel-tutorials.png
+-rw-r--r--   0        0        0    12541 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-1-0-layers.pdf
+-rw-r--r--   0        0        0    65246 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-1-0-layers.png
+-rw-r--r--   0        0        0    41004 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-1-0-layers.svg
+-rw-r--r--   0        0        0    14946 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-timeline.pdf
+-rw-r--r--   0        0        0   125180 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-timeline.png
+-rw-r--r--   0        0        0    70209 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-timeline.svg
+-rw-r--r--   0        0        0   436595 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
+-rw-r--r--   0        0        0   426911 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
+-rw-r--r--   0        0        0   335955 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip.png
+-rw-r--r--   0        0        0   325268 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip.svg
+-rw-r--r--   0        0        0   129696 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline.png
+-rw-r--r--   0        0        0   120554 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline.svg
+-rw-r--r--   0        0        0     5208 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-broadcasting.png
+-rw-r--r--   0        0        0    25065 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-broadcasting.svg
+-rw-r--r--   0        0        0     5754 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-cartesian.png
+-rw-r--r--   0        0        0    32616 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-cartesian.svg
+-rw-r--r--   0        0        0     9584 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-combinations.png
+-rw-r--r--   0        0        0    39524 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-combinations.svg
+-rw-r--r--   0        0        0    10808 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-schematic.png
+-rw-r--r--   0        0        0    25779 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/cartoon-schematic.svg
+-rw-r--r--   0        0        0    18178 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    36024 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/example-hierarchy.png
+-rw-r--r--   0        0        0    17092 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/example-hierarchy.svg
+-rw-r--r--   0        0        0    21120 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/example-reduction-sum-only.svg
+-rw-r--r--   0        0        0    29325 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    55553 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/example-reduction.png
+-rw-r--r--   0        0        0    21631 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/example-reduction.svg
+-rw-r--r--   0        0        0    10978 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/git-strategy.pdf
+-rw-r--r--   0        0        0    58904 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/git-strategy.png
+-rw-r--r--   0        0        0    28990 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/git-strategy.svg
+-rw-r--r--   0        0        0   113587 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/how-it-works-muons.png
+-rw-r--r--   0        0        0    57471 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/how-it-works-muons.svg
+-rw-r--r--   0        0        0    58475 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/how-it-works.svg
+-rw-r--r--   0        0        0    63989 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/sorting-axis.svg
+-rw-r--r--   0        0        0   124038 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/all.svg
+-rw-r--r--   0        0        0   128558 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/any.svg
+-rw-r--r--   0        0        0   134490 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/argmax.svg
+-rw-r--r--   0        0        0   133192 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/argmin.svg
+-rw-r--r--   0        0        0   106277 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/count.svg
+-rw-r--r--   0        0        0   116417 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/count_nonzero.svg
+-rw-r--r--   0        0        0   111789 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/max.svg
+-rw-r--r--   0        0        0   109239 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/min.svg
+-rw-r--r--   0        0        0   124702 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/product.svg
+-rw-r--r--   0        0        0   108897 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/diagrams/reducers/sum.svg
+-rw-r--r--   0        0        0     8347 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/logo/favicon.ico
+-rw-r--r--   0        0        0     8984 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/logo/logo-300px-white.png
+-rw-r--r--   0        0        0    11964 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    24707 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/logo/logo-600px.png
+-rw-r--r--   0        0        0    18767 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/logo/logo.svg
+-rw-r--r--   0        0        0    90413 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/photos/desire-path.jpg
+-rw-r--r--   0        0        0    52113 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/plots/awkward-0-popularity.pdf
+-rw-r--r--   0        0        0   146109 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/plots/awkward-0-popularity.png
+-rw-r--r--   0        0        0   147576 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/plots/awkward-0-popularity.svg
+-rw-r--r--   0        0        0    26938 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/plots/bikeroutes-scaling.svg
+-rw-r--r--   0        0        0     8891 2023-04-08 19:13:43.000000 awkward-2.1.2/docs-img/screenshots/github-issues-documentation.png
+-rw-r--r--   0        0        0     1301 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/__init__.py
+-rw-r--r--   0        0        0     7950 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_backends.py
+-rw-r--r--   0        0        0     5418 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_behavior.py
+-rw-r--r--   0        0        0    38002 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_broadcasting.py
+-rw-r--r--   0        0        0    13390 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_do.py
+-rw-r--r--   0        0        0    11875 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_errors.py
+-rw-r--r--   0        0        0     5130 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_kernels.py
+-rw-r--r--   0        0        0     5781 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_layout.py
+-rw-r--r--   0        0        0     9983 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_lookup.py
+-rw-r--r--   0        0        0     5454 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_parameters.py
+-rw-r--r--   0        0        0     9965 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_prettyprint.py
+-rw-r--r--   0        0        0    24569 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_reducers.py
+-rw-r--r--   0        0        0     2041 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_regularize.py
+-rw-r--r--   0        0        0      420 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_singleton.py
+-rw-r--r--   0        0        0    23977 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_slicing.py
+-rw-r--r--   0        0        0      647 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_typetracer.py
+-rw-r--r--   0        0        0     1163 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_typing.py
+-rw-r--r--   0        0        0     2439 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_util.py
+-rw-r--r--   0        0        0      758 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_v2.py
+-rw-r--r--   0        0        0      233 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/builder.py
+-rw-r--r--   0        0        0      866 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/cppyy.py
+-rw-r--r--   0        0        0      271 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forth.py
+-rw-r--r--   0        0        0   102580 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/highlevel.py
+-rw-r--r--   0        0        0     7899 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/index.py
+-rw-r--r--   0        0        0     3982 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/jax.py
+-rw-r--r--   0        0        0     2764 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/numba.py
+-rw-r--r--   0        0        0     7982 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/record.py
+-rw-r--r--   0        0        0      165 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/typetracer.py
+-rw-r--r--   0        0        0       88 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/__init__.py
+-rw-r--r--   0        0        0    32504 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/avro.py
+-rw-r--r--   0        0        0    53533 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cling.py
+-rw-r--r--   0        0        0      992 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/hist.py
+-rw-r--r--   0        0        0     4485 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numexpr.py
+-rw-r--r--   0        0        0    10031 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numpy.py
+-rw-r--r--   0        0        0    37991 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/pyarrow.py
+-rw-r--r--   0        0        0     7038 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/__init__.py
+-rw-r--r--   0        0        0     2555 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
+-rw-r--r--   0        0        0     4326 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
+-rw-r--r--   0        0        0      987 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu
+-rw-r--r--   0        0        0     2542 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3034 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0      630 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu
+-rw-r--r--   0        0        0      830 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3196 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0     2668 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0      749 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
+-rw-r--r--   0        0        0     2749 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
+-rw-r--r--   0        0        0      552 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu
+-rw-r--r--   0        0        0      637 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
+-rw-r--r--   0        0        0     2886 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
+-rw-r--r--   0        0        0     2904 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     3416 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0     3531 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu
+-rw-r--r--   0        0        0      556 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu
+-rw-r--r--   0        0        0      695 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     3036 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0      795 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
+-rw-r--r--   0        0        0     2523 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0     2729 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
+-rw-r--r--   0        0        0     1035 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
+-rw-r--r--   0        0        0      961 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
+-rw-r--r--   0        0        0     2593 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
+-rw-r--r--   0        0        0     1536 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
+-rw-r--r--   0        0        0     1710 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     2012 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1184 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
+-rw-r--r--   0        0        0      755 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu
+-rw-r--r--   0        0        0      806 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
+-rw-r--r--   0        0        0      744 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu
+-rw-r--r--   0        0        0     1169 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0     1059 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
+-rw-r--r--   0        0        0     3208 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
+-rw-r--r--   0        0        0      575 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu
+-rw-r--r--   0        0        0      830 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu
+-rw-r--r--   0        0        0      650 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu
+-rw-r--r--   0        0        0     2610 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu
+-rw-r--r--   0        0        0     1126 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu
+-rw-r--r--   0        0        0      951 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      721 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu
+-rw-r--r--   0        0        0     1003 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu
+-rw-r--r--   0        0        0     1339 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu
+-rw-r--r--   0        0        0      835 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
+-rw-r--r--   0        0        0      975 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
+-rw-r--r--   0        0        0      802 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
+-rw-r--r--   0        0        0     1123 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu
+-rw-r--r--   0        0        0      623 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu
+-rw-r--r--   0        0        0      789 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
+-rw-r--r--   0        0        0     1040 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     1020 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1045 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      974 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
+-rw-r--r--   0        0        0      946 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
+-rw-r--r--   0        0        0      980 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
+-rw-r--r--   0        0        0      663 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
+-rw-r--r--   0        0        0      586 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
+-rw-r--r--   0        0        0     2580 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
+-rw-r--r--   0        0        0     1360 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
+-rw-r--r--   0        0        0      461 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_carry_arange.cu
+-rw-r--r--   0        0        0      534 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu
+-rw-r--r--   0        0        0      529 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu
+-rw-r--r--   0        0        0      830 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu
+-rw-r--r--   0        0        0      636 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu
+-rw-r--r--   0        0        0      689 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0      457 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
+-rw-r--r--   0        0        0      830 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
+-rw-r--r--   0        0        0     2043 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
+-rw-r--r--   0        0        0     2198 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu
+-rw-r--r--   0        0        0     2043 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
+-rw-r--r--   0        0        0     2198 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu
+-rw-r--r--   0        0        0     3054 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
+-rw-r--r--   0        0        0     3289 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
+-rw-r--r--   0        0        0     2022 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
+-rw-r--r--   0        0        0     2022 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
+-rw-r--r--   0        0        0     3202 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
+-rw-r--r--   0        0        0     3012 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
+-rw-r--r--   0        0        0     3171 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
+-rw-r--r--   0        0        0     3439 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
+-rw-r--r--   0        0        0     3439 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
+-rw-r--r--   0        0        0      865 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu
+-rw-r--r--   0        0        0      443 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_zero_mask.cu
+-rw-r--r--   0        0        0     3195 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
+-rw-r--r--   0        0        0     1859 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/header-only/awkward/BuilderOptions.h
+-rw-r--r--   0        0        0    19867 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
+-rw-r--r--   0        0        0    89307 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
+-rw-r--r--   0        0        0      298 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/header-only/awkward/demo_impl.h
+-rw-r--r--   0        0        0     8025 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/header-only/awkward/utils.h
+-rw-r--r--   0        0        0      239 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/jax/__init__.py
+-rw-r--r--   0        0        0     6627 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/jax/reducers.py
+-rw-r--r--   0        0        0     5930 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/jax/trees.py
+-rw-r--r--   0        0        0       88 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numba/__init__.py
+-rw-r--r--   0        0        0    35824 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numba/arrayview.py
+-rw-r--r--   0        0        0     1148 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numba/arrayview_cuda.py
+-rw-r--r--   0        0        0    31514 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numba/builder.py
+-rw-r--r--   0        0        0    12431 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numba/growablebuffer.py
+-rw-r--r--   0        0        0    49132 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/numba/layout.py
+-rw-r--r--   0        0        0       88 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/rdataframe/__init__.py
+-rw-r--r--   0        0        0     9341 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/rdataframe/from_rdataframe.py
+-rw-r--r--   0        0        0     9922 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/rdataframe/to_rdataframe.py
+-rw-r--r--   0        0        0     1487 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
+-rw-r--r--   0        0        0     3526 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/__init__.py
+-rw-r--r--   0        0        0    12077 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/array_module.py
+-rw-r--r--   0        0        0     4754 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/cupy.py
+-rw-r--r--   0        0        0     2036 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/jax.py
+-rw-r--r--   0        0        0     2737 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/numpy.py
+-rw-r--r--   0        0        0    13660 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/numpylike.py
+-rw-r--r--   0        0        0     2330 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/shape.py
+-rw-r--r--   0        0        0    42156 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/typetracer.py
+-rw-r--r--   0        0        0     2527 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/_nplikes/ufuncs.py
+-rw-r--r--   0        0        0       88 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/behaviors/__init__.py
+-rw-r--r--   0        0        0     3479 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/behaviors/categorical.py
+-rw-r--r--   0        0        0     3898 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/behaviors/mixins.py
+-rw-r--r--   0        0        0     8509 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/behaviors/string.py
+-rw-r--r--   0        0        0      986 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/__init__.py
+-rw-r--r--   0        0        0    27770 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/bitmaskedarray.py
+-rw-r--r--   0        0        0    40807 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/bytemaskedarray.py
+-rw-r--r--   0        0        0    45218 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/content.py
+-rw-r--r--   0        0        0    13230 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/emptyarray.py
+-rw-r--r--   0        0        0    40314 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/indexedarray.py
+-rw-r--r--   0        0        0    63394 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/indexedoptionarray.py
+-rw-r--r--   0        0        0    59892 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/listarray.py
+-rw-r--r--   0        0        0    85099 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/listoffsetarray.py
+-rw-r--r--   0        0        0    49464 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/numpyarray.py
+-rw-r--r--   0        0        0    40376 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/recordarray.py
+-rw-r--r--   0        0        0    54508 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/regulararray.py
+-rw-r--r--   0        0        0    56977 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/unionarray.py
+-rw-r--r--   0        0        0    18810 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/contents/unmaskedarray.py
+-rw-r--r--   0        0        0      951 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/__init__.py
+-rw-r--r--   0        0        0     6081 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/bitmaskedform.py
+-rw-r--r--   0        0        0     5368 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/bytemaskedform.py
+-rw-r--r--   0        0        0     3369 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/emptyform.py
+-rw-r--r--   0        0        0    12414 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/form.py
+-rw-r--r--   0        0        0     5638 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/indexedform.py
+-rw-r--r--   0        0        0     5133 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/indexedoptionform.py
+-rw-r--r--   0        0        0     5621 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/listform.py
+-rw-r--r--   0        0        0     4715 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/listoffsetform.py
+-rw-r--r--   0        0        0     6004 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/numpyform.py
+-rw-r--r--   0        0        0     8208 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/recordform.py
+-rw-r--r--   0        0        0     5084 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/regularform.py
+-rw-r--r--   0        0        0     7760 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/unionform.py
+-rw-r--r--   0        0        0     4229 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/forms/unmaskedform.py
+-rw-r--r--   0        0        0     4779 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/__init__.py
+-rw-r--r--   0        0        0     3998 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_all.py
+-rw-r--r--   0        0        0     5132 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_almost_equal.py
+-rw-r--r--   0        0        0     4001 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_any.py
+-rw-r--r--   0        0        0     5049 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_argcartesian.py
+-rw-r--r--   0        0        0     3819 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_argcombinations.py
+-rw-r--r--   0        0        0     6888 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_argmax.py
+-rw-r--r--   0        0        0     6845 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_argmin.py
+-rw-r--r--   0        0        0     3158 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_argsort.py
+-rw-r--r--   0        0        0      915 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_backend.py
+-rw-r--r--   0        0        0     9442 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_broadcast_arrays.py
+-rw-r--r--   0        0        0     6522 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_broadcast_fields.py
+-rw-r--r--   0        0        0    16000 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_cartesian.py
+-rw-r--r--   0        0        0     1420 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_categories.py
+-rw-r--r--   0        0        0     8118 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_combinations.py
+-rw-r--r--   0        0        0    12195 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_concatenate.py
+-rw-r--r--   0        0        0     2715 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_copy.py
+-rw-r--r--   0        0        0     5817 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_corr.py
+-rw-r--r--   0        0        0     5228 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_count.py
+-rw-r--r--   0        0        0     4035 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_count_nonzero.py
+-rw-r--r--   0        0        0     5170 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_covar.py
+-rw-r--r--   0        0        0     4579 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_drop_none.py
+-rw-r--r--   0        0        0     1106 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_fields.py
+-rw-r--r--   0        0        0     5215 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_fill_none.py
+-rw-r--r--   0        0        0     3432 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_firsts.py
+-rw-r--r--   0        0        0     7802 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_flatten.py
+-rw-r--r--   0        0        0     3154 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_arrow.py
+-rw-r--r--   0        0        0      813 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_arrow_schema.py
+-rw-r--r--   0        0        0     2727 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_avro_file.py
+-rw-r--r--   0        0        0    14408 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_buffers.py
+-rw-r--r--   0        0        0     1839 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_categorical.py
+-rw-r--r--   0        0        0     1651 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_cupy.py
+-rw-r--r--   0        0        0     4111 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_iter.py
+-rw-r--r--   0        0        0     1716 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_jax.py
+-rw-r--r--   0        0        0    30067 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_json.py
+-rw-r--r--   0        0        0     2282 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_numpy.py
+-rw-r--r--   0        0        0    11860 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_parquet.py
+-rw-r--r--   0        0        0     3324 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_rdataframe.py
+-rw-r--r--   0        0        0     2965 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_from_regular.py
+-rw-r--r--   0        0        0     8859 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_full_like.py
+-rw-r--r--   0        0        0      873 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_is_categorical.py
+-rw-r--r--   0        0        0     2478 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_is_none.py
+-rw-r--r--   0        0        0      705 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_is_tuple.py
+-rw-r--r--   0        0        0      930 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_is_valid.py
+-rw-r--r--   0        0        0     2568 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_isclose.py
+-rw-r--r--   0        0        0     9122 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_linear_fit.py
+-rw-r--r--   0        0        0     3258 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_local_index.py
+-rw-r--r--   0        0        0     4757 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_mask.py
+-rw-r--r--   0        0        0     7430 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_max.py
+-rw-r--r--   0        0        0     9067 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_mean.py
+-rw-r--r--   0        0        0     3532 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_merge_option_of_records.py
+-rw-r--r--   0        0        0    12342 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_merge_union_of_records.py
+-rw-r--r--   0        0        0     3217 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_metadata_from_parquet.py
+-rw-r--r--   0        0        0     7382 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_min.py
+-rw-r--r--   0        0        0     4908 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_moment.py
+-rw-r--r--   0        0        0     2081 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_nan_to_none.py
+-rw-r--r--   0        0        0     5103 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_nan_to_num.py
+-rw-r--r--   0        0        0     3874 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_num.py
+-rw-r--r--   0        0        0     1951 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_ones_like.py
+-rw-r--r--   0        0        0     4362 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_pad_none.py
+-rw-r--r--   0        0        0     1786 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_parameters.py
+-rw-r--r--   0        0        0     6360 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_prod.py
+-rw-r--r--   0        0        0     4710 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_ptp.py
+-rw-r--r--   0        0        0     2275 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_ravel.py
+-rw-r--r--   0        0        0     9531 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_run_lengths.py
+-rw-r--r--   0        0        0     3028 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_singletons.py
+-rw-r--r--   0        0        0     3339 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_softmax.py
+-rw-r--r--   0        0        0     2670 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_sort.py
+-rw-r--r--   0        0        0     8124 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_std.py
+-rw-r--r--   0        0        0     3058 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_strings_astype.py
+-rw-r--r--   0        0        0    11718 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_sum.py
+-rw-r--r--   0        0        0     4931 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_arrow.py
+-rw-r--r--   0        0        0     6725 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_arrow_table.py
+-rw-r--r--   0        0        0     2325 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_backend.py
+-rw-r--r--   0        0        0     6333 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_buffers.py
+-rw-r--r--   0        0        0     6050 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_categorical.py
+-rw-r--r--   0        0        0     1073 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_cupy.py
+-rw-r--r--   0        0        0    13370 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_dataframe.py
+-rw-r--r--   0        0        0     1074 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_jax.py
+-rw-r--r--   0        0        0    11652 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_json.py
+-rw-r--r--   0        0        0     4461 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_layout.py
+-rw-r--r--   0        0        0     2612 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_list.py
+-rw-r--r--   0        0        0     2088 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_numpy.py
+-rw-r--r--   0        0        0     3354 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_packed.py
+-rw-r--r--   0        0        0    16968 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_parquet.py
+-rw-r--r--   0        0        0     2750 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_rdataframe.py
+-rw-r--r--   0        0        0     3347 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_to_regular.py
+-rw-r--r--   0        0        0    23906 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_transform.py
+-rw-r--r--   0        0        0     4304 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_type.py
+-rw-r--r--   0        0        0     9461 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_unflatten.py
+-rw-r--r--   0        0        0     2484 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_unzip.py
+-rw-r--r--   0        0        0     1138 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_validity_error.py
+-rw-r--r--   0        0        0     2659 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_values_astype.py
+-rw-r--r--   0        0        0     9352 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_var.py
+-rw-r--r--   0        0        0     5502 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_where.py
+-rw-r--r--   0        0        0     5065 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_with_field.py
+-rw-r--r--   0        0        0     2610 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_with_name.py
+-rw-r--r--   0        0        0     1848 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_with_parameter.py
+-rw-r--r--   0        0        0     3756 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_without_field.py
+-rw-r--r--   0        0        0     1509 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_without_parameters.py
+-rw-r--r--   0        0        0     2134 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_zeros_like.py
+-rw-r--r--   0        0        0     8819 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/operations/ak_zip.py
+-rw-r--r--   0        0        0      707 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/__init__.py
+-rw-r--r--   0        0        0   163323 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/_awkward_datashape_parser.py
+-rw-r--r--   0        0        0     1914 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/arraytype.py
+-rw-r--r--   0        0        0     2451 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/listtype.py
+-rw-r--r--   0        0        0     5652 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/numpytype.py
+-rw-r--r--   0        0        0     4180 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/optiontype.py
+-rw-r--r--   0        0        0     8067 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/recordtype.py
+-rw-r--r--   0        0        0     3133 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/regulartype.py
+-rw-r--r--   0        0        0     1105 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/scalartype.py
+-rw-r--r--   0        0        0     9622 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/type.py
+-rw-r--r--   0        0        0     3725 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/uniontype.py
+-rw-r--r--   0        0        0     1937 2023-04-08 19:13:43.000000 awkward-2.1.2/src/awkward/types/unknowntype.py
+-rw-r--r--   0        0        0       88 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     3358 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0002_minimal_listarray.py
+-rw-r--r--   0        0        0      487 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0006_deep_iteration.py
+-rw-r--r--   0        0        0     5565 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0008_slices_and_getitem.py
+-rw-r--r--   0        0        0    13378 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0011_listarray.py
+-rw-r--r--   0        0        0     4462 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0013_error_handling_struct.py
+-rw-r--r--   0        0        0    17019 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0014_finish_up_getitem.py
+-rw-r--r--   0        0        0     5169 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0018_fromiter_fillable.py
+-rw-r--r--   0        0        0     8833 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0019_use_json_library.py
+-rw-r--r--   0        0        0    13687 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0020_support_unsigned_indexes.py
+-rw-r--r--   0        0        0     6391 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0021_emptyarray.py
+-rw-r--r--   0        0        0    10743 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0023_regular_array.py
+-rw-r--r--   0        0        0     4890 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0024_use_regular_array.py
+-rw-r--r--   0        0        0    25581 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0025_record_array.py
+-rw-r--r--   0        0        0     3436 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0028_add_dressed_types.py
+-rw-r--r--   0        0        0     6361 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0032_replace_dressedtype.py
+-rw-r--r--   0        0        0    12027 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0046_start_indexedarray.py
+-rw-r--r--   0        0        0      898 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
+-rw-r--r--   0        0        0    12231 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0057_introducing_forms.py
+-rw-r--r--   0        0        0     5430 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0070_argmin_and_argmax.py
+-rw-r--r--   0        0        0     5384 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0072_fillna_operation.py
+-rw-r--r--   0        0        0    15655 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0074_argsort_and_sort.py
+-rw-r--r--   0        0        0     2836 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0077_zip_operation.py
+-rw-r--r--   0        0        0    11934 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0078_argcross_and_cross.py
+-rw-r--r--   0        0        0    12124 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0079_argchoose_and_choose.py
+-rw-r--r--   0        0        0     7071 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
+-rw-r--r--   0        0        0     6579 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0084_start_unionarray.py
+-rw-r--r--   0        0        0     6551 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0086_nep13_ufunc.py
+-rw-r--r--   0        0        0    12540 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0089_numpy_functions.py
+-rw-r--r--   0        0        0    46684 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0093_simplify_uniontypes_and_optiontypes.py
+-rw-r--r--   0        0        0     6959 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0107_assign_fields_to_records.py
+-rw-r--r--   0        0        0    46658 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0111_jagged_and_masked_getitem.py
+-rw-r--r--   0        0        0    77224 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0115_generic_reducer_operation.py
+-rw-r--r--   0        0        0    35084 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0118_numba_cpointers.py
+-rw-r--r--   0        0        0     1091 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0119_numexpr_and_broadcast_arrays.py
+-rw-r--r--   0        0        0     1106 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0124_strings_in_numba.py
+-rw-r--r--   0        0        0    32114 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0127_tomask_operation.py
+-rw-r--r--   0        0        0     3683 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0127b_tomask_operation_numba.py
+-rw-r--r--   0        0        0      838 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0138_emptyarray_type.py
+-rw-r--r--   0        0        0    17923 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0150_flatten.py
+-rw-r--r--   0        0        0     3602 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0163_negative_axis_wrap.py
+-rw-r--r--   0        0        0     9779 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0166_0167_0170_random_issues.py
+-rw-r--r--   0        0        0     4552 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0173_astype_operation.py
+-rw-r--r--   0        0        0    24034 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0184_concatenate_operation.py
+-rw-r--r--   0        0        0     2063 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0193_is_none_axis_parameter.py
+-rw-r--r--   0        0        0     3352 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0198_tutorial_documentation_1.py
+-rw-r--r--   0        0        0     8998 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0222_count_with_axis0.py
+-rw-r--r--   0        0        0    75605 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0224_arrow_to_awkward.py
+-rw-r--r--   0        0        0      581 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0264_reduce_last_empty.py
+-rw-r--r--   0        0        0     3251 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0273_path_for_with_field.py
+-rw-r--r--   0        0        0      743 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0286_broadcast_single_value_with_field.py
+-rw-r--r--   0        0        0     2205 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0290_bug_fixes_for_hats.py
+-rw-r--r--   0        0        0     4806 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0315_integerindex.py
+-rw-r--r--   0        0        0     5745 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0331_pandas_indexedarray.py
+-rw-r--r--   0        0        0     1257 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0334_fully_broadcastable_where.py
+-rw-r--r--   0        0        0      566 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0339_highlevel_sorting_function.py
+-rw-r--r--   0        0        0     6757 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0348_form_keys.py
+-rw-r--r--   0        0        0     4523 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0355_mixins.py
+-rw-r--r--   0        0        0    10396 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0395_complex_type_arrays.py
+-rw-r--r--   0        0        0     4934 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0395_fix_numba_indexedarray.py
+-rw-r--r--   0        0        0     3077 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0397_arrays_as_constants_in_numba.py
+-rw-r--r--   0        0        0    14529 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
+-rw-r--r--   0        0        0    22467 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0404_array_validity_check.py
+-rw-r--r--   0        0        0    14282 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0410_fix_argminmax_positions_for_missing_values.py
+-rw-r--r--   0        0        0    17455 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0437_stream_of_many_json_files.py
+-rw-r--r--   0        0        0    32921 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0447_preserve_regularness_in_reduce.py
+-rw-r--r--   0        0        0    24075 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0449_merge_many_arrays_in_one_pass.py
+-rw-r--r--   0        0        0     4059 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0493_zeros_ones_full_like.py
+-rw-r--r--   0        0        0     1606 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0496_provide_local_index.py
+-rw-r--r--   0        0        0     2059 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0499_getitem_indexedarray_bug.py
+-rw-r--r--   0        0        0     1286 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0504_block_ufuncs_for_strings.py
+-rw-r--r--   0        0        0     2926 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0511_copy_and_deepcopy.py
+-rw-r--r--   0        0        0     9119 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
+-rw-r--r--   0        0        0      365 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0546_fill_none_replacement_value_type.py
+-rw-r--r--   0        0        0     1102 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0549_numba_array_asarray.py
+-rw-r--r--   0        0        0     4268 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0557_min_max_initial_argument.py
+-rw-r--r--   0        0        0      537 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0559_fix_booleans_in_numba.py
+-rw-r--r--   0        0        0      636 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0572_numba_array_ndim.py
+-rw-r--r--   0        0        0     4901 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0582_propagate_context_in_broadcast_and_apply.py
+-rw-r--r--   0        0        0     1099 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0583_implement_unflatten_function.py
+-rw-r--r--   0        0        0     3084 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0590_allow_regulararray_size_zero.py
+-rw-r--r--   0        0        0     5957 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
+-rw-r--r--   0        0        0      478 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0627_behavior_from_dict_of_arrays.py
+-rw-r--r--   0        0        0     8205 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0652_tests_of_complex_numbers.py
+-rw-r--r--   0        0        0     2338 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0674_categorical_validation.py
+-rw-r--r--   0        0        0      750 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0713_getitem_field_should_simplify_optiontype.py
+-rw-r--r--   0        0        0     1242 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
+-rw-r--r--   0        0        0     1055 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0730_unflatten_axis_parameter.py
+-rw-r--r--   0        0        0     2569 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0733_run_lengths.py
+-rw-r--r--   0        0        0     2127 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0736_implement_argsort_for_strings.py
+-rw-r--r--   0        0        0      330 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0758_ak_zip_scallars.py
+-rw-r--r--   0        0        0     1122 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0766_prevent_combinations_of_characters.py
+-rw-r--r--   0        0        0    26349 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0773_typeparser.py
+-rw-r--r--   0        0        0      779 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
+-rw-r--r--   0        0        0      871 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0794_ak_cartesian_on_empty_array.py
+-rw-r--r--   0        0        0     1148 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0803_argsort_fix_type.py
+-rw-r--r--   0        0        0     1364 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0806_empty_lists_cartesian_fix.py
+-rw-r--r--   0        0        0     6311 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0813_full_like_dtype_arg.py
+-rw-r--r--   0        0        0     1661 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0815_broadcast_union_types_to_all_possibilities.py
+-rw-r--r--   0        0        0      488 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0819_issue.py
+-rw-r--r--   0        0        0      682 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0828_arrow_datatype_null.py
+-rw-r--r--   0        0        0    23609 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0835_datetime_type.py
+-rw-r--r--   0        0        0      676 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0835_datetime_type_pandas.py
+-rw-r--r--   0        0        0     4662 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0835_datetime_type_pyarrow.py
+-rw-r--r--   0        0        0      680 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0850_argsort_mask_array.py
+-rw-r--r--   0        0        0      449 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0863_is_none_numpy_array.py
+-rw-r--r--   0        0        0     1029 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0866_getitem_field_and_flatten_unions.py
+-rw-r--r--   0        0        0      929 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0875_arrow_null_type.py
+-rw-r--r--   0        0        0      901 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0879_non_primitive_with_field.py
+-rw-r--r--   0        0        0      563 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0884_index_and_identifier_refactoring.py
+-rw-r--r--   0        0        0     1086 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0889_ptp.py
+-rw-r--r--   0        0        0    53355 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0896_content_classes_refactoring.py
+-rw-r--r--   0        0        0     1751 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0898_unzip_heterogeneous_records.py
+-rw-r--r--   0        0        0      421 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
+-rw-r--r--   0        0        0      530 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0905_leading_zeros_in_unflatten.py
+-rw-r--r--   0        0        0     1048 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0906_arrow_fixed_size_list_type.py
+-rw-r--r--   0        0        0      666 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0910_unflatten_counts_relation.py
+-rw-r--r--   0        0        0     5261 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0912_packed.py
+-rw-r--r--   0        0        0   115760 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0914_types_and_forms.py
+-rw-r--r--   0        0        0     1877 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0916_datetime_values_astype.py
+-rw-r--r--   0        0        0     5522 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0927_numpy_array_nbytes.py
+-rw-r--r--   0        0        0      709 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0930_bug_in_unionarray_purelist_parameter.py
+-rw-r--r--   0        0        0     1627 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0945_argsort_sort_nan_array.py
+-rw-r--r--   0        0        0    28028 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0958_new_forms_must_accept_old_form_json.py
+-rw-r--r--   0        0        0    28284 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0959__getitem_array_implementation.py
+-rw-r--r--   0        0        0      651 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0975_mask_multidimensional_numpy_array.py
+-rw-r--r--   0        0        0      644 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0979_where_multidimentional_numpy_array.py
+-rw-r--r--   0        0        0     5803 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0982_missing_case_in_nonlocal_reducers.py
+-rw-r--r--   0        0        0     1976 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0984_ravel.py
+-rw-r--r--   0        0        0     1806 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_0992_correct_ptp_unmasking.py
+-rw-r--r--   0        0        0     2100 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
+-rw-r--r--   0        0        0      429 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1006_packed_regular_array_zero_size.py
+-rw-r--r--   0        0        0      416 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1007_from_buffers_empty_ndarray.py
+-rw-r--r--   0        0        0      551 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1017_numpyarray_broadcast.py
+-rw-r--r--   0        0        0      785 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1030_mixin_class_name.py
+-rw-r--r--   0        0        0    52114 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1031_start_getitem_next.py
+-rw-r--r--   0        0        0    18007 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1031b_start_getitem_next_specialized.py
+-rw-r--r--   0        0        0     1146 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1049_concatenate_single_array.py
+-rw-r--r--   0        0        0     1559 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1055_fill_none_numpy_dimension.py
+-rw-r--r--   0        0        0    42250 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1059_localindex.py
+-rw-r--r--   0        0        0      551 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1066_to_numpy_masked_structured_array.py
+-rw-r--r--   0        0        0      685 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1071_mask_identity_false_should_not_return_option_type.py
+-rw-r--r--   0        0        0    27714 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1072_sort.py
+-rw-r--r--   0        0        0    44140 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1074_combinations.py
+-rw-r--r--   0        0        0     5181 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1075_validityerror.py
+-rw-r--r--   0        0        0      273 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1106_argminmax_axis_None_missing_values.py
+-rw-r--r--   0        0        0    25531 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1110_type_tracer_1.py
+-rw-r--r--   0        0        0     1870 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1116_project_maskedarrays.py
+-rw-r--r--   0        0        0    28234 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1125_to_arrow_from_arrow.py
+-rw-r--r--   0        0        0     6276 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1132_utility_methods_for_highlevel_functions.py
+-rw-r--r--   0        0        0    21098 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1134_from_buffers_to_buffers.py
+-rw-r--r--   0        0        0    57322 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1135_rpad_operation.py
+-rw-r--r--   0        0        0     4639 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1136_regulararray_zeros_in_shape.py
+-rw-r--r--   0        0        0    10487 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1137_num.py
+-rw-r--r--   0        0        0    10222 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1142_numbers_to_type.py
+-rw-r--r--   0        0        0     2559 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1149_datetime_sort.py
+-rw-r--r--   0        0        0      630 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1154_arrow_tables_should_preserve_parameters.py
+-rw-r--r--   0        0        0    27983 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1162_ak_from_json_schema.py
+-rw-r--r--   0        0        0      766 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1183_bugs_found_by_dask_project_2.py
+-rw-r--r--   0        0        0     1286 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1189_fix_singletons_for_non_optional_data.py
+-rw-r--r--   0        0        0      551 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1192_iterables_in___array_function__.py
+-rw-r--r--   0        0        0      608 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1193_is_none_nested_option.py
+-rw-r--r--   0        0        0     2601 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1233_ak_with_name.py
+-rw-r--r--   0        0        0    26467 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1240_v2_implementation_of_numba_1.py
+-rw-r--r--   0        0        0     1146 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1259_simplify_optiontype.py
+-rw-r--r--   0        0        0     1560 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1260_simplify_masked_option_types.py
+-rw-r--r--   0        0        0      681 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1271_fix_4D_reducers.py
+-rw-r--r--   0        0        0    33003 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1294_to_and_from_parquet.py
+-rw-r--r--   0        0        0     1945 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
+-rw-r--r--   0        0        0    62340 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1300_awkward_to_cpp_converter_with_cling.py
+-rw-r--r--   0        0        0    39474 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1300b_same_for_numba.py
+-rw-r--r--   0        0        0      367 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1305_mixed_awkward_numpy_slicing.py
+-rw-r--r--   0        0        0     1702 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1308_zip_after_option.py
+-rw-r--r--   0        0        0     1703 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1318_array_function_types.py
+-rw-r--r--   0        0        0     1730 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1320_mask_identity_defaults.py
+-rw-r--r--   0        0        0      647 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1344_broadcast_arrays_depth_limit.py
+-rw-r--r--   0        0        0     6621 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1345_avro_reader.py
+-rw-r--r--   0        0        0     4562 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1351_is_tuple.py
+-rw-r--r--   0        0        0     8362 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1374_to_rdataframe.py
+-rw-r--r--   0        0        0     1755 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1377_ravel_string.py
+-rw-r--r--   0        0        0     1468 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1379_reducers_with_axis_None_and_typetracers.py
+-rw-r--r--   0        0        0     1384 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1399_from_jax.py
+-rw-r--r--   0        0        0     1227 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1399_to_jax.py
+-rw-r--r--   0        0        0      297 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1400_with_name_record.py
+-rw-r--r--   0        0        0      449 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1403_from_numpy_strings.py
+-rw-r--r--   0        0        0     3470 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1405_slicing_untested_cases.py
+-rw-r--r--   0        0        0     6909 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1415_behaviour_forwarding.py
+-rw-r--r--   0        0        0    18809 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1440_start_v2_to_parquet.py
+-rw-r--r--   0        0        0    14402 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1447_jax_autodiff_slices_ufuncs.py
+-rw-r--r--   0        0        0     8591 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1449_v2_to_json_from_json_functions.py
+-rw-r--r--   0        0        0      692 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1453_write_single_records_to_parquet.py
+-rw-r--r--   0        0        0     9828 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1473_from_rdataframe.py
+-rw-r--r--   0        0        0    24648 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1477_generator_entry_type_as_rvec.py
+-rw-r--r--   0        0        0     3579 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1490_jax_reducers_combinations.py
+-rw-r--r--   0        0        0     3905 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1502_getitem_jagged_issue1406.py
+-rw-r--r--   0        0        0     1733 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1504_typetracer_like.py
+-rw-r--r--   0        0        0     4913 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1508_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     2186 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1511_set_attribute.py
+-rw-r--r--   0        0        0      754 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1539_isnone_axis_check_issue1417.py
+-rw-r--r--   0        0        0     1570 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1559_fix_ufuncs_records_1439.py
+-rw-r--r--   0        0        0      990 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1565_axis_wrap_if_negative_record.py
+-rw-r--r--   0        0        0     1080 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1567_fix_longlong_in_Index.py
+-rw-r--r--   0        0        0     3022 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1568_fix_lengths_empty_regular_slices.py
+-rw-r--r--   0        0        0      385 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1578_to_arrow_empty_recordarray.py
+-rw-r--r--   0        0        0     5911 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1586_concatenate_should_preserve_regulararray.py
+-rw-r--r--   0        0        0      216 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1593_empty_slice_list_record.py
+-rw-r--r--   0        0        0     7260 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1604_preserve_form_in_concatenate.py
+-rw-r--r--   0        0        0     3636 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1607_no_reducers_on_records.py
+-rw-r--r--   0        0        0    10035 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1613_generator_tolayout_records.py
+-rw-r--r--   0        0        0      727 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1619_from_parquet_empty_field.py
+-rw-r--r--   0        0        0     6024 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1620_layout_builders.py
+-rw-r--r--   0        0        0     8122 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1625_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0      770 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1642_from_iter_of_tuples.py
+-rw-r--r--   0        0        0      389 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1644_concatenate_zeros_length.py
+-rw-r--r--   0        0        0     4317 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1650_Record_to_list_should_listify_itself.py
+-rw-r--r--   0        0        0      560 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1671_categorical_type.py
+-rw-r--r--   0        0        0    11761 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1672_broadcast_parameters.py
+-rw-r--r--   0        0        0     4453 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1677_array_builder_in_numba.py
+-rw-r--r--   0        0        0      544 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1685_IndexedArray_project_parameters.py
+-rw-r--r--   0        0        0      778 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1686_UnionArray_simplified_preserve_parameters.py
+-rw-r--r--   0        0        0      936 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1688_pack_categorical.py
+-rw-r--r--   0        0        0      525 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1703_fill_none_typetracer.py
+-rw-r--r--   0        0        0     1743 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1707_broadcast_parameters_ufunc.py
+-rw-r--r--   0        0        0      512 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1709_ak_array_constructor_behavior.py
+-rw-r--r--   0        0        0      398 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1735_from_numpy_mask.py
+-rw-r--r--   0        0        0      577 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1747_bytemaskedarray_mergemany.py
+-rw-r--r--   0        0        0      824 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1753_indexedarray_merge_kernel.py
+-rw-r--r--   0        0        0     1480 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1762_jax_behavior_support.py
+-rw-r--r--   0        0        0      589 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1764_jax_jacobian.py
+-rw-r--r--   0        0        0      962 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1765_add_ioanas_test_of_to_arraylib.py
+-rw-r--r--   0        0        0     4790 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1766_record_form_fields.py
+-rw-r--r--   0        0        0     2905 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1781_rdataframe_snapshot.py
+-rw-r--r--   0        0        0      701 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1784_reduce_leading_sublist.py
+-rw-r--r--   0        0        0      567 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1790_reduce_regulararray.py
+-rw-r--r--   0        0        0     4191 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1791_reduce_trailing_sublist.py
+-rw-r--r--   0        0        0     1027 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1794_run_lengths_empty_sublist.py
+-rw-r--r--   0        0        0      407 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1823_fill_none_axis_none.py
+-rw-r--r--   0        0        0      481 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1826_ravel_preserve_none.py
+-rw-r--r--   0        0        0     1451 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1829_to_from_rdataframe_bool.py
+-rw-r--r--   0        0        0      588 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
+-rw-r--r--   0        0        0     1097 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1847_numpy_array_contiguous.py
+-rw-r--r--   0        0        0      681 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
+-rw-r--r--   0        0        0     1640 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1867_pass_behavior_through_combinations.py
+-rw-r--r--   0        0        0    17239 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1904_drop_none.py
+-rw-r--r--   0        0        0     3553 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1914_improved_axis_to_posaxis.py
+-rw-r--r--   0        0        0     3444 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
+-rw-r--r--   0        0        0      921 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1930_unflatten_counts_checks.py
+-rw-r--r--   0        0        0      769 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1936_with_field_broadcasting.py
+-rw-r--r--   0        0        0      551 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1940_ak_backend.py
+-rw-r--r--   0        0        0     1457 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1943_regular_indexing.py
+-rw-r--r--   0        0        0      188 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1944_to_numpy_empty_record_array.py
+-rw-r--r--   0        0        0     1131 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1960_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     3286 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1961_ak_without_field.py
+-rw-r--r--   0        0        0      280 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1978_akRecord_constructor_should_retain_type.py
+-rw-r--r--   0        0        0      349 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
+-rw-r--r--   0        0        0      371 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2008_ak_type_layout.py
+-rw-r--r--   0        0        0    10222 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2020_reduce_axis_none.py
+-rw-r--r--   0        0        0      803 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2021_check_TypeTracerArray_in_ak_where.py
+-rw-r--r--   0        0        0      645 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2023_from_rdataframe.py
+-rw-r--r--   0        0        0     2854 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
+-rw-r--r--   0        0        0     1219 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2047_ak_transform_regular_to_jagged.py
+-rw-r--r--   0        0        0      406 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2051_arraybuilder_behavior_propagation.py
+-rw-r--r--   0        0        0     1275 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2055_array_builder_check.py
+-rw-r--r--   0        0        0     1659 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2058_merge_numpy_array.py
+-rw-r--r--   0        0        0      708 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2064_fill_none_record.py
+-rw-r--r--   0        0        0      799 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2067_to_buffers_byteorder.py
+-rw-r--r--   0        0        0      741 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2070_to_layout_string.py
+-rw-r--r--   0        0        0     1172 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2071_unflatten_non_packed_counts.py
+-rw-r--r--   0        0        0      291 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2076_ak_unzip_record.py
+-rw-r--r--   0        0        0      545 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2078_array_function_wrap.py
+-rw-r--r--   0        0        0      589 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2082_broadcast_zero_size.py
+-rw-r--r--   0        0        0     2765 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2096_ak_scalar_type.py
+-rw-r--r--   0        0        0      977 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2101_pickle_behavior_class.py
+-rw-r--r--   0        0        0      519 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2104_numpy_merge_option.py
+-rw-r--r--   0        0        0     2715 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2106_pickle_class.py
+-rw-r--r--   0        0        0      722 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2108_fill_none_indexed.py
+-rw-r--r--   0        0        0     2100 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2115_fix_up_typetracers.py
+-rw-r--r--   0        0        0      487 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2120_missing_field_error.py
+-rw-r--r--   0        0        0     1110 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2125_type_of_scalar.py
+-rw-r--r--   0        0        0     1893 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2150_typetracer_high_level_ufunc.py
+-rw-r--r--   0        0        0     1898 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2179_parameter_merging_rules.py
+-rw-r--r--   0        0        0      510 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2181_with_name_len.py
+-rw-r--r--   0        0        0     2957 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2185_merge_union_of_records.py
+-rw-r--r--   0        0        0      528 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
+-rw-r--r--   0        0        0     5548 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2198_almost_equal.py
+-rw-r--r--   0        0        0     1252 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2202_filter_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0     1453 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2214_offset_bool_index.py
+-rw-r--r--   0        0        0      334 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2219_flatten_empty.py
+-rw-r--r--   0        0        0      663 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2226_slice_regulararray_typetracer.py
+-rw-r--r--   0        0        0     1728 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2229_getitem_range_slice.py
+-rw-r--r--   0        0        0     4003 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2234_from_rdataframe_keep_order.py
+-rw-r--r--   0        0        0     3962 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2236_merge_union_of_records_option.py
+-rw-r--r--   0        0        0      485 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2240_merge_union_parameters.py
+-rw-r--r--   0        0        0     1338 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2240_simplify_merge_as_union.py
+-rw-r--r--   0        0        0      512 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2246_slice_not_packed.py
+-rw-r--r--   0        0        0      733 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2250_full_like_bool.py
+-rw-r--r--   0        0        0     1835 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2258_from_rdataframe_with_arguments.py
+-rw-r--r--   0        0        0      492 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2259_run_lengths_typetracer.py
+-rw-r--r--   0        0        0      549 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2263_to_packed_list.py
+-rw-r--r--   0        0        0      877 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2266_fix_nan_to_num.py
+-rw-r--r--   0        0        0      909 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2267_broadcast_fields.py
+-rw-r--r--   0        0        0     1336 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2293_unflatten_typetracer.py
+-rw-r--r--   0        0        0      406 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2294_view_unknown_scalar.py
+-rw-r--r--   0        0        0     2301 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2297_common_backend.py
+-rw-r--r--   0        0        0      455 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2304_index_typetracer.py
+-rw-r--r--   0        0        0     2929 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2306_cppyy_git.py
+-rw-r--r--   0        0        0     4386 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2319_from_buffers_array.py
+-rw-r--r--   0        0        0      865 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2327_array_interface.py
+-rw-r--r--   0        0        0     1728 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2329_cartesian_broadcasting_fixes.py
+-rw-r--r--   0        0        0      489 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2346_broadcast_depth_limit.py
+-rw-r--r--   0        0        0    15576 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2349_growablebuffer_in_numba.py
+-rw-r--r--   0        0        0      618 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2354_ufunc_same_backend.py
+-rw-r--r--   0        0        0      601 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2355_to_backend_record.py
+-rw-r--r--   0        0        0     1435 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2361_typetracer_asarray_nd.py
+-rw-r--r--   0        0        0     2921 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2368_type_is_equal.py
+-rw-r--r--   0        0        0     5259 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2373_unzip_touching.py
+-rw-r--r--   0        0        0     5857 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/test_2374_cartesian_touching.py
+-rw-r--r--   0        0        0      128 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/__init__.py
+-rw-r--r--   0        0        0      218 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/array_enum_test_data.avro
+-rw-r--r--   0        0        0      176 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/array_string_test_data.avro
+-rw-r--r--   0        0        0      152 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/array_test_data.avro
+-rw-r--r--   0        0        0      115 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/bool_test_data.avro
+-rw-r--r--   0        0        0      130 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/bytes_test_data.avro
+-rw-r--r--   0        0        0      158 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/double_test_data.avro
+-rw-r--r--   0        0        0      191 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/enum_null_test_data.avro
+-rw-r--r--   0        0        0      180 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/enum_test_data.avro
+-rw-r--r--   0        0        0      218 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/fixed_test_data.avro
+-rw-r--r--   0        0        0      116 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/float_test_data.avro
+-rw-r--r--   0        0        0      106 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/int_null_test_data.avro
+-rw-r--r--   0        0        0      128 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/int_string_null_test_data.avro
+-rw-r--r--   0        0        0       89 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/int_test_data.avro
+-rw-r--r--   0        0        0     3035 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2871 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/list-depths-records.parquet
+-rw-r--r--   0        0        0      497 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/list-depths-simple.parquet
+-rw-r--r--   0        0        0     1136 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/list-depths-strings.parquet
+-rw-r--r--   0        0        0     1060 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/list-depths.parquet
+-rw-r--r--   0        0        0      465 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/list-lengths.parquet
+-rw-r--r--   0        0        0      116 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/long_test_data.avro
+-rw-r--r--   0        0        0      681 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nonnullable-depths.parquet
+-rw-r--r--   0        0        0       75 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/null_test_data.avro
+-rw-r--r--   0        0        0      719 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-depths.parquet
+-rw-r--r--   0        0        0      635 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-levels.parquet
+-rw-r--r--   0        0        0     3050 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2926 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-list-depths-records.parquet
+-rw-r--r--   0        0        0     1179 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-list-depths-strings.parquet
+-rw-r--r--   0        0        0     1101 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-list-depths.parquet
+-rw-r--r--   0        0        0      430 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-record-primitives-simple.parquet
+-rw-r--r--   0        0        0     1181 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/nullable-record-primitives.parquet
+-rw-r--r--   0        0        0     1193 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/record-primitives.parquet
+-rw-r--r--   0        0        0      326 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/record_0_test_data.avro
+-rw-r--r--   0        0        0      368 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/record_1_test_data.avro
+-rw-r--r--   0        0        0      263 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/record_null_test_data.avro
+-rw-r--r--   0        0        0      423 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/record_test_data.avro
+-rw-r--r--   0        0        0      116 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/string_null_test_data.avro
+-rw-r--r--   0        0        0      125 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/string_test_data.avro
+-rw-r--r--   0        0        0      544 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/test-nan-inf.json
+-rw-r--r--   0        0        0      155 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/test-record-array.json
+-rw-r--r--   0        0        0      803 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/test-two-arrays.json
+-rw-r--r--   0        0        0      535 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/test.json
+-rw-r--r--   0        0        0      180 2023-04-08 19:13:43.000000 awkward-2.1.2/tests/samples/zero-record-batches.parquet
+-rw-r--r--   0        0        0       88 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/__init__.py
+-rw-r--r--   0        0        0     7072 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/test_1276_cuda_num.py
+-rw-r--r--   0        0        0     9911 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/test_1276_cuda_transfers.py
+-rw-r--r--   0        0        0     1197 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/test_1276_cupy_interop.py
+-rw-r--r--   0        0        0     1782 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/test_1276_from_cupy.py
+-rw-r--r--   0        0        0    42786 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/test_1300_same_for_numba_cuda.py
+-rw-r--r--   0        0        0      834 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/test_1381_check_errors.py
+-rw-r--r--   0        0        0    11252 2023-04-08 19:13:43.000000 awkward-2.1.2/tests-cuda/test_1809_array_cuda_jit.py
+-rw-r--r--   0        0        0     2212 2023-04-08 19:13:43.000000 awkward-2.1.2/.gitignore
+-rw-r--r--   0        0        0     1520 2023-04-08 19:13:43.000000 awkward-2.1.2/LICENSE
+-rw-r--r--   0        0        0     8479 2023-04-08 19:13:43.000000 awkward-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6933 2023-04-08 19:13:43.000000 awkward-2.1.2/PKG-INFO
```

### Comparing `awkward-2.1.1/CITATION.cff` & `awkward-2.1.2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/CONTRIBUTING.md` & `awkward-2.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/README.md` & `awkward-2.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 Arrays are **dynamically typed**, but operations on them are **compiled and fast**. Their behavior coincides with NumPy when array dimensions are regular and generalizes when they're not.
 
 # Motivating example
 
 Given an array of lists of objects with `x`, `y` fields (with nested lists in the `y` field),
 
 ```python
+import awkward as ak
+
 array = ak.Array([
     [{"x": 1.1, "y": [1]}, {"x": 2.2, "y": [1, 2]}, {"x": 3.3, "y": [1, 2, 3]}],
     [],
     [{"x": 4.4, "y": [1, 2, 3, 4]}, {"x": 5.5, "y": [1, 2, 3, 4, 5]}]
 ])
 ```
 
@@ -205,14 +207,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/ManasviGoyal"><img src="https://avatars.githubusercontent.com/u/55101825?v=4?s=100" width="100px;" alt="Manasvi Goyal"/><br /><sub><b>Manasvi Goyal</b></sub></a><br /><a href="https://github.com/scikit-hep/awkward/commits?author=ManasviGoyal" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/aryan26roy"><img src="https://avatars.githubusercontent.com/u/50577809?v=4?s=100" width="100px;" alt="Aryan Roy"/><br /><sub><b>Aryan Roy</b></sub></a><br /><a href="https://github.com/scikit-hep/awkward/commits?author=aryan26roy" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://saransh-cpp.github.io/"><img src="https://avatars.githubusercontent.com/u/74055102?v=4?s=100" width="100px;" alt="Saransh"/><br /><sub><b>Saransh</b></sub></a><br /><a href="https://github.com/scikit-hep/awkward/commits?author=Saransh-cpp" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/Laurits7"><img src="https://avatars.githubusercontent.com/u/30724920?v=4?s=100" width="100px;" alt="Laurits Tani"/><br /><sub><b>Laurits Tani</b></sub></a><br /><a href="https://github.com/scikit-hep/awkward/commits?author=Laurits7" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/dsavoiu"><img src="https://avatars.githubusercontent.com/u/17005255?v=4?s=100" width="100px;" alt="Daniel Savoiu"/><br /><sub><b>Daniel Savoiu</b></sub></a><br /><a href="https://github.com/scikit-hep/awkward/commits?author=dsavoiu" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://sites.google.com/view/raybellwaves/home"><img src="https://avatars.githubusercontent.com/u/17162724?v=4?s=100" width="100px;" alt="Ray Bell"/><br /><sub><b>Ray Bell</b></sub></a><br /><a href="https://github.com/scikit-hep/awkward/commits?author=raybellwaves" title="Documentation">📖</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `awkward-2.1.1/docs/_toc.yml` & `awkward-2.1.2/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/conf.py` & `awkward-2.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/index.md` & `awkward-2.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/prepare_docstrings.py` & `awkward-2.1.2/docs/prepare_docstrings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/redirects-user-guide.json` & `awkward-2.1.2/docs/redirects-user-guide.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/redirects.json` & `awkward-2.1.2/docs/redirects.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/_static/css/awkward.css` & `awkward-2.1.2/docs/_static/css/awkward.css`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/getting-started/community-tutorials.md` & `awkward-2.1.2/docs/getting-started/community-tutorials.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 - Ravel (flatten) ragged arrays with {func}`ak.ravel`.
 
 ## Loopy and unloopy programming techniques (SciPy 2022)
 A tutorial presented at the SciPy conference on July 11, 2022.
 
 ### Format
 - [{fab}`github` GitHub repository](https://github.com/jpivarski-talks/2022-07-11-scipy-loopy-tutorial)
- with Jupyter Notebooks that can be run on [MyBinder](https://mybinder.org/).
+ with Jupyter Notebooks that can be run on [MyBinder](https://mybinder.org/v2/gh/jpivarski-talks/2022-07-11-scipy-loopy-tutorial/v1.0?urlpath=lab/tree/narrative.ipynb).
 - [{fab}`youtube` YouTube](https://www.youtube.com/watch?v=Dovyd72eD70) recording of presentation.
 
 ### Objectives
 - Load data from a remote Parquet source with {func}`ak.from_parquet`.
 - Explore a complex dataset.
 - Mask and slice ragged array with {func}`ak.mask`.
 - Perform ragged reduction and broadcasting.
```

### Comparing `awkward-2.1.1/docs/getting-started/index.md` & `awkward-2.1.2/docs/getting-started/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/getting-started/papers-and-talks.md` & `awkward-2.1.2/docs/getting-started/papers-and-talks.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/getting-started/demo/what-is-an-awkward-array.ipynb` & `awkward-2.1.2/docs/getting-started/demo/what-is-an-awkward-array.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/image/example-hierarchy.svg` & `awkward-2.1.2/docs/image/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/reference/ak.behavior.rst` & `awkward-2.1.2/docs/reference/ak.behavior.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/reference/ak.builder.ArrayBuilder.rst` & `awkward-2.1.2/docs/reference/ak.builder.ArrayBuilder.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/reference/awkwardforth.rst` & `awkward-2.1.2/docs/reference/awkwardforth.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/reference/toctree.txt` & `awkward-2.1.2/docs/reference/toctree.txt`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/10-minutes-to-awkward-array.md` & `awkward-2.1.2/docs/user-guide/10-minutes-to-awkward-array.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-combinatorics-best-match.md` & `awkward-2.1.2/docs/user-guide/how-to-combinatorics-best-match.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-combinatorics-cartesian-combinations.md` & `awkward-2.1.2/docs/user-guide/how-to-combinatorics-cartesian-combinations.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-convert-arrow.md` & `awkward-2.1.2/docs/user-guide/how-to-convert-arrow.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-convert-buffers.md` & `awkward-2.1.2/docs/user-guide/how-to-convert-buffers.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-convert-json.md` & `awkward-2.1.2/docs/user-guide/how-to-convert-json.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-convert-numpy.md` & `awkward-2.1.2/docs/user-guide/how-to-convert-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-convert-pandas.md` & `awkward-2.1.2/docs/user-guide/how-to-convert-pandas.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-convert-python.md` & `awkward-2.1.2/docs/user-guide/how-to-convert-python.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-convert-rdataframe.md` & `awkward-2.1.2/docs/user-guide/how-to-convert-rdataframe.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-create-arraybuilder.md` & `awkward-2.1.2/docs/user-guide/how-to-create-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-create-constructors.md` & `awkward-2.1.2/docs/user-guide/how-to-create-constructors.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-create-lists.md` & `awkward-2.1.2/docs/user-guide/how-to-create-lists.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-create-missing.md` & `awkward-2.1.2/docs/user-guide/how-to-create-missing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-create-records.md` & `awkward-2.1.2/docs/user-guide/how-to-create-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-create-strings.md` & `awkward-2.1.2/docs/user-guide/how-to-create-strings.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-create-unflatten-group.md` & `awkward-2.1.2/docs/user-guide/how-to-create-unflatten-group.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-examine-checking-validity.md` & `awkward-2.1.2/docs/user-guide/how-to-examine-checking-validity.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-examine-list-fields.md` & `awkward-2.1.2/docs/user-guide/how-to-examine-list-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-examine-simple-slicing.md` & `awkward-2.1.2/docs/user-guide/how-to-examine-simple-slicing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-examine-single-item.md` & `awkward-2.1.2/docs/user-guide/how-to-examine-single-item.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-examine-type.md` & `awkward-2.1.2/docs/user-guide/how-to-examine-type.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-filter-cut-mask.md` & `awkward-2.1.2/docs/user-guide/how-to-filter-cut-mask.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-filter-masked.md` & `awkward-2.1.2/docs/user-guide/how-to-filter-masked.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-filter-num.md` & `awkward-2.1.2/docs/user-guide/how-to-filter-num.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-filter-ragged.md` & `awkward-2.1.2/docs/user-guide/how-to-filter-ragged.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-math-argminmax.md` & `awkward-2.1.2/docs/user-guide/how-to-math-argminmax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-math-broadcasting.md` & `awkward-2.1.2/docs/user-guide/how-to-math-broadcasting.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-math-gpu.md` & `awkward-2.1.2/docs/user-guide/how-to-math-gpu.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-math-numpy.md` & `awkward-2.1.2/docs/user-guide/how-to-math-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-math-reducing.md` & `awkward-2.1.2/docs/user-guide/how-to-math-reducing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-math-statistics.md` & `awkward-2.1.2/docs/user-guide/how-to-math-statistics.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-restructure-add-fields.md` & `awkward-2.1.2/docs/user-guide/how-to-restructure-add-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-restructure-concatenate.md` & `awkward-2.1.2/docs/user-guide/how-to-restructure-concatenate.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-restructure-flatten.md` & `awkward-2.1.2/docs/user-guide/how-to-restructure-flatten.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-restructure-pad.md` & `awkward-2.1.2/docs/user-guide/how-to-restructure-pad.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-restructure-rename-records.md` & `awkward-2.1.2/docs/user-guide/how-to-restructure-rename-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-restructure-sort.md` & `awkward-2.1.2/docs/user-guide/how-to-restructure-sort.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-restructure-zip-project.md` & `awkward-2.1.2/docs/user-guide/how-to-restructure-zip-project.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-specialize-differentiate-jax.md` & `awkward-2.1.2/docs/user-guide/how-to-specialize-differentiate-jax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-specialize-in-numba.md` & `awkward-2.1.2/docs/user-guide/how-to-specialize-in-numba.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-specialize-lorentz.md` & `awkward-2.1.2/docs/user-guide/how-to-specialize-lorentz.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-specialize-override-numpy.md` & `awkward-2.1.2/docs/user-guide/how-to-specialize-override-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-specialize-subclass.md` & `awkward-2.1.2/docs/user-guide/how-to-specialize-subclass.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-use-header-only-layoutbuilder.md` & `awkward-2.1.2/docs/user-guide/how-to-use-header-only-layoutbuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-use-in-numba-arraybuilder.md` & `awkward-2.1.2/docs/user-guide/how-to-use-in-numba-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-use-in-numba-cuda.ipynb` & `awkward-2.1.2/docs/user-guide/how-to-use-in-numba-cuda.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs/user-guide/how-to-use-in-numba-features.md` & `awkward-2.1.2/docs/user-guide/how-to-use-in-numba-features.md`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/panel-data-analysts.png` & `awkward-2.1.2/docs-img/panel-data-analysts.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/panel-data-analysts.svg` & `awkward-2.1.2/docs-img/panel-data-analysts.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/panel-developers.png` & `awkward-2.1.2/docs-img/panel-developers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/panel-developers.svg` & `awkward-2.1.2/docs-img/panel-developers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/panel-doxygen.png` & `awkward-2.1.2/docs-img/panel-doxygen.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/panel-sphinx.png` & `awkward-2.1.2/docs-img/panel-sphinx.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/panel-tutorials-alternate.png` & `awkward-2.1.2/docs-img/panel-tutorials-alternate.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/panel-tutorials.png` & `awkward-2.1.2/docs-img/panel-tutorials.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/awkward-1-0-layers.pdf` & `awkward-2.1.2/docs-img/diagrams/awkward-1-0-layers.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/awkward-1-0-layers.png` & `awkward-2.1.2/docs-img/diagrams/awkward-1-0-layers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/awkward-1-0-layers.svg` & `awkward-2.1.2/docs-img/diagrams/awkward-1-0-layers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/awkward-timeline.pdf` & `awkward-2.1.2/docs-img/diagrams/awkward-timeline.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/awkward-timeline.png` & `awkward-2.1.2/docs-img/diagrams/awkward-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/awkward-timeline.svg` & `awkward-2.1.2/docs-img/diagrams/awkward-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.png` & `awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip-github.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg` & `awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/awkward-uproot-timeline-pip.png` & `awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/awkward-uproot-timeline-pip.svg` & `awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline-pip.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/awkward-uproot-timeline.png` & `awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/awkward-uproot-timeline.svg` & `awkward-2.1.2/docs-img/diagrams/awkward-uproot-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/cartoon-broadcasting.png` & `awkward-2.1.2/docs-img/diagrams/cartoon-broadcasting.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/cartoon-broadcasting.svg` & `awkward-2.1.2/docs-img/diagrams/cartoon-broadcasting.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/cartoon-cartesian.png` & `awkward-2.1.2/docs-img/diagrams/cartoon-cartesian.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/cartoon-cartesian.svg` & `awkward-2.1.2/docs-img/diagrams/cartoon-cartesian.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/cartoon-combinations.png` & `awkward-2.1.2/docs-img/diagrams/cartoon-combinations.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/cartoon-combinations.svg` & `awkward-2.1.2/docs-img/diagrams/cartoon-combinations.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/cartoon-schematic.png` & `awkward-2.1.2/docs-img/diagrams/cartoon-schematic.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/cartoon-schematic.svg` & `awkward-2.1.2/docs-img/diagrams/cartoon-schematic.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/example-array.svg` & `awkward-2.1.2/docs-img/diagrams/example-array.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/example-hierarchy.png` & `awkward-2.1.2/docs-img/diagrams/example-hierarchy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/example-hierarchy.svg` & `awkward-2.1.2/docs-img/diagrams/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/example-reduction-sum-only.svg` & `awkward-2.1.2/docs-img/diagrams/example-reduction-sum-only.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/example-reduction-sum.svg` & `awkward-2.1.2/docs-img/diagrams/example-reduction-sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/example-reduction.png` & `awkward-2.1.2/docs-img/diagrams/example-reduction.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/example-reduction.svg` & `awkward-2.1.2/docs-img/diagrams/example-reduction.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/git-strategy.pdf` & `awkward-2.1.2/docs-img/diagrams/git-strategy.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/git-strategy.png` & `awkward-2.1.2/docs-img/diagrams/git-strategy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/git-strategy.svg` & `awkward-2.1.2/docs-img/diagrams/git-strategy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/how-it-works-muons.png` & `awkward-2.1.2/docs-img/diagrams/how-it-works-muons.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/how-it-works-muons.svg` & `awkward-2.1.2/docs-img/diagrams/how-it-works-muons.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/how-it-works.svg` & `awkward-2.1.2/docs-img/diagrams/how-it-works.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/sorting-axis.svg` & `awkward-2.1.2/docs-img/diagrams/sorting-axis.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/reducers/all.svg` & `awkward-2.1.2/docs-img/diagrams/reducers/all.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/reducers/any.svg` & `awkward-2.1.2/docs-img/diagrams/reducers/any.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/reducers/argmax.svg` & `awkward-2.1.2/docs-img/diagrams/reducers/argmax.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/reducers/argmin.svg` & `awkward-2.1.2/docs-img/diagrams/reducers/argmin.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/reducers/count.svg` & `awkward-2.1.2/docs-img/diagrams/reducers/count.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/reducers/count_nonzero.svg` & `awkward-2.1.2/docs-img/diagrams/reducers/count_nonzero.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/reducers/max.svg` & `awkward-2.1.2/docs-img/diagrams/reducers/max.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/reducers/min.svg` & `awkward-2.1.2/docs-img/diagrams/reducers/min.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/reducers/product.svg` & `awkward-2.1.2/docs-img/diagrams/reducers/product.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/diagrams/reducers/sum.svg` & `awkward-2.1.2/docs-img/diagrams/reducers/sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/logo/favicon.ico` & `awkward-2.1.2/docs-img/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/logo/logo-300px-white.png` & `awkward-2.1.2/docs-img/logo/logo-300px-white.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/logo/logo-300px.png` & `awkward-2.1.2/docs-img/logo/logo-300px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/logo/logo-600px.png` & `awkward-2.1.2/docs-img/logo/logo-600px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/logo/logo.svg` & `awkward-2.1.2/docs-img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/photos/desire-path.jpg` & `awkward-2.1.2/docs-img/photos/desire-path.jpg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/plots/awkward-0-popularity.pdf` & `awkward-2.1.2/docs-img/plots/awkward-0-popularity.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/plots/awkward-0-popularity.png` & `awkward-2.1.2/docs-img/plots/awkward-0-popularity.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/plots/awkward-0-popularity.svg` & `awkward-2.1.2/docs-img/plots/awkward-0-popularity.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/plots/bikeroutes-scaling.svg` & `awkward-2.1.2/docs-img/plots/bikeroutes-scaling.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/docs-img/screenshots/github-issues-documentation.png` & `awkward-2.1.2/docs-img/screenshots/github-issues-documentation.png`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/__init__.py` & `awkward-2.1.2/src/awkward/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import awkward._errors
 import awkward._lookup
 
 # third-party connectors
 import awkward._connect.numpy
 import awkward._connect.numexpr
 import awkward.numba
+import awkward.cppyy
 import awkward.jax
 import awkward.typetracer
 import awkward._typetracer  # todo: remove this after "deprecation" period
 
 # high-level interface
 from awkward.highlevel import *
```

### Comparing `awkward-2.1.1/src/awkward/_backends.py` & `awkward-2.1.2/src/awkward/_backends.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,43 +11,43 @@
 from awkward._nplikes import nplike_of
 from awkward._nplikes.cupy import Cupy
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyLike, NumpyMetadata
 from awkward._nplikes.typetracer import MaybeNone, TypeTracer, TypeTracerArray
 from awkward._singleton import Singleton
-from awkward.typing import Callable, Final, Tuple, TypeAlias, TypeVar, Unpack
+from awkward._typing import Callable, Final, Tuple, TypeAlias, TypeVar, Unpack
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
 T = TypeVar("T", covariant=True)
 KernelKeyType: TypeAlias = Tuple[str, Unpack[Tuple[np.dtype, ...]]]
 KernelType: TypeAlias = Callable[..., None]
 
 
 class Backend(Singleton, ABC):
     @property
     @abstractmethod
     def name(self) -> str:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @property
     @abstractmethod
     def nplike(self) -> NumpyLike:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @property
     @abstractmethod
     def index_nplike(self) -> NumpyLike:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def __getitem__(self, key: KernelKeyType) -> KernelType:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def apply_reducer(
         self,
         reducer: ak._reducers.Reducer,
         layout: ak.contents.NumpyArray,
         parents: ak.index.Index,
         outlength: int,
@@ -99,17 +99,15 @@
 
         cupy = cuda.import_cupy("Awkward Arrays with CUDA")
         _cuda_kernels = cuda.initialize_cuda_kernels(cupy)
         func = _cuda_kernels[index]
         if func is not None:
             return CupyKernel(func, index)
         else:
-            raise ak._errors.wrap_error(
-                AssertionError(f"CuPyKernel not found: {index!r}")
-            )
+            raise AssertionError(f"CuPyKernel not found: {index!r}")
 
 
 class JaxBackend(Backend):
     name: Final[str] = "jax"
 
     _jax: Jax
     _numpy: Numpy
@@ -142,17 +140,15 @@
         jax_reducer = get_jax_reducer(reducer)
         return jax_reducer.apply(layout, parents, outlength)
 
     def apply_ufunc(self, ufunc, method, args, kwargs):
         from awkward._connect.jax import get_jax_ufunc
 
         if method != "__call__":
-            raise ak._errors.wrap_error(
-                ValueError(f"unsupported ufunc method {method} called")
-            )
+            raise ValueError(f"unsupported ufunc method {method} called")
 
         jax_ufunc = get_jax_ufunc(ufunc)
         return jax_ufunc(*args, **kwargs)
 
 
 class TypeTracerBackend(Backend):
     name: Final[str] = "typetracer"
@@ -208,33 +204,31 @@
     elif isinstance(nplike, Cupy):
         return CupyBackend.instance()
     elif isinstance(nplike, Jax):
         return JaxBackend.instance()
     elif isinstance(nplike, TypeTracer):
         return TypeTracerBackend.instance()
     else:
-        raise ak._errors.wrap_error(ValueError("unrecognised nplike", nplike))
+        raise ValueError("unrecognised nplike", nplike)
 
 
 def common_backend(backends: Collection[Backend]) -> Backend:
     unique_backends = frozenset(backends)
     # Either we have one nplike, or one + typetracer
     if len(unique_backends) == 1:
         return next(iter(unique_backends))
     else:
         # We allow typetracers to mix with other nplikes, and take precedence
         for backend in unique_backends:
             if not backend.nplike.known_data:
                 return backend
 
-        raise ak._errors.wrap_error(
-            ValueError(
-                "cannot operate on arrays with incompatible backends. Use #ak.to_backend to coerce the arrays "
-                "to the same backend"
-            )
+        raise ValueError(
+            "cannot operate on arrays with incompatible backends. Use #ak.to_backend to coerce the arrays "
+            "to the same backend"
         )
 
 
 _UNSET = object()
 D = TypeVar("D")
 
 
@@ -251,15 +245,15 @@
     # Implementation detail: right now, we are one-to-one mapping `nplike` to a backend
     # The distinction is still useful because nplikes are just the array abstraction,
     # whilst backends incorporate more Awkward logic
     nplike = nplike_of(*objects, default=None)
     if nplike is not None:
         return _backend_for_nplike(nplike)
     elif default is _UNSET:
-        raise ak._errors.wrap_error(ValueError("could not find backend for", objects))
+        raise ValueError("could not find backend for", objects)
     else:
         return default
 
 
 _backends: Final[dict[str, type[Backend]]] = {
     b.name: b for b in (NumpyBackend, CupyBackend, JaxBackend, TypeTracerBackend)
 }
@@ -267,8 +261,8 @@
 
 def regularize_backend(backend: str | Backend) -> Backend:
     if isinstance(backend, Backend):
         return backend
     elif backend in _backends:
         return _backends[backend].instance()
     else:
-        raise ak._errors.wrap_error(ValueError(f"No such backend {backend!r} exists."))
+        raise ValueError(f"No such backend {backend!r} exists.")
```

### Comparing `awkward-2.1.1/src/awkward/_behavior.py` & `awkward-2.1.2/src/awkward/_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_broadcasting.py` & `awkward-2.1.2/src/awkward/_broadcasting.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 from collections.abc import Sequence
 
 import awkward as ak
 from awkward._behavior import find_custom_broadcast
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
+from awkward._parameters import (
+    parameters_are_empty,
+    parameters_are_equal,
+    parameters_intersect,
+)
+from awkward._typing import Any, Callable, Dict, List, TypeAlias, Union
 from awkward._util import unset
 from awkward.contents.bitmaskedarray import BitMaskedArray
 from awkward.contents.bytemaskedarray import ByteMaskedArray
 from awkward.contents.content import Content
 from awkward.contents.emptyarray import EmptyArray
 from awkward.contents.indexedarray import IndexedArray
 from awkward.contents.indexedoptionarray import IndexedOptionArray
@@ -28,15 +34,14 @@
 from awkward.contents.unmaskedarray import UnmaskedArray
 from awkward.index import (  # IndexU8,  ; Index32,  ; IndexU32,  ; noqa: F401
     Index,
     Index8,
     Index64,
 )
 from awkward.record import Record
-from awkward.typing import Any, Callable, Dict, List, TypeAlias, Union
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 optiontypes = (IndexedOptionArray, ByteMaskedArray, BitMaskedArray, UnmaskedArray)
 listtypes = (ListOffsetArray, ListArray, RegularArray)
 
@@ -102,23 +107,21 @@
         return "in " + options["function_name"]
 
 
 def checklength(inputs, options):
     length = inputs[0].length
     for x in inputs[1:]:
         if x.length != length:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "cannot broadcast {} of length {} with {} of length {}{}".format(
-                        type(inputs[0]).__name__,
-                        length,
-                        type(x).__name__,
-                        x.length,
-                        in_function(options),
-                    )
+            raise ValueError(
+                "cannot broadcast {} of length {} with {} of length {}{}".format(
+                    type(inputs[0]).__name__,
+                    length,
+                    type(x).__name__,
+                    x.length,
+                    in_function(options),
                 )
             )
 
 
 def all_same_offsets(backend: ak._backends.Backend, inputs: list) -> bool:
     index_nplike = backend.index_nplike
 
@@ -151,15 +154,15 @@
                 return False
 
         elif isinstance(x, RegularArray):
             if x.size == 0:
                 my_offsets = index_nplike.empty(0, dtype=np.int64)
             else:
                 my_offsets = index_nplike.arange(
-                    0, x.content.length, x.size, dtype=np.int64
+                    0, x.content.length + 1, x.size, dtype=np.int64
                 )
 
             if offsets is None:
                 offsets = my_offsets
             elif not index_nplike.array_equal(offsets, my_offsets):
                 return False
 
@@ -236,15 +239,15 @@
 
     parameters = None
     if len(input_parameters) > 0:
         # All parameters must match this first layout's parameters
         first_parameters = input_parameters[0]
         # Ensure all parameters match, or set parameters to None
         for other_parameters in input_parameters[1:]:
-            if not ak.forms.form._parameters_equal(first_parameters, other_parameters):
+            if not parameters_are_equal(first_parameters, other_parameters):
                 break
         else:
             parameters = first_parameters
 
     def apply(n_outputs: int) -> list[dict[str, Any] | None]:
         # NB: we don't make unique copies here, so let's hope everyone
         # is well-behaved downstream!
@@ -274,22 +277,22 @@
 
     intersected_parameters = None
     parameters_to_intersect = []
     # Build a list of set-like dict.items() views.
     # If we encounter None-parameters, then we stop early
     # as there can be no intersection.
     for parameters in input_parameters:
-        if ak.forms.form._parameters_is_empty(parameters):
+        if parameters_are_empty(parameters):
             break
         else:
             parameters_to_intersect.append(parameters)
     # Otherwise, build the intersected parameter dict
     else:
         intersected_parameters = functools.reduce(
-            ak.forms.form._parameters_intersect, parameters_to_intersect
+            parameters_intersect, parameters_to_intersect
         )
 
     def apply(n_outputs: int) -> list[dict[str, Any] | None]:
         # NB: we don't make unique copies here, so let's hope everyone
         # is well-behaved downstream!
         return [intersected_parameters] * n_outputs
 
@@ -313,19 +316,17 @@
     given contents does not match the requested list length, a ValueError is raised.
     """
     # Find the parameters of the inputs, with None values for non-Contents
     input_parameters = [_parameters_of(c, default=None) for c in inputs]
 
     def apply(n_outputs) -> list[dict[str, Any] | None]:
         if n_outputs != len(inputs):
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "cannot follow one-to-one parameter broadcasting rule for actions "
-                    "which change the number of outputs."
-                )
+            raise ValueError(
+                "cannot follow one-to-one parameter broadcasting rule for actions "
+                "which change the number of outputs."
             )
         return input_parameters
 
     return apply
 
 
 def none_parameters_factory(
@@ -353,14 +354,20 @@
     BroadcastParameterRule.INTERSECT: intersection_parameters_factory,
     BroadcastParameterRule.ALL_OR_NOTHING: all_or_nothing_parameters_factory,
     BroadcastParameterRule.ONE_TO_ONE: one_to_one_parameters_factory,
     BroadcastParameterRule.NONE: none_parameters_factory,
 }
 
 
+def left_broadcast_to(content: Content, depth: int) -> Content:
+    for _ in range(content.purelist_depth, depth):
+        content = RegularArray(content, 1, content.length)
+    return content
+
+
 def apply_step(
     backend: ak._backends.Backend,
     inputs: Sequence,
     action,
     depth: int,
     depth_context,
     lateral_context,
@@ -380,650 +387,645 @@
         isinstance(x, RegularArray) for x in inputs
     ):
         inputs = [
             x.to_ListOffsetArray64(False) if isinstance(x, RegularArray) else x
             for x in inputs
         ]
 
+    contents = [x for x in inputs if isinstance(x, Content)]
+
     # Handle implicit right-broadcasting (NumPy-like broadcasting).
     if options["right_broadcast"] and any(isinstance(x, listtypes) for x in inputs):
-        maxdepth = max(x.purelist_depth for x in inputs if isinstance(x, Content))
+        max_depth = max(x.purelist_depth for x in contents)
 
-        if maxdepth > 0 and all(
-            x.purelist_isregular for x in inputs if isinstance(x, Content)
-        ):
-            nextinputs = []
-            for obj in inputs:
-                if isinstance(obj, Content):
-                    while obj.purelist_depth < maxdepth:
-                        obj = RegularArray(obj, 1, obj.length)
-                nextinputs.append(obj)
+        if max_depth > 0 and all(x.purelist_isregular for x in contents):
+            nextinputs = [
+                left_broadcast_to(o, max_depth) if isinstance(o, Content) else o
+                for o in inputs
+            ]
+            # Did a broadcast take place?
             if any(x is not y for x, y in zip(inputs, nextinputs)):
                 return apply_step(
                     backend,
                     nextinputs,
                     action,
                     depth,
                     depth_context,
                     lateral_context,
                     behavior,
                     options,
                 )
 
     # Now all lengths must agree.
     if backend.nplike.known_data:
-        checklength([x for x in inputs if isinstance(x, Content)], options)
+        checklength(contents, options)
     else:
-        for x in inputs:
-            if isinstance(x, Content):
-                x._touch_shape(recursive=False)
+        for x in contents:
+            x._touch_shape(recursive=False)
 
     # Load the parameter broadcasting rule implementation
     rule = options["broadcast_parameters_rule"]
     try:
         parameters_factory_impl = BROADCAST_RULE_TO_FACTORY_IMPL[rule]
     except KeyError:
-        raise ak._errors.wrap_error(
-            ValueError(
-                f"`broadcast_parameters_rule` should be one of {[str(x) for x in BroadcastParameterRule]}, "
-                f"but this routine received `{rule}`"
-            )
+        raise ValueError(
+            f"`broadcast_parameters_rule` should be one of {[str(x) for x in BroadcastParameterRule]}, "
+            f"but this routine received `{rule}`"
         ) from None
     parameters_factory = parameters_factory_impl(inputs)
 
     # This whole function is one big switch statement.
-    def continuation():
-        # Any EmptyArrays?
-        if any(isinstance(x, EmptyArray) for x in inputs):
-            nextinputs = [
-                x.to_NumpyArray(np.float64, backend) if isinstance(x, EmptyArray) else x
-                for x in inputs
-            ]
-            return apply_step(
-                backend,
-                nextinputs,
-                action,
-                depth,
-                copy.copy(depth_context),
-                lateral_context,
-                behavior,
-                options,
-            )
-
-        # Any NumpyArrays with ndim != 1?
-        elif any(isinstance(x, NumpyArray) and x.data.ndim != 1 for x in inputs):
-            nextinputs = [
-                x.to_RegularArray() if isinstance(x, NumpyArray) else x for x in inputs
-            ]
-            return apply_step(
-                backend,
-                nextinputs,
-                action,
-                depth,
-                copy.copy(depth_context),
-                lateral_context,
-                behavior,
-                options,
-            )
-
-        # Any IndexedArrays?
-        elif any(isinstance(x, IndexedArray) for x in inputs):
-            nextinputs = [
-                x.project() if isinstance(x, IndexedArray) else x for x in inputs
-            ]
-            return apply_step(
-                backend,
-                nextinputs,
-                action,
-                depth,
-                copy.copy(depth_context),
-                lateral_context,
-                behavior,
-                options,
-            )
-
-        # Any UnionArrays?
-        elif any(isinstance(x, UnionArray) for x in inputs):
-            if not backend.nplike.known_data:
-                numtags, length = [], None
-                for x in inputs:
-                    if isinstance(x, UnionArray):
-                        x._touch_data(recursive=False)
-                        numtags.append(len(x.contents))
-                        if length is None:
-                            length = x.tags.data.shape[0]
-                assert length is not unknown_length
-
-                all_combos = list(itertools.product(*[range(x) for x in numtags]))
-
-                tags = backend.index_nplike.empty(length, dtype=np.int8)
-                index = backend.index_nplike.empty(length, dtype=np.int64)
-                numoutputs, outcontents = None, []
-                for combo in all_combos:
-                    nextinputs = []
-                    i = 0
-                    for x in inputs:
-                        if isinstance(x, UnionArray):
-                            nextinputs.append(x._contents[combo[i]])
-                            i += 1
-                        else:
-                            nextinputs.append(x)
-
-                    outcontents.append(
-                        apply_step(
-                            backend,
-                            nextinputs,
-                            action,
-                            depth,
-                            copy.copy(depth_context),
-                            lateral_context,
-                            behavior,
-                            options,
+    def broadcast_any_record():
+        if not options["allow_records"]:
+            raise ValueError(f"cannot broadcast records {in_function(options)}")
+
+        fields, length, istuple = unset, unset, unset
+        for x in contents:
+            if x.is_record:
+                if fields is unset:
+                    fields = x.fields
+                elif set(fields) != set(x.fields):
+                    raise ValueError(
+                        "cannot broadcast records because fields don't "
+                        "match{}:\n    {}\n    {}".format(
+                            in_function(options),
+                            ", ".join(sorted(fields)),
+                            ", ".join(sorted(x.fields)),
                         )
                     )
-                    assert isinstance(outcontents[-1], tuple)
-                    if numoutputs is None:
-                        numoutputs = outcontents[-1].length
-                    else:
-                        assert (
-                            numoutputs is unknown_length
-                            or outcontents[-1].length is unknown_length
-                        ) or numoutputs == outcontents[-1].length
-
-                assert numoutputs is not None
-
-            else:
-                tagslist, numtags, length = [], [], None
-                for x in inputs:
-                    if isinstance(x, UnionArray):
-                        tagslist.append(x.tags.raw(backend.index_nplike))
-                        numtags.append(len(x.contents))
-                        if length is None:
-                            length = tagslist[-1].shape[0]
-                        elif length != tagslist[-1].shape[0]:
-                            raise ak._errors.wrap_error(
-                                ValueError(
-                                    "cannot broadcast UnionArray of length {} "
-                                    "with UnionArray of length {}{}".format(
-                                        length,
-                                        tagslist[-1].shape[0],
-                                        in_function(options),
-                                    )
-                                )
-                            )
-                assert length is not unknown_length
-
-                combos = backend.index_nplike.stack(tagslist, axis=-1)
-
-                all_combos = backend.index_nplike.asarray(
-                    list(itertools.product(*[range(x) for x in numtags])),
-                    dtype=[(str(i), combos.dtype) for i in range(len(tagslist))],
-                )
-                combos = backend.index_nplike.reshape(
-                    combos.view([(str(i), combos.dtype) for i in range(len(tagslist))]),
-                    (length,),
-                )
-
-                tags = backend.index_nplike.empty(length, dtype=np.int8)
-                index = backend.index_nplike.empty(length, dtype=np.int64)
-                numoutputs, outcontents = None, []
-                for tag, combo in enumerate(all_combos):
-                    mask = combos == combo
-                    tags[mask] = tag
-                    index[mask] = backend.index_nplike.arange(
-                        backend.index_nplike.count_nonzero(mask), dtype=np.int64
-                    )
-                    nextinputs = []
-                    i = 0
-                    for x in inputs:
-                        if isinstance(x, UnionArray):
-                            nextinputs.append(x[mask].project(combo[str(i)]))
-                            i += 1
-                        elif isinstance(x, Content):
-                            nextinputs.append(x[mask])
-                        else:
-                            nextinputs.append(x)
-                    outcontents.append(
-                        apply_step(
-                            backend,
-                            nextinputs,
-                            action,
-                            depth,
-                            copy.copy(depth_context),
-                            lateral_context,
-                            behavior,
-                            options,
+                if length is unset:
+                    length = x.length
+                elif length != x.length:
+                    raise ValueError(
+                        "cannot broadcast RecordArray of length {} "
+                        "with RecordArray of length {}{}".format(
+                            length, x.length, in_function(options)
                         )
                     )
-                    assert isinstance(outcontents[-1], tuple)
-                    if numoutputs is None:
-                        numoutputs = len(outcontents[-1])
-                    else:
-                        assert numoutputs == len(outcontents[-1])
-
-                assert numoutputs is not None
-
-            parameters = parameters_factory(numoutputs)
-            return tuple(
-                UnionArray.simplified(
-                    Index8(tags),
-                    Index64(index),
-                    [x[i] for x in outcontents],
-                    parameters=p,
+                # Records win over tuples
+                if istuple is unset or not x.is_tuple:
+                    istuple = False
+
+        outcontents, numoutputs = [], None
+        for field in fields:
+            outcontents.append(
+                apply_step(
+                    backend,
+                    [x[field] if isinstance(x, RecordArray) else x for x in inputs],
+                    action,
+                    depth,
+                    copy.copy(depth_context),
+                    lateral_context,
+                    behavior,
+                    options,
                 )
-                for i, p in enumerate(parameters)
             )
+            assert isinstance(outcontents[-1], tuple)
+            if numoutputs is not None:
+                assert numoutputs == len(outcontents[-1])
+            numoutputs = len(outcontents[-1])
+
+        return tuple(
+            RecordArray(
+                [x[i] for x in outcontents],
+                None if istuple else fields,
+                length,
+                parameters=p,
+            )
+            for i, p in enumerate(parameters_factory(numoutputs))
+        )
+
+    def broadcast_any_list():
+        # All regular?
+        if all(x.is_regular or not x.is_list for x in contents):
+            # Ensure all layouts have same length
+            length = unset
+            for x in contents:
+                if length is unset:
+                    length = x.length
+                elif backend.nplike.known_data:
+                    assert length == x.length
+            assert length is not unset
+
+            if any(x.size == 0 for x in contents if x.is_regular):
+                dimsize = 0
+            else:
+                dimsize = max(x.size for x in contents if x.is_regular)
 
-        # Any option-types?
-        elif any(isinstance(x, optiontypes) for x in inputs):
             if backend.nplike.known_data:
-                mask = None
-                for x in inputs:
-                    if isinstance(x, optiontypes):
-                        m = x.mask_as_bool(valid_when=False)
-                        if mask is None:
-                            mask = m
-                        else:
-                            mask = backend.index_nplike.logical_or(
-                                mask, m, maybe_out=mask
+                for x in contents:
+                    if x.is_regular:
+                        if dimsize > 1 and x.size == 1:
+                            # For any (N, 1) array, we know we'll broadcast to (N, M) where M is maxsize
+                            tmpindex = Index64(
+                                backend.index_nplike.repeat(
+                                    backend.index_nplike.arange(
+                                        x.length, dtype=np.int64
+                                    ),
+                                    dimsize,
+                                ),
+                                nplike=backend.index_nplike,
                             )
 
-                nextmask = Index8(mask.view(np.int8))
-                index = backend.index_nplike.full(mask.shape[0], -1, dtype=np.int64)
-                index[~mask] = backend.index_nplike.arange(
-                    mask.shape[0] - backend.index_nplike.count_nonzero(mask),
-                    dtype=np.int64,
-                )
-                index = Index64(index)
-                if any(not isinstance(x, optiontypes) for x in inputs):
-                    nextindex = backend.index_nplike.arange(
-                        mask.shape[0], dtype=np.int64
-                    )
-                    nextindex[mask] = -1
-                    nextindex = Index64(nextindex)
-
                 nextinputs = []
                 for x in inputs:
-                    if isinstance(x, optiontypes):
-                        nextinputs.append(x.project(nextmask))
-                    elif isinstance(x, Content):
-                        nextinputs.append(
-                            IndexedOptionArray(nextindex, x).project(nextmask)
-                        )
+                    if isinstance(x, RegularArray):
+                        if dimsize > 1 and x.size == 1:
+                            nextinputs.append(
+                                x.content[: x.length * x.size]._carry(
+                                    tmpindex, allow_lazy=False
+                                )
+                            )
+                        elif x.size == dimsize:
+                            nextinputs.append(x.content[: x.length * x.size])
+                        elif dimsize == 0:
+                            nextinputs.append(x.content[:0])
+                        else:
+                            raise ValueError(
+                                "cannot broadcast RegularArray of size "
+                                "{} with RegularArray of size {} {}".format(
+                                    x.size, dimsize, in_function(options)
+                                )
+                            )
                     else:
                         nextinputs.append(x)
 
             else:
-                index = None
                 nextinputs = []
                 for x in inputs:
-                    if isinstance(x, optiontypes):
+                    if isinstance(x, RegularArray):
                         x._touch_data(recursive=False)
-                        index = Index64(
-                            backend.index_nplike.empty(x.length, dtype=np.int64)
-                        )
                         nextinputs.append(x.content)
                     else:
                         nextinputs.append(x)
-                assert index is not None
 
             outcontent = apply_step(
                 backend,
                 nextinputs,
                 action,
-                depth,
+                depth + 1,
                 copy.copy(depth_context),
                 lateral_context,
                 behavior,
                 options,
             )
             assert isinstance(outcontent, tuple)
             parameters = parameters_factory(len(outcontent))
             return tuple(
-                IndexedOptionArray.simplified(index, x, parameters=p)
+                RegularArray(x, dimsize, length, parameters=p)
                 for x, p in zip(outcontent, parameters)
             )
 
-        # Any list-types?
-        elif any(isinstance(x, listtypes) for x in inputs):
-            # All regular?
-            if all(
-                isinstance(x, RegularArray) or not isinstance(x, listtypes)
-                for x in inputs
-            ):
-                # Ensure all layouts have same length
-                length = unset
-                for x in inputs:
-                    if isinstance(x, Content):
-                        if length is unset:
-                            length = x.length
-                        elif backend.nplike.known_data:
-                            assert length == x.length
-                assert length is not unset
-
-                if any(x.size == 0 for x in inputs if isinstance(x, RegularArray)):
-                    dimsize = 0
+        elif not backend.nplike.known_data:
+            offsets = None
+            nextinputs = []
+            for x in inputs:
+                if isinstance(x, ListOffsetArray):
+                    x._touch_data(recursive=False)
+                    offsets = Index64(
+                        backend.index_nplike.empty(
+                            x.offsets.data.shape[0], dtype=np.int64
+                        ),
+                        nplike=backend.index_nplike,
+                    )
+                    nextinputs.append(x.content)
+                elif isinstance(x, ListArray):
+                    x._touch_data(recursive=False)
+                    offsets = Index64(
+                        backend.index_nplike.empty(
+                            x.starts.data.shape[0] + 1, dtype=np.int64
+                        ),
+                        nplike=backend.index_nplike,
+                    )
+                    nextinputs.append(x.content)
+                elif isinstance(x, RegularArray):
+                    x._touch_data(recursive=False)
+                    nextinputs.append(x.content)
                 else:
-                    dimsize = max(x.size for x in inputs if isinstance(x, RegularArray))
+                    nextinputs.append(x)
+            assert offsets is not None
 
-                if backend.nplike.known_data:
-                    for x in inputs:
-                        if isinstance(x, RegularArray):
-                            if dimsize > 1 and x.size == 1:
-                                # For any (N, 1) array, we know we'll broadcast to (N, M) where M is maxsize
-                                tmpindex = Index64(
-                                    backend.index_nplike.repeat(
-                                        backend.index_nplike.arange(
-                                            x.length, dtype=np.int64
-                                        ),
-                                        dimsize,
-                                    ),
-                                    nplike=backend.index_nplike,
-                                )
+            outcontent = apply_step(
+                backend,
+                nextinputs,
+                action,
+                depth + 1,
+                copy.copy(depth_context),
+                lateral_context,
+                behavior,
+                options,
+            )
+            assert isinstance(outcontent, tuple)
+            parameters = parameters_factory(len(outcontent))
+            return tuple(
+                ListOffsetArray(offsets, x, parameters=p)
+                for x, p in zip(outcontent, parameters)
+            )
 
-                    nextinputs = []
-                    for x in inputs:
-                        if isinstance(x, RegularArray):
-                            if dimsize > 1 and x.size == 1:
-                                nextinputs.append(
-                                    x.content[: x.length * x.size]._carry(
-                                        tmpindex, allow_lazy=False
-                                    )
-                                )
-                            elif x.size == dimsize:
-                                nextinputs.append(x.content[: x.length * x.size])
-                            elif dimsize == 0:
-                                nextinputs.append(x.content[:0])
-                            else:
-                                raise ak._errors.wrap_error(
-                                    ValueError(
-                                        "cannot broadcast RegularArray of size "
-                                        "{} with RegularArray of size {} {}".format(
-                                            x.size, dimsize, in_function(options)
-                                        )
-                                    )
-                                )
-                        else:
-                            nextinputs.append(x)
+        # Not all regular, but all same offsets?
+        # Optimization: https://github.com/scikit-hep/awkward-1.0/issues/442
+        elif all_same_offsets(backend, inputs):
+            lencontent, offsets, starts, stops = None, None, None, None
+            nextinputs = []
 
+            for x in inputs:
+                if isinstance(x, ListOffsetArray):
+                    offsets = x.offsets
+                    lencontent = offsets[-1]
+                    nextinputs.append(x.content[:lencontent])
+
+                elif isinstance(x, ListArray):
+                    starts, stops = x.starts, x.stops
+                    if starts.length == 0 or stops.length == 0:
+                        nextinputs.append(x.content[:0])
+                    else:
+                        lencontent = backend.index_nplike.max(stops)
+                        nextinputs.append(x.content[:lencontent])
+                elif isinstance(x, RegularArray):
+                    nextinputs.append(x.content[: x.size * x.length])
                 else:
-                    nextinputs = []
-                    for x in inputs:
-                        if isinstance(x, RegularArray):
-                            x._touch_data(recursive=False)
-                            nextinputs.append(x.content)
-                        else:
-                            nextinputs.append(x)
+                    nextinputs.append(x)
 
-                outcontent = apply_step(
-                    backend,
-                    nextinputs,
-                    action,
-                    depth + 1,
-                    copy.copy(depth_context),
-                    lateral_context,
-                    behavior,
-                    options,
-                )
-                assert isinstance(outcontent, tuple)
-                parameters = parameters_factory(len(outcontent))
+            outcontent = apply_step(
+                backend,
+                nextinputs,
+                action,
+                depth + 1,
+                copy.copy(depth_context),
+                lateral_context,
+                behavior,
+                options,
+            )
+            assert isinstance(outcontent, tuple)
+            parameters = parameters_factory(len(outcontent))
+
+            if isinstance(offsets, Index):
                 return tuple(
-                    RegularArray(x, dimsize, length, parameters=p)
+                    ListOffsetArray(offsets, x, parameters=p).to_ListOffsetArray64(
+                        False
+                    )
                     for x, p in zip(outcontent, parameters)
                 )
-
-            elif not backend.nplike.known_data:
-                offsets = None
-                nextinputs = []
-                for x in inputs:
-                    if isinstance(x, ListOffsetArray):
-                        x._touch_data(recursive=False)
-                        offsets = Index64(
-                            backend.index_nplike.empty(
-                                x.offsets.data.shape[0], dtype=np.int64
-                            ),
-                            nplike=backend.index_nplike,
-                        )
-                        nextinputs.append(x.content)
-                    elif isinstance(x, ListArray):
-                        x._touch_data(recursive=False)
-                        offsets = Index64(
-                            backend.index_nplike.empty(
-                                x.starts.data.shape[0] + 1, dtype=np.int64
-                            ),
-                            nplike=backend.index_nplike,
-                        )
-                        nextinputs.append(x.content)
-                    elif isinstance(x, RegularArray):
-                        x._touch_data(recursive=False)
-                        nextinputs.append(x.content)
-                    else:
-                        nextinputs.append(x)
-                assert offsets is not None
-
-                outcontent = apply_step(
-                    backend,
-                    nextinputs,
-                    action,
-                    depth + 1,
-                    copy.copy(depth_context),
-                    lateral_context,
-                    behavior,
-                    options,
-                )
-                assert isinstance(outcontent, tuple)
-                parameters = parameters_factory(len(outcontent))
+            elif isinstance(starts, Index) and isinstance(stops, Index):
                 return tuple(
-                    ListOffsetArray(offsets, x, parameters=p)
+                    ListArray(starts, stops, x, parameters=p).to_ListOffsetArray64(
+                        False
+                    )
                     for x, p in zip(outcontent, parameters)
                 )
+            else:
+                raise AssertionError(
+                    "unexpected offsets, starts: {}, {}".format(
+                        type(offsets), type(starts)
+                    )
+                )
 
-            # Not all regular, but all same offsets?
-            # Optimization: https://github.com/scikit-hep/awkward-1.0/issues/442
-            elif all_same_offsets(backend, inputs):
-                lencontent, offsets, starts, stops = None, None, None, None
-                nextinputs = []
+        # General list-handling case: the offsets of each list may be different.
+        else:
+            fcns = [
+                find_custom_broadcast(x, behavior) if isinstance(x, Content) else None
+                for x in inputs
+            ]
 
+            # Find first list without custom broadcasting which will define the broadcast offsets
+            # Don't consider RegularArray (handle case of 1-sized regular broadcasting)
+            # Do this to prioritise non-custom broadcasting
+            first = None
+
+            for x, fcn in zip(inputs, fcns):
+                if (
+                    isinstance(x, listtypes)
+                    and not isinstance(x, RegularArray)
+                    and fcn is None
+                ):
+                    first = x
+                    break
+
+            # Did we fail to find a list without custom broadcasting?
+            secondround = False
+            # If we failed to find an irregular, non-custom broadcasting list,
+            # continue search for *any* list.
+            if first is None:
+                secondround = True
                 for x in inputs:
-                    if isinstance(x, ListOffsetArray):
-                        offsets = x.offsets
-                        lencontent = offsets[-1]
-                        nextinputs.append(x.content[:lencontent])
+                    if isinstance(x, listtypes) and not isinstance(x, RegularArray):
+                        first = x
+                        break
 
-                    elif isinstance(x, ListArray):
-                        starts, stops = x.starts, x.stops
-                        if starts.length == 0 or stops.length == 0:
-                            nextinputs.append(x.content[:0])
-                        else:
-                            lencontent = backend.index_nplike.max(stops)
-                            nextinputs.append(x.content[:lencontent])
+            offsets = first._compact_offsets64(True)
+
+            nextinputs = []
+            for x, fcn in zip(inputs, fcns):
+                if callable(fcn) and not secondround:
+                    nextinputs.append(fcn(x, offsets))
+                elif isinstance(x, listtypes):
+                    nextinputs.append(x._broadcast_tooffsets64(offsets).content)
+
+                # Handle implicit left-broadcasting (non-NumPy-like broadcasting).
+                elif options["left_broadcast"] and isinstance(x, Content):
+                    nextinputs.append(
+                        RegularArray(x, 1, x.length)
+                        ._broadcast_tooffsets64(offsets)
+                        .content
+                    )
+                else:
+                    nextinputs.append(x)
 
+            outcontent = apply_step(
+                backend,
+                nextinputs,
+                action,
+                depth + 1,
+                copy.copy(depth_context),
+                lateral_context,
+                behavior,
+                options,
+            )
+            assert isinstance(outcontent, tuple)
+            parameters = parameters_factory(len(outcontent))
+
+            return tuple(
+                ListOffsetArray(offsets, x, parameters=p)
+                for x, p in zip(outcontent, parameters)
+            )
+
+    def broadcast_any_option():
+        if backend.nplike.known_data:
+            mask = None
+            for x in contents:
+                if x.is_option:
+                    m = x.mask_as_bool(valid_when=False)
+                    if mask is None:
+                        mask = m
                     else:
-                        nextinputs.append(x)
+                        mask = backend.index_nplike.logical_or(mask, m, maybe_out=mask)
 
-                outcontent = apply_step(
-                    backend,
-                    nextinputs,
-                    action,
-                    depth + 1,
-                    copy.copy(depth_context),
-                    lateral_context,
-                    behavior,
-                    options,
-                )
-                assert isinstance(outcontent, tuple)
-                parameters = parameters_factory(len(outcontent))
+            nextmask = Index8(mask.view(np.int8))
+            index = backend.index_nplike.full(mask.shape[0], -1, dtype=np.int64)
+            index[~mask] = backend.index_nplike.arange(
+                mask.shape[0] - backend.index_nplike.count_nonzero(mask),
+                dtype=np.int64,
+            )
+            index = Index64(index)
+            if any(not x.is_option for x in contents):
+                nextindex = backend.index_nplike.arange(mask.shape[0], dtype=np.int64)
+                nextindex[mask] = -1
+                nextindex = Index64(nextindex)
 
-                if isinstance(offsets, Index):
-                    return tuple(
-                        ListOffsetArray(offsets, x, parameters=p).to_ListOffsetArray64(
-                            False
-                        )
-                        for x, p in zip(outcontent, parameters)
-                    )
-                elif isinstance(starts, Index) and isinstance(stops, Index):
-                    return tuple(
-                        ListArray(starts, stops, x, parameters=p).to_ListOffsetArray64(
-                            False
-                        )
-                        for x, p in zip(outcontent, parameters)
+            nextinputs = []
+            for x in inputs:
+                if isinstance(x, optiontypes):
+                    nextinputs.append(x.project(nextmask))
+                elif isinstance(x, Content):
+                    nextinputs.append(
+                        IndexedOptionArray(nextindex, x).project(nextmask)
                     )
                 else:
-                    raise ak._errors.wrap_error(
-                        AssertionError(
-                            "unexpected offsets, starts: {}, {}".format(
-                                type(offsets), type(starts)
-                            )
-                        )
-                    )
+                    nextinputs.append(x)
 
-            # General list-handling case: the offsets of each list may be different.
-            else:
-                fcns = [
-                    find_custom_broadcast(x, behavior)
-                    if isinstance(x, Content)
-                    else None
-                    for x in inputs
-                ]
-
-                # Find first list without custom broadcasting which will define the broadcast offsets
-                # Don't consider RegularArray (handle case of 1-sized regular broadcasting)
-                # Do this to prioritise non-custom broadcasting
-                first = None
-
-                for x, fcn in zip(inputs, fcns):
-                    if (
-                        isinstance(x, listtypes)
-                        and not isinstance(x, RegularArray)
-                        and fcn is None
-                    ):
-                        first = x
-                        break
+        else:
+            index = None
+            nextinputs = []
+            for x in inputs:
+                if isinstance(x, optiontypes):
+                    x._touch_data(recursive=False)
+                    index = Index64(
+                        backend.index_nplike.empty(x.length, dtype=np.int64)
+                    )
+                    nextinputs.append(x.content)
+                else:
+                    nextinputs.append(x)
+            assert index is not None
+        outcontent = apply_step(
+            backend,
+            nextinputs,
+            action,
+            depth,
+            copy.copy(depth_context),
+            lateral_context,
+            behavior,
+            options,
+        )
+        assert isinstance(outcontent, tuple)
+        parameters = parameters_factory(len(outcontent))
+        return tuple(
+            IndexedOptionArray.simplified(index, x, parameters=p)
+            for x, p in zip(outcontent, parameters)
+        )
 
-                # Did we fail to find a list without custom broadcasting?
-                secondround = False
-                # If we failed to find an irregular, non-custom broadcasting list,
-                # continue search for *any* list.
-                if first is None:
-                    secondround = True
-                    for x in inputs:
-                        if isinstance(x, listtypes) and not isinstance(x, RegularArray):
-                            first = x
-                            break
+    def broadcast_any_union():
+        if not backend.nplike.known_data:
+            # assert False
+            union_num_contents, length = [], None
+            for x in contents:
+                if x.is_union:
+                    x._touch_data(recursive=False)
+                    union_num_contents.append(len(x.contents))
+                    if length is None:
+                        length = x.tags.data.shape[0]
+            assert length is not unknown_length
 
-                offsets = first._compact_offsets64(True)
+            all_combos = list(
+                itertools.product(*[range(x) for x in union_num_contents])
+            )
 
+            tags = backend.index_nplike.empty(length, dtype=np.int8)
+            index = backend.index_nplike.empty(length, dtype=np.int64)
+            numoutputs, outcontents = None, []
+            for combo in all_combos:
                 nextinputs = []
-                for x, fcn in zip(inputs, fcns):
-                    if callable(fcn) and not secondround:
-                        nextinputs.append(fcn(x, offsets))
-                    elif isinstance(x, listtypes):
-                        nextinputs.append(x._broadcast_tooffsets64(offsets).content)
-
-                    # Handle implicit left-broadcasting (non-NumPy-like broadcasting).
-                    elif options["left_broadcast"] and isinstance(x, Content):
-                        nextinputs.append(
-                            RegularArray(x, 1, x.length)
-                            ._broadcast_tooffsets64(offsets)
-                            .content
-                        )
+                i = 0
+                for x in inputs:
+                    if isinstance(x, UnionArray):
+                        nextinputs.append(x._contents[combo[i]])
+                        i += 1
                     else:
                         nextinputs.append(x)
 
-                outcontent = apply_step(
-                    backend,
-                    nextinputs,
-                    action,
-                    depth + 1,
-                    copy.copy(depth_context),
-                    lateral_context,
-                    behavior,
-                    options,
-                )
-                assert isinstance(outcontent, tuple)
-                parameters = parameters_factory(len(outcontent))
-
-                return tuple(
-                    ListOffsetArray(offsets, x, parameters=p)
-                    for x, p in zip(outcontent, parameters)
+                outcontents.append(
+                    apply_step(
+                        backend,
+                        nextinputs,
+                        action,
+                        depth,
+                        copy.copy(depth_context),
+                        lateral_context,
+                        behavior,
+                        options,
+                    )
                 )
+                assert isinstance(outcontents[-1], tuple)
+                if numoutputs is None:
+                    numoutputs = outcontents[-1].length
+                else:
+                    assert (
+                        numoutputs is unknown_length
+                        or outcontents[-1].length is unknown_length
+                    ) or numoutputs == outcontents[-1].length
 
-        # Any RecordArrays?
-        elif any(isinstance(x, RecordArray) for x in inputs):
-            if not options["allow_records"]:
-                raise ak._errors.wrap_error(
-                    ValueError(f"cannot broadcast records {in_function(options)}")
-                )
+            assert numoutputs is not None
 
-            fields, length, istuple = unset, unset, unset
-            for x in inputs:
-                if isinstance(x, RecordArray):
-                    if fields is unset:
-                        fields = x.fields
-                    elif set(fields) != set(x.fields):
-                        raise ak._errors.wrap_error(
-                            ValueError(
-                                "cannot broadcast records because fields don't "
-                                "match{}:\n    {}\n    {}".format(
-                                    in_function(options),
-                                    ", ".join(sorted(fields)),
-                                    ", ".join(sorted(x.fields)),
-                                )
-                            )
-                        )
-                    if length is unset:
-                        length = x.length
-                    elif length != x.length:
-                        raise ak._errors.wrap_error(
-                            ValueError(
-                                "cannot broadcast RecordArray of length {} "
-                                "with RecordArray of length {}{}".format(
-                                    length, x.length, in_function(options)
-                                )
+        else:
+            union_tags, union_num_contents, length = [], [], None
+            for x in contents:
+                if x.is_union:
+                    tags = x.tags.raw(backend.index_nplike)
+                    union_tags.append(tags)
+                    union_num_contents.append(len(x.contents))
+                    if tags.shape[0] is unknown_length:
+                        continue
+
+                    if length is None:
+                        length = tags.shape[0]
+                    elif length != tags.shape[0]:
+                        raise ValueError(
+                            "cannot broadcast UnionArray of length {} "
+                            "with UnionArray of length {}{}".format(
+                                length,
+                                tags.shape[0],
+                                in_function(options),
                             )
                         )
-                    # Records win over tuples
-                    if istuple is unset or not x.is_tuple:
-                        istuple = False
+            assert length is not unknown_length
+
+            # Stack all union tags
+            combos = backend.index_nplike.stack(union_tags, axis=-1)
+            # Build array of indices (c1, c2, c3, ..., cn) of contents in
+            # (union 1, union 2, union 3, ..., union n)
+            all_combos = backend.index_nplike.asarray(
+                list(itertools.product(*[range(x) for x in union_num_contents]))
+            )
 
-            outcontents, numoutputs = [], None
-            for field in fields:
+            tags = backend.index_nplike.empty(length, dtype=np.int8)
+            index = backend.index_nplike.empty(length, dtype=np.int64)
+            numoutputs, outcontents = None, []
+            for tag, combo in enumerate(all_combos):
+                mask = backend.index_nplike.all(combos == combo, axis=-1)
+                tags[mask] = tag
+                index[mask] = backend.index_nplike.arange(
+                    backend.index_nplike.count_nonzero(mask), dtype=np.int64
+                )
+                nextinputs = []
+                i = 0
+                for x in inputs:
+                    if isinstance(x, UnionArray):
+                        nextinputs.append(x[mask].project(combo[i]))
+                        i += 1
+                    elif isinstance(x, Content):
+                        nextinputs.append(x[mask])
+                    else:
+                        nextinputs.append(x)
                 outcontents.append(
                     apply_step(
                         backend,
-                        [x[field] if isinstance(x, RecordArray) else x for x in inputs],
+                        nextinputs,
                         action,
                         depth,
                         copy.copy(depth_context),
                         lateral_context,
                         behavior,
                         options,
                     )
                 )
                 assert isinstance(outcontents[-1], tuple)
-                if numoutputs is not None:
+                if numoutputs is None:
+                    numoutputs = len(outcontents[-1])
+                else:
                     assert numoutputs == len(outcontents[-1])
-                numoutputs = len(outcontents[-1])
 
-            return tuple(
-                RecordArray(
-                    [x[i] for x in outcontents],
-                    None if istuple else fields,
-                    length,
-                    parameters=p,
-                )
-                for i, p in enumerate(parameters_factory(numoutputs))
+            assert numoutputs is not None
+
+        parameters = parameters_factory(numoutputs)
+        return tuple(
+            UnionArray.simplified(
+                Index8(tags),
+                Index64(index),
+                [x[i] for x in outcontents],
+                parameters=p,
             )
+            for i, p in enumerate(parameters)
+        )
+
+    def broadcast_any_indexed():
+        nextinputs = [x.project() if isinstance(x, IndexedArray) else x for x in inputs]
+        return apply_step(
+            backend,
+            nextinputs,
+            action,
+            depth,
+            copy.copy(depth_context),
+            lateral_context,
+            behavior,
+            options,
+        )
+
+    def broadcast_any_nd_numpy():
+        nextinputs = [
+            x.to_RegularArray() if isinstance(x, NumpyArray) else x for x in inputs
+        ]
+        return apply_step(
+            backend,
+            nextinputs,
+            action,
+            depth,
+            copy.copy(depth_context),
+            lateral_context,
+            behavior,
+            options,
+        )
+
+    def broadcast_any_unknown():
+        nextinputs = [
+            x.to_NumpyArray(np.float64, backend) if isinstance(x, EmptyArray) else x
+            for x in inputs
+        ]
+        return apply_step(
+            backend,
+            nextinputs,
+            action,
+            depth,
+            copy.copy(depth_context),
+            lateral_context,
+            behavior,
+            options,
+        )
+
+    def continuation():
+        # Any EmptyArrays?
+        if any(x.is_unknown for x in contents):
+            return broadcast_any_unknown()
+
+        # Any NumpyArrays with ndim != 1?
+        elif any(x.is_numpy and x.purelist_depth != 1 for x in contents):
+            return broadcast_any_nd_numpy()
+
+        # Any IndexedArrays?
+        elif any((x.is_indexed and not x.is_option) for x in contents):
+            return broadcast_any_indexed()
+
+        # Any UnionArrays?
+        elif any(x.is_union for x in contents):
+            return broadcast_any_union()
+
+        # Any option-types?
+        elif any(x.is_option for x in contents):
+            return broadcast_any_option()
+
+        # Any list-types?
+        elif any(x.is_list for x in contents):
+            return broadcast_any_list()
+
+        # Any RecordArrays?
+        elif any(x.is_record for x in contents):
+            return broadcast_any_record()
 
         else:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "cannot broadcast: {}{}".format(
-                        ", ".join(repr(type(x)) for x in inputs), in_function(options)
-                    )
+            raise ValueError(
+                "cannot broadcast: {}{}".format(
+                    ", ".join(repr(type(x)) for x in inputs), in_function(options)
                 )
             )
 
     result = action(
         inputs,
         depth=depth,
         depth_context=depth_context,
@@ -1035,15 +1037,15 @@
     )
 
     if isinstance(result, tuple) and all(isinstance(x, Content) for x in result):
         return result
     elif result is None:
         return continuation()
     else:
-        raise ak._errors.wrap_error(AssertionError(result))
+        raise AssertionError(result)
 
 
 def broadcast_and_apply(
     inputs,
     action,
     behavior,
     depth_context=None,
```

### Comparing `awkward-2.1.1/src/awkward/_do.py` & `awkward-2.1.2/src/awkward/_do.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
-from collections.abc import Mapping, MutableMapping, Sequence
+from collections.abc import Mapping, MutableMapping
 from numbers import Integral
 
 import awkward as ak
 from awkward._backends import Backend
 from awkward._nplikes.numpylike import NumpyMetadata
+from awkward._typing import Any, AxisMaybeNone, Literal
 from awkward.contents.content import ActionType, Content
 from awkward.forms import form
 from awkward.record import Record
-from awkward.typing import Any, AxisMaybeNone, Literal
 
 np = NumpyMetadata.instance()
 
 
 def recursively_apply(
     layout: Content | Record,
     action: ActionType,
@@ -79,17 +79,15 @@
     byteorder: Literal["<", ">"] = "<",
 ) -> tuple[form.Form, int, Mapping[str, Any]]:
     if container is None:
         container = {}
     if backend is None:
         backend = content._backend
     if not backend.nplike.known_data:
-        raise ak._errors.wrap_error(
-            TypeError("cannot call 'to_buffers' on an array without concrete data")
-        )
+        raise TypeError("cannot call 'to_buffers' on an array without concrete data")
 
     if isinstance(buffer_key, str):
 
         def getkey(layout, form, attribute):
             return buffer_key.format(form_key=form.form_key, attribute=attribute)
 
     elif callable(buffer_key):
@@ -99,27 +97,21 @@
                 form_key=form.form_key,
                 attribute=attribute,
                 layout=layout,
                 form=form,
             )
 
     else:
-        raise ak._errors.wrap_error(
-            TypeError(
-                "buffer_key must be a string or a callable, not {}".format(
-                    type(buffer_key)
-                )
-            )
+        raise TypeError(
+            f"buffer_key must be a string or a callable, not {type(buffer_key)}"
         )
 
     if form_key is None:
-        raise ak._errors.wrap_error(
-            TypeError(
-                "a 'form_key' must be supplied, to match Form elements to buffers in the 'container'"
-            )
+        raise TypeError(
+            "a 'form_key' must be supplied, to match Form elements to buffers in the 'container'"
         )
 
     form = content.form_with_key(form_key=form_key, id_start=id_start)
 
     content._to_buffers(form, getkey, container, backend, byteorder)
 
     return form, len(content), container
@@ -134,25 +126,21 @@
     n: Integral,
     replacement: bool = False,
     axis: Integral = 1,
     fields: list[str] | None = None,
     parameters: dict | None = None,
 ):
     if n < 1:
-        raise ak._errors.wrap_error(
-            ValueError("in combinations, 'n' must be at least 1")
-        )
+        raise ValueError("in combinations, 'n' must be at least 1")
 
     recordlookup = None
     if fields is not None:
         recordlookup = fields
         if len(recordlookup) != n:
-            raise ak._errors.wrap_error(
-                ValueError("if provided, the length of 'fields' must be 'n'")
-            )
+            raise ValueError("if provided, the length of 'fields' must be 'n'")
     return layout._combinations(n, replacement, recordlookup, parameters, axis, 1)
 
 
 def is_unique(layout, axis: Integral | None = None) -> bool:
     negaxis = axis if axis is None else -axis
     starts = ak.index.Index64.zeros(1, nplike=layout._backend.index_nplike)
     parents = ak.index.Index64.zeros(layout.length, nplike=layout._backend.index_nplike)
@@ -162,54 +150,46 @@
 def unique(layout: Content, axis=None):
     if axis == -1 or axis is None:
         negaxis = axis if axis is None else -axis
         if negaxis is not None:
             branch, depth = layout.branch_depth
             if branch:
                 if negaxis <= 0:
-                    raise ak._errors.wrap_error(
-                        np.AxisError(
-                            "cannot use non-negative axis on a nested list structure "
-                            "of variable depth (negative axis counts from the leaves "
-                            "of the tree; non-negative from the root)"
-                        )
+                    raise np.AxisError(
+                        "cannot use non-negative axis on a nested list structure "
+                        "of variable depth (negative axis counts from the leaves "
+                        "of the tree; non-negative from the root)"
                     )
                 if negaxis > depth:
-                    raise ak._errors.wrap_error(
-                        np.AxisError(
-                            "cannot use axis={} on a nested list structure that splits into "
-                            "different depths, the minimum of which is depth={} from the leaves".format(
-                                axis, depth
-                            )
+                    raise np.AxisError(
+                        "cannot use axis={} on a nested list structure that splits into "
+                        "different depths, the minimum of which is depth={} from the leaves".format(
+                            axis, depth
                         )
                     )
             else:
                 if negaxis <= 0:
                     negaxis = negaxis + depth
                 if not (0 < negaxis and negaxis <= depth):
-                    raise ak._errors.wrap_error(
-                        np.AxisError(
-                            "axis={} exceeds the depth of this array ({})".format(
-                                axis, depth
-                            )
+                    raise np.AxisError(
+                        "axis={} exceeds the depth of this array ({})".format(
+                            axis, depth
                         )
                     )
 
         starts = ak.index.Index64.zeros(1, nplike=layout._backend.index_nplike)
         parents = ak.index.Index64.zeros(
             layout.length, nplike=layout._backend.index_nplike
         )
 
         return layout._unique(negaxis, starts, parents, 1)
 
-    raise ak._errors.wrap_error(
-        np.AxisError(
-            "unique expects axis 'None' or '-1', got axis={} that is not supported yet".format(
-                axis
-            )
+    raise np.AxisError(
+        "unique expects axis 'None' or '-1', got axis={} that is not supported yet".format(
+            axis
         )
     )
 
 
 def pad_none(
     layout: Content, length: Integral, axis: Integral, clip: bool = False
 ) -> Content:
@@ -266,41 +246,14 @@
     return layout._num(axis, 0)
 
 
 def mergeable(one: Content, two: Content, mergebool: bool = True) -> bool:
     return one._mergeable_next(two, mergebool=mergebool)
 
 
-def merge_as_union(
-    contents: Sequence[Content], parameters=None
-) -> ak.contents.UnionArray:
-    length = sum([c.length for c in contents])
-    first = contents[0]
-    tags = ak.index.Index8.empty(length, first.backend.index_nplike)
-    index = ak.index.Index64.empty(length, first.backend.index_nplike)
-
-    offset = 0
-    for i, content in enumerate(contents):
-        content._handle_error(
-            content.backend["awkward_UnionArray_filltags_const", tags.dtype.type](
-                tags.data, offset, content.length, i
-            )
-        )
-        content._handle_error(
-            content.backend["awkward_UnionArray_fillindex_count", index.dtype.type](
-                index.data, offset, content.length
-            )
-        )
-        offset += content.length
-
-    return ak.contents.UnionArray.simplified(
-        tags, index, contents, parameters=parameters
-    )
-
-
 def mergemany(contents: list[Content]) -> Content:
     assert len(contents) != 0
     return contents[0]._mergemany(contents[1:])
 
 
 def reduce(
     layout: Content,
@@ -314,18 +267,16 @@
         parts = remove_structure(
             layout, flatten_records=False, drop_nones=False, keepdims=keepdims
         )
 
         if len(parts) > 1:
             # We know that `flatten_records` must fail, so the only other type
             # that can return multiple parts here is the union array
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "cannot use axis=None on an array containing irreducible unions"
-                )
+            raise ValueError(
+                "cannot use axis=None on an array containing irreducible unions"
             )
         elif len(parts) == 0:
             parts = [ak.contents.EmptyArray()]
 
         (layout,) = parts
 
         starts = ak.index.Index64.zeros(1, layout.backend.index_nplike)
@@ -345,38 +296,32 @@
         return next[0]
     else:
         negaxis = -axis
         branch, depth = layout.branch_depth
 
         if branch:
             if negaxis <= 0:
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "cannot use non-negative axis on a nested list structure "
-                        "of variable depth (negative axis counts from the leaves of "
-                        "the tree; non-negative from the root)"
-                    )
+                raise ValueError(
+                    "cannot use non-negative axis on a nested list structure "
+                    "of variable depth (negative axis counts from the leaves of "
+                    "the tree; non-negative from the root)"
                 )
             if negaxis > depth:
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "cannot use axis={} on a nested list structure that splits into "
-                        "different depths, the minimum of which is depth={} "
-                        "from the leaves".format(axis, depth)
-                    )
+                raise ValueError(
+                    "cannot use axis={} on a nested list structure that splits into "
+                    "different depths, the minimum of which is depth={} "
+                    "from the leaves".format(axis, depth)
                 )
         else:
             if negaxis <= 0:
                 negaxis += depth
             if not 0 < negaxis <= depth:
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "axis={} exceeds the depth of the nested list structure "
-                        "(which is {})".format(axis, depth)
-                    )
+                raise ValueError(
+                    "axis={} exceeds the depth of the nested list structure "
+                    "(which is {})".format(axis, depth)
                 )
 
         starts = ak.index.Index64.zeros(1, layout.backend.index_nplike)
         parents = ak.index.Index64.zeros(layout.length, layout.backend.index_nplike)
         shifts = None
         next = layout._reduce_next(
             reducer,
@@ -406,39 +351,33 @@
     ascending: bool = True,
     stable: bool = False,
 ) -> Content:
     negaxis = -axis
     branch, depth = layout.branch_depth
     if branch:
         if negaxis <= 0:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "cannot use non-negative axis on a nested list structure "
-                    "of variable depth (negative axis counts from the leaves "
-                    "of the tree; non-negative from the root)"
-                )
+            raise ValueError(
+                "cannot use non-negative axis on a nested list structure "
+                "of variable depth (negative axis counts from the leaves "
+                "of the tree; non-negative from the root)"
             )
         if negaxis > depth:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "cannot use axis={} on a nested list structure that splits into "
-                    "different depths, the minimum of which is depth={} from the leaves".format(
-                        axis, depth
-                    )
+            raise ValueError(
+                "cannot use axis={} on a nested list structure that splits into "
+                "different depths, the minimum of which is depth={} from the leaves".format(
+                    axis, depth
                 )
             )
     else:
         if negaxis <= 0:
             negaxis = negaxis + depth
         if not 0 < negaxis <= depth:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "axis={} exceeds the depth of the nested list structure "
-                    "(which is {})".format(axis, depth)
-                )
+            raise ValueError(
+                "axis={} exceeds the depth of the nested list structure "
+                "(which is {})".format(axis, depth)
             )
 
     starts = ak.index.Index64.zeros(1, nplike=layout.backend.index_nplike)
     parents = ak.index.Index64.zeros(layout.length, nplike=layout.backend.index_nplike)
     return layout._argsort_next(
         negaxis,
         starts,
@@ -453,37 +392,31 @@
 def sort(
     layout: Content, axis: int = -1, ascending: bool = True, stable: bool = False
 ) -> Content:
     negaxis = -axis
     branch, depth = layout.branch_depth
     if branch:
         if negaxis <= 0:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "cannot use non-negative axis on a nested list structure "
-                    "of variable depth (negative axis counts from the leaves "
-                    "of the tree; non-negative from the root)"
-                )
+            raise ValueError(
+                "cannot use non-negative axis on a nested list structure "
+                "of variable depth (negative axis counts from the leaves "
+                "of the tree; non-negative from the root)"
             )
         if negaxis > depth:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "cannot use axis={} on a nested list structure that splits into "
-                    "different depths, the minimum of which is depth={} from the leaves".format(
-                        axis, depth
-                    )
+            raise ValueError(
+                "cannot use axis={} on a nested list structure that splits into "
+                "different depths, the minimum of which is depth={} from the leaves".format(
+                    axis, depth
                 )
             )
     else:
         if negaxis <= 0:
             negaxis = negaxis + depth
         if not 0 < negaxis <= depth:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "axis={} exceeds the depth of the nested list structure "
-                    "(which is {})".format(axis, depth)
-                )
+            raise ValueError(
+                "axis={} exceeds the depth of the nested list structure "
+                "(which is {})".format(axis, depth)
             )
 
     starts = ak.index.Index64.zeros(1, nplike=layout.backend.index_nplike)
     parents = ak.index.Index64.zeros(layout.length, nplike=layout.backend.index_nplike)
     return layout._sort_next(negaxis, starts, parents, 1, ascending, stable)
```

### Comparing `awkward-2.1.1/src/awkward/_errors.py` & `awkward-2.1.2/src/awkward/_errors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
+import sys
 import threading
 import warnings
 from collections.abc import Mapping, Sequence
 
 from awkward._nplikes.numpylike import NumpyMetadata
+from awkward._typing import TypeVar
 
 np = NumpyMetadata.instance()
 
 
+E = TypeVar("E", bound=Exception)
+
+
 class PartialFunction:
     """Analogue of `functools.partial`, but as a distinct type"""
 
     __slots__ = ("func", "args", "kwargs")
 
     def __init__(self, func, *args, **kwargs):
         self.func = func
@@ -39,17 +44,50 @@
         # Make it strictly non-reenterant. Only one ErrorContext (per thread) is primary.
         if self.primary() is None:
             self._slate.__dict__.clear()
             self._slate.__dict__.update(self._kwargs)
             self._slate.__dict__["__primary_context__"] = self
 
     def __exit__(self, exception_type, exception_value, traceback):
-        # Step out of the way so that another ErrorContext can become primary.
-        if self.primary() is self:
-            self._slate.__dict__.clear()
+        try:
+            # Handle caught exception
+            if exception_type is not None:
+                self.handle_exception(exception_type, exception_value)
+        finally:
+            # Step out of the way so that another ErrorContext can become primary.
+            if self.primary() is self:
+                self._slate.__dict__.clear()
+
+    def handle_exception(self, cls: type[E], exception: E) -> E:
+        if sys.version_info >= (3, 11, 0, "final"):
+            return self.decorate_exception(cls, exception)
+        else:
+            raise self.decorate_exception(cls, exception)
+
+    def decorate_exception(self, cls: type[E], exception: E) -> E:
+        if sys.version_info >= (3, 11, 0, "final"):
+            if issubclass(cls, (NotImplementedError, AssertionError)):
+                exception.add_note(
+                    "\n\nSee if this has been reported at https://github.com/scikit-hep/awkward/issues"
+                )
+            else:
+                exception.add_note(self.note)
+            return exception
+        else:
+            if issubclass(cls, (NotImplementedError, AssertionError)):
+                # Raise modified exception
+                new_exception = cls(
+                    str(exception)
+                    + "\n\nSee if this has been reported at https://github.com/scikit-hep/awkward/issues"
+                )
+                new_exception.__cause__ = exception
+            else:
+                new_exception = cls(self.format_exception(exception))
+                new_exception.__cause__ = exception
+            return new_exception
 
     def format_argument(self, width, value):
         from awkward import contents, highlevel, record
 
         if isinstance(value, contents.Content):
             return self.format_argument(width, highlevel.Array(value))
         elif isinstance(value, record.Record):
@@ -118,14 +156,18 @@
             return f"{type(value).__name__}-instance"
         else:
             return valuestr
 
     def format_exception(self, exception: Exception) -> str:
         raise NotImplementedError
 
+    @property
+    def note(self) -> str:
+        raise NotImplementedError
+
 
 class OperationErrorContext(ErrorContext):
     _width = 80 - 8
 
     def __init__(self, name, arguments):
         from awkward._backends import NumpyBackend, backend_of
 
@@ -165,27 +207,30 @@
     def arguments(self):
         out = self._kwargs["arguments"]
         if isinstance(out, PartialFunction):
             out = self._kwargs["arguments"] = out()
         return out
 
     def format_exception(self, exception):
+        return f"{exception}\n{self.note}"
+
+    @property
+    def note(self) -> str:
         arguments = []
         for name, valuestr in self.arguments.items():
             if isinstance(name, str):
                 arguments.append(f"\n        {name} = {valuestr}")
             else:
                 arguments.append(f"\n        {valuestr}")
 
         extra_line = "" if len(arguments) == 0 else "\n    "
-        return f"""while calling
+        return f"""
+This error occurred while calling
 
-    {self.name}({"".join(arguments)}{extra_line})
-
-Error details: {str(exception)}"""
+    {self.name}({"".join(arguments)}{extra_line})"""
 
 
 class SlicingErrorContext(ErrorContext):
     _width = 80 - 4
 
     def __init__(self, array, where):
         from awkward._backends import NumpyBackend, backend_of
@@ -219,28 +264,26 @@
     def where(self):
         out = self._kwargs["where"]
         if isinstance(out, PartialFunction):
             out = self._kwargs["where"] = out()
         return out
 
     def format_exception(self, exception):
-        if isinstance(exception, str):
-            message = exception
-        else:
-            message = f"Error details: {str(exception)}"
+        return f"{exception}\n{self.note}"
 
-        return f"""while attempting to slice
+    @property
+    def note(self) -> str:
+        return f"""
+This error occurred while attempting to slice
 
     {self.array}
 
 with
 
-    {self.where}
-
-{message}"""
+    {self.where}"""
 
     @staticmethod
     def format_slice(x):
         from awkward import contents, highlevel, index, record
 
         if isinstance(x, slice):
             if x.step is None:
@@ -273,68 +316,23 @@
             except Exception:
                 return x._repr("    ", "", "")
 
         else:
             return repr(x)
 
 
-def wrap_error(
-    exception: Exception | type[Exception], error_context: ErrorContext = None
-) -> Exception:
-    """
-    Args:
-        exception: exception object, or exception type to instantiate
-        error_context: context in which error was raised
-
-    Wrap the given exception, instantiating it if needed, to ensure meaningful error messages.
-    """
-    if isinstance(exception, type) and issubclass(exception, Exception):
-        try:
-            exception = exception()
-        except Exception:
-            return exception
-
-    if isinstance(exception, (NotImplementedError, AssertionError)):
-        return type(exception)(
-            str(exception)
-            + "\n\nSee if this has been reported at https://github.com/scikit-hep/awkward-1.0/issues"
-        )
-
-    if error_context is None:
-        error_context = ErrorContext.primary()
-
-    if isinstance(error_context, ErrorContext):
-        # Note: returns an error for the caller to raise!
-        return type(exception)(error_context.format_exception(exception))
-    else:
-        # Note: returns an error for the caller to raise!
-        return exception
-
-
 def index_error(subarray, slicer, details: str = None) -> IndexError:
-    detailsstr = ""
+    message = ""
     if details is not None:
-        detailsstr = f"""
+        message = f": {details}"
 
-Error details: {details}."""
-
-    error_context = ErrorContext.primary()
-    if not isinstance(error_context, SlicingErrorContext):
-        # Note: returns an error for the caller to raise!
-        return IndexError(
-            f"cannot slice {type(subarray).__name__} with {SlicingErrorContext.format_slice(slicer)}{detailsstr}"
-        )
-
-    else:
-        # Note: returns an error for the caller to raise!
-        return IndexError(
-            error_context.format_exception(
-                f"at inner {type(subarray).__name__} of length {subarray.length}, using sub-slice {error_context.format_slice(slicer)}.{detailsstr}"
-            )
-        )
+    # Note: returns an error for the caller to raise!
+    return IndexError(
+        f"cannot slice {type(subarray).__name__} (of length {subarray.length}) with {SlicingErrorContext.format_slice(slicer)}{message}"
+    )
 
 
 ###############################################################################
 
 # Enable warnings for the Awkward package
 warnings.filterwarnings("default", module="awkward.*")
```

### Comparing `awkward-2.1.1/src/awkward/_kernels.py` & `awkward-2.1.2/src/awkward/_kernels.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from abc import abstractmethod
 from typing import Any, Callable
 
 import awkward as ak
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
-from awkward.typing import Protocol, TypeAlias
+from awkward._typing import Protocol, TypeAlias
 
 KernelKeyType: TypeAlias = tuple  # Tuple[str, Unpack[Tuple[metadata.dtype, ...]]]
 
 
 metadata = NumpyMetadata.instance()
 
 
@@ -29,15 +29,15 @@
     @property
     @abstractmethod
     def key(self) -> KernelKeyType:
         ...
 
     @abstractmethod
     def __call__(self, *args) -> KernelError | None:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
 
 class BaseKernel(Kernel):
     _impl: Callable[..., Any]
     _key: KernelKeyType
 
     def __init__(self, impl: Callable[..., Any], key: KernelKeyType):
@@ -73,16 +73,16 @@
                     return ctypes.cast(x.ctypes.data, t)
                 else:
                     return x
             # Or, do we have a ctypes type
             elif hasattr(x, "_b_base_"):
                 return ctypes.cast(x, t)
             else:
-                raise ak._errors.wrap_error(
-                    AssertionError("CuPy buffers shouldn't be passed to Numpy Kernels.")
+                raise AssertionError(
+                    "CuPy buffers shouldn't be passed to Numpy Kernels."
                 )
         else:
             return x
 
     def __call__(self, *args) -> None:
         assert len(args) == len(self._impl.argtypes)
```

### Comparing `awkward-2.1.1/src/awkward/_layout.py` & `awkward-2.1.2/src/awkward/_layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 from collections.abc import Mapping
 
 from awkward._backends import NumpyBackend
 from awkward._behavior import behavior_of
-from awkward._errors import wrap_error
 from awkward._nplikes import nplike_of
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
@@ -48,17 +47,15 @@
     from awkward.index import Index8, Index64
 
     # overshadows global NumPy import for nplike-safety
     nplike = nplike_of(array)
 
     def recurse(array, mask=None):
         if Jax.is_tracer(array):
-            raise wrap_error(
-                TypeError("Jax tracers cannot be used with `ak.from_arraylib`")
-            )
+            raise TypeError("Jax tracers cannot be used with `ak.from_arraylib`")
 
         if regulararray and len(array.shape) > 1:
             new_shape = (-1,) + array.shape[2:]
             return RegularArray(
                 recurse(nplike.reshape(array, new_shape), mask),
                 array.shape[1],
                 array.shape[0],
@@ -126,17 +123,15 @@
                 return attach(data.to_RegularArray())
 
         else:
             # NumPy's MaskedArray is a ByteMaskedArray with valid_when=False
             return ByteMaskedArray(Index8(mask), data, valid_when=False)
 
     if array.dtype == np.dtype("O"):
-        raise wrap_error(
-            TypeError("Awkward Array does not support arrays with object dtypes.")
-        )
+        raise TypeError("Awkward Array does not support arrays with object dtypes.")
 
     if isinstance(array, numpy.ma.MaskedArray):
         mask = numpy.ma.getmask(array)
         array = numpy.ma.getdata(array)
         if isinstance(mask, np.ndarray) and len(mask.shape) > 1:
             regulararray = True
             mask = mask.reshape(-1)
@@ -156,17 +151,15 @@
 
 
 def maybe_posaxis(layout, axis, depth):
     from awkward.record import Record
 
     if isinstance(layout, Record):
         if axis == 0:
-            raise wrap_error(
-                np.AxisError("Record type at axis=0 is a scalar, not an array")
-            )
+            raise np.AxisError("Record type at axis=0 is a scalar, not an array")
         return maybe_posaxis(layout._array, axis, depth)
 
     if axis >= 0:
         return axis
 
     else:
         is_branching, additional_depth = layout.branch_depth
```

### Comparing `awkward-2.1.1/src/awkward/_lookup.py` & `awkward-2.1.2/src/awkward/_lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,17 +64,15 @@
     elif isinstance(layout, ak.record.Record):
         return RecordLookup.tolookup(layout, positions)
 
     elif isinstance(layout, ak.contents.UnionArray):
         return UnionLookup.tolookup(layout, positions)
 
     else:
-        raise ak._errors.wrap_error(
-            AssertionError(f"unrecognized Content: {type(layout)}")
-        )
+        raise AssertionError(f"unrecognized Content: {type(layout)}")
 
 
 class ContentLookup:
     pass
 
 
 class NumpyLookup(ContentLookup):
```

### Comparing `awkward-2.1.1/src/awkward/_prettyprint.py` & `awkward-2.1.2/src/awkward/_prettyprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,8 +312,8 @@
             elif data.is_tuple:
                 out[i] = val + ")"
             else:
                 out[i] = val + "}"
         return "\n".join(out)
 
     else:
-        raise ak._errors.wrap_error(AssertionError(type(data)))
+        raise AssertionError(type(data))
```

### Comparing `awkward-2.1.1/src/awkward/_reducers.py` & `awkward-2.1.2/src/awkward/_reducers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from abc import ABC, abstractmethod
 from typing import Any as AnyType
 
 import awkward as ak
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
-from awkward.typing import Final
+from awkward._typing import Final
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 DTypeLike = AnyType
 
 
@@ -55,19 +55,19 @@
             type = np.float64
         if dtype == np.complex64:
             type = np.float32
         return type
 
     @abstractmethod
     def identity_for(self, dtype: DTypeLike | None):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @abstractmethod
     def apply(self, array, parents, outlength: int):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
 
 class ArgMin(Reducer):
     name: Final = "argmin"
     needs_position: Final = True
     preferred_dtype: Final = np.int64
 
@@ -252,17 +252,15 @@
     name: Final = "sum"
     preferred_dtype: Final = np.float64
     needs_position: Final = False
 
     def apply(self, array, parents, outlength):
         assert isinstance(array, ak.contents.NumpyArray)
         if array.dtype.kind == "M":
-            raise ak._errors.wrap_error(
-                ValueError(f"cannot compute the sum (ak.sum) of {array.dtype!r}")
-            )
+            raise ValueError(f"cannot compute the sum (ak.sum) of {array.dtype!r}")
         else:
             dtype = self.maybe_other_type(array.dtype)
         result = array.backend.nplike.empty(
             self.maybe_double_length(array.dtype.type, outlength),
             dtype=self.return_dtype(dtype),
         )
 
@@ -296,15 +294,15 @@
                         array.data,
                         parents.data,
                         parents.length,
                         outlength,
                     )
                 )
             else:
-                raise ak._errors.wrap_error(NotImplementedError)
+                raise NotImplementedError
         elif array.dtype.type in (np.complex128, np.complex64):
             assert parents.nplike is array.backend.index_nplike
             array._handle_error(
                 array.backend[
                     "awkward_reduce_sum_complex",
                     np.float64 if array.dtype.type == np.complex128 else np.float32,
                     np.float64 if array.dtype.type == np.complex128 else np.float32,
@@ -357,17 +355,15 @@
     name: Final = "prod"
     preferred_dtype: Final = np.int64
     needs_position: Final = False
 
     def apply(self, array, parents, outlength):
         assert isinstance(array, ak.contents.NumpyArray)
         if array.dtype.kind.upper() == "M":
-            raise ak._errors.wrap_error(
-                ValueError(f"cannot compute the product (ak.prod) of {array.dtype!r}")
-            )
+            raise ValueError(f"cannot compute the product (ak.prod) of {array.dtype!r}")
         if array.dtype == np.bool_:
             result = array.backend.nplike.empty(
                 self.maybe_double_length(array.dtype.type, outlength),
                 dtype=np.dtype(np.bool_),
             )
             assert parents.nplike is array.backend.index_nplike
             array._handle_error(
```

### Comparing `awkward-2.1.1/src/awkward/_regularize.py` & `awkward-2.1.2/src/awkward/_regularize.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import numbers
 import os
 from collections.abc import Iterable, Sequence, Sized
 
 from awkward._nplikes.numpylike import NumpyMetadata
-from awkward.typing import AxisMaybeNone, SupportsInt
+from awkward._typing import AxisMaybeNone, SupportsInt
 
 np = NumpyMetadata.instance()
 
 
 def is_file_path(x) -> bool:
     try:
         return os.path.isfile(x)
```

### Comparing `awkward-2.1.1/src/awkward/_slicing.py` & `awkward-2.1.2/src/awkward/_slicing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import operator
 
 import awkward as ak
 from awkward._backends import Backend
-from awkward._errors import wrap_error
 from awkward._nplikes import to_nplike
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._regularize import is_array_like, is_integer_like, is_sized_iterable
-from awkward.typing import TYPE_CHECKING, Sequence, TypeAlias, TypeVar
+from awkward._typing import TYPE_CHECKING, Sequence, TypeAlias, TypeVar
 
 if TYPE_CHECKING:
     from awkward._nplikes.numpylike import ArrayLike
     from awkward.contents.content import Content
 
 np = NumpyMetadata.instance()
 
 
 SliceItem: TypeAlias = "int | slice | str | None | Ellipsis | ArrayLike | Content"
 
 
 def normalize_slice_item(item, *, backend: Backend):
     if backend.index_nplike.is_own_array(item):
         if item.ndim != 0:
-            raise wrap_error(
-                ValueError(
-                    f"slice items must be 0D arrays or Python integers, not {item!r}"
-                )
+            raise ValueError(
+                f"slice items must be 0D arrays or Python integers, not {item!r}"
             )
         else:
             return item
     else:
         return operator.index(item)
 
 
@@ -127,20 +124,18 @@
         else:
             # this includes integers (which broadcast to arrays)
             broadcastable_index.append(len(broadcastable))
             broadcastable.append(item)
 
     # Now ensure that we don't have mixed Awkward-NumPy style indexing
     if n_awkward_contents > 1 or (n_awkward_contents == 1 and len(broadcastable) != 0):
-        raise wrap_error(
-            ValueError(
-                "cannot mix Awkward slicing (using an array with missing or variable-length lists in the slice) with "
-                "NumPy advanced slicing (using more than one broadcastable array or integer in the slice), "
-                "though you can perform multiple slices "
-            )
+        raise ValueError(
+            "cannot mix Awkward slicing (using an array with missing or variable-length lists in the slice) with "
+            "NumPy advanced slicing (using more than one broadcastable array or integer in the slice), "
+            "though you can perform multiple slices "
         )
 
     # Then broadcast the index items
     nplike = backend.index_nplike
     broadcasted = nplike.broadcast_arrays(*broadcastable)
 
     # And re-assemble the index with the broadcasted items
@@ -169,19 +164,17 @@
                 current = ak.index.Index64(nplike.nonzero(x)[0])
                 prepared.append(current)
                 prepared[-1].metadata["shape"] = current.data.shape
             else:
                 for w in nplike.nonzero(x):
                     prepared.append(ak.index.Index64(w))
         else:
-            raise wrap_error(
-                TypeError(
-                    "array slice must be an array of integers or booleans, not\n\n    {}".format(
-                        repr(x).replace("\n", "\n    ")
-                    )
+            raise TypeError(
+                "array slice must be an array of integers or booleans, not\n\n    {}".format(
+                    repr(x).replace("\n", "\n    ")
                 )
             )
 
     # Finally, ensure that we don't have an unsupported mode of NumPy indexing
     # We do this here, rather than above the broadcast, because unlike the
     # Awkward-NumPy case, we don't want to treat integer indices as "advanced"
     # indices, i.e. `0, :, 0` should not trigger this case, but `0, :, [0]` should
@@ -195,31 +188,27 @@
     # Then find a separator
     for item in it:
         if (item is np.newaxis) or (item is Ellipsis) or isinstance(item, slice):
             break
     # Now error if we find another array
     for item in it:
         if isinstance(item, ak.index.Index):
-            raise wrap_error(
-                ValueError(
-                    "NumPy advanced indexing with array indices separated by None "
-                    "(np.newaxis), Ellipsis, or slice are not permitted with Awkward Arrays"
-                )
+            raise ValueError(
+                "NumPy advanced indexing with array indices separated by None "
+                "(np.newaxis), Ellipsis, or slice are not permitted with Awkward Arrays"
             )
     return tuple(prepared)
 
 
 def normalize_integer_like(x) -> int | ArrayLike:
     if is_array_like(x):
         if np.issubdtype(x.dtype, np.integer) and x.ndim == 0:
             return x
         else:
-            raise wrap_error(
-                TypeError("only 0D integer arrays are considered integral")
-            )
+            raise TypeError("only 0D integer arrays are considered integral")
     else:
         return int(x)
 
 
 def normalise_item(item, backend: Backend) -> SliceItem:
     """
     Args:
@@ -287,18 +276,16 @@
     elif is_sized_iterable(item):
         # Do we have an array
         nplike = ak._nplikes.nplike_of(item, default=None)
         # We can end up with non-array objects associated with an nplike
         if nplike is not None and nplike.is_own_array(item):
             # Is it a scalar, not array?
             if len(item.shape) == 0:
-                raise wrap_error(
-                    AssertionError(
-                        "scalar arrays should be handled by integer-like indexing"
-                    )
+                raise AssertionError(
+                    "scalar arrays should be handled by integer-like indexing"
                 )
             else:
                 layout = ak.operations.ak_to_layout._impl(
                     item, allow_record=False, allow_other=True, regulararray=False
                 )
                 return normalise_item(layout, backend)
 
@@ -314,22 +301,20 @@
         else:
             layout = ak.operations.ak_to_layout._impl(
                 item, allow_record=False, allow_other=True, regulararray=False
             )
             return normalise_item(layout, backend)
 
     else:
-        raise wrap_error(
-            TypeError(
-                "only integers, slices (`:`), ellipsis (`...`), np.newaxis (`None`), "
-                "integer/boolean arrays (possibly with variable-length nested "
-                "lists or missing values), field name (str) or names (non-tuple "
-                "iterable of str) are valid indices for slicing, not\n\n    "
-                + repr(item).replace("\n", "\n    ")
-            )
+        raise TypeError(
+            "only integers, slices (`:`), ellipsis (`...`), np.newaxis (`None`), "
+            "integer/boolean arrays (possibly with variable-length nested "
+            "lists or missing values), field name (str) or names (non-tuple "
+            "iterable of str) are valid indices for slicing, not\n\n    "
+            + repr(item).replace("\n", "\n    ")
         )
 
 
 def normalise_items(where: Sequence, backend: Backend) -> list:
     # First prepare items for broadcasting into like-types
     return [normalise_item(x, backend=backend) for x in where]
 
@@ -343,15 +328,15 @@
             parameters=item.parameters,
         )
 
     elif isinstance(item, ak.contents.NumpyArray) and item.purelist_depth == 1:
         return item
 
     else:
-        raise wrap_error(AssertionError(type(item)))
+        raise AssertionError(type(item))
 
 
 def _normalise_item_nested(item: Content) -> Content:
     if isinstance(item, ak.contents.EmptyArray):
         # policy: unknown -> int
         return _normalise_item_nested(item.to_NumpyArray(np.int64))
 
@@ -468,32 +453,28 @@
         return ak.contents.IndexedOptionArray(
             ak.index.Index64(nextindex, nplike=item.backend.index_nplike),
             nextcontent,
             parameters=item.parameters,
         )
 
     elif isinstance(item, ak.contents.UnionArray):
-        raise wrap_error(
-            TypeError(
-                "irreducible unions (different types at the same level in an array) can't be used as slices"
-            )
+        raise TypeError(
+            "irreducible unions (different types at the same level in an array) can't be used as slices"
         )
 
     elif isinstance(item, ak.contents.RecordArray):
-        raise wrap_error(TypeError("record arrays can't be used as slices"))
+        raise TypeError("record arrays can't be used as slices")
 
     else:
-        raise wrap_error(
-            TypeError(
-                "only integers, slices (`:`), ellipsis (`...`), np.newaxis (`None`), "
-                "integer/boolean arrays (possibly with variable-length nested "
-                "lists or missing values), field name (str) or names (non-tuple "
-                "iterable of str) are valid indices for slicing, not\n\n    "
-                + repr(item).replace("\n", "\n    ")
-            )
+        raise TypeError(
+            "only integers, slices (`:`), ellipsis (`...`), np.newaxis (`None`), "
+            "integer/boolean arrays (possibly with variable-length nested "
+            "lists or missing values), field name (str) or names (non-tuple "
+            "iterable of str) are valid indices for slicing, not\n\n    "
+            + repr(item).replace("\n", "\n    ")
         )
 
 
 def _normalise_item_bool_to_int(item: Content, backend: Backend) -> Content:
     """
     Args:
         item: content to normalise
@@ -546,17 +527,15 @@
         isinstance(item, ListOffsetArray)
         and isinstance(item.content, IndexedOptionArray)
         and isinstance(item.content.content, NumpyArray)
         and np.issubdtype(item.content.content.dtype, np.bool_)
     ):
         if item_backend.nplike.known_data:
             if isinstance(item_backend.nplike, Jax):
-                raise wrap_error(
-                    TypeError("This slice is not supported for JAX differentiation.")
-                )
+                raise TypeError("This slice is not supported for JAX differentiation.")
             # missing values as any integer other than -1 are extremely rare
             isnegative = item.content.index.data < 0
             if item_backend.index_nplike.any(item.content.index.data < -1):
                 safeindex = item.content.index.data.copy()
                 safeindex[isnegative] = -1
             else:
                 safeindex = item.content.index.data
@@ -616,18 +595,16 @@
             ).to_backend(backend)
 
         if isinstance(item.content, NumpyArray) and issubclass(
             item.content.dtype.type, (bool, np.bool_)
         ):
             if item_backend.nplike.known_data:
                 if isinstance(item_backend.nplike, Jax):
-                    raise wrap_error(
-                        TypeError(
-                            "This slice is not supported for JAX differentiation."
-                        )
+                    raise TypeError(
+                        "This slice is not supported for JAX differentiation."
                     )
 
                 # missing values as any integer other than -1 are extremely rare
                 isnegative = item.index.data < 0
                 if item_backend.index_nplike.any(item.index.data < -1):
                     safeindex = item.index.data.copy()
                     safeindex[isnegative] = -1
@@ -677,15 +654,15 @@
             ).to_backend(backend)
 
     elif isinstance(item, NumpyArray):
         assert item.data.shape == (item.length,)
         return item
 
     else:
-        raise wrap_error(AssertionError(type(item)))
+        raise AssertionError(type(item))
 
 
 def getitem_next_array_wrap(
     outcontent: Content, shape: tuple[int], outer_length: int = 0
 ) -> Content:
     for i in range(len(shape))[::-1]:
         length = shape[i - 1] if i > 0 else outer_length
```

### Comparing `awkward-2.1.1/src/awkward/_typetracer.py` & `awkward-2.1.2/src/awkward/_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_util.py` & `awkward-2.1.2/src/awkward/_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import sys
 from collections.abc import Collection
 
 import packaging.version
 
 from awkward._nplikes.numpylike import NumpyMetadata
-from awkward.typing import TypeVar
+from awkward._typing import TypeVar
 
 np = NumpyMetadata.instance()
 
 win = os.name == "nt"
 bits32 = np.iinfo(np.intp).bits == 32
 
 # matches include/awkward/common.h
```

### Comparing `awkward-2.1.1/src/awkward/_v2.py` & `awkward-2.1.2/src/awkward/_v2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
-raise ModuleNotFoundError(  # noqa: AK101
+raise ModuleNotFoundError(
     """The awkward._v2 submodule was provided for early access to awkward>=2, as it developed.
 
 Now that version 2 has been released, awkward._v2 is no longer needed.
 
 If you were an early adopter using
 
     import awkward._v2 as ak
```

### Comparing `awkward-2.1.1/src/awkward/highlevel.py` & `awkward-2.1.2/src/awkward/highlevel.py`

 * *Files 3% similar despite different names*

```diff
@@ -177,14 +177,15 @@
         data,
         *,
         behavior=None,
         with_name=None,
         check_valid=False,
         backend=None,
     ):
+        self._cpp_type = None
         if isinstance(data, ak.contents.Content):
             layout = data
 
         elif isinstance(data, Array):
             layout = data._layout
             behavior = behavior_of(data, behavior=behavior)
 
@@ -194,36 +195,30 @@
             length = None
             for k, v in data.items():
                 fields.append(k)
                 contents.append(Array(v).layout)
                 if length is None:
                     length = contents[-1].length
                 elif length != contents[-1].length:
-                    raise ak._errors.wrap_error(
-                        ValueError(
-                            "dict of arrays in ak.Array constructor must have arrays "
-                            "of equal length ({} vs {})".format(
-                                length, contents[-1].length
-                            )
-                        )
+                    raise ValueError(
+                        "dict of arrays in ak.Array constructor must have arrays "
+                        "of equal length ({} vs {})".format(length, contents[-1].length)
                     )
             layout = ak.contents.RecordArray(contents, fields)
 
         elif isinstance(data, str):
             layout = ak.operations.from_json(data, highlevel=False)
 
         else:
             layout = ak.operations.to_layout(
                 data, allow_record=False, regulararray=False
             )
 
         if not isinstance(layout, ak.contents.Content):
-            raise ak._errors.wrap_error(
-                TypeError("could not convert data into an ak.Array")
-            )
+            raise TypeError("could not convert data into an ak.Array")
 
         if with_name is not None:
             layout = ak.operations.with_name(
                 layout, with_name, highlevel=False, behavior=behavior
             )
 
         if backend is not None and backend != ak.operations.backend(layout):
@@ -291,17 +286,15 @@
 
     @layout.setter
     def layout(self, layout):
         if isinstance(layout, ak.contents.Content):
             self._layout = layout
             self._numbaview = None
         else:
-            raise ak._errors.wrap_error(
-                TypeError("layout must be a subclass of ak.contents.Content")
-            )
+            raise TypeError("layout must be a subclass of ak.contents.Content")
 
     @property
     def behavior(self):
         """
         The `behavior` parameter passed into this Array's constructor.
 
         * If a dict, this `behavior` overrides the global #ak.behavior.
@@ -320,15 +313,15 @@
 
     @behavior.setter
     def behavior(self, behavior):
         if behavior is None or isinstance(behavior, Mapping):
             self.__class__ = get_array_class(self._layout, behavior)
             self._behavior = behavior
         else:
-            raise ak._errors.wrap_error(TypeError("behavior must be None or a dict"))
+            raise TypeError("behavior must be None or a dict")
 
     class Mask:
         def __init__(self, array):
             self._array = array
 
         def __getitem__(self, where):
             with ak._errors.OperationErrorContext(
@@ -1023,17 +1016,15 @@
             "ak.Array.__setitem__",
             {"self": self, "field_name": where, "field_value": what},
         ):
             if not (
                 isinstance(where, str)
                 or (isinstance(where, tuple) and all(isinstance(x, str) for x in where))
             ):
-                raise ak._errors.wrap_error(
-                    TypeError("only fields may be assigned in-place (by field name)")
-                )
+                raise TypeError("only fields may be assigned in-place (by field name)")
 
             self._layout = ak.operations.with_field(
                 self._layout, what, where, highlevel=False
             )
             self._numbaview = None
 
     def __delitem__(self, where):
@@ -1056,17 +1047,15 @@
             "ak.Array.__delitem__",
             {"self": self, "field_name": where},
         ):
             if not (
                 isinstance(where, str)
                 or (isinstance(where, tuple) and all(isinstance(x, str) for x in where))
             ):
-                raise ak._errors.wrap_error(
-                    TypeError("only fields may be removed in-place (by field name)")
-                )
+                raise TypeError("only fields may be removed in-place (by field name)")
 
             self._layout = ak.operations.ak_without_field._impl(
                 self._layout, where, highlevel=False, behavior=self._behavior
             )
             self._numbaview = None
 
     def __getattr__(self, where):
@@ -1108,22 +1097,20 @@
         if hasattr(type(self), where):
             return super().__getattribute__(where)
         else:
             if where in self._layout.fields:
                 try:
                     return self[where]
                 except Exception as err:
-                    raise ak._errors.wrap_error(
-                        AttributeError(
-                            "while trying to get field {}, an exception "
-                            "occurred:\n{}: {}".format(repr(where), type(err), str(err))
-                        )
+                    raise AttributeError(
+                        "while trying to get field {}, an exception "
+                        "occurred:\n{}: {}".format(repr(where), type(err), str(err))
                     ) from err
             else:
-                raise ak._errors.wrap_error(AttributeError(f"no field named {where!r}"))
+                raise AttributeError(f"no field named {where!r}")
 
     def __setattr__(self, name, value):
         """
         Args:
             where (str): Attribute name to set
 
         Set an attribute on the array.
@@ -1144,24 +1131,20 @@
             array = ak.with_field(array, new_field, "z")
 
         to add or modify a field.
         """
         if name.startswith("_") or hasattr(type(self), name):
             super().__setattr__(name, value)
         elif name in self._layout.fields:
-            raise ak._errors.wrap_error(
-                AttributeError(
-                    "fields cannot be set as attributes. use #__setitem__ or #ak.with_field"
-                )
+            raise AttributeError(
+                "fields cannot be set as attributes. use #__setitem__ or #ak.with_field"
             )
         else:
-            raise ak._errors.wrap_error(
-                AttributeError(
-                    "only private attributes (started with an underscore) can be set on arrays"
-                )
+            raise AttributeError(
+                "only private attributes (started with an underscore) can be set on arrays"
             )
 
     def __dir__(self):
         """
         Lists all methods, properties, and field names (see #__getattr__)
         that can be accessed as attributes.
         """
@@ -1449,21 +1432,60 @@
             behavior=copy.deepcopy(self._behavior, memo),
         )
 
     def __bool__(self):
         if len(self) == 1:
             return bool(self[0])
         else:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "the truth value of an array whose length is not 1 is ambiguous; "
-                    "use ak.any() or ak.all()"
-                )
+            raise ValueError(
+                "the truth value of an array whose length is not 1 is ambiguous; "
+                "use ak.any() or ak.all()"
             )
 
+    @property
+    def cpp_type(self):
+        """
+        The C++ type of this Array when it is used in cppyy.
+
+            cpp_type (None or str): Generated on demand when the Array needs to be passed
+                to a C++ (possibly templated) function defined by a `cppyy` compiler.
+
+        See [cppyy documentation](https://cppyy.readthedocs.io/en/latest/index.html)
+        on types and signatures.
+        """
+        ak.cppyy.register_and_check()
+
+        import cppyy
+
+        if self._cpp_type is None:
+            self._generator = ak._connect.cling.togenerator(
+                self.layout.form, flatlist_as_rvec=False
+            )
+            self._lookup = ak._lookup.Lookup(self.layout)
+            self._generator.generate(cppyy.cppdef)
+            self._cpp_type = f"awkward::{self._generator.class_type()}"
+
+        return self._cpp_type
+
+    def __cast_cpp__(self):
+        """
+        The `__cast_cpp__` is called by cppyy to determine a C++ type of an `ak.Array`.
+        It returns the C++ dataset type that is already registered with cppyy with the
+        parameters needed to construct the C++ type of this Array when it is
+        used in cppyy.
+        """
+        import cppyy
+
+        if self._cpp_type is None:
+            self._cpp_type = self.cpp_type
+
+        return getattr(cppyy.gbl, self._cpp_type)(
+            0, len(self), 0, self._lookup.arrayptrs, 0
+        )
+
 
 class Record(NDArrayOperatorsMixin):
     """
     Args:
         data (#ak.record.Record, #ak.Record, str, or dict):
             Data to wrap or convert into a record.
             If a string, the data are assumed to be JSON.
@@ -1519,25 +1541,23 @@
                     contents.append(Array(v).layout[np.newaxis])
                 else:
                     contents.append(Array([v]).layout)
 
             layout = ak.record.Record(ak.contents.RecordArray(contents, fields), at=0)
 
         elif isinstance(data, Iterable):
-            raise ak._errors.wrap_error(
-                TypeError("could not convert non-dict into an ak.Record; try ak.Array")
+            raise TypeError(
+                "could not convert non-dict into an ak.Record; try ak.Array"
             )
 
         else:
             layout = None
 
         if not isinstance(layout, ak.record.Record):
-            raise ak._errors.wrap_error(
-                TypeError("could not convert data into an ak.Record")
-            )
+            raise TypeError("could not convert data into an ak.Record")
 
         if with_name is not None:
             layout = ak.operations.with_name(layout, with_name, highlevel=False)
 
         if library is not None and library != ak.operations.library(layout):
             layout = ak.operations.to_library(layout, library, highlevel=False)
 
@@ -1595,17 +1615,15 @@
 
     @layout.setter
     def layout(self, layout):
         if isinstance(layout, ak.record.Record):
             self._layout = layout
             self._numbaview = None
         else:
-            raise ak._errors.wrap_error(
-                TypeError("layout must be a subclass of ak.record.Record")
-            )
+            raise TypeError("layout must be a subclass of ak.record.Record")
 
     @property
     def behavior(self):
         """
         The `behavior` parameter passed into this Record's constructor.
 
         * If a dict, this `behavior` overrides the global #ak.behavior.
@@ -1624,15 +1642,15 @@
 
     @behavior.setter
     def behavior(self, behavior):
         if behavior is None or isinstance(behavior, Mapping):
             self.__class__ = get_record_class(self._layout, behavior)
             self._behavior = behavior
         else:
-            raise ak._errors.wrap_error(TypeError("behavior must be None or a dict"))
+            raise TypeError("behavior must be None or a dict")
 
     def tolist(self):
         """
         Converts this Record into Python objects; same as #ak.to_list
         (but without the underscore, like NumPy's
         [tolist](https://docs.scipy.org/doc/numpy/reference/generated/numpy.ndarray.tolist.html)).
         """
@@ -1769,17 +1787,15 @@
             "ak.Record.__setitem__",
             {"self": self, "field_name": where, "field_value": what},
         ):
             if not (
                 isinstance(where, str)
                 or (isinstance(where, tuple) and all(isinstance(x, str) for x in where))
             ):
-                raise ak._errors.wrap_error(
-                    TypeError("only fields may be assigned in-place (by field name)")
-                )
+                raise TypeError("only fields may be assigned in-place (by field name)")
 
             self._layout = ak.operations.ak_with_field._impl(
                 self._layout, what, where, highlevel=False, behavior=self._behavior
             )
             self._numbaview = None
 
     def __delitem__(self, where):
@@ -1803,17 +1819,15 @@
             "ak.Record.__delitem__",
             {"self": self, "field_name": where},
         ):
             if not (
                 isinstance(where, str)
                 or (isinstance(where, tuple) and all(isinstance(x, str) for x in where))
             ):
-                raise ak._errors.wrap_error(
-                    TypeError("only fields may be removed in-place (by field name)")
-                )
+                raise TypeError("only fields may be removed in-place (by field name)")
 
             self._layout = ak.operations.ak_without_field._impl(
                 self._layout, where, highlevel=False, behavior=self._behavior
             )
             self._numbaview = None
 
     def __getattr__(self, where):
@@ -1847,22 +1861,20 @@
         if hasattr(type(self), where):
             return super().__getattribute__(where)
         else:
             if where in self._layout.fields:
                 try:
                     return self[where]
                 except Exception as err:
-                    raise ak._errors.wrap_error(
-                        AttributeError(
-                            "while trying to get field {}, an exception "
-                            "occurred:\n{}: {}".format(repr(where), type(err), str(err))
-                        )
+                    raise AttributeError(
+                        "while trying to get field {}, an exception "
+                        "occurred:\n{}: {}".format(repr(where), type(err), str(err))
                     ) from err
             else:
-                raise ak._errors.wrap_error(AttributeError(f"no field named {where!r}"))
+                raise AttributeError(f"no field named {where!r}")
 
     def __setattr__(self, name, value):
         """
         Args:
             where (str): Attribute name to set
 
         Set an attribute on the record.
@@ -1883,24 +1895,20 @@
             record = ak.with_field(record, new_field, "z")
 
         to add or modify a field.
         """
         if name.startswith("_") or hasattr(type(self), name):
             super().__setattr__(name, value)
         elif name in self._layout.fields:
-            raise ak._errors.wrap_error(
-                AttributeError(
-                    "fields cannot be set as attributes. use #__setitem__ or #ak.with_field"
-                )
+            raise AttributeError(
+                "fields cannot be set as attributes. use #__setitem__ or #ak.with_field"
             )
         else:
-            raise ak._errors.wrap_error(
-                AttributeError(
-                    "only private attributes (started with an underscore) can be set on records"
-                )
+            raise AttributeError(
+                "only private attributes (started with an underscore) can be set on records"
             )
 
     def __dir__(self):
         """
         Lists all methods, properties, and field names (see #__getattr__)
         that can be accessed as attributes.
         """
@@ -2083,19 +2091,17 @@
     def __deepcopy__(self, memo):
         return Record(
             copy.deepcopy(self._layout, memo),
             behavior=copy.deepcopy(self._behavior, memo),
         )
 
     def __bool__(self):
-        raise ak._errors.wrap_error(
-            ValueError(
-                "the truth value of a record is ambiguous; "
-                "use ak.any() or ak.all() or pick a field"
-            )
+        raise ValueError(
+            "the truth value of a record is ambiguous; "
+            "use ak.any() or ak.all() or pick a field"
         )
 
 
 class ArrayBuilder(Sized):
     """
     Args:
         behavior (None or dict): Custom #ak.behavior for arrays built by
@@ -2272,15 +2278,15 @@
         return self._behavior
 
     @behavior.setter
     def behavior(self, behavior):
         if behavior is None or isinstance(behavior, dict):
             self._behavior = behavior
         else:
-            raise ak._errors.wrap_error(TypeError("behavior must be None or a dict"))
+            raise TypeError("behavior must be None or a dict")
 
     def tolist(self):
         """
         Converts this Array into Python objects; same as #ak.to_list
         (but without the underscore, like NumPy's
         [tolist](https://docs.scipy.org/doc/numpy/reference/generated/numpy.ndarray.tolist.html)).
         """
@@ -2391,19 +2397,17 @@
 
         return ak._connect.numba.builder.ArrayBuilderType(self._behavior)
 
     def __bool__(self):
         if len(self) == 1:
             return bool(self[0])
         else:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "the truth value of an array whose length is not 1 is ambiguous; "
-                    "use ak.any() or ak.all()"
-                )
+            raise ValueError(
+                "the truth value of an array whose length is not 1 is ambiguous; "
+                "use ak.any() or ak.all()"
             )
 
     def snapshot(self):
         """
         Converts the currently accumulated data into an #ak.Array.
 
         The currently accumulated data are *copied* into the new array.
```

### Comparing `awkward-2.1.1/src/awkward/index.py` & `awkward-2.1.2/src/awkward/index.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 
-import awkward as ak
 from awkward._nplikes import nplike_of, to_nplike
 from awkward._nplikes.cupy import Cupy
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyLike, NumpyMetadata
 from awkward._nplikes.typetracer import TypeTracer
-from awkward.typing import Self
+from awkward._typing import Self
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
 _dtype_to_form = {
     np.dtype(np.int8): "i8",
@@ -33,39 +32,35 @@
     elif form == "i32":
         return Index32(numpy.zeros(0, dtype=np.int32))
     elif form == "u32":
         return IndexU32(numpy.zeros(0, dtype=np.uint32))
     elif form == "i64":
         return Index64(numpy.zeros(0, dtype=np.int64))
     else:
-        raise ak._errors.wrap_error(
-            AssertionError(f"unrecognized Index form: {form!r}")
-        )
+        raise AssertionError(f"unrecognized Index form: {form!r}")
 
 
 class Index:
     _expected_dtype = None
 
     def __init__(self, data, *, metadata=None, nplike=None):
         if nplike is None:
             nplike = nplike_of(data)
         self._nplike = nplike
         if metadata is not None and not isinstance(metadata, dict):
-            raise ak._errors.wrap_error(
-                TypeError("Index metadata must be None or a dict")
-            )
+            raise TypeError("Index metadata must be None or a dict")
         self._metadata = metadata
         # We don't care about F, C (it's one dimensional), but we do need
         # the array to be contiguous. This should _not_ return a copy if already
         self._data = self._nplike.ascontiguousarray(
             self._nplike.asarray(data, dtype=self._expected_dtype)
         )
 
         if len(self._data.shape) != 1:
-            raise ak._errors.wrap_error(TypeError("Index data must be one-dimensional"))
+            raise TypeError("Index data must be one-dimensional")
 
         if issubclass(self._data.dtype.type, np.longlong):
             assert (
                 np.dtype(np.longlong).itemsize == 8
             ), "longlong is always 64-bit, right?"
 
             self._data = self._data.view(np.int64)
@@ -78,27 +73,23 @@
             elif self._data.dtype == np.dtype(np.int32):
                 self.__class__ = Index32
             elif self._data.dtype == np.dtype(np.uint32):
                 self.__class__ = IndexU32
             elif self._data.dtype == np.dtype(np.int64):
                 self.__class__ = Index64
             else:
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "Index data must be int8, uint8, int32, uint32, int64, not "
-                        + repr(self._data.dtype)
-                    )
+                raise TypeError(
+                    "Index data must be int8, uint8, int32, uint32, int64, not "
+                    + repr(self._data.dtype)
                 )
         else:
             if self._data.dtype != self._expected_dtype:
                 # self._data = self._data.astype(self._expected_dtype)   # copy/convert
-                raise ak._errors.wrap_error(
-                    NotImplementedError(
-                        "while developing, we want to catch these errors"
-                    )
+                raise NotImplementedError(
+                    "while developing, we want to catch these errors"
                 )
 
     @classmethod
     def zeros(cls, length, nplike, dtype=None):
         if dtype is None:
             dtype = cls._expected_dtype
         return Index(nplike.zeros(length, dtype=dtype), nplike=nplike)
@@ -145,16 +136,21 @@
 
     def raw(self, nplike):
         return to_nplike(self.data, nplike, from_nplike=self._nplike)
 
     def __len__(self):
         return self.length
 
-    def __array__(self, dtype=None):
-        return self._nplike.asarray(self._data, dtype=dtype)
+    @property
+    def __cuda_array_interface__(self):
+        return self._data.__cuda_array_interface__
+
+    @property
+    def __array_interface__(self):
+        return self._data.__array_interface__
 
     def __repr__(self):
         return self._repr("", "", "")
 
     def _repr(self, indent, pre, post):
         out = [indent, pre, "<Index dtype="]
         out.append(repr(str(self.dtype)))
```

### Comparing `awkward-2.1.1/src/awkward/jax.py` & `awkward-2.1.2/src/awkward/jax.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 
 import enum
 import threading
 import weakref
 
 import awkward as ak
 from awkward import highlevel
-from awkward._errors import wrap_error
 from awkward._nplikes.numpy import Numpy
-from awkward.typing import TypeVar
+from awkward._typing import TypeVar
 
 numpy = Numpy.instance()
 
 
 def assert_never(arg) -> None:
-    raise wrap_error(AssertionError(f"this should never be run: {arg}"))
+    raise AssertionError(f"this should never be run: {arg}")
 
 
 class _RegistrationState(enum.Enum):
     INIT = enum.auto()
     SUCCESS = enum.auto()
     FAILED = enum.auto()
 
@@ -31,25 +30,23 @@
     """
     Register Awkward Array node types with JAX's tree mechanism.
     """
     try:
         import jax  # noqa: TID251
 
     except ModuleNotFoundError:
-        raise wrap_error(
-            ModuleNotFoundError(
-                """install the 'jax' package with:
+        raise ModuleNotFoundError(
+            """install the 'jax' package with:
 
         python3 -m pip install jax jaxlib
 
     or
 
         conda install -c conda-forge jax jaxlib
     """
-            )
         ) from None
 
     _register()
 
 
 HighLevelType = TypeVar(
     "HighLevelType", bound="type[highlevel.Array | highlevel.Record]"
@@ -107,33 +104,29 @@
             ]:
                 jax_connect.register_pytree_class(cls)
 
             for cls in _known_highlevel_classes:
                 jax_connect.register_pytree_class(cls)
         except Exception:
             _registration_state = _RegistrationState.FAILED
-            raise  # noqa: AK101
+            raise
         else:
             _registration_state = _RegistrationState.SUCCESS
 
 
 def assert_registered():
     """Ensure that JAX integration is registered. Raise a RuntimeError if not."""
     with _registration_lock:
         if _registration_state == _RegistrationState.INIT:
-            raise wrap_error(
-                RuntimeError("JAX features require `ak.jax.register_and_check()`")
-            )
+            raise RuntimeError("JAX features require `ak.jax.register_and_check()`")
         elif _registration_state == _RegistrationState.FAILED:
-            raise wrap_error(
-                RuntimeError(
-                    "JAX features require `ak.jax.register_and_check()`, "
-                    "but the last call to `ak.jax.register_and_check()` did not succeed. "
-                    "Please look for a traceback to identify the error."
-                )
+            raise RuntimeError(
+                "JAX features require `ak.jax.register_and_check()`, "
+                "but the last call to `ak.jax.register_and_check()` did not succeed. "
+                "Please look for a traceback to identify the error."
             )
         elif _registration_state == _RegistrationState.SUCCESS:
             return
 
         assert_never(_registration_state)
```

### Comparing `awkward-2.1.1/src/awkward/numba.py` & `awkward-2.1.2/src/awkward/numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/record.py` & `awkward-2.1.2/src/awkward/record.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import copy
 from collections.abc import Iterable
 
 import awkward as ak
+from awkward._backends import Backend
 from awkward._behavior import get_record_class
 from awkward._layout import wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._regularize import is_integer
+from awkward._typing import Self
 from awkward._util import unset
 from awkward.contents.content import Content
-from awkward.typing import Self
 
 np = NumpyMetadata.instance()
 
 
 class Record:
     """
     Represents a single value from a #ak.contents.RecordArray.
@@ -30,26 +31,20 @@
 
     The Record shares a reference with its #ak.layout.RecordArray;
     it is not a copy.
     """
 
     def __init__(self, array, at):
         if not isinstance(array, ak.contents.RecordArray):
-            raise ak._errors.wrap_error(
-                TypeError(f"Record 'array' must be a RecordArray, not {array!r}")
-            )
+            raise TypeError(f"Record 'array' must be a RecordArray, not {array!r}")
         if not is_integer(at):
-            raise ak._errors.wrap_error(
-                TypeError(f"Record 'at' must be an integer, not {array!r}")
-            )
+            raise TypeError(f"Record 'at' must be an integer, not {array!r}")
         if not (array.length is unknown_length or 0 <= at < array.length):
-            raise ak._errors.wrap_error(
-                ValueError(
-                    f"Record 'at' must be >= 0 and < len(array) == {array.length}, not {at}"
-                )
+            raise ValueError(
+                f"Record 'at' must be >= 0 and < len(array) == {array.length}, not {at}"
             )
         else:
             self._array = array
             self._at = at
 
     @property
     def array(self):
@@ -136,75 +131,57 @@
 
     def __getitem__(self, where):
         with ak._errors.SlicingErrorContext(self, where):
             return self._getitem(where)
 
     def _getitem(self, where):
         if is_integer(where):
-            raise ak._errors.wrap_error(
-                IndexError("scalar Record cannot be sliced by an integer")
-            )
+            raise IndexError("scalar Record cannot be sliced by an integer")
 
         elif isinstance(where, slice):
-            raise ak._errors.wrap_error(
-                IndexError("scalar Record cannot be sliced by a range slice (`:`)")
-            )
+            raise IndexError("scalar Record cannot be sliced by a range slice (`:`)")
 
         elif isinstance(where, str):
             return self._getitem_field(where)
 
         elif where is np.newaxis:
-            raise ak._errors.wrap_error(
-                IndexError("scalar Record cannot be sliced by np.newaxis (`None`)")
-            )
+            raise IndexError("scalar Record cannot be sliced by np.newaxis (`None`)")
 
         elif where is Ellipsis:
-            raise ak._errors.wrap_error(
-                IndexError("scalar Record cannot be sliced by an ellipsis (`...`)")
-            )
+            raise IndexError("scalar Record cannot be sliced by an ellipsis (`...`)")
 
         elif isinstance(where, tuple) and len(where) == 0:
             return self
 
         elif isinstance(where, tuple) and len(where) == 1:
             return self._getitem(where[0])
 
         elif isinstance(where, tuple) and isinstance(where[0], str):
             return self._getitem_field(where[0])._getitem(where[1:])
 
         elif isinstance(where, ak.highlevel.Array):
-            raise ak._errors.wrap_error(
-                IndexError("scalar Record cannot be sliced by an array")
-            )
+            raise IndexError("scalar Record cannot be sliced by an array")
 
         elif isinstance(where, ak.contents.Content):
-            raise ak._errors.wrap_error(
-                IndexError("scalar Record cannot be sliced by an array")
-            )
+            raise IndexError("scalar Record cannot be sliced by an array")
 
         elif isinstance(where, Content):
-            raise ak._errors.wrap_error(
-                IndexError("scalar Record cannot be sliced by an array")
-            )
+            raise IndexError("scalar Record cannot be sliced by an array")
 
         elif isinstance(where, Iterable) and all(isinstance(x, str) for x in where):
             return self._getitem_fields(where)
 
         elif isinstance(where, Iterable):
-            raise ak._errors.wrap_error(
-                IndexError("scalar Record cannot be sliced by an array")
-            )
+            raise IndexError("scalar Record cannot be sliced by an array")
 
         else:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "only field name (str) or names (non-tuple iterable of str) "
-                    "are valid indices for slicing a scalar record, not\n\n    "
-                    + repr(where)
-                )
+            raise TypeError(
+                "only field name (str) or names (non-tuple iterable of str) "
+                "are valid indices for slicing a scalar record, not\n\n    "
+                + repr(where)
             )
 
     def _getitem_field(self, where, only_fields: tuple[str, ...] = ()) -> Content:
         return self._array._getitem_field(where)._getitem_at(self._at)
 
     def _getitem_fields(self, where, only_fields: tuple[str, ...] = ()):
         return self._array._getitem_fields(where)._getitem_at(self._at)
@@ -243,14 +220,24 @@
             ]
 
         if self.is_tuple and json_conversions is None:
             return tuple(contents)
         else:
             return dict(zip(self._array.fields, contents))
 
+    def to_backend(self, backend: Backend | str | None = None) -> Self:
+        if backend is None:
+            backend = self._array.backend
+        else:
+            backend = ak._backends.regularize_backend(backend)
+        if backend is self._array.backend:
+            return self
+        else:
+            return Record(self._array._to_backend(backend), self._at)
+
     def __copy__(self) -> Self:
         return self.copy()
 
     def __deepcopy__(self, memo):
         return Record(copy.deepcopy(self._array, memo), self._at)
 
     def copy(self, array=unset, at=unset) -> Self:
```

### Comparing `awkward-2.1.1/src/awkward/_connect/avro.py` & `awkward-2.1.2/src/awkward/_connect/avro.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
         self.temp_header = bytearray()
         self.metadata = {}
 
         while True:
             try:
                 self.temp_header += self.data.read(numbytes)
                 if not self.check_valid():
-                    raise ak._errors.wrap_error(
-                        TypeError("invalid Avro file: first 4 bytes are not b'Obj\x01'")
+                    raise TypeError(
+                        "invalid Avro file: first 4 bytes are not b'Obj\x01'"
                     )
                 pos = 4
                 pos, self.pairs = self.decode_varint(4, self.temp_header)
                 self.pairs = self.decode_zigzag(self.pairs)
                 if self.pairs < 0:
                     pos, self.header_size = self.decode_varint(pos, self.temp_header)
                     self.header_size = self.decode_zigzag(self.pairs)
@@ -79,15 +79,15 @@
         machine = awkward.forth.ForthMachine64(forth_code)
         break_flag = False
         while True:
             try:
                 pos, num_items, len_block = self.decode_block()
                 temp_data = self.data.read(len_block)
                 if len(temp_data) < len_block:
-                    raise _ReachedEndofArrayError  # noqa: AK101
+                    raise _ReachedEndofArrayError
                 self.update_pos(len_block)
             except _ReachedEndofArrayError:
                 break
 
             if limit_entries is not None and self.blocks > limit_entries:
                 temp_diff = int(self.blocks - limit_entries)
                 self.blocks -= temp_diff
@@ -140,43 +140,43 @@
         temp_count = 0
         while temp_count < self.pairs:
             pos, dat = self.decode_varint(pos, self.temp_header)
             dat = self.decode_zigzag(dat)
             key = self.temp_header[pos : pos + int(dat)]
             pos = pos + int(dat)
             if len(key) < int(dat):
-                raise _ReachedEndofArrayError  # noqa: AK101
+                raise _ReachedEndofArrayError
 
             pos, dat = self.decode_varint(pos, self.temp_header)
             dat = self.decode_zigzag(dat)
             val = self.temp_header[pos : pos + int(dat)]
             pos = pos + int(dat)
             if len(val) < int(dat):
-                raise _ReachedEndofArrayError  # noqa: AK101
+                raise _ReachedEndofArrayError
             if key == b"avro.schema":
                 self.metadata[key.decode()] = json.loads(val.decode())
             else:
                 self.metadata[key.decode()] = val
 
             temp_count += 1
 
         return pos
 
     def check_valid(self):
         init = self.temp_header[0:4]
         if len(init) < 4:
-            raise _ReachedEndofArrayError  # noqa: AK101
+            raise _ReachedEndofArrayError
         return init == b"Obj\x01"
 
     def decode_varint(self, pos, _data):
         shift = 0
         result = 0
         while True:
             if pos >= len(_data):
-                raise _ReachedEndofArrayError  # noqa: AK101
+                raise _ReachedEndofArrayError
             i = _data[pos]
             pos += 1
             result |= (i & 0x7F) << shift
             shift += 7
             if not i & 0x80:
                 break
 
@@ -199,15 +199,15 @@
         elif dtype["type"] == "bytes":
             return f"1 node{count}-offsets +<- stack 97 node{count+1}-data <- stack "
         elif dtype["type"] == "string":
             return f"0 node{count}-offsets +<- stack "
         elif dtype["type"] == "enum":
             return f"0 node{count}-index <- stack "
         else:
-            raise AssertionError  # noqa: AK101
+            raise AssertionError
 
     def rec_exp_json_code(
         self,
         file,
         exec_code,
         ind,
         form_next_id,
@@ -907,13 +907,11 @@
             #         kk = "\n"+"    "*ind+'''if out != 0:
             #     raise
             #             '''
             #         exec_code = exec_code+gg
             #         exec_code = exec_code+hh
             #         exec_code = exec_code+jj
             #         exec_code = exec_code+kk
-            raise ak._errors.wrap_error(NotImplementedError)
+            raise NotImplementedError
 
         else:
-            raise ak._errors.wrap_error(
-                AssertionError(f"unrecognized Avro type: {file['type']}")
-            )
+            raise AssertionError(f"unrecognized Avro type: {file['type']}")
```

### Comparing `awkward-2.1.1/src/awkward/_connect/cling.py` & `awkward-2.1.2/src/awkward/_connect/cling.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,15 +478,15 @@
     elif isinstance(form, ak.forms.RecordForm):
         return RecordArrayGenerator.from_form(form, flatlist_as_rvec)
 
     elif isinstance(form, ak.forms.UnionForm):
         return UnionArrayGenerator.from_form(form, flatlist_as_rvec)
 
     else:
-        raise ak._errors.wrap_error(AssertionError(f"unrecognized Form: {type(form)}"))
+        raise AssertionError(f"unrecognized Form: {type(form)}")
 
 
 class Generator:
     def IndexOf(self, arraytype):
         if arraytype == "int8_t":
             return ak.index.Index8
         elif arraytype == "uint8_t":
@@ -496,15 +496,15 @@
         elif arraytype == "uint32_t":
             return ak.index.IndexU32
         elif arraytype == "int64_t":
             return ak.index.Index64
         elif arraytype == "uint64_t":
             return ak.index.IndexU64
         else:
-            raise ak._errors.wrap_error(AssertionError(arraytype))
+            raise AssertionError(arraytype)
 
     def class_type_suffix(self, key):
         return ak._util.identifier_hash(key)
 
     def _generate_common(self, key):
         params = [
             f"if (parameter == {json.dumps(name)}) return {json.dumps(json.dumps(value))};\n      "
@@ -789,15 +789,15 @@
         if index_type == "i32":
             self.index_type = "int32_t"
         elif index_type == "u32":
             self.index_type = "uint32_t"
         elif index_type == "i64":
             self.index_type = "int64_t"
         else:
-            raise ak._errors.wrap_error(AssertionError(index_type))
+            raise AssertionError(index_type)
         self.content = content
 
         # FIXME: satisfy the ContentLookup super-class
         self.contenttype = content
         self.indextype = self.index_type
 
         self.parameters = parameters
@@ -938,15 +938,15 @@
         if index_type == "i32":
             self.indextype = "int32_t"
         elif index_type == "u32":
             self.indextype = "uint32_t"
         elif index_type == "i64":
             self.indextype = "int64_t"
         else:
-            raise ak._errors.wrap_error(AssertionError(index_type))
+            raise AssertionError(index_type)
         self.contenttype = content
         self.parameters = parameters
         self.flatlist_as_rvec = flatlist_as_rvec
         assert self.flatlist_as_rvec == self.contenttype.flatlist_as_rvec
 
     def __hash__(self):
         return hash(
@@ -1013,15 +1013,15 @@
 
     def __init__(self, index_type, content, parameters, flatlist_as_rvec):
         if index_type == "i32":
             self.index_type = "int32_t"
         elif index_type == "i64":
             self.index_type = "int64_t"
         else:
-            raise ak._errors.wrap_error(AssertionError(index_type))
+            raise AssertionError(index_type)
         self.contenttype = content
         self.parameters = parameters
         self.flatlist_as_rvec = flatlist_as_rvec
         self.indextype = self.index_type
         assert self.flatlist_as_rvec == self.contenttype.flatlist_as_rvec
 
     def __hash__(self):
@@ -1505,15 +1505,15 @@
         if index_type == "i32":
             self.indextype = "int32_t"
         elif index_type == "u32":
             self.indextype = "uint32_t"
         elif index_type == "i64":
             self.indextype = "int64_t"
         else:
-            raise ak._errors.wrap_error(AssertionError(index_type))
+            raise AssertionError(index_type)
         self.contenttypes = tuple(contents)
         self.parameters = parameters
         self.flatlist_as_rvec = flatlist_as_rvec
         for content in self.contenttypes:
             assert self.flatlist_as_rvec == content.flatlist_as_rvec
 
     def __hash__(self):
```

### Comparing `awkward-2.1.1/src/awkward/_connect/hist.py` & `awkward-2.1.2/src/awkward/_connect/hist.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 """
 from __future__ import annotations
 
 import numpy as np
 
 import awkward as ak
 from awkward._backends import NumpyBackend
-from awkward.typing import Any, Sequence
+from awkward._typing import Any, Sequence
 
 numpy = NumpyBackend.instance()
 
 
 def unpack(array: ak.Array) -> dict[str, ak.Array] | None:
     if not ak.fields(array):
         return None
@@ -23,13 +23,11 @@
 def broadcast_and_flatten(args: Sequence[Any]) -> tuple[np.ndarray]:
     try:
         arrays = [ak.Array(x, backend=numpy) for x in args]
     except TypeError:
         return NotImplementedError
 
     if any(x.fields for x in arrays):
-        raise ak._errors.wrap_error(
-            ValueError("cannot broadcast-and-flatten array with structure (fields)")
-        )
+        raise ValueError("cannot broadcast-and-flatten array with structure (fields)")
     return tuple(
         ak.to_numpy(ak.flatten(x, axis=None)) for x in ak.broadcast_arrays(*arrays)
     )
```

### Comparing `awkward-2.1.1/src/awkward/_connect/numexpr.py` & `awkward-2.1.2/src/awkward/_connect/numexpr.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,34 +10,33 @@
 
 
 def _import_numexpr():
     global _has_checked_version
     try:
         import numexpr
     except ModuleNotFoundError as err:
-        raise ak._errors.wrap_error(
-            ModuleNotFoundError(
-                """install the 'numexpr' package with:
+        raise ModuleNotFoundError(
+            """install the 'numexpr' package with:
 
     pip install numexpr --upgrade
 
 or
 
     conda install numexpr"""
-            )
         ) from err
     else:
         if not _has_checked_version:
             if ak._util.parse_version(numexpr.__version__) < ak._util.parse_version(
                 "2.7.1"
             ):
                 warnings.warn(
                     "Awkward Array is only known to work with numexpr 2.7.1 or later"
                     "(you have version {})".format(numexpr.__version__),
                     RuntimeWarning,
+                    stacklevel=1,
                 )
             _has_checked_version = True
         return numexpr
 
 
 def getArguments(names, local_dict=None, global_dict=None):
     call_frame = sys._getframe(2)
@@ -120,17 +119,15 @@
 
 def re_evaluate(local_dict=None):
     numexpr = _import_numexpr()
 
     try:
         compiled_ex = numexpr.necompiler._numexpr_last["ex"]  # noqa: F841
     except KeyError as err:
-        raise ak._errors.wrap_error(
-            RuntimeError("not a previous evaluate() execution found")
-        ) from err
+        raise RuntimeError("not a previous evaluate() execution found") from err
     names = numexpr.necompiler._numexpr_last["argnames"]
     arguments = getArguments(names, local_dict)
 
     arrays = [
         ak.operations.to_layout(x, allow_record=True, allow_other=True)
         for x in arguments
     ]
```

### Comparing `awkward-2.1.1/src/awkward/_connect/numpy.py` & `awkward-2.1.2/src/awkward/_connect/numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import functools
 import inspect
 
 import numpy
 
 import awkward as ak
+from awkward._backends import backend_of
 from awkward._behavior import (
     behavior_of,
     find_custom_cast,
     find_ufunc,
     find_ufunc_generic,
 )
 from awkward._layout import wrap_layout
@@ -49,19 +50,17 @@
     if backend is not None:
         return ak.operations.to_numpy(arg)
     elif isinstance(arg, tuple):
         return tuple(_to_rectilinear(x) for x in arg)
     elif isinstance(arg, list):
         return [_to_rectilinear(x) for x in arg]
     elif is_non_string_like_iterable(arg):
-        raise ak._errors.wrap_error(
-            TypeError(
-                f"encountered an unsupported iterable value {arg!r} whilst converting arguments to NumPy-friendly "
-                f"types. If this argument should be supported, please file a bug report."
-            )
+        raise TypeError(
+            f"encountered an unsupported iterable value {arg!r} whilst converting arguments to NumPy-friendly "
+            f"types. If this argument should be supported, please file a bug report."
         )
     else:
         return arg
 
 
 def _array_function_no_impl(func, types, args, kwargs, behavior):
     rectilinear_args = tuple(_to_rectilinear(x) for x in args)
@@ -92,43 +91,43 @@
 
         @functools.wraps(function)
         def ensure_valid_args(*args, **kwargs):
             parameters = signature.bind(*args, **kwargs)
             provided_invalid_names = parameters.arguments.keys() & unsupported_names
             if provided_invalid_names:
                 names = ", ".join(provided_invalid_names)
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        f"Awkward NEP-18 overload was provided with unsupported argument(s): {names}"
-                    )
+                raise TypeError(
+                    f"Awkward NEP-18 overload was provided with unsupported argument(s): {names}"
                 )
             return function(*args, **kwargs)
 
         implemented[getattr(numpy, numpy_function)] = ensure_valid_args
         return function
 
     return decorator
 
 
-def _array_ufunc_custom_cast(inputs, behavior):
+def _array_ufunc_custom_cast(inputs, behavior, backend):
     args = [
         wrap_layout(x, behavior)
         if isinstance(x, (ak.contents.Content, ak.record.Record))
         else x
         for x in inputs
     ]
 
     nextinputs = []
     for x in args:
         cast_fcn = find_custom_cast(x, behavior)
         if cast_fcn is not None:
             x = cast_fcn(x)
-        nextinputs.append(
-            ak.operations.to_layout(x, allow_record=True, allow_other=True)
-        )
+        maybe_layout = ak.operations.to_layout(x, allow_record=True, allow_other=True)
+        if isinstance(maybe_layout, (ak.contents.Content, ak.record.Record)):
+            maybe_layout = maybe_layout.to_backend(backend)
+
+        nextinputs.append(maybe_layout)
     return nextinputs
 
 
 def _array_ufunc_adjust(custom, inputs, kwargs, behavior):
     args = [
         wrap_layout(x, behavior)
         if isinstance(x, (ak.contents.Content, ak.record.Record))
@@ -180,36 +179,34 @@
 
 
 def array_ufunc(ufunc, method, inputs, kwargs):
     if method != "__call__" or len(inputs) == 0 or "out" in kwargs:
         return NotImplemented
 
     behavior = behavior_of(*inputs)
+    backend = backend_of(*inputs)
 
-    inputs = _array_ufunc_custom_cast(inputs, behavior)
+    inputs = _array_ufunc_custom_cast(inputs, behavior, backend)
 
     def action(inputs, **ignore):
         signature = _array_ufunc_signature(ufunc, inputs)
         custom = find_ufunc(behavior, signature)
         # Do we have a custom ufunc (an override of the given ufunc)?
         if custom is not None:
             return _array_ufunc_adjust(custom, inputs, kwargs, behavior)
 
         if ufunc is numpy.matmul:
-            raise ak._errors.wrap_error(
-                NotImplementedError(
-                    "matrix multiplication (`@` or `np.matmul`) is not yet implemented for Awkward Arrays"
-                )
+            raise NotImplementedError(
+                "matrix multiplication (`@` or `np.matmul`) is not yet implemented for Awkward Arrays"
             )
 
         if all(
             isinstance(x, NumpyArray) or not isinstance(x, ak.contents.Content)
             for x in inputs
         ):
-            backend = ak._backends.backend_of(*inputs)
             nplike = backend.nplike
 
             # Broadcast parameters against one another
             parameters_factory = ak._broadcasting.intersection_parameters_factory(
                 inputs
             )
             (parameters,) = parameters_factory(1)
@@ -249,19 +246,17 @@
                         error_message.append(x.parameter("__array__"))
                     elif x.parameter("__record__") is not None:
                         error_message.append(x.parameter("__record__"))
                     else:
                         error_message.append(type(x).__name__)
                 else:
                     error_message.append(type(x).__name__)
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "no {}.{} overloads for custom types: {}".format(
-                        type(ufunc).__module__, ufunc.__name__, ", ".join(error_message)
-                    )
+            raise TypeError(
+                "no {}.{} overloads for custom types: {}".format(
+                    type(ufunc).__module__, ufunc.__name__, ", ".join(error_message)
                 )
             )
 
         return None
 
     if sum(int(isinstance(x, ak.contents.Content)) for x in inputs) == 1:
         where = None
@@ -297,8 +292,8 @@
         assert isinstance(out, tuple) and len(out) == 1
         out = out[0]
 
     return wrap_layout(out, behavior)
 
 
 def action_for_matmul(inputs):
-    raise ak._errors.wrap_error(NotImplementedError)
+    raise NotImplementedError
```

### Comparing `awkward-2.1.1/src/awkward/_connect/pyarrow.py` & `awkward-2.1.2/src/awkward/_connect/pyarrow.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import json
 from collections.abc import Iterable, Sized
 
 import awkward as ak
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
-from awkward.forms.form import _parameters_union
+from awkward._parameters import parameters_union
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 try:
     import pyarrow
 
@@ -367,18 +367,16 @@
     # Start by removing the ExtensionArray wrapper.
     if awkwardarrow_type is not None:
         paarray = paarray.storage
 
     ### Beginning of the big if-elif-elif chain!
 
     if isinstance(storage_type, pyarrow.lib.PyExtensionType):
-        raise ak._errors.wrap_error(
-            ValueError(
-                "Arrow arrays containing pickled Python objects can't be converted into Awkward Arrays"
-            )
+        raise ValueError(
+            "Arrow arrays containing pickled Python objects can't be converted into Awkward Arrays"
         )
 
     elif isinstance(storage_type, pyarrow.lib.ExtensionType):
         # AwkwardArrowType should already be unwrapped; this must be some other ExtensionType.
         assert not isinstance(storage_type, AwkwardArrowType)
         # In that case, just ignore its logical type and use its storage type.
         return popbuffers(
@@ -403,15 +401,15 @@
             mask = masked_index.mask_as_bool(valid_when=False)
             if mask.any():
                 index = numpy.asarray(index, copy=True)
                 index[mask] = -1
 
         content = handle_arrow(paarray.dictionary, generate_bitmasks)
 
-        parameters = ak.forms.form._parameters_union(
+        parameters = parameters_union(
             mask_parameters(awkwardarrow_type), node_parameters(awkwardarrow_type)
         )
         if parameters is None:
             parameters = {"__array__": "categorical"}
 
         return revertable(
             ak.contents.IndexedOptionArray.simplified(
@@ -469,25 +467,23 @@
         return popbuffers_finalize(
             out, paarray, validbits, awkwardarrow_type, generate_bitmasks
         )
 
     elif isinstance(storage_type, pyarrow.lib.MapType):
         # FIXME: make a ListOffsetArray of 2-tuples with __array__ == "sorted_map".
         # (Make sure the keys are sorted).
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     elif isinstance(
         storage_type, (pyarrow.lib.Decimal128Type, pyarrow.lib.Decimal256Type)
     ):
         # Note: Decimal128Type and Decimal256Type are subtypes of FixedSizeBinaryType.
         # NumPy doesn't support decimal: https://github.com/numpy/numpy/issues/9789
-        raise ak._errors.wrap_error(
-            ValueError(
-                "Arrow arrays containing pyarrow.decimal128 or pyarrow.decimal256 types can't be converted into Awkward Arrays"
-            )
+        raise ValueError(
+            "Arrow arrays containing pyarrow.decimal128 or pyarrow.decimal256 types can't be converted into Awkward Arrays"
         )
 
     elif isinstance(storage_type, pyarrow.lib.FixedSizeBinaryType):
         assert storage_type.num_buffers == 2
         validbits = buffers.pop(0)
         pacontent = buffers.pop(0)
 
@@ -661,27 +657,23 @@
             backend=ak._backends.NumpyBackend.instance(),
         )
         return popbuffers_finalize(
             out, paarray, validbits, awkwardarrow_type, generate_bitmasks
         )
 
     else:
-        raise ak._errors.wrap_error(
-            TypeError(f"unrecognized Arrow array type: {storage_type!r}")
-        )
+        raise TypeError(f"unrecognized Arrow array type: {storage_type!r}")
 
 
 def form_popbuffers(awkwardarrow_type, storage_type):
     ### Beginning of the big if-elif-elif chain!
 
     if isinstance(storage_type, pyarrow.lib.PyExtensionType):
-        raise ak._errors.wrap_error(
-            ValueError(
-                "Arrow arrays containing pickled Python objects can't be converted into Awkward Arrays"
-            )
+        raise ValueError(
+            "Arrow arrays containing pickled Python objects can't be converted into Awkward Arrays"
         )
 
     elif isinstance(storage_type, pyarrow.lib.ExtensionType):
         # AwkwardArrowType should already be unwrapped; this must be some other ExtensionType.
         assert not isinstance(storage_type, AwkwardArrowType)
         # In that case, just ignore its logical type and use its storage type.
         return form_popbuffers(awkwardarrow_type, storage_type.storage_type)
@@ -691,22 +683,22 @@
         if index_type is np.int64:
             index = "i64"
         elif index_type is np.uint32:
             index = "u32"
         elif index_type is np.int32:
             index = "i32"
         else:
-            raise ak._errors.wrap_error(
-                TypeError(f"unrecognized Arrow DictionaryType index type: {index_type}")
+            raise TypeError(
+                f"unrecognized Arrow DictionaryType index type: {index_type}"
             )
 
         a, b = to_awkwardarrow_storage_types(storage_type.value_type)
         content = form_popbuffers(a, b)
 
-        parameters = _parameters_union(
+        parameters = parameters_union(
             mask_parameters(awkwardarrow_type), node_parameters(awkwardarrow_type)
         )
         if parameters is None:
             parameters = {"__array__": "categorical"}
 
         return revertable(
             ak.forms.IndexedOptionForm.simplified(
@@ -751,25 +743,23 @@
 
         out = ak.forms.ListOffsetForm(
             akoffsets, akcontent, parameters=node_parameters(awkwardarrow_type)
         )
         return form_popbuffers_finalize(out, awkwardarrow_type)
 
     elif isinstance(storage_type, pyarrow.lib.MapType):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     elif isinstance(
         storage_type, (pyarrow.lib.Decimal128Type, pyarrow.lib.Decimal256Type)
     ):
         # Note: Decimal128Type and Decimal256Type are subtypes of FixedSizeBinaryType.
         # NumPy doesn't support decimal: https://github.com/numpy/numpy/issues/9789
-        raise ak._errors.wrap_error(
-            ValueError(
-                "Arrow arrays containing pyarrow.decimal128 or pyarrow.decimal256 types can't be converted into Awkward Arrays"
-            )
+        raise ValueError(
+            "Arrow arrays containing pyarrow.decimal128 or pyarrow.decimal256 types can't be converted into Awkward Arrays"
         )
 
     elif isinstance(storage_type, pyarrow.lib.FixedSizeBinaryType):
         parameters = node_parameters(awkwardarrow_type)
         if parameters is None:
             parameters = {"__array__": "bytestring"}
         sub_parameters = {"__array__": "byte"}
@@ -864,17 +854,15 @@
             ak.types.numpytype.dtype_to_primitive(dt),
             parameters=node_parameters(awkwardarrow_type),
         )
 
         return form_popbuffers_finalize(out, awkwardarrow_type)
 
     else:
-        raise ak._errors.wrap_error(
-            TypeError(f"unrecognized Arrow array type: {storage_type!r}")
-        )
+        raise TypeError(f"unrecognized Arrow array type: {storage_type!r}")
 
 
 def to_awkwardarrow_type(
     storage_type, use_extensionarray, record_is_scalar, mask, node
 ):
     if use_extensionarray:
         return AwkwardArrowType(
@@ -1050,15 +1038,15 @@
         else:
             return ak.operations.concatenate(chunks, highlevel=False)
 
     elif isinstance(obj, Iterable) and len(obj) == 0:
         return ak.contents.RecordArray([], [], length=0)
 
     else:
-        raise ak._errors.wrap_error(TypeError(f"unrecognized Arrow type: {type(obj)}"))
+        raise TypeError(f"unrecognized Arrow type: {type(obj)}")
 
 
 def form_handle_arrow(schema, pass_empty_field=False):
     if pass_empty_field and list(schema.names) == [""]:
         awkwardarrow_type, storage_type = to_awkwardarrow_storage_types(schema.types[0])
         akform = form_popbuffers(awkwardarrow_type, storage_type)
         if not schema.field(0).nullable:
```

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/__init__.py` & `awkward-2.1.2/src/awkward/_connect/cuda/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 
 import glob
 import math
 import os
 
 import numpy
 
-import awkward
-
 try:
     import cupy
 
     error_message = None
 
 except ModuleNotFoundError:
     cupy = None
@@ -145,17 +143,16 @@
     @property
     def error_context(self):
         return self._error_context
 
 
 def import_cupy(name="Awkward Arrays with CUDA"):
     if cupy is None:
-        raise awkward._errors.wrap_error(
-            ModuleNotFoundError(error_message.format(name))
-        )
+        raise ModuleNotFoundError(error_message.format(name))
+
     return cupy
 
 
 def initialize_cuda_kernels(cupy):
     if cupy is not None:
         global kernel
 
@@ -193,17 +190,15 @@
             )
             kernel = awkward._connect.cuda._kernel_signatures.by_signature(
                 cuda_kernel_templates
             )
 
         return kernel
     else:
-        raise awkward._errors.wrap_error(
-            ModuleNotFoundError(error_message.format("Awkward Arrays with CUDA"))
-        )
+        raise ModuleNotFoundError(error_message.format("Awkward Arrays with CUDA"))
 
 
 def synchronize_cuda(stream=None):
     cupy = import_cupy("Awkward Arrays with CUDA")
 
     if stream is None:
         stream = cupy.cuda.get_current_stream()
@@ -215,13 +210,12 @@
 
     if invocation_index != NO_ERROR:
         invoked_kernel = contexts[int(invocation_index // math.pow(2, ERROR_BITS))]
         cuda_streamptr_to_contexts[stream.ptr] = (
             cupy.array(NO_ERROR),
             [],
         )
-        raise awkward._errors.wrap_error(
+        raise invoked_kernel.error_context.decorate_exception(
             ValueError(
                 f"{kernel_errors[invoked_kernel.name][int(invocation_index % math.pow(2, ERROR_BITS))]} in compiled CUDA code ({invoked_kernel.name})"
-            ),
-            invoked_kernel.error_context,
+            )
         )
```

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_to_Index64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_global_startstop_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_init.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_contiguous_next.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill_tobool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_boolean_nonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_getitem_next_range_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_broadcast_tooffsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_combinations.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_content_reduce_zeroparents_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_carry_nocheck.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/awkward_regularize_arrayslice.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu` & `awkward-2.1.2/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/header-only/awkward/BuilderOptions.h` & `awkward-2.1.2/src/awkward/_connect/header-only/awkward/BuilderOptions.h`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/header-only/awkward/GrowableBuffer.h` & `awkward-2.1.2/src/awkward/_connect/header-only/awkward/GrowableBuffer.h`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,23 @@
     /// @param reserved Currently allocated number of elements in the panel.
     Panel(std::unique_ptr<PRIMITIVE[]> ptr, size_t length, size_t reserved)
         : ptr_(std::move(ptr)),
           length_(length),
           reserved_(reserved),
           next_(nullptr) {}
 
-    ~Panel() = default;
+    /// @brief Deletes a Panel.
+    ///
+    /// Unchain the pointers to avoid a stack overflow when
+    /// a recursive implicit destructor is invoked.
+    ~Panel() {
+      for (std::unique_ptr<Panel> current = std::move(next_);
+           current;
+           current = std::move(current->next_));
+    }
 
     /// @brief Overloads [] operator to access elements like an array.
     PRIMITIVE& operator[](size_t i) { return ptr_.get()[i]; }
 
     /// @brief Creates a new panel with slots equal to #reserved and
     /// appends it after the current panel.
     Panel*
```

### Comparing `awkward-2.1.1/src/awkward/_connect/header-only/awkward/LayoutBuilder.h` & `awkward-2.1.2/src/awkward/_connect/header-only/awkward/LayoutBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/header-only/awkward/utils.h` & `awkward-2.1.2/src/awkward/_connect/header-only/awkward/utils.h`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/jax/reducers.py` & `awkward-2.1.2/src/awkward/_connect/jax/reducers.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,72 +16,66 @@
 
     @classmethod
     def return_dtype(cls, given_dtype):
         return np.int64
 
     @classmethod
     def apply(cls, array, parents, outlength):
-        raise ak._errors.wrap_error(RuntimeError("Cannot differentiate through argmin"))
+        raise RuntimeError("Cannot differentiate through argmin")
 
 
 class ArgMax(Reducer):
     name = "argmax"
     needs_position = True
     preferred_dtype = np.int64
 
     @classmethod
     def return_dtype(cls, given_dtype):
         return np.int64
 
     @classmethod
     def apply(cls, array, parents, outlength):
-        raise ak._errors.wrap_error(RuntimeError("Cannot differentiate through argmax"))
+        raise RuntimeError("Cannot differentiate through argmax")
 
 
 class Count(Reducer):
     name = "count"
     preferred_dtype = np.float64
 
     @classmethod
     def return_dtype(cls, given_dtype):
         return np.int64
 
     @classmethod
     def apply(cls, array, parents, outlength):
-        raise ak._errors.wrap_error(
-            RuntimeError("Cannot differentiate through count_zero")
-        )
+        raise RuntimeError("Cannot differentiate through count_zero")
 
 
 class CountNonzero(Reducer):
     name = "count_nonzero"
     preferred_dtype = np.float64
 
     @classmethod
     def return_dtype(cls, given_dtype):
         return np.int64
 
     @classmethod
     def apply(cls, array, parents, outlength):
-        raise ak._errors.wrap_error(
-            RuntimeError("Cannot differentiate through count_nonzero")
-        )
+        raise RuntimeError("Cannot differentiate through count_nonzero")
 
 
 class Sum(Reducer):
     name = "sum"
     preferred_dtype = np.float64
 
     @classmethod
     def apply(cls, array, parents, outlength):
         assert isinstance(array, ak.contents.NumpyArray)
         if array.dtype.kind == "M":
-            raise ak._errors.wrap_error(
-                TypeError(f"cannot compute the sum (ak.sum) of {array.dtype!r}")
-            )
+            raise TypeError(f"cannot compute the sum (ak.sum) of {array.dtype!r}")
 
         result = jax.ops.segment_sum(array.data, parents.data)
 
         if array.dtype.kind == "m":
             return ak.contents.NumpyArray(
                 array.backend.nplike.asarray(result, dtype=array.dtype)
             )
```

### Comparing `awkward-2.1.1/src/awkward/_connect/jax/trees.py` & `awkward-2.1.2/src/awkward/_connect/jax/trees.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,21 @@
 from __future__ import annotations
 
 import jax
 
 import awkward as ak
 from awkward import contents, highlevel, record
 from awkward._behavior import behavior_of
-from awkward._errors import wrap_error
 from awkward._layout import wrap_layout
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import NumpyMetadata
+from awkward._typing import Generic, TypeVar, Union
 from awkward.contents import Content
 from awkward.record import Record
-from awkward.typing import Generic, TypeVar, Union
 
 numpy = Numpy.instance()
 np = NumpyMetadata.instance()
 
 
 def find_all_buffers(
     layout: Content | Record,
@@ -75,15 +74,15 @@
     def from_array_or_layout(cls, obj: T):
         is_highlevel = isinstance(obj, (highlevel.Array, highlevel.Record))
         if is_highlevel:
             layout = obj.layout
         elif isinstance(obj, (contents.Content, record.Record)):
             layout = obj
         else:
-            raise wrap_error(TypeError)
+            raise TypeError
 
         # First, make sure we're all JAX
         jax_backend = ak._backends.JaxBackend.instance()
         layout = layout.to_backend(jax_backend)
 
         # Now pull out the Jax tracers / arrays
         buffers = find_all_buffers(layout)
@@ -127,21 +126,19 @@
         return self._is_highlevel
 
     def unflatten(self, buffers: tuple) -> T:
         for buffer in buffers:
             # Check that JAX isn't trying to give us float0 types
             dtype = getattr(buffer, "dtype", None)
             if dtype == np.dtype([("float0", "V")]):
-                raise wrap_error(
-                    TypeError(
-                        f"a buffer with the dtype {buffer.dtype} was encountered during unflattening. "
-                        "JAX uses this dtype for the tangents of integer/boolean outputs; these cannot "
-                        "reasonably be differentiated. Make sure that you are not computing the derivative "
-                        "of a boolean/integer (array) valued function."
-                    )
+                raise TypeError(
+                    f"a buffer with the dtype {buffer.dtype} was encountered during unflattening. "
+                    "JAX uses this dtype for the tangents of integer/boolean outputs; these cannot "
+                    "reasonably be differentiated. Make sure that you are not computing the derivative "
+                    "of a boolean/integer (array) valued function."
                 )
 
         # Replace the mixed NumPy-JAX layout leaves with the given buffers (and use the JAX nplike)
         layout = replace_all_buffers(
             self._layout, list(buffers), backend=ak._backends.JaxBackend.instance()
         )
         return wrap_layout(
```

### Comparing `awkward-2.1.1/src/awkward/_connect/numba/arrayview.py` & `awkward-2.1.2/src/awkward/_connect/numba/arrayview.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/numba/arrayview_cuda.py` & `awkward-2.1.2/src/awkward/_connect/numba/arrayview_cuda.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,15 @@
                 stop = val._numbaview.stop
                 pos = val._numbaview.pos
                 arrayptrs = val._numbaview.lookup.arrayptrs.data.ptr
                 pylookup = 0
 
                 return tys, (pos, start, stop, arrayptrs, pylookup)
             else:
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        '`ak.to_backend` should be called with `backend="cuda"` to put '
-                        "the array on the GPU before using it: "
-                        'ak.to_backend(array, backend="cuda")'
-                    )
+                raise TypeError(
+                    '`ak.to_backend` should be called with `backend="cuda"` to put '
+                    "the array on the GPU before using it: "
+                    'ak.to_backend(array, backend="cuda")'
                 )
 
         else:
             return ty, val
```

### Comparing `awkward-2.1.1/src/awkward/_connect/numba/builder.py` & `awkward-2.1.2/src/awkward/_connect/numba/builder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_connect/numba/layout.py` & `awkward-2.1.2/src/awkward/_connect/numba/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,17 +94,15 @@
         elif arraytype.dtype.bitwidth == 32 and arraytype.dtype.signed:
             return ak.index.Index32
         elif arraytype.dtype.bitwidth == 32:
             return ak.index.IndexU32
         elif arraytype.dtype.bitwidth == 64:
             return ak.index.Index64
         else:
-            raise ak._errors.wrap_error(
-                AssertionError(f"no Index* type for array: {arraytype}")
-            )
+            raise AssertionError(f"no Index* type for array: {arraytype}")
 
     def getitem_at_check(self, viewtype):
         typer = find_numba_array_typer(viewtype.type, viewtype.behavior)
         if typer is None:
             return self.getitem_at(viewtype)
         else:
             return typer(viewtype)
```

### Comparing `awkward-2.1.1/src/awkward/_connect/rdataframe/from_rdataframe.py` & `awkward-2.1.2/src/awkward/_connect/rdataframe/from_rdataframe.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,19 +49,17 @@
         os.path.join(
             os.path.dirname(os.path.realpath(__file__)),
             os.path.pardir,
             "header-only",
         )
     )
 )
-compiler = ROOT.gInterpreter.Declare
 
 
-done = compiler('\n#include "rdataframe/jagged_builders.h"\n')
-assert done is True
+cppyy.include("rdataframe/jagged_builders.h")
 
 
 def from_rdataframe(
     data_frame, columns, highlevel, behavior, with_name, offsets_type, keep_order
 ):
     def cpp_builder_type(depth, data_type):
         if depth == 1:
@@ -122,14 +120,15 @@
             return form_dtype(form.content)
 
     # Register Take action for each column
     # 'Take' is a lazy action:
     column_types = {}
     result_ptrs = {}
     contents = {}
+    index = {}
     awkward_type_cols = {}
 
     columns = (*columns, "rdfentry_")
     maybe_indexed = keep_order
 
     # Important note: This loop is separate from the next one
     # in order not to trigger the additional RDataFrame
@@ -156,18 +155,16 @@
             layout = generator.tolayout(lookup[col], 0, ())
             awkward_type_cols[col] = layout
 
         else:  # Convert the C++ vectors to Awkward arrays
             form_str = ROOT.awkward.type_to_form[column_types[col], offsets_type](0)
 
             if form_str == "unsupported type":
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        f"{col!r} column's type {column_types[col]!r} is not supported."
-                    )
+                raise TypeError(
+                    f"{col!r} column's type {column_types[col]!r} is not supported."
                 )
 
             form = ak.forms.from_json(form_str)
 
             list_depth = form.purelist_depth
             form_dtype_name = form_dtype(form).name
             data_type = cpp_type_of[form_dtype_name]
@@ -208,50 +205,56 @@
                 fill_from_func = getattr(
                     cppyy.gbl.awkward, f"fill_offsets_and_flatten{list_depth}"
                 )
                 fill_from_func[builder_type, column_types[col]](
                     builder, result_ptrs[col]
                 )
             else:
-                raise ak._errors.wrap_error(
-                    AssertionError(f"unrecognized Form: {type(form)}")
-                )
+                raise AssertionError(f"unrecognized Form: {type(form)}")
 
             names_nbytes = cpp_buffers_self.names_nbytes[builder_type](builder)
 
             buffers = {}
             for item in names_nbytes:
                 buffers[item.first] = numpy.empty(item.second, dtype=np.uint8)
                 cpp_buffers_self.append(
                     item.first,
                     buffers[item.first].ctypes.data_as(ctypes.POINTER(ctypes.c_ubyte)),
                 )
 
             length = cpp_buffers_self.to_char_buffers[builder_type](builder)
 
-            contents[col] = ak.from_buffers(
-                form,
-                length,
-                buffers,
-                byteorder=ak._util.native_byteorder,
-                highlevel=highlevel,
-                behavior=behavior,
-            )
-
             if col == "rdfentry_":
-                contents[col] = ak.index.Index64(
-                    contents[col].layout.to_backend_array(
+                index[col] = ak.from_buffers(
+                    form,
+                    length,
+                    buffers,
+                    byteorder=ak._util.native_byteorder,
+                    highlevel=highlevel,
+                    behavior=behavior,
+                )
+                index[col] = ak.index.Index64(
+                    index[col].layout.to_backend_array(
                         allow_missing=True, backend=ak._backends.NumpyBackend.instance()
                     )
                 )
+            else:
+                contents[col] = ak.from_buffers(
+                    form,
+                    length,
+                    buffers,
+                    byteorder=ak._util.native_byteorder,
+                    highlevel=highlevel,
+                    behavior=behavior,
+                )
 
     for key, value in awkward_type_cols.items():
-        if len(contents["rdfentry_"]) < len(value):
+        if len(index["rdfentry_"]) < len(value):
             contents[key] = wrap_layout(
-                ak.contents.IndexedArray(contents["rdfentry_"], value),
+                ak.contents.IndexedArray(index["rdfentry_"], value),
                 highlevel=highlevel,
                 behavior=behavior,
             )
         else:
             contents[key] = value
 
     out = ak.zip(
@@ -259,18 +262,15 @@
         depth_limit=1,
         highlevel=highlevel,
         behavior=behavior,
         with_name=with_name,
     )
 
     if keep_order:
-        sorted = ak.index.Index64(contents["rdfentry_"].data.argsort())
+        sorted = ak.index.Index64(index["rdfentry_"].data.argsort())
         out = wrap_layout(
             ak.contents.IndexedArray(sorted, out.layout),
             highlevel=highlevel,
             behavior=behavior,
         )
 
-    if maybe_indexed:
-        del contents["rdfentry_"]
-
     return out
```

### Comparing `awkward-2.1.1/src/awkward/_connect/rdataframe/to_rdataframe.py` & `awkward-2.1.2/src/awkward/_connect/rdataframe/to_rdataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,20 @@
         array_data_source = self.class_type()
 
         if self.use_cached:
             cpp_code = cache.get(array_data_source)
         else:
             cpp_code = None
 
+        init_method = (
+            "Initialize"
+            if hasattr(ROOT.RDF.RDataSource, "Initialize")
+            else "Initialise"
+        )
+
         if cpp_code is None:
             cpp_code = f"""
 namespace awkward {{
 
     class {array_data_source} final
       : public ROOT::RDF::RDataSource {{
     private:
@@ -254,15 +260,15 @@
 
         void SetNSlots(unsigned int nSlots) {{
             fNSlots = nSlots;
 
             {cpp_code_resize_slots}
         }}
 
-        void Initialise() {{
+        void {init_method}() {{
             // initialize fEntryRanges
             const auto chunkSize = fSize / fNSlots;
             auto start = 0UL;
             auto end = 0UL;
             for (auto i : ROOT::TSeqUL(fNSlots)) {{
                 start = end;
                 end += chunkSize;
```

### Comparing `awkward-2.1.1/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h` & `awkward-2.1.2/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/_nplikes/__init__.py` & `awkward-2.1.2/src/awkward/_nplikes/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from collections.abc import Collection
 
-import awkward as ak
-from awkward.typing import TYPE_CHECKING, TypeVar
+from awkward._typing import TYPE_CHECKING, TypeVar
 
 if TYPE_CHECKING:
     from awkward._nplikes.numpylike import ArrayLike, NumpyLike
 
 # Temporary sentinel marking "argument not given"
 _UNSET = object()
 
@@ -27,19 +26,17 @@
         return next(iter(nplikes))
     else:
         # We allow typetracers to mix with other nplikes, and take precedence
         for nplike in nplikes:
             if not nplike.known_data:
                 return nplike
 
-        raise ak._errors.wrap_error(
-            ValueError(
-                "cannot operate on arrays with incompatible array libraries. Use #ak.to_backend to coerce the arrays "
-                "to the same backend"
-            )
+        raise ValueError(
+            "cannot operate on arrays with incompatible array libraries. Use #ak.to_backend to coerce the arrays "
+            "to the same backend"
         )
 
 
 def nplike_of(*arrays, default: D = _UNSET) -> NumpyLike | D:
     """
     Args:
         *arrays: iterable of possible array objects
@@ -90,33 +87,27 @@
     from awkward._nplikes.jax import Jax
     from awkward._nplikes.numpy import Numpy
     from awkward._nplikes.typetracer import TypeTracer
 
     if from_nplike is None:
         from_nplike = nplike_of(array, default=None)
         if from_nplike is None:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    f"internal error: expected an array supported by an existing nplike, got {type(array).__name__!r}"
-                )
+            raise TypeError(
+                f"internal error: expected an array supported by an existing nplike, got {type(array).__name__!r}"
             )
 
     if from_nplike is to_nplike:
         return array
 
     if isinstance(from_nplike, TypeTracer) and nplike is not from_nplike:
-        raise ak._errors.wrap_error(
-            TypeError(
-                "Converting a TypeTracer nplike to an nplike with `known_data=True` is not possible"
-            )
+        raise TypeError(
+            "Converting a TypeTracer nplike to an nplike with `known_data=True` is not possible"
         )
 
     # Copy to host memory
     if isinstance(from_nplike, Cupy):
         array = array.get()
 
     if isinstance(nplike, (Numpy, Cupy, Jax, TypeTracer)):
         return nplike.asarray(array)
     else:
-        raise ak._errors.wrap_error(
-            TypeError(f"internal error: invalid nplike {type(nplike).__name__!r}")
-        )
+        raise TypeError(f"internal error: invalid nplike {type(nplike).__name__!r}")
```

### Comparing `awkward-2.1.1/src/awkward/_nplikes/array_module.py` & `awkward-2.1.2/src/awkward/_nplikes/array_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import math
 
 import numpy
 
-from awkward._errors import wrap_error
 from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyLike, NumpyMetadata
 from awkward._nplikes.shape import ShapeItem, unknown_length
-from awkward.typing import Final, Literal
+from awkward._typing import Final, Literal
 
 np = NumpyMetadata.instance()
 
 
 class ArrayModuleNumpyLike(NumpyLike):
     known_data: Final = True
 
@@ -27,18 +26,16 @@
     ) -> ArrayLike:
         if copy:
             return self._module.array(obj, dtype=dtype, copy=True)
         elif copy is None:
             return self._module.asarray(obj, dtype=dtype)
         else:
             if getattr(obj, "dtype", dtype) != dtype:
-                raise wrap_error(
-                    ValueError(
-                        "asarray was called with copy=False for an array of a different dtype"
-                    )
+                raise ValueError(
+                    "asarray was called with copy=False for an array of a different dtype"
                 )
             else:
                 return self._module.asarray(obj, dtype=dtype)
 
     def ascontiguousarray(
         self, x: ArrayLike, *, dtype: np.dtype | None = None
     ) -> ArrayLike:
@@ -127,28 +124,24 @@
         elif copy:
             return self._module.reshape(self._module.copy(x, order="C"), shape)
         else:
             result = self._module.asarray(x)
             try:
                 result.shape = shape
             except AttributeError:
-                raise wrap_error(
-                    ValueError("cannot reshape array without copying")
-                ) from None
+                raise ValueError("cannot reshape array without copying") from None
             return result
 
     def shape_item_as_index(self, x1: ShapeItem) -> int:
         if x1 is unknown_length:
-            raise wrap_error(
-                TypeError("array module nplikes do not support unknown lengths")
-            )
+            raise TypeError("array module nplikes do not support unknown lengths")
         elif isinstance(x1, int):
             return x1
         else:
-            raise wrap_error(TypeError(f"expected None or int type, received {x1}"))
+            raise TypeError(f"expected None or int type, received {x1}")
 
     def index_as_shape_item(self, x1: IndexType) -> int:
         return int(x1)
 
     def derive_slice_for_length(
         self, slice_: slice, length: ShapeItem
     ) -> tuple[IndexType, IndexType, IndexType, ShapeItem]:
@@ -177,17 +170,15 @@
         """  # We have known length and index
         if index < 0:
             index = index + length
 
         if 0 <= index < length:
             return index
         else:
-            raise wrap_error(
-                IndexError(f"index value out of bounds (0, {length}): {index}")
-            )
+            raise IndexError(f"index value out of bounds (0, {length}): {index}")
 
     def nonzero(self, x: ArrayLike) -> tuple[ArrayLike, ...]:
         return self._module.nonzero(x)
 
     def where(self, condition: ArrayLike, x1: ArrayLike, x2: ArrayLike) -> ArrayLike:
         return self._module.where(condition, x1, x2)
```

### Comparing `awkward-2.1.1/src/awkward/_nplikes/cupy.py` & `awkward-2.1.2/src/awkward/_nplikes/cupy.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,41 +2,37 @@
 from __future__ import annotations
 
 import numpy
 
 import awkward as ak
 from awkward._nplikes.array_module import ArrayModuleNumpyLike
 from awkward._nplikes.numpylike import ArrayLike
-from awkward.typing import Final
+from awkward._typing import Final
 
 
 class Cupy(ArrayModuleNumpyLike):
     is_eager: Final = False
 
     def __init__(self):
         import awkward._connect.cuda  # noqa: F401
 
         self._module = ak._connect.cuda.import_cupy("Awkward Arrays with CUDA")
 
     @property
     def ma(self):
-        raise ak._errors.wrap_error(
-            ValueError(
-                "CUDA arrays cannot have missing values until CuPy implements "
-                "numpy.ma.MaskedArray"
-            )
+        raise ValueError(
+            "CUDA arrays cannot have missing values until CuPy implements "
+            "numpy.ma.MaskedArray"
         )
 
     @property
     def char(self):
-        raise ak._errors.wrap_error(
-            ValueError(
-                "CUDA arrays cannot do string manipulations until CuPy implements "
-                "numpy.char"
-            )
+        raise ValueError(
+            "CUDA arrays cannot do string manipulations until CuPy implements "
+            "numpy.char"
         )
 
     @property
     def ndarray(self):
         return self._module.ndarray
 
     def frombuffer(
@@ -51,17 +47,15 @@
         else:
             return self._module.all(x1 - x2 == 0)
 
     def repeat(
         self, x: ArrayLike, repeats: ArrayLike | int, *, axis: int | None = None
     ):
         if axis is not None:
-            raise ak._errors.wrap_error(
-                NotImplementedError(f"repeat for CuPy with axis={axis!r}")
-            )
+            raise NotImplementedError(f"repeat for CuPy with axis={axis!r}")
         # https://github.com/cupy/cupy/issues/3849
         if isinstance(repeats, self._module.ndarray):
             all_stops = self._module.cumsum(repeats)
             parents = self._module.zeros(all_stops[-1].item(), dtype=int)
             stops, stop_counts = self._module.unique(all_stops[:-1], return_counts=True)
             parents[stops] = stop_counts
             self._module.cumsum(parents, out=parents)
```

### Comparing `awkward-2.1.1/src/awkward/_nplikes/jax.py` & `awkward-2.1.2/src/awkward/_nplikes/jax.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,40 +2,36 @@
 from __future__ import annotations
 
 import numpy
 
 import awkward as ak
 from awkward._nplikes.array_module import ArrayModuleNumpyLike
 from awkward._nplikes.numpylike import ArrayLike
-from awkward.typing import Final
+from awkward._typing import Final
 
 
 class Jax(ArrayModuleNumpyLike):
     is_eager: Final = True
 
     def __init__(self):
         jax = ak.jax.import_jax()
         self._module = jax.numpy
 
     @property
     def ma(self):
-        raise ak._errors.wrap_error(
-            ValueError(
-                "JAX arrays cannot have missing values until JAX implements "
-                "numpy.ma.MaskedArray"
-            )
+        raise ValueError(
+            "JAX arrays cannot have missing values until JAX implements "
+            "numpy.ma.MaskedArray"
         )
 
     @property
     def char(self):
-        raise ak._errors.wrap_error(
-            ValueError(
-                "JAX arrays cannot do string manipulations until JAX implements "
-                "numpy.char"
-            )
+        raise ValueError(
+            "JAX arrays cannot do string manipulations until JAX implements "
+            "numpy.char"
         )
 
     @property
     def ndarray(self):
         return self._module.ndarray
 
     @classmethod
```

### Comparing `awkward-2.1.1/src/awkward/_nplikes/numpy.py` & `awkward-2.1.2/src/awkward/_nplikes/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 import numpy
 
 import awkward as ak
 from awkward._nplikes.array_module import ArrayModuleNumpyLike
 from awkward._nplikes.numpylike import ArrayLike, NumpyMetadata
-from awkward.typing import Final, Literal
+from awkward._typing import Final, Literal
 
 np = NumpyMetadata.instance()
 
 
 class Numpy(ArrayModuleNumpyLike):
     is_eager: Final = True
```

### Comparing `awkward-2.1.1/src/awkward/_nplikes/numpylike.py` & `awkward-2.1.2/src/awkward/_nplikes/numpylike.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from abc import abstractmethod
 
 import numpy
 
 from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._singleton import Singleton
-from awkward.typing import (
+from awkward._typing import (
     Literal,
     Protocol,
     Self,
     SupportsIndex,
     TypeAlias,
     overload,
 )
```

### Comparing `awkward-2.1.1/src/awkward/_nplikes/shape.py` & `awkward-2.1.2/src/awkward/_nplikes/shape.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
-from awkward.typing import Self, TypeAlias
+from awkward._typing import Self, TypeAlias
 
 ShapeItem: TypeAlias = "int | _UnknownLength"
 
 
 class _UnknownLength:
     _name: str
 
     @classmethod
     def _new(cls, name: str) -> Self:
         self = super().__new__(cls)
         self._name = name
         return self
 
     def __new__(cls, *args, **kwargs):
-        from awkward._errors import wrap_error
-
-        raise wrap_error(
-            TypeError(
-                "internal_error: the `TypeTracer` nplike's `TypeTracerArray` object should never be directly instantiated"
-            )
+        raise TypeError(
+            "internal_error: the `TypeTracer` nplike's `TypeTracerArray` object should never be directly instantiated"
         )
 
     def __add__(self, other) -> Self | NotImplemented:
         if isinstance(other, int) or other is self:
             return self
         else:
             return NotImplemented
@@ -63,41 +59,27 @@
     def __str__(self) -> str:
         return "##"
 
     def __repr__(self):
         return f"{__name__}.{self._name}"
 
     def __eq__(self, other) -> bool:
-        from awkward._errors import wrap_error
-
         if other is self:
             return True
         else:
-            raise wrap_error(
-                TypeError("cannot compare unknown lengths against known values")
-            )
+            raise TypeError("cannot compare unknown lengths against known values")
 
     def __gt__(self, other):
-        from awkward._errors import wrap_error
-
-        raise wrap_error(TypeError("cannot order unknown lengths"))
+        raise TypeError("cannot order unknown lengths")
 
     def __index__(self):  # pylint: disable=invalid-index-returned
-        from awkward._errors import wrap_error
-
-        raise wrap_error(
-            TypeError("cannot interpret unknown lengths as concrete index values")
-        )
+        raise TypeError("cannot interpret unknown lengths as concrete index values")
 
     def __int__(self):
-        from awkward._errors import wrap_error
-
-        raise wrap_error(
-            TypeError("cannot interpret unknown lengths as concrete values")
-        )
+        raise TypeError("cannot interpret unknown lengths as concrete values")
 
     __bool__ = __int__
     __float__ = __int__
 
     __ge__ = __gt__
     __le__ = __gt__
     __lt__ = __gt__
```

### Comparing `awkward-2.1.1/src/awkward/_nplikes/typetracer.py` & `awkward-2.1.2/src/awkward/_nplikes/typetracer.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 
 from numbers import Number
 
 import numpy
 from numpy.lib.mixins import NDArrayOperatorsMixin
 
 import awkward as ak
-from awkward._errors import wrap_error
 from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyLike, NumpyMetadata
 from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._regularize import is_integer, is_non_string_like_sequence
-from awkward.typing import (
+from awkward._typing import (
     Any,
     Final,
     Literal,
     Self,
     SupportsIndex,
     TypeVar,
 )
@@ -186,17 +185,15 @@
         layout.tags.data.report = report
         layout.index.data.form_key = form.form_key
         layout.index.data.report = report
         for x, y in zip(layout.contents, form.contents):
             _attach_report(x, y, report)
 
     else:
-        raise ak._errors.wrap_error(
-            AssertionError(f"unrecognized layout type {type(layout)}")
-        )
+        raise AssertionError(f"unrecognized layout type {type(layout)}")
 
 
 def typetracer_with_report(form, forget_length=True):
     layout = form.length_zero_array(highlevel=False).to_typetracer(
         forget_length=forget_length
     )
     report = TypeTracerReport()
@@ -205,18 +202,16 @@
 
 
 class TypeTracerArray(NDArrayOperatorsMixin, ArrayLike):
     _dtype: numpy.dtype
     _shape: tuple[ShapeItem, ...]
 
     def __new__(cls, *args, **kwargs):
-        raise wrap_error(
-            TypeError(
-                "internal_error: the `TypeTracer` nplike's `TypeTracerArray` object should never be directly instantiated"
-            )
+        raise TypeError(
+            "internal_error: the `TypeTracer` nplike's `TypeTracerArray` object should never be directly instantiated"
         )
 
     def __reduce__(self):
         # Fix pickling, as we ban `__new__`
         return object.__new__, (type(self),), vars(self)
 
     @classmethod
@@ -228,19 +223,17 @@
         report: TypeTracerReport | None = None,
     ):
         self = super().__new__(cls)
         self.form_key = form_key
         self.report = report
 
         if not isinstance(shape, tuple):
-            raise wrap_error(TypeError("typetracer shape must be a tuple"))
+            raise TypeError("typetracer shape must be a tuple")
         if any(is_unknown_scalar(x) for x in shape):
-            raise wrap_error(
-                TypeError("typetracer shape must be integers or unknown-length")
-            )
+            raise TypeError("typetracer shape must be integers or unknown-length")
         self._shape = shape
         self._dtype = np.dtype(dtype)
 
         return self
 
     def __repr__(self):
         dtype = repr(self._dtype)
@@ -282,27 +275,25 @@
     @property
     def form_key(self):
         return self._form_key
 
     @form_key.setter
     def form_key(self, value):
         if value is not None and not isinstance(value, str):
-            raise ak._errors.wrap_error(TypeError("form_key must be None or a string"))
+            raise TypeError("form_key must be None or a string")
         self._form_key = value
 
     @property
     def report(self):
         return self._report
 
     @report.setter
     def report(self, value):
         if value is not None and not isinstance(value, TypeTracerReport):
-            raise ak._errors.wrap_error(
-                TypeError("report must be None or a TypeTracerReport")
-            )
+            raise TypeError("report must be None or a TypeTracerReport")
         self._report = value
 
     def touch_shape(self):
         if self._report is not None:
             self._report.touch_shape(self._form_key)
 
     def touch_data(self):
@@ -348,43 +339,37 @@
             self._dtype,
             (unknown_length,) + self._shape[1:],
             self._form_key,
             self._report,
         )
 
     def __iter__(self):
-        raise ak._errors.wrap_error(
-            AssertionError(
-                "bug in Awkward Array: attempt to convert TypeTracerArray into a concrete array"
-            )
+        raise AssertionError(
+            "bug in Awkward Array: attempt to convert TypeTracerArray into a concrete array"
         )
 
     def __array__(self, dtype=None):
-        raise ak._errors.wrap_error(
-            AssertionError(
-                "bug in Awkward Array: attempt to convert TypeTracerArray into a concrete array"
-            )
+        raise AssertionError(
+            "bug in Awkward Array: attempt to convert TypeTracerArray into a concrete array"
         )
 
     @property
     def itemsize(self):
         return self._dtype.itemsize
 
     class _CTypes:
         data = 0
 
     @property
     def ctypes(self):
         return self._CTypes
 
     def __len__(self):
-        raise ak._errors.wrap_error(
-            AssertionError(
-                "bug in Awkward Array: attempt to get length of a TypeTracerArray"
-            )
+        raise AssertionError(
+            "bug in Awkward Array: attempt to get length of a TypeTracerArray"
         )
 
     def __getitem__(
         self,
         key: SupportsIndex
         | slice
         | Ellipsis
@@ -409,35 +394,29 @@
             ):
                 n_advanced += 1
             # Basic ellipsis
             elif item is Ellipsis:
                 if not has_seen_ellipsis:
                     has_seen_ellipsis = True
                 else:
-                    raise wrap_error(
-                        NotImplementedError(
-                            "only one ellipsis value permitted for advanced index"
-                        )
+                    raise NotImplementedError(
+                        "only one ellipsis value permitted for advanced index"
                     )
             # Basic newaxis
             elif item is np.newaxis:
                 pass
             else:
-                raise wrap_error(
-                    NotImplementedError(
-                        "only integer, unknown scalar, slice, ellipsis, or array indices are permitted"
-                    )
+                raise NotImplementedError(
+                    "only integer, unknown scalar, slice, ellipsis, or array indices are permitted"
                 )
 
         n_dim_index = n_basic_non_ellipsis + n_advanced
         if n_dim_index > self.ndim:
-            raise wrap_error(
-                IndexError(
-                    f"too many indices for array: array is {self.ndim}-dimensional, but {n_dim_index} were indexed"
-                )
+            raise IndexError(
+                f"too many indices for array: array is {self.ndim}-dimensional, but {n_dim_index} were indexed"
             )
 
         # 2. Normalise Ellipsis and boolean arrays
         key_parts = []
         for item in key:
             if item is Ellipsis:
                 # How many more dimensions do we have than the index provides
@@ -497,17 +476,15 @@
                 elif isinstance(item, int) or is_unknown_integer(item):
                     item = self.nplike.promote_scalar(item)
 
                     if is_unknown_length(dimension_length) or is_unknown_integer(item):
                         continue
 
                     if not 0 <= item < dimension_length:
-                        raise wrap_error(
-                            NotImplementedError("integer index out of bounds")
-                        )
+                        raise NotImplementedError("integer index out of bounds")
 
         advanced_shape = self.nplike.broadcast_shapes(*advanced_shapes)
         if advanced_is_at_front:
             result_shape_parts.insert(0, advanced_shape)
         else:
             adjacent_advanced_shape[:] = advanced_shape
 
@@ -528,45 +505,43 @@
         | Ellipsis
         | tuple[SupportsIndex | slice | Ellipsis | ArrayLike, ...]
         | ArrayLike,
         value: int | float | bool | complex | ArrayLike,
     ):
         existing_value = self.__getitem__(key)
         if isinstance(value, TypeTracerArray) and value.ndim > existing_value.ndim:
-            raise wrap_error(ValueError("cannot assign shape larger than destination"))
+            raise ValueError("cannot assign shape larger than destination")
 
     def copy(self):
         self.touch_data()
         return self
 
     def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
         # raise ak._errors.wrap_error(
         #     RuntimeError(
         #         "TypeTracerArray objects should not be used directly with ufuncs"
         #     )
         # )
         kwargs.pop("out", None)
 
         if method != "__call__" or len(inputs) == 0:
-            raise ak._errors.wrap_error(NotImplementedError)
+            raise NotImplementedError
 
         if len(kwargs) > 0:
-            raise ak._errors.wrap_error(
-                ValueError("TypeTracerArray does not support kwargs for ufuncs")
-            )
+            raise ValueError("TypeTracerArray does not support kwargs for ufuncs")
         return self.nplike._apply_ufunc(ufunc, *inputs)
 
     def __bool__(self) -> bool:
-        raise ak._errors.wrap_error(RuntimeError("cannot realise an unknown value"))
+        raise RuntimeError("cannot realise an unknown value")
 
     def __int__(self) -> int:
-        raise ak._errors.wrap_error(RuntimeError("cannot realise an unknown value"))
+        raise RuntimeError("cannot realise an unknown value")
 
     def __index__(self) -> int:
-        raise ak._errors.wrap_error(RuntimeError("cannot realise an unknown value"))
+        raise RuntimeError("cannot realise an unknown value")
 
 
 def _scalar_type_of(obj) -> numpy.dtype:
     if is_unknown_scalar(obj):
         return obj.dtype
     else:
         return numpy.obj2sctype(obj)
@@ -598,28 +573,28 @@
             return TypeTracerArray._new(result.dtype, shape=broadcasted[0].shape)
         elif isinstance(result, tuple):
             return (
                 TypeTracerArray._new(x.dtype, shape=b.shape)
                 for x, b in zip(result, broadcasted)
             )
         else:
-            raise wrap_error(TypeError)
+            raise TypeError
 
     def _axis_is_valid(self, axis: int, ndim: int) -> bool:
         if axis < 0:
             axis = axis + ndim
         return 0 <= axis < ndim
 
     @property
     def ma(self):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @property
     def char(self):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @property
     def ndarray(self):
         return TypeTracerArray
 
     ############################ array creation
 
@@ -638,67 +613,99 @@
         if isinstance(obj, TypeTracerArray):
             form_key = obj._form_key
             report = obj._report
 
             if dtype is None:
                 return obj
             elif copy is False and dtype != obj.dtype:
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "asarray was called with copy=False for an array of a different dtype"
-                    )
+                raise ValueError(
+                    "asarray was called with copy=False for an array of a different dtype"
                 )
             else:
                 return TypeTracerArray._new(
                     dtype, obj.shape, form_key=form_key, report=report
                 )
         else:
             # Convert NumPy generics to scalars
             if isinstance(obj, np.generic):
                 obj = numpy.asarray(obj)
 
             # Support array-like objects
             if hasattr(obj, "shape") and hasattr(obj, "dtype"):
                 if obj.dtype.kind == "S":
-                    raise ak._errors.wrap_error(
-                        TypeError("TypeTracerArray cannot be created from strings")
-                    )
+                    raise TypeError("TypeTracerArray cannot be created from strings")
                 elif copy is False and dtype != obj.dtype:
-                    raise ak._errors.wrap_error(
-                        ValueError(
-                            "asarray was called with copy=False for an array of a different dtype"
-                        )
+                    raise ValueError(
+                        "asarray was called with copy=False for an array of a different dtype"
                     )
                 else:
                     return TypeTracerArray._new(obj.dtype, obj.shape)
             # Python objects
             elif isinstance(obj, (Number, bool)):
                 as_array = numpy.asarray(obj)
                 return TypeTracerArray._new(as_array.dtype, ())
 
             elif is_non_string_like_sequence(obj):
-                assert not any(is_non_string_like_sequence(x) for x in obj)
-                shape = (len(obj),)
-                result_type = numpy.result_type(*obj)  # TODO: result_type
-                return TypeTracerArray._new(result_type, shape)
+                shape = []
+                flat_items = []
+                has_seen_leaf = False
+
+                # DFS walk into sequence, construct shape, then validate
+                # remainder of the sequence against this shape.
+                def populate_shape_and_items(node, dim):
+                    nonlocal has_seen_leaf
+
+                    # If we've already computed the shape,
+                    # ensure this item matches!
+                    if has_seen_leaf:
+                        if len(node) != shape[dim - 1]:
+                            raise ValueError(
+                                f"sequence at dimension {dim} does not match shape {shape[dim-1]}"
+                            )
+                    else:
+                        shape.append(len(node))
+
+                    if isinstance(node, TypeTracerArray):
+                        raise AssertionError(
+                            "typetracer arrays inside sequences not currently supported"
+                        )
+                    # Found leaf!
+                    elif len(node) == 0 or not is_non_string_like_sequence(node[0]):
+                        has_seen_leaf = True
+                        flat_items.extend(
+                            [
+                                item.dtype if is_unknown_scalar(item) else item
+                                for item in node
+                            ]
+                        )
+
+                    # Keep recursing!
+                    else:
+                        for child in node:
+                            populate_shape_and_items(child, dim + 1)
+
+                populate_shape_and_items(obj, 1)
+                if dtype is None:
+                    dtype = numpy.result_type(*flat_items)
+                return TypeTracerArray._new(dtype, shape=tuple(shape))
             else:
-                raise wrap_error(TypeError)
+                raise TypeError
 
     def ascontiguousarray(
         self, x: ArrayLike, *, dtype: numpy.dtype | None = None
     ) -> TypeTracerArray:
         try_touch_data(x)
         return TypeTracerArray._new(dtype or x.dtype, shape=x.shape)
 
     def frombuffer(
         self, buffer, *, dtype: np.dtype | None = None, count: int = -1
     ) -> TypeTracerArray:
         for x in (buffer, count):
             try_touch_data(x)
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def zeros(
         self, shape: ShapeItem | tuple[ShapeItem, ...], *, dtype: np.dtype | None = None
     ) -> TypeTracerArray:
         if not isinstance(shape, tuple):
             shape = (shape,)
         return TypeTracerArray._new(dtype, shape)
@@ -811,37 +818,37 @@
             not (
                 is_unknown_length(x.size)
                 or sorter is None
                 or is_unknown_length(sorter.size)
             )
             and x.size != sorter.size
         ):
-            raise wrap_error(ValueError("x.size should equal sorter.size"))
+            raise ValueError("x.size should equal sorter.size")
 
         return TypeTracerArray._new(x.dtype, (values.size,))
 
     ############################ manipulation
 
     def promote_scalar(self, obj) -> TypeTracerArray:
         if is_unknown_scalar(obj):
             return obj
         elif isinstance(obj, (Number, bool)):
             # TODO: statically define these types for all nplikes
             as_array = numpy.asarray(obj)
             return TypeTracerArray._new(as_array.dtype, ())
         else:
-            raise wrap_error(TypeError(f"expected scalar type, received {obj}"))
+            raise TypeError(f"expected scalar type, received {obj}")
 
     def shape_item_as_index(self, x1: ShapeItem) -> IndexType:
         if x1 is unknown_length:
             return TypeTracerArray._new(np.int64, shape=())
         elif isinstance(x1, int):
             return x1
         else:
-            raise wrap_error(TypeError(f"expected None or int type, received {x1}"))
+            raise TypeError(f"expected None or int type, received {x1}")
 
     def index_as_shape_item(self, x1: IndexType) -> ShapeItem:
         if is_unknown_scalar(x1) and np.issubdtype(x1.dtype, np.integer):
             return unknown_length
         else:
             return int(x1)
 
@@ -867,17 +874,15 @@
         # We have known length and index
         if index < 0:
             index = index + length
 
         if 0 <= index < length:
             return index
         else:
-            raise wrap_error(
-                IndexError(f"index value out of bounds (0, {length}): {index}")
-            )
+            raise IndexError(f"index value out of bounds (0, {length}): {index}")
 
     def derive_slice_for_length(
         self, slice_: slice, length: ShapeItem
     ) -> tuple[IndexType, IndexType, IndexType, ShapeItem]:
         """
         Args:
             slice_: normalized slice object
@@ -972,18 +977,16 @@
                 # Item is broadcastable, take existing
                 elif item == 1:
                     continue
                 # Existing is broadcastable, take it
                 elif result[i] == 1:
                     result[i] = item
                 else:
-                    raise wrap_error(
-                        ValueError(
-                            "known component of shape does not match broadcast result"
-                        )
+                    raise ValueError(
+                        "known component of shape does not match broadcast result"
                     )
         return tuple(result)
 
     def broadcast_arrays(self, *arrays: ArrayLike) -> list[TypeTracerArray]:
         for x in arrays:
             try_touch_data(x)
 
@@ -1000,15 +1003,15 @@
         shape = self.broadcast_shapes(*shapes)
 
         return [TypeTracerArray._new(x.dtype, shape=shape) for x in all_arrays]
 
     def broadcast_to(
         self, x: ArrayLike, shape: tuple[ShapeItem, ...]
     ) -> TypeTracerArray:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def reshape(
         self, x: ArrayLike, shape: tuple[ShapeItem, ...], *, copy: bool | None = None
     ) -> TypeTracerArray:
         x.touch_shape()
 
         size = x.size
@@ -1017,27 +1020,25 @@
         n_placeholders = 0
         new_size = 1
         for item in shape:
             if item is unknown_length:
                 # Size is no longer defined
                 new_size = unknown_length
             elif not is_integer(item):
-                raise wrap_error(
-                    ValueError(
-                        "shape must be comprised of positive integers, -1 (for placeholders), or unknown lengths"
-                    )
+                raise ValueError(
+                    "shape must be comprised of positive integers, -1 (for placeholders), or unknown lengths"
                 )
             elif item == -1:
                 if n_placeholders == 1:
-                    raise wrap_error(
-                        ValueError("only one placeholder dimension permitted per shape")
+                    raise ValueError(
+                        "only one placeholder dimension permitted per shape"
                     )
                 n_placeholders += 1
             elif item == 0:
-                raise wrap_error(ValueError("shape items cannot be zero"))
+                raise ValueError("shape items cannot be zero")
             else:
                 new_size *= item
 
         # Populate placeholders
         new_shape = [*shape]
         for i, item in enumerate(shape):
             if item == -1:
@@ -1076,87 +1077,83 @@
         try_touch_data(x)
         return TypeTracerArray._new(x.dtype, shape=(unknown_length,))
 
     def concat(self, arrays, *, axis: int | None = 0) -> TypeTracerArray:
         if axis is None:
             assert all(x.ndim == 1 for x in arrays)
         elif axis != 0:
-            raise ak._errors.wrap_error(NotImplementedError("concat with axis != 0"))
+            raise NotImplementedError("concat with axis != 0")
         for x in arrays:
             try_touch_data(x)
 
         inner_shape = None
         emptyarrays = []
         for x in arrays:
             if inner_shape is None:
                 inner_shape = x.shape[1:]
             elif inner_shape != x.shape[1:]:
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "inner dimensions don't match in concatenate: {} vs {}".format(
-                            inner_shape, x.shape[1:]
-                        )
+                raise ValueError(
+                    "inner dimensions don't match in concatenate: {} vs {}".format(
+                        inner_shape, x.shape[1:]
                     )
                 )
             emptyarrays.append(_emptyarray(x))
 
         if inner_shape is None:
-            raise ak._errors.wrap_error(
-                ValueError("need at least one array to concatenate")
-            )
+            raise ValueError("need at least one array to concatenate")
 
         return TypeTracerArray._new(
             numpy.concatenate(emptyarrays).dtype, (unknown_length, *inner_shape)
         )
 
     def repeat(
         self,
         x: ArrayLike,
         repeats: ArrayLike | int,
         *,
         axis: int | None = None,
     ) -> TypeTracerArray:
         try_touch_data(x)
         try_touch_data(repeats)
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def tile(self, x: ArrayLike, reps: int) -> TypeTracerArray:
         try_touch_data(x)
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def stack(
         self,
         arrays: list[ArrayLike] | tuple[ArrayLike, ...],
         *,
         axis: int = 0,
     ) -> TypeTracerArray:
         for x in arrays:
             try_touch_data(x)
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def packbits(
         self,
         x: ArrayLike,
         *,
         axis: int | None = None,
         bitorder: Literal["big", "little"] = "big",
     ) -> TypeTracerArray:
         try_touch_data(x)
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def unpackbits(
         self,
         x: ArrayLike,
         *,
         axis: int | None = None,
         count: int | None = None,
         bitorder: Literal["big", "little"] = "big",
     ) -> TypeTracerArray:
         try_touch_data(x)
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     ############################ ufuncs
 
     def add(
         self,
         x1: ArrayLike,
         x2: ArrayLike,
@@ -1241,57 +1238,57 @@
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> TypeTracerArray:
         try_touch_data(x)
         if axis is None:
             return TypeTracerArray._new(np.bool_, shape=())
         else:
-            raise ak._errors.wrap_error(NotImplementedError)
+            raise NotImplementedError
 
     def any(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> TypeTracerArray:
         try_touch_data(x)
         if axis is None:
             return TypeTracerArray._new(np.bool_, shape=())
         else:
-            raise ak._errors.wrap_error(NotImplementedError)
+            raise NotImplementedError
 
     def count_nonzero(
         self, x: ArrayLike, *, axis: int | None = None, keepdims: bool = False
     ) -> TypeTracerArray:
         try_touch_data(x)
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def min(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> TypeTracerArray:
         try_touch_data(x)
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def max(
         self,
         x: ArrayLike,
         *,
         axis: int | tuple[int, ...] | None = None,
         keepdims: bool = False,
         maybe_out: ArrayLike | None = None,
     ) -> TypeTracerArray:
         try_touch_data(x)
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def array_str(
         self,
         x: ArrayLike,
         *,
         max_line_width: int | None = None,
         precision: int | None = None,
```

### Comparing `awkward-2.1.1/src/awkward/_nplikes/ufuncs.py` & `awkward-2.1.2/src/awkward/_nplikes/ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/behaviors/categorical.py` & `awkward-2.1.2/src/awkward/behaviors/categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/behaviors/mixins.py` & `awkward-2.1.2/src/awkward/behaviors/mixins.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,17 +84,15 @@
 
     Using this decorator ensures that derived classes that are declared with the
     #ak.mixin_class decorator will also have the behaviors that this class has.
     """
 
     def register(method):
         if not isinstance(rhs, (set, type(None))):
-            raise ak._errors.wrap_error(
-                ValueError("expected a set of right-hand-side argument types")
-            )
+            raise ValueError("expected a set of right-hand-side argument types")
         if transpose and rhs is not None:
             # make a copy of rhs, we will edit it later
             # use partial & a module-scoped function so that this is pickleable
             method._awkward_mixin = (
                 ufunc,
                 set(rhs),
                 functools.partial(_call_transposed, method),
```

### Comparing `awkward-2.1.1/src/awkward/behaviors/string.py` & `awkward-2.1.2/src/awkward/behaviors/string.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,25 +37,21 @@
     def __ne__(self, other):
         return not self.__eq__(self, other)
 
     def __add__(self, other):
         if isinstance(other, (bytes, ByteBehavior)):
             return bytes(self) + bytes(other)
         else:
-            raise ak._errors.wrap_error(
-                TypeError("can only concatenate bytes to bytes")
-            )
+            raise TypeError("can only concatenate bytes to bytes")
 
     def __radd__(self, other):
         if isinstance(other, (bytes, ByteBehavior)):
             return bytes(other) + bytes(self)
         else:
-            raise ak._errors.wrap_error(
-                TypeError("can only concatenate bytes to bytes")
-            )
+            raise TypeError("can only concatenate bytes to bytes")
 
 
 class CharBehavior(Array):
     __name__ = "Array"
 
     def __bytes__(self):
         tmp = self.layout.backend.nplike.asarray(self.layout)
@@ -82,21 +78,21 @@
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __add__(self, other):
         if isinstance(other, (str, CharBehavior)):
             return str(self) + str(other)
         else:
-            raise ak._errors.wrap_error(TypeError("can only concatenate str to str"))
+            raise TypeError("can only concatenate str to str")
 
     def __radd__(self, other):
         if isinstance(other, (str, CharBehavior)):
             return str(other) + str(self)
         else:
-            raise ak._errors.wrap_error(TypeError("can only concatenate str to str"))
+            raise TypeError("can only concatenate str to str")
 
 
 class ByteStringBehavior(Array):
     __name__ = "Array"
 
     def __iter__(self):
         for x in super().__iter__():
@@ -240,14 +236,16 @@
         kind = context.get_constant(numba.types.int32, pyapi.py_unicode_1byte_kind)
         pystr = pyapi.string_from_kind_and_data(kind, strptr, strsize_cast)
     else:
         pystr = pyapi.bytes_from_string_and_size(strptr, strsize_cast)
 
     out = pyapi.to_native_value(rettype, pystr).value
 
+    pyapi.decref(pystr)
+
     pyapi.gil_release(gil)
 
     return out
 
 
 def _cast_bytes_or_str_to_string(string):
     return ak.to_layout([string])
```

### Comparing `awkward-2.1.1/src/awkward/contents/__init__.py` & `awkward-2.1.2/src/awkward/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/contents/bitmaskedarray.py` & `awkward-2.1.2/src/awkward/contents/bitmaskedarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 import math
 
 import awkward as ak
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import MaybeNone, TypeTracer
+from awkward._parameters import (
+    type_parameters_equal,
+)
 from awkward._regularize import is_integer, is_integer_like
 from awkward._slicing import NO_HEAD
+from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 from awkward._util import unset
 from awkward.contents.bytemaskedarray import ByteMaskedArray
 from awkward.contents.content import Content
 from awkward.forms.bitmaskedform import BitMaskedForm
-from awkward.forms.form import _type_parameters_equal
 from awkward.index import Index
-from awkward.typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
@@ -114,82 +116,66 @@
 
     is_option = True
 
     def __init__(
         self, mask, content, valid_when, length, lsb_order, *, parameters=None
     ):
         if not (isinstance(mask, Index) and mask.dtype == np.dtype(np.uint8)):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'mask' must be an Index with dtype=uint8, not {}".format(
-                        type(self).__name__, repr(mask)
-                    )
+            raise TypeError(
+                "{} 'mask' must be an Index with dtype=uint8, not {}".format(
+                    type(self).__name__, repr(mask)
                 )
             )
         if not isinstance(content, Content):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'content' must be a Content subtype, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} 'content' must be a Content subtype, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
         if content.is_union or content.is_indexed or content.is_option:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{0} cannot contain a union-type, option-type, or indexed 'content' ({1}); try {0}.simplified instead".format(
-                        type(self).__name__, type(content).__name__
-                    )
+            raise TypeError(
+                "{0} cannot contain a union-type, option-type, or indexed 'content' ({1}); try {0}.simplified instead".format(
+                    type(self).__name__, type(content).__name__
                 )
             )
         if not isinstance(valid_when, bool):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'valid_when' must be boolean, not {}".format(
-                        type(self).__name__, repr(valid_when)
-                    )
+            raise TypeError(
+                "{} 'valid_when' must be boolean, not {}".format(
+                    type(self).__name__, repr(valid_when)
                 )
             )
         if length is not unknown_length:
             if not (is_integer(length) and length >= 0):
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} 'length' must be a non-negative integer, not {}".format(
-                            type(self).__name__, length
-                        )
+                raise TypeError(
+                    "{} 'length' must be a non-negative integer, not {}".format(
+                        type(self).__name__, length
                     )
                 )
         if not isinstance(lsb_order, bool):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'lsb_order' must be boolean, not {}".format(
-                        type(self).__name__, repr(lsb_order)
-                    )
+            raise TypeError(
+                "{} 'lsb_order' must be boolean, not {}".format(
+                    type(self).__name__, repr(lsb_order)
                 )
             )
         if (
             not (length is unknown_length or mask.length is unknown_length)
             and length > mask.length * 8
         ):
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "{} 'length' ({}) must be <= len(mask) * 8 ({})".format(
-                        type(self).__name__, length, mask.length * 8
-                    )
+            raise ValueError(
+                "{} 'length' ({}) must be <= len(mask) * 8 ({})".format(
+                    type(self).__name__, length, mask.length * 8
                 )
             )
         if (
             not (length is unknown_length or content.length is unknown_length)
             and length > content.length * 8
         ):
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "{} 'length' ({}) must be <= len(content) ({})".format(
-                        type(self).__name__, length, content.length
-                    )
+            raise ValueError(
+                "{} 'length' ({}) must be <= len(content) ({})".format(
+                    type(self).__name__, length, content.length
                 )
             )
 
         assert mask.nplike is content.backend.index_nplike
 
         self._mask = mask
         self._content = content
@@ -550,15 +536,15 @@
         elif head is Ellipsis:
             return self._getitem_next_ellipsis(tail, advanced)
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             return self._getitem_next_missing(head, tail, advanced)
 
         else:
-            raise ak._errors.wrap_error(AssertionError(repr(head)))
+            raise AssertionError(repr(head))
 
     def project(self, mask=None):
         return self.to_ByteMaskedArray().project(mask)
 
     def _offsets_and_flattened(self, axis, depth):
         return self.to_ByteMaskedArray._offsets_and_flattened(axis, depth)
 
@@ -566,15 +552,15 @@
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # We can only combine option types whose array-record parameters agree
         elif other.is_option or other.is_indexed:
             return self._content._mergeable_next(
                 other.content, mergebool
-            ) and _type_parameters_equal(self._parameters, other._parameters)
+            ) and type_parameters_equal(self._parameters, other._parameters)
         else:
             return self._content._mergeable_next(other, mergebool)
 
     def _reverse_merge(self, other):
         return self.to_IndexedOptionArray64()._reverse_merge(other)
 
     def _mergemany(self, others):
@@ -748,15 +734,15 @@
         )
 
         if isinstance(result, Content):
             return result
         elif result is None:
             return continuation()
         else:
-            raise ak._errors.wrap_error(AssertionError(result))
+            raise AssertionError(result)
 
     def to_packed(self) -> Self:
         if self._content.is_record:
             next = self.to_IndexedOptionArray64()
 
             content = next._content.to_packed()
             if content.length > self._length:
@@ -784,17 +770,15 @@
                 self._length,
                 self._lsb_order,
                 parameters=self._parameters,
             )
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
-            raise ak._errors.wrap_error(
-                TypeError("cannot convert typetracer arrays to Python lists")
-            )
+            raise TypeError("cannot convert typetracer arrays to Python lists")
 
         out = self._to_list_custom(behavior, json_conversions)
         if out is not None:
             return out
 
         mask = self.mask_as_bool(valid_when=True)[: self._length]
         out = self._content._getitem_range(0, self._length)._to_list(
```

### Comparing `awkward-2.1.1/src/awkward/contents/bytemaskedarray.py` & `awkward-2.1.2/src/awkward/contents/bytemaskedarray.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,22 +7,25 @@
 
 import awkward as ak
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import MaybeNone, TypeTracer
+from awkward._parameters import (
+    parameters_intersect,
+    type_parameters_equal,
+)
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
+from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 from awkward._util import unset
 from awkward.contents.content import Content
 from awkward.forms.bytemaskedform import ByteMaskedForm
-from awkward.forms.form import _type_parameters_equal
 from awkward.index import Index
-from awkward.typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 
@@ -84,54 +87,44 @@
                     raise AssertionError(where)
     """
 
     is_option = True
 
     def __init__(self, mask, content, valid_when, *, parameters=None):
         if not (isinstance(mask, Index) and mask.dtype == np.dtype(np.int8)):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'mask' must be an Index with dtype=int8, not {}".format(
-                        type(self).__name__, repr(mask)
-                    )
+            raise TypeError(
+                "{} 'mask' must be an Index with dtype=int8, not {}".format(
+                    type(self).__name__, repr(mask)
                 )
             )
         if not isinstance(content, Content):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'content' must be a Content subtype, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} 'content' must be a Content subtype, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
         if content.is_union or content.is_indexed or content.is_option:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{0} cannot contain a union-type, option-type, or indexed 'content' ({1}); try {0}.simplified instead".format(
-                        type(self).__name__, type(content).__name__
-                    )
+            raise TypeError(
+                "{0} cannot contain a union-type, option-type, or indexed 'content' ({1}); try {0}.simplified instead".format(
+                    type(self).__name__, type(content).__name__
                 )
             )
         if not isinstance(valid_when, bool):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'valid_when' must be boolean, not {}".format(
-                        type(self).__name__, repr(valid_when)
-                    )
+            raise TypeError(
+                "{} 'valid_when' must be boolean, not {}".format(
+                    type(self).__name__, repr(valid_when)
                 )
             )
         if (
             not (mask.length is unknown_length or content.length is unknown_length)
             and mask.length > content.length
         ):
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "{} len(mask) ({}) must be <= len(content) ({})".format(
-                        type(self).__name__, mask.length, content.length
-                    )
+            raise ValueError(
+                "{} len(mask) ({}) must be <= len(content) ({})".format(
+                    type(self).__name__, mask.length, content.length
                 )
             )
 
         assert mask.nplike is content.backend.index_nplike
 
         self._mask = mask
         self._content = content
@@ -565,27 +558,25 @@
         elif head is Ellipsis:
             return self._getitem_next_ellipsis(tail, advanced)
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             return self._getitem_next_missing(head, tail, advanced)
 
         else:
-            raise ak._errors.wrap_error(AssertionError(repr(head)))
+            raise AssertionError(repr(head))
 
     def project(self, mask=None):
         mask_length = self._mask.length
         numnull = ak.index.Index64.zeros(1, nplike=self._backend.index_nplike)
 
         if mask is not None:
             if self._backend.nplike.known_data and mask_length != mask.length:
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "mask length ({}) is not equal to {} length ({})".format(
-                            mask.length, type(self).__name__, mask_length
-                        )
+                raise ValueError(
+                    "mask length ({}) is not equal to {} length ({})".format(
+                        mask.length, type(self).__name__, mask_length
                     )
                 )
 
             nextmask = ak.index.Index8.empty(
                 mask_length, nplike=self._backend.index_nplike
             )
             assert (
@@ -651,15 +642,15 @@
             )
 
             return self._content._carry(nextcarry, False)
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise ak._errors.wrap_error(np.AxisError("axis=0 not allowed for flatten"))
+            raise np.AxisError("axis=0 not allowed for flatten")
         else:
             numnull, nextcarry, outindex = self._nextcarry_outindex()
 
             next = self._content._carry(nextcarry, False)
 
             offsets, flattened = next._offsets_and_flattened(axis, depth)
 
@@ -703,15 +694,15 @@
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # We can only combine option types whose array-record parameters agree
         elif other.is_option or other.is_indexed:
             return self._content._mergeable_next(
                 other.content, mergebool
-            ) and _type_parameters_equal(self._parameters, other._parameters)
+            ) and type_parameters_equal(self._parameters, other._parameters)
         else:
             return self._content._mergeable_next(other, mergebool)
 
     def _reverse_merge(self, other):
         return self.to_IndexedOptionArray64()._reverse_merge(other)
 
     def _mergemany(self, others):
@@ -727,17 +718,15 @@
                 self.length
             )
             masks = [self._mask.data[:self_length_scalar]]
             tail_contents = []
             length = 0
             for x in others:
                 length_scalar = self._backend.index_nplike.shape_item_as_index(x.length)
-                parameters = ak.forms.form._parameters_intersect(
-                    parameters, x._parameters
-                )
+                parameters = parameters_intersect(parameters, x._parameters)
                 masks.append(x._mask.data[:length_scalar])
                 tail_contents.append(x._content[:length_scalar])
                 length += x.length
 
             return ByteMaskedArray(
                 ak.index.Index8(self._backend.nplike.concat(masks)),
                 self._content[:self_length_scalar]._mergemany(tail_contents),
@@ -796,17 +785,15 @@
     def _sort_next(self, negaxis, starts, parents, outlength, ascending, stable):
         return self.to_IndexedOptionArray64()._sort_next(
             negaxis, starts, parents, outlength, ascending, stable
         )
 
     def _combinations(self, n, replacement, recordlookup, parameters, axis, depth):
         if n < 1:
-            raise ak._errors.wrap_error(
-                ValueError("in combinations, 'n' must be at least 1")
-            )
+            raise ValueError("in combinations, 'n' must be at least 1")
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             return self._combinations_axis0(n, replacement, recordlookup, parameters)
         else:
             _, nextcarry, outindex = self._nextcarry_outindex()
 
             next = self._content._carry(nextcarry, True)
@@ -949,20 +936,18 @@
             return out
         else:
             if out.is_list:
                 out_content = out.content[out.starts[0] :]
             elif out.is_regular:
                 out_content = out.content
             else:
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "reduce_next with unbranching depth > negaxis is only "
-                        "expected to return RegularArray or ListOffsetArray64; "
-                        "instead, it returned " + out
-                    )
+                raise ValueError(
+                    "reduce_next with unbranching depth > negaxis is only "
+                    "expected to return RegularArray or ListOffsetArray64; "
+                    "instead, it returned " + out
                 )
 
             outoffsets = ak.index.Index64.empty(
                 starts.length + 1, nplike=self._backend.index_nplike
             )
             assert outoffsets.nplike is self._backend.nplike
             self._handle_error(
@@ -1105,15 +1090,15 @@
         )
 
         if isinstance(result, Content):
             return result
         elif result is None:
             return continuation()
         else:
-            raise ak._errors.wrap_error(AssertionError(result))
+            raise AssertionError(result)
 
     def to_packed(self) -> Self:
         if self._content.is_record:
             next = self.to_IndexedOptionArray64()
             content = next._content.to_packed()
             if content.length > self._mask.length:
                 content = content[: self._mask.length]
@@ -1129,17 +1114,15 @@
 
             return ByteMaskedArray(
                 self._mask, content, self._valid_when, parameters=self._parameters
             )
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
-            raise ak._errors.wrap_error(
-                TypeError("cannot convert typetracer arrays to Python lists")
-            )
+            raise TypeError("cannot convert typetracer arrays to Python lists")
 
         out = self._to_list_custom(behavior, json_conversions)
         if out is not None:
             return out
 
         mask = self.mask_as_bool(valid_when=True)
         out = self._content._getitem_range(0, mask.size)._to_list(
```

### Comparing `awkward-2.1.1/src/awkward/contents/content.py` & `awkward-2.1.2/src/awkward/contents/content.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,34 +8,39 @@
 
 import awkward as ak
 from awkward._backends import Backend
 from awkward._behavior import get_array_class, get_record_class
 from awkward._layout import wrap_layout
 from awkward._nplikes import to_nplike
 from awkward._nplikes.numpy import Numpy
-from awkward._nplikes.numpylike import IndexType, NumpyLike, NumpyMetadata
+from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import ShapeItem, unknown_length
 from awkward._nplikes.typetracer import TypeTracer
+from awkward._parameters import (
+    type_parameters_equal,
+)
 from awkward._regularize import is_integer_like, is_sized_iterable
 from awkward._slicing import normalize_slice
-from awkward._util import unset
-from awkward.forms.form import Form, JSONMapping, _type_parameters_equal
-from awkward.index import Index, Index64
-from awkward.typing import (
+from awkward._typing import (
     TYPE_CHECKING,
     Any,
     AxisMaybeNone,
+    JSONMapping,
     Literal,
     Self,
     SupportsIndex,
     TypeAlias,
     TypedDict,
 )
+from awkward._util import unset
+from awkward.forms.form import Form
+from awkward.index import Index, Index64
 
 if TYPE_CHECKING:
+    from awkward._nplikes.numpy import NumpyLike
     from awkward._slicing import SliceItem
 
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
 ActionType: TypeAlias = """Callable[
@@ -74,66 +79,54 @@
     is_union = False
     is_leaf = False
 
     def _init(self, parameters: dict[str, Any] | None, backend: Backend):
         if parameters is None:
             pass
         elif not isinstance(parameters, dict):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'parameters' must be a dict or None, not {}".format(
-                        type(self).__name__, repr(parameters)
-                    )
+            raise TypeError(
+                "{} 'parameters' must be a dict or None, not {}".format(
+                    type(self).__name__, repr(parameters)
                 )
             )
         else:
             if not self.is_list and parameters.get("__array__") in (
                 "string",
                 "bytestring",
             ):
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        '{} is not allowed to have parameters["__array__"] = "{}"'.format(
-                            type(self).__name__, parameters["__array__"]
-                        )
+                raise TypeError(
+                    '{} is not allowed to have parameters["__array__"] = "{}"'.format(
+                        type(self).__name__, parameters["__array__"]
                     )
                 )
             if not isinstance(self, ak.contents.NumpyArray) and parameters.get(
                 "__array__"
             ) in ("char", "byte"):
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        '{} is not allowed to have parameters["__array__"] = "{}"'.format(
-                            type(self).__name__, parameters["__array__"]
-                        )
+                raise TypeError(
+                    '{} is not allowed to have parameters["__array__"] = "{}"'.format(
+                        type(self).__name__, parameters["__array__"]
                     )
                 )
             if not self.is_indexed and parameters.get("__array__") == "categorical":
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        '{} is not allowed to have parameters["__array__"] = "{}"'.format(
-                            type(self).__name__, parameters["__array__"]
-                        )
+                raise TypeError(
+                    '{} is not allowed to have parameters["__array__"] = "{}"'.format(
+                        type(self).__name__, parameters["__array__"]
                     )
                 )
             if not self.is_record and parameters.get("__array__") == "sorted_map":
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        '{} is not allowed to have parameters["__array__"] = "{}"'.format(
-                            type(self).__name__, parameters["__array__"]
-                        )
+                raise TypeError(
+                    '{} is not allowed to have parameters["__array__"] = "{}"'.format(
+                        type(self).__name__, parameters["__array__"]
                     )
                 )
 
         if not isinstance(backend, Backend):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'backend' must be a Backend, not {}".format(
-                        type(self).__name__, repr(backend)
-                    )
+            raise TypeError(
+                "{} 'backend' must be a Backend, not {}".format(
+                    type(self).__name__, repr(backend)
                 )
             )
 
         self._parameters = parameters
         self._backend = backend
 
     @property
@@ -190,59 +183,57 @@
 
             def getkey(layout):
                 out = form_key(id=hold_id[0], layout=layout)
                 hold_id[0] += 1
                 return out
 
         else:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "form_key must be None, a string, or a callable, not {}".format(
-                        type(form_key)
-                    )
+            raise TypeError(
+                "form_key must be None, a string, or a callable, not {}".format(
+                    type(form_key)
                 )
             )
 
         return self._form_with_key(getkey)
 
     def _form_with_key(
         self,
         getkey: Callable[[Content], Form],
     ) -> Form:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @property
     def form_cls(self) -> type[Form]:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def to_typetracer(self, forget_length: bool = False) -> Self:
         return self._to_typetracer(forget_length)
 
     def _to_typetracer(self, forget_length: bool) -> Self:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _touch_data(self, recursive):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _touch_shape(self, recursive):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @property
     def length(self) -> ShapeItem:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _to_buffers(
         self,
         form: Form,
         getkey: Callable[[Content, Form, str], str],
         container: MutableMapping[str, Any] | None,
         backend: Backend,
         byteorder: Literal["<", ">"],
     ) -> tuple[Form, int, Mapping[str, Any]]:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def __len__(self) -> int:
         return int(self.length)
 
     def _repr_extra(self, indent: str) -> list[str]:
         out = []
         if self._parameters is not None:
@@ -265,24 +256,24 @@
                 filename = " (in compiled code: " + error.filename.decode(
                     errors="surrogateescape"
                 ).lstrip("\n").lstrip("(")
 
             message = error.str.decode(errors="surrogateescape")
 
             if error.pass_through:
-                raise ak._errors.wrap_error(ValueError(message + filename))
+                raise ValueError(message + filename)
 
             else:
                 if error.attempt != ak._util.kSliceNone:
                     message += f" while attempting to get index {error.attempt}"
 
                 message += filename
 
                 if slicer is None:
-                    raise ak._errors.wrap_error(ValueError(message))
+                    raise ValueError(message)
                 else:
                     raise ak._errors.index_error(self, slicer, message)
 
     @staticmethod
     def _selfless_handle_error(error):
         if error.str is not None:
             if error.filename is None:
@@ -291,50 +282,42 @@
                 filename = " (in compiled code: " + error.filename.decode(
                     errors="surrogateescape"
                 ).lstrip("\n").lstrip("(")
 
             message = error.str.decode(errors="surrogateescape")
 
             if error.pass_through:
-                raise ak._errors.wrap_error(ValueError(message + filename))
+                raise ValueError(message + filename)
 
             else:
                 if error.attempt != ak._util.kSliceNone:
                     message += f" while attempting to get index {error.attempt}"
 
                 message += filename
 
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
 
     def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
-        raise ak._errors.wrap_error(
-            TypeError(
-                "do not apply NumPy functions to low-level layouts (Content subclasses); put them in ak.highlevel.Array"
-            )
+        raise TypeError(
+            "do not apply NumPy functions to low-level layouts (Content subclasses); put them in ak.highlevel.Array"
         )
 
     def __array_function__(self, func, types, args, kwargs):
-        raise ak._errors.wrap_error(
-            TypeError(
-                "do not apply NumPy functions to low-level layouts (Content subclasses); put them in ak.highlevel.Array"
-            )
+        raise TypeError(
+            "do not apply NumPy functions to low-level layouts (Content subclasses); put them in ak.highlevel.Array"
         )
 
     def __array__(self, **kwargs):
-        raise ak._errors.wrap_error(
-            TypeError(
-                "do not try to convert low-level layouts (Content subclasses) into NumPy arrays; put them in ak.highlevel.Array"
-            )
+        raise TypeError(
+            "do not try to convert low-level layouts (Content subclasses) into NumPy arrays; put them in ak.highlevel.Array"
         )
 
     def __iter__(self):
         if not self._backend.nplike.known_data:
-            raise ak._errors.wrap_error(
-                TypeError("cannot iterate on an array without concrete data")
-            )
+            raise TypeError("cannot iterate on an array without concrete data")
 
         for i in range(len(self)):
             yield self._getitem_at(i)
 
     def _getitem_next_field(
         self,
         head: SliceItem | tuple,
@@ -494,17 +477,15 @@
                 self,
                 head,
                 "cannot mix missing values in slice with NumPy-style advanced indexing",
             )
 
         if isinstance(head.content, ak.contents.ListOffsetArray):
             if self._backend.nplike.known_data and self.length != 1:
-                raise ak._errors.wrap_error(
-                    NotImplementedError("reached a not-well-considered code path")
-                )
+                raise NotImplementedError("reached a not-well-considered code path")
             return self._getitem_next_missing_jagged(head, tail, advanced, self)
 
         if isinstance(head.content, ak.contents.NumpyArray):
             headcontent = Index64(head.content.data)
             nextcontent = self._getitem_next(headcontent, tail, advanced)
         else:
             nextcontent = self._getitem_next(head.content, tail, advanced)
@@ -524,34 +505,30 @@
                 if isinstance(content, ak.contents.RegularArray):
                     contents.append(
                         self._getitem_next_regular_missing(
                             head, tail, advanced, content, content.length
                         )
                     )
                 else:
-                    raise ak._errors.wrap_error(
-                        NotImplementedError(
-                            "FIXME: unhandled case of SliceMissing with RecordArray containing {}".format(
-                                content
-                            )
+                    raise NotImplementedError(
+                        "FIXME: unhandled case of SliceMissing with RecordArray containing {}".format(
+                            content
                         )
                     )
 
             return ak.contents.RecordArray(
                 contents,
                 nextcontent._fields,
                 parameters=self._parameters,
                 backend=self._backend,
             )
 
         else:
-            raise ak._errors.wrap_error(
-                NotImplementedError(
-                    f"FIXME: unhandled case of SliceMissing with {nextcontent}"
-                )
+            raise NotImplementedError(
+                f"FIXME: unhandled case of SliceMissing with {nextcontent}"
             )
 
     def __getitem__(self, where):
         return self._getitem(where)
 
     def _getitem(self, where):
         if is_integer_like(where):
@@ -642,19 +619,17 @@
                     where = self._backend.index_nplike.nonzero(data_as_index)[0]
                     carry = Index64(where, nplike=self._backend.index_nplike)
                     allow_lazy = "copied"  # True, but also can be modified in-place
                 else:
                     wheres = self._backend.index_nplike.nonzero(data_as_index)
                     return self._getitem(wheres)
             else:
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "array slice must be an array of integers or booleans, not\n\n    {}".format(
-                            repr(where.data).replace("\n", "\n    ")
-                        )
+                raise TypeError(
+                    "array slice must be an array of integers or booleans, not\n\n    {}".format(
+                        repr(where.data).replace("\n", "\n    ")
                     )
                 )
 
             out = ak._slicing.getitem_next_array_wrap(
                 self._carry(carry, allow_lazy), where.shape
             )
             if out.length is not unknown_length and out.length == 0:
@@ -686,18 +661,16 @@
         elif is_sized_iterable(where):
             # Do we have an array
             nplike = ak._nplikes.nplike_of(where, default=None)
             # We can end up with non-array objects associated with an nplike
             if nplike is not None and nplike.is_own_array(where):
                 # Is it a scalar, not array?
                 if len(where.shape) == 0:
-                    raise ak._errors.wrap_error(
-                        AssertionError(
-                            "scalar arrays should be handled by integer-like indexing"
-                        )
+                    raise AssertionError(
+                        "scalar arrays should be handled by integer-like indexing"
                     )
                 else:
                     layout = ak.operations.ak_to_layout._impl(
                         where, allow_record=False, allow_other=False, regulararray=False
                     )
                     return self._getitem(layout)
 
@@ -716,80 +689,76 @@
             else:
                 layout = ak.operations.ak_to_layout._impl(
                     where, allow_record=False, allow_other=False, regulararray=False
                 )
                 return self._getitem(layout)
 
         else:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "only integers, slices (`:`), ellipsis (`...`), np.newaxis (`None`), "
-                    "integer/boolean arrays (possibly with variable-length nested "
-                    "lists or missing values), field name (str) or names (non-tuple "
-                    "iterable of str) are valid indices for slicing, not\n\n    "
-                    + repr(where).replace("\n", "\n    ")
-                )
+            raise TypeError(
+                "only integers, slices (`:`), ellipsis (`...`), np.newaxis (`None`), "
+                "integer/boolean arrays (possibly with variable-length nested "
+                "lists or missing values), field name (str) or names (non-tuple "
+                "iterable of str) are valid indices for slicing, not\n\n    "
+                + repr(where).replace("\n", "\n    ")
             )
 
     def _getitem_at(self, where: IndexType):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _getitem_range(self, start: SupportsIndex, stop: IndexType) -> Content:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _getitem_field(
         self, where: str | SupportsIndex, only_fields: tuple[str, ...] = ()
     ) -> Content:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _getitem_fields(
         self, where: list[str], only_fields: tuple[str, ...] = ()
     ) -> Content:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _getitem_next(
         self,
         head: SliceItem | tuple,
         tail: tuple[SliceItem, ...],
         advanced: Index | None,
     ) -> Content:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _carry(self, carry: Index, allow_lazy: bool) -> Content:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _local_index_axis0(self) -> ak.contents.NumpyArray:
         localindex = Index64.empty(self.length, self._backend.index_nplike)
         self._handle_error(
             self._backend["awkward_localindex", np.int64](
                 localindex.data,
                 localindex.length,
             )
         )
         return ak.contents.NumpyArray(
             localindex.data, parameters=None, backend=self._backend
         )
 
     def _mergeable_next(self, other: Content, mergebool: bool) -> bool:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _mergemany(
         self,
         others: list[Content],
     ) -> Content:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _merging_strategy(
         self, others: list[Content]
     ) -> tuple[list[Content], list[Content]]:
         if len(others) == 0:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "to merge this array with 'others', at least one other must be provided"
-                )
+            raise ValueError(
+                "to merge this array with 'others', at least one other must be provided"
             )
 
         head = [self]
         tail = []
         i = 0
 
         while i < len(others):
@@ -823,52 +792,52 @@
                 x if isinstance(x.backend.nplike, TypeTracer) else x.to_typetracer()
                 for x in tail
             ]
 
         return (head, tail)
 
     def _local_index(self, axis: int, depth: int):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _reduce_next(
         self,
         reducer: ak._reducers.Reducer,
         negaxis: int,
         starts: Index,
         shifts: Index | None,
         parents: Index,
         outlength: int,
         mask: bool,
         keepdims: bool,
         behavior: dict | None,
     ):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _argsort_next(
         self,
         negaxis: int,
         starts: Index,
         shifts: Index | None,
         parents: Index,
         outlength: int,
         ascending: bool,
         stable: bool,
     ):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _sort_next(
         self,
         negaxis: int,
         starts: Index,
         parents: Index,
         outlength: int,
         ascending: bool,
         stable: bool,
     ):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _combinations_axis0(
         self,
         n: int,
         replacement: bool,
         recordlookup: list[str] | None,
         parameters: dict | None,
@@ -944,26 +913,26 @@
         n: int,
         replacement: bool,
         recordlookup: list[str] | None,
         parameters: dict[str, Any] | None,
         axis: int,
         depth: int,
     ):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _validity_error_parameters(self, path: str) -> str:
         if self.parameter("__array__") == "categorical":
             if not ak._do.is_unique(self._content):
                 return 'at {} ("{}"): __array__ = "categorical" requires contents to be unique'.format(
                     path, type(self)
                 )
         return ""
 
     def _validity_error(self, path: str) -> str:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @property
     def nbytes(self) -> int:
         return self._nbytes_part()
 
     def purelist_parameter(self, key: str):
         """
@@ -978,24 +947,24 @@
     def _is_unique(
         self,
         negaxis: AxisMaybeNone,
         starts: Index,
         parents: Index,
         outlength: int,
     ) -> bool:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _unique(
         self,
         negaxis: AxisMaybeNone,
         starts: Index,
         parents: Index,
         outlength: int,
     ):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @property
     def is_identity_like(self) -> bool:
         return self.form_cls.is_identity_like.__get__(self)
 
     @property
     def purelist_isregular(self) -> bool:
@@ -1057,15 +1026,15 @@
             )
 
         return ak.contents.IndexedOptionArray.simplified(
             index, self, parameters=self._parameters
         )
 
     def _pad_none(self, target: int, axis: int, depth: int, clip: bool) -> Content:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def to_arrow(
         self,
         list_to32: bool = False,
         string_to32: bool = False,
         bytestring_to32: bool = False,
         emptyarray_to=None,
@@ -1098,15 +1067,15 @@
         self,
         pyarrow: Any,
         mask_node: Any,
         validbytes: Any,
         length: int,
         options: dict[str, Any],
     ):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def to_numpy(self, allow_missing: bool = True):
         ak._errors.deprecate(
             "`Content.to_numpy` is deprecated. Please replace calls to "
             "`Content.to_numpy(...)` with `Content.to_backend_array(..., backend='cpu')`.",
             "2.2.0",
         )
@@ -1120,35 +1089,35 @@
         if backend is None:
             backend = self._backend
         else:
             backend = ak._backends.regularize_backend(backend)
         return self._to_backend_array(allow_missing, backend)
 
     def _to_backend_array(self, allow_missing: bool, backend: ak._backends.Backend):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def drop_none(self):
         return self._drop_none()
 
     def _drop_none(self) -> Content:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _remove_structure(self, backend, options):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _recursively_apply(
         self,
         action: ActionType,
         behavior: dict | None,
         depth: int,
         depth_context: dict | None,
         lateral_context: dict | None,
         options: RecursivelyApplyOptionsType,
     ) -> Content | None:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def to_json(
         self,
         nan_string: str | None = None,
         posinf_string: str | None = None,
         neginf_string: str | None = None,
         complex_record_fields: tuple[str, str] | None = None,
@@ -1178,23 +1147,23 @@
                 "complex_real_string": complex_real_string,
                 "complex_imag_string": complex_imag_string,
                 "convert_bytes": convert_bytes,
             },
         )
 
     def to_packed(self) -> Content:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def to_list(self, behavior: dict | None = None) -> list:
         return self.to_packed()._to_list(behavior, None)
 
     def _to_list(
         self, behavior: dict | None, json_conversions: dict[str, Any] | None
     ) -> list:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _to_list_custom(
         self, behavior: dict | None, json_conversions: dict[str, Any] | None
     ):
         if self.is_record:
             getitem = get_record_class(self, behavior).__getitem__
             overloaded = getitem is not ak.highlevel.Record.__getitem__ and not getattr(
@@ -1289,64 +1258,64 @@
                 if outimag is not None:
                     for i, (real, imag) in enumerate(zip(out, outimag)):
                         out[i] = {complex_real_string: real, complex_imag_string: imag}
 
             return out
 
     def _offsets_and_flattened(self, axis: int, depth: int) -> tuple[Index, Content]:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def to_backend(self, backend: Backend | str | None = None) -> Self:
         if backend is None:
             backend = self._backend
         else:
             backend = ak._backends.regularize_backend(backend)
         if backend is self._backend:
             return self
         else:
             return self._to_backend(backend)
 
     def _to_backend(self, backend: Backend) -> Self:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def with_parameter(self, key: str, value: Any) -> Self:
         out = copy.copy(self)
 
         if self._parameters is None:
             parameters = {}
         else:
             parameters = copy.copy(self._parameters)
         parameters[key] = value
         out._parameters = parameters
 
         return out
 
     def __copy__(self):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def __deepcopy__(self, memo):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def is_equal_to(
         self, other: Content, index_dtype: bool = True, numpyarray: bool = True
     ) -> bool:
         return (
             self.__class__ is other.__class__
             and len(self) == len(other)
-            and _type_parameters_equal(self.parameters, other.parameters)
+            and type_parameters_equal(self.parameters, other.parameters)
             and self._is_equal_to(other, index_dtype, numpyarray)
         )
 
     def _is_equal_to(self, other: Self, index_dtype: bool, numpyarray: bool) -> bool:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _repr(self, indent: str, pre: str, post: str) -> str:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _numbers_to_type(self, name: str, including_unknown: bool) -> Content:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _fill_none(self, value: Content) -> Content:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def copy(self, *, parameters: JSONMapping | None = unset) -> Self:
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
```

### Comparing `awkward-2.1.1/src/awkward/contents/emptyarray.py` & `awkward-2.1.2/src/awkward/contents/emptyarray.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 import awkward as ak
 from awkward._errors import deprecate
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
+from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 from awkward._util import unset
 from awkward.contents.content import Content
 from awkward.forms.emptyform import EmptyForm
 from awkward.index import Index
-from awkward.typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
@@ -224,22 +224,20 @@
         elif isinstance(head, ak.contents.ListOffsetArray):
             raise ak._errors.index_error(self, head, "array is empty")
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             raise ak._errors.index_error(self, head, "array is empty")
 
         else:
-            raise ak._errors.wrap_error(AssertionError(repr(head)))
+            raise AssertionError(repr(head))
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise ak._errors.wrap_error(
-                np.AxisError(self, "axis=0 not allowed for flatten")
-            )
+            raise np.AxisError(self, "axis=0 not allowed for flatten")
         else:
             offsets = ak.index.Index64.zeros(1, nplike=self._backend.index_nplike)
             return (
                 offsets,
                 EmptyArray(parameters=self._parameters, backend=self._backend),
             )
 
@@ -262,17 +260,15 @@
         if posaxis is not None and posaxis + 1 == depth:
             return ak.contents.NumpyArray(
                 self._backend.nplike.empty(0, dtype=np.int64),
                 parameters=None,
                 backend=self._backend,
             )
         else:
-            raise ak._errors.wrap_error(
-                np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
-            )
+            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
 
     def _numbers_to_type(self, name, including_unknown):
         if including_unknown:
             return self.to_NumpyArray(ak.types.numpytype.primitive_to_dtype(name))
         else:
             return self
 
@@ -328,17 +324,15 @@
 
     def _nbytes_part(self):
         return 0
 
     def _pad_none(self, target, axis, depth, clip):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 != depth:
-            raise ak._errors.wrap_error(
-                np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
-            )
+            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
         else:
             return self._pad_none_axis0(target, True)
 
     def _to_arrow(self, pyarrow, mask_node, validbytes, length, options):
         if options["emptyarray_to"] is None:
             return pyarrow.Array.from_buffers(
                 ak._connect.pyarrow.to_awkwardarrow_type(
@@ -398,24 +392,22 @@
         )
 
         if isinstance(result, Content):
             return result
         elif result is None:
             return continuation()
         else:
-            raise ak._errors.wrap_error(AssertionError(result))
+            raise AssertionError(result)
 
     def to_packed(self) -> Self:
         return self
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
-            raise ak._errors.wrap_error(
-                TypeError("cannot convert typetracer arrays to Python lists")
-            )
+            raise TypeError("cannot convert typetracer arrays to Python lists")
         return []
 
     def _to_backend(self, backend: ak._backends.Backend) -> Self:
         return EmptyArray(parameters=self._parameters, backend=backend)
 
     def _is_equal_to(self, other, index_dtype, numpyarray):
         return True
```

### Comparing `awkward-2.1.1/src/awkward/contents/indexedarray.py` & `awkward-2.1.2/src/awkward/contents/indexedarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 import copy
 
 import awkward as ak
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.typetracer import TypeTracer
+from awkward._parameters import (
+    parameters_intersect,
+    parameters_union,
+    type_parameters_equal,
+)
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
+from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 from awkward._util import unset
 from awkward.contents.content import Content
-from awkward.forms.form import _type_parameters_equal
 from awkward.forms.indexedform import IndexedForm
 from awkward.index import Index
-from awkward.typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
@@ -84,35 +88,29 @@
             and index.dtype
             in (
                 np.dtype(np.int32),
                 np.dtype(np.uint32),
                 np.dtype(np.int64),
             )
         ):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'index' must be an Index with dtype in (int32, uint32, int64), "
-                    "not {}".format(type(self).__name__, repr(index))
-                )
+            raise TypeError(
+                "{} 'index' must be an Index with dtype in (int32, uint32, int64), "
+                "not {}".format(type(self).__name__, repr(index))
             )
         if not isinstance(content, Content):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'content' must be a Content subtype, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} 'content' must be a Content subtype, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
         is_cat = parameters is not None and parameters.get("__array__") == "categorical"
         if (content.is_union and not is_cat) or content.is_indexed or content.is_option:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{0} cannot contain a union-type (unless categorical), option-type, or indexed 'content' ({1}); try {0}.simplified instead".format(
-                        type(self).__name__, type(content).__name__
-                    )
+            raise TypeError(
+                "{0} cannot contain a union-type (unless categorical), option-type, or indexed 'content' ({1}); try {0}.simplified instead".format(
+                    type(self).__name__, type(content).__name__
                 )
             )
 
         assert index.nplike is content.backend.index_nplike
 
         self._index = index
         self._content = content
@@ -147,17 +145,15 @@
 
     @classmethod
     def simplified(cls, index, content, *, parameters=None):
         is_cat = parameters is not None and parameters.get("__array__") == "categorical"
 
         if content.is_union and not is_cat:
             return content._carry(index, allow_lazy=False).copy(
-                parameters=ak.forms.form._parameters_union(
-                    content._parameters, parameters
-                )
+                parameters=parameters_union(content._parameters, parameters)
             )
 
         elif content.is_indexed or content.is_option:
             backend = content.backend
             if content.is_indexed:
                 inner = content.index
             else:
@@ -178,25 +174,21 @@
                     inner.length,
                 )
             )
             if isinstance(content, ak.contents.IndexedArray):
                 return ak.contents.IndexedArray(
                     result,
                     content.content,
-                    parameters=ak.forms.form._parameters_union(
-                        content._parameters, parameters
-                    ),
+                    parameters=parameters_union(content._parameters, parameters),
                 )
             else:
                 return ak.contents.IndexedOptionArray(
                     result,
                     content.content,
-                    parameters=ak.forms.form._parameters_union(
-                        content._parameters, parameters
-                    ),
+                    parameters=parameters_union(content._parameters, parameters),
                 )
 
         else:
             return cls(index, content, parameters=parameters)
 
     def _form_with_key(self, getkey):
         form_key = getkey(self)
@@ -405,24 +397,22 @@
         elif head is Ellipsis:
             return self._getitem_next_ellipsis(tail, advanced)
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             return self._getitem_next_missing(head, tail, advanced)
 
         else:
-            raise ak._errors.wrap_error(AssertionError(repr(head)))
+            raise AssertionError(repr(head))
 
     def project(self, mask=None):
         if mask is not None:
             if self._backend.nplike.known_data and self._index.length != mask.length:
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "mask length ({}) is not equal to {} length ({})".format(
-                            mask.length(), type(self).__name__, self._index.length
-                        )
+                raise ValueError(
+                    "mask length ({}) is not equal to {} length ({})".format(
+                        mask.length(), type(self).__name__, self._index.length
                     )
                 )
             nextindex = ak.index.Index64.empty(
                 self._index.length, self._backend.index_nplike
             )
             assert (
                 nextindex.nplike is self._backend.index_nplike
@@ -463,47 +453,45 @@
                     self._index.data,
                     self._index.length,
                     self._content.length,
                 )
             )
             next = self._content._carry(nextcarry, False)
             return next.copy(
-                parameters=ak.forms.form._parameters_union(
+                parameters=parameters_union(
                     next._parameters,
                     self._parameters,
                     exclude=(("__array__", "categorical"),),
                 )
             )
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise ak._errors.wrap_error(np.AxisError("axis=0 not allowed for flatten"))
+            raise np.AxisError("axis=0 not allowed for flatten")
 
         else:
             return self.project()._offsets_and_flattened(axis, depth)
 
     def _mergeable_next(self, other, mergebool):
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # We can only combine option/indexed types whose array-record parameters agree
         elif other.is_option or other.is_indexed:
             return self._content._mergeable_next(
                 other.content, mergebool
-            ) and _type_parameters_equal(self._parameters, other._parameters)
+            ) and type_parameters_equal(self._parameters, other._parameters)
         else:
             return self._content._mergeable_next(other, mergebool)
 
     def _merging_strategy(self, others):
         if len(others) == 0:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "to merge this array with 'others', at least one other must be provided"
-                )
+            raise ValueError(
+                "to merge this array with 'others', at least one other must be provided"
             )
 
         head = [self]
         tail = []
 
         i = 0
         while i < len(others):
@@ -563,17 +551,15 @@
                 self.index.data,
                 mylength,
                 theirlength,
             )
         )
         # We can directly merge with other options and indexed types, but we must merge parameters
         if other.is_option or other.is_indexed:
-            parameters = ak.forms.form._parameters_union(
-                self._parameters, other._parameters
-            )
+            parameters = parameters_union(self._parameters, other._parameters)
         # Otherwise, this option parameters win out
         else:
             parameters = self._parameters
 
         return ak.contents.IndexedArray.simplified(
             index, content, parameters=parameters
         )
@@ -609,17 +595,15 @@
                 ),
             ):
                 array = array.to_IndexedOptionArray64()
 
             if isinstance(
                 array, (ak.contents.IndexedOptionArray, ak.contents.IndexedArray)
             ):
-                parameters = ak.forms.form._parameters_intersect(
-                    parameters, array._parameters
-                )
+                parameters = parameters_intersect(parameters, array._parameters)
 
                 contents.append(array.content)
                 array_index = array.index
                 assert (
                     nextindex.nplike is self._backend.index_nplike
                     and array_index.nplike is self._backend.index_nplike
                 )
@@ -675,16 +659,16 @@
         if len(tail) == 1:
             return reversed
         else:
             return reversed._mergemany(tail[1:])
 
     def _fill_none(self, value: Content) -> Content:
         if value.backend.nplike.known_data and value.length != 1:
-            raise ak._errors.wrap_error(
-                ValueError(f"fill_none value length ({value.length}) is not equal to 1")
+            raise ValueError(
+                f"fill_none value length ({value.length}) is not equal to 1"
             )
         return IndexedArray(
             self._index, self._content._fill_none(value), parameters=self._parameters
         )
 
     def _local_index(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
@@ -857,20 +841,18 @@
             return unique
         else:
             if isinstance(unique, ak.contents.RegularArray):
                 unique = unique.to_ListOffsetArray64(True)
 
             if isinstance(unique, ak.contents.ListOffsetArray):
                 if starts.nplike.known_data and starts.length > 0 and starts[0] != 0:
-                    raise ak._errors.wrap_error(
-                        AssertionError(
-                            "reduce_next with unbranching depth > negaxis expects a "
-                            "ListOffsetArray64 whose offsets start at zero ({})".format(
-                                starts[0]
-                            )
+                    raise AssertionError(
+                        "reduce_next with unbranching depth > negaxis expects a "
+                        "ListOffsetArray64 whose offsets start at zero ({})".format(
+                            starts[0]
                         )
                     )
 
                 outoffsets = ak.index.Index64.empty(
                     starts.length + 1, self._backend.index_nplike
                 )
                 assert (
@@ -901,15 +883,15 @@
                     self._backend.index_nplike.arange(unique.length, dtype=np.int64),
                     nplike=self._backend.index_nplike,
                 )
                 return ak.contents.IndexedOptionArray.simplified(
                     nextoutindex, unique, parameters=self._parameters
                 )
 
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _argsort_next(
         self, negaxis, starts, shifts, parents, outlength, ascending, stable
     ):
         next = self._content._carry(self._index, False)
         return next._argsort_next(
             negaxis, starts, shifts, parents, outlength, ascending, stable
@@ -1029,17 +1011,15 @@
                 # every masked value is self._content[0], unless self._content.length == 0.
                 # In that case, don't call self._content[index]; it's empty anyway.
                 next = self._content
             else:
                 next = self._content._carry(ak.index.Index(index), False)
 
             next2 = next.copy(
-                parameters=ak.forms.form._parameters_union(
-                    next._parameters, self._parameters
-                )
+                parameters=parameters_union(next._parameters, self._parameters)
             )
             return next2._to_arrow(pyarrow, mask_node, validbytes, length, options)
 
     def _to_backend_array(self, allow_missing, backend):
         return self.project()._to_backend_array(allow_missing, backend)
 
     def _remove_structure(self, backend, options):
@@ -1108,29 +1088,27 @@
         )
 
         if isinstance(result, Content):
             return result
         elif result is None:
             return continuation()
         else:
-            raise ak._errors.wrap_error(AssertionError(result))
+            raise AssertionError(result)
 
     def to_packed(self) -> Self:
         if self.parameter("__array__") == "categorical":
             return IndexedArray(
                 self._index, self._content.to_packed(), parameters=self._parameters
             )
         else:
             return self.project().to_packed()
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
-            raise ak._errors.wrap_error(
-                TypeError("cannot convert typetracer arrays to Python lists")
-            )
+            raise TypeError("cannot convert typetracer arrays to Python lists")
 
         out = self._to_list_custom(behavior, json_conversions)
         if out is not None:
             return out
 
         index = self._index.raw(numpy)
         nextcontent = self._content._carry(ak.index.Index(index), False)
```

### Comparing `awkward-2.1.1/src/awkward/contents/indexedoptionarray.py` & `awkward-2.1.2/src/awkward/contents/indexedoptionarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,26 @@
 
 import awkward as ak
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import MaybeNone, TypeTracer
+from awkward._parameters import (
+    parameters_intersect,
+    parameters_union,
+    type_parameters_equal,
+)
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
+from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 from awkward._util import unset
 from awkward.contents.content import Content
-from awkward.forms.form import _type_parameters_equal
 from awkward.forms.indexedoptionform import IndexedOptionForm
 from awkward.index import Index
-from awkward.typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
@@ -82,35 +86,29 @@
             isinstance(index, Index)
             and index.dtype
             in (
                 np.dtype(np.int32),
                 np.dtype(np.int64),
             )
         ):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'index' must be an Index with dtype in (int32, uint32, int64), "
-                    "not {}".format(type(self).__name__, repr(index))
-                )
+            raise TypeError(
+                "{} 'index' must be an Index with dtype in (int32, uint32, int64), "
+                "not {}".format(type(self).__name__, repr(index))
             )
         if not isinstance(content, Content):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'content' must be a Content subtype, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} 'content' must be a Content subtype, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
         is_cat = parameters is not None and parameters.get("__array__") == "categorical"
         if (content.is_union and not is_cat) or content.is_indexed or content.is_option:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{0} cannot contain a union-type (unless categorical), option-type, or indexed 'content' ({1}); try {0}.simplified instead".format(
-                        type(self).__name__, type(content).__name__
-                    )
+            raise TypeError(
+                "{0} cannot contain a union-type (unless categorical), option-type, or indexed 'content' ({1}); try {0}.simplified instead".format(
+                    type(self).__name__, type(content).__name__
                 )
             )
 
         assert index.nplike is content.backend.index_nplike
 
         self._index = index
         self._content = content
@@ -171,17 +169,15 @@
                     inner.data,
                     inner.length,
                 )
             )
             return IndexedOptionArray(
                 result,
                 content.content,
-                parameters=ak.forms.form._parameters_union(
-                    content._parameters, parameters
-                ),
+                parameters=parameters_union(content._parameters, parameters),
             )
 
         else:
             return cls(index, content, parameters=parameters)
 
     def _form_with_key(self, getkey):
         form_key = getkey(self)
@@ -483,24 +479,22 @@
         elif head is Ellipsis:
             return self._getitem_next_ellipsis(tail, advanced)
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             return self._getitem_next_missing(head, tail, advanced)
 
         else:
-            raise ak._errors.wrap_error(AssertionError(repr(head)))
+            raise AssertionError(repr(head))
 
     def project(self, mask=None):
         if mask is not None:
             if self._backend.nplike.known_data and self._index.length != mask.length:
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "mask length ({}) is not equal to {} length ({})".format(
-                            mask.length(), type(self).__name__, self._index.length
-                        )
+                raise ValueError(
+                    "mask length ({}) is not equal to {} length ({})".format(
+                        mask.length(), type(self).__name__, self._index.length
                     )
                 )
             nextindex = ak.index.Index64.empty(
                 self._index.length, self._backend.index_nplike
             )
             assert (
                 nextindex.nplike is self._backend.index_nplike
@@ -565,15 +559,15 @@
             )
 
             return self._content._carry(nextcarry, False)
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise ak._errors.wrap_error(np.AxisError("axis=0 not allowed for flatten"))
+            raise np.AxisError("axis=0 not allowed for flatten")
         else:
             numnull, nextcarry, outindex = self._nextcarry_outindex()
             next = self._content._carry(nextcarry, False)
 
             offsets, flattened = next._offsets_and_flattened(axis, depth)
 
             if offsets.length == 0:
@@ -616,24 +610,22 @@
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # We can only combine option/indexed types whose array-record parameters agree
         elif other.is_option or other.is_indexed:
             return self._content._mergeable_next(
                 other.content, mergebool
-            ) and _type_parameters_equal(self._parameters, other._parameters)
+            ) and type_parameters_equal(self._parameters, other._parameters)
         else:
             return self._content._mergeable_next(other, mergebool)
 
     def _merging_strategy(self, others):
         if len(others) == 0:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "to merge this array with 'others', at least one other must be provided"
-                )
+            raise ValueError(
+                "to merge this array with 'others', at least one other must be provided"
             )
 
         head = [self]
         tail = []
 
         i = 0
         while i < len(others):
@@ -702,17 +694,15 @@
                 reinterpreted_index.data,
                 mylength,
                 theirlength,
             )
         )
         # We can directly merge with other options, but we must merge parameters
         if other.is_option:
-            parameters = ak.forms.form._parameters_union(
-                self._parameters, other._parameters
-            )
+            parameters = parameters_union(self._parameters, other._parameters)
         # Otherwise, this option parameters win out
         else:
             parameters = self._parameters
 
         return ak.contents.IndexedOptionArray.simplified(
             index, content, parameters=parameters
         )
@@ -747,17 +737,15 @@
             ):
                 array = array.to_IndexedOptionArray64()
 
             if isinstance(
                 array, (ak.contents.IndexedOptionArray, ak.contents.IndexedArray)
             ):
                 # If we're merging an option, then merge parameters before pulling out `content`
-                parameters = ak.forms.form._parameters_intersect(
-                    parameters, array._parameters
-                )
+                parameters = parameters_intersect(parameters, array._parameters)
                 contents.append(array.content)
                 array_index = array.index
                 assert (
                     nextindex.nplike is self._backend.index_nplike
                     and array_index.nplike is self._backend.index_nplike
                 )
                 self._handle_error(
@@ -808,16 +796,16 @@
         if len(tail) == 1:
             return reversed
         else:
             return reversed._mergemany(tail[1:])
 
     def _fill_none(self, value: Content) -> Content:
         if value.backend.nplike.known_data and value.length != 1:
-            raise ak._errors.wrap_error(
-                ValueError(f"fill_none value length ({value.length}) is not equal to 1")
+            raise ValueError(
+                f"fill_none value length ({value.length}) is not equal to 1"
             )
 
         contents = [self._content, value]
         tags = ak.index.Index8(self.mask_as_bool(valid_when=False))
         index = ak.index.Index64.empty(tags.length, self._backend.index_nplike)
 
         assert (
@@ -1387,31 +1375,25 @@
             return out
         else:
             if out.is_list:
                 out_content = out.content[out.starts[0] :]
             elif out.is_regular:
                 out_content = out.content
             else:
-                raise ak._errors.wrap_error(
-                    AssertionError(
-                        "reduce_next with unbranching depth > negaxis is only "
-                        "expected to return RegularArray or ListOffsetArray or "
-                        "IndexedOptionArray; "
-                        "instead, it returned {}".format(type(out).__name__)
-                    )
+                raise AssertionError(
+                    "reduce_next with unbranching depth > negaxis is only "
+                    "expected to return RegularArray or ListOffsetArray or "
+                    "IndexedOptionArray; "
+                    "instead, it returned {}".format(type(out).__name__)
                 )
 
             if starts.nplike.known_data and starts.length > 0 and starts[0] != 0:
-                raise ak._errors.wrap_error(
-                    AssertionError(
-                        "reduce_next with unbranching depth > negaxis expects a "
-                        "ListOffsetArray whose offsets start at zero ({})".format(
-                            starts[0]
-                        )
-                    )
+                raise AssertionError(
+                    "reduce_next with unbranching depth > negaxis expects a "
+                    "ListOffsetArray whose offsets start at zero ({})".format(starts[0])
                 )
             # In this branch, we're above the axis at which the reduction takes place.
             # `next._reduce_next` is therefore expected to return a list/regular layout
             # node. As detailed in `RegularArray._reduce_next`, `_reduce_next` wraps the
             # reduction in a list-type of length `outlength` before returning to the caller,
             # which effectively means that the reduction of *this* layout corresponds to the
             # child of the returned `next._reduce_next(...)`, i.e. `out.content`. So, we unpack
@@ -1576,26 +1558,22 @@
                         [np.iinfo(np.int64).max], dtype=content.dtype
                     )[0]
                 elif np.issubdtype(content.dtype, np.str_):
                     data[mask0] = ""
                 elif np.issubdtype(content.dtype, np.bytes_):
                     data[mask0] = b""
                 else:
-                    raise ak._errors.wrap_error(
-                        AssertionError(f"unrecognized dtype: {content.dtype}")
-                    )
+                    raise AssertionError(f"unrecognized dtype: {content.dtype}")
 
                 return nplike.ma.MaskedArray(data, mask)
             else:
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "Content.to_nplike cannot convert 'None' values to "
-                        "np.ma.MaskedArray unless the "
-                        "'allow_missing' parameter is set to True"
-                    )
+                raise ValueError(
+                    "Content.to_nplike cannot convert 'None' values to "
+                    "np.ma.MaskedArray unless the "
+                    "'allow_missing' parameter is set to True"
                 )
         else:
             if allow_missing:
                 return nplike.ma.MaskedArray(content)
             else:
                 return content
 
@@ -1676,15 +1654,15 @@
         )
 
         if isinstance(result, Content):
             return result
         elif result is None:
             return continuation()
         else:
-            raise ak._errors.wrap_error(AssertionError(result))
+            raise AssertionError(result)
 
     def to_packed(self) -> Self:
         original_index = self._index.raw(self._backend.nplike)
         is_none = original_index < 0
         num_none = self._backend.index_nplike.count_nonzero(is_none)
         if self.parameter("__array__") == "categorical" or self._content.length <= (
             len(original_index) - num_none
@@ -1706,17 +1684,15 @@
                 ak.index.Index(new_index, nplike=self._backend.index_nplike),
                 self.project().to_packed(),
                 parameters=self._parameters,
             )
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
-            raise ak._errors.wrap_error(
-                TypeError("cannot convert typetracer arrays to Python lists")
-            )
+            raise TypeError("cannot convert typetracer arrays to Python lists")
 
         out = self._to_list_custom(behavior, json_conversions)
         if out is not None:
             return out
 
         index = self._index.raw(numpy)
         not_missing = index >= 0
```

### Comparing `awkward-2.1.1/src/awkward/contents/listarray.py` & `awkward-2.1.2/src/awkward/contents/listarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 import copy
 
 import awkward as ak
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import TypeTracer
+from awkward._parameters import (
+    parameters_intersect,
+    type_parameters_equal,
+)
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
+from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 from awkward._util import unset
 from awkward.contents.content import Content
 from awkward.contents.listoffsetarray import ListOffsetArray
-from awkward.forms.form import _type_parameters_equal
 from awkward.forms.listform import ListForm
 from awkward.index import Index
-from awkward.typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 
 
@@ -101,66 +104,52 @@
 
     def __init__(self, starts, stops, content, *, parameters=None):
         if not isinstance(starts, Index) and starts.dtype in (
             np.dtype(np.int32),
             np.dtype(np.uint32),
             np.dtype(np.int64),
         ):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'starts' must be an Index with dtype in (int32, uint32, int64), "
-                    "not {}".format(type(self).__name__, repr(starts))
-                )
+            raise TypeError(
+                "{} 'starts' must be an Index with dtype in (int32, uint32, int64), "
+                "not {}".format(type(self).__name__, repr(starts))
             )
         if not (isinstance(stops, Index) and starts.dtype == stops.dtype):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'stops' must be an Index with the same dtype as 'starts' ({}), "
-                    "not {}".format(
-                        type(self).__name__, repr(starts.dtype), repr(stops)
-                    )
-                )
+            raise TypeError(
+                "{} 'stops' must be an Index with the same dtype as 'starts' ({}), "
+                "not {}".format(type(self).__name__, repr(starts.dtype), repr(stops))
             )
         if not isinstance(content, Content):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'content' must be a Content subtype, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} 'content' must be a Content subtype, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
         if (
             starts.nplike.known_data
             and stops.nplike.known_data
             and starts.length > stops.length
         ):
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "{} len(starts) ({}) must be <= len(stops) ({})".format(
-                        type(self).__name__, starts.length, stops.length
-                    )
+            raise ValueError(
+                "{} len(starts) ({}) must be <= len(stops) ({})".format(
+                    type(self).__name__, starts.length, stops.length
                 )
             )
 
         if parameters is not None and parameters.get("__array__") == "string":
             if not content.is_numpy or not content.parameter("__array__") == "char":
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "{} is a string, so its 'content' must be uint8 NumpyArray of char, not {}".format(
-                            type(self).__name__, repr(content)
-                        )
+                raise ValueError(
+                    "{} is a string, so its 'content' must be uint8 NumpyArray of char, not {}".format(
+                        type(self).__name__, repr(content)
                     )
                 )
         if parameters is not None and parameters.get("__array__") == "bytestring":
             if not content.is_numpy or not content.parameter("__array__") == "byte":
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "{} is a bytestring, so its 'content' must be uint8 NumpyArray of byte, not {}".format(
-                            type(self).__name__, repr(content)
-                        )
+                raise ValueError(
+                    "{} is a bytestring, so its 'content' must be uint8 NumpyArray of byte, not {}".format(
+                        type(self).__name__, repr(content)
                     )
                 )
 
         assert starts.nplike is content.backend.index_nplike
         assert stops.nplike is content.backend.index_nplike
 
         self._starts = starts
@@ -629,39 +618,33 @@
                 if largeoffsets.nplike.known_data:
                     missing_trim = missing[0 : largeoffsets[-1]]
                 else:
                     missing_trim = missing
                 out = ak.contents.IndexedOptionArray.simplified(
                     missing_trim, content, parameters=self._parameters
                 )
-                if isinstance(self._backend.nplike, TypeTracer):
-                    out = out.to_typetracer()
                 return ak.contents.ListOffsetArray(
                     largeoffsets,
                     out,
                     parameters=self._parameters,
                 )
             else:
-                raise ak._errors.wrap_error(
-                    AssertionError(
-                        "expected ListOffsetArray from ListArray._getitem_next_jagged, got {}".format(
-                            type(out).__name__
-                        )
+                raise AssertionError(
+                    "expected ListOffsetArray from ListArray._getitem_next_jagged, got {}".format(
+                        type(out).__name__
                     )
                 )
 
         elif isinstance(slicecontent, ak.contents.EmptyArray):
             return self
 
         else:
-            raise ak._errors.wrap_error(
-                AssertionError(
-                    "expected Index/IndexedOptionArray/ListOffsetArray in ListArray._getitem_next_jagged, got {}".format(
-                        type(slicecontent).__name__
-                    )
+            raise AssertionError(
+                "expected Index/IndexedOptionArray/ListOffsetArray in ListArray._getitem_next_jagged, got {}".format(
+                    type(slicecontent).__name__
                 )
             )
 
     def _getitem_next(
         self,
         head: SliceItem | tuple,
         tail: tuple[SliceItem, ...],
@@ -1016,28 +999,28 @@
                 down, headlength, 1, parameters=self._parameters
             )
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             return self._getitem_next_missing(head, tail, advanced)
 
         else:
-            raise ak._errors.wrap_error(AssertionError(repr(head)))
+            raise AssertionError(repr(head))
 
     def _offsets_and_flattened(self, axis, depth):
         return self.to_ListOffsetArray64(True)._offsets_and_flattened(axis, depth)
 
     def _mergeable_next(self, other, mergebool):
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # Check against option contents
         elif other.is_option or other.is_indexed:
             return self._mergeable_next(other.content, mergebool)
         # Otherwise, do the parameters match? If not, we can't merge.
-        elif not _type_parameters_equal(self._parameters, other._parameters):
+        elif not type_parameters_equal(self._parameters, other._parameters):
             return False
         elif isinstance(
             other,
             (
                 ak.contents.RegularArray,
                 ak.contents.ListArray,
                 ak.contents.ListOffsetArray,
@@ -1063,35 +1046,31 @@
 
         parameters = self._parameters
 
         for array in head:
             if isinstance(array, ak.contents.EmptyArray):
                 continue
 
-            parameters = ak.forms.form._parameters_intersect(
-                parameters, array._parameters
-            )
+            parameters = parameters_intersect(parameters, array._parameters)
             if isinstance(
                 array,
                 (
                     ak.contents.ListArray,
                     ak.contents.ListOffsetArray,
                     ak.contents.RegularArray,
                 ),
             ):
                 contents.append(array.content)
             else:
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "cannot merge "
-                        + type(self).__name__
-                        + " with "
-                        + type(array).__name__
-                        + "."
-                    )
+                raise ValueError(
+                    "cannot merge "
+                    + type(self).__name__
+                    + " with "
+                    + type(array).__name__
+                    + "."
                 )
 
         tail_contents = contents[1:]
         nextcontent = contents[0]._mergemany(tail_contents)
 
         nextstarts = ak.index.Index64.empty(total_length, self._backend.index_nplike)
         nextstops = ak.index.Index64.empty(total_length, self._backend.index_nplike)
@@ -1524,24 +1503,22 @@
         )
 
         if isinstance(result, Content):
             return result
         elif result is None:
             return continuation()
         else:
-            raise ak._errors.wrap_error(AssertionError(result))
+            raise AssertionError(result)
 
     def to_packed(self) -> Self:
         return self.to_ListOffsetArray64(True).to_packed()
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
-            raise ak._errors.wrap_error(
-                TypeError("cannot convert typetracer arrays to Python lists")
-            )
+            raise TypeError("cannot convert typetracer arrays to Python lists")
 
         return ListOffsetArray._to_list(self, behavior, json_conversions)
 
     def _to_backend(self, backend: ak._backends.Backend) -> Self:
         content = self._content.to_backend(backend)
         starts = self._starts.to_nplike(backend.index_nplike)
         stops = self._stops.to_nplike(backend.index_nplike)
```

### Comparing `awkward-2.1.1/src/awkward/contents/listoffsetarray.py` & `awkward-2.1.2/src/awkward/contents/listoffsetarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 
 import awkward as ak
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import TypeTracer, is_unknown_scalar
+from awkward._parameters import (
+    type_parameters_equal,
+)
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
+from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 from awkward._util import unset
 from awkward.contents.content import Content
-from awkward.forms.form import _type_parameters_equal
 from awkward.forms.listoffsetform import ListOffsetForm
 from awkward.index import Index
-from awkward.typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
@@ -94,53 +96,43 @@
 
     def __init__(self, offsets, content, *, parameters=None):
         if not isinstance(offsets, Index) and offsets.dtype in (
             np.dtype(np.int32),
             np.dtype(np.uint32),
             np.dtype(np.int64),
         ):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'offsets' must be an Index with dtype in (int32, uint32, int64), "
-                    "not {}".format(type(self).__name__, repr(offsets))
-                )
+            raise TypeError(
+                "{} 'offsets' must be an Index with dtype in (int32, uint32, int64), "
+                "not {}".format(type(self).__name__, repr(offsets))
             )
         if not isinstance(content, Content):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'content' must be a Content subtype, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} 'content' must be a Content subtype, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
         if offsets.length is not unknown_length and offsets.length == 0:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "{} len(offsets) ({}) must be >= 1".format(
-                        type(self).__name__, offsets.length
-                    )
+            raise ValueError(
+                "{} len(offsets) ({}) must be >= 1".format(
+                    type(self).__name__, offsets.length
                 )
             )
 
         if parameters is not None and parameters.get("__array__") == "string":
             if not content.is_numpy or not content.parameter("__array__") == "char":
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "{} is a string, so its 'content' must be uint8 NumpyArray of char, not {}".format(
-                            type(self).__name__, repr(content)
-                        )
+                raise ValueError(
+                    "{} is a string, so its 'content' must be uint8 NumpyArray of char, not {}".format(
+                        type(self).__name__, repr(content)
                     )
                 )
         if parameters is not None and parameters.get("__array__") == "bytestring":
             if not content.is_numpy or not content.parameter("__array__") == "byte":
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "{} is a bytestring, so its 'content' must be uint8 NumpyArray of byte, not {}".format(
-                            type(self).__name__, repr(content)
-                        )
+                raise ValueError(
+                    "{} is a bytestring, so its 'content' must be uint8 NumpyArray of byte, not {}".format(
+                        type(self).__name__, repr(content)
                     )
                 )
 
         assert offsets.nplike is content.backend.index_nplike
 
         self._offsets = offsets
         self._content = content
@@ -372,28 +364,24 @@
                 self._offsets.dtype.type,
             ](out.data, self._offsets.data, offsets_len)
         )
         return out
 
     def _broadcast_tooffsets64(self, offsets):
         if offsets.nplike.known_data and (offsets.length == 0 or offsets[0] != 0):
-            raise ak._errors.wrap_error(
-                AssertionError(
-                    "broadcast_tooffsets64 can only be used with offsets that start at 0, not {}".format(
-                        "(empty)" if offsets.length == 0 else str(offsets[0])
-                    )
+            raise AssertionError(
+                "broadcast_tooffsets64 can only be used with offsets that start at 0, not {}".format(
+                    "(empty)" if offsets.length == 0 else str(offsets[0])
                 )
             )
 
         if offsets.nplike.known_data and offsets.length - 1 != self.length:
-            raise ak._errors.wrap_error(
-                AssertionError(
-                    "cannot broadcast {} of length {} to length {}".format(
-                        type(self).__name__, self.length, offsets.length - 1
-                    )
+            raise AssertionError(
+                "cannot broadcast {} of length {} to length {}".format(
+                    type(self).__name__, self.length, offsets.length - 1
                 )
             )
 
         starts, stops = self.starts, self.stops
 
         nextcarry = ak.index.Index64.empty(offsets[-1], self._backend.index_nplike)
         assert (
@@ -710,20 +698,20 @@
             )
             return listarray._getitem_next(head, tail, advanced)
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             return self._getitem_next_missing(head, tail, advanced)
 
         else:
-            raise ak._errors.wrap_error(AssertionError(repr(head)))
+            raise AssertionError(repr(head))
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise ak._errors.wrap_error(np.AxisError("axis=0 not allowed for flatten"))
+            raise np.AxisError("axis=0 not allowed for flatten")
 
         elif posaxis is not None and posaxis + 1 == depth + 1:
             listoffsetarray = self.to_ListOffsetArray64(True)
             stop = listoffsetarray.offsets[-1]
             content = listoffsetarray.content._getitem_range(0, stop)
             return (listoffsetarray.offsets, content)
 
@@ -788,15 +776,15 @@
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # Check against option contents
         elif other.is_option or other.is_indexed:
             return self._mergeable_next(other.content, mergebool)
         # Otherwise, do the parameters match? If not, we can't merge.
-        elif not _type_parameters_equal(self._parameters, other._parameters):
+        elif not type_parameters_equal(self._parameters, other._parameters):
             return False
         elif isinstance(
             other,
             (
                 ak.contents.RegularArray,
                 ak.contents.ListArray,
                 ak.contents.ListOffsetArray,
@@ -878,18 +866,16 @@
         branch, depth = self.branch_depth
 
         if (
             self.parameter("__array__") == "string"
             or self.parameter("__array__") == "bytestring"
         ):
             if branch or (negaxis is not None and negaxis != depth):
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "array with strings can only be checked on uniqueness with axis=-1"
-                    )
+                raise ValueError(
+                    "array with strings can only be checked on uniqueness with axis=-1"
                 )
 
             # FIXME: check validity error
 
             if isinstance(self._content, ak.contents.NumpyArray):
                 out, outoffsets = self._content._as_unique_strings(self._offsets)
                 out2 = ak.contents.ListOffsetArray(
@@ -933,34 +919,30 @@
         branch, depth = self.branch_depth
 
         if (
             self.parameter("__array__") == "string"
             or self.parameter("__array__") == "bytestring"
         ):
             if branch or (negaxis != depth):
-                raise ak._errors.wrap_error(
-                    np.AxisError("array with strings can only be sorted with axis=-1")
-                )
+                raise np.AxisError("array with strings can only be sorted with axis=-1")
 
             # FIXME: check validity error
 
             if isinstance(self._content, ak.contents.NumpyArray):
                 out, nextoffsets = self._content._as_unique_strings(self._offsets)
                 return ak.contents.ListOffsetArray(
                     nextoffsets, out, parameters=self._parameters
                 )
 
         if not branch and (negaxis == depth):
             if (
                 self.parameter("__array__") == "string"
                 or self.parameter("__array__") == "bytestring"
             ):
-                raise ak._errors.wrap_error(
-                    np.AxisError("array with strings can only be sorted with axis=-1")
-                )
+                raise np.AxisError("array with strings can only be sorted with axis=-1")
 
             if self._backend.nplike.known_data and parents.nplike.known_data:
                 assert self._offsets.length - 1 == parents.length
 
             (
                 distincts,
                 maxcount,
@@ -1053,17 +1035,15 @@
         branch, depth = self.branch_depth
 
         if (
             self.parameter("__array__") == "string"
             or self.parameter("__array__") == "bytestring"
         ):
             if branch or (negaxis != depth):
-                raise ak._errors.wrap_error(
-                    np.AxisError("array with strings can only be sorted with axis=-1")
-                )
+                raise np.AxisError("array with strings can only be sorted with axis=-1")
 
             # FIXME: check validity error
 
             if isinstance(self._content, ak.contents.NumpyArray):
                 nextcarry = ak.index.Index64.empty(
                     self._offsets.length - 1, self._backend.index_nplike
                 )
@@ -1101,17 +1081,15 @@
                 )
 
         if not branch and (negaxis == depth):
             if (
                 self.parameter("__array__") == "string"
                 or self.parameter("__array__") == "bytestring"
             ):
-                raise ak._errors.wrap_error(
-                    np.AxisError("array with strings can only be sorted with axis=-1")
-                )
+                raise np.AxisError("array with strings can only be sorted with axis=-1")
 
             if self._backend.nplike.known_data and parents.nplike.known_data:
                 assert self._offsets.length - 1 == parents.length
 
             (
                 distincts,
                 maxcount,
@@ -1242,17 +1220,15 @@
         index_nplike = self._backend.index_nplike
 
         if (
             self.parameter("__array__") == "string"
             or self.parameter("__array__") == "bytestring"
         ):
             if branch or (negaxis != depth):
-                raise ak._errors.wrap_error(
-                    np.AxisError("array with strings can only be sorted with axis=-1")
-                )
+                raise np.AxisError("array with strings can only be sorted with axis=-1")
 
             # FIXME: check validity error
 
             if isinstance(self._content, ak.contents.NumpyArray):
                 nextcarry = ak.index.Index64.empty(
                     self._offsets.length - 1, index_nplike
                 )
@@ -1288,17 +1264,15 @@
                 return self._carry(nextcarry, False)
 
         if not branch and (negaxis == depth):
             if (
                 self.parameter("__array__") == "string"
                 or self.parameter("__array__") == "bytestring"
             ):
-                raise ak._errors.wrap_error(
-                    np.AxisError("array with strings can only be sorted with axis=-1")
-                )
+                raise np.AxisError("array with strings can only be sorted with axis=-1")
 
             if self._backend.nplike.known_data and parents.nplike.known_data:
                 assert self._offsets.length - 1 == parents.length
 
             (
                 distincts,
                 maxcount,
@@ -1381,18 +1355,16 @@
         if posaxis is not None and posaxis + 1 == depth:
             return self._combinations_axis0(n, replacement, recordlookup, parameters)
         elif posaxis is not None and posaxis + 1 == depth + 1:
             if (
                 self.parameter("__array__") == "string"
                 or self.parameter("__array__") == "bytestring"
             ):
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "ak.combinations does not compute combinations of the characters of a string; please split it into lists"
-                    )
+                raise ValueError(
+                    "ak.combinations does not compute combinations of the characters of a string; please split it into lists"
                 )
 
             starts = self.starts
             stops = self.stops
 
             _totallen = ak.index.Index64.empty(1, index_nplike, dtype=np.int64)
             offsets = ak.index.Index64.empty(
@@ -2145,15 +2117,15 @@
         )
 
         if isinstance(result, Content):
             return result
         elif result is None:
             return continuation()
         else:
-            raise ak._errors.wrap_error(AssertionError(result))
+            raise AssertionError(result)
 
     def to_packed(self) -> Self:
         next = self.to_ListOffsetArray64(True)
         content = next._content.to_packed()
         packed_length = self._backend.index_nplike.index_as_shape_item(
             next._offsets[-1]
         )
@@ -2163,17 +2135,15 @@
             and content.length != packed_length
         ):
             content = content[: next._offsets[-1]]
         return ListOffsetArray(next._offsets, content, parameters=next._parameters)
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
-            raise ak._errors.wrap_error(
-                TypeError("cannot convert typetracer arrays to Python lists")
-            )
+            raise TypeError("cannot convert typetracer arrays to Python lists")
 
         starts, stops = self.starts, self.stops
         starts_data = starts.raw(numpy)
         stops_data = stops.raw(numpy)[: len(starts_data)]
 
         nonempty = starts_data != stops_data
         if numpy.count_nonzero(nonempty) == 0:
```

### Comparing `awkward-2.1.1/src/awkward/contents/numpyarray.py` & `awkward-2.1.2/src/awkward/contents/numpyarray.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,26 @@
 import awkward as ak
 from awkward._layout import maybe_posaxis
 from awkward._nplikes import to_nplike
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import ArrayLike, IndexType, NumpyMetadata
 from awkward._nplikes.typetracer import TypeTracerArray
+from awkward._parameters import (
+    parameters_intersect,
+    type_parameters_equal,
+)
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
+from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 from awkward._util import unset
 from awkward.contents.content import Content
-from awkward.forms.form import _type_parameters_equal
 from awkward.forms.numpyform import NumpyForm
 from awkward.index import Index
 from awkward.types.numpytype import primitive_to_dtype
-from awkward.typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
@@ -94,29 +97,25 @@
 
         self._data = backend.nplike.asarray(data)
 
         if not isinstance(backend.nplike, Jax):
             ak.types.numpytype.dtype_to_primitive(self._data.dtype)
 
         if len(self._data.shape) == 0:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'data' must be an array, not a scalar: {}".format(
-                        type(self).__name__, repr(data)
-                    )
+            raise TypeError(
+                "{} 'data' must be an array, not a scalar: {}".format(
+                    type(self).__name__, repr(data)
                 )
             )
 
         if parameters is not None and parameters.get("__array__") in ("char", "byte"):
             if data.dtype != np.dtype(np.uint8) or len(data.shape) != 1:
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "{} is a {}, so its 'data' must be 1-dimensional and uint8, not {}".format(
-                            type(self).__name__, parameters["__array__"], repr(data)
-                        )
+                raise ValueError(
+                    "{} is a {}, so its 'data' must be 1-dimensional and uint8, not {}".format(
+                        type(self).__name__, parameters["__array__"], repr(data)
                     )
                 )
 
         self._init(parameters, backend)
 
     @property
     def data(self) -> ArrayLike:
@@ -397,38 +396,36 @@
             return NumpyArray(out, parameters=self._parameters, backend=self._backend)
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             next = self.to_RegularArray()
             return next._getitem_next_missing(head, tail, advanced)
 
         else:
-            raise ak._errors.wrap_error(AssertionError(repr(head)))
+            raise AssertionError(repr(head))
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise ak._errors.wrap_error(np.AxisError("axis=0 not allowed for flatten"))
+            raise np.AxisError("axis=0 not allowed for flatten")
 
         elif len(self.shape) != 1:
             return self.to_RegularArray()._offsets_and_flattened(axis, depth)
 
         else:
-            raise ak._errors.wrap_error(
-                np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
-            )
+            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
 
     def _mergeable_next(self, other, mergebool):
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # Check against option contents
         elif other.is_option or other.is_indexed:
             return self._mergeable_next(other.content, mergebool)
         # Otherwise, do the parameters match? If not, we can't merge.
-        elif not _type_parameters_equal(self._parameters, other._parameters):
+        elif not type_parameters_equal(self._parameters, other._parameters):
             return False
         # Simplify *this* branch to be 1D self
         elif len(self.shape) > 1:
             return self._to_regular_primitive()._mergeable_next(other, mergebool)
 
         elif isinstance(other, ak.contents.NumpyArray):
             if self._data.ndim != other._data.ndim:
@@ -477,27 +474,23 @@
         contiguous_arrays = []
 
         parameters = self._parameters
         for array in head:
             if isinstance(array, ak.contents.EmptyArray):
                 continue
 
-            parameters = ak.forms.form._parameters_intersect(
-                parameters, array._parameters
-            )
+            parameters = parameters_intersect(parameters, array._parameters)
             if isinstance(array, ak.contents.NumpyArray):
                 contiguous_arrays.append(array.data)
             else:
-                raise ak._errors.wrap_error(
-                    AssertionError(
-                        "cannot merge "
-                        + type(self).__name__
-                        + " with "
-                        + type(array).__name__
-                    )
+                raise AssertionError(
+                    "cannot merge "
+                    + type(self).__name__
+                    + " with "
+                    + type(array).__name__
                 )
 
         contiguous_arrays = self._backend.nplike.concat(contiguous_arrays)
 
         next = NumpyArray(
             contiguous_arrays, parameters=parameters, backend=self._backend
         )
@@ -515,17 +508,15 @@
         return self
 
     def _local_index(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             return self._local_index_axis0()
         elif len(self.shape) <= 1:
-            raise ak._errors.wrap_error(
-                np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
-            )
+            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
         else:
             return self.to_RegularArray()._local_index(axis, depth)
 
     def to_contiguous(self) -> Self:
         if self.is_contiguous:
             return self
         else:
@@ -880,17 +871,15 @@
                 outoffsets, ak.contents.NumpyArray(out), parameters=self._parameters
             )
 
     def _argsort_next(
         self, negaxis, starts, shifts, parents, outlength, ascending, stable
     ):
         if len(self.shape) == 0:
-            raise ak._errors.wrap_error(
-                TypeError(f"{type(self).__name__} attempting to argsort a scalar ")
-            )
+            raise TypeError(f"{type(self).__name__} attempting to argsort a scalar ")
         elif len(self.shape) != 1 or not self.is_contiguous:
             contiguous_self = self.to_contiguous()
             return contiguous_self.to_RegularArray()._argsort_next(
                 negaxis, starts, shifts, parents, outlength, ascending, stable
             )
 
         else:
@@ -989,17 +978,15 @@
                     )
                 )
             out = NumpyArray(nextcarry.data, parameters=None, backend=self._backend)
             return out
 
     def _sort_next(self, negaxis, starts, parents, outlength, ascending, stable):
         if len(self.shape) == 0:
-            raise ak._errors.wrap_error(
-                TypeError(f"{type(self).__name__} attempting to sort a scalar ")
-            )
+            raise TypeError(f"{type(self).__name__} attempting to sort a scalar ")
 
         elif len(self.shape) != 1 or not self.is_contiguous:
             contiguous_self = self.to_contiguous()
             return contiguous_self.to_RegularArray()._sort_next(
                 negaxis, starts, parents, outlength, ascending, stable
             )
 
@@ -1075,17 +1062,15 @@
             )
 
     def _combinations(self, n, replacement, recordlookup, parameters, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
             return self._combinations_axis0(n, replacement, recordlookup, parameters)
         elif len(self.shape) <= 1:
-            raise ak._errors.wrap_error(
-                np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
-            )
+            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
         else:
             return self.to_RegularArray()._combinations(
                 n, replacement, recordlookup, parameters, axis, depth
             )
 
     def _reduce_next(
         self,
@@ -1208,24 +1193,20 @@
         for i, stride in enumerate(self.strides):
             if stride % self.dtype.itemsize != 0:
                 return f"at {path} ({type(self)!r}): shape[{i}] % itemsize != 0"
         return ""
 
     def _pad_none(self, target, axis, depth, clip):
         if len(self.shape) == 0:
-            raise ak._errors.wrap_error(
-                ValueError("cannot apply ak.pad_none to a scalar")
-            )
+            raise ValueError("cannot apply ak.pad_none to a scalar")
         elif len(self.shape) > 1 or not self.is_contiguous:
             return self.to_RegularArray()._pad_none(target, axis, depth, clip)
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 != depth:
-            raise ak._errors.wrap_error(
-                np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
-            )
+            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
         if not clip:
             if target < self.length:
                 return self
             else:
                 return self._pad_none(target, axis, depth, clip=True)
         else:
             return self._pad_none_axis0(target, clip=True)
@@ -1313,24 +1294,22 @@
         )
 
         if isinstance(result, Content):
             return result
         elif result is None:
             return continuation()
         else:
-            raise ak._errors.wrap_error(AssertionError(result))
+            raise AssertionError(result)
 
     def to_packed(self) -> Self:
         return self.to_contiguous().to_RegularArray()
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
-            raise ak._errors.wrap_error(
-                TypeError("cannot convert typetracer arrays to Python lists")
-            )
+            raise TypeError("cannot convert typetracer arrays to Python lists")
 
         if self.parameter("__array__") == "byte":
             convert_bytes = (
                 None if json_conversions is None else json_conversions["convert_bytes"]
             )
             if convert_bytes is None:
                 return ak._util.tobytes(self._data)
```

### Comparing `awkward-2.1.1/src/awkward/contents/recordarray.py` & `awkward-2.1.2/src/awkward/contents/recordarray.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 
 import awkward as ak
 from awkward._behavior import find_record_reducer
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
+from awkward._parameters import (
+    parameters_intersect,
+    type_parameters_equal,
+)
 from awkward._regularize import is_integer
 from awkward._slicing import NO_HEAD
+from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 from awkward._util import unset
 from awkward.contents.content import Content
-from awkward.forms.form import _type_parameters_equal
 from awkward.forms.recordform import RecordForm
 from awkward.index import Index
 from awkward.record import Record
-from awkward.typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
@@ -129,57 +132,49 @@
         *,
         parameters=None,
         backend=None,
     ):
         if not (length is None or length is unknown_length):
             length = int(length)  # TODO: this should not happen!
         if not isinstance(contents, Iterable):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'contents' must be iterable, not {}".format(
-                        type(self).__name__, repr(contents)
-                    )
+            raise TypeError(
+                "{} 'contents' must be iterable, not {}".format(
+                    type(self).__name__, repr(contents)
                 )
             )
         if not isinstance(contents, list):
             contents = list(contents)
 
         for content in contents:
             if not isinstance(content, Content):
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} all 'contents' must be Content subclasses, not {}".format(
-                            type(self).__name__, repr(content)
-                        )
+                raise TypeError(
+                    "{} all 'contents' must be Content subclasses, not {}".format(
+                        type(self).__name__, repr(content)
                     )
                 )
             if backend is None:
                 backend = content.backend
             elif backend is not content.backend:
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} 'contents' must use the same array library (backend): {} vs {}".format(
-                            type(self).__name__,
-                            type(backend).__name__,
-                            type(content.backend).__name__,
-                        )
+                raise TypeError(
+                    "{} 'contents' must use the same array library (backend): {} vs {}".format(
+                        type(self).__name__,
+                        type(backend).__name__,
+                        type(content.backend).__name__,
                     )
                 )
 
         # If no content backend was found, then choose our own
         if backend is None:
             backend = ak._backends.NumpyBackend.instance()
 
         if length is None:
             if len(contents) == 0:
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} if len(contents) == 0, a 'length' must be specified".format(
-                            type(self).__name__
-                        )
+                raise TypeError(
+                    "{} if len(contents) == 0, a 'length' must be specified".format(
+                        type(self).__name__
                     )
                 )
 
             if backend.nplike.known_data:
                 for content in contents:
                     assert content.length is not unknown_length
                     # First time we're setting length, and content.length is not unknown_length
@@ -202,56 +197,46 @@
                         break
                     # `length` is set, can't be unknown_length
                     else:
                         length = min(length, content.length)
         elif length is not unknown_length:
             for content in contents:
                 if content.length is not unknown_length and content.length < length:
-                    raise ak._errors.wrap_error(
-                        ValueError(
-                            "{} len(content) ({}) must be >= length ({}) for all 'contents'".format(
-                                type(self).__name__, content.length, length
-                            )
+                    raise ValueError(
+                        "{} len(content) ({}) must be >= length ({}) for all 'contents'".format(
+                            type(self).__name__, content.length, length
                         )
                     )
 
             if not (is_integer(length) and length >= 0):
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} 'length' must be a non-negative integer or None, not {}".format(
-                            type(self).__name__, repr(length)
-                        )
+                raise TypeError(
+                    "{} 'length' must be a non-negative integer or None, not {}".format(
+                        type(self).__name__, repr(length)
                     )
                 )
 
         if isinstance(fields, Iterable):
             if not isinstance(fields, list):
                 fields = list(fields)
             if not all(isinstance(x, str) for x in fields):
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} 'fields' must all be strings, not {}".format(
-                            type(self).__name__, repr(fields)
-                        )
+                raise TypeError(
+                    "{} 'fields' must all be strings, not {}".format(
+                        type(self).__name__, repr(fields)
                     )
                 )
             if not len(contents) == len(fields):
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "{} len(contents) ({}) must be equal to len(fields) ({})".format(
-                            type(self).__name__, len(contents), len(fields)
-                        )
+                raise ValueError(
+                    "{} len(contents) ({}) must be equal to len(fields) ({})".format(
+                        type(self).__name__, len(contents), len(fields)
                     )
                 )
         elif fields is not None:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'fields' must be an iterable or None, not {}".format(
-                        type(self).__name__, repr(fields)
-                    )
+            raise TypeError(
+                "{} 'fields' must be an iterable or None, not {}".format(
+                    type(self).__name__, repr(fields)
                 )
             )
 
         self._contents = contents
         self._fields = fields
         self._length = length
         self._init(parameters, backend)
@@ -603,33 +588,29 @@
                 backend=self._backend,
             )
             return next._getitem_next(nexthead, nexttail, advanced)
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise ak._errors.wrap_error(np.AxisError("axis=0 not allowed for flatten"))
+            raise np.AxisError("axis=0 not allowed for flatten")
 
         elif posaxis is not None and posaxis + 1 == depth + 1:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "arrays of records cannot be flattened (but their contents can be; try a different 'axis')"
-                )
+            raise ValueError(
+                "arrays of records cannot be flattened (but their contents can be; try a different 'axis')"
             )
 
         else:
             contents = []
             for content in self._contents:
                 trimmed = content._getitem_range(0, self.length)
                 offsets, flattened = trimmed._offsets_and_flattened(axis, depth)
                 if self._backend.nplike.known_data and offsets.length != 0:
-                    raise ak._errors.wrap_error(
-                        AssertionError(
-                            "RecordArray content with axis > depth + 1 returned a non-empty offsets from offsets_and_flattened"
-                        )
+                    raise AssertionError(
+                        "RecordArray content with axis > depth + 1 returned a non-empty offsets from offsets_and_flattened"
                     )
                 contents.append(flattened)
             offsets = ak.index.Index64.zeros(
                 1,
                 nplike=self._backend.index_nplike,
                 dtype=np.int64,
             )
@@ -648,15 +629,15 @@
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # Check against option contents
         elif other.is_option or other.is_indexed:
             return self._mergeable_next(other.content, mergebool)
         # Otherwise, do the parameters match? If not, we can't merge.
-        elif not _type_parameters_equal(self._parameters, other._parameters):
+        elif not type_parameters_equal(self._parameters, other._parameters):
             return False
         elif isinstance(other, RecordArray):
             if self.is_tuple and other.is_tuple:
                 if len(self._contents) == len(other._contents):
                     for self_cont, other_cont in zip(self._contents, other._contents):
                         if not self_cont._mergeable_next(other_cont, mergebool):
                             return False
@@ -695,85 +676,69 @@
             for_each_field.append([trimmed])
 
         if self.is_tuple:
             for array in headless:
                 if isinstance(array, ak.contents.EmptyArray):
                     continue
 
-                parameters = ak.forms.form._parameters_intersect(
-                    parameters, array._parameters
-                )
+                parameters = parameters_intersect(parameters, array._parameters)
 
                 if isinstance(array, ak.contents.RecordArray):
                     if self.is_tuple:
                         if len(self.contents) == len(array.contents):
                             for i in range(len(self.contents)):
                                 field = array[self.index_to_field(i)]
                                 for_each_field[i].append(field[0 : array.length])
                         else:
-                            raise ak._errors.wrap_error(
-                                ValueError(
-                                    "cannot merge tuples with different numbers of fields"
-                                )
+                            raise ValueError(
+                                "cannot merge tuples with different numbers of fields"
                             )
                     else:
-                        raise ak._errors.wrap_error(
-                            ValueError("cannot merge tuple with non-tuple record")
-                        )
+                        raise ValueError("cannot merge tuple with non-tuple record")
                 else:
-                    raise ak._errors.wrap_error(
-                        AssertionError(
-                            "cannot merge "
-                            + type(self).__name__
-                            + " with "
-                            + type(array).__name__
-                        )
+                    raise AssertionError(
+                        "cannot merge "
+                        + type(self).__name__
+                        + " with "
+                        + type(array).__name__
                     )
 
         else:
             these_fields = self._fields.copy()
             these_fields.sort()
 
             for array in headless:
-                parameters = ak.forms.form._parameters_intersect(
-                    parameters, array._parameters
-                )
+                parameters = parameters_intersect(parameters, array._parameters)
 
                 if isinstance(array, ak.contents.RecordArray):
                     if not array.is_tuple:
                         those_fields = array._fields.copy()
                         those_fields.sort()
 
                         if these_fields == those_fields:
                             for i in range(len(self.contents)):
                                 field = array[self.index_to_field(i)]
 
                                 trimmed = field[0 : array.length]
                                 for_each_field[i].append(trimmed)
                         else:
-                            raise ak._errors.wrap_error(
-                                AssertionError(
-                                    "cannot merge records with different sets of field names"
-                                )
+                            raise AssertionError(
+                                "cannot merge records with different sets of field names"
                             )
                     else:
-                        raise ak._errors.wrap_error(
-                            AssertionError("cannot merge non-tuple record with tuple")
-                        )
+                        raise AssertionError("cannot merge non-tuple record with tuple")
 
                 elif isinstance(array, ak.contents.EmptyArray):
                     pass
                 else:
-                    raise ak._errors.wrap_error(
-                        AssertionError(
-                            "cannot merge "
-                            + type(self).__name__
-                            + " with "
-                            + type(array).__name__
-                        )
+                    raise AssertionError(
+                        "cannot merge "
+                        + type(self).__name__
+                        + " with "
+                        + type(array).__name__
                     )
 
         nextcontents = []
         minlength = ak._util.unset
         for forfield in for_each_field:
             merged = forfield[0]._mergemany(forfield[1:])
 
@@ -850,20 +815,20 @@
     def _is_unique(self, negaxis, starts, parents, outlength):
         for content in self._contents:
             if not content._is_unique(negaxis, starts, parents, outlength):
                 return False
         return True
 
     def _unique(self, negaxis, starts, parents, outlength):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _argsort_next(
         self, negaxis, starts, shifts, parents, outlength, ascending, stable
     ):
-        raise ak._errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _sort_next(self, negaxis, starts, parents, outlength, ascending, stable):
         if self._fields is None or len(self._fields) == 0:
             return ak.contents.NumpyArray(
                 self._backend.nplike.instance().empty(0, dtype=np.int64),
                 parameters=None,
                 backend=self._backend,
@@ -914,26 +879,22 @@
         outlength,
         mask,
         keepdims,
         behavior,
     ):
         reducer_recordclass = find_record_reducer(reducer, self, behavior)
         if reducer_recordclass is None:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "no ak.{} overloads for custom types: {}".format(
-                        reducer.name, ", ".join(self._fields)
-                    )
+            raise TypeError(
+                "no ak.{} overloads for custom types: {}".format(
+                    reducer.name, ", ".join(self._fields)
                 )
             )
         else:
-            raise ak._errors.wrap_error(
-                NotImplementedError(
-                    "overloading reducers for RecordArrays has not been implemented yet"
-                )
+            raise NotImplementedError(
+                "overloading reducers for RecordArrays has not been implemented yet"
             )
 
     def _validity_error(self, path):
         for i, cont in enumerate(self.contents):
             if cont.length < self.length:
                 return f"at {path} ({type(self)!r}): len(field({i})) < len(recordarray)"
         for i, cont in enumerate(self.contents):
@@ -1004,17 +965,15 @@
         )
 
     def _to_backend_array(self, allow_missing, backend):
         if self.fields is None:
             return backend.nplike.empty(self.length, dtype=[])
         contents = [x._to_backend_array(allow_missing, backend) for x in self._contents]
         if any(len(x.shape) != 1 for x in contents):
-            raise ak._errors.wrap_error(
-                ValueError(f"cannot convert {self} into np.ndarray")
-            )
+            raise ValueError(f"cannot convert {self} into np.ndarray")
         out = backend.nplike.empty(
             self.length,
             dtype=[(str(n), x.dtype) for n, x in zip(self.fields, contents)],
         )
         mask = None
         for n, x in zip(self.fields, contents):
             if allow_missing and isinstance(x, self._backend.nplike.ma.MaskedArray):
@@ -1037,22 +996,20 @@
             for content in self._contents:
                 out.extend(content[: self._length]._remove_structure(backend, options))
             return out
         else:
             in_function = ""
             if options["function_name"] is not None:
                 in_function = " in " + options["function_name"]
-            raise ak._errors.wrap_error(
-                TypeError(
-                    (
-                        "encountered a record whilst removing array structure{}, "
-                        "but this operation does not support erasing records. "
-                        "Try first calling `ak.ravel` or `ak.flatten(..., axis=None)."
-                    ).format(in_function)
-                )
+            raise TypeError(
+                (
+                    "encountered a record whilst removing array structure{}, "
+                    "but this operation does not support erasing records. "
+                    "Try first calling `ak.ravel` or `ak.flatten(..., axis=None)."
+                ).format(in_function)
             )
 
     def _recursively_apply(
         self, action, behavior, depth, depth_context, lateral_context, options
     ):
         if self._backend.nplike.known_data:
             contents = [x[: self._length] for x in self._contents]
@@ -1060,18 +1017,16 @@
             self._touch_data(recursive=False)
             contents = self._contents
 
         if options["return_array"]:
 
             def continuation():
                 if not options["allow_records"]:
-                    raise ak._errors.wrap_error(
-                        ValueError(
-                            f"cannot broadcast records in {options['function_name']}"
-                        )
+                    raise ValueError(
+                        f"cannot broadcast records in {options['function_name']}"
                     )
                 return RecordArray(
                     [
                         content._recursively_apply(
                             action,
                             behavior,
                             depth,
@@ -1112,15 +1067,15 @@
         )
 
         if isinstance(result, Content):
             return result
         elif result is None:
             return continuation()
         else:
-            raise ak._errors.wrap_error(AssertionError(result))
+            raise AssertionError(result)
 
     def to_packed(self) -> Self:
         return RecordArray(
             [
                 x.to_packed()
                 if x.length == self._length
                 else x[: self._length].to_packed()
@@ -1130,17 +1085,15 @@
             self._length,
             parameters=self._parameters,
             backend=self._backend,
         )
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
-            raise ak._errors.wrap_error(
-                TypeError("cannot convert typetracer arrays to Python lists")
-            )
+            raise TypeError("cannot convert typetracer arrays to Python lists")
 
         out = self._to_list_custom(behavior, json_conversions)
         if out is not None:
             return out
 
         if self.is_tuple and json_conversions is None:
             contents = [x._to_list(behavior, json_conversions) for x in self._contents]
```

### Comparing `awkward-2.1.1/src/awkward/contents/regulararray.py` & `awkward-2.1.2/src/awkward/contents/regulararray.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 import copy
 
 import awkward as ak
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
+from awkward._parameters import (
+    parameters_intersect,
+    parameters_union,
+    type_parameters_equal,
+)
 from awkward._regularize import is_integer, is_integer_like
 from awkward._slicing import NO_HEAD
+from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 from awkward._util import unset
 from awkward.contents.content import Content
-from awkward.forms.form import _type_parameters_equal
 from awkward.forms.regularform import RegularForm
 from awkward.index import Index
-from awkward.typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
@@ -96,75 +100,61 @@
     """
 
     is_list = True
     is_regular = True
 
     def __init__(self, content, size, zeros_length=0, *, parameters=None):
         if not isinstance(content, Content):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'content' must be a Content subtype, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} 'content' must be a Content subtype, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
         if size is unknown_length:
             if content.backend.index_nplike.known_data:
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} 'size' must be a non-negative integer for backends with known shapes, not None".format(
-                            type(self).__name__
-                        )
+                raise TypeError(
+                    "{} 'size' must be a non-negative integer for backends with known shapes, not None".format(
+                        type(self).__name__
                     )
                 )
         else:
             if not (is_integer(size) and size >= 0):
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} 'size' must be a non-negative integer, not {}".format(
-                            type(self).__name__, size
-                        )
+                raise TypeError(
+                    "{} 'size' must be a non-negative integer, not {}".format(
+                        type(self).__name__, size
                     )
                 )
 
         if zeros_length is unknown_length:
             if content.backend.index_nplike.known_data:
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} 'zeros_length' must be a non-negative integer for backends with known shapes, not None".format(
-                            type(self).__name__
-                        )
+                raise TypeError(
+                    "{} 'zeros_length' must be a non-negative integer for backends with known shapes, not None".format(
+                        type(self).__name__
                     )
                 )
         else:
             if not (is_integer(zeros_length) and zeros_length >= 0):
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} 'zeros_length' must be a non-negative integer, not {}".format(
-                            type(self).__name__, zeros_length
-                        )
+                raise TypeError(
+                    "{} 'zeros_length' must be a non-negative integer, not {}".format(
+                        type(self).__name__, zeros_length
                     )
                 )
 
         if parameters is not None and parameters.get("__array__") == "string":
             if not content.is_numpy or not content.parameter("__array__") == "char":
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "{} is a string, so its 'content' must be uint8 NumpyArray of char, not {}".format(
-                            type(self).__name__, repr(content)
-                        )
+                raise ValueError(
+                    "{} is a string, so its 'content' must be uint8 NumpyArray of char, not {}".format(
+                        type(self).__name__, repr(content)
                     )
                 )
         if parameters is not None and parameters.get("__array__") == "bytestring":
             if not content.is_numpy or not content.parameter("__array__") == "byte":
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "{} is a bytestring, so its 'content' must be uint8 NumpyArray of byte, not {}".format(
-                            type(self).__name__, repr(content)
-                        )
+                raise ValueError(
+                    "{} is a bytestring, so its 'content' must be uint8 NumpyArray of byte, not {}".format(
+                        type(self).__name__, repr(content)
                     )
                 )
 
         self._content = content
         self._size = size
         if content.length is unknown_length or size is unknown_length:
             self._length = unknown_length
@@ -276,17 +266,15 @@
     def maybe_to_NumpyArray(self) -> ak.contents.NumpyArray | None:
         content = self._content[: self._length * self._size].maybe_to_NumpyArray()
 
         if content is not None:
             shape = (self._length, self._size) + content.data.shape[1:]
             return ak.contents.NumpyArray(
                 self._backend.nplike.reshape(content.data, shape),
-                parameters=ak.forms.form._parameters_union(
-                    self._parameters, content.parameters
-                ),
+                parameters=parameters_union(self._parameters, content.parameters),
                 backend=content.backend,
             )
         else:
             return None
 
     def _getitem_nothing(self):
         return self._content._getitem_range(0, 0)
@@ -400,28 +388,24 @@
                 self._size,
             )
         )
         return out
 
     def _broadcast_tooffsets64(self, offsets):
         if offsets.nplike.known_data and (offsets.length == 0 or offsets[0] != 0):
-            raise ak._errors.wrap_error(
-                AssertionError(
-                    "broadcast_tooffsets64 can only be used with offsets that start at 0, not {}".format(
-                        "(empty)" if offsets.length == 0 else str(offsets[0])
-                    )
+            raise AssertionError(
+                "broadcast_tooffsets64 can only be used with offsets that start at 0, not {}".format(
+                    "(empty)" if offsets.length == 0 else str(offsets[0])
                 )
             )
 
         if offsets.nplike.known_data and offsets.length - 1 != self._length:
-            raise ak._errors.wrap_error(
-                AssertionError(
-                    "cannot broadcast RegularArray of length {} to length {}".format(
-                        self._length, offsets.length - 1
-                    )
+            raise AssertionError(
+                "cannot broadcast RegularArray of length {} to length {}".format(
+                    self._length, offsets.length - 1
                 )
             )
 
         if self._size == 1:
             carrylen = self._backend.index_nplike.index_as_shape_item(offsets[-1])
             nextcarry = ak.index.Index64.empty(carrylen, self._backend.index_nplike)
             assert (
@@ -712,28 +696,28 @@
                 down, headlength, self._length, parameters=self._parameters
             )
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             return self._getitem_next_missing(head, tail, advanced)
 
         else:
-            raise ak._errors.wrap_error(AssertionError(repr(head)))
+            raise AssertionError(repr(head))
 
     def _offsets_and_flattened(self, axis, depth):
         return self.to_ListOffsetArray64(True)._offsets_and_flattened(axis, depth)
 
     def _mergeable_next(self, other, mergebool):
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # Check against option contents
         elif other.is_option or other.is_indexed:
             return self._mergeable_next(other.content, mergebool)
         # Otherwise, do the parameters match? If not, we can't merge.
-        elif not _type_parameters_equal(self._parameters, other._parameters):
+        elif not type_parameters_equal(self._parameters, other._parameters):
             return False
         elif isinstance(
             other,
             (
                 ak.contents.RegularArray,
                 ak.contents.ListArray,
                 ak.contents.ListOffsetArray,
@@ -759,17 +743,15 @@
         ]
 
         if all(x.is_regular and x.size == self.size for x in others):
             parameters = self._parameters
             tail_contents = []
             zeros_length = self._length
             for x in others:
-                parameters = ak.forms.form._parameters_intersect(
-                    parameters, x._parameters
-                )
+                parameters = parameters_intersect(parameters, x._parameters)
                 tail_contents.append(x._content[: x._length * x._size])
                 zeros_length += x._length
 
             return RegularArray(
                 self._content[: self._length * self._size]._mergemany(tail_contents),
                 self._size,
                 zeros_length,
@@ -895,18 +877,16 @@
         if posaxis is not None and posaxis + 1 == depth:
             return self._combinations_axis0(n, replacement, recordlookup, parameters)
         elif posaxis is not None and posaxis + 1 == depth + 1:
             if (
                 self.parameter("__array__") == "string"
                 or self.parameter("__array__") == "bytestring"
             ):
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "ak.combinations does not compute combinations of the characters of a string; please split it into lists"
-                    )
+                raise ValueError(
+                    "ak.combinations does not compute combinations of the characters of a string; please split it into lists"
                 )
 
             size = self._size
             if replacement:
                 size = size + (n - 1)
             thisn = n
             if thisn > size:
@@ -1374,15 +1354,15 @@
         )
 
         if isinstance(result, Content):
             return result
         elif result is None:
             return continuation()
         else:
-            raise ak._errors.wrap_error(AssertionError(result))
+            raise AssertionError(result)
 
     def to_packed(self) -> Self:
         index_nplike = self._backend.index_nplike
         length = self._length * self._size
         if self._content.length == length:
             content = self._content.to_packed()
         else:
@@ -1392,17 +1372,15 @@
 
         return RegularArray(
             content, self._size, self._length, parameters=self._parameters
         )
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
-            raise ak._errors.wrap_error(
-                TypeError("cannot convert typetracer arrays to Python lists")
-            )
+            raise TypeError("cannot convert typetracer arrays to Python lists")
 
         if self.parameter("__array__") == "bytestring":
             convert_bytes = (
                 None if json_conversions is None else json_conversions["convert_bytes"]
             )
             content = ak._util.tobytes(self._content.data)
             length, size = self._length, self._size
```

### Comparing `awkward-2.1.1/src/awkward/contents/unionarray.py` & `awkward-2.1.2/src/awkward/contents/unionarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 import awkward as ak
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.jax import Jax
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.shape import unknown_length
 from awkward._nplikes.typetracer import OneOf, TypeTracer
+from awkward._parameters import parameters_intersect, parameters_union
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
+from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 from awkward._util import unset
 from awkward.contents.content import Content
 from awkward.forms.unionform import UnionForm
 from awkward.index import Index, Index8, Index64
-from awkward.typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
@@ -83,91 +84,75 @@
                     raise AssertionError(where)
     """
 
     is_union = True
 
     def __init__(self, tags, index, contents, *, parameters=None):
         if not (isinstance(tags, Index) and tags.dtype == np.dtype(np.int8)):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'tags' must be an Index with dtype=int8, not {}".format(
-                        type(self).__name__, repr(tags)
-                    )
+            raise TypeError(
+                "{} 'tags' must be an Index with dtype=int8, not {}".format(
+                    type(self).__name__, repr(tags)
                 )
             )
 
         if not isinstance(index, Index) and index.dtype in (
             np.dtype(np.int32),
             np.dtype(np.uint32),
             np.dtype(np.int64),
         ):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'index' must be an Index with dtype in (int32, uint32, int64), "
-                    "not {}".format(type(self).__name__, repr(index))
-                )
+            raise TypeError(
+                "{} 'index' must be an Index with dtype in (int32, uint32, int64), "
+                "not {}".format(type(self).__name__, repr(index))
             )
 
         if not isinstance(contents, Iterable):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'contents' must be iterable, not {}".format(
-                        type(self).__name__, repr(contents)
-                    )
+            raise TypeError(
+                "{} 'contents' must be iterable, not {}".format(
+                    type(self).__name__, repr(contents)
                 )
             )
         if not isinstance(contents, list):
             contents = list(contents)
 
         if len(contents) < 2:
-            raise ak._errors.wrap_error(
-                TypeError(f"{type(self).__name__} must have at least 2 'contents'")
-            )
+            raise TypeError(f"{type(self).__name__} must have at least 2 'contents'")
         for content in contents:
             if not isinstance(content, Content):
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} all 'contents' must be Content subclasses, not {}".format(
-                            type(self).__name__, repr(content)
-                        )
+                raise TypeError(
+                    "{} all 'contents' must be Content subclasses, not {}".format(
+                        type(self).__name__, repr(content)
                     )
                 )
             if content.is_union:
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{0} cannot contain union-types in its 'contents' ({1}); try {0}.simplified instead".format(
-                            type(self).__name__, type(content).__name__
-                        )
+                raise TypeError(
+                    "{0} cannot contain union-types in its 'contents' ({1}); try {0}.simplified instead".format(
+                        type(self).__name__, type(content).__name__
                     )
                 )
 
         if (
             not (tags.length is unknown_length or index.length is unknown_length)
             and tags.length > index.length
         ):
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "{} len(tags) ({}) must be <= len(index) ({})".format(
-                        type(self).__name__, tags.length, index.length
-                    )
+            raise ValueError(
+                "{} len(tags) ({}) must be <= len(index) ({})".format(
+                    type(self).__name__, tags.length, index.length
                 )
             )
 
         backend = None
         for content in contents:
             if backend is None:
                 backend = content.backend
             elif backend is not content.backend:
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} 'contents' must use the same array library (backend): {} vs {}".format(
-                            type(self).__name__,
-                            type(backend).__name__,
-                            type(content.backend).__name__,
-                        )
+                raise TypeError(
+                    "{} 'contents' must use the same array library (backend): {} vs {}".format(
+                        type(self).__name__,
+                        type(backend).__name__,
+                        type(content.backend).__name__,
                     )
                 )
 
         assert tags.nplike is backend.index_nplike
         assert index.nplike is backend.index_nplike
 
         self._tags = tags
@@ -231,28 +216,24 @@
         self_contents = contents
 
         backend = None
         for content in contents:
             if backend is None:
                 backend = content.backend
             elif backend is not content.backend:
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} 'contents' must use the same array library (backend): {} vs {}".format(
-                            cls.__name__,
-                            type(backend).__name__,
-                            type(content.backend).__name__,
-                        )
+                raise TypeError(
+                    "{} 'contents' must use the same array library (backend): {} vs {}".format(
+                        cls.__name__,
+                        type(backend).__name__,
+                        type(content.backend).__name__,
                     )
                 )
 
         if backend.nplike.known_data and self_index.length < self_tags.length:
-            raise ak._errors.wrap_error(
-                ValueError("invalid UnionArray: len(index) < len(tags)")
-            )
+            raise ValueError("invalid UnionArray: len(index) < len(tags)")
 
         length = self_tags.length
         tags = ak.index.Index8.empty(length, backend.index_nplike)
         index = ak.index.Index64.empty(length, backend.index_nplike)
         contents = []
 
         # For each outer union content
@@ -260,17 +241,15 @@
             # Is one of our new contents also a union?
             if isinstance(self_cont, UnionArray):
                 innertags = self_cont._tags
                 innerindex = self_cont._index
                 innercontents = self_cont._contents
 
                 # Update outermost parameters with this union's parameters
-                parameters = ak.forms.form._parameters_union(
-                    self_cont._parameters, parameters
-                )
+                parameters = parameters_union(self_cont._parameters, parameters)
 
                 # For each inner union content
                 for j, inner_cont in enumerate(innercontents):
                     unmerged = True
 
                     # For each "final" outer union content
                     for k in range(len(contents)):
@@ -396,25 +375,21 @@
                             length,
                             0,
                         )
                     )
                     contents.append(self_cont)
 
         if len(contents) > 2**7:
-            raise ak._errors.wrap_error(
-                NotImplementedError(
-                    "FIXME: handle UnionArray with more than 127 contents"
-                )
+            raise NotImplementedError(
+                "FIXME: handle UnionArray with more than 127 contents"
             )
 
         if len(contents) == 1:
             next = contents[0]._carry(index, True)
-            return next.copy(
-                parameters=ak.forms.form._parameters_union(next._parameters, parameters)
-            )
+            return next.copy(parameters=parameters_union(next._parameters, parameters))
 
         else:
             return cls(
                 tags,
                 index,
                 contents,
                 parameters=parameters,
@@ -629,15 +604,15 @@
                 else:
                     contents.append(ak.contents.UnmaskedArray.simplified(content))
 
         return UnionArray.simplified(
             ak.index.Index(nexttags),
             ak.index.Index(nextindex),
             contents,
-            parameters=ak.forms.form._parameters_union(self._parameters, parameters),
+            parameters=parameters_union(self._parameters, parameters),
         )
 
     def project(self, index):
         lentags = self._tags.length
         assert (
             self._index.length is unknown_length or lentags is unknown_length
         ) or self._index.length >= lentags
@@ -767,23 +742,14 @@
                     tag,
                     count.data,
                     f_offsets.length - 1,
                 )
             )
         return (tags, index)
 
-    def _nested_tags_index(self, offsets: Index, counts: Sequence[Index]):
-        return self.nested_tags_index(
-            offsets,
-            counts,
-            backend=self._backend,
-            tags_cls=type(self._tags),
-            index_cls=type(self._index),
-        )
-
     def _getitem_next_jagged_generic(self, slicestarts, slicestops, slicecontent, tail):
         if isinstance(self, ak.contents.UnionArray):
             raise ak._errors.index_error(
                 self,
                 ak.contents.ListArray(
                     slicestarts, slicestops, slicecontent, parameters=None
                 ),
@@ -833,21 +799,21 @@
         elif head is Ellipsis:
             return self._getitem_next_ellipsis(tail, advanced)
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             return self._getitem_next_missing(head, tail, advanced)
 
         else:
-            raise ak._errors.wrap_error(AssertionError(repr(head)))
+            raise AssertionError(repr(head))
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
 
         if posaxis is not None and posaxis + 1 == depth:
-            raise ak._errors.wrap_error(np.AxisError("axis=0 not allowed for flatten"))
+            raise np.AxisError("axis=0 not allowed for flatten")
 
         else:
             has_offsets = False
             offsetsraws = self._backend.index_nplike.empty(
                 len(self._contents), dtype=np.intp
             )
             contents = []
@@ -953,18 +919,16 @@
                 )
 
     def _mergeable_next(self, other, mergebool):
         return True
 
     def _merging_strategy(self, others):
         if len(others) == 0:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "to merge this array with 'others', at least one other must be provided"
-                )
+            raise ValueError(
+                "to merge this array with 'others', at least one other must be provided"
             )
 
         head = [self]
         tail = []
 
         for i in range(len(others)):
             head.append(others[i])
@@ -1048,17 +1012,15 @@
                 theirlength,
                 self.index.data,
                 mylength,
             )
         )
 
         if len(contents) > 2**7:
-            raise ak._errors.wrap_error(
-                AssertionError("FIXME: handle UnionArray with more than 127 contents")
-            )
+            raise AssertionError("FIXME: handle UnionArray with more than 127 contents")
 
         return ak.contents.UnionArray.simplified(
             tags, index, contents, parameters=self._parameters
         )
 
     def _mergemany(self, others):
         if len(others) == 0:
@@ -1081,17 +1043,15 @@
         length_so_far = 0
 
         parameters = self._parameters
         for array in head:
             if isinstance(array, ak.contents.EmptyArray):
                 continue
 
-            parameters = ak.forms.form._parameters_intersect(
-                parameters, array._parameters
-            )
+            parameters = parameters_intersect(parameters, array._parameters)
             if isinstance(array, ak.contents.UnionArray):
                 union_tags = ak.index.Index(array.tags)
                 union_index = ak.index.Index(array.index)
                 union_contents = array.contents
                 assert (
                     nexttags.nplike is self._backend.index_nplike
                     and union_tags.nplike is self._backend.index_nplike
@@ -1151,17 +1111,15 @@
                 )
 
                 length_so_far += array.length
 
                 nextcontents.append(array)
 
         if len(nextcontents) > 127:
-            raise ak._errors.wrap_error(
-                ValueError("FIXME: handle UnionArray with more than 127 contents")
-            )
+            raise ValueError("FIXME: handle UnionArray with more than 127 contents")
 
         next = ak.contents.UnionArray.simplified(
             nexttags,
             nextindex,
             nextcontents,
             parameters=parameters,
         )
@@ -1232,33 +1190,29 @@
             self._index,
             self._contents,
             parameters=self._parameters,
             merge=True,
             mergebool=True,
         )
         if isinstance(simplified, ak.contents.UnionArray):
-            raise ak._errors.wrap_error(
-                ValueError("cannot check if an irreducible UnionArray is unique")
-            )
+            raise ValueError("cannot check if an irreducible UnionArray is unique")
 
         return simplified._is_unique(negaxis, starts, parents, outlength)
 
     def _unique(self, negaxis, starts, parents, outlength):
         simplified = type(self).simplified(
             self._tags,
             self._index,
             self._contents,
             parameters=self._parameters,
             merge=True,
             mergebool=True,
         )
         if isinstance(simplified, ak.contents.UnionArray):
-            raise ak._errors.wrap_error(
-                ValueError("cannot make a unique irreducible UnionArray")
-            )
+            raise ValueError("cannot make a unique irreducible UnionArray")
 
         return simplified._unique(negaxis, starts, parents, outlength)
 
     def _argsort_next(
         self, negaxis, starts, shifts, parents, outlength, ascending, stable
     ):
         simplified = type(self).simplified(
@@ -1272,17 +1226,15 @@
             return ak.contents.NumpyArray(
                 self._backend.nplike.empty(0, dtype=np.int64),
                 parameters=None,
                 backend=self._backend,
             )
 
         if isinstance(simplified, ak.contents.UnionArray):
-            raise ak._errors.wrap_error(
-                ValueError("cannot argsort an irreducible UnionArray")
-            )
+            raise ValueError("cannot argsort an irreducible UnionArray")
 
         return simplified._argsort_next(
             negaxis, starts, shifts, parents, outlength, ascending, stable
         )
 
     def _sort_next(self, negaxis, starts, parents, outlength, ascending, stable):
         if self.length == 0:
@@ -1295,17 +1247,15 @@
             parameters=self._parameters,
             mergebool=True,
         )
         if simplified.length == 0:
             return simplified
 
         if isinstance(simplified, ak.contents.UnionArray):
-            raise ak._errors.wrap_error(
-                ValueError("cannot sort an irreducible UnionArray")
-            )
+            raise ValueError("cannot sort an irreducible UnionArray")
 
         return simplified._sort_next(
             negaxis, starts, parents, outlength, ascending, stable
         )
 
     def _reduce_next(
         self,
@@ -1317,17 +1267,15 @@
         outlength,
         mask,
         keepdims,
         behavior,
     ):
         # If we have a UnionArray, it must be irreducible, thanks to the
         # canonical checks in the constructor.
-        raise ak._errors.wrap_error(
-            ValueError(f"cannot call ak.{reducer.name} on an irreducible UnionArray")
-        )
+        raise ValueError(f"cannot call ak.{reducer.name} on an irreducible UnionArray")
 
     def _validity_error(self, path):
         if self._backend.nplike.known_data and self.index.length < self.tags.length:
             return f"at {path} ({type(self)!r}): len(index) < len(tags)"
 
         lencontents = self._backend.index_nplike.empty(
             len(self.contents), dtype=np.int64
@@ -1484,24 +1432,22 @@
             for i in range(len(self.contents))
         ]
 
         if any(isinstance(x, backend.nplike.ma.MaskedArray) for x in contents):
             try:
                 out = backend.nplike.ma.concatenate(contents)
             except Exception as err:
-                raise ak._errors.wrap_error(
-                    ValueError(f"cannot convert {self} into numpy.ma.MaskedArray")
+                raise ValueError(
+                    f"cannot convert {self} into numpy.ma.MaskedArray"
                 ) from err
         else:
             try:
                 out = backend.nplike.concat(contents)
             except Exception as err:
-                raise ak._errors.wrap_error(
-                    ValueError(f"cannot convert {self} into np.ndarray")
-                ) from err
+                raise ValueError(f"cannot convert {self} into np.ndarray") from err
 
         tags = backend.index_nplike.asarray(self.tags)
         for tag, content in enumerate(contents):
             mask = tags == tag
             if Jax.is_own_array(out):
                 out = out.at[mask].set(content)
             else:
@@ -1572,15 +1518,15 @@
         )
 
         if isinstance(result, Content):
             return result
         elif result is None:
             return continuation()
         else:
-            raise ak._errors.wrap_error(AssertionError(result))
+            raise AssertionError(result)
 
     def to_packed(self) -> Self:
         tags = self._tags.raw(self._backend.nplike)
         original_index = index = self._index.raw(self._backend.nplike)[: tags.shape[0]]
 
         contents = list(self._contents)
 
@@ -1603,17 +1549,15 @@
             ak.index.Index(index, nplike=self._backend.index_nplike),
             contents,
             parameters=self._parameters,
         )
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
-            raise ak._errors.wrap_error(
-                TypeError("cannot convert typetracer arrays to Python lists")
-            )
+            raise TypeError("cannot convert typetracer arrays to Python lists")
 
         out = self._to_list_custom(behavior, json_conversions)
         if out is not None:
             return out
 
         tags = self._tags.raw(numpy)
         index = self._index.raw(numpy)
```

### Comparing `awkward-2.1.1/src/awkward/contents/unmaskedarray.py` & `awkward-2.1.2/src/awkward/contents/unmaskedarray.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,26 @@
 import math
 
 import awkward as ak
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpy import Numpy
 from awkward._nplikes.numpylike import IndexType, NumpyMetadata
 from awkward._nplikes.typetracer import MaybeNone
+from awkward._parameters import (
+    parameters_intersect,
+    parameters_union,
+    type_parameters_equal,
+)
 from awkward._regularize import is_integer_like
 from awkward._slicing import NO_HEAD
+from awkward._typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 from awkward._util import unset
 from awkward.contents.content import Content
-from awkward.forms.form import _type_parameters_equal
 from awkward.forms.unmaskedform import UnmaskedForm
 from awkward.index import Index
-from awkward.typing import TYPE_CHECKING, Final, Self, SupportsIndex, final
 
 if TYPE_CHECKING:
     from awkward._slicing import SliceItem
 
 np = NumpyMetadata.instance()
 numpy = Numpy.instance()
 
@@ -59,27 +63,23 @@
                     return UnmaskedArray(self.content[where])
     """
 
     is_option = True
 
     def __init__(self, content, *, parameters=None):
         if not isinstance(content, Content):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'content' must be a Content subtype, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} 'content' must be a Content subtype, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
         if content.is_union or content.is_indexed or content.is_option:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{0} cannot contain a union-type, option-type, or indexed 'content' ({1}); try {0}.simplified instead".format(
-                        type(self).__name__, type(content).__name__
-                    )
+            raise TypeError(
+                "{0} cannot contain a union-type, option-type, or indexed 'content' ({1}); try {0}.simplified instead".format(
+                    type(self).__name__, type(content).__name__
                 )
             )
         self._content = content
         self._init(parameters, content.backend)
 
     @property
     def content(self):
@@ -103,23 +103,19 @@
         )
 
     @classmethod
     def simplified(cls, content, *, parameters=None):
         if content.is_union:
             return content.copy(
                 contents=[cls.simplified(x) for x in content.contents],
-                parameters=ak.forms.form._parameters_union(
-                    content._parameters, parameters
-                ),
+                parameters=parameters_union(content._parameters, parameters),
             )
         elif content.is_indexed or content.is_option:
             return content.copy(
-                parameters=ak.forms.form._parameters_union(
-                    content._parameters, parameters
-                )
+                parameters=parameters_union(content._parameters, parameters)
             )
         else:
             return cls(content, parameters=parameters)
 
     def _form_with_key(self, getkey):
         form_key = getkey(self)
         return self.form_cls(
@@ -285,28 +281,28 @@
         elif head is Ellipsis:
             return self._getitem_next_ellipsis(tail, advanced)
 
         elif isinstance(head, ak.contents.IndexedOptionArray):
             return self._getitem_next_missing(head, tail, advanced)
 
         else:
-            raise ak._errors.wrap_error(AssertionError(repr(head)))
+            raise AssertionError(repr(head))
 
     def project(self, mask=None):
         if mask is not None:
             return ak.contents.ByteMaskedArray(
                 mask, self._content, False, parameters=self._parameters
             ).project()
         else:
             return self._content
 
     def _offsets_and_flattened(self, axis, depth):
         posaxis = maybe_posaxis(self, axis, depth)
         if posaxis is not None and posaxis + 1 == depth:
-            raise ak._errors.wrap_error(np.AxisError("axis=0 not allowed for flatten"))
+            raise np.AxisError("axis=0 not allowed for flatten")
         else:
             offsets, flattened = self._content._offsets_and_flattened(axis, depth)
             if offsets.length == 0:
                 return (
                     offsets,
                     UnmaskedArray(flattened, parameters=self._parameters),
                 )
@@ -318,32 +314,30 @@
         # Is the other content is an identity, or a union?
         if other.is_identity_like or other.is_union:
             return True
         # We can only combine option types whose array-record parameters agree
         elif other.is_option or other.is_indexed:
             return self._mergeable_next(
                 other.content, mergebool
-            ) and _type_parameters_equal(self._parameters, other._parameters)
+            ) and type_parameters_equal(self._parameters, other._parameters)
         else:
             return self._content._mergeable_next(other, mergebool)
 
     def _reverse_merge(self, other):
         return self.to_IndexedOptionArray64()._reverse_merge(other)
 
     def _mergemany(self, others):
         if len(others) == 0:
             return self
 
         if all(isinstance(x, UnmaskedArray) for x in others):
             parameters = self._parameters
             tail_contents = []
             for x in others:
-                parameters = ak.forms.form._parameters_intersect(
-                    parameters, x._parameters
-                )
+                parameters = parameters_intersect(parameters, x._parameters)
                 tail_contents.append(x._content)
 
             return UnmaskedArray(
                 self._content._mergemany(tail_contents), parameters=parameters
             )
 
         else:
@@ -530,24 +524,22 @@
         )
 
         if isinstance(result, Content):
             return result
         elif result is None:
             return continuation()
         else:
-            raise ak._errors.wrap_error(AssertionError(result))
+            raise AssertionError(result)
 
     def to_packed(self) -> Self:
         return UnmaskedArray(self._content.to_packed(), parameters=self._parameters)
 
     def _to_list(self, behavior, json_conversions):
         if not self._backend.nplike.known_data:
-            raise ak._errors.wrap_error(
-                TypeError("cannot convert typetracer arrays to Python lists")
-            )
+            raise TypeError("cannot convert typetracer arrays to Python lists")
 
         out = self._to_list_custom(behavior, json_conversions)
         if out is not None:
             return out
 
         return self._content._to_list(behavior, json_conversions)
```

### Comparing `awkward-2.1.1/src/awkward/forms/__init__.py` & `awkward-2.1.2/src/awkward/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/forms/bitmaskedform.py` & `awkward-2.1.2/src/awkward/forms/bitmaskedform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
 from awkward._behavior import find_typestr
+from awkward._parameters import type_parameters_equal
+from awkward._typing import final
 from awkward._util import unset
-from awkward.forms.form import Form, _type_parameters_equal
-from awkward.typing import final
+from awkward.forms.form import Form
 
 
 @final
 class BitMaskedForm(Form):
     is_option = True
 
     def __init__(
@@ -17,43 +18,35 @@
         valid_when,
         lsb_order,
         *,
         parameters=None,
         form_key=None,
     ):
         if not isinstance(mask, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'mask' must be of type str, not {}".format(
-                        type(self).__name__, repr(mask)
-                    )
+            raise TypeError(
+                "{} 'mask' must be of type str, not {}".format(
+                    type(self).__name__, repr(mask)
                 )
             )
         if not isinstance(content, Form):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} all 'contents' must be Form subclasses, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} all 'contents' must be Form subclasses, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
         if not isinstance(valid_when, bool):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'valid_when' must be bool, not {}".format(
-                        type(self).__name__, repr(valid_when)
-                    )
+            raise TypeError(
+                "{} 'valid_when' must be bool, not {}".format(
+                    type(self).__name__, repr(valid_when)
                 )
             )
         if not isinstance(lsb_order, bool):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'lsb_order' must be bool, not {}".format(
-                        type(self).__name__, repr(lsb_order)
-                    )
+            raise TypeError(
+                "{} 'lsb_order' must be bool, not {}".format(
+                    type(self).__name__, repr(lsb_order)
                 )
             )
 
         self._mask = mask
         self._content = content
         self._valid_when = valid_when
         self._lsb_order = lsb_order
@@ -159,15 +152,15 @@
     def __eq__(self, other):
         if isinstance(other, BitMaskedForm):
             return (
                 self._form_key == other._form_key
                 and self._mask == other._mask
                 and self._valid_when == other._valid_when
                 and self._lsb_order == other._lsb_order
-                and _type_parameters_equal(self._parameters, other._parameters)
+                and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
     def purelist_parameter(self, key):
         if self._parameters is None or key not in self._parameters:
```

### Comparing `awkward-2.1.1/src/awkward/forms/bytemaskedform.py` & `awkward-2.1.2/src/awkward/forms/bytemaskedform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
 from awkward._behavior import find_typestr
+from awkward._parameters import type_parameters_equal
+from awkward._typing import final
 from awkward._util import unset
-from awkward.forms.form import Form, _type_parameters_equal
-from awkward.typing import final
+from awkward.forms.form import Form
 
 
 @final
 class ByteMaskedForm(Form):
     is_option = True
 
     def __init__(
@@ -16,35 +17,29 @@
         content,
         valid_when,
         *,
         parameters=None,
         form_key=None,
     ):
         if not isinstance(mask, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'mask' must be of type str, not {}".format(
-                        type(self).__name__, repr(mask)
-                    )
+            raise TypeError(
+                "{} 'mask' must be of type str, not {}".format(
+                    type(self).__name__, repr(mask)
                 )
             )
         if not isinstance(content, Form):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} all 'contents' must be Form subclasses, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} all 'contents' must be Form subclasses, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
         if not isinstance(valid_when, bool):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'valid_when' must be bool, not {}".format(
-                        type(self).__name__, repr(valid_when)
-                    )
+            raise TypeError(
+                "{} 'valid_when' must be bool, not {}".format(
+                    type(self).__name__, repr(valid_when)
                 )
             )
 
         self._mask = mask
         self._content = content
         self._valid_when = valid_when
         self._init(parameters=parameters, form_key=form_key)
@@ -134,15 +129,15 @@
 
     def __eq__(self, other):
         if isinstance(other, ByteMaskedForm):
             return (
                 self._form_key == other._form_key
                 and self._mask == other._mask
                 and self._valid_when == other._valid_when
-                and _type_parameters_equal(self._parameters, other._parameters)
+                and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
     def purelist_parameter(self, key):
         if self._parameters is None or key not in self._parameters:
```

### Comparing `awkward-2.1.1/src/awkward/forms/emptyform.py` & `awkward-2.1.2/src/awkward/forms/emptyform.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import awkward as ak
 from awkward._behavior import find_typestr
 from awkward._errors import deprecate
+from awkward._typing import final
 from awkward._util import unset
 from awkward.forms.form import Form, JSONMapping
-from awkward.typing import final
 
 
 @final
 class EmptyForm(Form):
     is_numpy = True
     is_unknown = True
```

### Comparing `awkward-2.1.1/src/awkward/forms/form.py` & `awkward-2.1.2/src/awkward/forms/form.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from __future__ import annotations
 
 import itertools
 import json
 import re
-from collections.abc import Collection, Mapping
+from collections.abc import Mapping
 
 import awkward as ak
-from awkward import _errors
 from awkward._behavior import find_typestrs
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._nplikes.shape import unknown_length
-from awkward.typing import Final, TypeAlias
+from awkward._typing import Final, JSONMapping, JSONSerializable
 
 np = NumpyMetadata.instance()
 numpy_backend = ak._backends.NumpyBackend.instance()
 
-JSONSerialisable: TypeAlias = (
-    "str | int | float | bool | None | list | tuple | JSONMapping"
-)
-JSONMapping: TypeAlias = "dict[str, JSONSerialisable]"
-
 
 reserved_nominal_parameters: Final = frozenset(
     {
         ("__array__", "string"),
         ("__array__", "bytestring"),
         ("__array__", "char"),
         ("__array__", "byte"),
@@ -83,17 +77,15 @@
             form_key=form_key,
         )
 
     elif input["class"] == "RecordArray":
         # New serialisation
         if "fields" in input:
             if isinstance(input["contents"], Mapping):
-                raise _errors.wrap_error(
-                    TypeError("new-style RecordForm contents must not be mappings")
-                )
+                raise TypeError("new-style RecordForm contents must not be mappings")
             contents = [from_dict(content) for content in input["contents"]]
             fields = input["fields"]
         # Old style record
         elif isinstance(input["contents"], dict):
             contents = []
             fields = []
             for key, content in input["contents"].items():
@@ -172,210 +164,26 @@
             index=input["index"],
             contents=[from_dict(content) for content in input["contents"]],
             parameters=parameters,
             form_key=form_key,
         )
 
     elif input["class"] == "VirtualArray":
-        raise _errors.wrap_error(
-            ValueError("Awkward 1.x VirtualArrays are not supported")
-        )
+        raise ValueError("Awkward 1.x VirtualArrays are not supported")
 
     else:
-        raise _errors.wrap_error(
-            ValueError(
-                "input class: {} was not recognised".format(repr(input["class"]))
-            )
+        raise ValueError(
+            "input class: {} was not recognised".format(repr(input["class"]))
         )
 
 
 def from_json(input: str) -> Form:
     return from_dict(json.loads(input))
 
 
-def _type_parameters_equal(
-    one: JSONMapping | None, two: JSONMapping | None, *, allow_missing: bool = False
-) -> bool:
-    if one is None and two is None:
-        return True
-
-    elif one is None:
-        # NB: __categorical__ is currently a type-only parameter, but
-        # we check it here as types check this too.
-        for key in ("__array__", "__record__", "__categorical__"):
-            if two.get(key) is not None:
-                return allow_missing
-        return True
-
-    elif two is None:
-        for key in ("__array__", "__record__", "__categorical__"):
-            if one.get(key) is not None:
-                return allow_missing
-        return True
-
-    else:
-        for key in ("__array__", "__record__", "__categorical__"):
-            if one.get(key) != two.get(key):
-                return False
-        return True
-
-
-def _parameters_equal(
-    one: JSONMapping, two: JSONMapping, only_array_record=False
-) -> bool:
-    if one is None and two is None:
-        return True
-    elif one is None:
-        if only_array_record:
-            # NB: __categorical__ is currently a type-only parameter, but
-            # we check it here as types check this too.
-            for key in ("__array__", "__record__", "__categorical__"):
-                if two.get(key) is not None:
-                    return False
-            return True
-        else:
-            for value in two.values():
-                if value is not None:
-                    return False
-            return True
-
-    elif two is None:
-        if only_array_record:
-            for key in ("__array__", "__record__", "__categorical__"):
-                if one.get(key) is not None:
-                    return False
-            return True
-        else:
-            for value in one.values():
-                if value is not None:
-                    return False
-            return True
-
-    else:
-        if only_array_record:
-            keys = ("__array__", "__record__", "__categorical__")
-        else:
-            keys = set(one.keys()).union(two.keys())
-        for key in keys:
-            if one.get(key) != two.get(key):
-                return False
-        return True
-
-
-def _parameters_intersect(
-    left: JSONMapping | None,
-    right: JSONMapping | None,
-    *,
-    exclude: Collection[tuple[str, JSONSerialisable]] = (),
-) -> JSONMapping | None:
-    """
-    Args:
-        left: first parameters mapping
-        right: second parameters mapping
-        exclude: collection of (key, value) items to exclude
-
-    Returns the intersected key-value pairs of `left` and `right` as a dictionary.
-    """
-    if left is None or right is None:
-        return None
-
-    common_keys = iter(left.keys() & right.keys())
-    has_no_exclusions = len(exclude) == 0
-
-    # Avoid creating `result` unless we have to
-    for key in common_keys:
-        left_value = left[key]
-        # Do our keys match?
-        if (
-            left_value is not None
-            and left_value == right[key]
-            and (has_no_exclusions or (key, left_value) not in exclude)
-        ):
-            # Exit, indicating that we want to create `result`
-            break
-    else:
-        return None
-
-    # We found a meaningful key, so create a result dict
-    result = {key: left_value}
-    for key in common_keys:
-        left_value = left[key]
-        if (
-            left_value is not None
-            and left_value == right[key]
-            and (has_no_exclusions or (key, left_value) not in exclude)
-        ):
-            result[key] = left_value
-
-    return result
-
-
-def _parameters_union(
-    left: JSONMapping | None,
-    right: JSONMapping | None,
-    *,
-    exclude: Collection[tuple[str, JSONSerialisable]] = (),
-) -> JSONMapping | None:
-    """
-    Args:
-        left: first parameters mapping
-        right: second parameters mapping
-        exclude: collection of (key, value) items to exclude
-
-    Returns the merged key-value pairs of `left` and `right` as a dictionary.
-
-    """
-    has_no_exclusions = len(exclude) == 0
-    if left is None:
-        if right is None:
-            return None
-        else:
-            return {
-                k: v
-                for k, v in right.items()
-                if v is not None and (has_no_exclusions or (k, v) not in exclude)
-            }
-    else:
-        result = {
-            k: v
-            for k, v in left.items()
-            if v is not None and (has_no_exclusions or (k, v) not in exclude)
-        }
-        if right is None:
-            return result
-        else:
-            for key in right:
-                right_value = right[key]
-                if right_value is not None and (
-                    has_no_exclusions or (key, right_value) not in exclude
-                ):
-                    result[key] = right_value
-
-            return result
-
-
-def _parameters_is_empty(parameters: JSONMapping | None) -> bool:
-    """
-    Args:
-        parameters (dict or None): parameters dictionary, or None
-
-    Return True if the parameters dictionary is considered empty, either because it is
-    None, or because it does not have any meaningful (non-None) values; otherwise,
-    return False.
-    """
-    if parameters is None:
-        return True
-
-    for item in parameters.values():
-        if item is not None:
-            return False
-
-    return True
-
-
 def _expand_braces(text, seen=None):
     if seen is None:
         seen = set()
 
     spans = [m.span() for m in re.finditer(r"\{[^\{\}]*\}", text)][::-1]
     alts = [text[start + 1 : stop - 1].split(",") for start, stop in spans]
 
@@ -400,27 +208,23 @@
     is_option = False
     is_indexed = False
     is_record = False
     is_union = False
 
     def _init(self, *, parameters, form_key):
         if parameters is not None and not isinstance(parameters, dict):
-            raise _errors.wrap_error(
-                TypeError(
-                    "{} 'parameters' must be of type dict or None, not {}".format(
-                        type(self).__name__, repr(parameters)
-                    )
+            raise TypeError(
+                "{} 'parameters' must be of type dict or None, not {}".format(
+                    type(self).__name__, repr(parameters)
                 )
             )
         if form_key is not None and not isinstance(form_key, str):
-            raise _errors.wrap_error(
-                TypeError(
-                    "{} 'form_key' must be of type string or None, not {}".format(
-                        type(self).__name__, repr(form_key)
-                    )
+            raise TypeError(
+                "{} 'form_key' must be of type string or None, not {}".format(
+                    type(self).__name__, repr(form_key)
                 )
             )
 
         self._parameters = parameters
         self._form_key = form_key
 
     @property
@@ -428,57 +232,57 @@
         if self._parameters is None:
             self._parameters = {}
         return self._parameters
 
     @property
     def is_identity_like(self):
         """Return True if the content or its non-list descendents are an identity"""
-        raise _errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
-    def parameter(self, key: str) -> JSONSerialisable:
+    def parameter(self, key: str) -> JSONSerializable:
         if self._parameters is None:
             return None
         else:
             return self._parameters.get(key)
 
-    def purelist_parameter(self, key: str) -> JSONSerialisable:
-        raise _errors.wrap_error(NotImplementedError)
+    def purelist_parameter(self, key: str) -> JSONSerializable:
+        raise NotImplementedError
 
     @property
     def purelist_isregular(self):
-        raise _errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @property
     def purelist_depth(self):
-        raise _errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @property
     def minmax_depth(self):
-        raise _errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @property
     def branch_depth(self):
-        raise _errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @property
     def fields(self):
-        raise _errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @property
     def is_tuple(self):
-        raise _errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     @property
     def form_key(self):
         return self._form_key
 
     @form_key.setter
     def form_key(self, value):
         if value is not None and not isinstance(value, str):
-            raise ak._errors.wrap_error(TypeError("form_key must be None or a string"))
+            raise TypeError("form_key must be None or a string")
         self._form_key = value
 
     def __str__(self):
         return json.dumps(self.to_dict(verbose=False), indent=4)
 
     def to_dict(self, verbose=True):
         return self._to_dict_part(verbose, toplevel=True)
@@ -515,16 +319,16 @@
 
     def select_columns(self, specifier, expand_braces=True):
         if isinstance(specifier, str):
             specifier = [specifier]
 
         for item in specifier:
             if not isinstance(item, str):
-                raise _errors.wrap_error(
-                    TypeError("a column-selection specifier must be a list of strings")
+                raise TypeError(
+                    "a column-selection specifier must be a list of strings"
                 )
 
         if expand_braces:
             next_specifier = []
             for item in specifier:
                 for result in _expand_braces(item):
                     next_specifier.append(result)
@@ -536,27 +340,27 @@
         output = []
         return self._select_columns(0, specifier, matches, output)
 
     def column_types(self):
         return self._column_types()
 
     def _columns(self, path, output, list_indicator):
-        raise _errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _select_columns(self, index, specifier, matches, output):
-        raise _errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _column_types(self):
-        raise _errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _to_dict_part(self, verbose, toplevel):
-        raise _errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def _type(self, typestrs):
-        raise _errors.wrap_error(NotImplementedError)
+        raise NotImplementedError
 
     def length_zero_array(
         self, *, backend=numpy_backend, highlevel=True, behavior=None
     ):
         return ak.operations.ak_from_buffers._impl(
             form=self,
             length=0,
```

### Comparing `awkward-2.1.1/src/awkward/forms/indexedform.py` & `awkward-2.1.2/src/awkward/forms/indexedform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import awkward as ak
+from awkward._parameters import parameters_union, type_parameters_equal
+from awkward._typing import final
 from awkward._util import unset
-from awkward.forms.form import Form, _parameters_union, _type_parameters_equal
-from awkward.typing import final
+from awkward.forms.form import Form
 
 
 @final
 class IndexedForm(Form):
     is_indexed = True
 
     def __init__(
@@ -15,27 +16,23 @@
         index,
         content=None,
         *,
         parameters=None,
         form_key=None,
     ):
         if not isinstance(index, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'index' must be of type str, not {}".format(
-                        type(self).__name__, repr(index)
-                    )
+            raise TypeError(
+                "{} 'index' must be of type str, not {}".format(
+                    type(self).__name__, repr(index)
                 )
             )
         if not isinstance(content, Form):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} all 'contents' must be Form subclasses, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} all 'contents' must be Form subclasses, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
 
         self._index = index
         self._content = content
         self._init(parameters=parameters, form_key=form_key)
 
@@ -71,35 +68,29 @@
         parameters=None,
         form_key=None,
     ):
         is_cat = parameters is not None and parameters.get("__array__") == "categorical"
 
         if content.is_union and not is_cat:
             return content.copy(
-                parameters=ak.forms.form._parameters_union(
-                    content._parameters, parameters
-                )
+                parameters=parameters_union(content._parameters, parameters)
             )
 
         elif content.is_option:
             return ak.forms.IndexedOptionForm.simplified(
                 "i64",
                 content.content,
-                parameters=ak.forms.form._parameters_union(
-                    content._parameters, parameters
-                ),
+                parameters=parameters_union(content._parameters, parameters),
             )
 
         elif content.is_indexed:
             return IndexedForm(
                 "i64",
                 content.content,
-                parameters=ak.forms.form._parameters_union(
-                    content._parameters, parameters
-                ),
+                parameters=parameters_union(content._parameters, parameters),
             )
 
         else:
             return cls(index, content, parameters=parameters, form_key=form_key)
 
     def __repr__(self):
         args = [repr(self._index), repr(self._content), *self._repr_args()]
@@ -118,15 +109,15 @@
     def _type(self, typestrs):
         out = self._content._type(typestrs)
 
         if self._parameters is not None:
             if out._parameters is None:
                 out._parameters = self._parameters
             else:
-                out._parameters = _parameters_union(out._parameters, self._parameters)
+                out._parameters = parameters_union(out._parameters, self._parameters)
 
             if self._parameters.get("__array__") == "categorical":
                 if out._parameters is self._parameters:
                     out._parameters = dict(out._parameters)
 
                 # Restore content __array__
                 out_array = self._content.parameter("__array__")
@@ -139,15 +130,15 @@
         return out
 
     def __eq__(self, other):
         if isinstance(other, IndexedForm):
             return (
                 self._form_key == other._form_key
                 and self._index == other._index
-                and _type_parameters_equal(self._parameters, other._parameters)
+                and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
     def purelist_parameter(self, key):
         if self._parameters is None or key not in self._parameters:
```

### Comparing `awkward-2.1.1/src/awkward/forms/indexedoptionform.py` & `awkward-2.1.2/src/awkward/forms/indexedoptionform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
 from awkward._behavior import find_typestr
+from awkward._parameters import parameters_union, type_parameters_equal
+from awkward._typing import final
 from awkward._util import unset
-from awkward.forms.form import Form, _type_parameters_equal
-from awkward.typing import final
+from awkward.forms.form import Form
 
 
 @final
 class IndexedOptionForm(Form):
     is_option = True
     is_indexed = True
 
@@ -16,27 +17,23 @@
         index,
         content,
         *,
         parameters=None,
         form_key=None,
     ):
         if not isinstance(index, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'index' must be of type str, not {}".format(
-                        type(self).__name__, repr(index)
-                    )
+            raise TypeError(
+                "{} 'index' must be of type str, not {}".format(
+                    type(self).__name__, repr(index)
                 )
             )
         if not isinstance(content, Form):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} all 'contents' must be Form subclasses, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} all 'contents' must be Form subclasses, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
 
         self._index = index
         self._content = content
         self._init(parameters=parameters, form_key=form_key)
 
@@ -77,17 +74,15 @@
         if content.is_union and not is_cat:
             return content._union_of_optionarrays(index, parameters)
 
         elif content.is_indexed or content.is_option:
             return ak.forms.IndexedOptionForm.simplified(
                 "i64",
                 content.content,
-                parameters=ak.forms.form._parameters_union(
-                    content._parameters, parameters
-                ),
+                parameters=parameters_union(content._parameters, parameters),
             )
 
         else:
             return cls(index, content, parameters=parameters, form_key=form_key)
 
     def __repr__(self):
         args = [repr(self._index), repr(self._content), *self._repr_args()]
@@ -118,15 +113,15 @@
         ).simplify_option_union()
 
     def __eq__(self, other):
         if isinstance(other, IndexedOptionForm):
             return (
                 self._form_key == other._form_key
                 and self._index == other._index
-                and _type_parameters_equal(self._parameters, other._parameters)
+                and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
     def purelist_parameter(self, key):
         if self._parameters is None or key not in self._parameters:
```

### Comparing `awkward-2.1.1/src/awkward/forms/listform.py` & `awkward-2.1.2/src/awkward/forms/listform.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
 from awkward._behavior import find_typestr
+from awkward._parameters import type_parameters_equal
+from awkward._typing import final
 from awkward._util import unset
-from awkward.forms.form import Form, _type_parameters_equal
-from awkward.typing import final
+from awkward.forms.form import Form
 
 
 @final
 class ListForm(Form):
     is_list = True
 
     def __init__(
@@ -16,35 +17,29 @@
         stops,
         content,
         *,
         parameters=None,
         form_key=None,
     ):
         if not isinstance(starts, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'starts' must be of type str, not {}".format(
-                        type(self).__name__, repr(starts)
-                    )
+            raise TypeError(
+                "{} 'starts' must be of type str, not {}".format(
+                    type(self).__name__, repr(starts)
                 )
             )
         if not isinstance(stops, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'starts' must be of type str, not {}".format(
-                        type(self).__name__, repr(starts)
-                    )
+            raise TypeError(
+                "{} 'starts' must be of type str, not {}".format(
+                    type(self).__name__, repr(starts)
                 )
             )
         if not isinstance(content, Form):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} all 'contents' must be Form subclasses, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} all 'contents' must be Form subclasses, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
 
         self._starts = starts
         self._stops = stops
         self._content = content
         self._init(parameters=parameters, form_key=form_key)
@@ -119,15 +114,15 @@
 
     def __eq__(self, other):
         if isinstance(other, ListForm):
             return (
                 self._form_key == other._form_key
                 and self._starts == other._starts
                 and self._stops == other._stops
-                and _type_parameters_equal(self._parameters, other._parameters)
+                and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
     def purelist_parameter(self, key):
         if self._parameters is None or key not in self._parameters:
```

### Comparing `awkward-2.1.1/src/awkward/forms/listoffsetform.py` & `awkward-2.1.2/src/awkward/forms/listoffsetform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
 from awkward._behavior import find_typestr
+from awkward._parameters import type_parameters_equal
+from awkward._typing import final
 from awkward._util import unset
-from awkward.forms.form import Form, _type_parameters_equal
-from awkward.typing import final
+from awkward.forms.form import Form
 
 
 @final
 class ListOffsetForm(Form):
     is_list = True
 
     def __init__(self, offsets, content, *, parameters=None, form_key=None):
         if not isinstance(offsets, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'offsets' must be of type str, not {}".format(
-                        type(self).__name__, repr(offsets)
-                    )
+            raise TypeError(
+                "{} 'offsets' must be of type str, not {}".format(
+                    type(self).__name__, repr(offsets)
                 )
             )
 
         self._offsets = offsets
         self._content = content
         self._init(parameters=parameters, form_key=form_key)
 
@@ -73,15 +72,15 @@
         )
 
     def __eq__(self, other):
         if isinstance(other, ListOffsetForm):
             return (
                 self._form_key == other._form_key
                 and self._offsets == other._offsets
-                and _type_parameters_equal(self._parameters, other._parameters)
+                and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
     def purelist_parameter(self, key):
         if self._parameters is None or key not in self._parameters:
```

### Comparing `awkward-2.1.1/src/awkward/forms/numpyform.py` & `awkward-2.1.2/src/awkward/forms/numpyform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from collections.abc import Iterable
 
 import awkward as ak
 from awkward._behavior import find_typestr
 from awkward._nplikes.numpylike import NumpyMetadata
+from awkward._parameters import type_parameters_equal
+from awkward._typing import final
 from awkward._util import unset
-from awkward.forms.form import Form, _type_parameters_equal
-from awkward.typing import final
+from awkward.forms.form import Form
 
 np = NumpyMetadata.instance()
 
 
 def from_dtype(dtype, parameters=None):
     if dtype.subdtype is None:
         inner_shape = ()
@@ -48,19 +49,17 @@
         parameters=None,
         form_key=None,
     ):
         primitive = ak.types.numpytype.dtype_to_primitive(
             ak.types.numpytype.primitive_to_dtype(primitive)
         )
         if not isinstance(inner_shape, Iterable):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'inner_shape' must be iterable, not {}".format(
-                        type(self).__name__, repr(inner_shape)
-                    )
+            raise TypeError(
+                "{} 'inner_shape' must be iterable, not {}".format(
+                    type(self).__name__, repr(inner_shape)
                 )
             )
 
         self._primitive = primitive
         self._inner_shape = tuple(inner_shape)
         self._init(parameters=parameters, form_key=form_key)
 
@@ -143,15 +142,15 @@
 
     def __eq__(self, other):
         if isinstance(other, NumpyForm):
             return (
                 self._form_key == other._form_key
                 and self._primitive == other._primitive
                 and self._inner_shape == other._inner_shape
-                and _type_parameters_equal(self._parameters, other._parameters)
+                and type_parameters_equal(self._parameters, other._parameters)
             )
         else:
             return False
 
     def to_RegularForm(self):
         out = NumpyForm(self._primitive, (), parameters=None, form_key=None)
         for x in self._inner_shape[::-1]:
```

### Comparing `awkward-2.1.1/src/awkward/forms/recordform.py` & `awkward-2.1.2/src/awkward/forms/recordform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import glob
 from collections.abc import Iterable
 
 import awkward as ak
 from awkward._behavior import find_typestr
+from awkward._parameters import type_parameters_equal
 from awkward._regularize import is_integer
+from awkward._typing import final
 from awkward._util import unset
-from awkward.forms.form import Form, _type_parameters_equal
-from awkward.typing import final
+from awkward.forms.form import Form
 
 
 @final
 class RecordForm(Form):
     is_record = True
 
     def __init__(
@@ -19,36 +20,30 @@
         contents,
         fields,
         *,
         parameters=None,
         form_key=None,
     ):
         if not isinstance(contents, Iterable):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'contents' must be iterable, not {}".format(
-                        type(self).__name__, repr(contents)
-                    )
+            raise TypeError(
+                "{} 'contents' must be iterable, not {}".format(
+                    type(self).__name__, repr(contents)
                 )
             )
         for content in contents:
             if not isinstance(content, Form):
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} all 'contents' must be Form subclasses, not {}".format(
-                            type(self).__name__, repr(content)
-                        )
+                raise TypeError(
+                    "{} all 'contents' must be Form subclasses, not {}".format(
+                        type(self).__name__, repr(content)
                     )
                 )
         if fields is not None and not isinstance(fields, Iterable):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'fields' must be iterable, not {}".format(
-                        type(self).__name__, repr(contents)
-                    )
+            raise TypeError(
+                "{} 'fields' must be iterable, not {}".format(
+                    type(self).__name__, repr(contents)
                 )
             )
 
         self._fields = fields
         self._contents = list(contents)
         self._init(parameters=parameters, form_key=form_key)
 
@@ -100,19 +95,17 @@
     def index_to_field(self, index):
         if 0 <= index < len(self._contents):
             if self._fields is None:
                 return str(index)
             else:
                 return self._fields[index]
         else:
-            raise ak._errors.wrap_error(
-                IndexError(
-                    "no index {} in record with {} fields".format(
-                        index, len(self._contents)
-                    )
+            raise IndexError(
+                "no index {} in record with {} fields".format(
+                    index, len(self._contents)
                 )
             )
 
     def field_to_index(self, field):
         if self._fields is None:
             try:
                 i = int(field)
@@ -124,19 +117,17 @@
         else:
             try:
                 i = self._fields.index(field)
             except ValueError:
                 pass
             else:
                 return i
-        raise ak._errors.wrap_error(
-            ak._errors.FieldNotFoundError(
-                "no field {} in record with {} fields".format(
-                    repr(field), len(self._contents)
-                )
+        raise ak._errors.FieldNotFoundError(
+            "no field {} in record with {} fields".format(
+                repr(field), len(self._contents)
             )
         )
 
     def has_field(self, field):
         if self._fields is None:
             try:
                 i = int(field)
@@ -149,19 +140,17 @@
 
     def content(self, index_or_field):
         if is_integer(index_or_field):
             index = index_or_field
         elif isinstance(index_or_field, str):
             index = self.field_to_index(index_or_field)
         else:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "index_or_field must be an integer (index) or string (field), not {}".format(
-                        repr(index_or_field)
-                    )
+            raise TypeError(
+                "index_or_field must be an integer (index) or string (field), not {}".format(
+                    repr(index_or_field)
                 )
             )
         return self._contents[index]
 
     def _to_dict_part(self, verbose, toplevel):
         out = {"class": "RecordArray"}
 
@@ -186,15 +175,15 @@
 
     def __eq__(self, other):
         if isinstance(other, RecordForm):
             if (
                 self._form_key == other._form_key
                 and self.is_tuple == other.is_tuple
                 and len(self._contents) == len(other._contents)
-                and _type_parameters_equal(self._parameters, other._parameters)
+                and type_parameters_equal(self._parameters, other._parameters)
             ):
                 if self.is_tuple:
                     return self._contents == other._contents
                 else:
                     return dict(zip(self._fields, self._contents)) == dict(
                         zip(other._fields, other._contents)
                     )
```

### Comparing `awkward-2.1.1/src/awkward/forms/regularform.py` & `awkward-2.1.2/src/awkward/forms/regularform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
 from awkward._behavior import find_typestr
 from awkward._nplikes.shape import unknown_length
+from awkward._parameters import type_parameters_equal
 from awkward._regularize import is_integer
+from awkward._typing import final
 from awkward._util import unset
-from awkward.forms.form import Form, _type_parameters_equal
-from awkward.typing import final
+from awkward.forms.form import Form
 
 
 @final
 class RegularForm(Form):
     is_list = True
     is_regular = True
 
     def __init__(self, content, size, *, parameters=None, form_key=None):
         if not isinstance(content, Form):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} all 'contents' must be Form subclasses, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} all 'contents' must be Form subclasses, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
         if not (size is unknown_length or (is_integer(size) and size >= 0)):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'size' must be a non-negative int or None, not {}".format(
-                        type(self).__name__, repr(size)
-                    )
+            raise TypeError(
+                "{} 'size' must be a non-negative int or None, not {}".format(
+                    type(self).__name__, repr(size)
                 )
             )
 
         self._content = content
         self._size = size
         self._init(parameters=parameters, form_key=form_key)
 
@@ -78,15 +75,15 @@
         )
 
     def __eq__(self, other):
         if isinstance(other, RegularForm):
             return (
                 self._form_key == other._form_key
                 and self._size == other._size
-                and _type_parameters_equal(self._parameters, other._parameters)
+                and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
     def purelist_parameter(self, key):
         if self._parameters is None or key not in self._parameters:
```

### Comparing `awkward-2.1.1/src/awkward/forms/unionform.py` & `awkward-2.1.2/src/awkward/forms/unionform.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 from collections import Counter
 from collections.abc import Iterable
 
 import awkward as ak
 from awkward._behavior import find_typestr
+from awkward._parameters import type_parameters_equal
+from awkward._typing import final
 from awkward._util import unset
-from awkward.forms.form import Form, _type_parameters_equal
-from awkward.typing import final
+from awkward.forms.form import Form
 
 
 @final
 class UnionForm(Form):
     is_union = True
 
     def __init__(
@@ -19,44 +20,36 @@
         index,
         contents,
         *,
         parameters=None,
         form_key=None,
     ):
         if not isinstance(tags, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'tags' must be of type str, not {}".format(
-                        type(self).__name__, repr(tags)
-                    )
+            raise TypeError(
+                "{} 'tags' must be of type str, not {}".format(
+                    type(self).__name__, repr(tags)
                 )
             )
         if not isinstance(index, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'index' must be of type str, not {}".format(
-                        type(self).__name__, repr(index)
-                    )
+            raise TypeError(
+                "{} 'index' must be of type str, not {}".format(
+                    type(self).__name__, repr(index)
                 )
             )
         if not isinstance(contents, Iterable):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'contents' must be iterable, not {}".format(
-                        type(self).__name__, repr(contents)
-                    )
+            raise TypeError(
+                "{} 'contents' must be iterable, not {}".format(
+                    type(self).__name__, repr(contents)
                 )
             )
         for content in contents:
             if not isinstance(content, Form):
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} all 'contents' must be Form subclasses, not {}".format(
-                            type(self).__name__, repr(content)
-                        )
+                raise TypeError(
+                    "{} all 'contents' must be Form subclasses, not {}".format(
+                        type(self).__name__, repr(content)
                     )
                 )
 
         self._tags = tags
         self._index = index
         self._contents = list(contents)
         self._init(parameters=parameters, form_key=form_key)
@@ -150,15 +143,15 @@
     def __eq__(self, other):
         if (
             isinstance(other, UnionForm)
             and self._form_key == other._form_key
             and self._tags == other._tags
             and self._index == other._index
             and len(self._contents) == len(other._contents)
-            and _type_parameters_equal(self._parameters, other._parameters)
+            and type_parameters_equal(self._parameters, other._parameters)
         ):
             return self._contents == other._contents
 
         return False
 
     def purelist_parameter(self, key):
         if self._parameters is None or key not in self._parameters:
```

### Comparing `awkward-2.1.1/src/awkward/forms/unmaskedform.py` & `awkward-2.1.2/src/awkward/forms/unmaskedform.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 import awkward as ak
 from awkward._behavior import find_typestr
+from awkward._parameters import parameters_union, type_parameters_equal
+from awkward._typing import final
 from awkward._util import unset
-from awkward.forms.form import Form, _type_parameters_equal
-from awkward.typing import final
+from awkward.forms.form import Form
 
 
 @final
 class UnmaskedForm(Form):
     is_option = True
 
     def __init__(
         self,
         content,
         *,
         parameters=None,
         form_key=None,
     ):
         if not isinstance(content, Form):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} all 'contents' must be Form subclasses, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} all 'contents' must be Form subclasses, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
 
         self._content = content
         self._init(parameters=parameters, form_key=form_key)
 
     @property
@@ -53,23 +52,19 @@
         *,
         parameters=None,
         form_key=None,
     ):
         if content.is_union:
             return content.copy(
                 contents=[cls.simplified(x) for x in content.contents],
-                parameters=ak.forms.form._parameters_union(
-                    content._parameters, parameters
-                ),
+                parameters=parameters_union(content._parameters, parameters),
             )
         elif content.is_indexed or content.is_option:
             return content.copy(
-                parameters=ak.forms.form._parameters_union(
-                    content._parameters, parameters
-                )
+                parameters=parameters_union(content._parameters, parameters)
             )
         else:
             return cls(content, parameters=parameters, form_key=form_key)
 
     def __repr__(self):
         args = [repr(self._content), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
@@ -90,15 +85,15 @@
             typestr=find_typestr(self._parameters, typestrs),
         ).simplify_option_union()
 
     def __eq__(self, other):
         if isinstance(other, UnmaskedForm):
             return (
                 self._form_key == other._form_key
-                and _type_parameters_equal(self._parameters, other._parameters)
+                and type_parameters_equal(self._parameters, other._parameters)
                 and self._content == other._content
             )
         else:
             return False
 
     def purelist_parameter(self, key):
         if self._parameters is None or key not in self._parameters:
```

### Comparing `awkward-2.1.1/src/awkward/operations/__init__.py` & `awkward-2.1.2/src/awkward/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_all.py` & `awkward-2.1.2/src/awkward/operations/ak_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
 
 def _impl(array, axis, keepdims, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_almost_equal.py` & `awkward-2.1.2/src/awkward/operations/ak_almost_equal.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 from __future__ import annotations
 
 __all__ = ("almost_equal",)
 
 
 from awkward._backends import backend_of
 from awkward._behavior import behavior_of, get_array_class, get_record_class
-from awkward._errors import wrap_error
 from awkward._nplikes.numpylike import NumpyMetadata
-from awkward.forms.form import _parameters_equal
+from awkward._parameters import parameters_are_equal
 from awkward.operations.ak_to_layout import to_layout
 
 np = NumpyMetadata.instance()
 
 
 def almost_equal(
     left,
@@ -50,18 +49,16 @@
     right_behavior = behavior_of(right)
 
     left = to_layout(left, allow_record=False).to_packed()
     right = to_layout(right, allow_record=False).to_packed()
 
     backend = backend_of(left, right)
     if not backend.nplike.known_data:
-        raise wrap_error(
-            NotImplementedError(
-                "Awkward Arrays with typetracer backends cannot yet be compared with `ak.almost_equal`."
-            )
+        raise NotImplementedError(
+            "Awkward Arrays with typetracer backends cannot yet be compared with `ak.almost_equal`."
         )
 
     def is_approx_dtype(left, right) -> bool:
         if not dtype_exact:
             for family in np.integer, np.floating:
                 if np.issubdtype(left, family):
                     return np.issubdtype(right, family)
@@ -82,15 +79,15 @@
                 right = right.to_ListOffsetArray64()
             else:
                 return False
 
         if left.length != right.length:
             return False
 
-        if check_parameters and not _parameters_equal(
+        if check_parameters and not parameters_are_equal(
             left.parameters, right.parameters
         ):
             return False
 
         # Require that the arrays have the same evaluated types
         if not (
             get_array_class(left, left_behavior)
@@ -138,10 +135,10 @@
                 and (left.is_tuple == right.is_tuple)
                 and all(visitor(x, y) for x, y in zip(left.contents, right.contents))
             )
         elif left.is_unknown:
             return True
 
         else:
-            raise wrap_error(AssertionError)
+            raise AssertionError
 
     return visitor(left, right)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_any.py` & `awkward-2.1.2/src/awkward/operations/ak_any.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
 
 def _impl(array, axis, keepdims, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_argcartesian.py` & `awkward-2.1.2/src/awkward/operations/ak_argcartesian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_argcombinations.py` & `awkward-2.1.2/src/awkward/operations/ak_argcombinations.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,17 +89,15 @@
         parameters = {}
     else:
         parameters = dict(parameters)
     if with_name is not None:
         parameters["__record__"] = with_name
 
     if axis < 0:
-        raise ak._errors.wrap_error(
-            ValueError("the 'axis' for argcombinations must be non-negative")
-        )
+        raise ValueError("the 'axis' for argcombinations must be non-negative")
     else:
         layout = ak._do.local_index(
             ak.operations.to_layout(array, allow_record=False, allow_other=False),
             axis,
         )
         out = ak._do.combinations(
             layout,
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_argmax.py` & `awkward-2.1.2/src/awkward/operations/ak_argmax.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
 
 def nanargmax(
     array,
@@ -138,15 +138,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         array = ak.operations.ak_nan_to_none._impl(array, False, None)
 
         return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_argmin.py` & `awkward-2.1.2/src/awkward/operations/ak_argmin.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
 
 def nanargmin(
     array,
@@ -137,15 +137,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         array = ak.operations.ak_nan_to_none._impl(array, False, None)
 
         return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_argsort.py` & `awkward-2.1.2/src/awkward/operations/ak_argsort.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,13 +73,11 @@
     if kind is None:
         stable = False
     elif kind in ("stable", "mergesort"):
         stable = True
     elif kind in ("heapsort", "quicksort"):
         stable = False
     else:
-        raise ak._errors.wrap_error(
-            ValueError(
-                f"unsupported value for 'kind' passed to overloaded NumPy function 'argsort': {kind!r}"
-            )
+        raise ValueError(
+            f"unsupported value for 'kind' passed to overloaded NumPy function 'argsort': {kind!r}"
         )
     return argsort(a, axis=axis, stable=stable)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_backend.py` & `awkward-2.1.2/src/awkward/operations/ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_broadcast_arrays.py` & `awkward-2.1.2/src/awkward/operations/ak_broadcast_arrays.py`

 * *Files 0% similar despite different names*

```diff
@@ -212,18 +212,15 @@
     for x in arrays:
         y = ak.operations.to_layout(x, allow_record=True, allow_other=True)
         if not isinstance(y, (ak.contents.Content, ak.Record)):
             y = ak.contents.NumpyArray(backend.nplike.asarray([y]))
         inputs.append(y.to_backend(backend))
 
     def action(inputs, depth, **kwargs):
-        if depth == depth_limit or (
-            depth_limit is None
-            and all(isinstance(x, ak.contents.NumpyArray) for x in inputs)
-        ):
+        if depth == depth_limit or all(x.is_numpy for x in inputs):
             return tuple(inputs)
         else:
             return None
 
     behavior = behavior_of(*arrays, behavior=behavior)
     out = ak._broadcasting.broadcast_and_apply(
         inputs,
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_broadcast_fields.py` & `awkward-2.1.2/src/awkward/operations/ak_broadcast_fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,33 +76,31 @@
             def next_pull(content):
                 return pullback(layout.copy(content=content))
 
             return descend_to_record_or_identity(layout.content, next_pull)
         elif layout.is_leaf:
             return pullback, layout
         elif layout.is_union:
-            raise ak._errors.wrap_error(TypeError("unions are not supported"))
+            raise TypeError("unions are not supported")
         else:
-            raise ak._errors.wrap_error(AssertionError("unexpected content type"))
+            raise AssertionError("unexpected content type")
 
     # Like broadcast_and_apply, we want to walk into each layout, correct the structure, and then rebuilt the arrays
     # We do this using "pull back" functions that accept a child content, and return the top-level layout. Unlike
     # layout.copy, the pull-back functions can be arbitrarily deep: the closures maintain the structure of the array
     def recurse(inputs):
         # Descend to records, identities, or leaves
         pullbacks, next_inputs = zip(
             *[descend_to_record_or_identity(x) for x in inputs]
         )
         # We can only work with all non-record, or all record/identity
         if any(c.is_record for c in next_inputs):
             if not all(c.is_record or c.is_identity_like for c in next_inputs):
-                raise ak._errors.wrap_error(
-                    AssertionError(
-                        "if any inputs are records, all inputs must be records or identities"
-                    )
+                raise AssertionError(
+                    "if any inputs are records, all inputs must be records or identities"
                 )
         # With no records, we can exit here
         else:
             return [pull(layout) for pull, layout in zip(pullbacks, next_inputs)]
 
         # Broadcast the fields of only the records
         records = [r for r in next_inputs if r.is_record]
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_cartesian.py` & `awkward-2.1.2/src/awkward/operations/ak_cartesian.py`

 * *Files 14% similar despite different names*

```diff
@@ -173,18 +173,15 @@
          [(3, 2.2, 'a'), (3, 2.2, 'b')],
          [(3, 3.3, 'a'), (3, 3.3, 'b')],
          [(4, 1.1, 'a'), (4, 1.1, 'b')],
          [(4, 2.2, 'a'), (4, 2.2, 'b')],
          [(4, 3.3, 'a'), (4, 3.3, 'b')]]
 
     The order of the output is fixed: it is always lexicographical in the
-    order that the `arrays` are written. (Before Python 3.6, the order of
-    keys in a dict were not guaranteed, so the dict interface is not
-    recommended for these versions of Python.) Thus, it is not possible to
-    group by `three` in the example above.
+    order that the `arrays` are written.
 
     To emulate an SQL or Pandas "group by" operation, put the keys that you
     wish to group by *first* and use `nested=[0]` or `nested=[n]` to group by
     unique n-tuples. If necessary, record keys can later be reordered with a
     list of strings in #ak.Array.__getitem__.
 
     To get list index positions in the tuples/records, rather than data from
@@ -208,223 +205,217 @@
 
 
 def _impl(arrays, axis, nested, parameters, with_name, highlevel, behavior):
     axis = regularize_axis(axis)
     if isinstance(arrays, dict):
         backend = ak._backends.backend_of(*arrays.values(), default=cpu)
         behavior = behavior_of(*arrays.values(), behavior=behavior)
-        new_arrays = {}
-        for n, x in arrays.items():
-            new_arrays[n] = ak.operations.to_layout(
-                x, allow_record=False, allow_other=False
+        array_layouts = {
+            name: ak.operations.to_layout(
+                layout, allow_record=False, allow_other=False
             ).to_backend(backend)
+            for name, layout in arrays.items()
+        }
 
     else:
         arrays = list(arrays)
         backend = ak._backends.backend_of(*arrays, default=cpu)
         behavior = behavior_of(*arrays, behavior=behavior)
-        new_arrays = []
-        for x in arrays:
-            new_arrays.append(
-                ak.operations.to_layout(
-                    x, allow_record=False, allow_other=False
-                ).to_backend(backend)
-            )
+        array_layouts = [
+            ak.operations.to_layout(
+                layout, allow_record=False, allow_other=False
+            ).to_backend(backend)
+            for layout in arrays
+        ]
 
     if with_name is not None:
         if parameters is None:
             parameters = {}
         else:
             parameters = dict(parameters)
         parameters["__record__"] = with_name
 
-    if isinstance(new_arrays, dict):
-        new_arrays_values = list(new_arrays.values())
+    if isinstance(array_layouts, dict):
+        layouts = list(array_layouts.values())
     else:
-        new_arrays_values = new_arrays
+        layouts = array_layouts
 
-    posaxis = maybe_posaxis(new_arrays_values[0], axis, 1)
+    posaxis = maybe_posaxis(layouts[0], axis, 1)
+
+    # Validate `posaxis`
     if posaxis is None or posaxis < 0:
-        raise ak._errors.wrap_error(ValueError("negative axis depth is ambiguous"))
-    for x in new_arrays_values[1:]:
-        if maybe_posaxis(x, axis, 1) != posaxis:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "arrays to cartesian-product do not have the same depth for negative axis"
-                )
+        raise ValueError("negative axis depth is ambiguous")
+    for layout in layouts[1:]:
+        if maybe_posaxis(layout, axis, 1) != posaxis:
+            raise ValueError(
+                "arrays to cartesian-product do not have the same depth for negative axis"
             )
 
-    if posaxis == 0:
-        if nested is None or nested is False:
-            nested = []
-
-        if isinstance(new_arrays, dict):
-            if nested is True:
-                nested = list(new_arrays.keys())  # last key is ignored below
-            if any(not (isinstance(n, str) and n in new_arrays) for x in nested):
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "the 'nested' parameter of cartesian must be dict keys "
-                        "for a dict of arrays"
-                    )
+    # Validate `nested`
+    if nested is None or nested is False:
+        nested = []
+    elif nested is True:
+        if isinstance(array_layouts, dict):
+            nested = list(array_layouts.keys())[:-1]
+        else:
+            nested = list(range(len(array_layouts))[:-1])
+    else:
+        if isinstance(array_layouts, dict):
+            if any(not (isinstance(x, str) and x in array_layouts) for x in nested):
+                raise ValueError(
+                    "the 'nested' parameter of cartesian must be dict keys "
+                    "for a dict of arrays"
+                )
+            if len(nested) >= len(array_layouts):
+                raise ValueError(
+                    "the `nested` parameter of cartesian must contain "
+                    "fewer items than there are arrays"
                 )
+        else:
+            if any(
+                not (isinstance(x, int) and 0 <= x < len(array_layouts) - 1)
+                for x in nested
+            ):
+                raise ValueError(
+                    "the 'nested' parameter of cartesian must be integers in "
+                    "[0, len(arrays) - 1) for an iterable of arrays"
+                )
+
+    if posaxis == 0:
+        if isinstance(array_layouts, dict):
             fields = []
-            layouts = []
             tonested = []
-            for i, (n, x) in enumerate(new_arrays.items()):
-                fields.append(n)
-                layouts.append(x)
-                if n in nested:
+            for i, (name, _) in enumerate(array_layouts.items()):
+                fields.append(name)
+                if name in nested:
                     tonested.append(i)
             nested = tonested
 
         else:
-            if nested is True:
-                nested = list(range(len(new_arrays) - 1))
-            if any(
-                not (isinstance(x, int) and 0 <= x < len(new_arrays) - 1)
-                for x in nested
-            ):
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "the 'nested' prarmeter of cartesian must be integers in "
-                        "[0, len(arrays) - 1) for an iterable of arrays"
-                    )
-                )
             fields = None
-            layouts = []
-            for x in new_arrays:
-                layouts.append(x)
-
-        layouts = list(layouts)
 
         indexes = [
             ak.index.Index64(backend.index_nplike.reshape(x, (-1,)))
             for x in backend.index_nplike.meshgrid(
-                *[backend.index_nplike.arange(len(x), dtype=np.int64) for x in layouts],
+                *[
+                    backend.index_nplike.arange(x.length, dtype=np.int64)
+                    for x in layouts
+                ],
                 indexing="ij",
             )
         ]
         outs = [
-            ak.contents.IndexedArray.simplified(x, y)
-            for x, y in __builtins__["zip"](indexes, layouts)
+            ak.contents.IndexedArray.simplified(x, y) for x, y in zip(indexes, layouts)
         ]
 
         result = ak.contents.RecordArray(outs, fields, parameters=parameters)
-        for i in range(len(new_arrays) - 1, -1, -1):
+        for i in range(len(array_layouts))[::-1]:
             if i in nested:
-                result = ak.contents.RegularArray(result, len(layouts[i + 1]), 0)
+                result = ak.contents.RegularArray(result, layouts[i + 1].length, 0)
 
     else:
 
-        def newaxis(layout, i):
-            if i == 0:
+        def add_outer_dimensions(
+            layout: ak.contents.Content, n: int
+        ) -> ak.contents.Content:
+            if n == 0:
                 return layout
             else:
-                return ak.contents.RegularArray(newaxis(layout, i - 1), 1, 0)
+                return ak.contents.RegularArray(
+                    add_outer_dimensions(layout, n - 1), 1, 0
+                )
 
-        def getgetfunction1(i, **kwargs):
-            def getfunction1(layout, depth, **kwargs):
-                if depth == 2:
-                    return newaxis(layout, i)
-                else:
-                    return None
-
-            return getfunction1
-
-        def getgetfunction2(i, **kwargs):
-            def getfunction2(layout, depth, **kwargs):
-                if depth == posaxis:
-                    inside = len(new_arrays) - i - 1
-                    outside = i
-                    if (
-                        layout.parameter("__array__") == "string"
-                        or layout.parameter("__array__") == "bytestring"
-                    ):
-                        raise ak._errors.wrap_error(
-                            ValueError(
-                                "ak.cartesian does not compute combinations of the "
-                                "characters of a string; please split it into lists"
-                            )
-                        )
-                    nextlayout = ak._do.recursively_apply(
-                        layout, getgetfunction1(inside), behavior
-                    )
-                    return newaxis(nextlayout, outside)
-                else:
-                    return None
-
-            return getfunction2
-
-        def apply(x, i):
-            layout = ak.operations.to_layout(x, allow_record=False, allow_other=False)
-            return ak._do.recursively_apply(layout, getgetfunction2(i), behavior)
-
-        toflatten = []
-        if nested is None or nested is False:
-            nested = []
-
-        if isinstance(new_arrays, dict):
-            if nested is True:
-                nested = list(new_arrays.keys())  # last key is ignored below
-            if any(not (isinstance(n, str) and n in new_arrays) for x in nested):
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "the 'nested' parameter of cartesian must be dict keys "
-                        "for a dict of arrays"
+        def apply_pad_inner_list(layout, depth, lateral_context, **kwargs):
+            """
+            Add new dimensions (given by lateral_context["n"]) above innermost list
+            """
+            n = lateral_context["n"]
+            # We want to be above at least one dimension (list)
+            if depth == 2:
+                return add_outer_dimensions(layout, n)
+            else:
+                return None
+
+        def apply_pad_inner_list_at_axis(layout, depth, lateral_context, **kwargs):
+            """
+            Each array in arrays contributes to one of these new dimensions.
+            To make the cartesian product of the given arrays broadcastable,
+            each array is padded by (n, m) new length-1 regular dimensions
+            (above, below) the target depth. The values of (n, m) are given by
+            the position of the array; the first array is the outermost axis.
+            """
+            i = lateral_context["i"]
+            if depth == posaxis:
+                n_inside = len(array_layouts) - i - 1
+                n_outside = i
+                if (
+                    layout.parameter("__array__") == "string"
+                    or layout.parameter("__array__") == "bytestring"
+                ):
+                    raise ValueError(
+                        "ak.cartesian does not compute combinations of the "
+                        "characters of a string; please split it into lists"
                     )
+                nextlayout = ak._do.recursively_apply(
+                    layout,
+                    apply_pad_inner_list,
+                    behavior,
+                    lateral_context={"n": n_inside},
                 )
-            fields = []
-            layouts = []
-            for i, (n, x) in enumerate(new_arrays.items()):
-                fields.append(n)
-                layouts.append(apply(x, i))
-                if i < len(new_arrays) - 1 and n not in nested:
-                    toflatten.append(posaxis + i + 1)
+                return add_outer_dimensions(nextlayout, n_outside)
+            else:
+                return None
 
-        else:
-            if nested is True:
-                nested = list(range(len(new_arrays) - 1))
-            if any(
-                not (isinstance(x, int) and 0 <= x < len(new_arrays) - 1)
-                for x in nested
-            ):
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "the 'nested' parameter of cartesian must be integers in "
-                        "[0, len(arrays) - 1) for an iterable of arrays"
-                    )
+        # New _interior_ axes are added to the result layout, but
+        # unless explicitly named, these axes should be flattened.
+        axes_to_flatten = [
+            posaxis + i + 1
+            for i, _ in enumerate(array_layouts)
+            if i < len(array_layouts) - 1 and i not in nested
+        ]
+        # This list *must* be sorted in reverse order
+        axes_to_flatten.reverse()
+
+        if isinstance(array_layouts, dict):
+            fields = list(array_layouts.keys())
+            new_layouts = [
+                ak._do.recursively_apply(
+                    layout,
+                    apply_pad_inner_list_at_axis,
+                    behavior,
+                    lateral_context={"i": i},
                 )
+                for i, (_, layout) in enumerate(array_layouts.items())
+            ]
+
+        else:
             fields = None
-            layouts = []
-            for i, x in enumerate(new_arrays):
-                layouts.append(apply(x, i))
-                if i < len(new_arrays) - 1 and i not in nested:
-                    toflatten.append(posaxis + i + 1)
-
-        def getfunction3(inputs, depth, **kwargs):
-            if depth == posaxis + len(new_arrays):
-                if all(len(x) == 0 for x in inputs):
-                    inputs = [
-                        x.content
-                        if isinstance(x, ak.contents.RegularArray) and x.size == 1
-                        else x
-                        for x in inputs
-                    ]
+            new_layouts = [
+                ak._do.recursively_apply(
+                    layout,
+                    apply_pad_inner_list_at_axis,
+                    behavior,
+                    lateral_context={"i": i},
+                )
+                for i, layout in enumerate(array_layouts)
+            ]
+
+        def apply_build_record(inputs, depth, **kwargs):
+            if depth == posaxis + len(array_layouts):
                 return (ak.contents.RecordArray(inputs, fields, parameters=parameters),)
 
             else:
                 return None
 
         out = ak._broadcasting.broadcast_and_apply(
-            layouts, getfunction3, behavior, right_broadcast=False
+            new_layouts, apply_build_record, behavior, right_broadcast=False
         )
         assert isinstance(out, tuple) and len(out) == 1
         result = out[0]
 
-        while len(toflatten) != 0:
-            flatten_axis = toflatten.pop()
+        # Remove surplus dimensions, iterating from smallest to greatest
+        for axis_to_flatten in axes_to_flatten:
             result = ak.operations.flatten(
-                result, axis=flatten_axis, highlevel=False, behavior=behavior
+                result, axis=axis_to_flatten, highlevel=False, behavior=behavior
             )
 
     return wrap_layout(result, behavior, highlevel)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_categories.py` & `awkward-2.1.2/src/awkward/operations/ak_categories.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_combinations.py` & `awkward-2.1.2/src/awkward/operations/ak_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_concatenate.py` & `awkward-2.1.2/src/awkward/operations/ak_concatenate.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 __all__ = ("concatenate",)
 import awkward as ak
 from awkward._backends import NumpyBackend, backend_of
 from awkward._behavior import behavior_of
 from awkward._layout import maybe_posaxis, wrap_layout
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import is_integer, regularize_axis
+from awkward._typing import Sequence
+from awkward.contents import Content
 from awkward.operations.ak_fill_none import fill_none
 
 np = NumpyMetadata.instance()
 cpu = NumpyBackend.instance()
 
 
 @ak._connect.numpy.implements("concatenate")
@@ -73,39 +75,33 @@
             )
             for x in arrays
         )
     ]
 
     contents = [x for x in content_or_others if isinstance(x, ak.contents.Content)]
     if len(contents) == 0:
-        raise ak._errors.wrap_error(
-            ValueError("need at least one array to concatenate")
-        )
+        raise ValueError("need at least one array to concatenate")
 
     posaxis = maybe_posaxis(contents[0], axis, 1)
     maxdepth = max(
         x.minmax_depth[1]
         for x in content_or_others
         if isinstance(x, ak.contents.Content)
     )
     if posaxis is None or not 0 <= posaxis < maxdepth:
-        raise ak._errors.wrap_error(
-            ValueError(
-                "axis={} is beyond the depth of this array or the depth of this array "
-                "is ambiguous".format(axis)
-            )
+        raise ValueError(
+            "axis={} is beyond the depth of this array or the depth of this array "
+            "is ambiguous".format(axis)
         )
     for x in content_or_others:
         if isinstance(x, ak.contents.Content):
             if maybe_posaxis(x, axis, 1) != posaxis:
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "arrays to concatenate do not have the same depth for negative "
-                        "axis={}".format(axis)
-                    )
+                raise ValueError(
+                    "arrays to concatenate do not have the same depth for negative "
+                    "axis={}".format(axis)
                 )
 
     if posaxis == 0:
         content_or_others = [
             x if isinstance(x, ak.contents.Content) else ak.operations.to_layout([x])
             for x in content_or_others
         ]
@@ -115,15 +111,15 @@
             if ak._do.mergeable(batch[-1], x, mergebool=mergebool):
                 batch.append(x)
             else:
                 batches.append([x])
 
         contents = [ak._do.mergemany(b) for b in batches]
         if len(contents) > 1:
-            out = ak._do.merge_as_union(contents)
+            out = _merge_as_union(contents)
         else:
             out = contents[0]
 
         if isinstance(out, ak.contents.UnionArray):
             out = type(out).simplified(
                 out._tags,
                 out._index,
@@ -151,19 +147,17 @@
 
                 length = None
                 for x in inputs:
                     if isinstance(x, ak.contents.Content):
                         if not is_integer(length):
                             length = x.length
                         elif length != x.length and is_integer(x.length):
-                            raise ak._errors.wrap_error(
-                                ValueError(
-                                    "all arrays must have the same length for "
-                                    "axis={}".format(axis)
-                                )
+                            raise ValueError(
+                                "all arrays must have the same length for "
+                                "axis={}".format(axis)
                             )
 
             if depth == posaxis and all(
                 isinstance(x, ak.contents.Content)
                 and x.is_regular
                 or (isinstance(x, ak.contents.NumpyArray) and x.data.ndim > 1)
                 or not isinstance(x, ak.contents.Content)
@@ -269,26 +263,51 @@
                 return (ak.contents.ListOffsetArray(offsets, inner),)
 
             elif any(
                 x.minmax_depth == (1, 1)
                 for x in inputs
                 if isinstance(x, ak.contents.Content)
             ):
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "at least one array is not deep enough to concatenate at "
-                        "axis={}".format(axis)
-                    )
+                raise ValueError(
+                    "at least one array is not deep enough to concatenate at "
+                    "axis={}".format(axis)
                 )
 
             else:
                 return None
 
         out = ak._broadcasting.broadcast_and_apply(
             content_or_others,
             action,
             behavior=behavior,
             allow_records=True,
             right_broadcast=False,
         )[0]
 
     return wrap_layout(out, behavior, highlevel)
+
+
+def _merge_as_union(
+    contents: Sequence[Content], parameters=None
+) -> ak.contents.UnionArray:
+    length = sum([c.length for c in contents])
+    first = contents[0]
+    tags = ak.index.Index8.empty(length, first.backend.index_nplike)
+    index = ak.index.Index64.empty(length, first.backend.index_nplike)
+
+    offset = 0
+    for i, content in enumerate(contents):
+        content._handle_error(
+            content.backend["awkward_UnionArray_filltags_const", tags.dtype.type](
+                tags.data, offset, content.length, i
+            )
+        )
+        content._handle_error(
+            content.backend["awkward_UnionArray_fillindex_count", index.dtype.type](
+                index.data, offset, content.length
+            )
+        )
+        offset += content.length
+
+    return ak.contents.UnionArray.simplified(
+        tags, index, contents, parameters=parameters
+    )
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_copy.py` & `awkward-2.1.2/src/awkward/operations/ak_copy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_corr.py` & `awkward-2.1.2/src/awkward/operations/ak_corr.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(x, y, weight, axis, keepdims, mask_identity)
 
 
 def _impl(x, y, weight, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_count.py` & `awkward-2.1.2/src/awkward/operations/ak_count.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
 
 def _impl(array, axis, keepdims, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_count_nonzero.py` & `awkward-2.1.2/src/awkward/operations/ak_count_nonzero.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
 
 def _impl(array, axis, keepdims, mask_identity, highlevel, behavior):
     axis = regularize_axis(axis)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_covar.py` & `awkward-2.1.2/src/awkward/operations/ak_covar.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(x, y, weight, axis, keepdims, mask_identity)
 
 
 def _impl(x, y, weight, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_drop_none.py` & `awkward-2.1.2/src/awkward/operations/ak_drop_none.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,18 +65,16 @@
 
         def action(layout, continuation, **kwargs):
             return drop_nones(continuation())
 
     else:
         max_axis = layout.branch_depth[1] - 1
         if axis > max_axis:
-            raise ak._errors.wrap_error(
-                np.AxisError(
-                    f"axis={axis} exceeds the depth ({max_axis}) of this array"
-                )
+            raise np.AxisError(
+                f"axis={axis} exceeds the depth ({max_axis}) of this array"
             )
 
         def recompute_offsets(layout, depth, **kwargs):
             posaxis = maybe_posaxis(layout, axis, depth)
             if (
                 posaxis == 0
                 and posaxis == depth - 1
@@ -87,18 +85,16 @@
                 out = layout._rebuild_without_nones(none_indexes, layout.content)
                 return out
 
         def action(layout, depth, **kwargs):
             if layout.is_record:
                 posaxises = {maybe_posaxis(x, axis, depth) for x in layout.contents}
                 if len(posaxises) > 1 and any(x < depth for x in posaxises):
-                    raise ak._errors.wrap_error(
-                        np.AxisError(
-                            f"axis={axis} implies different levels in records that might require part of a record to be dropped, which is impossible"
-                        )
+                    raise np.AxisError(
+                        f"axis={axis} implies different levels in records that might require part of a record to be dropped, which is impossible"
                     )
             posaxis = maybe_posaxis(layout, axis, depth)
             if posaxis == 0:
                 if not layout.is_option:
                     return layout
                 else:
                     return layout.drop_none()
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_fields.py` & `awkward-2.1.2/src/awkward/operations/ak_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_fill_none.py` & `awkward-2.1.2/src/awkward/operations/ak_fill_none.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,15 +130,13 @@
                     return ak._do.fill_none(layout, valuelayout)
                 elif layout.is_union or layout.is_record or layout.is_indexed:
                     return None
                 else:
                     return layout
 
             elif layout.is_leaf:
-                raise ak._errors.wrap_error(
-                    np.AxisError(
-                        f"axis={axis} exceeds the depth of this array ({depth})"
-                    )
+                raise np.AxisError(
+                    f"axis={axis} exceeds the depth of this array ({depth})"
                 )
 
     out = ak._do.recursively_apply(arraylayout, action, behavior)
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_firsts.py` & `awkward-2.1.2/src/awkward/operations/ak_firsts.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,17 +49,15 @@
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array)
     behavior = behavior_of(array, behavior=behavior)
 
     if not is_integer(axis):
-        raise ak._errors.wrap_error(
-            TypeError(f"'axis' must be an integer, not {axis!r}")
-        )
+        raise TypeError(f"'axis' must be an integer, not {axis!r}")
 
     if maybe_posaxis(layout, axis, 1) == 0:
         # specialized logic; it's tested in test_0582-propagate-context-in-broadcast_and_apply.py
         # Build an integer-typed slice array, so that we can
         # ensure we have advanced indexing for both length==0
         # and length > 0 cases.
         slicer = ak.from_iter([None, 0])
@@ -88,16 +86,14 @@
                 index[empties] = -1
 
                 return ak.contents.IndexedOptionArray.simplified(
                     ak.index.Index64(index), layout._content
                 )
 
             elif layout.is_leaf:
-                raise ak._errors.wrap_error(
-                    np.AxisError(
-                        f"axis={axis} exceeds the depth of this array ({depth})"
-                    )
+                raise np.AxisError(
+                    f"axis={axis} exceeds the depth of this array ({depth})"
                 )
 
         out = ak._do.recursively_apply(layout, action, behavior, numpy_to_regular=True)
 
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_flatten.py` & `awkward-2.1.2/src/awkward/operations/ak_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_from_arrow.py` & `awkward-2.1.2/src/awkward/operations/ak_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_from_arrow_schema.py` & `awkward-2.1.2/src/awkward/operations/ak_from_arrow_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_from_avro_file.py` & `awkward-2.1.2/src/awkward/operations/ak_from_avro_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("from_avro_file",)
 
-# from awkward.typing import Type
+# from awkward._typing import Type
 import pathlib
 
 import awkward as ak
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
@@ -48,18 +48,16 @@
                 form, length, container = awkward._connect.avro.ReadAvroFT(
                     opened_file, limit_entries, debug_forth
                 ).outcontents
                 return _impl(form, length, container, highlevel, behavior)
 
         else:
             if not hasattr(file, "read") or not hasattr(file, "seek"):
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "'file' must either be a filename string or be a file-like object with 'read' and 'seek' methods"
-                    )
+                raise TypeError(
+                    "'file' must either be a filename string or be a file-like object with 'read' and 'seek' methods"
                 )
             else:
                 form, length, container = awkward._connect.avro.ReadAvroFT(
                     file, limit_entries, debug_forth
                 ).outarr
                 return _impl(form, length, container, highlevel, behavior)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_from_buffers.py` & `awkward-2.1.2/src/awkward/operations/ak_from_buffers.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,40 +116,34 @@
             form = ak.forms.NumpyForm(form)
         else:
             form = ak.forms.from_json(form)
     elif isinstance(form, dict):
         form = ak.forms.from_dict(form)
 
     if not (is_integer(length) and length >= 0):
-        raise ak._errors.wrap_error(
-            TypeError("'length' argument must be a non-negative integer")
-        )
+        raise TypeError("'length' argument must be a non-negative integer")
 
     if not isinstance(form, ak.forms.Form):
-        raise ak._errors.wrap_error(
-            TypeError(
-                "'form' argument must be a Form or its Python dict/JSON string representation"
-            )
+        raise TypeError(
+            "'form' argument must be a Form or its Python dict/JSON string representation"
         )
 
     if isinstance(buffer_key, str):
 
         def getkey(form, attribute):
             return buffer_key.format(form_key=form.form_key, attribute=attribute)
 
     elif callable(buffer_key):
 
         def getkey(form, attribute):
             return buffer_key(form_key=form.form_key, attribute=attribute, form=form)
 
     else:
-        raise ak._errors.wrap_error(
-            TypeError(
-                f"buffer_key must be a string or a callable, not {type(buffer_key)}"
-            )
+        raise TypeError(
+            f"buffer_key must be a string or a callable, not {type(buffer_key)}"
         )
 
     out = reconstitute(form, length, container, getkey, backend, byteorder, simplify)
     return wrap_layout(out, behavior, highlevel)
 
 
 _index_to_dtype = {
@@ -163,35 +157,31 @@
 
 def _from_buffer(nplike, buffer, dtype, count, byteorder):
     if nplike.is_own_array(buffer):
         array = nplike.reshape(buffer.view(dtype), shape=(-1,), copy=False)
 
         # Require 1D
         if array.size < count:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    f"size of array ({array.size}) is less than size of form ({count})"
-                )
+            raise TypeError(
+                f"size of array ({array.size}) is less than size of form ({count})"
             )
 
         return array[:count]
     else:
         array = nplike.frombuffer(buffer, dtype=dtype, count=count)
         if byteorder != ak._util.native_byteorder:
             return array.byteswap(inplace=False)
         else:
             return array
 
 
 def reconstitute(form, length, container, getkey, backend, byteorder, simplify):
     if isinstance(form, ak.forms.EmptyForm):
         if length != 0:
-            raise ak._errors.wrap_error(
-                ValueError(f"EmptyForm node, but the expected length is {length}")
-            )
+            raise ValueError(f"EmptyForm node, but the expected length is {length}")
         return ak.contents.EmptyArray()
 
     elif isinstance(form, ak.forms.NumpyForm):
         dtype = ak.types.numpytype.primitive_to_dtype(form.primitive)
         raw_array = container[getkey(form, "data")]
         real_length = length
         for x in form.inner_shape:
@@ -435,10 +425,8 @@
             ak.index.Index(tags),
             ak.index.Index(index),
             contents,
             parameters=form.parameters,
         )
 
     else:
-        raise ak._errors.wrap_error(
-            AssertionError("unexpected form node type: " + str(type(form)))
-        )
+        raise AssertionError("unexpected form node type: " + str(type(form)))
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_from_categorical.py` & `awkward-2.1.2/src/awkward/operations/ak_from_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_from_cupy.py` & `awkward-2.1.2/src/awkward/operations/ak_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_from_iter.py` & `awkward-2.1.2/src/awkward/operations/ak_from_iter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 __all__ = ("from_iter",)
 
+from collections.abc import Iterable
+
 from awkward_cpp.lib import _ext
 
 import awkward as ak
 from awkward._nplikes.numpylike import NumpyMetadata
 
 np = NumpyMetadata.instance()
 
@@ -68,31 +70,35 @@
             "resize": resize,
         },
     ):
         return _impl(iterable, highlevel, behavior, allow_record, initial, resize)
 
 
 def _impl(iterable, highlevel, behavior, allow_record, initial, resize):
+    if not isinstance(iterable, Iterable):
+        raise TypeError(
+            f"cannot produce an array from a non-iterable object ({type(iterable)!r})"
+        )
+
     if isinstance(iterable, dict):
         if allow_record:
             return _impl(
                 [iterable],
                 highlevel,
                 behavior,
                 False,
                 initial,
                 resize,
             )[0]
         else:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "cannot produce an array from a single dict (that would be a record)"
-                )
+            raise ValueError(
+                "cannot produce an array from a single dict (that would be a record)"
             )
 
+    # Ensure that tuples are treated as iterables, not records
     if isinstance(iterable, tuple):
         iterable = list(iterable)
 
     builder = _ext.ArrayBuilder(initial=initial, resize=resize)
     builder.fromiter(iterable)
 
     formstr, length, buffers = builder.to_buffers()
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_from_jax.py` & `awkward-2.1.2/src/awkward/operations/ak_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_from_json.py` & `awkward-2.1.2/src/awkward/operations/ak_from_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -445,26 +445,22 @@
                     ):
                         with numpy._module.errstate(invalid="ignore"):
                             return ak.contents.NumpyArray(
                                 node.backend.nplike.asarray(real)
                                 + node.backend.nplike.asarray(imag) * 1j
                             )
                     else:
-                        raise ak._errors.wrap_error(
-                            ValueError(
-                                f"expected record with fields {complex_record_fields[0]!r} and {complex_record_fields[1]!r} to have integer or floating point types, not {str(real.form.type)!r} and {str(imag.form.type)!r}"
-                            )
+                        raise ValueError(
+                            f"expected record with fields {complex_record_fields[0]!r} and {complex_record_fields[1]!r} to have integer or floating point types, not {str(real.form.type)!r} and {str(imag.form.type)!r}"
                         )
 
         return ak._do.recursively_apply(layout, action)
 
     else:
-        raise ak._errors.wrap_error(
-            TypeError("complex_record_fields must be None or a pair of strings")
-        )
+        raise TypeError("complex_record_fields must be None or a pair of strings")
 
 
 def _no_schema(
     source,
     line_delimited,
     nan_string,
     posinf_string,
@@ -488,15 +484,15 @@
                 read_one,
                 buffersize,
                 nan_string,
                 posinf_string,
                 neginf_string,
             )
         except Exception as err:
-            raise ak._errors.wrap_error(ValueError(str(err))) from None
+            raise ValueError(str(err)) from None
 
     formstr, length, buffers = builder.to_buffers()
     form = ak.forms.from_json(formstr)
     layout = ak.operations.from_buffers(
         form, length, buffers, byteorder=ak._util.native_byteorder, highlevel=False
     )
 
@@ -525,40 +521,34 @@
     highlevel,
     behavior,
 ):
     if isinstance(schema, (bytes, str)):
         schema = json.loads(schema)
 
     if not isinstance(schema, dict):
-        raise ak._errors.wrap_error(
-            TypeError(f"unrecognized JSONSchema: expected dict, got {schema!r}")
-        )
+        raise TypeError(f"unrecognized JSONSchema: expected dict, got {schema!r}")
 
     container = {}
     instructions = []
 
     if schema.get("type") == "array":
         if "items" not in schema:
-            raise ak._errors.wrap_error(
-                TypeError("JSONSchema type is not concrete: array without items")
-            )
+            raise TypeError("JSONSchema type is not concrete: array without items")
 
         instructions.append(["TopLevelArray"])
         form = build_assembly(schema["items"], container, instructions)
         is_record = False
 
     elif schema.get("type") == "object":
         form = build_assembly(schema, container, instructions)
         is_record = True
 
     else:
-        raise ak._errors.wrap_error(
-            TypeError(
-                "only 'array' and 'object' types supported at the JSONSchema root"
-            )
+        raise TypeError(
+            "only 'array' and 'object' types supported at the JSONSchema root"
         )
 
     read_one = not line_delimited
 
     with _get_reader(source)() as obj:
         try:
             length = _ext.fromjsonobj_schema(
@@ -570,15 +560,15 @@
                 posinf_string,
                 neginf_string,
                 json.dumps(instructions),
                 initial,
                 resize,
             )
         except Exception as err:
-            raise ak._errors.wrap_error(ValueError(str(err))) from None
+            raise ValueError(str(err)) from None
 
     layout = ak.operations.from_buffers(
         form, length, container, byteorder=ak._util.native_byteorder, highlevel=False
     )
     layout = _record_to_complex(layout, complex_record_fields)
 
     if is_record and read_one:
@@ -588,22 +578,18 @@
         return wrap_layout(layout, behavior, highlevel)
     else:
         return layout
 
 
 def build_assembly(schema, container, instructions):
     if not isinstance(schema, dict):
-        raise ak._errors.wrap_error(
-            TypeError(f"unrecognized JSONSchema: expected dict, got {schema!r}")
-        )
+        raise TypeError(f"unrecognized JSONSchema: expected dict, got {schema!r}")
 
     if "type" not in schema is None:
-        raise ak._errors.wrap_error(
-            TypeError(f"unrecognized JSONSchema: no 'type' in {schema!r}")
-        )
+        raise TypeError(f"unrecognized JSONSchema: no 'type' in {schema!r}")
 
     tpe = schema["type"]
 
     is_optional = False
     if isinstance(tpe, list):
         if "null" in tpe:
             is_optional = True
@@ -722,17 +708,15 @@
             else:
                 return out
 
     elif tpe == "array":
         # https://json-schema.org/understanding-json-schema/reference/array.html
 
         if "items" not in schema:
-            raise ak._errors.wrap_error(
-                TypeError("JSONSchema type is not concrete: array without 'items'")
-            )
+            raise TypeError("JSONSchema type is not concrete: array without 'items'")
 
         if schema.get("minItems") == schema.get("maxItems") != None:  # noqa: E711
             assert is_integer(schema.get("minItems"))
 
             if is_optional:
                 mask = f"node{len(container)}"
                 container[mask + "-index"] = None
@@ -770,18 +754,16 @@
             else:
                 return out
 
     elif tpe == "object":
         # https://json-schema.org/understanding-json-schema/reference/object.html
 
         if "properties" not in schema:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "JSONSchema type is not concrete: object without 'properties'"
-                )
+            raise TypeError(
+                "JSONSchema type is not concrete: object without 'properties'"
             )
 
         names = []
         subschemas = []
         for name, subschema in schema["properties"].items():
             names.append(name)
             subschemas.append(subschema)
@@ -806,13 +788,11 @@
         out = ak.forms.RecordForm(contents, names)
         if is_optional:
             return ak.forms.IndexedOptionForm("i64", out, form_key=mask)
         else:
             return out
 
     elif isinstance(tpe, list):
-        raise ak._errors.wrap_error(
-            NotImplementedError("arbitrary unions of types are not yet supported")
-        )
+        raise NotImplementedError("arbitrary unions of types are not yet supported")
 
     else:
-        raise ak._errors.wrap_error(TypeError(f"unrecognized JSONSchema: {tpe!r}"))
+        raise TypeError(f"unrecognized JSONSchema: {tpe!r}")
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_from_numpy.py` & `awkward-2.1.2/src/awkward/operations/ak_from_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_from_parquet.py` & `awkward-2.1.2/src/awkward/operations/ak_from_parquet.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,19 +100,17 @@
 
     # early exit if missing deps
     pyarrow_parquet = awkward._connect.pyarrow.import_pyarrow_parquet("ak.from_parquet")
     import fsspec.parquet
 
     if row_groups is not None:
         if not all(is_integer(x) and x >= 0 for x in row_groups):
-            raise ak._errors.wrap_error(
-                ValueError("row_groups must be a set of non-negative integers")
-            )
+            raise ValueError("row_groups must be a set of non-negative integers")
         if len(set(row_groups)) < len(row_groups):
-            raise ak._errors.wrap_error(ValueError("row group indices must not repeat"))
+            raise ValueError("row group indices must not repeat")
 
     fs, _, paths = fsspec.get_fs_token_paths(
         path, mode="rb", storage_options=storage_options
     )
     all_paths, path_for_schema, can_sub = _all_and_metadata_paths(
         path, fs, paths, ignore_metadata, scan_files
     )
@@ -155,24 +153,20 @@
             with fs.open(apath, "rb") as f:
                 md = pyarrow_parquet.ParquetFile(f).metadata
                 # TODO: not nested directory structure yet
                 md.set_file_path(apath.rsplit("/", 1)[-1])
                 metadata.append_row_groups(md)
     if row_groups is not None:
         if any(_ >= metadata.num_row_groups for _ in row_groups):
-            raise ak._errors.wrap_error(
-                ValueError(
-                    f"Row group selection out of bounds 0..{metadata.num_row_groups - 1}"
-                )
+            raise ValueError(
+                f"Row group selection out of bounds 0..{metadata.num_row_groups - 1}"
             )
         if not can_sub:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "Requested selection of row-groups, but not scanning metadata"
-                )
+            raise TypeError(
+                "Requested selection of row-groups, but not scanning metadata"
             )
 
         path_rgs = {}
         rgs_path = {}
         subrg = []
         col_counts = []
         for i in range(metadata.num_row_groups):
@@ -352,12 +346,10 @@
                 path_for_metadata = all_paths[0][0]
         # we will still know rew-groups and counts if we scan, so can sub-select
         can_sub = scan_files or len(all_paths) == 1
 
     all_paths = [x for x, is_meta, is_comm in all_paths if not is_meta and not is_comm]
 
     if len(all_paths) == 0:
-        raise ak._errors.wrap_error(
-            ValueError(f"no *.parquet or *.parq matches for path {path!r}")
-        )
+        raise ValueError(f"no *.parquet or *.parq matches for path {path!r}")
 
     return all_paths, path_for_metadata, can_sub
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_from_rdataframe.py` & `awkward-2.1.2/src/awkward/operations/ak_from_rdataframe.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,30 +71,26 @@
         columns = (columns,)
         project = True
     else:
         columns = tuple(columns)
         project = False
 
     if not all(isinstance(x, str) for x in columns):
-        raise ak._errors.wrap_error(
-            TypeError(
-                f"'columns' must be a string or an iterable of strings, not {columns!r}"
-            )
+        raise TypeError(
+            f"'columns' must be a string or an iterable of strings, not {columns!r}"
         )
 
     if not isinstance(offsets_type, str) or offsets_type not in (
         "int32",
         "uint32",
         "int64",
     ):
-        raise ak._errors.wrap_error(
-            TypeError(
-                "'offsets_type' must be a string in (int32, uint32, int64), "
-                "not {}".format(repr(offsets_type))
-            )
+        raise TypeError(
+            "'offsets_type' must be a string in (int32, uint32, int64), "
+            "not {}".format(repr(offsets_type))
         )
     else:
         offsets_type = f"{offsets_type}_t"
 
     out = ak._connect.rdataframe.from_rdataframe.from_rdataframe(
         data_frame,
         columns,
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_from_regular.py` & `awkward-2.1.2/src/awkward/operations/ak_from_regular.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,16 +65,14 @@
         def action(layout, depth, **kwargs):
             posaxis = maybe_posaxis(layout, axis, depth)
             if posaxis == depth and layout.is_regular:
                 return layout.to_ListOffsetArray64(False)
             elif posaxis == depth and layout.is_list:
                 return layout
             elif layout.is_leaf:
-                raise ak._errors.wrap_error(
-                    np.AxisError(
-                        f"axis={axis} exceeds the depth of this array ({depth})"
-                    )
+                raise np.AxisError(
+                    f"axis={axis} exceeds the depth of this array ({depth})"
                 )
 
         out = ak._do.recursively_apply(layout, action, behavior, numpy_to_regular=True)
 
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_full_like.py` & `awkward-2.1.2/src/awkward/operations/ak_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_is_categorical.py` & `awkward-2.1.2/src/awkward/operations/ak_is_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_is_none.py` & `awkward-2.1.2/src/awkward/operations/ak_is_none.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,17 +34,15 @@
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array)
     behavior = behavior_of(array, behavior=behavior)
 
     if not is_integer(axis):
-        raise ak._errors.wrap_error(
-            TypeError(f"'axis' must be an integer, not {axis!r}")
-        )
+        raise TypeError(f"'axis' must be an integer, not {axis!r}")
 
     def action(layout, depth, lateral_context, **kwargs):
         posaxis = maybe_posaxis(layout, axis, depth)
 
         if posaxis is not None and posaxis + 1 == depth:
             if layout.is_union or layout.is_record:
                 return None
@@ -55,14 +53,12 @@
             else:
                 nplike = layout._backend.nplike
                 return ak.contents.NumpyArray(
                     nplike.zeros(layout.length, dtype=np.bool_)
                 )
 
         elif layout.is_leaf:
-            raise ak._errors.wrap_error(
-                np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
-            )
+            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
 
     out = ak._do.recursively_apply(layout, action, behavior, numpy_to_regular=True)
 
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_is_tuple.py` & `awkward-2.1.2/src/awkward/operations/ak_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_is_valid.py` & `awkward-2.1.2/src/awkward/operations/ak_is_valid.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_isclose.py` & `awkward-2.1.2/src/awkward/operations/ak_isclose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_linear_fit.py` & `awkward-2.1.2/src/awkward/operations/ak_linear_fit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_local_index.py` & `awkward-2.1.2/src/awkward/operations/ak_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_mask.py` & `awkward-2.1.2/src/awkward/operations/ak_mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,17 +103,15 @@
 
 def _impl(array, mask, valid_when, highlevel, behavior):
     def action(inputs, backend, **kwargs):
         layoutarray, layoutmask = inputs
         if isinstance(layoutmask, ak.contents.NumpyArray):
             m = backend.nplike.asarray(layoutmask)
             if not issubclass(m.dtype.type, (bool, np.bool_)):
-                raise ak._errors.wrap_error(
-                    ValueError(f"mask must have boolean type, not {repr(m.dtype)}")
-                )
+                raise ValueError(f"mask must have boolean type, not {repr(m.dtype)}")
             bytemask = ak.index.Index8(m.view(np.int8))
             return (
                 ak.contents.ByteMaskedArray.simplified(
                     bytemask, layoutarray, valid_when=valid_when
                 ),
             )
         else:
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_max.py` & `awkward-2.1.2/src/awkward/operations/ak_max.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(
             array,
             axis,
             keepdims,
             initial,
@@ -150,15 +150,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         array = ak.operations.ak_nan_to_none._impl(array, False, None)
 
         return _impl(
             array,
             axis,
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_mean.py` & `awkward-2.1.2/src/awkward/operations/ak_var.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,231 +1,230 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
-__all__ = ("mean",)
+__all__ = ("var",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import unsupported
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 from awkward._util import unset
 
 np = NumpyMetadata.instance()
 
 
-def mean(
+def var(
     x,
     weight=None,
+    ddof=0,
     axis=None,
     *,
     keepdims=False,
     mask_identity=False,
     flatten_records=unset,
 ):
     """
     Args:
-        x: The data on which to compute the mean (anything #ak.to_layout recognizes).
+        x: The data on which to compute the variance (anything #ak.to_layout recognizes).
         weight: Data that can be broadcasted to `x` to give each value a
             weight. Weighting values equally is the same as no weights;
             weighting some values higher increases the significance of those
             values. Weights can be zero or negative.
+        ddof (int): "delta degrees of freedom": the divisor used in the
+            calculation is `sum(weights) - ddof`. Use this for "reduced
+            variance."
         axis (None or int): If None, combine all values from the array into
             a single scalar result; if an int, group by that axis: `0` is the
             outermost, `1` is the first level of nested lists, etc., and
             negative `axis` counts from the innermost: `-1` is the innermost,
             `-2` is the next level up, etc.
         keepdims (bool): If False, this function decreases the number of
             dimensions by 1; if True, the output values are wrapped in a new
             length-1 dimension so that the result of this operation may be
             broadcasted with the original array.
         mask_identity (bool): If True, the application of this function on
             empty lists results in None (an option type); otherwise, the
             calculation is followed through with the reducers' identities,
             usually resulting in floating-point `nan`.
 
-    Computes the mean in each group of elements from `x` (many
+    Computes the variance in each group of elements from `x` (many
     types supported, including all Awkward Arrays and Records). The grouping
     is performed the same way as for reducers, though this operation is not a
     reducer and has no identity. It is the same as NumPy's
-    [mean](https://docs.scipy.org/doc/numpy/reference/generated/numpy.mean.html)
+    [var](https://docs.scipy.org/doc/numpy/reference/generated/numpy.var.html)
     if all lists at a given dimension have the same length and no None values,
     but it generalizes to cases where they do not.
 
-    Passing all arguments to the reducers, the mean is calculated as
+    Passing all arguments to the reducers, the variance is calculated as
 
-        ak.sum(x*weight) / ak.sum(weight)
+        ak.sum((x - ak.mean(x))**2 * weight) / ak.sum(weight)
 
-    For example, with an `array` like
+    If `ddof` is not zero, the above is further corrected by a factor of
 
-        >>> array = ak.Array([[0, 1, 2, 3],
-                              [          ],
-                              [4, 5      ]])
+        ak.sum(weight) / (ak.sum(weight) - ddof)
 
-    The mean of the innermost lists is
-
-        >>> ak.mean(array, axis=-1)
-        <Array [1.5, nan, 4.5] type='3 * float64'>
-
-    because there are three lists, the first has mean `1.5`, the second is
-    empty, and the third has mean `4.5`.
-
-    The mean of the outermost lists is
-
-        >>> ak.mean(array, axis=0)
-        <Array [2, 3, 2, 3] type='4 * float64'>
-
-    because the longest list has length 4, the mean of `0` and `4` is `2.0`,
-    the mean of `1` and `5` is `3.0`, the mean of `2` (by itself) is `2.0`,
-    and the mean of `3` (by itself) is `3.0`. This follows the same grouping
-    behavior as reducers.
+    Even without `ddof`, #ak.var differs from #ak.moment with `n=2` because
+    the mean is subtracted from all points before summing their squares.
 
     See #ak.sum for a complete description of handling nested lists and
-    missing values (None) in reducers.
+    missing values (None) in reducers, and #ak.mean for an example with another
+    non-reducer.
 
-    See also #ak.nanmean.
+    See also #ak.nanvar.
     """
     with ak._errors.OperationErrorContext(
-        "ak.mean",
+        "ak.var",
         {
             "x": x,
             "weight": weight,
+            "ddof": ddof,
             "axis": axis,
             "keepdims": keepdims,
             "mask_identity": mask_identity,
         },
     ):
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
-        return _impl(x, weight, axis, keepdims, mask_identity)
+        return _impl(x, weight, ddof, axis, keepdims, mask_identity)
 
 
-def nanmean(
+def nanvar(
     x,
     weight=None,
+    ddof=0,
     axis=None,
     *,
     keepdims=False,
     mask_identity=True,
     flatten_records=unset,
 ):
     """
     Args:
-        x: The data on which to compute the mean (anything #ak.to_layout recognizes).
+        x: The data on which to compute the variance (anything #ak.to_layout recognizes).
         weight: Data that can be broadcasted to `x` to give each value a
             weight. Weighting values equally is the same as no weights;
             weighting some values higher increases the significance of those
             values. Weights can be zero or negative.
+        ddof (int): "delta degrees of freedom": the divisor used in the
+            calculation is `sum(weights) - ddof`. Use this for "reduced
+            variance."
         axis (None or int): If None, combine all values from the array into
             a single scalar result; if an int, group by that axis: `0` is the
             outermost, `1` is the first level of nested lists, etc., and
             negative `axis` counts from the innermost: `-1` is the innermost,
             `-2` is the next level up, etc.
         keepdims (bool): If False, this function decreases the number of
             dimensions by 1; if True, the output values are wrapped in a new
             length-1 dimension so that the result of this operation may be
             broadcasted with the original array.
         mask_identity (bool): If True, the application of this function on
             empty lists results in None (an option type); otherwise, the
             calculation is followed through with the reducers' identities,
             usually resulting in floating-point `nan`.
 
-    Like #ak.mean, but treating NaN ("not a number") values as missing.
+    Like #ak.var, but treating NaN ("not a number") values as missing.
 
     Equivalent to
 
-        ak.mean(ak.nan_to_none(array))
+        ak.var(ak.nan_to_none(array))
 
     with all other arguments unchanged.
 
-    See also #ak.mean.
+    See also #ak.var.
     """
     with ak._errors.OperationErrorContext(
-        "ak.nanmean",
+        "ak.nanvar",
         {
             "x": x,
             "weight": weight,
+            "ddof": ddof,
             "axis": axis,
             "keepdims": keepdims,
             "mask_identity": mask_identity,
         },
     ):
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         x = ak.operations.ak_nan_to_none._impl(x, False, None)
         if weight is not None:
             weight = ak.operations.ak_nan_to_none._impl(weight, False, None)
 
-        return _impl(x, weight, axis, keepdims, mask_identity)
+        return _impl(x, weight, ddof, axis, keepdims, mask_identity)
 
 
-def _impl(x, weight, axis, keepdims, mask_identity):
+def _impl(x, weight, ddof, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
     behavior = behavior_of(x, weight)
     x = ak.highlevel.Array(
         ak.operations.to_layout(x, allow_record=False, allow_other=False),
         behavior=behavior,
     )
     if weight is not None:
         weight = ak.highlevel.Array(
             ak.operations.to_layout(weight, allow_record=False, allow_other=False),
             behavior=behavior,
         )
 
     with np.errstate(invalid="ignore", divide="ignore"):
+        xmean = ak.operations.ak_mean._impl(
+            x, weight, axis, keepdims=True, mask_identity=True
+        )
         if weight is None:
             sumw = ak.operations.ak_count._impl(
                 x,
                 axis,
                 keepdims=True,
                 mask_identity=True,
                 highlevel=True,
                 behavior=None,
             )
-            sumwx = ak.operations.ak_sum._impl(
-                x,
+            sumwxx = ak.operations.ak_sum._impl(
+                (x - xmean) ** 2,
                 axis,
                 keepdims=True,
                 mask_identity=True,
                 highlevel=True,
                 behavior=None,
             )
         else:
             sumw = ak.operations.ak_sum._impl(
                 x * 0 + weight,
                 axis,
-                keepdims,
-                mask_identity,
+                keepdims=True,
+                mask_identity=True,
                 highlevel=True,
                 behavior=None,
             )
-            sumwx = ak.operations.ak_sum._impl(
-                x * weight,
+            sumwxx = ak.operations.ak_sum._impl(
+                (x - xmean) ** 2 * weight,
                 axis,
                 keepdims=True,
                 mask_identity=True,
                 highlevel=True,
                 behavior=None,
             )
-
-        out = sumwx / sumw
+        if ddof != 0:
+            out = (sumwxx / sumw) * (sumw / (sumw - ddof))
+        else:
+            out = sumwxx / sumw
 
         if not mask_identity:
             out = ak.highlevel.Array(ak.operations.fill_none(out, np.nan, axis=-1))
 
         if axis is None:
             if not keepdims:
                 out = out[(0,) * out.ndim]
@@ -233,31 +232,33 @@
             if not keepdims:
                 posaxis = maybe_posaxis(out.layout, axis, 1)
                 out = out[(slice(None, None),) * posaxis + (0,)]
 
         return out
 
 
-@ak._connect.numpy.implements("mean")
-def _nep_18_impl_mean(
+@ak._connect.numpy.implements("var")
+def _nep_18_impl_var(
     a,
     axis=None,
     dtype=unsupported,
     out=unsupported,
+    ddof=0,
     keepdims=False,
     *,
     where=unsupported,
 ):
-    return mean(a, axis=axis, keepdims=keepdims)
+    return var(a, axis=axis, keepdims=keepdims, ddof=ddof)
 
 
-@ak._connect.numpy.implements("nanmean")
-def _nep_18_impl_nanmean(
+@ak._connect.numpy.implements("nanvar")
+def _nep_18_impl_nanvar(
     a,
     axis=None,
     dtype=unsupported,
     out=unsupported,
+    ddof=0,
     keepdims=False,
     *,
     where=unsupported,
 ):
-    return nanmean(a, axis=axis, keepdims=keepdims)
+    return nanvar(a, axis=axis, keepdims=keepdims, ddof=ddof)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_merge_option_of_records.py` & `awkward-2.1.2/src/awkward/operations/ak_merge_option_of_records.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,17 +63,15 @@
             )
 
     layout = ak._do.recursively_apply(layout, apply_displace_index)
 
     def apply(layout, depth, backend, **kwargs):
         posaxis = maybe_posaxis(layout, axis, depth)
         if depth < posaxis + 1 and layout.is_leaf:
-            raise ak._errors.wrap_error(
-                np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
-            )
+            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
         elif depth == posaxis + 1 and layout.is_option and layout.content.is_record:
             layout = layout.to_IndexedOptionArray64()
 
             record = layout.content
             # Transpose option-of-record to record-of-option
             return ak.contents.RecordArray(
                 [
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_merge_union_of_records.py` & `awkward-2.1.2/src/awkward/operations/ak_merge_union_of_records.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,17 +150,15 @@
             dtype=index.dtype,
         )
         return dense_index
 
     def apply(layout, depth, backend, **kwargs):
         posaxis = maybe_posaxis(layout, axis, depth)
         if depth < posaxis + 1 and layout.is_leaf:
-            raise ak._errors.wrap_error(
-                np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
-            )
+            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
         elif depth == posaxis + 1 and layout.is_union:
             if not all(
                 x.is_record or x.is_indexed or x.is_option for x in layout.contents
             ):
                 return
 
             # Any option types need to be re-written
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_metadata_from_parquet.py` & `awkward-2.1.2/src/awkward/operations/ak_metadata_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_min.py` & `awkward-2.1.2/src/awkward/operations/ak_min.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(
             array,
             axis,
             keepdims,
             initial,
@@ -148,15 +148,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         array = ak.operations.ak_nan_to_none._impl(array, False, None)
 
         return _impl(
             array,
             axis,
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_moment.py` & `awkward-2.1.2/src/awkward/operations/ak_moment.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(x, n, weight, axis, keepdims, mask_identity)
 
 
 def _impl(x, n, weight, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_nan_to_none.py` & `awkward-2.1.2/src/awkward/operations/ak_nan_to_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_nan_to_num.py` & `awkward-2.1.2/src/awkward/operations/ak_nan_to_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_num.py` & `awkward-2.1.2/src/awkward/operations/ak_num.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,31 +77,27 @@
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array)
     behavior = behavior_of(array, behavior=behavior)
 
     if not is_integer(axis):
-        raise ak._errors.wrap_error(
-            TypeError(f"'axis' must be an integer, not {axis!r}")
-        )
+        raise TypeError(f"'axis' must be an integer, not {axis!r}")
 
     if maybe_posaxis(layout, axis, 1) == 0:
         if isinstance(layout, ak.record.Record):
             return 1
         else:
             return layout.length
 
     def action(layout, depth, **kwargs):
         posaxis = maybe_posaxis(layout, axis, depth)
 
         if posaxis == depth and layout.is_list:
             return ak.contents.NumpyArray(layout.stops.data - layout.starts.data)
 
         elif layout.is_leaf:
-            raise ak._errors.wrap_error(
-                np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
-            )
+            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
 
     out = ak._do.recursively_apply(layout, action, behavior, numpy_to_regular=True)
 
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_ones_like.py` & `awkward-2.1.2/src/awkward/operations/ak_ones_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_pad_none.py` & `awkward-2.1.2/src/awkward/operations/ak_pad_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_parameters.py` & `awkward-2.1.2/src/awkward/operations/ak_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_prod.py` & `awkward-2.1.2/src/awkward/operations/ak_prod.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
 
 def nanprod(
     array,
@@ -127,15 +127,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         array = ak.operations.ak_nan_to_none._impl(array, False, None)
 
         return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_ptp.py` & `awkward-2.1.2/src/awkward/operations/ak_ptp.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(array, axis, keepdims, mask_identity)
 
 
 def _impl(array, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_ravel.py` & `awkward-2.1.2/src/awkward/operations/ak_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_run_lengths.py` & `awkward-2.1.2/src/awkward/operations/ak_run_lengths.py`

 * *Files 7% similar despite different names*

```diff
@@ -153,29 +153,25 @@
                 layout.parameter("__array__") == "string"
                 or layout.parameter("__array__") == "bytestring"
             ):
                 nextcontent, _ = lengths_of(ak.highlevel.Array(layout), None)
                 return ak.contents.NumpyArray(nextcontent)
 
             if not isinstance(layout, (ak.contents.NumpyArray, ak.contents.EmptyArray)):
-                raise ak._errors.wrap_error(
-                    NotImplementedError("run_lengths on " + type(layout).__name__)
-                )
+                raise NotImplementedError("run_lengths on " + type(layout).__name__)
 
             nextcontent, _ = lengths_of(backend.nplike.asarray(layout), None)
             return ak.contents.NumpyArray(nextcontent)
 
         elif layout.branch_depth == (False, 2):
             if layout.is_indexed:
                 layout = layout.project()
 
             if not layout.is_list:
-                raise ak._errors.wrap_error(
-                    NotImplementedError("run_lengths on " + type(layout).__name__)
-                )
+                raise NotImplementedError("run_lengths on " + type(layout).__name__)
 
             if (
                 layout.content.parameter("__array__") == "string"
                 or layout.content.parameter("__array__") == "bytestring"
             ):
                 # We also want to trim the _upper_ bound of content,
                 # so we manually convert the list type to zero-based
@@ -200,21 +196,19 @@
 
             if content.is_indexed:
                 content = content.project()
 
             if not isinstance(
                 content, (ak.contents.NumpyArray, ak.contents.EmptyArray)
             ):
-                raise ak._errors.wrap_error(
-                    NotImplementedError(
-                        "run_lengths on "
-                        + type(layout).__name__
-                        + " with content "
-                        + type(content).__name__
-                    )
+                raise NotImplementedError(
+                    "run_lengths on "
+                    + type(layout).__name__
+                    + " with content "
+                    + type(content).__name__
                 )
 
             nextcontent, nextoffsets = lengths_of(
                 backend.nplike.asarray(content), offsets - offsets[0]
             )
             return ak.contents.ListOffsetArray(
                 ak.index.Index64(nextoffsets),
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_singletons.py` & `awkward-2.1.2/src/awkward/operations/ak_singletons.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,17 +49,15 @@
 
 def _impl(array, axis, highlevel, behavior):
     axis = regularize_axis(axis)
     layout = ak.operations.to_layout(array)
     behavior = behavior_of(array, behavior=behavior)
 
     if not is_integer(axis):
-        raise ak._errors.wrap_error(
-            TypeError(f"'axis' must be an integer, not {axis!r}")
-        )
+        raise TypeError(f"'axis' must be an integer, not {axis!r}")
 
     def action(layout, depth, **kwargs):
         posaxis = maybe_posaxis(layout, axis, depth)
 
         if posaxis is not None and posaxis + 1 == depth:
             if layout.is_union or layout.is_record:
                 return None
@@ -78,14 +76,12 @@
                     ak.index.Index64(offsets), layout.project()
                 )
 
             else:
                 return ak.contents.RegularArray(layout, 1).to_ListOffsetArray64(True)
 
         elif layout.is_leaf:
-            raise ak._errors.wrap_error(
-                np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
-            )
+            raise np.AxisError(f"axis={axis} exceeds the depth of this array ({depth})")
 
     out = ak._do.recursively_apply(layout, action, behavior, numpy_to_regular=True)
 
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_softmax.py` & `awkward-2.1.2/src/awkward/operations/ak_softmax.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(x, axis, keepdims, mask_identity)
 
 
 def _impl(x, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_sort.py` & `awkward-2.1.2/src/awkward/operations/ak_sort.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,13 +60,11 @@
     if kind is None:
         stable = False
     elif kind in ("stable", "mergesort"):
         stable = True
     elif kind in ("heapsort", "quicksort"):
         stable = False
     else:
-        raise ak._errors.wrap_error(
-            ValueError(
-                f"unsupported value for 'kind' passed to overloaded NumPy function 'sort': {kind!r}"
-            )
+        raise ValueError(
+            f"unsupported value for 'kind' passed to overloaded NumPy function 'sort': {kind!r}"
         )
     return sort(a, axis=axis, stable=stable)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_std.py` & `awkward-2.1.2/src/awkward/operations/ak_std.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(x, weight, ddof, axis, keepdims, mask_identity)
 
 
 def nanstd(
     x,
@@ -147,15 +147,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         x = ak.operations.ak_nan_to_none._impl(x, False, None)
         if weight is not None:
             weight = ak.operations.ak_nan_to_none._impl(weight, False, None)
 
         return _impl(x, weight, ddof, axis, keepdims, mask_identity)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_strings_astype.py` & `awkward-2.1.2/src/awkward/operations/ak_strings_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_sum.py` & `awkward-2.1.2/src/awkward/operations/ak_sum.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
 
 
 def nansum(
     array,
@@ -275,15 +275,15 @@
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         array = ak.operations.ak_nan_to_none._impl(array, False, None)
 
         return _impl(array, axis, keepdims, mask_identity, highlevel, behavior)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_arrow.py` & `awkward-2.1.2/src/awkward/operations/ak_to_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_arrow_table.py` & `awkward-2.1.2/src/awkward/operations/ak_to_arrow_table.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_backend.py` & `awkward-2.1.2/src/awkward/operations/ak_to_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_buffers.py` & `awkward-2.1.2/src/awkward/operations/ak_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_categorical.py` & `awkward-2.1.2/src/awkward/operations/ak_to_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_cupy.py` & `awkward-2.1.2/src/awkward/operations/ak_to_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_dataframe.py` & `awkward-2.1.2/src/awkward/operations/ak_to_dataframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,24 +134,22 @@
         return _impl(array, how, levelname, anonymous)
 
 
 def _impl(array, how, levelname, anonymous):
     try:
         import pandas
     except ImportError as err:
-        raise ak._errors.wrap_error(
-            ImportError(
-                """install the 'pandas' package with:
+        raise ImportError(
+            """install the 'pandas' package with:
 
     pip install pandas --upgrade
 
 or
 
     conda install pandas"""
-            )
         ) from err
 
     if how is not None:
         out = None
         for df in to_dataframe(
             array, how=None, levelname=levelname, anonymous=anonymous
         ):
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_jax.py` & `awkward-2.1.2/src/awkward/operations/ak_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_json.py` & `awkward-2.1.2/src/awkward/operations/ak_to_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,17 +181,15 @@
     elif isinstance(array, ak.contents.Content):
         out = array
 
     elif hasattr(array, "shape") and hasattr(array, "dtype"):
         out = ak.contents.NumpyArray(array)
 
     else:
-        raise ak._errors.wrap_error(
-            TypeError(f"unrecognized array type: {repr(array)}")
-        )
+        raise TypeError(f"unrecognized array type: {repr(array)}")
 
     jsondata = out.to_json(
         nan_string=nan_string,
         posinf_string=posinf_string,
         neginf_string=neginf_string,
         complex_record_fields=complex_record_fields,
         convert_bytes=convert_bytes,
@@ -291,15 +289,15 @@
                         indent=num_indent_spaces,
                         separators=separators,
                         default=convert_other,
                         sort_keys=False,
                     )
 
     except Exception as err:
-        raise ak._errors.wrap_error(err) from err
+        raise err from err
 
 
 class _NoContextManager:
     def __init__(self, file):
         self.file = file
 
     def __enter__(self):
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_layout.py` & `awkward-2.1.2/src/awkward/operations/ak_to_layout.py`

 * *Files 17% similar despite different names*

```diff
@@ -54,28 +54,24 @@
 
 def _impl(array, allow_record, allow_other, regulararray):
     if isinstance(array, ak.contents.Content):
         return array
 
     elif isinstance(array, ak.record.Record):
         if not allow_record:
-            raise _errors.wrap_error(
-                TypeError("ak.Record objects are not allowed in this function")
-            )
+            raise TypeError("ak.Record objects are not allowed in this function")
         else:
             return array
 
     elif isinstance(array, ak.highlevel.Array):
         return array.layout
 
     elif isinstance(array, ak.highlevel.Record):
         if not allow_record:
-            raise _errors.wrap_error(
-                TypeError("ak.Record objects are not allowed in this function")
-            )
+            raise TypeError("ak.Record objects are not allowed in this function")
         else:
             return array.layout
 
     elif isinstance(array, ak.highlevel.ArrayBuilder):
         return array.snapshot().layout
 
     elif isinstance(array, _ext.ArrayBuilder):
@@ -97,18 +93,16 @@
     elif TypeTracer.is_own_array(array):
         backend = ak._backends.TypeTracerBackend.instance()
 
         if len(array.shape) == 0:
             array = backend.nplike.reshape(array, (1,))
 
         if array.dtype.kind in {"S", "U"}:
-            raise _errors.wrap_error(
-                NotImplementedError(
-                    "strings are currently not supported for typetracer arrays"
-                )
+            raise NotImplementedError(
+                "strings are currently not supported for typetracer arrays"
             )
 
         return ak.contents.NumpyArray(array, parameters=None, backend=backend)
 
     elif ak._util.in_module(array, "pyarrow"):
         return ak.operations.from_arrow(array, highlevel=False)
 
@@ -120,15 +114,13 @@
             ak.operations.from_iter(array, highlevel=False),
             allow_record,
             allow_other,
             regulararray,
         )
 
     elif not allow_other:
-        raise _errors.wrap_error(
-            TypeError(
-                f"{array} cannot be converted into an Awkward Array, and non-array-like objects are not supported."
-            )
+        raise TypeError(
+            f"{array} cannot be converted into an Awkward Array, and non-array-like objects are not supported."
         )
 
     else:
         return array
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_list.py` & `awkward-2.1.2/src/awkward/operations/ak_to_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_numpy.py` & `awkward-2.1.2/src/awkward/operations/ak_to_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_packed.py` & `awkward-2.1.2/src/awkward/operations/ak_to_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_parquet.py` & `awkward-2.1.2/src/awkward/operations/ak_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_rdataframe.py` & `awkward-2.1.2/src/awkward/operations/ak_to_rdataframe.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,39 +53,31 @@
 def _impl(
     arrays,
     flatlist_as_rvec,
 ):
     import awkward._connect.rdataframe.to_rdataframe  # noqa: F401
 
     if not isinstance(arrays, Mapping):
-        raise ak._errors.wrap_error(
-            TypeError("'arrays' must be a dict (to provide C++ names for the arrays)")
-        )
+        raise TypeError("'arrays' must be a dict (to provide C++ names for the arrays)")
     elif not all(isinstance(name, str) for name in arrays):
-        raise ak._errors.wrap_error(
-            TypeError(
-                "keys of 'arrays' dict must be strings (to provide C++ names for the arrays)"
-            )
+        raise TypeError(
+            "keys of 'arrays' dict must be strings (to provide C++ names for the arrays)"
         )
     elif len(arrays) == 0:
-        raise ak._errors.wrap_error(
-            TypeError("'arrays' must contain at least one array")
-        )
+        raise TypeError("'arrays' must contain at least one array")
 
     layouts = {}
     length = None
     for name, array in arrays.items():
         layouts[name] = ak.operations.ak_to_layout._impl(
             array, allow_record=False, allow_other=False, regulararray=True
         ).to_backend(cpu)
         if length is None:
             length = layouts[name].length
         elif length != layouts[name].length:
-            raise ak._errors.wrap_error(
-                ValueError("lengths of 'arrays' must all be the same")
-            )
+            raise ValueError("lengths of 'arrays' must all be the same")
 
     return ak._connect.rdataframe.to_rdataframe.to_rdataframe(
         layouts,
         length,
         flatlist_as_rvec=flatlist_as_rvec,
     )
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_to_regular.py` & `awkward-2.1.2/src/awkward/operations/ak_to_regular.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,16 +77,14 @@
 
         def action(layout, depth, **kwargs):
             posaxis = maybe_posaxis(layout, axis, depth)
             if posaxis == depth and layout.is_list:
                 return layout.to_RegularArray()
 
             elif layout.is_leaf:
-                raise ak._errors.wrap_error(
-                    np.AxisError(
-                        f"axis={axis} exceeds the depth of this array ({depth})"
-                    )
+                raise np.AxisError(
+                    f"axis={axis} exceeds the depth of this array ({depth})"
                 )
 
         out = ak._do.recursively_apply(layout, action, behavior)
 
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_transform.py` & `awkward-2.1.2/src/awkward/operations/ak_transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -493,18 +493,16 @@
             if out is None:
                 return out
 
             elif isinstance(out, ak.contents.Content):
                 return out
 
             else:
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        f"transformation must return a Content or None, not {type(out)}\n\n{out!r}"
-                    )
+                raise TypeError(
+                    f"transformation must return a Content or None, not {type(out)}\n\n{out!r}"
                 )
 
         # An exception to the rule of ak._do.recursively_apply, for symmetry with
         # ak._broadcasting.apply_step, below. ak_transform._impl knows implementation details.
         out = layout._recursively_apply(
             action,
             behavior,
@@ -527,29 +525,25 @@
                     return tuple(inputs)
                 else:
                     return None
 
             elif isinstance(out, tuple):
                 for x in out:
                     if not isinstance(x, ak.contents.Content):
-                        raise ak._errors.wrap_error(
-                            TypeError(
-                                f"transformation must return a Content, tuple of Contents, or None, not a tuple containing {type(x)}\n\n{x!r}"
-                            )
+                        raise TypeError(
+                            f"transformation must return a Content, tuple of Contents, or None, not a tuple containing {type(x)}\n\n{x!r}"
                         )
                 return out
 
             elif isinstance(out, ak.contents.Content):
                 return (out,)
 
             else:
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        f"transformation must return a Content, tuple of Contents, or None, not {type(out)}\n\n{out!r}"
-                    )
+                raise TypeError(
+                    f"transformation must return a Content, tuple of Contents, or None, not {type(out)}\n\n{out!r}"
                 )
 
         inputs = [layout, *more_layouts]
         isscalar = []
         out = ak._broadcasting.apply_step(
             backend,
             ak._broadcasting.broadcast_pack(inputs, isscalar),
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_type.py` & `awkward-2.1.2/src/awkward/operations/ak_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,10 +125,8 @@
         if layout is None:
             return ak.types.ScalarType(ak.types.UnknownType())
 
         elif isinstance(layout, (ak.contents.Content, ak.record.Record)):
             return _impl(layout, behavior)
 
         else:
-            raise ak._errors.wrap_error(
-                TypeError(f"unrecognized array type: {array!r}")
-            )
+            raise TypeError(f"unrecognized array type: {array!r}")
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_unflatten.py` & `awkward-2.1.2/src/awkward/operations/ak_unflatten.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,42 +112,38 @@
             counts = ak.operations.fill_none(
                 counts, 0, axis=-1, highlevel=False
             ).to_backend_array()
         elif counts.is_numpy or counts.is_unknown:
             counts = counts.to_backend_array()
             mask = False
         else:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "counts must be an integer or a one-dimensional array of integers"
-                )
+            raise ValueError(
+                "counts must be an integer or a one-dimensional array of integers"
             )
 
         if counts.ndim != 1:
-            raise ak._errors.wrap_error(ValueError("counts must be one-dimensional"))
+            raise ValueError("counts must be one-dimensional")
 
         if not np.issubdtype(counts.dtype, np.integer):
-            raise ak._errors.wrap_error(ValueError("counts must be integers"))
+            raise ValueError("counts must be integers")
 
         current_offsets = backend.index_nplike.empty(counts.size + 1, dtype=np.int64)
         current_offsets[0] = 0
         backend.index_nplike.cumsum(counts, maybe_out=current_offsets[1:])
 
     def unflatten_this_layout(layout):
         nonlocal current_offsets
 
         if isinstance(counts, int) or counts is unknown_length:
             if (
                 counts is not unknown_length
                 and layout.length is not unknown_length
                 and not 0 <= counts < layout.length
             ):
-                raise ak._errors.wrap_error(
-                    ValueError("too large counts for array or negative counts")
-                )
+                raise ValueError("too large counts for array or negative counts")
             out = ak.contents.RegularArray(layout, counts)
 
         else:
             position = (
                 backend.index_nplike.searchsorted(
                     current_offsets,
                     backend.index_nplike.asarray(
@@ -162,19 +158,17 @@
                 and layout.length is not unknown_length
                 and not is_unknown_scalar(position)
                 and (
                     position >= current_offsets.size
                     or current_offsets[position] != layout.length
                 )
             ):
-                raise ak._errors.wrap_error(
-                    ValueError(
-                        "structure imposed by 'counts' does not fit in the array or partition "
-                        "at axis={}".format(axis)
-                    )
+                raise ValueError(
+                    "structure imposed by 'counts' does not fit in the array or partition "
+                    "at axis={}".format(axis)
                 )
 
             offsets = current_offsets[: position + 1]
             current_offsets = current_offsets[
                 position:
             ] - backend.index_nplike.shape_item_as_index(layout.length)
 
@@ -217,32 +211,28 @@
                         inneroffsets, outeroffsets, side="right"
                     )
                     - 1
                 )
                 if not backend.index_nplike.array_equal(
                     inneroffsets[positions], outeroffsets
                 ):
-                    raise ak._errors.wrap_error(
-                        ValueError(
-                            "structure imposed by 'counts' does not fit in the array or partition "
-                            "at axis={}".format(axis)
-                        )
+                    raise ValueError(
+                        "structure imposed by 'counts' does not fit in the array or partition "
+                        "at axis={}".format(axis)
                     )
                 positions[0] = 0
 
                 return ak.contents.ListOffsetArray(ak.index.Index64(positions), content)
 
         out = ak._do.recursively_apply(layout, apply)
 
     if (
         current_offsets is not None
         and current_offsets.size is not unknown_length
         and not (current_offsets.size == 1 and current_offsets[0] == 0)
     ):
-        raise ak._errors.wrap_error(
-            ValueError(
-                "structure imposed by 'counts' does not fit in the array or partition "
-                "at axis={}".format(axis)
-            )
+        raise ValueError(
+            "structure imposed by 'counts' does not fit in the array or partition "
+            "at axis={}".format(axis)
         )
 
     return wrap_layout(out, behavior, highlevel)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_unzip.py` & `awkward-2.1.2/src/awkward/operations/ak_unzip.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,26 +44,23 @@
 def _impl(array, highlevel, behavior):
     behavior = behavior_of(array, behavior=behavior)
     layout = ak.operations.to_layout(array, allow_record=True, allow_other=False)
     fields = ak.operations.fields(layout)
 
     def check_for_union(layout, **kwargs):
         if isinstance(layout, (ak.contents.RecordArray, ak.Record)):
-            pass  # don't descend into nested records
+            return layout  # don't descend into nested records
 
-        elif isinstance(layout, ak.contents.UnionArray):
+        elif layout.is_union:
             for content in layout.contents:
                 if set(ak.operations.fields(content)) != set(fields):
-                    raise ak._errors.wrap_error(
-                        ValueError("union of different sets of fields, cannot ak.unzip")
+                    raise ValueError(
+                        "union of different sets of fields, cannot ak.unzip"
                     )
 
-        elif hasattr(layout, "content"):
-            check_for_union(layout.content)
-
     ak._do.recursively_apply(layout, check_for_union, behavior, return_array=False)
 
     if len(fields) == 0:
         return (wrap_layout(layout, behavior, highlevel, allow_other=True),)
     else:
         return tuple(
             wrap_layout(layout[n], behavior, highlevel, allow_other=True)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_validity_error.py` & `awkward-2.1.2/src/awkward/operations/ak_validity_error.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,10 +27,10 @@
 
 
 def _impl(array, exception):
     layout = ak.operations.to_layout(array, allow_record=False, allow_other=False)
     out = ak._do.validity_error(layout, path="highlevel")
 
     if out not in (None, "") and exception:
-        raise ak._errors.wrap_error(ValueError(out))
+        raise ValueError(out)
     else:
         return out
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_values_astype.py` & `awkward-2.1.2/src/awkward/operations/ak_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_var.py` & `awkward-2.1.2/src/awkward/operations/ak_mean.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,230 +1,231 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
-__all__ = ("var",)
+__all__ = ("mean",)
 import awkward as ak
 from awkward._behavior import behavior_of
 from awkward._connect.numpy import unsupported
 from awkward._layout import maybe_posaxis
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward._regularize import regularize_axis
 from awkward._util import unset
 
 np = NumpyMetadata.instance()
 
 
-def var(
+def mean(
     x,
     weight=None,
-    ddof=0,
     axis=None,
     *,
     keepdims=False,
     mask_identity=False,
     flatten_records=unset,
 ):
     """
     Args:
-        x: The data on which to compute the variance (anything #ak.to_layout recognizes).
+        x: The data on which to compute the mean (anything #ak.to_layout recognizes).
         weight: Data that can be broadcasted to `x` to give each value a
             weight. Weighting values equally is the same as no weights;
             weighting some values higher increases the significance of those
             values. Weights can be zero or negative.
-        ddof (int): "delta degrees of freedom": the divisor used in the
-            calculation is `sum(weights) - ddof`. Use this for "reduced
-            variance."
         axis (None or int): If None, combine all values from the array into
             a single scalar result; if an int, group by that axis: `0` is the
             outermost, `1` is the first level of nested lists, etc., and
             negative `axis` counts from the innermost: `-1` is the innermost,
             `-2` is the next level up, etc.
         keepdims (bool): If False, this function decreases the number of
             dimensions by 1; if True, the output values are wrapped in a new
             length-1 dimension so that the result of this operation may be
             broadcasted with the original array.
         mask_identity (bool): If True, the application of this function on
             empty lists results in None (an option type); otherwise, the
             calculation is followed through with the reducers' identities,
             usually resulting in floating-point `nan`.
 
-    Computes the variance in each group of elements from `x` (many
+    Computes the mean in each group of elements from `x` (many
     types supported, including all Awkward Arrays and Records). The grouping
     is performed the same way as for reducers, though this operation is not a
     reducer and has no identity. It is the same as NumPy's
-    [var](https://docs.scipy.org/doc/numpy/reference/generated/numpy.var.html)
+    [mean](https://docs.scipy.org/doc/numpy/reference/generated/numpy.mean.html)
     if all lists at a given dimension have the same length and no None values,
     but it generalizes to cases where they do not.
 
-    Passing all arguments to the reducers, the variance is calculated as
+    Passing all arguments to the reducers, the mean is calculated as
 
-        ak.sum((x - ak.mean(x))**2 * weight) / ak.sum(weight)
+        ak.sum(x*weight) / ak.sum(weight)
 
-    If `ddof` is not zero, the above is further corrected by a factor of
+    For example, with an `array` like
 
-        ak.sum(weight) / (ak.sum(weight) - ddof)
+        >>> array = ak.Array([[0, 1, 2, 3],
+                              [          ],
+                              [4, 5      ]])
 
-    Even without `ddof`, #ak.var differs from #ak.moment with `n=2` because
-    the mean is subtracted from all points before summing their squares.
+    The mean of the innermost lists is
+
+        >>> ak.mean(array, axis=-1)
+        <Array [1.5, nan, 4.5] type='3 * float64'>
+
+    because there are three lists, the first has mean `1.5`, the second is
+    empty, and the third has mean `4.5`.
+
+    The mean of the outermost lists is
+
+        >>> ak.mean(array, axis=0)
+        <Array [2, 3, 2, 3] type='4 * float64'>
+
+    because the longest list has length 4, the mean of `0` and `4` is `2.0`,
+    the mean of `1` and `5` is `3.0`, the mean of `2` (by itself) is `2.0`,
+    and the mean of `3` (by itself) is `3.0`. This follows the same grouping
+    behavior as reducers.
 
     See #ak.sum for a complete description of handling nested lists and
-    missing values (None) in reducers, and #ak.mean for an example with another
-    non-reducer.
+    missing values (None) in reducers.
 
-    See also #ak.nanvar.
+    See also #ak.nanmean.
     """
     with ak._errors.OperationErrorContext(
-        "ak.var",
+        "ak.mean",
         {
             "x": x,
             "weight": weight,
-            "ddof": ddof,
             "axis": axis,
             "keepdims": keepdims,
             "mask_identity": mask_identity,
         },
     ):
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
-        return _impl(x, weight, ddof, axis, keepdims, mask_identity)
+        return _impl(x, weight, axis, keepdims, mask_identity)
 
 
-def nanvar(
+def nanmean(
     x,
     weight=None,
-    ddof=0,
     axis=None,
     *,
     keepdims=False,
     mask_identity=True,
     flatten_records=unset,
 ):
     """
     Args:
-        x: The data on which to compute the variance (anything #ak.to_layout recognizes).
+        x: The data on which to compute the mean (anything #ak.to_layout recognizes).
         weight: Data that can be broadcasted to `x` to give each value a
             weight. Weighting values equally is the same as no weights;
             weighting some values higher increases the significance of those
             values. Weights can be zero or negative.
-        ddof (int): "delta degrees of freedom": the divisor used in the
-            calculation is `sum(weights) - ddof`. Use this for "reduced
-            variance."
         axis (None or int): If None, combine all values from the array into
             a single scalar result; if an int, group by that axis: `0` is the
             outermost, `1` is the first level of nested lists, etc., and
             negative `axis` counts from the innermost: `-1` is the innermost,
             `-2` is the next level up, etc.
         keepdims (bool): If False, this function decreases the number of
             dimensions by 1; if True, the output values are wrapped in a new
             length-1 dimension so that the result of this operation may be
             broadcasted with the original array.
         mask_identity (bool): If True, the application of this function on
             empty lists results in None (an option type); otherwise, the
             calculation is followed through with the reducers' identities,
             usually resulting in floating-point `nan`.
 
-    Like #ak.var, but treating NaN ("not a number") values as missing.
+    Like #ak.mean, but treating NaN ("not a number") values as missing.
 
     Equivalent to
 
-        ak.var(ak.nan_to_none(array))
+        ak.mean(ak.nan_to_none(array))
 
     with all other arguments unchanged.
 
-    See also #ak.var.
+    See also #ak.mean.
     """
     with ak._errors.OperationErrorContext(
-        "ak.nanvar",
+        "ak.nanmean",
         {
             "x": x,
             "weight": weight,
-            "ddof": ddof,
             "axis": axis,
             "keepdims": keepdims,
             "mask_identity": mask_identity,
         },
     ):
         if flatten_records is not unset:
             message = (
                 "`flatten_records` is no longer a supported argument for reducers. "
                 "Instead, use `ak.ravel(array)` first to remove the record structure "
                 "and flatten the array."
             )
             if flatten_records:
-                raise ak._errors.wrap_error(ValueError(message))
+                raise ValueError(message)
             else:
                 ak._errors.deprecate(message, "2.2.0")
         x = ak.operations.ak_nan_to_none._impl(x, False, None)
         if weight is not None:
             weight = ak.operations.ak_nan_to_none._impl(weight, False, None)
 
-        return _impl(x, weight, ddof, axis, keepdims, mask_identity)
+        return _impl(x, weight, axis, keepdims, mask_identity)
 
 
-def _impl(x, weight, ddof, axis, keepdims, mask_identity):
+def _impl(x, weight, axis, keepdims, mask_identity):
     axis = regularize_axis(axis)
     behavior = behavior_of(x, weight)
     x = ak.highlevel.Array(
         ak.operations.to_layout(x, allow_record=False, allow_other=False),
         behavior=behavior,
     )
     if weight is not None:
         weight = ak.highlevel.Array(
             ak.operations.to_layout(weight, allow_record=False, allow_other=False),
             behavior=behavior,
         )
 
     with np.errstate(invalid="ignore", divide="ignore"):
-        xmean = ak.operations.ak_mean._impl(
-            x, weight, axis, keepdims=True, mask_identity=True
-        )
         if weight is None:
             sumw = ak.operations.ak_count._impl(
                 x,
                 axis,
                 keepdims=True,
                 mask_identity=True,
                 highlevel=True,
                 behavior=None,
             )
-            sumwxx = ak.operations.ak_sum._impl(
-                (x - xmean) ** 2,
+            sumwx = ak.operations.ak_sum._impl(
+                x,
                 axis,
                 keepdims=True,
                 mask_identity=True,
                 highlevel=True,
                 behavior=None,
             )
         else:
             sumw = ak.operations.ak_sum._impl(
                 x * 0 + weight,
                 axis,
-                keepdims=True,
-                mask_identity=True,
+                keepdims,
+                mask_identity,
                 highlevel=True,
                 behavior=None,
             )
-            sumwxx = ak.operations.ak_sum._impl(
-                (x - xmean) ** 2 * weight,
+            sumwx = ak.operations.ak_sum._impl(
+                x * weight,
                 axis,
                 keepdims=True,
                 mask_identity=True,
                 highlevel=True,
                 behavior=None,
             )
-        if ddof != 0:
-            out = (sumwxx / sumw) * (sumw / (sumw - ddof))
-        else:
-            out = sumwxx / sumw
+
+        out = sumwx / sumw
 
         if not mask_identity:
             out = ak.highlevel.Array(ak.operations.fill_none(out, np.nan, axis=-1))
 
         if axis is None:
             if not keepdims:
                 out = out[(0,) * out.ndim]
@@ -232,33 +233,31 @@
             if not keepdims:
                 posaxis = maybe_posaxis(out.layout, axis, 1)
                 out = out[(slice(None, None),) * posaxis + (0,)]
 
         return out
 
 
-@ak._connect.numpy.implements("var")
-def _nep_18_impl_var(
+@ak._connect.numpy.implements("mean")
+def _nep_18_impl_mean(
     a,
     axis=None,
     dtype=unsupported,
     out=unsupported,
-    ddof=0,
     keepdims=False,
     *,
     where=unsupported,
 ):
-    return var(a, axis=axis, keepdims=keepdims, ddof=ddof)
+    return mean(a, axis=axis, keepdims=keepdims)
 
 
-@ak._connect.numpy.implements("nanvar")
-def _nep_18_impl_nanvar(
+@ak._connect.numpy.implements("nanmean")
+def _nep_18_impl_nanmean(
     a,
     axis=None,
     dtype=unsupported,
     out=unsupported,
-    ddof=0,
     keepdims=False,
     *,
     where=unsupported,
 ):
-    return nanvar(a, axis=axis, keepdims=keepdims, ddof=ddof)
+    return nanmean(a, axis=axis, keepdims=keepdims)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_where.py` & `awkward-2.1.2/src/awkward/operations/ak_where.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,17 +45,15 @@
         with ak._errors.OperationErrorContext(
             "ak.where",
             {"condition": condition, "mergebool": mergebool, "highlevel": highlevel},
         ):
             return _impl1(condition, mergebool, highlevel, behavior)
 
     elif len(args) == 1:
-        raise ak._errors.wrap_error(
-            ValueError("either both or neither of x and y should be given")
-        )
+        raise ValueError("either both or neither of x and y should be given")
 
     elif len(args) == 2:
         x, y = args
         with ak._errors.OperationErrorContext(
             "ak.where",
             {
                 "condition": condition,
@@ -64,19 +62,17 @@
                 "mergebool": mergebool,
                 "highlevel": highlevel,
             },
         ):
             return _impl3(condition, x, y, mergebool, highlevel, behavior)
 
     else:
-        raise ak._errors.wrap_error(
-            TypeError(
-                "where() takes from 1 to 3 positional arguments but {} were "
-                "given".format(len(args) + 1)
-            )
+        raise TypeError(
+            "where() takes from 1 to 3 positional arguments but {} were "
+            "given".format(len(args) + 1)
         )
 
 
 def _impl1(condition, mergebool, highlevel, behavior):
     akcondition = ak.operations.to_layout(
         condition, allow_record=False, allow_other=False
     )
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_with_field.py` & `awkward-2.1.2/src/awkward/operations/ak_with_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,19 +52,17 @@
         where is None
         or isinstance(where, str)
         or (
             is_non_string_like_sequence(where)
             and all(isinstance(x, str) for x in where)
         )
     ):
-        raise ak._errors.wrap_error(
-            TypeError(
-                "New fields may only be assigned by field name(s) "
-                "or as a new integer slot by passing None for 'where'"
-            )
+        raise TypeError(
+            "New fields may only be assigned by field name(s) "
+            "or as a new integer slot by passing None for 'where'"
         )
 
     if is_non_string_like_sequence(where) and len(where) > 1:
         return _impl(
             base,
             _impl(
                 base[where[0]],
@@ -82,17 +80,15 @@
         if is_non_string_like_sequence(where):
             where = where[0]
 
         behavior = behavior_of(base, what, behavior=behavior)
         base = ak.operations.to_layout(base, allow_record=True, allow_other=False)
 
         if len(base.fields) == 0:
-            raise ak._errors.wrap_error(
-                ValueError("no tuples or records in array; cannot add a new field")
-            )
+            raise ValueError("no tuples or records in array; cannot add a new field")
 
         what = ak.operations.to_layout(what, allow_record=True, allow_other=True)
 
         keys = copy.copy(base.fields)
         if where in base.fields:
             keys.remove(where)
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_with_name.py` & `awkward-2.1.2/src/awkward/operations/ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_with_parameter.py` & `awkward-2.1.2/src/awkward/operations/ak_with_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_without_field.py` & `awkward-2.1.2/src/awkward/operations/ak_without_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,16 @@
         return _impl(array, where, highlevel, behavior)
 
 
 def _impl(base, where, highlevel, behavior):
     if isinstance(where, str):
         where = [where]
     elif not (isinstance(where, Sequence) and all(isinstance(x, str) for x in where)):
-        raise ak._errors.wrap_error(
-            TypeError(
-                "Field names must be given as a single string, or a sequence of strings"
-            )
+        raise TypeError(
+            "Field names must be given as a single string, or a sequence of strings"
         )
 
     behavior = behavior_of(base, behavior=behavior)
     base = ak.operations.to_layout(base, allow_record=True, allow_other=False)
 
     def action(layout, depth_context, **kwargs):
         if isinstance(layout, ak.contents.RecordArray):
```

### Comparing `awkward-2.1.1/src/awkward/operations/ak_without_parameters.py` & `awkward-2.1.2/src/awkward/operations/ak_without_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_zeros_like.py` & `awkward-2.1.2/src/awkward/operations/ak_zeros_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/operations/ak_zip.py` & `awkward-2.1.2/src/awkward/operations/ak_zip.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,17 +163,15 @@
     with_name,
     right_broadcast,
     optiontype_outside_record,
     highlevel,
     behavior,
 ):
     if depth_limit is not None and depth_limit <= 0:
-        raise ak._errors.wrap_error(
-            ValueError("depth_limit must be None or at least 1")
-        )
+        raise ValueError("depth_limit must be None or at least 1")
 
     if isinstance(arrays, dict):
         behavior = behavior_of(*arrays.values(), behavior=behavior)
         recordlookup = []
         layouts = []
         num_scalars = 0
         for n, x in arrays.items():
@@ -213,24 +211,21 @@
         if parameters is None:
             parameters = {}
         else:
             parameters = dict(parameters)
         parameters["__record__"] = with_name
 
     def action(inputs, depth, **ignore):
-        if depth_limit == depth or (
-            depth_limit is None
-            and all(
-                x.purelist_depth == 1
-                or (
-                    x.purelist_depth == 2
-                    and x.purelist_parameter("__array__") in ("string", "bytestring")
-                )
-                for x in inputs
+        if depth_limit == depth or all(
+            x.purelist_depth == 1
+            or (
+                x.purelist_depth == 2
+                and x.purelist_parameter("__array__") in ("string", "bytestring")
             )
+            for x in inputs
         ):
             # If we want to zip after option types at this depth
             if optiontype_outside_record and any(x.is_option for x in inputs):
                 return None
 
             return (
                 ak.contents.RecordArray(inputs, recordlookup, parameters=parameters),
```

### Comparing `awkward-2.1.1/src/awkward/types/__init__.py` & `awkward-2.1.2/src/awkward/types/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/types/_awkward_datashape_parser.py` & `awkward-2.1.2/src/awkward/types/_awkward_datashape_parser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/src/awkward/types/arraytype.py` & `awkward-2.1.2/src/awkward/types/arraytype.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
+from __future__ import annotations
+
 import sys
 
 import awkward as ak
 from awkward._nplikes.shape import unknown_length
 from awkward._regularize import is_integer
 
 
 class ArrayType:
     def __init__(self, content, length):
         if not isinstance(content, ak.types.Type):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} all 'contents' must be Type subclasses, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} all 'contents' must be Type subclasses, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
         if not ((is_integer(length) and length >= 0) or length is unknown_length):
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "{} 'length' must be a non-negative integer or unknown length, not {}".format(
-                        type(self).__name__, repr(length)
-                    )
+            raise ValueError(
+                "{} 'length' must be a non-negative integer or unknown length, not {}".format(
+                    type(self).__name__, repr(length)
                 )
             )
         self._content = content
         self._length = length
 
     @property
     def content(self):
@@ -44,16 +42,19 @@
     def _str(self, indent, compact):
         return [f"{self._length} * ", *self._content._str(indent, compact)]
 
     def __repr__(self):
         args = [repr(self._content), repr(self._length)]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
-    def __eq__(self, other):
-        if isinstance(other, ArrayType):
-            return (
+    def is_equal_to(self, other, *, all_parameters: bool = False) -> bool:
+        return (
+            isinstance(other, type(self))
+            and (
                 other._length is unknown_length
                 or self._length is unknown_length
                 or self._length == other._length
-            ) and self._content == other._content
-        else:
-            return False
+            )
+            and self._content.is_equal_to(other._content, all_parameters=all_parameters)
+        )
+
+    __eq__ = is_equal_to
```

### Comparing `awkward-2.1.1/src/awkward/types/listtype.py` & `awkward-2.1.2/src/awkward/types/listtype.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
-import awkward as ak
-from awkward.forms.form import _type_parameters_equal
+from awkward._parameters import parameters_are_equal, type_parameters_equal
+from awkward._typing import final
 from awkward.types.type import Type
-from awkward.typing import final
 
 
 @final
 class ListType(Type):
     def __init__(self, content, *, parameters=None, typestr=None):
         if not isinstance(content, Type):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'content' must be a Type subtype, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} 'content' must be a Type subtype, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
         if parameters is not None and not isinstance(parameters, dict):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'parameters' must be of type dict or None, not {}".format(
-                        type(self).__name__, repr(parameters)
-                    )
+            raise TypeError(
+                "{} 'parameters' must be of type dict or None, not {}".format(
+                    type(self).__name__, repr(parameters)
                 )
             )
         if typestr is not None and not isinstance(typestr, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'typestr' must be of type string or None, not {}".format(
-                        type(self).__name__, repr(typestr)
-                    )
+            raise TypeError(
+                "{} 'typestr' must be of type string or None, not {}".format(
+                    type(self).__name__, repr(typestr)
                 )
             )
         self._content = content
         self._parameters = parameters
         self._typestr = typestr
 
     @property
@@ -62,15 +55,16 @@
 
         return [self._str_categorical_begin(), *out] + [self._str_categorical_end()]
 
     def __repr__(self):
         args = [repr(self._content), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
-    def __eq__(self, other):
-        if isinstance(other, ListType):
-            return (
-                _type_parameters_equal(self._parameters, other._parameters)
-                and self._content == other._content
-            )
-        else:
-            return False
+    def _is_equal_to(self, other, all_parameters: bool):
+        compare_parameters = (
+            parameters_are_equal if all_parameters else type_parameters_equal
+        )
+        return (
+            isinstance(other, type(self))
+            and compare_parameters(self._parameters, other._parameters)
+            and self._content == other._content
+        )
```

### Comparing `awkward-2.1.1/src/awkward/types/numpytype.py` & `awkward-2.1.2/src/awkward/types/numpytype.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import json
 import re
 
-import awkward as ak
 from awkward._nplikes.numpylike import NumpyMetadata
-from awkward.forms.form import _type_parameters_equal
+from awkward._parameters import parameters_are_equal, type_parameters_equal
+from awkward._typing import final
 from awkward.types.type import Type
-from awkward.typing import final
 
 np = NumpyMetadata.instance()
 
 
 def is_primitive(primitive):
     if _primitive_to_dtype_datetime.match(primitive) is not None:
         return True
@@ -25,37 +24,33 @@
     if _primitive_to_dtype_datetime.match(primitive) is not None:
         return np.dtype(primitive)
     elif _primitive_to_dtype_timedelta.match(primitive) is not None:
         return np.dtype(primitive)
     else:
         out = _primitive_to_dtype_dict.get(primitive)
         if out is None:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "unrecognized primitive: {}. Must be one of\n\n    {}\n\nor a "
-                    "datetime64/timedelta64 with units (e.g. 'datetime64[15us]')".format(
-                        repr(primitive), ", ".join(_primitive_to_dtype_dict)
-                    )
+            raise TypeError(
+                "unrecognized primitive: {}. Must be one of\n\n    {}\n\nor a "
+                "datetime64/timedelta64 with units (e.g. 'datetime64[15us]')".format(
+                    repr(primitive), ", ".join(_primitive_to_dtype_dict)
                 )
             )
         return out
 
 
 def dtype_to_primitive(dtype):
     if dtype.kind.upper() == "M" and dtype == dtype.newbyteorder("="):
         return str(dtype)
     else:
         out = _dtype_to_primitive_dict.get(dtype)
         if out is None:
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "unsupported dtype: {}. Must be one of\n\n    {}\n\nor a "
-                    "datetime64/timedelta64 with units (e.g. 'datetime64[15us]')".format(
-                        repr(dtype), ", ".join(_primitive_to_dtype_dict)
-                    )
+            raise TypeError(
+                "unsupported dtype: {}. Must be one of\n\n    {}\n\nor a "
+                "datetime64/timedelta64 with units (e.g. 'datetime64[15us]')".format(
+                    repr(dtype), ", ".join(_primitive_to_dtype_dict)
                 )
             )
         return out
 
 
 _primitive_to_dtype_datetime = re.compile(
     r"datetime64\[(\s*-?[0-9]*)?(Y|M|W|D|h|m|s|ms|us|\u03bc|ns|ps|fs|as)\]"
@@ -95,27 +90,23 @@
 
 
 @final
 class NumpyType(Type):
     def __init__(self, primitive, *, parameters=None, typestr=None):
         primitive = dtype_to_primitive(primitive_to_dtype(primitive))
         if parameters is not None and not isinstance(parameters, dict):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'parameters' must be of type dict or None, not {}".format(
-                        type(self).__name__, repr(parameters)
-                    )
+            raise TypeError(
+                "{} 'parameters' must be of type dict or None, not {}".format(
+                    type(self).__name__, repr(parameters)
                 )
             )
         if typestr is not None and not isinstance(typestr, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'typestr' must be of type string or None, not {}".format(
-                        type(self).__name__, repr(typestr)
-                    )
+            raise TypeError(
+                "{} 'typestr' must be of type string or None, not {}".format(
+                    type(self).__name__, repr(typestr)
                 )
             )
         self._primitive = primitive
         self._parameters = parameters
         self._typestr = typestr
 
     @property
@@ -157,14 +148,16 @@
 
         return [self._str_categorical_begin(), *out] + [self._str_categorical_end()]
 
     def __repr__(self):
         args = [repr(self._primitive), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
-    def __eq__(self, other):
-        if isinstance(other, NumpyType):
-            return self._primitive == other._primitive and _type_parameters_equal(
-                self._parameters, other._parameters
-            )
-        else:
-            return False
+    def _is_equal_to(self, other, all_parameters: bool) -> bool:
+        compare_parameters = (
+            parameters_are_equal if all_parameters else type_parameters_equal
+        )
+        return (
+            isinstance(other, type(self))
+            and (self._primitive == other._primitive)
+            and compare_parameters(self._parameters, other._parameters)
+        )
```

### Comparing `awkward-2.1.1/src/awkward/types/optiontype.py` & `awkward-2.1.2/src/awkward/types/uniontype.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,125 +1,102 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
-import awkward as ak
-from awkward.forms.form import _type_parameters_equal
-from awkward.types.listtype import ListType
-from awkward.types.regulartype import RegularType
+from collections.abc import Iterable
+from itertools import permutations
+
+from awkward._parameters import parameters_are_equal, type_parameters_equal
+from awkward._typing import final
 from awkward.types.type import Type
-from awkward.types.uniontype import UnionType
-from awkward.typing import final
 
 
 @final
-class OptionType(Type):
-    def __init__(self, content, *, parameters=None, typestr=None):
-        if not isinstance(content, Type):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'content' must be a Type subclass, not {}".format(
+class UnionType(Type):
+    def __init__(self, contents, *, parameters=None, typestr=None):
+        if not isinstance(contents, Iterable):
+            raise TypeError(
+                "{} 'contents' must be iterable, not {}".format(
+                    type(self).__name__, repr(contents)
+                )
+            )
+        if not isinstance(contents, list):
+            contents = list(contents)
+        for content in contents:
+            if not isinstance(content, Type):
+                raise TypeError(
+                    "{} all 'contents' must be Type subclasses, not {}".format(
                         type(self).__name__, repr(content)
                     )
                 )
-            )
         if parameters is not None and not isinstance(parameters, dict):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'parameters' must be of type dict or None, not {}".format(
-                        type(self).__name__, repr(parameters)
-                    )
+            raise TypeError(
+                "{} 'parameters' must be of type dict or None, not {}".format(
+                    type(self).__name__, repr(parameters)
                 )
             )
         if typestr is not None and not isinstance(typestr, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'typestr' must be of type string or None, not {}".format(
-                        type(self).__name__, repr(typestr)
-                    )
+            raise TypeError(
+                "{} 'typestr' must be of type string or None, not {}".format(
+                    type(self).__name__, repr(typestr)
                 )
             )
-        self._content = content
+        self._contents = contents
         self._parameters = parameters
         self._typestr = typestr
 
     @property
-    def content(self):
-        return self._content
+    def contents(self):
+        return self._contents
 
     def _str(self, indent, compact):
-        head = []
-        tail = []
         if self._typestr is not None:
-            content_out = [self._typestr]
+            out = [self._typestr]
 
         else:
-            content_out = self._content._str(indent, compact)
-            params = self._str_parameters()
-            if params is None:
-                if isinstance(
-                    self._content, (RegularType, ListType)
-                ) and self._content.parameter("__array__") not in (
-                    "string",
-                    "bytestring",
-                    "char",
-                    "byte",
-                ):
-                    head = ["option["]
-                    tail = ["]"]
+            if compact:
+                pre, post = "", ""
+            else:
+                pre, post = "\n" + indent + "    ", "\n" + indent
+
+            children = []
+            for i, x in enumerate(self._contents):
+                if i + 1 < len(self._contents):
+                    if compact:
+                        y = [*x._str(indent, compact), ", "]
+                    else:
+                        y = [*x._str(indent + "    ", compact), ",\n", indent, "    "]
                 else:
-                    head = ["?"]
+                    if compact:
+                        y = x._str(indent, compact)
+                    else:
+                        y = x._str(indent + "    ", compact)
+                children.append(y)
+
+            flat_children = [y for x in children for y in x]
+            params = self._str_parameters()
 
+            if params is None:
+                out = ["union[", pre, *flat_children] + [post, "]"]
             else:
-                head = ["option["]
-                tail = [f", {params}]"]
+                out = ["union[", pre, *flat_children] + [", ", post, params, "]"]
 
-        return (
-            [*head, self._str_categorical_begin(), *content_out]
-            + [self._str_categorical_end()]
-            + tail
-        )
+        return [self._str_categorical_begin(), *out] + [self._str_categorical_end()]
 
     def __repr__(self):
-        args = [repr(self._content), *self._repr_args()]
+        args = [repr(self._contents), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
-    def __eq__(self, other):
-        if isinstance(other, OptionType):
-            return (
-                _type_parameters_equal(self._parameters, other._parameters)
-                and self._content == other._content
-            )
-        else:
-            return False
-
-    def simplify_option_union(self):
-        if isinstance(self._content, UnionType):
-            contents = []
-            for content in self._content.contents:
-                if isinstance(content, OptionType):
-                    typestr = (
-                        content._typestr if self._typestr is None else self._typestr
-                    )
-                    contents.append(
-                        OptionType(
-                            content.content,
-                            parameters=ak.forms.form._parameters_union(
-                                self._parameters, content._parameters
-                            ),
-                            typestr=typestr,
-                        )
-                    )
-
-                else:
-                    contents.append(
-                        OptionType(
-                            content, parameters=self._parameters, typestr=self._typestr
-                        )
-                    )
-
-            return UnionType(
-                contents,
-                parameters=self._content.parameters,
-                typestr=self._content.typestr,
+    def _is_equal_to(self, other, all_parameters: bool):
+        compare_parameters = (
+            parameters_are_equal if all_parameters else type_parameters_equal
+        )
+        return (
+            isinstance(other, type(self))
+            and compare_parameters(self._parameters, other._parameters)
+            and len(self._contents) == len(other._contents)
+            and any(
+                all(
+                    this._is_equal_to(that, all_parameters)
+                    for this, that in zip(self._contents, contents)
+                )
+                for contents in permutations(other._contents)
             )
-
-        else:
-            return self
+        )
```

### Comparing `awkward-2.1.1/src/awkward/types/recordtype.py` & `awkward-2.1.2/src/awkward/types/recordtype.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,63 +1,54 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
 import json
 from collections.abc import Iterable
+from itertools import permutations
 
 import awkward as ak
 import awkward._prettyprint
-from awkward.forms.form import _type_parameters_equal
+from awkward._parameters import parameters_are_equal, type_parameters_equal
+from awkward._typing import final
 from awkward.types.type import Type
-from awkward.typing import final
 
 
 @final
 class RecordType(Type):
     def __init__(self, contents, fields, *, parameters=None, typestr=None):
         if not isinstance(contents, Iterable):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'contents' must be iterable, not {}".format(
-                        type(self).__name__, repr(contents)
-                    )
+            raise TypeError(
+                "{} 'contents' must be iterable, not {}".format(
+                    type(self).__name__, repr(contents)
                 )
             )
         if not isinstance(contents, list):
             contents = list(contents)
         for content in contents:
             if not isinstance(content, Type):
-                raise ak._errors.wrap_error(
-                    TypeError(
-                        "{} all 'contents' must be Type subclasses, not {}".format(
-                            type(self).__name__, repr(content)
-                        )
+                raise TypeError(
+                    "{} all 'contents' must be Type subclasses, not {}".format(
+                        type(self).__name__, repr(content)
                     )
                 )
         if fields is not None and not isinstance(fields, Iterable):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'fields' must be iterable, not {}".format(
-                        type(self).__name__, repr(contents)
-                    )
+            raise TypeError(
+                "{} 'fields' must be iterable, not {}".format(
+                    type(self).__name__, repr(contents)
                 )
             )
         if parameters is not None and not isinstance(parameters, dict):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'parameters' must be of type dict or None, not {}".format(
-                        type(self).__name__, repr(parameters)
-                    )
+            raise TypeError(
+                "{} 'parameters' must be of type dict or None, not {}".format(
+                    type(self).__name__, repr(parameters)
                 )
             )
         if typestr is not None and not isinstance(typestr, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'typestr' must be of type string or None, not {}".format(
-                        type(self).__name__, repr(typestr)
-                    )
+            raise TypeError(
+                "{} 'typestr' must be of type string or None, not {}".format(
+                    type(self).__name__, repr(typestr)
                 )
             )
         self._contents = contents
         self._fields = fields
         self._parameters = parameters
         self._typestr = typestr
 
@@ -179,34 +170,46 @@
 
         return [self._str_categorical_begin(), *out] + [self._str_categorical_end()]
 
     def __repr__(self):
         args = [repr(self._contents), repr(self._fields), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
-    def __eq__(self, other):
-        if isinstance(other, RecordType):
-            if not _type_parameters_equal(self._parameters, other._parameters):
-                return False
-
-            if self._fields is None and other._fields is None:
-                return self._contents == other._contents
-
-            elif self._fields is not None and other._fields is not None:
-                if set(self._fields) != set(other._fields):
-                    return False
-                for field in self._fields:
-                    if self.content(field) != other.content(field):
-                        return False
+    def _is_equal_to(self, other, all_parameters: bool) -> bool:
+        if not isinstance(other, type(self)):
+            return False
 
-                return True
+        compare_parameters = (
+            parameters_are_equal if all_parameters else type_parameters_equal
+        )
+        if not compare_parameters(self._parameters, other._parameters):
+            return False
 
-            else:
+        # Both tuples
+        if self.is_tuple and other.is_tuple:
+            return all(
+                this._is_equal_to(that, all_parameters)
+                for this, that in zip(self._contents, other._contents)
+            )
+        # Both records
+        elif not (self.is_tuple or other.is_tuple):
+            if set(self._fields) != set(other._fields):
                 return False
 
+            self_contents = [self.content(f) for f in self._fields]
+            other_contents = [other.content(f) for f in other._fields]
+
+            return any(
+                all(
+                    this._is_equal_to(that, all_parameters)
+                    for this, that in zip(self_contents, contents)
+                )
+                for contents in permutations(other_contents)
+            )
+        # Mixed
         else:
             return False
 
     def index_to_field(self, index):
         return ak.forms.RecordForm.index_to_field(self, index)
 
     def field_to_index(self, field):
```

### Comparing `awkward-2.1.1/src/awkward/types/regulartype.py` & `awkward-2.1.2/src/awkward/types/regulartype.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,40 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
-import awkward as ak
 from awkward._nplikes.shape import unknown_length
+from awkward._parameters import parameters_are_equal, type_parameters_equal
 from awkward._regularize import is_integer
-from awkward.forms.form import _type_parameters_equal
+from awkward._typing import final
 from awkward.types.type import Type
-from awkward.typing import final
 
 
 @final
 class RegularType(Type):
     def __init__(self, content, size, *, parameters=None, typestr=None):
         if not isinstance(content, Type):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'content' must be a Type subtype, not {}".format(
-                        type(self).__name__, repr(content)
-                    )
+            raise TypeError(
+                "{} 'content' must be a Type subtype, not {}".format(
+                    type(self).__name__, repr(content)
                 )
             )
         if not (size is unknown_length or (is_integer(size) and size >= 0)):
-            raise ak._errors.wrap_error(
-                ValueError(
-                    "{} 'size' must be a non-negative int or None, not {}".format(
-                        type(self).__name__, repr(size)
-                    )
+            raise ValueError(
+                "{} 'size' must be a non-negative int or None, not {}".format(
+                    type(self).__name__, repr(size)
                 )
             )
         if parameters is not None and not isinstance(parameters, dict):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'parameters' must be of type dict or None, not {}".format(
-                        type(self).__name__, repr(parameters)
-                    )
+            raise TypeError(
+                "{} 'parameters' must be of type dict or None, not {}".format(
+                    type(self).__name__, repr(parameters)
                 )
             )
         if typestr is not None and not isinstance(typestr, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'typestr' must be of type string or None, not {}".format(
-                        type(self).__name__, repr(typestr)
-                    )
+            raise TypeError(
+                "{} 'typestr' must be of type string or None, not {}".format(
+                    type(self).__name__, repr(typestr)
                 )
             )
         self._content = content
         self._size = size
         self._parameters = parameters
         self._typestr = typestr
 
@@ -80,16 +71,17 @@
 
         return [self._str_categorical_begin(), *out] + [self._str_categorical_end()]
 
     def __repr__(self):
         args = [repr(self._content), repr(self._size), *self._repr_args()]
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
-    def __eq__(self, other):
-        if isinstance(other, RegularType):
-            return (
-                self._size == other._size
-                and _type_parameters_equal(self._parameters, other._parameters)
-                and self._content == other._content
-            )
-        else:
-            return False
+    def _is_equal_to(self, other, all_parameters: bool) -> bool:
+        compare_parameters = (
+            parameters_are_equal if all_parameters else type_parameters_equal
+        )
+        return (
+            isinstance(other, type(self))
+            and compare_parameters(self._parameters, other._parameters)
+            and (self._size == other._size)
+            and self._content._is_equal_to(other._content, all_parameters)
+        )
```

### Comparing `awkward-2.1.1/src/awkward/types/type.py` & `awkward-2.1.2/src/awkward/types/type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
+from __future__ import annotations
 
 import json
 import sys
 
 import awkward as ak
 from awkward._nplikes.numpylike import NumpyMetadata
 from awkward.types._awkward_datashape_parser import Lark_StandAlone, Transformer
@@ -66,14 +67,22 @@
             out.append("parameters=" + repr(self._parameters))
 
         if self._typestr is not None:
             out.append("typestr=" + repr(self._typestr))
 
         return out
 
+    def is_equal_to(self, other, *, all_parameters: bool = False) -> bool:
+        return self._is_equal_to(other, all_parameters)
+
+    __eq__ = is_equal_to
+
+    def _is_equal_to(self, other, all_parameters: bool) -> bool:
+        raise ak._errors.wrap_error(NotImplementedError)
+
 
 class _DataShapeTransformer(Transformer):
     @staticmethod
     def _parameters(args, i):
         if i < len(args):
             return args[i]
         else:
@@ -314,15 +323,13 @@
 
     if highlevel:
         if isinstance(out, RegularType):
             return ArrayType(out.content, out.size)
         elif isinstance(out, RecordType):
             return out
         else:
-            raise ak._errors.wrap_error(
-                ValueError(
-                    f"type {type(out).__name__!r} is not compatible with highlevel=True"
-                )
+            raise ValueError(
+                f"type {type(out).__name__!r} is not compatible with highlevel=True"
             )
 
     else:
         return out
```

### Comparing `awkward-2.1.1/src/awkward/types/unknowntype.py` & `awkward-2.1.2/src/awkward/types/unknowntype.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,32 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward-1.0/blob/main/LICENSE
 
-import awkward as ak
 from awkward._errors import deprecate
-from awkward.forms.form import _type_parameters_equal
+from awkward._parameters import parameters_are_equal, type_parameters_equal
+from awkward._typing import final
 from awkward.types.type import Type
-from awkward.typing import final
 
 
 @final
 class UnknownType(Type):
     def __init__(self, *, parameters=None, typestr=None):
         if parameters is not None:
             deprecate(
                 f"{type(self).__name__} cannot contain parameters", version="2.2.0"
             )
         if parameters is not None and not isinstance(parameters, dict):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'parameters' must be of type dict or None, not {}".format(
-                        type(self).__name__, repr(parameters)
-                    )
+            raise TypeError(
+                "{} 'parameters' must be of type dict or None, not {}".format(
+                    type(self).__name__, repr(parameters)
                 )
             )
         if typestr is not None and not isinstance(typestr, str):
-            raise ak._errors.wrap_error(
-                TypeError(
-                    "{} 'typestr' must be of type string or None, not {}".format(
-                        type(self).__name__, repr(typestr)
-                    )
+            raise TypeError(
+                "{} 'typestr' must be of type string or None, not {}".format(
+                    type(self).__name__, repr(typestr)
                 )
             )
         self._parameters = parameters
         self._typestr = typestr
 
     def _str(self, indent, compact):
         if self._typestr is not None:
@@ -46,12 +41,14 @@
 
         return [self._str_categorical_begin(), *out] + [self._str_categorical_end()]
 
     def __repr__(self):
         args = self._repr_args()
         return "{}({})".format(type(self).__name__, ", ".join(args))
 
-    def __eq__(self, other):
-        if isinstance(other, UnknownType):
-            return _type_parameters_equal(self._parameters, other._parameters)
-        else:
-            return False
+    def _is_equal_to(self, other, all_parameters: bool):
+        compare_parameters = (
+            parameters_are_equal if all_parameters else type_parameters_equal
+        )
+        return isinstance(other, type(self)) and compare_parameters(
+            self._parameters, other._parameters
+        )
```

### Comparing `awkward-2.1.1/tests/test_0002_minimal_listarray.py` & `awkward-2.1.2/tests/test_0002_minimal_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0008_slices_and_getitem.py` & `awkward-2.1.2/tests/test_0008_slices_and_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0011_listarray.py` & `awkward-2.1.2/tests/test_0011_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0013_error_handling_struct.py` & `awkward-2.1.2/tests/test_0013_error_handling_struct.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0014_finish_up_getitem.py` & `awkward-2.1.2/tests/test_0014_finish_up_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0018_fromiter_fillable.py` & `awkward-2.1.2/tests/test_0018_fromiter_fillable.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0019_use_json_library.py` & `awkward-2.1.2/tests/test_0019_use_json_library.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0020_support_unsigned_indexes.py` & `awkward-2.1.2/tests/test_0020_support_unsigned_indexes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0021_emptyarray.py` & `awkward-2.1.2/tests/test_0021_emptyarray.py`

 * *Files 11% similar despite different names*

```diff
@@ -141,42 +141,32 @@
     assert a[2].to_list() == [[], [], []]
 
     assert a[2, 1].to_list() == []
     with pytest.raises(IndexError) as excinfo:
         a[2, 1, 0]
     assert "index out of range while attempting to get index 0" in str(excinfo.value)
     assert a[2, 1][()].to_list() == []
-    with pytest.raises(IndexError) as excinfo:
+    with pytest.raises(IndexError, match=r"array is empty") as excinfo:
         a[2, 1][0]
-    assert (
-        "<Array [] type='0 * unknown'>\n\nwith\n\n    0\n\nat inner EmptyArray of length 0, using sub-slice 0.\n\nError details: array is empty."
-        in str(excinfo.value)
-    )
     assert a[2, 1][100:200].to_list() == []
     assert a[2, 1, 100:200].to_list() == []
     assert a[2, 1][np.array([], dtype=np.int64)].to_list() == []
     assert a[2, 1, np.array([], dtype=np.int64)].to_list() == []
-    with pytest.raises(IndexError) as excinfo:
+    with pytest.raises(
+        IndexError, match=r"index out of range while attempting to get index 0"
+    ) as excinfo:
         a[2, 1, np.array([0], dtype=np.int64)]
-    assert "index out of range while attempting to get index 0" in str(excinfo.value)
-    with pytest.raises(IndexError) as excinfo:
+    with pytest.raises(IndexError, match="array is empty") as excinfo:
         a[2, 1][100:200, 0]
-    assert (
-        "<Array [] type='0 * unknown'>\n\nwith\n\n    (100:200, 0)\n\nat inner EmptyArray of length 0, using sub-slice array(0).\n\nError details: array is empty."
-        in str(excinfo.value)
-    )
-    with pytest.raises(IndexError) as excinfo:
+    with pytest.raises(IndexError, match="array is empty") as excinfo:
         a[2, 1][100:200, 200:300]
-    assert (
-        "<Array [] type='0 * unknown'>\n\nwith\n\n    (100:200, 200:300)\n\nat inner EmptyArray of length 0, using sub-slice 200:300.\n\nError details: array is empty."
-        in str(excinfo.value)
-    )
 
     # FIXME: Failed: DID NOT RAISE <class 'IndexError'>
     # with pytest.raises(IndexError) as excinfo:
     #     a[2, 1][100:200, np.array([], dtype=np.int64)]
     # assert ", too many dimensions in slice" in str(excinfo.value)
 
     assert a[1:, 1:].to_list() == [[[]], [[], []]]
-    with pytest.raises(IndexError) as excinfo:
+    with pytest.raises(
+        IndexError, match=r"index out of range while attempting to get index 0"
+    ) as excinfo:
         a[1:, 1:, 0]
-    assert "index out of range while attempting to get index 0" in str(excinfo.value)
```

### Comparing `awkward-2.1.1/tests/test_0023_regular_array.py` & `awkward-2.1.2/tests/test_0023_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0024_use_regular_array.py` & `awkward-2.1.2/tests/test_0024_use_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0025_record_array.py` & `awkward-2.1.2/tests/test_0025_record_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0028_add_dressed_types.py` & `awkward-2.1.2/tests/test_0028_add_dressed_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0032_replace_dressedtype.py` & `awkward-2.1.2/tests/test_0032_replace_dressedtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0046_start_indexedarray.py` & `awkward-2.1.2/tests/test_0046_start_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0049_distinguish_record_and_recordarray_behaviors.py` & `awkward-2.1.2/tests/test_0049_distinguish_record_and_recordarray_behaviors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0057_introducing_forms.py` & `awkward-2.1.2/tests/test_0057_introducing_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0070_argmin_and_argmax.py` & `awkward-2.1.2/tests/test_0070_argmin_and_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0072_fillna_operation.py` & `awkward-2.1.2/tests/test_0072_fillna_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0074_argsort_and_sort.py` & `awkward-2.1.2/tests/test_0074_argsort_and_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0077_zip_operation.py` & `awkward-2.1.2/tests/test_0077_zip_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0078_argcross_and_cross.py` & `awkward-2.1.2/tests/test_0078_argcross_and_cross.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0079_argchoose_and_choose.py` & `awkward-2.1.2/tests/test_0079_argchoose_and_choose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0080_flatpandas_multiindex_rows_and_columns.py` & `awkward-2.1.2/tests/test_0080_flatpandas_multiindex_rows_and_columns.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0084_start_unionarray.py` & `awkward-2.1.2/tests/test_0084_start_unionarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0086_nep13_ufunc.py` & `awkward-2.1.2/tests/test_0086_nep13_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0089_numpy_functions.py` & `awkward-2.1.2/tests/test_0089_numpy_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0093_simplify_uniontypes_and_optiontypes.py` & `awkward-2.1.2/tests/test_0093_simplify_uniontypes_and_optiontypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0107_assign_fields_to_records.py` & `awkward-2.1.2/tests/test_0107_assign_fields_to_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0111_jagged_and_masked_getitem.py` & `awkward-2.1.2/tests/test_0111_jagged_and_masked_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0115_generic_reducer_operation.py` & `awkward-2.1.2/tests/test_0115_generic_reducer_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0118_numba_cpointers.py` & `awkward-2.1.2/tests/test_0118_numba_cpointers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0119_numexpr_and_broadcast_arrays.py` & `awkward-2.1.2/tests/test_0119_numexpr_and_broadcast_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0124_strings_in_numba.py` & `awkward-2.1.2/tests/test_0124_strings_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0127_tomask_operation.py` & `awkward-2.1.2/tests/test_0127_tomask_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0127b_tomask_operation_numba.py` & `awkward-2.1.2/tests/test_0127b_tomask_operation_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0138_emptyarray_type.py` & `awkward-2.1.2/tests/test_0138_emptyarray_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0150_flatten.py` & `awkward-2.1.2/tests/test_0150_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0163_negative_axis_wrap.py` & `awkward-2.1.2/tests/test_0163_negative_axis_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0166_0167_0170_random_issues.py` & `awkward-2.1.2/tests/test_0166_0167_0170_random_issues.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0173_astype_operation.py` & `awkward-2.1.2/tests/test_0173_astype_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0184_concatenate_operation.py` & `awkward-2.1.2/tests/test_0184_concatenate_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0193_is_none_axis_parameter.py` & `awkward-2.1.2/tests/test_0193_is_none_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0198_tutorial_documentation_1.py` & `awkward-2.1.2/tests/test_0198_tutorial_documentation_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0222_count_with_axis0.py` & `awkward-2.1.2/tests/test_0222_count_with_axis0.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0224_arrow_to_awkward.py` & `awkward-2.1.2/tests/test_0224_arrow_to_awkward.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0264_reduce_last_empty.py` & `awkward-2.1.2/tests/test_0264_reduce_last_empty.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0273_path_for_with_field.py` & `awkward-2.1.2/tests/test_0273_path_for_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0286_broadcast_single_value_with_field.py` & `awkward-2.1.2/tests/test_0286_broadcast_single_value_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0290_bug_fixes_for_hats.py` & `awkward-2.1.2/tests/test_0290_bug_fixes_for_hats.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0315_integerindex.py` & `awkward-2.1.2/tests/test_0315_integerindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0331_pandas_indexedarray.py` & `awkward-2.1.2/tests/test_0331_pandas_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0334_fully_broadcastable_where.py` & `awkward-2.1.2/tests/test_0334_fully_broadcastable_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0339_highlevel_sorting_function.py` & `awkward-2.1.2/tests/test_0339_highlevel_sorting_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0348_form_keys.py` & `awkward-2.1.2/tests/test_0348_form_keys.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0355_mixins.py` & `awkward-2.1.2/tests/test_0355_mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0395_complex_type_arrays.py` & `awkward-2.1.2/tests/test_0395_complex_type_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0395_fix_numba_indexedarray.py` & `awkward-2.1.2/tests/test_0395_fix_numba_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0397_arrays_as_constants_in_numba.py` & `awkward-2.1.2/tests/test_0397_arrays_as_constants_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0401_add_categorical_type_for_arrow_dictionary.py` & `awkward-2.1.2/tests/test_0401_add_categorical_type_for_arrow_dictionary.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0404_array_validity_check.py` & `awkward-2.1.2/tests/test_0404_array_validity_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0410_fix_argminmax_positions_for_missing_values.py` & `awkward-2.1.2/tests/test_0410_fix_argminmax_positions_for_missing_values.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0437_stream_of_many_json_files.py` & `awkward-2.1.2/tests/test_0437_stream_of_many_json_files.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0447_preserve_regularness_in_reduce.py` & `awkward-2.1.2/tests/test_0447_preserve_regularness_in_reduce.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0449_merge_many_arrays_in_one_pass.py` & `awkward-2.1.2/tests/test_0449_merge_many_arrays_in_one_pass.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0493_zeros_ones_full_like.py` & `awkward-2.1.2/tests/test_0493_zeros_ones_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0496_provide_local_index.py` & `awkward-2.1.2/tests/test_0496_provide_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0499_getitem_indexedarray_bug.py` & `awkward-2.1.2/tests/test_0499_getitem_indexedarray_bug.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0504_block_ufuncs_for_strings.py` & `awkward-2.1.2/tests/test_0504_block_ufuncs_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0511_copy_and_deepcopy.py` & `awkward-2.1.2/tests/test_0511_copy_and_deepcopy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py` & `awkward-2.1.2/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0549_numba_array_asarray.py` & `awkward-2.1.2/tests/test_0549_numba_array_asarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0557_min_max_initial_argument.py` & `awkward-2.1.2/tests/test_0557_min_max_initial_argument.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0559_fix_booleans_in_numba.py` & `awkward-2.1.2/tests/test_0559_fix_booleans_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0572_numba_array_ndim.py` & `awkward-2.1.2/tests/test_0572_numba_array_ndim.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0582_propagate_context_in_broadcast_and_apply.py` & `awkward-2.1.2/tests/test_0582_propagate_context_in_broadcast_and_apply.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0583_implement_unflatten_function.py` & `awkward-2.1.2/tests/test_0583_implement_unflatten_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0590_allow_regulararray_size_zero.py` & `awkward-2.1.2/tests/test_0590_allow_regulararray_size_zero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py` & `awkward-2.1.2/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0652_tests_of_complex_numbers.py` & `awkward-2.1.2/tests/test_0652_tests_of_complex_numbers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0674_categorical_validation.py` & `awkward-2.1.2/tests/test_0674_categorical_validation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0713_getitem_field_should_simplify_optiontype.py` & `awkward-2.1.2/tests/test_0713_getitem_field_should_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py` & `awkward-2.1.2/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0730_unflatten_axis_parameter.py` & `awkward-2.1.2/tests/test_0730_unflatten_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0733_run_lengths.py` & `awkward-2.1.2/tests/test_0733_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0736_implement_argsort_for_strings.py` & `awkward-2.1.2/tests/test_0736_implement_argsort_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0766_prevent_combinations_of_characters.py` & `awkward-2.1.2/tests/test_0766_prevent_combinations_of_characters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0773_typeparser.py` & `awkward-2.1.2/tests/test_0773_typeparser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0788_indexedarray_carrying_recordarray_parameters.py` & `awkward-2.1.2/tests/test_0788_indexedarray_carrying_recordarray_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0794_ak_cartesian_on_empty_array.py` & `awkward-2.1.2/tests/test_0794_ak_cartesian_on_empty_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0803_argsort_fix_type.py` & `awkward-2.1.2/tests/test_0803_argsort_fix_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0806_empty_lists_cartesian_fix.py` & `awkward-2.1.2/tests/test_0806_empty_lists_cartesian_fix.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0813_full_like_dtype_arg.py` & `awkward-2.1.2/tests/test_0813_full_like_dtype_arg.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0815_broadcast_union_types_to_all_possibilities.py` & `awkward-2.1.2/tests/test_0815_broadcast_union_types_to_all_possibilities.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0828_arrow_datatype_null.py` & `awkward-2.1.2/tests/test_0828_arrow_datatype_null.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0835_datetime_type.py` & `awkward-2.1.2/tests/test_0835_datetime_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0835_datetime_type_pandas.py` & `awkward-2.1.2/tests/test_0835_datetime_type_pandas.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0835_datetime_type_pyarrow.py` & `awkward-2.1.2/tests/test_0835_datetime_type_pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0850_argsort_mask_array.py` & `awkward-2.1.2/tests/test_0850_argsort_mask_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0866_getitem_field_and_flatten_unions.py` & `awkward-2.1.2/tests/test_0866_getitem_field_and_flatten_unions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0875_arrow_null_type.py` & `awkward-2.1.2/tests/test_0875_arrow_null_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0879_non_primitive_with_field.py` & `awkward-2.1.2/tests/test_0879_non_primitive_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0884_index_and_identifier_refactoring.py` & `awkward-2.1.2/tests/test_0884_index_and_identifier_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0889_ptp.py` & `awkward-2.1.2/tests/test_0889_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0896_content_classes_refactoring.py` & `awkward-2.1.2/tests/test_0896_content_classes_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0898_unzip_heterogeneous_records.py` & `awkward-2.1.2/tests/test_0898_unzip_heterogeneous_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0905_leading_zeros_in_unflatten.py` & `awkward-2.1.2/tests/test_0905_leading_zeros_in_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0906_arrow_fixed_size_list_type.py` & `awkward-2.1.2/tests/test_0906_arrow_fixed_size_list_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0910_unflatten_counts_relation.py` & `awkward-2.1.2/tests/test_0910_unflatten_counts_relation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0912_packed.py` & `awkward-2.1.2/tests/test_0912_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0914_types_and_forms.py` & `awkward-2.1.2/tests/test_0914_types_and_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0916_datetime_values_astype.py` & `awkward-2.1.2/tests/test_0916_datetime_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0927_numpy_array_nbytes.py` & `awkward-2.1.2/tests/test_0927_numpy_array_nbytes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0930_bug_in_unionarray_purelist_parameter.py` & `awkward-2.1.2/tests/test_0930_bug_in_unionarray_purelist_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0945_argsort_sort_nan_array.py` & `awkward-2.1.2/tests/test_0945_argsort_sort_nan_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0958_new_forms_must_accept_old_form_json.py` & `awkward-2.1.2/tests/test_0958_new_forms_must_accept_old_form_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0959__getitem_array_implementation.py` & `awkward-2.1.2/tests/test_0959__getitem_array_implementation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0975_mask_multidimensional_numpy_array.py` & `awkward-2.1.2/tests/test_0975_mask_multidimensional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0979_where_multidimentional_numpy_array.py` & `awkward-2.1.2/tests/test_0979_where_multidimentional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0982_missing_case_in_nonlocal_reducers.py` & `awkward-2.1.2/tests/test_0982_missing_case_in_nonlocal_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0984_ravel.py` & `awkward-2.1.2/tests/test_0984_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_0992_correct_ptp_unmasking.py` & `awkward-2.1.2/tests/test_0992_correct_ptp_unmasking.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py` & `awkward-2.1.2/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1017_numpyarray_broadcast.py` & `awkward-2.1.2/tests/test_1017_numpyarray_broadcast.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1030_mixin_class_name.py` & `awkward-2.1.2/tests/test_1030_mixin_class_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1031_start_getitem_next.py` & `awkward-2.1.2/tests/test_1031_start_getitem_next.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1031b_start_getitem_next_specialized.py` & `awkward-2.1.2/tests/test_1031b_start_getitem_next_specialized.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1049_concatenate_single_array.py` & `awkward-2.1.2/tests/test_1049_concatenate_single_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1055_fill_none_numpy_dimension.py` & `awkward-2.1.2/tests/test_1055_fill_none_numpy_dimension.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1059_localindex.py` & `awkward-2.1.2/tests/test_1059_localindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1066_to_numpy_masked_structured_array.py` & `awkward-2.1.2/tests/test_1066_to_numpy_masked_structured_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1071_mask_identity_false_should_not_return_option_type.py` & `awkward-2.1.2/tests/test_1071_mask_identity_false_should_not_return_option_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1072_sort.py` & `awkward-2.1.2/tests/test_1072_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1074_combinations.py` & `awkward-2.1.2/tests/test_1074_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1075_validityerror.py` & `awkward-2.1.2/tests/test_1075_validityerror.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1110_type_tracer_1.py` & `awkward-2.1.2/tests/test_1110_type_tracer_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1116_project_maskedarrays.py` & `awkward-2.1.2/tests/test_1116_project_maskedarrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1125_to_arrow_from_arrow.py` & `awkward-2.1.2/tests/test_1125_to_arrow_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1132_utility_methods_for_highlevel_functions.py` & `awkward-2.1.2/tests/test_1132_utility_methods_for_highlevel_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1134_from_buffers_to_buffers.py` & `awkward-2.1.2/tests/test_1134_from_buffers_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1135_rpad_operation.py` & `awkward-2.1.2/tests/test_1135_rpad_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1136_regulararray_zeros_in_shape.py` & `awkward-2.1.2/tests/test_1136_regulararray_zeros_in_shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1137_num.py` & `awkward-2.1.2/tests/test_1137_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1142_numbers_to_type.py` & `awkward-2.1.2/tests/test_1142_numbers_to_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1149_datetime_sort.py` & `awkward-2.1.2/tests/test_1149_datetime_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1154_arrow_tables_should_preserve_parameters.py` & `awkward-2.1.2/tests/test_1154_arrow_tables_should_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1162_ak_from_json_schema.py` & `awkward-2.1.2/tests/test_1162_ak_from_json_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1183_bugs_found_by_dask_project_2.py` & `awkward-2.1.2/tests/test_1183_bugs_found_by_dask_project_2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1189_fix_singletons_for_non_optional_data.py` & `awkward-2.1.2/tests/test_1189_fix_singletons_for_non_optional_data.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1192_iterables_in___array_function__.py` & `awkward-2.1.2/tests/test_1192_iterables_in___array_function__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1193_is_none_nested_option.py` & `awkward-2.1.2/tests/test_1193_is_none_nested_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1233_ak_with_name.py` & `awkward-2.1.2/tests/test_1233_ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1240_v2_implementation_of_numba_1.py` & `awkward-2.1.2/tests/test_1240_v2_implementation_of_numba_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1259_simplify_optiontype.py` & `awkward-2.1.2/tests/test_1259_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1260_simplify_masked_option_types.py` & `awkward-2.1.2/tests/test_1260_simplify_masked_option_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1271_fix_4D_reducers.py` & `awkward-2.1.2/tests/test_1271_fix_4D_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1294_to_and_from_parquet.py` & `awkward-2.1.2/tests/test_1294_to_and_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py` & `awkward-2.1.2/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1300_awkward_to_cpp_converter_with_cling.py` & `awkward-2.1.2/tests/test_1300_awkward_to_cpp_converter_with_cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1300b_same_for_numba.py` & `awkward-2.1.2/tests/test_1300b_same_for_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1308_zip_after_option.py` & `awkward-2.1.2/tests/test_1308_zip_after_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1318_array_function_types.py` & `awkward-2.1.2/tests/test_1318_array_function_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1320_mask_identity_defaults.py` & `awkward-2.1.2/tests/test_1320_mask_identity_defaults.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1344_broadcast_arrays_depth_limit.py` & `awkward-2.1.2/tests/test_1344_broadcast_arrays_depth_limit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1345_avro_reader.py` & `awkward-2.1.2/tests/test_1345_avro_reader.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1351_is_tuple.py` & `awkward-2.1.2/tests/test_1351_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1374_to_rdataframe.py` & `awkward-2.1.2/tests/test_1374_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1377_ravel_string.py` & `awkward-2.1.2/tests/test_1377_ravel_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1379_reducers_with_axis_None_and_typetracers.py` & `awkward-2.1.2/tests/test_1379_reducers_with_axis_None_and_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1399_from_jax.py` & `awkward-2.1.2/tests/test_1399_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1399_to_jax.py` & `awkward-2.1.2/tests/test_1399_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1405_slicing_untested_cases.py` & `awkward-2.1.2/tests/test_1405_slicing_untested_cases.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1415_behaviour_forwarding.py` & `awkward-2.1.2/tests/test_1415_behaviour_forwarding.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1440_start_v2_to_parquet.py` & `awkward-2.1.2/tests/test_1440_start_v2_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1447_jax_autodiff_slices_ufuncs.py` & `awkward-2.1.2/tests/test_1447_jax_autodiff_slices_ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1449_v2_to_json_from_json_functions.py` & `awkward-2.1.2/tests/test_1449_v2_to_json_from_json_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1453_write_single_records_to_parquet.py` & `awkward-2.1.2/tests/test_1453_write_single_records_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1473_from_rdataframe.py` & `awkward-2.1.2/tests/test_1473_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1477_generator_entry_type_as_rvec.py` & `awkward-2.1.2/tests/test_1477_generator_entry_type_as_rvec.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1490_jax_reducers_combinations.py` & `awkward-2.1.2/tests/test_1490_jax_reducers_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1502_getitem_jagged_issue1406.py` & `awkward-2.1.2/tests/test_1502_getitem_jagged_issue1406.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1504_typetracer_like.py` & `awkward-2.1.2/tests/test_1504_typetracer_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1508_awkward_from_rdataframe.py` & `awkward-2.1.2/tests/test_1508_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1511_set_attribute.py` & `awkward-2.1.2/tests/test_1511_set_attribute.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1539_isnone_axis_check_issue1417.py` & `awkward-2.1.2/tests/test_1539_isnone_axis_check_issue1417.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1559_fix_ufuncs_records_1439.py` & `awkward-2.1.2/tests/test_1559_fix_ufuncs_records_1439.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1565_axis_wrap_if_negative_record.py` & `awkward-2.1.2/tests/test_1565_axis_wrap_if_negative_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1567_fix_longlong_in_Index.py` & `awkward-2.1.2/tests/test_1567_fix_longlong_in_Index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1568_fix_lengths_empty_regular_slices.py` & `awkward-2.1.2/tests/test_1568_fix_lengths_empty_regular_slices.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1586_concatenate_should_preserve_regulararray.py` & `awkward-2.1.2/tests/test_1586_concatenate_should_preserve_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1604_preserve_form_in_concatenate.py` & `awkward-2.1.2/tests/test_1604_preserve_form_in_concatenate.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1607_no_reducers_on_records.py` & `awkward-2.1.2/tests/test_1607_no_reducers_on_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1613_generator_tolayout_records.py` & `awkward-2.1.2/tests/test_1613_generator_tolayout_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1619_from_parquet_empty_field.py` & `awkward-2.1.2/tests/test_1619_from_parquet_empty_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1620_layout_builders.py` & `awkward-2.1.2/tests/test_1620_layout_builders.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1625_multiple_columns_from_rdataframe.py` & `awkward-2.1.2/tests/test_1625_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1642_from_iter_of_tuples.py` & `awkward-2.1.2/tests/test_1642_from_iter_of_tuples.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1650_Record_to_list_should_listify_itself.py` & `awkward-2.1.2/tests/test_1650_Record_to_list_should_listify_itself.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1671_categorical_type.py` & `awkward-2.1.2/tests/test_1671_categorical_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1672_broadcast_parameters.py` & `awkward-2.1.2/tests/test_1672_broadcast_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1677_array_builder_in_numba.py` & `awkward-2.1.2/tests/test_1677_array_builder_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1685_IndexedArray_project_parameters.py` & `awkward-2.1.2/tests/test_1685_IndexedArray_project_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1686_UnionArray_simplified_preserve_parameters.py` & `awkward-2.1.2/tests/test_1686_UnionArray_simplified_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1688_pack_categorical.py` & `awkward-2.1.2/tests/test_1688_pack_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1703_fill_none_typetracer.py` & `awkward-2.1.2/tests/test_1703_fill_none_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1707_broadcast_parameters_ufunc.py` & `awkward-2.1.2/tests/test_1707_broadcast_parameters_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1709_ak_array_constructor_behavior.py` & `awkward-2.1.2/tests/test_1709_ak_array_constructor_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1747_bytemaskedarray_mergemany.py` & `awkward-2.1.2/tests/test_1747_bytemaskedarray_mergemany.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1753_indexedarray_merge_kernel.py` & `awkward-2.1.2/tests/test_1753_indexedarray_merge_kernel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1762_jax_behavior_support.py` & `awkward-2.1.2/tests/test_1762_jax_behavior_support.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1764_jax_jacobian.py` & `awkward-2.1.2/tests/test_1764_jax_jacobian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1765_add_ioanas_test_of_to_arraylib.py` & `awkward-2.1.2/tests/test_1765_add_ioanas_test_of_to_arraylib.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1766_record_form_fields.py` & `awkward-2.1.2/tests/test_1766_record_form_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1781_rdataframe_snapshot.py` & `awkward-2.1.2/tests/test_1781_rdataframe_snapshot.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1784_reduce_leading_sublist.py` & `awkward-2.1.2/tests/test_1784_reduce_leading_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1790_reduce_regulararray.py` & `awkward-2.1.2/tests/test_1790_reduce_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1791_reduce_trailing_sublist.py` & `awkward-2.1.2/tests/test_1791_reduce_trailing_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1794_run_lengths_empty_sublist.py` & `awkward-2.1.2/tests/test_1794_run_lengths_empty_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1829_to_from_rdataframe_bool.py` & `awkward-2.1.2/tests/test_1829_to_from_rdataframe_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py` & `awkward-2.1.2/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1847_numpy_array_contiguous.py` & `awkward-2.1.2/tests/test_1847_numpy_array_contiguous.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1850_bytemasked_array_to_bytemaskedarray.py` & `awkward-2.1.2/tests/test_1850_bytemasked_array_to_bytemaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1867_pass_behavior_through_combinations.py` & `awkward-2.1.2/tests/test_1867_pass_behavior_through_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1904_drop_none.py` & `awkward-2.1.2/tests/test_1904_drop_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1914_improved_axis_to_posaxis.py` & `awkward-2.1.2/tests/test_1914_improved_axis_to_posaxis.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py` & `awkward-2.1.2/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1930_unflatten_counts_checks.py` & `awkward-2.1.2/tests/test_1930_unflatten_counts_checks.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1936_with_field_broadcasting.py` & `awkward-2.1.2/tests/test_1936_with_field_broadcasting.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1940_ak_backend.py` & `awkward-2.1.2/tests/test_1940_ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1943_regular_indexing.py` & `awkward-2.1.2/tests/test_1943_regular_indexing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1960_awkward_from_rdataframe.py` & `awkward-2.1.2/tests/test_1960_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_1961_ak_without_field.py` & `awkward-2.1.2/tests/test_1961_ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2020_reduce_axis_none.py` & `awkward-2.1.2/tests/test_2020_reduce_axis_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2021_check_TypeTracerArray_in_ak_where.py` & `awkward-2.1.2/tests/test_2021_check_TypeTracerArray_in_ak_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2023_from_rdataframe.py` & `awkward-2.1.2/tests/test_2023_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py` & `awkward-2.1.2/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2047_ak_transform_regular_to_jagged.py` & `awkward-2.1.2/tests/test_2047_ak_transform_regular_to_jagged.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2055_array_builder_check.py` & `awkward-2.1.2/tests/test_2055_array_builder_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2058_merge_numpy_array.py` & `awkward-2.1.2/tests/test_2058_merge_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2064_fill_none_record.py` & `awkward-2.1.2/tests/test_2064_fill_none_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2067_to_buffers_byteorder.py` & `awkward-2.1.2/tests/test_2067_to_buffers_byteorder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2070_to_layout_string.py` & `awkward-2.1.2/tests/test_2070_to_layout_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2071_unflatten_non_packed_counts.py` & `awkward-2.1.2/tests/test_2071_unflatten_non_packed_counts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2078_array_function_wrap.py` & `awkward-2.1.2/tests/test_2078_array_function_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2082_broadcast_zero_size.py` & `awkward-2.1.2/tests/test_2082_broadcast_zero_size.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2096_ak_scalar_type.py` & `awkward-2.1.2/tests/test_2096_ak_scalar_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2101_pickle_behavior_class.py` & `awkward-2.1.2/tests/test_2101_pickle_behavior_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2104_numpy_merge_option.py` & `awkward-2.1.2/tests/test_2104_numpy_merge_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2106_pickle_class.py` & `awkward-2.1.2/tests/test_2106_pickle_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2108_fill_none_indexed.py` & `awkward-2.1.2/tests/test_2108_fill_none_indexed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2115_fix_up_typetracers.py` & `awkward-2.1.2/tests/test_2115_fix_up_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2125_type_of_scalar.py` & `awkward-2.1.2/tests/test_2125_type_of_scalar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2150_typetracer_high_level_ufunc.py` & `awkward-2.1.2/tests/test_2150_typetracer_high_level_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2179_parameter_merging_rules.py` & `awkward-2.1.2/tests/test_2179_parameter_merging_rules.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2185_merge_union_of_records.py` & `awkward-2.1.2/tests/test_2185_merge_union_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py` & `awkward-2.1.2/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2198_almost_equal.py` & `awkward-2.1.2/tests/test_2198_almost_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2202_filter_multiple_columns_from_rdataframe.py` & `awkward-2.1.2/tests/test_2202_filter_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2214_offset_bool_index.py` & `awkward-2.1.2/tests/test_2214_offset_bool_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2226_slice_regulararray_typetracer.py` & `awkward-2.1.2/tests/test_2226_slice_regulararray_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2229_getitem_range_slice.py` & `awkward-2.1.2/tests/test_2229_getitem_range_slice.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2234_from_rdataframe_keep_order.py` & `awkward-2.1.2/tests/test_2234_from_rdataframe_keep_order.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2236_merge_union_of_records_option.py` & `awkward-2.1.2/tests/test_2236_merge_union_of_records_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2240_simplify_merge_as_union.py` & `awkward-2.1.2/tests/test_2240_simplify_merge_as_union.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2246_slice_not_packed.py` & `awkward-2.1.2/tests/test_2246_slice_not_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2250_full_like_bool.py` & `awkward-2.1.2/tests/test_2250_full_like_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2258_from_rdataframe_with_arguments.py` & `awkward-2.1.2/tests/test_2258_from_rdataframe_with_arguments.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2263_to_packed_list.py` & `awkward-2.1.2/tests/test_2263_to_packed_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2266_fix_nan_to_num.py` & `awkward-2.1.2/tests/test_2266_fix_nan_to_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2267_broadcast_fields.py` & `awkward-2.1.2/tests/test_2267_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2293_unflatten_typetracer.py` & `awkward-2.1.2/tests/test_2293_unflatten_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2297_common_backend.py` & `awkward-2.1.2/tests/test_2297_common_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/test_2319_from_buffers_array.py` & `awkward-2.1.2/tests/test_2319_from_buffers_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/list-depths-records-list.parquet` & `awkward-2.1.2/tests/samples/list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/list-depths-records.parquet` & `awkward-2.1.2/tests/samples/list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/list-depths-strings.parquet` & `awkward-2.1.2/tests/samples/list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/list-depths.parquet` & `awkward-2.1.2/tests/samples/list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/nonnullable-depths.parquet` & `awkward-2.1.2/tests/samples/nonnullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/nullable-depths.parquet` & `awkward-2.1.2/tests/samples/nullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/nullable-levels.parquet` & `awkward-2.1.2/tests/samples/nullable-levels.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/nullable-list-depths-records-list.parquet` & `awkward-2.1.2/tests/samples/nullable-list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/nullable-list-depths-records.parquet` & `awkward-2.1.2/tests/samples/nullable-list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/nullable-list-depths-strings.parquet` & `awkward-2.1.2/tests/samples/nullable-list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/nullable-list-depths.parquet` & `awkward-2.1.2/tests/samples/nullable-list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/nullable-record-primitives.parquet` & `awkward-2.1.2/tests/samples/nullable-record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/record-primitives.parquet` & `awkward-2.1.2/tests/samples/record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/test-nan-inf.json` & `awkward-2.1.2/tests/samples/test-nan-inf.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/test-two-arrays.json` & `awkward-2.1.2/tests/samples/test-two-arrays.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests/samples/test.json` & `awkward-2.1.2/tests/samples/test.json`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests-cuda/test_1276_cuda_num.py` & `awkward-2.1.2/tests-cuda/test_1276_cuda_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests-cuda/test_1276_cuda_transfers.py` & `awkward-2.1.2/tests-cuda/test_1276_cuda_transfers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests-cuda/test_1276_cupy_interop.py` & `awkward-2.1.2/tests-cuda/test_1276_cupy_interop.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests-cuda/test_1276_from_cupy.py` & `awkward-2.1.2/tests-cuda/test_1276_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests-cuda/test_1300_same_for_numba_cuda.py` & `awkward-2.1.2/tests-cuda/test_1300_same_for_numba_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests-cuda/test_1381_check_errors.py` & `awkward-2.1.2/tests-cuda/test_1381_check_errors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/tests-cuda/test_1809_array_cuda_jit.py` & `awkward-2.1.2/tests-cuda/test_1809_array_cuda_jit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/.gitignore` & `awkward-2.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/LICENSE` & `awkward-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `awkward-2.1.1/pyproject.toml` & `awkward-2.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "hatchling>=1.10.0",
     "hatch-fancy-pypi-readme"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "awkward"
-version = "2.1.1"
+version = "2.1.2"
 description = "Manipulate JSON-like data with NumPy-like idioms."
 license = { text = "BSD-3-Clause" }
 requires-python = ">=3.7"
 authors = [
     { name = "Jim Pivarski", email = "pivarski@princeton.edu" },
 ]
 classifiers = [
@@ -36,15 +36,15 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development",
     "Topic :: Utilities",
 ]
 dependencies = [
-    "awkward_cpp==12",
+    "awkward_cpp==13",
     "importlib_resources;python_version < \"3.9\"",
     "numpy>=1.17.0",
     "packaging",
     "typing_extensions>=4.1.0; python_version < \"3.11\""
 ]
 dynamic = [
     "readme"
@@ -286,23 +286,24 @@
     "E501",    # Line too long
     "UP030",   # {0} -> {}
     "PLR",     # Design related pylint codes
     "PT011",   # Exception too broad
     "NPY002",  # Replace legacy `np.random` call with `np.random.Generator`
     "PLW2901", # Outer for loop variable  overwritten by inner assignment target
     "PLW0603", # Using the global statement to update is discouraged
+    "PLC1901", # x == "" can be simplified to not x (empty string is falsey)
 ]
 target-version = "py37"
-typing-modules = ["awkward.typing"]
+typing-modules = ["awkward._typing"]
 src = ["src"]
 unfixable = [
     "T20",  # Removes print statements
     "F841", # Removes unused variables
 ]
-external = ["AK101"]
+external = []
 mccabe.max-complexity = 100
 
 [tool.ruff.per-file-ignores]
 "dev/*" = ["T20", "TID251"]
 "src/awkward/_connect/*" = ["TID251"]
 "src/awkward/__init__.py" = ["E402", "F401", "F403", "I001"]
 "src/awkward/operations/__init__.py" = ["F403"]
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 [build-system] requires = [ "hatchling>=1.10.0", "hatch-fancy-pypi-readme" ]
-build-backend = "hatchling.build" [project] name = "awkward" version = "2.1.1"
+build-backend = "hatchling.build" [project] name = "awkward" version = "2.1.2"
 description = "Manipulate JSON-like data with NumPy-like idioms." license =
 { text = "BSD-3-Clause" } requires-python = ">=3.7" authors = [ { name = "Jim
 Pivarski", email = "pivarski@princeton.edu" }, ] classifiers = [ "Development
 Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Intended
 Audience :: Information Technology", "Intended Audience :: Science/Research",
 "License :: OSI Approved :: BSD License", "Operating System :: MacOS :: MacOS
 X", "Operating System :: Microsoft :: Windows", "Operating System :: POSIX ::
@@ -11,15 +11,15 @@
 "Programming Language :: Python :: 3", "Programming Language :: Python :: 3 ::
 Only", "Programming Language :: Python :: 3.7", "Programming Language :: Python
 :: 3.8", "Programming Language :: Python :: 3.9", "Programming Language ::
 Python :: 3.10", "Programming Language :: Python :: 3.11", "Topic ::
 Scientific/Engineering", "Topic :: Scientific/Engineering :: Information
 Analysis", "Topic :: Scientific/Engineering :: Mathematics", "Topic ::
 Scientific/Engineering :: Physics", "Topic :: Software Development", "Topic ::
-Utilities", ] dependencies = [ "awkward_cpp==12",
+Utilities", ] dependencies = [ "awkward_cpp==13",
 "importlib_resources;python_version < \"3.9\"", "numpy>=1.17.0", "packaging",
 "typing_extensions>=4.1.0; python_version < \"3.11\"" ] dynamic = [ "readme" ]
 [project.entry-points.numba_extensions] init = "awkward.numba:_register"
 [project.urls] "Bug Tracker" = "https://github.com/scikit-hep/awkward-1.0/
 issues" "Chat" = "https://gitter.im/Scikit-HEP/awkward-array" "Discussions" =
 "https://github.com/scikit-hep/awkward-1.0/discussions" "Documentation" =
 "https://awkward-array.org" "Homepage" = "https://github.com/scikit-hep/
@@ -83,17 +83,18 @@
 flake8-pie "PL", # pylint "RUF", # Ruff-specific "T20", # flake8-print "UP", #
 pyupgrade "YTT", # flake8-2020 "EXE", # flake8-executable "NPY", # NumPy
 specific rules "TID251", # flake8-tidy-imports ] extend-ignore = [ "E501", #
 Line too long "UP030", # {0} -> {} "PLR", # Design related pylint codes
 "PT011", # Exception too broad "NPY002", # Replace legacy `np.random` call with
 `np.random.Generator` "PLW2901", # Outer for loop variable overwritten by inner
 assignment target "PLW0603", # Using the global statement to update is
-discouraged ] target-version = "py37" typing-modules = ["awkward.typing"] src =
+discouraged "PLC1901", # x == "" can be simplified to not x (empty string is
+falsey) ] target-version = "py37" typing-modules = ["awkward._typing"] src =
 ["src"] unfixable = [ "T20", # Removes print statements "F841", # Removes
-unused variables ] external = ["AK101"] mccabe.max-complexity = 100
-[tool.ruff.per-file-ignores] "dev/*" = ["T20", "TID251"] "src/awkward/_connect/
-*" = ["TID251"] "src/awkward/__init__.py" = ["E402", "F401", "F403", "I001"]
-"src/awkward/operations/__init__.py" = ["F403"] "src/awkward/_nplikes/*" =
-["TID251"] "tests*/*" = ["T20", "TID251"] [tool.ruff.flake8-tidy-
-imports.banned-api] "numpy".msg = "Use `numpy = ak._nplikes.Numpy.instance()`
-instead" "jax".msg = "Use `jax = ak._nplikes.Jax.instance()` instead"
-"cupy".msg = "Use `cupy = ak._nplikes.Cupy.instance()` instead"
+unused variables ] external = [] mccabe.max-complexity = 100 [tool.ruff.per-
+file-ignores] "dev/*" = ["T20", "TID251"] "src/awkward/_connect/*" = ["TID251"]
+"src/awkward/__init__.py" = ["E402", "F401", "F403", "I001"] "src/awkward/
+operations/__init__.py" = ["F403"] "src/awkward/_nplikes/*" = ["TID251"]
+"tests*/*" = ["T20", "TID251"] [tool.ruff.flake8-tidy-imports.banned-api]
+"numpy".msg = "Use `numpy = ak._nplikes.Numpy.instance()` instead" "jax".msg =
+"Use `jax = ak._nplikes.Jax.instance()` instead" "cupy".msg = "Use `cupy =
+ak._nplikes.Cupy.instance()` instead"
```

### Comparing `awkward-2.1.1/PKG-INFO` & `awkward-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awkward
-Version: 2.1.1
+Version: 2.1.2
 Summary: Manipulate JSON-like data with NumPy-like idioms.
 Project-URL: Bug Tracker, https://github.com/scikit-hep/awkward-1.0/issues
 Project-URL: Chat, https://gitter.im/Scikit-HEP/awkward-array
 Project-URL: Discussions, https://github.com/scikit-hep/awkward-1.0/discussions
 Project-URL: Documentation, https://awkward-array.org
 Project-URL: Homepage, https://github.com/scikit-hep/awkward-1.0
 Project-URL: Releases, https://github.com/scikit-hep/awkward-1.0/releases
@@ -32,15 +32,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
-Requires-Dist: awkward-cpp==12
+Requires-Dist: awkward-cpp==13
 Requires-Dist: importlib-resources; python_version < '3.9'
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: packaging
 Requires-Dist: typing-extensions>=4.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/scikit-hep/awkward-1.0">
@@ -65,14 +65,16 @@
 Arrays are **dynamically typed**, but operations on them are **compiled and fast**. Their behavior coincides with NumPy when array dimensions are regular and generalizes when they're not.
 
 # Motivating example
 
 Given an array of lists of objects with `x`, `y` fields (with nested lists in the `y` field),
 
 ```python
+import awkward as ak
+
 array = ak.Array([
     [{"x": 1.1, "y": [1]}, {"x": 2.2, "y": [1, 2]}, {"x": 3.3, "y": [1, 2, 3]}],
     [],
     [{"x": 4.4, "y": [1, 2, 3, 4]}, {"x": 5.5, "y": [1, 2, 3, 4, 5]}]
 ])
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: awkward Version: 2.1.1 Summary: Manipulate JSON-
+Metadata-Version: 2.1 Name: awkward Version: 2.1.2 Summary: Manipulate JSON-
 like data with NumPy-like idioms. Project-URL: Bug Tracker, https://github.com/
 scikit-hep/awkward-1.0/issues Project-URL: Chat, https://gitter.im/Scikit-HEP/
 awkward-array Project-URL: Discussions, https://github.com/scikit-hep/awkward-
 1.0/discussions Project-URL: Documentation, https://awkward-array.org Project-
 URL: Homepage, https://github.com/scikit-hep/awkward-1.0 Project-URL: Releases,
 https://github.com/scikit-hep/awkward-1.0/releases Project-URL: Source Code,
 https://github.com/scikit-hep/awkward-1.0 Author-email: Jim Pivarski
@@ -18,15 +18,15 @@
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics Classifier: Topic ::
 Software Development Classifier: Topic :: Utilities Requires-Python: >=3.7
-Requires-Dist: awkward-cpp==12 Requires-Dist: importlib-resources;
+Requires-Dist: awkward-cpp==13 Requires-Dist: importlib-resources;
 python_version < '3.9' Requires-Dist: numpy>=1.17.0 Requires-Dist: packaging
 Requires-Dist: typing-extensions>=4.1.0; python_version < '3.11' Description-
 Content-Type: text/markdown [https://github.com/scikit-hep/awkward-1.0/raw/
 main/docs-img/logo/logo-300px.png] [![PyPI version](https://badge.fury.io/py/
 awkward.svg)](https://pypi.org/project/awkward) [![Conda-Forge](https://
 img.shields.io/conda/vn/conda-forge/awkward)](https://github.com/conda-forge/
 awkward-feedstock) [![Python 3.7â3.11](https://img.shields.io/badge/python-
@@ -44,45 +44,46 @@
 chat-online-success)](https://gitter.im/Scikit-HEP/awkward-array) Awkward Array
 is a library for **nested, variable-sized data**, including arbitrary-length
 lists, records, mixed types, and missing data, using **NumPy-like idioms**.
 Arrays are **dynamically typed**, but operations on them are **compiled and
 fast**. Their behavior coincides with NumPy when array dimensions are regular
 and generalizes when they're not. # Motivating example Given an array of lists
 of objects with `x`, `y` fields (with nested lists in the `y` field), ```python
-array = ak.Array([ [{"x": 1.1, "y": [1]}, {"x": 2.2, "y": [1, 2]}, {"x": 3.3,
-"y": [1, 2, 3]}], [], [{"x": 4.4, "y": [1, 2, 3, 4]}, {"x": 5.5, "y": [1, 2, 3,
-4, 5]}] ]) ``` the following slices out the `y` values, drops the first element
-from each inner list, and runs NumPy's `np.square` function on everything that
-is left: ```python output = np.square(array["y", ..., 1:]) ``` The result is
-```python [ [[], [4], [4, 9]], [], [[4, 9, 16], [4, 9, 16, 25]] ] ``` The
-equivalent using only Python is ```python output = [] for sublist in array:
-tmp1 = [] for record in sublist: tmp2 = [] for number in record["y"][1:]:
-tmp2.append(np.square(number)) tmp1.append(tmp2) output.append(tmp1) ``` The
-expression using Awkward Arrays is more concise, using idioms familiar from
-NumPy, and it also has NumPy-like performance. For a similar problem 10 million
-times larger than the one above (single-threaded on a 2.2 GHz processor), * the
-Awkward Array one-liner takes **1.5 seconds** to run and uses **2.1 GB** of
-memory, * the equivalent using Python lists and dicts takes **140 seconds** to
-run and uses **22 GB** of memory. Awkward Array is even faster when used in
-[Numba](https://numba.pydata.org/)'s JIT-compiled functions. See the [Getting
-started](https://awkward-array.org/doc/main/getting-started/index.html)
-documentation on [awkward-array.org](https://awkward-array.org) for an
-introduction, including a [no-install demo](https://awkward-array.org/doc/main/
-getting-started/try-awkward-array.html) you can try in your web browser. #
-Getting help * View the documentation on [awkward-array.org](https://awkward-
-array.org/). * Report bugs, request features, and ask for additional
-documentation on [GitHub Issues](https://github.com/scikit-hep/awkward/issues).
-* If you have a "How do I...?" question, start a [GitHub Discussion](https://
-github.com/scikit-hep/awkward/discussions) with category "Q&A". *
-Alternatively, ask about it on [StackOverflow with the [awkward-array] tag]
-(https://stackoverflow.com/questions/tagged/awkward-array). Be sure to include
-tags for any other libraries that you use, such as Pandas or PyTorch. * To ask
-questions in real time, try the Gitter [Scikit-HEP/awkward-array](https://
-gitter.im/Scikit-HEP/awkward-array) chat room. # Installation Awkward Array can
-be installed from [PyPI](https://pypi.org/project/awkward) using pip: ```bash
-pip install awkward ``` The `awkward` package is pure Python, and it will
-download the `awkward-cpp` compiled components as a dependency. If there is no
-`awkward-cpp` binary package (wheel) for your platform and Python version, pip
-will attempt to compile it from source (which has additional dependencies, such
-as a C++ compiler). Awkward Array is also available on [conda-forge](https://
-conda-forge.org/docs/user/introduction.html#how-can-i-install-packages-from-
-conda-forge): ```bash conda install -c conda-forge awkward ```
+import awkward as ak array = ak.Array([ [{"x": 1.1, "y": [1]}, {"x": 2.2, "y":
+[1, 2]}, {"x": 3.3, "y": [1, 2, 3]}], [], [{"x": 4.4, "y": [1, 2, 3, 4]}, {"x":
+5.5, "y": [1, 2, 3, 4, 5]}] ]) ``` the following slices out the `y` values,
+drops the first element from each inner list, and runs NumPy's `np.square`
+function on everything that is left: ```python output = np.square(array["y",
+..., 1:]) ``` The result is ```python [ [[], [4], [4, 9]], [], [[4, 9, 16], [4,
+9, 16, 25]] ] ``` The equivalent using only Python is ```python output = [] for
+sublist in array: tmp1 = [] for record in sublist: tmp2 = [] for number in
+record["y"][1:]: tmp2.append(np.square(number)) tmp1.append(tmp2) output.append
+(tmp1) ``` The expression using Awkward Arrays is more concise, using idioms
+familiar from NumPy, and it also has NumPy-like performance. For a similar
+problem 10 million times larger than the one above (single-threaded on a 2.2
+GHz processor), * the Awkward Array one-liner takes **1.5 seconds** to run and
+uses **2.1 GB** of memory, * the equivalent using Python lists and dicts takes
+**140 seconds** to run and uses **22 GB** of memory. Awkward Array is even
+faster when used in [Numba](https://numba.pydata.org/)'s JIT-compiled
+functions. See the [Getting started](https://awkward-array.org/doc/main/
+getting-started/index.html) documentation on [awkward-array.org](https://
+awkward-array.org) for an introduction, including a [no-install demo](https://
+awkward-array.org/doc/main/getting-started/try-awkward-array.html) you can try
+in your web browser. # Getting help * View the documentation on [awkward-
+array.org](https://awkward-array.org/). * Report bugs, request features, and
+ask for additional documentation on [GitHub Issues](https://github.com/scikit-
+hep/awkward/issues). * If you have a "How do I...?" question, start a [GitHub
+Discussion](https://github.com/scikit-hep/awkward/discussions) with category
+"Q&A". * Alternatively, ask about it on [StackOverflow with the [awkward-array]
+tag](https://stackoverflow.com/questions/tagged/awkward-array). Be sure to
+include tags for any other libraries that you use, such as Pandas or PyTorch. *
+To ask questions in real time, try the Gitter [Scikit-HEP/awkward-array](https:
+//gitter.im/Scikit-HEP/awkward-array) chat room. # Installation Awkward Array
+can be installed from [PyPI](https://pypi.org/project/awkward) using pip:
+```bash pip install awkward ``` The `awkward` package is pure Python, and it
+will download the `awkward-cpp` compiled components as a dependency. If there
+is no `awkward-cpp` binary package (wheel) for your platform and Python
+version, pip will attempt to compile it from source (which has additional
+dependencies, such as a C++ compiler). Awkward Array is also available on
+[conda-forge](https://conda-forge.org/docs/user/introduction.html#how-can-i-
+install-packages-from-conda-forge): ```bash conda install -c conda-forge
+awkward ```
```

