# Comparing `tmp/sigmaepsilon-0.0.29.tar.gz` & `tmp/sigmaepsilon-0.0.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmaepsilon-0.0.29.tar", last modified: Sat Apr  8 20:39:41 2023, max compression
+gzip compressed data, was "sigmaepsilon-0.0.2b0.tar", last modified: Wed Oct 19 13:13:38 2022, max compression
```

## Comparing `sigmaepsilon-0.0.29.tar` & `sigmaepsilon-0.0.2b0.tar`

### file list

```diff
@@ -1,139 +1,132 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.243548 sigmaepsilon-0.0.29/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36022 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4735 2023-04-08 20:39:41.243548 sigmaepsilon-0.0.29/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3777 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-08 20:39:41.243548 sigmaepsilon-0.0.29/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2229 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.231548 sigmaepsilon-0.0.29/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.235548 sigmaepsilon-0.0.29/src/sigmaepsilon/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      345 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      288 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.235548 sigmaepsilon-0.0.29/src/sigmaepsilon/core/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/core/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/core/material.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.235548 sigmaepsilon-0.0.29/src/sigmaepsilon/examples/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/examples/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      762 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/examples/downloads.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3046 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/examples/examples.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.235548 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.239548 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8557 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/Q5V.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11142 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/andes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14798 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/bernoulli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/bernoulli2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      807 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/bernoulli3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11203 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/celldata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/cst.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    46938 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/elem.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.239548 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/gen/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/gen/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7675 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/gen/b2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9905 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/gen/b3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/h27.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/h8.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1720 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/lst.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6464 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/meta.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/q4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1134 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/q9.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/tet10.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/tet4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/wedge.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1543 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/dofmap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12459 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/ebc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11699 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/femsolver.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3992 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/linemesh.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.239548 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/material/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/material/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5804 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/material/beam.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2360 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/material/membrane.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2844 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/material/mindlinplate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3138 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/material/mindlinshell.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2418 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/material/solid.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3687 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/material/solid3d.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2372 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/material/surface.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24692 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/mesh.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/metamesh.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7644 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/pointdata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19982 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/structure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fem/surfacemesh.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.239548 sigmaepsilon-0.0.29/src/sigmaepsilon/fourier/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fourier/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3551 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fourier/beam.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16520 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fourier/loads.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3264 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fourier/plate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15433 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fourier/postproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11996 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fourier/preproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      245 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fourier/problem.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2355 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fourier/proc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/fourier/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.239548 sigmaepsilon-0.0.29/src/sigmaepsilon/material/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       94 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.239548 sigmaepsilon-0.0.29/src/sigmaepsilon/material/beam/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/beam/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.239548 sigmaepsilon-0.0.29/src/sigmaepsilon/material/beam/bernoulli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/beam/bernoulli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7415 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/beam/bernoulli/section.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.239548 sigmaepsilon-0.0.29/src/sigmaepsilon/material/homg/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/homg/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3528 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/homg/ebc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5295 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/homg/rvs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6816 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/homg/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.243548 sigmaepsilon-0.0.29/src/sigmaepsilon/material/hooke/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/hooke/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2723 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/hooke/sym.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1504 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/hooke/tensor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14058 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/hooke/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.243548 sigmaepsilon-0.0.29/src/sigmaepsilon/material/surface/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/surface/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4212 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/surface/membrane.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5730 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/surface/meta.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10528 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/material/surface/mindlin.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.243548 sigmaepsilon-0.0.29/src/sigmaepsilon/topopt/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/topopt/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.243548 sigmaepsilon-0.0.29/src/sigmaepsilon/topopt/joint/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/topopt/joint/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18323 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/topopt/joint/cubejoint.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.243548 sigmaepsilon-0.0.29/src/sigmaepsilon/topopt/oc/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/topopt/oc/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1020 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/topopt/oc/filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8481 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/topopt/oc/oc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2738 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/topopt/oc/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.243548 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.243548 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.243548 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/cells/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/cells/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9073 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/cells/bernoulli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10935 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/cells/cells.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7332 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/dyn.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1966 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/ebc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6038 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/eigsolve.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16553 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/fem.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7213 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/imap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8165 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/linsolve.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6541 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/postproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17705 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/preproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4588 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/tr.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.243548 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/material/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/material/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2316 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/material/bernoulli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2123 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/material/hmh.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/material/material.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8490 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/material/mindlin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10269 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/material/postproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4180 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/src/sigmaepsilon/utils/material/surface.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-08 20:39:41.235548 sigmaepsilon-0.0.29/src/sigmaepsilon.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4735 2023-04-08 20:39:41.000000 sigmaepsilon-0.0.29/src/sigmaepsilon.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4132 2023-04-08 20:39:41.000000 sigmaepsilon-0.0.29/src/sigmaepsilon.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-08 20:39:41.000000 sigmaepsilon-0.0.29/src/sigmaepsilon.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-08 20:39:41.000000 sigmaepsilon-0.0.29/src/sigmaepsilon.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-04-08 20:39:41.000000 sigmaepsilon-0.0.29/src/sigmaepsilon.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-08 20:39:41.000000 sigmaepsilon-0.0.29/src/sigmaepsilon.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-04-08 20:39:35.000000 sigmaepsilon-0.0.29/test-requirements.txt
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.437022 sigmaepsilon-0.0.2b0/
+-rw-rw-rw-   0        0        0    11558 2022-05-11 05:24:57.000000 sigmaepsilon-0.0.2b0/LICENSE
+-rw-rw-rw-   0        0        0      206 2022-08-16 16:03:22.000000 sigmaepsilon-0.0.2b0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4571 2022-10-19 13:13:38.437022 sigmaepsilon-0.0.2b0/PKG-INFO
+-rw-rw-rw-   0        0        0     3705 2022-09-29 17:48:15.000000 sigmaepsilon-0.0.2b0/README.md
+-rw-rw-rw-   0        0        0      110 2021-11-30 19:14:54.000000 sigmaepsilon-0.0.2b0/pyproject.toml
+-rw-rw-rw-   0        0        0      127 2022-10-19 12:56:46.000000 sigmaepsilon-0.0.2b0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2022-10-19 13:13:38.438023 sigmaepsilon-0.0.2b0/setup.cfg
+-rw-rw-rw-   0        0        0     2270 2022-08-16 16:13:09.000000 sigmaepsilon-0.0.2b0/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.260017 sigmaepsilon-0.0.2b0/src/
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.301019 sigmaepsilon-0.0.2b0/src/sigmaepsilon/
+-rw-rw-rw-   0        0        0      122 2022-10-19 13:09:43.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.329018 sigmaepsilon-0.0.2b0/src/sigmaepsilon/examples/
+-rw-rw-rw-   0        0        0       49 2022-10-11 09:18:23.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/examples/__init__.py
+-rw-rw-rw-   0        0        0      798 2022-10-12 17:20:34.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/examples/downloads.py
+-rw-rw-rw-   0        0        0     3280 2022-10-19 12:39:45.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/examples/examples.py
+-rw-rw-rw-   0        0        0      277 2022-10-17 17:00:18.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/io.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.331019 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/
+-rw-rw-rw-   0        0        0      282 2022-10-14 16:41:26.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/__init__.py
+-rw-rw-rw-   0        0        0      343 2022-02-22 09:20:58.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/config.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.351036 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/
+-rw-rw-rw-   0        0        0      215 2022-10-14 16:41:26.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.371018 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/
+-rw-rw-rw-   0        0        0      848 2022-10-12 12:55:26.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/__init__.py
+-rw-rw-rw-   0        0        0    11393 2022-10-19 11:42:30.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/bernoulli.py
+-rw-rw-rw-   0        0        0      703 2022-10-10 22:06:22.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/bernoulli2.py
+-rw-rw-rw-   0        0        0      609 2022-10-10 22:06:22.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/bernoulli3.py
+-rw-rw-rw-   0        0        0     9417 2022-10-19 01:28:55.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/celldata.py
+-rw-rw-rw-   0        0        0      759 2022-08-15 22:53:20.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/cst.py
+-rw-rw-rw-   0        0        0    39063 2022-10-18 13:11:04.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/elem.py
+-rw-rw-rw-   0        0        0     7151 2022-08-15 22:53:44.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/felippa.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.375019 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/gen/
+-rw-rw-rw-   0        0        0       23 2022-10-11 04:18:58.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/gen/__init__.py
+-rw-rw-rw-   0        0        0     4655 2022-07-11 17:02:13.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/gen/b2.py
+-rw-rw-rw-   0        0        0     6294 2022-07-11 17:02:13.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/gen/b3.py
+-rw-rw-rw-   0        0        0      520 2022-08-15 22:54:02.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/h27.py
+-rw-rw-rw-   0        0        0      518 2022-08-15 22:53:54.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/h8.py
+-rw-rw-rw-   0        0        0     1222 2022-08-15 22:54:08.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/lst.py
+-rw-rw-rw-   0        0        0     6602 2022-10-14 16:41:26.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/meta.py
+-rw-rw-rw-   0        0        0     2252 2022-08-15 22:54:33.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/q4.py
+-rw-rw-rw-   0        0        0      813 2022-09-06 14:21:43.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/q9.py
+-rw-rw-rw-   0        0        0      806 2022-08-15 22:54:53.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/tet10.py
+-rw-rw-rw-   0        0        0      375 2022-08-15 22:54:47.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/tet4.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.378019 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/utils/
+-rw-rw-rw-   0        0        0       49 2022-03-08 19:23:06.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/utils/__init__.py
+-rw-rw-rw-   0        0        0     9249 2022-10-19 11:32:49.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/utils/bernoulli.py
+-rw-rw-rw-   0        0        0    18771 2022-08-15 23:11:07.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/utils/utils.py
+-rw-rw-rw-   0        0        0      263 2022-05-19 13:40:29.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/config.py
+-rw-rw-rw-   0        0        0     7658 2022-10-11 04:37:39.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/dyn.py
+-rw-rw-rw-   0        0        0     6333 2022-09-29 17:48:16.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/eigsolve.py
+-rw-rw-rw-   0        0        0    11277 2022-10-11 04:24:28.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/femsolver.py
+-rw-rw-rw-   0        0        0     6459 2022-08-15 22:48:37.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/imap.py
+-rw-rw-rw-   0        0        0    10475 2022-10-12 17:08:37.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/io.py
+-rw-rw-rw-   0        0        0     7614 2022-10-12 17:13:20.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/linemesh.py
+-rw-rw-rw-   0        0        0     9727 2022-09-29 17:48:16.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/linsolve.py
+-rw-rw-rw-   0        0        0    18446 2022-10-18 18:10:38.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/mesh.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.389019 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/
+-rw-rw-rw-   0        0        0       20 2022-07-11 17:01:44.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/__init__.py
+-rw-rw-rw-   0        0        0     4201 2022-07-30 09:17:16.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/beam.py
+-rw-rw-rw-   0        0        0     2555 2022-07-12 21:42:22.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/membrane.py
+-rw-rw-rw-   0        0        0     2828 2022-07-12 21:35:19.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/plate.py
+-rw-rw-rw-   0        0        0     2662 2022-08-15 22:55:06.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/solid.py
+-rw-rw-rw-   0        0        0     2048 2022-07-30 09:17:32.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/solid3d.py
+-rw-rw-rw-   0        0        0     2503 2022-08-15 22:55:14.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/surface.py
+-rw-rw-rw-   0        0        0     1733 2022-07-31 12:31:15.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/utils.py
+-rw-rw-rw-   0        0        0     6823 2022-09-29 17:48:16.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/pointdata.py
+-rw-rw-rw-   0        0        0     1568 2022-10-18 14:54:46.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/postproc.py
+-rw-rw-rw-   0        0        0     8458 2022-08-15 22:49:26.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/preproc.py
+-rw-rw-rw-   0        0        0    14635 2022-10-09 16:55:09.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/structure.py
+-rw-rw-rw-   0        0        0      907 2022-08-15 22:50:04.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/surfacemesh.py
+-rw-rw-rw-   0        0        0     5077 2022-10-14 16:41:26.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/tr.py
+-rw-rw-rw-   0        0        0    19839 2022-10-09 15:16:48.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/utils.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.401020 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fourier/
+-rw-rw-rw-   0        0        0       90 2022-07-03 12:13:18.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fourier/__init__.py
+-rw-rw-rw-   0        0        0    17249 2022-09-05 20:59:01.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fourier/doc.py
+-rw-rw-rw-   0        0        0     1774 2022-08-10 11:38:28.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fourier/latex.py
+-rw-rw-rw-   0        0        0    12396 2022-08-15 22:51:33.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fourier/loads.py
+-rw-rw-rw-   0        0        0     3606 2022-07-03 14:57:05.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fourier/plate.py
+-rw-rw-rw-   0        0        0      559 2022-08-15 22:51:48.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fourier/plot.py
+-rw-rw-rw-   0        0        0    12577 2022-08-15 22:51:54.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fourier/postproc.py
+-rw-rw-rw-   0        0        0     4645 2022-08-15 22:52:01.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fourier/preproc.py
+-rw-rw-rw-   0        0        0     1148 2022-08-15 22:52:07.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fourier/proc.py
+-rw-rw-rw-   0        0        0      630 2022-07-03 15:47:26.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fourier/symtools.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.403019 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/material/
+-rw-rw-rw-   0        0        0       25 2022-02-21 20:12:29.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/material/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.406019 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/material/hooke/
+-rw-rw-rw-   0        0        0     2726 2022-10-19 08:30:51.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/material/hooke/sym.py
+-rw-rw-rw-   0        0        0     5328 2022-08-15 22:52:26.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/material/hooke/utils.py
+-rw-rw-rw-   0        0        0     1675 2022-09-08 22:12:41.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/material/utils.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.410020 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/
+-rw-rw-rw-   0        0        0      106 2022-02-21 23:37:24.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.413017 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/bernoulli/
+-rw-rw-rw-   0        0        0       47 2022-09-08 19:37:05.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/bernoulli/__init__.py
+-rw-rw-rw-   0        0        0    19036 2022-10-09 19:40:44.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/bernoulli/section.py
+-rw-rw-rw-   0        0        0     2499 2022-09-08 22:22:13.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/bernoulli/utils.py
+-rw-rw-rw-   0        0        0     4773 2022-09-05 23:29:34.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/membrane.py
+-rw-rw-rw-   0        0        0     5681 2022-09-05 23:48:05.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/metashell.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.418020 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/mindlin/
+-rw-rw-rw-   0        0        0       74 2022-02-21 23:37:10.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/mindlin/__init__.py
+-rw-rw-rw-   0        0        0    10928 2022-10-19 08:09:11.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/mindlin/mindlin.py
+-rw-rw-rw-   0        0        0    10725 2022-08-15 23:12:33.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/mindlin/postproc.py
+-rw-rw-rw-   0        0        0     8659 2022-07-03 16:46:24.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/mindlin/utils.py
+-rw-rw-rw-   0        0        0     4299 2022-09-05 23:55:35.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/utils.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.419019 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/
+-rw-rw-rw-   0        0        0       25 2022-08-21 11:12:27.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.421019 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/fem/
+-rw-rw-rw-   0        0        0      161 2022-08-15 22:45:17.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/fem/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.423021 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/fem/cells/
+-rw-rw-rw-   0        0        0     8949 2022-08-15 22:44:23.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/fem/cells/Q5V.py
+-rw-rw-rw-   0        0        0       29 2022-02-11 19:04:31.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/fem/cells/__init__.py
+-rw-rw-rw-   0        0        0     3518 2022-08-15 22:46:25.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/fem/mesh.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.427019 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/fem/structure/
+-rw-rw-rw-   0        0        0      140 2022-08-15 22:45:28.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/fem/structure/__init__.py
+-rw-rw-rw-   0        0        0      300 2022-08-04 09:48:05.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/fem/structure/domain.py
+-rw-rw-rw-   0        0        0     1036 2022-10-17 17:00:18.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/fem/structure/structure.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.429020 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/joint/
+-rw-rw-rw-   0        0        0       24 2022-08-21 11:09:47.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/joint/__init__.py
+-rw-rw-rw-   0        0        0    18610 2022-08-24 18:25:45.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/joint/cubejoint.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.435023 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/oc/
+-rw-rw-rw-   0        0        0     6434 2022-08-15 23:20:01.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/oc/SIMP_OC_FEM_old.py
+-rw-rw-rw-   0        0        0       42 2022-10-17 17:00:18.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/oc/__init__.py
+-rw-rw-rw-   0        0        0     1100 2022-08-15 23:19:38.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/oc/filter.py
+-rw-rw-rw-   0        0        0     8672 2022-10-19 12:03:18.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/oc/oc.py
+-rw-rw-rw-   0        0        0     2847 2022-08-21 11:12:04.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/oc/utils.py
+drwxrwxrwx   0        0        0        0 2022-10-19 13:13:38.326053 sigmaepsilon-0.0.2b0/src/sigmaepsilon.egg-info/
+-rw-rw-rw-   0        0        0     4571 2022-10-19 13:13:38.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4221 2022-10-19 13:13:38.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-19 13:13:38.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-07-30 11:00:03.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      113 2022-10-19 13:13:38.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2022-10-19 13:13:38.000000 sigmaepsilon-0.0.2b0/src/sigmaepsilon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       45 2022-10-10 21:39:06.000000 sigmaepsilon-0.0.2b0/test-requirements.txt
```

### Comparing `sigmaepsilon-0.0.29/PKG-INFO` & `sigmaepsilon-0.0.2b0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,99 @@
-Metadata-Version: 2.1
-Name: sigmaepsilon
-Version: 0.0.29
-Summary: High-Performance Computational Mechanics in Python.
-Home-page: https://github.com/dewloosh/sigmaepsilon
-Download-URL: https://github.com/dewloosh/sigmaepsilon/archive/refs/tags/0.0.29.zip
-Author: Bence Balogh
-Author-email: benceeok@gmail.com
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: Free for non-commercial use
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6, <3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **SigmaEpsilon** - High-Performance Computational Solid Mechanics in Python
-
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dewloosh/SigmaEpsilon/main?labpath=notebooksnotebooks%2Flpp.ipynb?urlpath=lab)
-[![CircleCI](https://circleci.com/gh/dewloosh/SigmaEpsilon.svg?style=shield)](https://circleci.com/gh/dewloosh/SigmaEpsilon) 
-[![Documentation Status](https://readthedocs.org/projects/sigmaepsilon/badge/?version=latest)](https://sigmaepsilon.readthedocs.io/en/latest/?badge=latest) 
-[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![PyPI](https://badge.fury.io/py/sigmaepsilon.svg)](https://pypi.org/project/sigmaepsilon)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-> **Warning**
-> This package is under active development and in an **alpha stage**. Come back later, or star the repo to make sure you don’t miss the first stable release!
-
-## Highlights
-
-Head over to the Quick Examples page in the docs to explore our gallery of examples showcasing what SigmaEpsilon can do! Want to test-drive SigmaEpsilon? All of the examples from the gallery are live on MyBinder for you to test drive without installing anything locally: Launch on Binder.
-
-### Overview
-
-* A `solid` submodule to analyze and optimize solid structures of all kinds with the **Finite Element Method**. The implementations so far only cover linear behaviour, but with practically no limits on the complexity of the shape and topology of the domain under investigation.
-
-## Installation
-
-This is optional, but we suggest you to create a dedicated virtual enviroment at all times to avoid conflicts with your other projects. Create a folder, open a command shell in that folder and use the following command
-
-```console
->>> python -m venv venv_name
-```
-
-Once the enviroment is created, activate it via typing
-
-```console
->>> .\venv_name\Scripts\activate
-```
-
-`sigmaepsilon` can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.6:
-
-```console
->>> pip install sigmaepsilon
-```
-
-## **Documentation**
-
-Refer to the [docs](https://sigmaepsilon.readthedocs.io/en/latest/) for further details on installation and usage.
-
-## **Testing**
-
-To run all tests, open up a console in the root directory of the project and type the following
-
-```console
->>> python -m unittest
-```
-
-## **Dependencies**
-
-We use Numba's JIT compiler to speed up heavy computations, and it relies on the C++ redistributable package. It is likely already installed on your system, but if it is not, you can download it from Microsoft's website under "Other Tools, Frameworks, and Redistributables".
-
-must have
-
-* `Numba`, `NumPy`, `SciPy`, `SymPy`, `awkward`
-
-strongly suggested
-
-* `PyVista`, `Plotly`, `matplotlib`, `sectionproperties`
-
-optional
-
-* `networkx`
-
-## **License**
-
-SigmaEpsilon is Copyright(C) 2022: Bence Balogh
-
-All rights reserved.
-
-This program is dual-licensed as follows:
-
-(1) You may use SigmaEpsilon as free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
-
-In this case the program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License at http://www.gnu.org/licenses/gpl.txt or in the LICENSE file of this repository for more details.
-
-(2) You may use SigmaEpsilon as part of a commercial software. In this case a proper agreement must be reached with the Authors based on a proper licensing contract.
+Metadata-Version: 2.1
+Name: sigmaepsilon
+Version: 0.0.2b0
+Summary: High-Performance Computational Mechanics in Python.
+Home-page: https://github.com/dewloosh/sigmaepsilon
+Author: Bence Balogh
+Author-email: benceeok@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/dewloosh/sigmaepsilon/archive/refs/tags/0.0.2b.zip
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6, <3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **SigmaEpsilon** - High-Performance Computational Solid Mechanics in Python
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dewloosh/SigmaEpsilon/main?labpath=notebooksnotebooks%2Flpp.ipynb?urlpath=lab)
+[![CircleCI](https://circleci.com/gh/dewloosh/SigmaEpsilon.svg?style=shield)](https://circleci.com/gh/dewloosh/SigmaEpsilon) 
+[![Documentation Status](https://readthedocs.org/projects/sigmaepsilon/badge/?version=latest)](https://sigmaepsilon.readthedocs.io/en/latest/?badge=latest) 
+[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI](https://badge.fury.io/py/sigmaepsilon.svg)](https://pypi.org/project/sigmaepsilon) 
+
+> **Warning**
+> This package is under active development and in an **alpha stage**. Come back later, or star the repo to make sure you donâ€™t miss the first stable release!
+
+## Highlights
+
+Head over to the Quick Examples page in the docs to explore our gallery of examples showcasing what SigmaEpsilon can do! Want to test-drive SigmaEpsilon? All of the examples from the gallery are live on MyBinder for you to test drive without installing anything locally: Launch on Binder.
+
+### Overview
+
+* A `solid` submodule to analyze and optimize solid structures of all kinds with the **Finite Element Method**. The implementations so far only cover linear behaviour, but with practically no limits on the complexity of the shape and topology of the domain under investigation.
+
+## **Installation**
+This is optional, but we suggest you to create a dedicated virtual enviroment at all times to avoid conflicts with your other projects. Create a folder, open a command shell in that folder and use the following command
+
+```console
+>>> python -m venv venv_name
+```
+
+Once the enviroment is created, activate it via typing
+
+```console
+>>> .\venv_name\Scripts\activate
+```
+
+`sigmaepsilon` can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.6:
+
+```console
+>>> pip install sigmaepsilon
+```
+
+## **Documentation**
+
+Refer to the [docs](https://sigmaepsilon.readthedocs.io/en/latest/) for further details on installation and usage.
+
+## **Testing**
+
+To run all tests, open up a console in the root directory of the project and type the following
+
+```console
+>>> python -m unittest
+```
+
+## **Dependencies**
+
+We use Numba's JIT compiler to speed up heavy computations, and it relies on the C++ redistributable package. It is likely already installed on your system, but if it is not, you can download it from Microsoft's website under "Other Tools, Frameworks, and Redistributables".
+
+must have 
+  * `Numba`, `NumPy`, `SciPy`, `SymPy`, `awkward`
+
+strongly suggested
+  * `PyVista`, `Plotly`, `matplotlib`, `sectionproperties`
+
+optional 
+  * `networkx`
+
+## **License**
+
+SigmaEpsilon is Copyright(C) 2022: Bence Balogh
+
+All rights reserved.
+
+This program is dual-licensed as follows:
+
+(1) You may use SigmaEpsilon as free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
+
+In this case the program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License (http://www.gnu.org/licenses/gpl.txt) for more details.
+
+(2) You may use SigmaEpsilon as part of a commercial software. In this case a proper agreement must be reached with the Authors based on a proper licensing contract.
+
```

### Comparing `sigmaepsilon-0.0.29/README.md` & `sigmaepsilon-0.0.2b0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,76 @@
-# **SigmaEpsilon** - High-Performance Computational Solid Mechanics in Python
-
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dewloosh/SigmaEpsilon/main?labpath=notebooksnotebooks%2Flpp.ipynb?urlpath=lab)
-[![CircleCI](https://circleci.com/gh/dewloosh/SigmaEpsilon.svg?style=shield)](https://circleci.com/gh/dewloosh/SigmaEpsilon) 
-[![Documentation Status](https://readthedocs.org/projects/sigmaepsilon/badge/?version=latest)](https://sigmaepsilon.readthedocs.io/en/latest/?badge=latest) 
-[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![PyPI](https://badge.fury.io/py/sigmaepsilon.svg)](https://pypi.org/project/sigmaepsilon)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-> **Warning**
-> This package is under active development and in an **alpha stage**. Come back later, or star the repo to make sure you don’t miss the first stable release!
-
-## Highlights
-
-Head over to the Quick Examples page in the docs to explore our gallery of examples showcasing what SigmaEpsilon can do! Want to test-drive SigmaEpsilon? All of the examples from the gallery are live on MyBinder for you to test drive without installing anything locally: Launch on Binder.
-
-### Overview
-
-* A `solid` submodule to analyze and optimize solid structures of all kinds with the **Finite Element Method**. The implementations so far only cover linear behaviour, but with practically no limits on the complexity of the shape and topology of the domain under investigation.
-
-## Installation
-
-This is optional, but we suggest you to create a dedicated virtual enviroment at all times to avoid conflicts with your other projects. Create a folder, open a command shell in that folder and use the following command
-
-```console
->>> python -m venv venv_name
-```
-
-Once the enviroment is created, activate it via typing
-
-```console
->>> .\venv_name\Scripts\activate
-```
-
-`sigmaepsilon` can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.6:
-
-```console
->>> pip install sigmaepsilon
-```
-
-## **Documentation**
-
-Refer to the [docs](https://sigmaepsilon.readthedocs.io/en/latest/) for further details on installation and usage.
-
-## **Testing**
-
-To run all tests, open up a console in the root directory of the project and type the following
-
-```console
->>> python -m unittest
-```
-
-## **Dependencies**
-
-We use Numba's JIT compiler to speed up heavy computations, and it relies on the C++ redistributable package. It is likely already installed on your system, but if it is not, you can download it from Microsoft's website under "Other Tools, Frameworks, and Redistributables".
-
-must have
-
-* `Numba`, `NumPy`, `SciPy`, `SymPy`, `awkward`
-
-strongly suggested
-
-* `PyVista`, `Plotly`, `matplotlib`, `sectionproperties`
-
-optional
-
-* `networkx`
-
-## **License**
-
-SigmaEpsilon is Copyright(C) 2022: Bence Balogh
-
-All rights reserved.
-
-This program is dual-licensed as follows:
-
-(1) You may use SigmaEpsilon as free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
-
-In this case the program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License at http://www.gnu.org/licenses/gpl.txt or in the LICENSE file of this repository for more details.
-
+# **SigmaEpsilon** - High-Performance Computational Solid Mechanics in Python
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dewloosh/SigmaEpsilon/main?labpath=notebooksnotebooks%2Flpp.ipynb?urlpath=lab)
+[![CircleCI](https://circleci.com/gh/dewloosh/SigmaEpsilon.svg?style=shield)](https://circleci.com/gh/dewloosh/SigmaEpsilon) 
+[![Documentation Status](https://readthedocs.org/projects/sigmaepsilon/badge/?version=latest)](https://sigmaepsilon.readthedocs.io/en/latest/?badge=latest) 
+[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI](https://badge.fury.io/py/sigmaepsilon.svg)](https://pypi.org/project/sigmaepsilon) 
+
+> **Warning**
+> This package is under active development and in an **alpha stage**. Come back later, or star the repo to make sure you don’t miss the first stable release!
+
+## Highlights
+
+Head over to the Quick Examples page in the docs to explore our gallery of examples showcasing what SigmaEpsilon can do! Want to test-drive SigmaEpsilon? All of the examples from the gallery are live on MyBinder for you to test drive without installing anything locally: Launch on Binder.
+
+### Overview
+
+* A `solid` submodule to analyze and optimize solid structures of all kinds with the **Finite Element Method**. The implementations so far only cover linear behaviour, but with practically no limits on the complexity of the shape and topology of the domain under investigation.
+
+## **Installation**
+This is optional, but we suggest you to create a dedicated virtual enviroment at all times to avoid conflicts with your other projects. Create a folder, open a command shell in that folder and use the following command
+
+```console
+>>> python -m venv venv_name
+```
+
+Once the enviroment is created, activate it via typing
+
+```console
+>>> .\venv_name\Scripts\activate
+```
+
+`sigmaepsilon` can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.6:
+
+```console
+>>> pip install sigmaepsilon
+```
+
+## **Documentation**
+
+Refer to the [docs](https://sigmaepsilon.readthedocs.io/en/latest/) for further details on installation and usage.
+
+## **Testing**
+
+To run all tests, open up a console in the root directory of the project and type the following
+
+```console
+>>> python -m unittest
+```
+
+## **Dependencies**
+
+We use Numba's JIT compiler to speed up heavy computations, and it relies on the C++ redistributable package. It is likely already installed on your system, but if it is not, you can download it from Microsoft's website under "Other Tools, Frameworks, and Redistributables".
+
+must have 
+  * `Numba`, `NumPy`, `SciPy`, `SymPy`, `awkward`
+
+strongly suggested
+  * `PyVista`, `Plotly`, `matplotlib`, `sectionproperties`
+
+optional 
+  * `networkx`
+
+## **License**
+
+SigmaEpsilon is Copyright(C) 2022: Bence Balogh
+
+All rights reserved.
+
+This program is dual-licensed as follows:
+
+(1) You may use SigmaEpsilon as free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
+
+In this case the program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License (http://www.gnu.org/licenses/gpl.txt) for more details.
+
 (2) You may use SigmaEpsilon as part of a commercial software. In this case a proper agreement must be reached with the Authors based on a proper licensing contract.
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/examples/downloads.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/examples/downloads.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from dewloosh.core.downloads import download_stand, _download_file
-from polymesh import PolyData
-from typing import Union
-
-
-def download_bernoulli_console_json_linstat():  # pragma: no cover
-    """
-    Downloads the description of a simple bernoulli console as a json file.
-
-    Returns
-    -------
-    str
-        A path to a file on your filesystem.
-
-    Example
-    --------
-    >>> from sigmaepsilon.examples import download_bernoulli_console_json_20B2
-    >>> jsonpath = download_bernoulli_console_json_20B2()
-
-    """
-    return _download_file("console_bernoulli_linstat.json")[0]
-
-
-"""def stand_vtk(read=False) -> Union[str, PolyData]:
-    vtkpath = download_stand()
-    if read:
-        return PolyData.read(vtkpath)
-    else:
-        return vtkpath"""
+from dewloosh.core.downloads import download_stand, _download_file
+from polymesh import PolyData
+from typing import Union
+
+
+
+def download_bernoulli_console_json_linstat():  # pragma: no cover
+    """
+    Downloads the description of a simple bernoulli console as a json file.
+   
+    Returns
+    -------
+    str
+        A path to a file on your filesystem.
+
+    Example
+    --------
+    >>> from sigmaepsilon.examples import download_bernoulli_console_json_20B2
+    >>> jsonpath = download_bernoulli_console_json_20B2()
+    
+    """
+    return _download_file('console_bernoulli_linstat.json')[0]
+
+
+"""def stand_vtk(read=False) -> Union[str, PolyData]:
+    vtkpath = download_stand()
+    if read:
+        return PolyData.read(vtkpath)
+    else:
+        return vtkpath"""
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/examples/examples.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/examples/examples.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,112 @@
-import numpy as np
-from linkeddeepdict import LinkedDeepDict
-from linkeddeepdict.tools import getallfromkwargs
-
-from polymesh.space import StandardFrame, PointCloud
-from polymesh.grid import gridH8 as grid
-from polymesh.utils.topology.tr import H8_to_L2
-from polymesh.utils.space import index_of_closest_point, frames_of_lines
-
-from sigmaepsilon import BeamSection
-from sigmaepsilon import Structure, LineMesh, PointData
-from sigmaepsilon.fem.cells import B2 as Beam
-
-
-def console_grid_bernoulli() -> Structure:
-    """
-    Returns a simple console as a grid of 2-noded Bernoulli beams.
-
-    Example
-    -------
-    >>> from sigmaepsilon.examples import console_grid_bernoulli
-    >>> structure = console_grid_bernoulli()
-    >>> structure.linsolve()
-    """
-    # units in kN and cm
-
-    Lx, Ly, Lz = 100.0, 15.0, 10.0  # size of the grid
-    nx, ny, nz = 4, 2, 2  # desity of the grid
-
-    d = 1.2  # outer diameter of the tube
-    t = 0.4  # thickness of the tube
-
-    Ex = 21000.0
-    nu = 0.25
-    fy = 35.0
-
-    loads = LinkedDeepDict()
-
-    # load case 1
-    loads["LC1", "position"] = [Lx, 0, 0]
-    loads["LC1", "value"] = [0, 0, 2.0, 0, 0, 0]
-
-    # load case 2
-    loads["LC2", "position"] = [Lx, Ly / 2, 0]
-    loads["LC2", "value"] = [0, 2.0, 0, 0, 0, 0]
-
-    # load case 3
-    loads["LC3", "position"] = [Lx, -Ly / 2, 0]
-    loads["LC3", "value"] = [0, -2.0, 0, 0, 0, 0]
-
-    gridparams = {
-        "size": (Lx, Ly, Lz),
-        "shape": (nx, ny, nz),
-        "origo": (0, 0, 0),
-        "start": 0,
-    }
-
-    coords, topo = grid(**gridparams)
-    coords, topo = H8_to_L2(coords, topo)
-
-    GlobalFrame = StandardFrame(dim=3)
-
-    points = PointCloud(coords, frame=GlobalFrame).centralize()
-    dx = -np.array([points[:, 0].min(), 0.0, 0.0])
-    points.move(dx)
-    coords = points.show()
-
-    section = BeamSection("CHS", d=d, t=t, n=16)
-    section.calculate_section_properties()
-    section_props = section.section_properties
-    A, Ix, Iy, Iz = getallfromkwargs(["A", "Ix", "Iy", "Iz"], **section_props)
-
-    G = Ex / (2 * (1 + nu))
-    Hooke = np.array(
-        [[Ex * A, 0, 0, 0], [0, G * Ix, 0, 0], [0, 0, Ex * Iy, 0], [0, 0, 0, Ex * Iz]]
-    )
-
-    # essential boundary conditions
-    ebcinds = np.where(coords[:, 0] < 1e-12)[0]
-    fixity = np.zeros((coords.shape[0], 6)).astype(bool)
-    fixity[ebcinds, :] = True
-
-    # natural boundary conditions
-    nLoadCase = len(loads)
-    nodal_loads = np.zeros((coords.shape[0], 6, nLoadCase))
-    for iLC, key in enumerate(loads):
-        x = loads[key]["position"]
-        f = loads[key]["value"]
-        iN = index_of_closest_point(coords, np.array(x))
-        loads[key]["node"] = iN
-        nodal_loads[iN, :, iLC] = f
-
-    # pointdata
-    pd = PointData(coords=coords, frame=GlobalFrame, loads=nodal_loads, fixity=fixity)
-
-    # celldata
-    frames = frames_of_lines(coords, topo)
-    cd = Beam(topo=topo, frames=frames)
-
-    # set up mesh and structure
-    mesh = LineMesh(pd, cd, model=Hooke, frame=GlobalFrame)
-    structure = Structure(mesh=mesh)
-
-    return structure
+# -*- coding: utf-8 -*-
+import numpy as np
+from linkeddeepdict import LinkedDeepDict
+from linkeddeepdict.tools import getallfromkwargs
+
+from polymesh.space import StandardFrame, PointCloud
+from polymesh.grid import gridH8 as grid
+from polymesh.topo.tr import H8_to_L2
+from polymesh.space import frames_of_lines
+from polymesh.space.utils import index_of_closest_point
+
+from sigmaepsilon.solid import BeamSection
+from sigmaepsilon.solid import Structure, LineMesh, PointData
+from sigmaepsilon.solid.fem.cells import B2 as Beam
+
+
+def console_grid_bernoulli() -> Structure:
+    """
+    Returns a simple console as a grid of 2-noded Bernoulli beams.
+
+    Example
+    -------
+    >>> from sigmaepsilon.examples import console_grid_bernoulli
+    >>> structure = console_grid_bernoulli()
+    >>> structure.linsolve()
+
+    """
+    # units in kN and cm
+
+    Lx, Ly, Lz = 100., 15., 10.  # size of the grid
+    nx, ny, nz = 4, 2, 2  # desity of the grid
+
+    d = 1.2  # outer diameter of the tube
+    t = 0.4  # thickness of the tube
+
+    Ex = 21000.0
+    nu = 0.25
+    fy = 35.0
+
+    loads = LinkedDeepDict()
+
+    # load case 1
+    loads['LC1', 'position'] = [Lx, 0, 0]
+    loads['LC1', 'value'] = [0, 0, 2.0, 0, 0, 0]
+
+    # load case 2
+    loads['LC2', 'position'] = [Lx, Ly/2, 0]
+    loads['LC2', 'value'] = [0, 2.0, 0, 0, 0, 0]
+
+    # load case 3
+    loads['LC3', 'position'] = [Lx, -Ly/2, 0]
+    loads['LC3', 'value'] = [0, -2.0, 0, 0, 0, 0]
+
+    gridparams = {
+        'size': (Lx, Ly, Lz),
+        'shape': (nx, ny, nz),
+        'origo': (0, 0, 0),
+        'start': 0
+    }
+
+    coords, topo = grid(**gridparams)
+    coords, topo = H8_to_L2(coords, topo)
+
+    GlobalFrame = StandardFrame(dim=3)
+
+    points = PointCloud(coords, frame=GlobalFrame).centralize()
+    dx = - np.array([points[:, 0].min(), 0., 0.])
+    points.move(dx)
+    coords = points.show()
+
+    section = BeamSection('CHS', d=d, t=t, n=16)
+    section.calculate_section_properties()
+    section_props = section.section_properties
+    A, Ix, Iy, Iz = getallfromkwargs(['A', 'Ix', 'Iy', 'Iz'],
+                                     **section_props)
+
+    G = Ex / (2 * (1 + nu))
+    Hooke = np.array([
+        [Ex*A, 0, 0, 0],
+        [0, G*Ix, 0, 0],
+        [0, 0, Ex*Iy, 0],
+        [0, 0, 0, Ex*Iz]
+    ])
+
+    # essential boundary conditions
+    ebcinds = np.where(coords[:, 0] < 1e-12)[0]
+    fixity = np.zeros((coords.shape[0], 6)).astype(bool)
+    fixity[ebcinds, :] = True
+
+    # natural boundary conditions
+    nLoadCase = len(loads)
+    nodal_loads = np.zeros((coords.shape[0], 6, nLoadCase))
+    for iLC, key in enumerate(loads):
+        x = loads[key]['position']
+        f = loads[key]['value']
+        iN = index_of_closest_point(coords, np.array(x))
+        loads[key]['node'] = iN
+        nodal_loads[iN, :, iLC] = f
+
+    # pointdata
+    pd = PointData(coords=coords, frame=GlobalFrame,
+                   loads=nodal_loads, fixity=fixity)
+
+    # celldata
+    frames = frames_of_lines(coords, topo)
+    cd = Beam(topo=topo, frames=frames)
+
+    # set up mesh and structure
+    mesh = LineMesh(pd, cd, model=Hooke, frame=GlobalFrame)
+    structure = Structure(mesh=mesh)
+
+    return structure
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/Q5V.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/fem/cells/Q5V.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,247 +1,246 @@
-import numpy as np
-from numpy import ndarray
-from numba import njit, prange
-
-from polymesh.cells import Q9 as Quadrilateral
-from polymesh.utils.tri import area_tri, glob_to_nat_tri, loc_to_nat_tri
-from polymesh.utils import nodal_distribution_factors
-
-from .elem import FiniteElement
-from ..material.membrane import Membrane
-from ...utils.fem.fem import topo_to_gnum
-
-
-__cache = True
-
-
-__all__ = ["Q5MV"]
-
-
-topoT2 = np.array(
-    [[0, 1, 3, 4, 8, 7], [1, 2, 3, 5, 6, 8], [0, 1, 2, 4, 5, 8], [0, 2, 3, 8, 6, 7]]
-)
-ndfT2 = nodal_distribution_factors(topoT2, np.ones(4))
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def dofmapT2():
-    """Returns the indices of dofs in each subtriangle relative
-    to the index array of active nodes `activeT2`."""
-    topoT2a = np.array([[0, 4, 3], [1, 2, 4], [0, 1, 4], [4, 2, 3]])
-    res = np.zeros((4, 6), dtype=np.int64)
-    for i in prange(4):
-        for j in prange(3):
-            for k in prange(2):
-                res[i, j * 2 + k] = topoT2a[i, j] * 2 + k
-    return res
-
-
-@njit(nogil=True, cache=__cache)
-def Turner_to_Veubeke():
-    """Transformation matrix of nodal variables in the
-    direction Turner -> Veubeke."""
-    return (
-        np.array(
-            [
-                [1, 0, 1, 0, 0, 0],
-                [0, 1, 0, 1, 0, 0],
-                [0, 0, 1, 0, 1, 0],
-                [0, 0, 0, 1, 0, 1],
-                [1, 0, 0, 0, 1, 0],
-                [0, 1, 0, 0, 0, 1],
-            ]
-        )
-        / 2
-    )
-
-
-@njit(nogil=True, cache=__cache)
-def shp_Veubeke_a(acoord: np.ndarray):
-    A1, A2, A3 = acoord
-    return np.array([A1 + A2 - A3, -A1 + A2 + A3, A1 - A2 + A3], dtype=acoord.dtype)
-
-
-@njit(nogil=True, cache=__cache)
-def shp_Veubeke_g(gcoord: np.ndarray, ecoords: np.ndarray):
-    return shp_Veubeke_a(glob_to_nat_tri(gcoord, ecoords))
-
-
-@njit(nogil=True, cache=__cache)
-def shp_Veubeke_p(pcoord: np.ndarray):
-    return shp_Veubeke_a(loc_to_nat_tri(pcoord))
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def nodal_approximation_matrix_V6():
-    """Returns a matrix of nodal approximation coefficients.
-    The coefficients in the ith row describe the approximation
-    at node i as a linear combination of values at every node.
-    At a compatible element, this is an identity matrix."""
-    pcoords = np.array(
-        [[0.0, 0.0], [1.0, 0.0], [0.0, 1.0], [0.5, 0.0], [0.5, 0.5], [0.0, 0.5]]
-    )
-    res = np.zeros((6, 6), dtype=pcoords.dtype)
-    for i in prange(6):
-        res[i, 3:] = shp_Veubeke_p(pcoords[i])
-    return res
-
-
-@njit(nogil=True, parallel=False, fastmath=True, cache=__cache)
-def nodal_approximation_matrix_T2():
-    """Returns a matrix of nodal approximation coefficients
-    for the T2 variant, for the whole element."""
-    nshpV6 = nodal_approximation_matrix_V6()
-    res = np.zeros((9, 9), dtype=nshpV6.dtype)
-    for iE in prange(4):
-        for iN in prange(6):
-            i = topoT2[iE, iN]
-            ndf = ndfT2[iE, iN]
-            for jN in prange(6):
-                j = topoT2[iE, jN]
-                res[i, j] += nshpV6[iN, jN] * ndf
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def nodal_approximation_matrix_T2_bulk(ndf: ndarray):
-    """Returns a matrix of nodal approximation coefficients for all elements."""
-    nE = ndf.shape[0]
-    nappr = nodal_approximation_matrix_T2()
-    res = np.zeros((nE, 9, 9), dtype=nappr.dtype)
-    for iE in prange(nE):
-        for i in prange(9):
-            for j in prange(9):
-                res[iE, i, j] = nappr[i, j] * ndf[iE, i]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def approximation_matrix_T2_bulk(ndf: ndarray):
-    """Returns a matrix of approximation coefficients for all elements."""
-    nE = ndf.shape[0]
-    nappr = nodal_approximation_matrix_T2()
-    res = np.zeros((nE, 18, 18), dtype=nappr.dtype)
-    for iE in prange(nE):
-        for i in prange(9):
-            for j in prange(9):
-                for ii in prange(2):
-                    for jj in prange(2):
-                        res[iE, i * 2 + ii, j * 2 + jj] = nappr[i, j] * ndf[iE, i]
-    return res
-
-
-@njit(nogil=True, cache=__cache)
-def _stiffness_matrix_V_(C: ndarray, ecoords: ndarray):
-    (x1, x2, x3), (y1, y2, y3) = ecoords[:, 0], ecoords[:, 1]
-    x12, x31, x23 = x1 - x2, x3 - x1, x2 - x3
-    y21, y13, y32 = y2 - y1, y1 - y3, y3 - y2
-    A = area_tri(ecoords)
-    B = np.zeros((3, 6), dtype=C.dtype)
-    B[0, :] = np.array([y21, 0, y32, 0, y13, 0], dtype=C.dtype)
-    B[1, :] = np.array([0, x12, 0, x23, 0, x31], dtype=C.dtype)
-    B[2, :] = np.array([x12, y21, x23, y32, x31, y13], dtype=C.dtype)
-    return B.T @ C @ B / A
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def stiffness_matrix_V(C: np.ndarray, ecoords: np.ndarray):
-    nE = len(C)
-    res = np.zeros((nE, 6, 6), dtype=C.dtype)
-    for i in prange(nE):
-        res[i, :, :] = _stiffness_matrix_V_(C[i], ecoords[i])
-    return res
-
-
-@njit(nogil=True, parallel=False, fastmath=True, cache=__cache)
-def stiffness_matrix_T2(C: ndarray, ecoords: ndarray):
-    nE = len(C)
-    dmapT2 = dofmapT2()
-    res = np.zeros((nE, 10, 10), dtype=C.dtype)
-    C = C / 2
-    for i in prange(4):
-        Ki = stiffness_matrix_V(C, ecoords[:, topoT2[i, :3], :])
-        for j in prange(6):
-            for k in prange(6):
-                res[:, dmapT2[i, j], dmapT2[i, k]] += Ki[:, j, k]
-    return res
-
-
-@njit(nogil=True, parallel=False, fastmath=True, cache=__cache)
-def transfer_passive_loads_T2(cellloadsT2: ndarray):
-    """(2) Transforms loads on passive nodes to active nodes
-    according to the transformation described by `Turner_to_Veubeke`."""
-    nE = cellloadsT2.shape[0]
-    res = np.zeros_like(cellloadsT2)
-    T_to_V = Turner_to_Veubeke()
-    for iE in prange(nE):
-        for iSE in prange(4):
-            loads_Turner = np.ravel(cellloadsT2[iE, iSE, :3, :])
-            loads_Veubeke = T_to_V @ loads_Turner
-            loads_Veubeke = np.reshape(loads_Veubeke, (3, 2))
-            for i in prange(3, 6):
-                for j in prange(2):
-                    res[iE, iSE, i, j] += cellloadsT2[iE, iSE, i, j]
-                    res[iE, iSE, i, j] += loads_Veubeke[i - 3, j]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def distribute_nodal_data_T2(celldata: ndarray):
-    """(1) Distributes master element data to subelement level."""
-    nE, _, nD = celldata.shape
-    res = np.zeros((nE, 4, 6, nD))
-    for iE in prange(nE):
-        for iSE in prange(4):
-            for iSNE in prange(6):
-                res[iE, iSE, iSNE] = celldata[iE, topoT2[iSE, iSNE]] * ndfT2[iSE, iSNE]
-    return res
-
-
-@njit(nogil=True, parallel=False, fastmath=True, cache=__cache)
-def collect_nodal_dataT2(celldataT2: ndarray):
-    """(3) Collects master element data from subelement level."""
-    nE, _, _, nD = celldataT2.shape
-    res = np.zeros((nE, 9, nD), dtype=celldataT2.dtype)
-    for iE in prange(nE):
-        for iSE in prange(4):
-            for iNSE in prange(6):
-                res[iE, topoT2[iSE, iNSE]] += celldataT2[iE, iSE, iNSE]
-    return res
-
-
-@njit(nogil=True, cache=__cache)
-def nodal_data_T2(celldata: ndarray):
-    """
-    Handles loads defined on passive nodes in 3 steps:
-    (1) Distribute master element data further to subelement level.
-    (2) On every subelement, transforms passive loads to uniform
-        body loads and integrates to active nodes.
-    (3) Collects master element data from subelement level.
-    """
-    celldataT2 = distribute_nodal_data_T2(celldata)
-    celldataT2 = transfer_passive_loads_T2(celldataT2)
-    return collect_nodal_dataT2(celldataT2)
-
-
-class Q5MV(Quadrilateral, Membrane, FiniteElement):
-    def stiffness_matrix(self, *args, topo=None, **kwargs):
-        topo = self.nodes.to_numpy() if topo is None else topo
-        ecoords = self.local_coordinates(topo=topo)
-        C = self.model_stiffness_matrix()
-        return stiffness_matrix_T2(C, ecoords)
-
-    def global_dof_numbering(self, *args, topo=None, **kwargs):
-        topo = self.nodes.to_numpy() if topo is None else topo
-        return topo_to_gnum(topo[:, 4:], self.NDOFN)
-
-    def distribute_nodal_data(self, data, key):
-        super().distribute_nodal_data(data, key)
-        if key == "loads":
-            celldata = self._wrapped["loads"].to_numpy()
-            self._wrapped["loads"] = nodal_data_T2(celldata)
-
-    def approximation_matrix(self, *args, **kwargs):
-        return approximation_matrix_T2_bulk(self.ndf.to_numpy())
-
-    def nodal_approximation_matrix(self, *args, **kwargs):
-        return nodal_approximation_matrix_T2_bulk(self.ndf.to_numpy())
+# -*- coding: utf-8 -*-
+import numpy as np
+from numpy import ndarray
+from numba import njit, prange
+
+from polymesh.cells import Q9 as Quadrilateral
+from polymesh.tri.triutils import area_tri, glob_to_nat_tri, loc_to_nat_tri
+from polymesh.utils import nodal_distribution_factors
+
+from ....solid.fem.cells import FiniteElement
+from ....solid.fem.model.membrane import Membrane
+from ....solid.fem.utils import topo_to_gnum
+
+
+__cache = True
+
+
+__all__ = ['Q5MV']
+
+
+topoT2 = np.array([[0, 1, 3, 4, 8, 7], [1, 2, 3, 5, 6, 8],
+                   [0, 1, 2, 4, 5, 8], [0, 2, 3, 8, 6, 7]])
+ndfT2 = nodal_distribution_factors(topoT2, np.ones(4))
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def dofmapT2():
+    """Returns the indices of dofs in each subtriangle relative
+    to the index array of active nodes `activeT2`."""
+    topoT2a = np.array([[0, 4, 3], [1, 2, 4],
+                        [0, 1, 4], [4, 2, 3]])
+    res = np.zeros((4, 6), dtype=np.int64)
+    for i in prange(4):
+        for j in prange(3):
+            for k in prange(2):
+                res[i, j*2 + k] = topoT2a[i, j]*2 + k
+    return res
+
+
+@njit(nogil=True, cache=__cache)
+def Turner_to_Veubeke():
+    """Transformation matrix of nodal variables in the 
+    direction Turner -> Veubeke."""
+    return np.array([[1, 0, 1, 0, 0, 0],
+                     [0, 1, 0, 1, 0, 0],
+                     [0, 0, 1, 0, 1, 0],
+                     [0, 0, 0, 1, 0, 1],
+                     [1, 0, 0, 0, 1, 0],
+                     [0, 1, 0, 0, 0, 1]]) / 2
+
+
+@njit(nogil=True, cache=__cache)
+def shp_Veubeke_a(acoord: np.ndarray):
+    A1, A2, A3 = acoord
+    return np.array([A1 + A2 - A3, -A1 + A2 + A3, A1 - A2 + A3],
+                    dtype=acoord.dtype)
+
+
+@njit(nogil=True, cache=__cache)
+def shp_Veubeke_g(gcoord: np.ndarray, ecoords: np.ndarray):
+    return shp_Veubeke_a(glob_to_nat_tri(gcoord, ecoords))
+
+
+@njit(nogil=True, cache=__cache)
+def shp_Veubeke_p(pcoord: np.ndarray):
+    return shp_Veubeke_a(loc_to_nat_tri(pcoord))
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def nodal_approximation_matrix_V6():
+    """Returns a matrix of nodal approximation coefficients.
+    The coefficients in the ith row describe the approximation
+    at node i as a linear combination of values at every node.
+    At a compatible element, this is an identity matrix."""
+    pcoords = np.array([[0.0, 0.0], [1.0, 0.0], [0.0, 1.0],
+                        [0.5, 0.0], [0.5, 0.5], [0.0, 0.5]])
+    res = np.zeros((6, 6), dtype=pcoords.dtype)
+    for i in prange(6):
+        res[i, 3:] = shp_Veubeke_p(pcoords[i])
+    return res
+
+
+@njit(nogil=True, parallel=False, fastmath=True, cache=__cache)
+def nodal_approximation_matrix_T2():
+    """Returns a matrix of nodal approximation coefficients
+    for the T2 variant, for the whole element."""
+    nshpV6 = nodal_approximation_matrix_V6()
+    res = np.zeros((9, 9), dtype=nshpV6.dtype)
+    for iE in prange(4):
+        for iN in prange(6):
+            i = topoT2[iE, iN]
+            ndf = ndfT2[iE, iN]
+            for jN in prange(6):
+                j = topoT2[iE, jN]
+                res[i, j] += nshpV6[iN, jN] * ndf
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def nodal_approximation_matrix_T2_bulk(ndf: ndarray):
+    """Returns a matrix of nodal approximation coefficients for all elements."""
+    nE = ndf.shape[0]
+    nappr = nodal_approximation_matrix_T2()
+    res = np.zeros((nE, 9, 9), dtype=nappr.dtype)
+    for iE in prange(nE):
+        for i in prange(9):
+            for j in prange(9):
+                res[iE, i, j] = nappr[i, j] * ndf[iE, i]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def approximation_matrix_T2_bulk(ndf: ndarray):
+    """Returns a matrix of approximation coefficients for all elements."""
+    nE = ndf.shape[0]
+    nappr = nodal_approximation_matrix_T2()
+    res = np.zeros((nE, 18, 18), dtype=nappr.dtype)
+    for iE in prange(nE):
+        for i in prange(9):
+            for j in prange(9):
+                for ii in prange(2):
+                    for jj in prange(2):
+                        res[iE, i*2 + ii, j*2 + jj] = nappr[i, j] * ndf[iE, i]
+    return res
+             
+
+@njit(nogil=True, cache=__cache)
+def _stiffness_matrix_V_(C: ndarray, ecoords: ndarray):
+    (x1, x2, x3), (y1, y2, y3) = ecoords[:, 0], ecoords[:, 1]
+    x12, x31, x23 = x1 - x2, x3 - x1, x2 - x3
+    y21, y13, y32 = y2 - y1, y1 - y3, y3 - y2
+    A = area_tri(ecoords)
+    B = np.zeros((3, 6), dtype=C.dtype)
+    B[0, :] = np.array([y21, 0, y32, 0, y13, 0], dtype=C.dtype)
+    B[1, :] = np.array([0, x12, 0, x23, 0, x31], dtype=C.dtype)
+    B[2, :] = np.array([x12, y21, x23, y32, x31, y13], dtype=C.dtype)
+    return B.T @ C @ B / A
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def stiffness_matrix_V(C: np.ndarray, ecoords: np.ndarray):
+    nE = len(C)
+    res = np.zeros((nE, 6, 6), dtype=C.dtype)
+    for i in prange(nE):
+        res[i, :, :] = _stiffness_matrix_V_(C[i], ecoords[i])
+    return res
+
+
+@njit(nogil=True, parallel=False, fastmath=True, cache=__cache)
+def stiffness_matrix_T2(C: ndarray, ecoords: ndarray):
+    nE = len(C)
+    dmapT2 = dofmapT2()
+    res = np.zeros((nE, 10, 10), dtype=C.dtype)
+    C = C/2
+    for i in prange(4):
+        Ki = stiffness_matrix_V(C, ecoords[:, topoT2[i, :3], :])
+        for j in prange(6):
+            for k in prange(6):
+                res[:, dmapT2[i, j], dmapT2[i, k]] += Ki[:, j, k]
+    return res
+
+
+@njit(nogil=True, parallel=False, fastmath=True, cache=__cache)
+def transfer_passive_loads_T2(cellloadsT2: ndarray):
+    """(2) Transforms loads on passive nodes to active nodes
+    according to the transformation described by `Turner_to_Veubeke`."""
+    nE = cellloadsT2.shape[0]
+    res = np.zeros_like(cellloadsT2)
+    T_to_V = Turner_to_Veubeke()
+    for iE in prange(nE):
+        for iSE in prange(4):
+            loads_Turner = np.ravel(cellloadsT2[iE, iSE, :3, :])
+            loads_Veubeke = T_to_V @ loads_Turner
+            loads_Veubeke = np.reshape(loads_Veubeke, (3, 2))
+            for i in prange(3, 6):
+                for j in prange(2):
+                    res[iE, iSE, i, j] += cellloadsT2[iE, iSE, i, j]
+                    res[iE, iSE, i, j] += loads_Veubeke[i-3, j]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def distribute_nodal_data_T2(celldata: ndarray):
+    """(1) Distributes master element data to subelement level."""
+    nE, _, nD = celldata.shape
+    res = np.zeros((nE, 4, 6, nD))
+    for iE in prange(nE):
+        for iSE in prange(4):
+            for iSNE in prange(6):
+                res[iE, iSE, iSNE] = \
+                    celldata[iE, topoT2[iSE, iSNE]] * ndfT2[iSE, iSNE]
+    return res
+
+
+@njit(nogil=True, parallel=False, fastmath=True, cache=__cache)
+def collect_nodal_dataT2(celldataT2: ndarray):
+    """(3) Collects master element data from subelement level."""
+    nE, _, _, nD = celldataT2.shape
+    res = np.zeros((nE, 9, nD), dtype=celldataT2.dtype)
+    for iE in prange(nE):
+        for iSE in prange(4):
+            for iNSE in prange(6):
+                res[iE, topoT2[iSE, iNSE]] += celldataT2[iE, iSE, iNSE]
+    return res
+
+
+@njit(nogil=True, cache=__cache)
+def nodal_data_T2(celldata: ndarray):
+    """
+    Handles loads defined on passive nodes in 3 steps:
+    (1) Distribute master element data further to subelement level.
+    (2) On every subelement, transforms passive loads to uniform
+        body loads and integrates to active nodes.
+    (3) Collects master element data from subelement level.
+    """
+    celldataT2 = distribute_nodal_data_T2(celldata)
+    celldataT2 = transfer_passive_loads_T2(celldataT2)
+    return collect_nodal_dataT2(celldataT2)
+
+
+class Q5MV(Quadrilateral, Membrane, FiniteElement):
+
+    compatible = False
+
+    def stiffness_matrix(self, *args, topo=None, **kwargs):
+        topo = self.nodes.to_numpy() if topo is None else topo
+        ecoords = self.local_coordinates(topo=topo)
+        C = self.model_stiffness_matrix()
+        return stiffness_matrix_T2(C, ecoords)
+
+    def global_dof_numbering(self, *args, topo=None, **kwargs):
+        topo = self.nodes.to_numpy() if topo is None else topo
+        return topo_to_gnum(topo[:, 4:], self.NDOFN)
+
+    def distribute_nodal_data(self, data, key):
+        super().distribute_nodal_data(data, key)
+        if key == 'loads':
+            celldata = self._wrapped['loads'].to_numpy()
+            self._wrapped['loads'] = nodal_data_T2(celldata)
+                
+    def approximation_matrix(self, *args, **kwargs):
+        return approximation_matrix_T2_bulk(self.ndf.to_numpy())
+    
+    def nodal_approximation_matrix(self, *args, **kwargs):
+        return nodal_approximation_matrix_T2_bulk(self.ndf.to_numpy())
+
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/bernoulli.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/bernoulli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,380 +1,286 @@
-import numpy as np
-from numpy import ndarray
-from typing import Union, Callable, Iterable
-
-from scipy import interpolate
-
-from neumann import atleast1d, atleastnd, ascont
-from neumann.utils import to_range_1d
-
-from ...utils.fem.cells.bernoulli import (
-    shape_function_matrix_Bernoulli_bulk,
-    body_load_vector_Bernoulli,
-    global_shape_function_derivatives_Bernoulli_bulk as gdshpB,
-    lumped_mass_matrices_direct_Bernoulli as dlump,
-)
-
-from ...utils.fem.postproc import (
-    approx_element_solution_bulk,
-    calculate_internal_forces_bulk,
-)
-from ..material.beam import (
-    BernoulliBeam,
-    _postproc_bernoulli_internal_forces_H_,
-    _postproc_bernoulli_internal_forces_L_,
-)
-
-__all__ = ["BernoulliBase"]
-
-
-class BernoulliBase(BernoulliBeam):
-    """
-    Skeleton class for 1d finite elements, whose bending behaviour
-    is governed by the Bernoulli theory. The implementations covered
-    by this class are independent of the number of nodes of the cells.
-    Specification of an actual finite element consists of specifying class
-    level attributes only.
-
-    See Also
-    --------
-    :class:`~sigmaepsilon.fem.cells.bernoulli2.Bernoulli2`
-    :class:`~sigmaepsilon.fem.cells.bernoulli3.Bernoulli3`
-    """
-
-    qrule: str = None
-    quadrature: dict = None
-    shpfnc: Callable = None
-    dshpfnc: Callable = None
-    dshpfnc_geom: Callable = None
-
-    def shape_function_values(
-        self,
-        pcoords: Union[float, Iterable[float]],
-        *_,
-        rng: Iterable = None,
-        lengths: Iterable[float] = None,
-        **__,
-    ) -> ndarray:
-        """
-        Evaluates the shape functions at the points specified by 'pcoords'.
-
-        Parameters
-        ----------
-        pcoords : float or Iterable[float]
-            Locations of the evaluation points.
-        rng : Iterable, Optional
-            The range in which the locations ought to be understood,
-            typically [0, 1] or [-1, 1]. Default is [0, 1].
-        lengths : Iterable, Optional
-            The lengths of the beams in the block. Default is None.
-
-        Returns
-        -------
-        numpy.ndarray
-            The returned array has a shape of (nP, nNE=2, nDOF=6), where nP,
-            nNE and nDOF stand for the number of evaluation points, nodes
-            per element and number of degrees of freedom, respectively.
-        """
-        rng = np.array([-1, 1]) if rng is None else np.array(rng)
-        pcoords = atleast1d(np.array(pcoords))
-        pcoords = to_range_1d(pcoords, source=rng, target=[-1, 1])
-        lengths = self.lengths() if lengths is None else lengths
-        return self.__class__.shpfnc(pcoords, lengths).astype(float)
-
-    def shape_function_derivatives(
-        self,
-        pcoords: Union[float, Iterable[float]] = None,
-        *_,
-        rng: Iterable = None,
-        jac: ndarray = None,
-        dshp: ndarray = None,
-        lengths: Iterable[float] = None,
-        **__,
-    ) -> ndarray:
-        """
-        Evaluates the shape function derivatives (up to third) at the points specified
-        by 'pcoords'. The function either returns the derivatives on the master or the actual
-        element, depending on the inputs.
-
-        Valid combination of inputs are:
-
-            * 'pcoords' and optionally 'jac' : this can be used to calculate the derivatives
-              in both the global ('jac' is provided) and the master frame ('jac' is not provided).
-
-            * 'dshp' and 'jac' : this combination can only be used to return the derivatives
-              wrt. to the global frame.
-
-        Parameters
-        ----------
-        pcoords : float or Iterable, Optional
-            Locations of the evaluation points. Default is None.
-        rng : Iterable, Optional
-            The range in which the locations ought to be understood,
-            typically [0, 1] or [-1, 1]. Only if 'pcoords' is provided.
-            Default is [0, 1].
-        lengths : Iterable, Optional
-            The lengths of the beams in the block. Default is None.
-        jac : Iterable, Optional
-            The jacobian matrix as a float array of shape (nE, nP, 1, 1), evaluated for
-            each point in each cell. Default is None.
-        dshp : Iterable, Optional
-            The shape function derivatives of the master element as a float array of
-            shape (nP, nNE, nDOF=6, 3), evaluated at a 'nP' number of points.
-            Default is None.
-
-        Returns
-        -------
-        numpy.ndarray
-            The returned array has a shape of (nP, nNE=2, nDOF=6, 3), where nP, nNE and
-            nDOF stand for the number of evaluation points, nodes per element and number of
-            degrees of freedom, respectively. Number 3 refers to first, second and third
-            derivatives.
-
-        Notes
-        -----
-        The returned array is always 4 dimensional, even if there is only one
-        evaluation point.
-        """
-        if pcoords is not None:
-            lengths = self.lengths() if lengths is None else lengths
-            # calculate derivatives wrt. the parametric coordinates in the range [-1, 1]
-            pcoords = atleast1d(np.array(pcoords))
-            rng = np.array([-1.0, 1.0]) if rng is None else np.array(rng)
-            pcoords = to_range_1d(pcoords, source=rng, target=[-1.0, 1.0])
-            dshp = self.__class__.dshpfnc(pcoords, lengths)
-            if jac is None:
-                # return derivatives wrt. the master frame
-                return dshp.astype(float)
-            else:
-                # return derivatives wrt. the global frame
-                return gdshpB(dshp, jac).astype(float)
-        elif dshp is not None and jac is not None:
-            # return derivatives wrt. the local frame
-            return gdshpB(dshp, jac).astype(float)
-
-    def shape_function_matrix(
-        self,
-        pcoords: Union[float, Iterable[float]] = None,
-        *_,
-        rng: Iterable = None,
-        lengths: Iterable[float] = None,
-        **__,
-    ) -> ndarray:
-        """
-        Evaluates the shape function matrix at the points specified by 'pcoords'.
-
-        Parameters
-        ----------
-        pcoords : float or Iterable
-            Locations of the evaluation points.
-        rng : Iterable, Optional
-            The range in which the locations ought to be understood,
-            typically [0, 1] or [-1, 1]. Default is [0, 1].
-
-        Other Parameters
-        ----------------
-        These parameters are for advanced users and can be omitted.
-        They are here only to avoid repeated evaulation of common quantities.
-
-        lengths : Iterable, Optional
-            The lengths of the beams in the block. Default is None.
-
-        Returns
-        -------
-        numpy.ndarray
-            The returned array has a shape of (nE, nP, nDOF, nDOF * nNE), where nE, nP,
-            nNE and nDOF stand for the number of elements, evaluation points, nodes
-            per element and number of degrees of freedom respectively.
-
-        Notes
-        -----
-        The returned array is always 4 dimensional, even if there is only one
-        evaluation point.
-        """
-        pcoords = atleast1d(np.array(pcoords))
-        rng = np.array([-1.0, 1.0]) if rng is None else np.array(rng)
-        pcoords = to_range_1d(pcoords, source=rng, target=[-1, 1])
-        lengths = self.lengths() if lengths is None else lengths
-        dshp = self.__class__.dshpfnc(pcoords, lengths)
-        ecoords = self.local_coordinates()
-        jac = self.jacobian_matrix(dshp=dshp, ecoords=ecoords)
-        shp = self.shape_function_values(pcoords, rng=rng)
-        gdshp = self.shape_function_derivatives(jac=jac, dshp=dshp)
-        return shape_function_matrix_Bernoulli_bulk(shp, gdshp).astype(float)
-
-    def integrate_body_loads(self, values: ndarray) -> ndarray:
-        """
-        Returns nodal representation of body loads.
-
-        Parameters
-        ----------
-        values : numpy.ndarray
-            2d or 3d numpy float array of material densities of shape
-            (nE, nNE * nDOF, nRHS) or (nE, nNE * nDOF), where nE, nNE, nDOF and nRHS
-            stand for the number of elements, nodes per element, number of degrees
-            of freedom and number of load cases respectively.
-
-        Returns
-        -------
-        numpy.ndarray
-            An array of shape (nE, nNE * 6, nRHS).
-
-        Notes
-        -----
-        The returned array is always 3 dimensional, even if there is only one
-        load case.
-
-        See Also
-        --------
-        :func:`~body_load_vector_bulk`
-        """
-        values = atleastnd(values, 3, back=True).astype(float)
-        # (nE, nNE * nDOF, nRHS) -> (nE, nRHS, nNE * nDOF)
-        values = np.swapaxes(values, 1, 2)
-        values = ascont(values)
-        qpos, qweights = self.quadrature["full"]
-        rng = np.array([-1.0, 1.0])
-        shp = self.shape_function_values(qpos, rng=rng)
-        # (nP, nNE=2, nDOF=6)
-        dshp = self.shape_function_derivatives(qpos, rng=rng)
-        # (nP, nNE=2, nDOF=6, 3)
-        ecoords = self.local_coordinates()
-        jac = self.jacobian_matrix(dshp=dshp, ecoords=ecoords)
-        # (nE, nP, 1, 1)
-        djac = self.jacobian(jac=jac)  # (nE, nG)
-        gdshp = self.shape_function_derivatives(jac=jac, dshp=dshp)
-        # (nE, nP, nNE=2, nDOF=6, 3)
-        return body_load_vector_Bernoulli(values, shp, gdshp, djac, qweights)
-
-    def _internal_forces_H_(
-        self,
-        *_,
-        cells: Union[int, Iterable[int]] = None,
-        points: Union[float, Iterable] = None,  # [-1, 1]
-    ) -> ndarray:
-        shp = self.shape_function_values(points, rng=[-1, 1])[cells]
-        dshp = self.shape_function_derivatives(points, rng=[-1, 1])[cells]
-        ecoords = self.local_coordinates()[cells]
-        jac = self.jacobian_matrix(dshp=dshp, ecoords=ecoords)
-        # jac -> (nE, nP, 1, 1)
-        B = self.strain_displacement_matrix(shp=shp, dshp=dshp, jac=jac)
-        # B -> (nE, nP, nSTRE, nNODE * 6)
-
-        dofsol = self.dof_solution(flatten=True, cells=cells)
-        # dofsol -> (nE, nNE * nDOF, nRHS)
-        dofsol = ascont(np.swapaxes(dofsol, 1, 2))
-        # dofsol -> (nE, nRHS, nEVAB)
-        strains = approx_element_solution_bulk(dofsol, B)
-        # strains -> (nE, nRHS, nP, nSTRE)
-        strains -= self.kinetic_strains(points=points)[cells]
-        D = self.elastic_material_stiffness_matrix()[cells]
-        forces = calculate_internal_forces_bulk(strains, D)
-        # forces -> (nE, nRHS, nP, nSTRE)
-        forces = ascont(np.moveaxis(forces, 1, -1))
-        dofsol = ascont(np.swapaxes(dofsol, 1, 2))
-        # dofsol -> (nE, nEVAB, nRHS)
-        # forces -> (nE, nP, nSTRE, nRHS)
-        gdshp = self.shape_function_derivatives(jac=jac, dshp=dshp)
-        nE, _, nRHS = dofsol.shape
-        nNE, nDOF = self.__class__.NNODE, self.__class__.NDOFN
-        dofsol = dofsol.reshape(nE, nNE, nDOF, nRHS)
-        D = self.elastic_material_stiffness_matrix()[cells]
-        forces = _postproc_bernoulli_internal_forces_H_(dofsol, forces, D, gdshp)
-        return forces  # (nE, nP, 6, nRHS)
-
-    def _internal_forces_L_(
-        self,
-        *_,
-        cells: Union[int, Iterable[int]] = None,
-        points: Union[float, Iterable] = None,  # [-1, 1]
-    ) -> ndarray:
-        local_points = np.array(self.lcoords()).flatten()
-
-        shp = self.shape_function_values(local_points, rng=[-1, 1])[cells]
-        dshp = self.shape_function_derivatives(local_points, rng=[-1, 1])[cells]
-        ecoords = self.local_coordinates()[cells]
-        jac = self.jacobian_matrix(dshp=dshp, ecoords=ecoords)
-        # jac -> (nE, nNE, 1, 1)
-        B = self.strain_displacement_matrix(shp=shp, dshp=dshp, jac=jac)
-        # B -> (nE, nNE, nSTRE, nNODE * 6)
-
-        dofsol = self.dof_solution(flatten=True, cells=cells)
-        # dofsol -> (nE, nNE * nDOF, nRHS)
-        dofsol = ascont(np.swapaxes(dofsol, 1, 2))
-        # dofsol -> (nE, nRHS, nEVAB)
-        strains = approx_element_solution_bulk(dofsol, B)
-        # strains -> (nE, nRHS, nNE, nSTRE)
-        strains -= self.kinetic_strains(points=local_points)[cells]
-        D = self.elastic_material_stiffness_matrix()[cells]
-
-        nE, nRHS, nP = strains.shape[:3]
-        forces = np.zeros((nE, nRHS, nP, 6), dtype=float)
-        inds = np.array([0, 3, 4, 5], dtype=int)
-        calculate_internal_forces_bulk(strains, D, forces, inds)
-        # forces -> (nE, nRHS, nNE, nSTRE)
-        forces = np.moveaxis(forces, 1, -1)
-        # forces -> (nE, nNE, nSTRE, nRHS)
-
-        *_, dshpf = self.Geometry.generate_class_functions(update=False, return_symbolic=False)
-        dshp_geom = np.squeeze(dshpf([[i] for i in local_points]))
-        # dshp_geom -> (nNE, nNE)
-        _postproc_bernoulli_internal_forces_L_(forces, dshp_geom, jac)
-        # forces -> (nE, nNE, nSTRE, nRHS)
-
-        if isinstance(points, Iterable):
-            approx = interpolate.interp1d(
-                local_points, forces, axis=1, assume_sorted=True
-            )
-            forces = approx(points)
-
-        return ascont(forces)
-
-    def _internal_forces_(self, *args, **kwargs):
-        return self._internal_forces_L_(self, *args, **kwargs)
-        # return self._internal_forces_H_(self, *args, **kwargs)
-
-    def lumped_mass_matrix(
-        self,
-        *_,
-        lumping: str = "direct",
-        alpha: float = 1 / 50,
-        frmt: str = "full",
-        **__,
-    ) -> ndarray:
-        """
-        Returns the lumped mass matrix of the block.
-
-        Parameters
-        ----------
-        alpha: float, Optional
-            A nonnegative parameter, typically between 0 and 1/50 (see notes).
-            Default is 1/20.
-        lumping: str, Optional
-            Controls lumping. Currently only direct lumping is available.
-            Default is 'direct'.
-        frmt: str, Optional
-            Possible values are 'full' or 'diag'. If 'diag', only the diagonal
-            entries are returned, if 'full' a full matrix is returned.
-            Default is 'full'.
-        """
-        dbkey = self.__class__._attr_map_["M"]
-        if lumping == "direct":
-            dens = self.db.density
-            try:
-                areas = self.areas()
-            except Exception:
-                areas = np.ones_like(dens)
-            lengths = self.lengths()
-            topo = self.topology()
-            ediags = dlump(dens, lengths, areas, topo, alpha)
-            if frmt == "full":
-                N = ediags.shape[-1]
-                M = np.zeros((ediags.shape[0], N, N))
-                inds = np.arange(N)
-                M[:, inds, inds] = ediags
-                self.db[dbkey] = M
-                return M
-            elif frmt == "diag":
-                self.db[dbkey] = ediags
-                return ediags
-        raise RuntimeError("Lumping mode not recognized :(")
+# -*- coding: utf-8 -*-
+import numpy as np
+from numpy import ndarray
+from collections import Iterable
+from typing import Union, Callable
+
+from neumann import squeeze, is_none_or_false
+from neumann.array import atleast1d, atleastnd, ascont
+from neumann.utils import to_range
+
+from .utils.bernoulli import (
+    shape_function_matrix_bulk, body_load_vector_bulk,
+    global_shape_function_derivatives_bulk as gdshpB,
+    lumped_mass_matrices_direct as dlump
+)
+
+from .meta import MetaFiniteElement
+from ..model.beam import BernoulliBeam, calculate_shear_forces
+
+
+__all__ = ['BernoulliBase']
+
+
+ArrayOrFloat = Union[ndarray, float]
+
+
+class MetaBernoulli(MetaFiniteElement):
+    """
+    Python metaclass for safe inheritance. Throws a TypeError
+    if a method tries to shadow a definition in any of the base
+    classes.
+    """
+
+    def __init__(self, name, bases, namespace, *args, **kwargs):
+        super().__init__(name, bases, namespace, *args, **kwargs)
+
+    def __new__(metaclass, name, bases, namespace, *args, **kwargs):
+        cls = super().__new__(metaclass, name, bases, namespace, *args, **kwargs)
+
+        if hasattr(cls, 'shpfnc'):
+            if cls.shpfnc is None and isinstance(cls.NNODE, int):
+                # generate functions
+                N = cls.NNODE
+
+    @classmethod
+    def generate_functions(cls, N):
+        pass
+
+
+class ABCBernoulli(metaclass=MetaBernoulli):
+    """
+    Helper class.
+    """
+    __slots__ = ()
+    dofs = ()
+    dofmap = ()
+
+
+class BernoulliBase(BernoulliBeam):
+    """
+    Skeleton class for 1d finite elements, whose bending behaviour
+    is governed by the Bernoulli theory. The implementations covered
+    by this class are independent of the number of nodes of the cells.
+    Specification of an actual finite element consists of specifying class
+    level attributes only.
+
+    See Also
+    --------
+    :class:`sigmaepsilon.solid.fem.cells.bernoulli2.Bernoulli2`
+    :class:`sigmaepsilon.solid.fem.cells.bernoulli3.Bernoulli3`
+
+    Note
+    ----
+    Among normal circumstances, you do not have to interact with this class 
+    directly. Only use it if you know what you are doing and understand the 
+    meaning of the inputs precisely.
+
+    """
+
+    qrule: str = None
+    quadrature: dict = None
+    shpfnc: Callable = None
+    dshpfnc: Callable = None
+
+    def shape_function_values(self, pcoords: ArrayOrFloat, *args,
+                              rng: Iterable = None, lengths: Iterable = None,
+                              **kwargs) -> ndarray:
+        """
+        Evaluates the shape functions at the points specified by 'pcoords'.
+
+        Parameters
+        ----------
+        pcoords : float or Iterable
+            Locations of the evaluation points.
+
+        rng : Iterable, Optional
+            The range in which the locations ought to be understood, 
+            typically [0, 1] or [-1, 1]. Default is [0, 1].
+
+        Other Parameters
+        ----------------
+        These parameters are for advanced users and can be omitted.
+        They are here only to avoid repeated evaulation of common quantities.
+
+        lengths : Iterable, Optional
+            The lengths of the beams in the block. Default is None.
+
+        Returns
+        -------
+        numpy.ndarray
+            The returned array has a shape of (nE, nP, nNE=2, nDOF=6), where nE, nP, 
+            nNE and nDOF stand for the number of elements, evaluation points, nodes 
+            per element and number of degrees of freedom, respectively.
+
+        Notes
+        -----
+        The returned array is always 4 dimensional, even if there is only one 
+        evaluation point.
+
+        """
+        rng = np.array([-1, 1]) if rng is None else np.array(rng)
+        pcoords = atleast1d(np.array(pcoords) if isinstance(
+            pcoords, list) else pcoords)
+        pcoords = to_range(pcoords, source=rng, target=[-1, 1])
+        lengths = self.lengths() if lengths is None else lengths
+        return self.__class__.shpfnc(pcoords, lengths).astype(float)
+
+    def shape_function_derivatives(self, pcoords=None, *args, rng=None,
+                                   jac: ndarray = None, dshp: ndarray = None,
+                                   lengths=None, **kwargs) -> ndarray:
+        """
+        Evaluates the shape function derivatives (up to third) at the points specified 
+        by 'pcoords'. The function either returns the derivatives of the master element, 
+        or the actual element, depending on the inputs.
+
+        Valid combination of inputs are:
+
+        - 'pcoords' and optionally 'jac' : this can be used to calculate the derivatives
+        in both the local ('jac' is provided) and the parametric frame ('jac' is not provided).
+
+        - 'dshp' and 'jac' : this combination can only be used to return the derivatives
+        wrt. the local frame.
+
+        Parameters
+        ----------
+        pcoords : float or Iterable, Optional
+            Locations of the evaluation points. Default is None.
+
+        rng : Iterable, Optional
+            The range in which the locations ought to be understood, 
+            typically [0, 1] or [-1, 1]. Only if 'pcoords' is provided.
+            Default is [0, 1].
+
+        jac : Iterable, Optional
+            The jacobian matrix. Default is None.
+
+        dshp : Iterable, Optional
+            The shape function derivatives of the master element, readily evaluated
+            at a certain number of points. Default is None.
+
+        Other Parameters
+        ----------------
+        These parameters are for advanced users and can be omitted.
+        They are here only to avoid repeated evaulation of common quantities.
+
+        lengths : Iterable, Optional
+            The lengths of the beams in the block. Only if 'pcoords' is provided. 
+            Default is None.
+
+        Returns
+        -------
+        numpy.ndarray
+            The returned array has a shape of (nE, nP, nNE=2, nDOF=6, 3), where nE, 
+            nP, nNE and nDOF stand for the number of elements, evaluation points, nodes 
+            per element and number of degrees of freedom, respectively. Number 3 refers 
+            to first, second and third derivatives.
+
+        Notes
+        -----
+        The returned array is always 5 dimensional, even if there is only one 
+        evaluation point.
+
+        """
+        if pcoords is not None:
+            lengths = self.lengths() if lengths is None else lengths
+            # calculate derivatives wrt. the parametric coordinates in the range [-1, 1]
+            pcoords = atleast1d(np.array(pcoords) if isinstance(
+                pcoords, list) else pcoords)
+            rng = np.array([-1, 1]) if rng is None else np.array(rng)
+            pcoords = to_range(pcoords, source=rng, target=[-1, 1])
+            dshp = self.__class__.dshpfnc(pcoords, lengths)
+            # return derivatives wrt. the local frame if jacobian is provided, otherwise
+            # return derivatives wrt. the parametric coordinate in the range [-1, 1]
+            return dshp.astype(float) if jac is None else gdshpB(dshp, jac).astype(float)
+        elif dshp is not None and jac is not None:
+            # return derivatives wrt. the local frame
+            return gdshpB(dshp, jac).astype(float)
+
+    def shape_function_matrix(self, pcoords=None, *args, rng=None,
+                              lengths=None, **kwargs) -> ndarray:
+        """
+        (nE, nP, nDOF, nDOF * nNODE)
+        """
+        pcoords = atleast1d(np.array(pcoords) if isinstance(
+            pcoords, list) else pcoords)
+        rng = np.array([-1., 1.]) if rng is None else np.array(rng)
+        lengths = self.lengths() if lengths is None else lengths
+        shp = self.shape_function_values(pcoords, rng=rng, lengths=lengths)
+        gdshp = self.shape_function_derivatives(pcoords, *args, rng=rng,
+                                                lengths=lengths, **kwargs)
+        return shape_function_matrix_bulk(shp, gdshp).astype(float)
+
+    def integrate_body_loads(self, values: ndarray) -> ndarray:
+        """
+        values (nE, nNE * nDOF, nRHS)
+        """
+        values = atleastnd(values, 3, back=True)
+        # (nE, nNE * nDOF, nRHS) -> (nE, nRHS, nNE * nDOF)
+        values = np.swapaxes(values, 1, 2)
+        values = ascont(values)
+        qpos, qweights = self.quadrature['full']
+        rng = np.array([-1., 1.])
+        shp = self.shape_function_values(
+            qpos, rng=rng)  # (nE, nP, nNE=2, nDOF=6)
+        dshp = self.shape_function_derivatives(
+            qpos, rng=rng)  # (nE, nP, nNE=2, nDOF=6, 3)
+        ecoords = self.local_coordinates()
+        jac = self.jacobian_matrix(
+            dshp=dshp, ecoords=ecoords)  # (nE, nP, 1, 1)
+        djac = self.jacobian(jac=jac)  # (nE, nG)
+        gdshp = self.shape_function_derivatives(
+            qpos, rng=rng, jac=jac, dshp=dshp)  # (nE, nP, nNE=2, nDOF=6, 3)
+        return body_load_vector_bulk(values, shp, gdshp, djac, qweights).astype(float)
+
+    def _postproc_local_internal_forces(self, values: np.ndarray, *args,
+                                        rng, points, cells, dofsol, **kwargs):
+        """
+        Documentation is at the base element at '...solid\\fem\\elem.py'
+        values (nE, nP, 4, nRHS)
+        dofsol (nE, nEVAB, nRHS)
+        points (nP,)
+        (nE, nP, 6, nRHS) out
+        """
+        ecoords = self.local_coordinates()[cells]
+        dshp = self.shape_function_derivatives(points, rng=rng)[cells]
+        jac = self.jacobian_matrix(
+            dshp=dshp, ecoords=ecoords)  # (nE, nP, 1, 1)
+        gdshp = self.shape_function_derivatives(
+            points, rng=rng, jac=jac, dshp=dshp)
+        nE, nEVAB, nRHS = dofsol.shape
+        nNE, nDOF = self.__class__.NNODE, self.__class__.NDOFN
+        dofsol = dofsol.reshape(nE, nNE, nDOF, nRHS)
+        D = self.model_stiffness_matrix()[cells]
+        values = calculate_shear_forces(dofsol, values, D, gdshp)
+        return values  # (nE, nP, 6, nRHS)
+
+    @squeeze(True)
+    def consistent_mass_matrix(self, *args, lumping=None, alpha: float = 1/50,
+                               frmt='full', **kwargs):
+        """
+        lumping : 'direct', None or False
+        frmt : only if lumping is specified
+        """
+        dbkey = self.__class__._attr_map_['M']
+        if is_none_or_false(lumping):
+            return super().consistent_mass_matrix(*args, squeeze=False, **kwargs)
+        if lumping == 'direct':
+            dens = self.db.density
+            try:
+                areas = self.areas()
+            except Exception:
+                areas = np.ones_like(dens)
+            lengths = self.lengths()
+            topo = self.topology()
+            ediags = dlump(dens, lengths, areas, topo, alpha)
+            if frmt == 'full':
+                N = ediags.shape[-1]
+                M = np.zeros((ediags.shape[0], N, N))
+                inds = np.arange(N)
+                M[:, inds, inds] = ediags
+                self.db[dbkey] = M
+                return M
+            elif frmt == 'diag':
+                self.db[dbkey] = ediags
+                return ediags
+        raise RuntimeError("Lumping mode not recognized :(")
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/bernoulli2.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/bernoulli2.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-from polymesh.cells import L2 as Line
-from polymesh.utils.cells.gauss import Gauss_Legendre_Line_Grid
-
-from .bernoulli import BernoulliBase as Bernoulli
-from .gen.b2 import (
-    shape_function_values_bulk,
-    shape_function_derivatives_bulk,
-    shape_function_derivatives_multi_L,
-)
-
-from .elem import FiniteElement
-from .meta import ABCFiniteElement as ABC
-
-__all__ = ["Bernoulli2"]
-
-
-class Bernoulli2(ABC, Bernoulli, Line, FiniteElement):
-    """
-    Finite element class to handle 2-noded Bernoulli beams.
-    """
-
-    qrule = "full"
-    quadrature = {
-        "full": Gauss_Legendre_Line_Grid(2),
-        "selective": {(0, 1): "full", (2): "reduced"},
-        "reduced": Gauss_Legendre_Line_Grid(1),
-        "mass": Gauss_Legendre_Line_Grid(4),
-    }
-    shpfnc = shape_function_values_bulk
-    dshpfnc = shape_function_derivatives_bulk
-    dshpfnc_geom = shape_function_derivatives_multi_L
+# -*- coding: utf-8 -*-
+from neumann.numint import GaussPoints as Gauss
+from polymesh.cells import L2 as Line
+
+from .bernoulli import BernoulliBase as Bernoulli
+from .gen.b2 import shape_function_values_bulk as shpB2, \
+    shape_function_derivatives_bulk as dshpB2
+from .elem import FiniteElement
+from .meta import ABCFiniteElement as ABC
+
+__all__ = ['Bernoulli2']
+
+
+class Bernoulli2(ABC, Bernoulli, Line, FiniteElement):
+
+    qrule = 'full'
+    quadrature = {
+        'full': Gauss(2),
+        'selective': {
+            (0, 1): 'full',
+            (2): 'reduced'
+        },
+        'reduced': Gauss(1),
+        'mass' : Gauss(4)
+    }
+    shpfnc = shpB2
+    dshpfnc = dshpB2
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/fem/cells/meta.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/meta.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,207 +1,211 @@
-from typing import Iterable
-
-import numpy as np
-from numpy import ndarray
-
-from neumann import atleastnd
-from polymesh.abcdata import ABCMeta_MeshData
-from polymesh.cell import PolyCell
-
-from ..dofmap import DOF
-from ...utils.fem.fem import (
-    expand_shape_function_matrix_bulk,
-    element_dofmap_bulk,
-)
-
-
-class FemMixin:
-    dofs = ()
-    dofmap = ()
-
-    # optional
-    qrule: str = None
-    quadrature = None
-
-    # advanced settings
-    compatible = True
-
-    # must be reimplemented
-    NNODE: int = None  # number of nodes, normally inherited
-
-    # from the mesh object
-    # it affects sizing of all kinds of intermediate variables
-    # during calculations (eg. element transformation matrix)
-    NDOFN: int = None  # numper of dofs per node, normally
-
-    # inherited form the model object
-    NDIM: int = None  # number of geometrical dimensions,
-    # normally inherited from the mesh object
-
-    # inherited form the model object
-    NSTRE: int = None  # number of internal force components,
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    @property
-    def geometry(self):
-        pd, cd = self.pdb, self.db
-        return self.__class__.Geometry(pointdata=pd, celldata=cd)
-
-    @property
-    def pdb(self):
-        return self.pointdata
-
-    @property
-    def db(self):
-        return self._wrapped
-
-    def topology(self) -> ndarray:
-        raise NotImplementedError
-
-    # !TODO : this should be implemented at geometry
-    @classmethod
-    def lcoords(cls, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    # !TODO : this should be implemented at geometry
-    @classmethod
-    def lcenter(cls, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    def local_coordinates(self) -> ndarray:
-        # implemented at PolyCell
-        raise NotImplementedError
-
-    def points_of_cells(self) -> ndarray:
-        # implemented at PolyCell
-        raise NotImplementedError
-
-    # !TODO : this should be implemented at geometry
-    # !TODO : can be reimplemented if the element is not IsoP
-    def jacobian_matrix(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    # !TODO : this should be implemented at geometry
-    # !TODO : can be reimplemented if the element is not IsoP
-    def jacobian(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    # !TODO : this should be implemented at material
-    def strain_displacement_matrix(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    # !TODO : this should be implemented at geometry
-    def shape_function_values(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    # !TODO : this should be implemented at geometry
-    # !TODO : can be reimplemented if the element is not IsoP
-    def shape_function_matrix(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    # !TODO : this should be implemented at geometry
-    def shape_function_derivatives(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    # !TODO : this should be implemented at material
-    def elastic_material_stiffness_matrix(self) -> ndarray:
-        raise NotImplementedError
-
-    # !TODO : this should be implemented at material
-    def stresses_at_centers(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    # !TODO : this should be implemented at material
-    def stresses_at_cells_nodes(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    def direction_cosine_matrix(self) -> ndarray:
-        return None
-
-    def integrate_body_loads(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    def masses(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    def areas(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    def lengths(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    def volumes(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    def densities(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    def weights(self, *args, **kwargs) -> ndarray:
-        raise NotImplementedError
-
-    def dof_solution(self, *, cells: Iterable, flatten: bool) -> ndarray:
-        raise NotImplementedError
-
-    def kinetic_strains(self, *, cells: Iterable, points: Iterable) -> ndarray:
-        raise NotImplementedError
-
-
-class FemMaterial(FemMixin):
-    """
-    Base class for FEM material classes.
-    """
-
-
-class MetaFiniteElement(ABCMeta_MeshData):
-    """
-    Python metaclass for safe inheritance. Throws a TypeError
-    if a method tries to shadow a definition in any of the base
-    classes.
-    """
-
-    def __init__(self, name, bases, namespace, *args, **kwargs):
-        super().__init__(name, bases, namespace, *args, **kwargs)
-
-    def __new__(metaclass, name, bases, namespace, *args, **kwargs):
-        cls = super().__new__(metaclass, name, bases, namespace, *args, **kwargs)
-        for base in bases:
-            if issubclass(base, PolyCell):
-                cls.Geometry = base
-            if issubclass(base, FemMaterial):
-                if len(base.dofs) > 0:
-                    cls.Material = base
-                    cls.dofs = base.dofs
-                    cls.NDOFN = len(cls.dofs)
-                    cls.dofmap = np.array(DOF.dofmap(cls.dofs), dtype=int)
-        return cls
-
-
-class ABCFiniteElement(FemMixin, metaclass=MetaFiniteElement):
-    """
-    Helper class that provides a standard way to create an ABC using
-    inheritance.
-    """
-
-    __slots__ = ()
-    dofs = ()
-    dofmap = ()
-
-    def shape_function_matrix(self, *args, expand: bool = False, **kwargs):
-        N = super().shape_function_matrix(*args, **kwargs)
-        if expand:
-            constant_metric = len(N.shape) == 3
-            N = atleastnd(N, 4, front=True)
-            nDOFN = self.container.NDOFN
-            dofmap = self.__class__.dofmap
-            if len(dofmap) < nDOFN:
-                # the model has more dofs than the element
-                nE, nP, nX = N.shape[:3]
-                nTOTV = nDOFN * self.NNODE
-                # nE, nP, nX, nDOF * nNE
-                N_ = np.zeros((nE, nP, nX, nTOTV), dtype=float)
-                dofmap = element_dofmap_bulk(dofmap, nDOFN, self.NNODE)
-                N = expand_shape_function_matrix_bulk(N, N_, dofmap)
-            return N[0] if constant_metric else N
-        else:
-            return N
+# -*- coding: utf-8 -*-
+from abc import abstractmethod
+from inspect import signature, Parameter
+import numpy as np
+
+from polymesh.abc import ABCMeta_MeshData
+from polymesh.cell import PolyCell
+
+from copy import deepcopy
+from functools import partial
+from typing import Callable, Any
+
+
+dofs = ('UX', 'UY', 'UZ', 'ROTX', 'ROTY', 'ROTZ')
+dofmap = {d : i for i, d in enumerate(dofs)}
+
+
+class FemMixin:
+    
+    dofs = ()
+    dofmap = ()
+            
+    # optional
+    qrule: str = None
+    quadrature = None
+
+    # advanced settings
+    compatible = True
+    
+    # must be reimplemented
+    NNODE: int = None  # number of nodes, normally inherited
+
+    # from the mesh object
+    # it affects sizing of all kinds of intermediate variables
+    # during calculations (eg. element transformation matrix)
+    NDOFN: int = None  # numper of dofs per node, normally
+
+    # inherited form the model object
+    NDIM: int = None  # number of geometrical dimensions,
+    # normally inherited from the mesh object
+
+    # inherited form the model object
+    NSTRE: int = None  # number of internal force components,
+    
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+    
+    @property    
+    def geometry(self):
+        pd, cd = self.pdb, self.db 
+        return self.__class__.Geometry(pointdata=pd, celldata=cd)
+    
+    @property
+    def pdb(self):
+        return self.pointdata
+    
+    @property
+    def db(self):
+        return self._wrapped
+    
+    def topology(self):
+        raise NotImplementedError
+    
+    # !TODO : this should be implemented at geometry
+    @classmethod
+    def lcoords(cls, *args, **kwargs):
+        raise NotImplementedError
+
+    # !TODO : this should be implemented at geometry
+    @classmethod
+    def lcenter(cls, *args, **kwargs):
+        raise NotImplementedError
+    
+    def local_coordinates(self, *args, frames=None, _topo=None, **kwargs):
+        # implemented at PolyCell
+        raise NotImplementedError
+
+    def points_of_cells(self):
+        # implemented at PolyCell
+        raise NotImplementedError
+
+    # !TODO : this should be implemented at geometry
+    # !TODO : can be reimplemented if the element is not IsoP
+    def jacobian_matrix(self, *args, **kwargs):
+        raise NotImplementedError
+
+    # !TODO : this should be implemented at geometry
+    # !TODO : can be reimplemented if the element is not IsoP
+    def jacobian(self, *args, **kwargs):
+        raise NotImplementedError
+
+    # !TODO : this should be implemented at model
+    def strain_displacement_matrix(self, *args, **kwargs):
+        raise NotImplementedError
+
+    # !TODO : this should be implemented at geometry
+    def shape_function_values(self, *args, **kwargs):
+        raise NotImplementedError
+
+    # !TODO : this should be implemented at geometry
+    # !TODO : can be reimplemented if the element is not IsoP
+    def shape_function_matrix(self, *args, **kwargs):
+        raise NotImplementedError
+
+    # !TODO : this should be implemented at geometry
+    def shape_function_derivatives(self, *args, **kwargs):
+        raise NotImplementedError
+
+    # !TODO : this should be implemented at model
+    def model_stiffness_matrix(self, *args, **kwargs):
+        raise NotImplementedError
+
+    # !TODO : this should be implemented at model
+    def stresses_at_centers(self, *args, **kwargs):
+        raise NotImplementedError
+
+    # !TODO : this should be implemented at model
+    def stresses_at_cells_nodes(self, *args, **kwargs):
+        raise NotImplementedError
+
+    def direction_cosine_matrix(self):
+        return None
+    
+    def integrate_body_loads(self, *args, **kwargs):
+        raise NotImplementedError
+    
+    def masses(self, *args, **kwargs):
+        raise NotImplementedError
+    
+    def volumes(self, *args, **kwargs):
+        raise NotImplementedError
+    
+    def densities(self, *args, **kwargs):
+        raise NotImplementedError
+        
+    def weights(self, *args, **kwargs):
+        raise NotImplementedError
+    
+    def _postproc_local_internal_forces(self, forces, *args, points, rng, cells, **kwargs):
+        """
+        The aim of this function os to guarantee a standard shape of output, that contains
+        values for each of the 6 internal force compoents, irrespective of the kinematical
+        model being used.
+
+        Example use case : the Bernoulli beam element, where, as a consequence of the absence
+        of shear forces, there are only 4 internal force components, and the shear forces
+        must be calculated a-posteriori.
+
+        Parameters
+        ----------
+        forces : numpy array of shape (nE, nP, nSTRE, nRHS)
+            4d float array of internal forces for many elements, evaluation points,
+            and load cases. The number of force components (nSTRE) is dictated by the
+            reduced kinematical model (eg. 4 for the Bernoulli beam).
+
+        dofsol (nE, nEVAB, nRHS)
+
+        Notes
+        -----
+        Arguments are based on the reimplementation in the Bernoulli base element.
+        
+        Returns
+        -------
+        numpy.ndarray 
+            shape : (nE, nP, 6, nRHS)
+        
+        """
+        return forces
+    
+
+
+class FemModel(FemMixin):
+    ...
+        
+
+class FemModel1d(FemModel):
+    ...
+
+
+class MetaFiniteElement(ABCMeta_MeshData):
+    """
+    Python metaclass for safe inheritance. Throws a TypeError
+    if a method tries to shadow a definition in any of the base
+    classes.
+    """
+
+    def __init__(self, name, bases, namespace, *args, **kwargs):
+        super().__init__(name, bases, namespace, *args, **kwargs)
+
+    def __new__(metaclass, name, bases, namespace, *args, **kwargs):     
+        cls = super().__new__(metaclass, name, bases, namespace, *args, **kwargs)    
+        for base in bases:                
+            if issubclass(base, PolyCell):
+                cls.Geometry = base  
+            if issubclass(base, FemModel):
+                if len(base.dofs) > 0:
+                    cls.Model = base
+                    cls.dofs = base.dofs
+                    cls.NDOFN = len(cls.dofs)
+                    cls.dofmap = np.array([dofmap[d] for d in cls.dofs], dtype=int)
+        return cls
+    
+
+class ABCFiniteElement(metaclass=MetaFiniteElement):
+    """
+    Helper class that provides a standard way to create an ABC using
+    inheritance.
+    """
+    __slots__ = ()
+    dofs = ()
+    dofmap = ()
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/fem/material/membrane.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/membrane.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,100 @@
-from numba import njit, prange
-import numpy as np
-from numpy import ndarray
-
-from ...utils.material.hmh import HMH_M
-from .surface import Surface
-
-
-__cache = True
-
-
-__all__ = ["Membrane", "DrillingMembrane"]
-
-
-_NSTRE_ = 3
-_NDOFN_ = 2
-_NHOOKE_ = 3
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def strain_displacement_matrix(dshp: ndarray, jac: ndarray):
-    nE = jac.shape[0]
-    nP, nN = dshp.shape[:2]
-    nTOTV = nN * _NDOFN_
-    B = np.zeros((nE, nP, _NSTRE_, nTOTV), dtype=dshp.dtype)
-    for iE in prange(nE):
-        for iP in prange(nP):
-            gdshp = dshp[iP] @ np.linalg.inv(jac[iE, iP])
-            for i in prange(nN):
-                B[iE, iP, 0, 0 + i * _NDOFN_] = gdshp[i, 0]
-                B[iE, iP, 1, 1 + i * _NDOFN_] = gdshp[i, 1]
-                B[iE, iP, 2, 0 + i * _NDOFN_] = gdshp[i, 1]
-                B[iE, iP, 2, 1 + i * _NDOFN_] = gdshp[i, 0]
-    return B
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def material_strains(strns: ndarray, z: float):
-    nE, nP = strns.shape[:2]
-    res = np.zeros((nE, nP, _NHOOKE_), dtype=strns.dtype)
-    res[:, :, :3] = strns[:, :, :3]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def HMH(estrs: np.ndarray):
-    nE, nP = estrs.shape[:2]
-    res = np.zeros((nE, nP), dtype=estrs.dtype)
-    for iE in prange(nE):
-        for jNE in prange(nP):
-            res[iE, jNE] = HMH_M(estrs[iE, jNE])
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def model_stiffness_iso_homg(C: ndarray, t: ndarray):
-    res = np.zeros_like(C)
-    for i in prange(res.shape[0]):
-        res[i, :, :] = C[i, :, :] * t[i]
-    return res
-
-
-class Membrane(Surface):
-    dofs = ("UX", "UY")
-    strn = ("exx", "eyy", "exy")
-
-    NDOFN = _NDOFN_
-    NSTRE = _NSTRE_
-
-    @classmethod
-    def model_stiffness_matrix_iso_homg(cls, C, t, *args, **kwargs):
-        return model_stiffness_iso_homg(C, t)
-
-    @classmethod
-    def strain_displacement_matrix(cls, *args, dshp=None, jac=None, **kwargs):
-        return strain_displacement_matrix(dshp, jac)
-
-    @classmethod
-    def HMH(cls, data, *args, **kwargs):
-        return HMH(data)
-
-    @classmethod
-    def material_strains(cls, model_strains, z, t, *args, **kwargs):
-        return material_strains(model_strains, z)
-
-
-class DrillingMembrane(Membrane):
-    dofs = ("UX", "UY", "ROTZ")
-
-    NDOFN = 3
-    NSTRE = _NSTRE_
+# -*- coding: utf-8 -*-
+from numba import njit, prange
+import numpy as np
+from numpy import ndarray
+
+from ...material.utils import HMH_M
+from .surface import Surface
+
+
+__cache = True
+
+
+__all__ = ['Membrane', 'DrillingMembrane']
+
+
+_NSTRE_ = 3
+_NDOFN_ = 2
+_NHOOKE_ = 3
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def strain_displacement_matrix(dshp: ndarray, jac: ndarray):
+    nE = jac.shape[0]
+    nP, nN = dshp.shape[:2]
+    nTOTV = nN * _NDOFN_
+    B = np.zeros((nE, nP, _NSTRE_, nTOTV), dtype=dshp.dtype)
+    for iE in prange(nE):
+        for iP in prange(nP):
+            gdshp = dshp[iP] @ np.linalg.inv(jac[iE, iP])
+            for i in prange(nN):
+                B[iE, iP, 0, 0 + i*_NDOFN_] = gdshp[i, 0]
+                B[iE, iP, 1, 1 + i*_NDOFN_] = gdshp[i, 1]
+                B[iE, iP, 2, 0 + i*_NDOFN_] = gdshp[i, 1]
+                B[iE, iP, 2, 1 + i*_NDOFN_] = gdshp[i, 0]
+    return B
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def material_strains(strns: ndarray, z: float):
+    nE, nP = strns.shape[:2]
+    res = np.zeros((nE, nP, _NHOOKE_), dtype=strns.dtype)
+    res[:, :, :3] = strns[:, :, :3]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def HMH(estrs: np.ndarray):
+    nE, nP = estrs.shape[:2]
+    res = np.zeros((nE, nP), dtype=estrs.dtype)
+    for iE in prange(nE):
+        for jNE in prange(nP):
+            res[iE, jNE] = HMH_M(estrs[iE, jNE])
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def model_stiffness_iso_homg(C: ndarray, t: ndarray):
+    res = np.zeros_like(C)
+    for i in prange(res.shape[0]):
+        res[i, :, :] = C[i, :, :] * t[i]
+    return res
+
+
+class Membrane(Surface):
+    
+    dofs = ('UX', 'UY')
+    strn = ('exx', 'eyy', 'exy')
+    
+    NDOFN = _NDOFN_
+    NSTRE = _NSTRE_
+
+    @classmethod
+    def model_stiffness_matrix_iso_homg(cls, C, t, *args, **kwargs):
+        return model_stiffness_iso_homg(C, t)
+
+    @classmethod
+    def strain_displacement_matrix(cls, *args, dshp=None, jac=None, **kwargs):
+        return strain_displacement_matrix(dshp, jac)
+
+    @classmethod
+    def HMH(cls, data, *args, **kwargs):
+        return HMH(data)
+
+    @classmethod
+    def material_strains(cls, model_strains, z, t, *args, **kwargs):
+        return material_strains(model_strains, z)
+    
+
+class DrillingMembrane(Membrane):
+    
+    dofs = ('UX', 'UY', 'ROTZ')
+
+    NDOFN = 3
+    NSTRE = _NSTRE_
+    
+
+if __name__ == '__main__':
+    
+    print(Membrane.NDOFN)
+
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/fem/material/mindlinplate.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/plate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,94 +1,95 @@
-from numba import njit, prange
-import numpy as np
-from numpy import ndarray
-
-from ...utils.material.hmh import HMH_S
-
-from .surface import Surface
-
-
-__cache = True
-
-
-__all__ = ["MindlinPlate"]
-
-
-_NSTRE_ = 5
-_NDOFN_ = 3
-_NHOOKE_ = 5
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def strain_displacement_matrix(shp: ndarray, dshp: ndarray, jac: ndarray) -> ndarray:
-    nE = jac.shape[0]
-    nP, nN = dshp.shape[:2]
-    nTOTV = nN * _NDOFN_
-    B = np.zeros((nE, nP, _NSTRE_, nTOTV), dtype=dshp.dtype)
-    for iE in prange(nE):
-        for iP in prange(nP):
-            gdshp = dshp[iP] @ np.linalg.inv(jac[iE, iP])
-            for i in prange(nN):
-                B[iE, iP, 0, 2 + i * _NDOFN_] = gdshp[i, 0]
-                B[iE, iP, 1, 1 + i * _NDOFN_] = -gdshp[i, 1]
-                B[iE, iP, 2, 1 + i * _NDOFN_] = -gdshp[i, 0]
-                B[iE, iP, 2, 2 + i * _NDOFN_] = gdshp[i, 1]
-                B[iE, iP, 3, 0 + i * _NDOFN_] = gdshp[i, 0]
-                B[iE, iP, 3, 2 + i * _NDOFN_] = shp[iP, i]
-                B[iE, iP, 4, 0 + i * _NDOFN_] = gdshp[i, 1]
-                B[iE, iP, 4, 1 + i * _NDOFN_] = -shp[iP, i]
-    return B
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def material_strains(model_strains: ndarray, z: float, t: float) -> ndarray:
-    nE, nP = model_strains.shape[:2]
-    res = np.zeros((nE, nP, _NHOOKE_), dtype=model_strains.dtype)
-    res[:, :, :3] = model_strains[:, :, :3] * z
-    for i in prange(nE):
-        res[i, :, 3:] = (5 / 4) * (1 - 4 * (z / t[i]) ** 2) * model_strains[i, :, 3:]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def HMH(estrs: np.ndarray) -> ndarray:
-    nE, nP = estrs.shape[:2]
-    res = np.zeros((nE, nP), dtype=estrs.dtype)
-    for iE in prange(nE):
-        for jNE in prange(nP):
-            res[iE, jNE] = HMH_S(estrs[iE, jNE])
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def model_stiffness_iso_homg(C: ndarray, t: ndarray) -> ndarray:
-    res = np.zeros_like(C)
-    for i in prange(res.shape[0]):
-        res[i, :3, :3] = C[i, :3, :3] * (t[i] ** 3 / 12)
-        res[i, 3:, 3:] = C[i, 3:, 3:] * (t[i] * 5 / 6)
-    return res
-
-
-class MindlinPlate(Surface):
-    dofs = ("UZ", "ROTX", "ROTY")
-    strn = ("kxx", "kyy", "kxy" "exz", "eyz")
-
-    NDOFN = _NDOFN_
-    NSTRE = _NSTRE_
-
-    @classmethod
-    def model_stiffness_matrix_iso_homg(cls, C, t, *_, **__) -> ndarray:
-        return model_stiffness_iso_homg(C, t)
-
-    @classmethod
-    def strain_displacement_matrix(
-        cls, *_, shp=None, dshp=None, jac=None, **__
-    ) -> ndarray:
-        return strain_displacement_matrix(shp, dshp, jac)
-
-    @classmethod
-    def HMH(cls, data, *_, **__) -> ndarray:
-        return HMH(data)
-
-    @classmethod
-    def material_strains(cls, model_strains, z, t, *_, **__) -> ndarray:
-        return material_strains(model_strains, z, t)
+# -*- coding: utf-8 -*-
+from numba import njit, prange
+import numpy as np
+from numpy import ndarray
+
+from ...material.utils import HMH_S
+
+from .surface import Surface
+
+
+__cache = True
+
+
+__all__ = ['Plate']
+
+
+_NSTRE_ = 5
+_NDOFN_ = 3
+_NHOOKE_ = 5
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def strain_displacement_matrix(dshp: ndarray, jac: ndarray):
+    nE = jac.shape[0]
+    nP, nN = dshp.shape[:2]
+    nTOTV = nN * _NDOFN_
+    B = np.zeros((nE, nP, _NSTRE_, nTOTV), dtype=dshp.dtype)
+    for iE in prange(nE):
+        for iP in prange(nP):
+            gdshp = dshp[iP] @ np.linalg.inv(jac[iE, iP])
+            for i in prange(nN):
+                B[iE, iP, 0, 1 + i*_NDOFN_] = -gdshp[i, 0]
+                B[iE, iP, 1, 2 + i*_NDOFN_] = -gdshp[i, 1]
+                B[iE, iP, 2, 1 + i*_NDOFN_] = -gdshp[i, 1]
+                B[iE, iP, 2, 2 + i*_NDOFN_] = -gdshp[i, 0]
+                B[iE, iP, 3, 0 + i*_NDOFN_] = gdshp[i, 0]
+                B[iE, iP, 3, 1 + i*_NDOFN_] = -1
+                B[iE, iP, 4, 0 + i*_NDOFN_] = gdshp[i, 1]
+                B[iE, iP, 4, 2 + i*_NDOFN_] = -1
+    return B
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def material_strains(model_strains: ndarray, z: float, t: float):
+    nE, nP = model_strains.shape[:2]
+    res = np.zeros((nE, nP, _NHOOKE_), dtype=model_strains.dtype)
+    res[:, :, :3] = model_strains[:, :, :3] * z
+    for i in prange(nE):
+        res[i, :, 3:] = (5/4) * (1 - 4 * (z / t[i])**2) * \
+            model_strains[i, :, 3:]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def HMH(estrs: np.ndarray):
+    nE, nP = estrs.shape[:2]
+    res = np.zeros((nE, nP), dtype=estrs.dtype)
+    for iE in prange(nE):
+        for jNE in prange(nP):
+            res[iE, jNE] = HMH_S(estrs[iE, jNE])
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def model_stiffness_iso_homg(C: ndarray, t: ndarray):
+    res = np.zeros_like(C)
+    for i in prange(res.shape[0]):
+        res[i, :3, :3] = C[i, :3, :3] * (t[i]**3 / 12)
+        res[i, 3:, 3:] = C[i, 3:, 3:] * (t[i] * 5 / 6)
+    return res
+
+
+class Plate(Surface):
+    
+    dofs = ('UZ', 'ROTX', 'ROTY')
+    strn = ('kxx', 'kyy', 'kxy' 'exz', 'eyz')
+    
+    NDOFN = _NDOFN_
+    NSTRE = _NSTRE_
+
+    @classmethod
+    def model_stiffness_matrix_iso_homg(cls, C, t, *args, **kwargs):
+        return model_stiffness_iso_homg(C, t)
+
+    @classmethod
+    def strain_displacement_matrix(cls, *args, dshp=None, jac=None, **kwargs):
+        return strain_displacement_matrix(dshp, jac)
+
+    @classmethod
+    def HMH(cls, data, *args, **kwargs):
+        return HMH(data)
+
+    @classmethod
+    def material_strains(cls, model_strains, z, t, *args, **kwargs):
+        return material_strains(model_strains, z, t)
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/fem/material/solid.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/solid.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,70 +1,76 @@
-from numpy import ndarray
-
-from neumann import atleast2d, atleast3d
-
-from ...utils.material import model_strains, model_strains_multi, stresses_from_strains
-from ...utils.fem.fem import topo_to_gnum
-from ..cells.meta import FemMaterial
-
-
-__all__ = ["Solid"]
-
-
-class Solid(FemMaterial):
-    dofs = ("UX", "UY", "UZ")
-    strn = ("exx", "eyy", "ezz", "eyz", "exz", "exy")
-
-    NDOFN = 3
-    NSTRE = 6
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def elastic_material_stiffness_matrix(self) -> ndarray:
-        return self.material_stiffness
-
-    @classmethod
-    def HMH(cls, *args, **kwargs):
-        raise NotImplementedError
-
-    @classmethod
-    def model_strains(cls, dofsol1d, gnum, B, *args, **kwargs):
-        if len(dofsol1d.shape) == 2:
-            return model_strains_multi(dofsol1d, gnum, B)
-        return model_strains(dofsol1d, gnum, B)
-
-    def strains_at(self, lcoords, *args, z=None, topo=None, **kwargs):
-        topo = self.topology().to_numpy() if topo is None else topo
-        gnum = topo_to_gnum(topo, self.NDOFN)
-        lcoords = atleast2d(lcoords)
-        dshp = self.shape_function_derivatives(lcoords)
-        ecoords = self.local_coordinates(topo=topo)
-        jac = self.jacobian_matrix(dshp=dshp, ecoords=ecoords)
-        B = self.strain_displacement_matrix(dshp=dshp, jac=jac)
-        dofsol = self.pointdata.dofsol.to_numpy()
-        dofsol = atleast3d(dofsol, back=True)
-        return self.model_strains(dofsol, gnum, B)
-
-    def stresses_at(self, *args, z=None, topo=None, **kwargs):
-        """
-        Returns stresses for every node of every element.
-        """
-        # The next code line returns either generalized strains
-        # or material strains, depending on the value of z
-        strns = self.strains_at(*args, z=z, topo=topo, **kwargs)
-        C = self.elastic_material_stiffness_matrix()
-        if "HMH" in args:
-            return self.HMH(stresses_from_strains(C, strns))
-        return stresses_from_strains(C, strns)
-
-    def stresses_at_nodes(self, *args, **kwargs):
-        """
-        Returns stresses for every node of every element.
-        """
-        return self.stresses_at(self.lcoords(), *args, **kwargs)
-
-    def stresses_at_centers(self, *args, **kwargs):
-        """
-        Returns stresses at the centre of every element.
-        """
-        return self.stresses_at(self.lcenter(), *args, **kwargs)
+# -*- coding: utf-8 -*-
+from abc import abstractmethod
+
+from neumann.array import atleast2d, atleast3d
+
+from .utils import (model_strains, model_strains_multi,
+                    stresses_from_strains, stresses_from_strains_multi)
+from ..utils import topo_to_gnum
+from ..cells.meta import FemModel
+
+
+__all__ = ['Solid']
+
+
+class Solid(FemModel):
+    
+    dofs = ('UX', 'UY', 'UZ')
+    strn = ('exx', 'eyy', 'ezz', 'eyz', 'exz', 'exy')
+
+    NDOFN = 3
+    NSTRE = 6
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def material_stiffness_matrix(self, *args, **kwargs):
+        return self._wrapped.mat.to_numpy()
+
+    def model_stiffness_matrix(self, *args, **kwargs):
+        return self.material_stiffness_matrix()
+
+    @classmethod
+    def HMH(cls, *args,  **kwargs):
+        raise NotImplementedError
+
+    @classmethod
+    def model_strains(cls, dofsol1d, gnum, B, *args, **kwargs):
+        if len(dofsol1d.shape) == 2:
+            return model_strains_multi(dofsol1d, gnum, B)
+        return model_strains(dofsol1d, gnum, B)
+
+    def strains_at(self, lcoords, *args,  z=None, topo=None, **kwargs):
+        topo = self.topology().to_numpy() if topo is None else topo
+        gnum = topo_to_gnum(topo, self.NDOFN)
+        lcoords = atleast2d(lcoords)
+        dshp = self.shape_function_derivatives(lcoords)
+        ecoords = self.local_coordinates(topo=topo)
+        jac = self.jacobian_matrix(dshp=dshp, ecoords=ecoords)
+        B = self.strain_displacement_matrix(dshp=dshp, jac=jac)   
+        dofsol = self.pointdata.dofsol.to_numpy()
+        dofsol = atleast3d(dofsol, back=True)  
+        return self.model_strains(dofsol, gnum, B)
+
+    def stresses_at(self, *args, z=None, topo=None, **kwargs):
+        """
+        Returns stresses for every node of every element.
+        """
+        # The next code line returns either generalized strains
+        # or material strains, depending on the value of z
+        strns = self.strains_at(*args, z=z, topo=topo, **kwargs)
+        C = self.model_stiffness_matrix()
+        if 'HMH' in args:
+            return self.HMH(stresses_from_strains(C, strns))
+        return stresses_from_strains(C, strns)
+
+    def stresses_at_nodes(self, *args, **kwargs):
+        """
+        Returns stresses for every node of every element.
+        """
+        return self.stresses_at(self.lcoords(), *args, **kwargs)
+
+    def stresses_at_centers(self, *args, **kwargs):
+        """
+        Returns stresses at the centre of every element.
+        """
+        return self.stresses_at(self.lcenter(), *args, **kwargs)
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/fem/material/solid3d.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/beam.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,118 +1,132 @@
-from numba import njit, prange
-import numpy as np
-from numpy import ndarray
-
-from .solid import Solid
-from ...utils.material.hmh import HMH_3d
-
-__cache = True
-
-
-__all__ = ["Solid3d"]
-
-
-_NSTRE_ = 6
-_NDOFN_ = 3
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def strain_displacement_matrix(dshp: ndarray, jac: ndarray) -> ndarray:
-    # sxx, syy, szz, syz, sxz, sxy
-    nE = jac.shape[0]
-    nP, nN = dshp.shape[:2]
-    nTOTV = nN * _NDOFN_
-    B = np.zeros((nE, nP, _NSTRE_, nTOTV), dtype=dshp.dtype)
-    for iE in prange(nE):
-        for iP in prange(nP):
-            gdshp = dshp[iP] @ np.linalg.inv(jac[iE, iP]).T
-            for i in prange(nN):
-                B[iE, iP, 0, 0 + i * _NDOFN_] = gdshp[i, 0]
-                B[iE, iP, 1, 1 + i * _NDOFN_] = gdshp[i, 1]
-                B[iE, iP, 2, 2 + i * _NDOFN_] = gdshp[i, 2]
-                B[iE, iP, 3, 1 + i * _NDOFN_] = gdshp[i, 2]
-                B[iE, iP, 3, 2 + i * _NDOFN_] = gdshp[i, 1]
-                B[iE, iP, 4, 0 + i * _NDOFN_] = gdshp[i, 2]
-                B[iE, iP, 4, 2 + i * _NDOFN_] = gdshp[i, 0]
-                B[iE, iP, 5, 0 + i * _NDOFN_] = gdshp[i, 1]
-                B[iE, iP, 5, 1 + i * _NDOFN_] = gdshp[i, 0]
-    return B
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def HMH_3d_bulk_multi(estrs: np.ndarray) -> ndarray:
-    nE, nP = estrs.shape[:2]
-    res = np.zeros((nE, nP), dtype=estrs.dtype)
-    for iE in prange(nE):
-        for jNE in prange(nP):
-            res[iE, jNE] = HMH_3d(estrs[iE, jNE])
-    return res
-
-
-class Solid3d(Solid):
-    """
-    A model for 3d solids.
-
-    See Also
-    --------
-    :class:`sigmaepsilon.fem.model.solid.Solid`
-    """
-
-    dofs = ("UX", "UY", "UZ")
-
-    NDOFN = 3
-    NSTRE = 6
-
-    def strain_displacement_matrix(
-        self, pcoords: ndarray = None, *, dshp: ndarray = None, jac: ndarray = None, **_
-    ) -> ndarray:
-        """
-        Calculates the strain displacement matrix for solids.
-
-        Parameters
-        ----------
-        pcoords : numpy.ndarray, Optional
-            Locations of evaluation points. Either 'pcoords' or
-            both 'dshp' and 'jac' must be provided.
-        dshp : numpy.ndarray, Optional
-            Shape function derivatives evaluated at some points.
-            Only required if 'pcoords' is not provided.
-        jac : numpy.ndarray
-            Jacobian matrices evaluated at some points.
-            Only required if 'pcoords' is not provided.
-
-        Returns
-        -------
-        numpy.ndarray
-            An array of shape (nE, nP, nSTRE, nTOTV), where nE, nP
-            nSTRE and nTOTV are the number of elements, evaulation
-            points, stress components and total DOFs per element.
-        """
-        if dshp is None and pcoords is not None:
-            dshp = self.shape_function_derivatives(pcoords)
-        if jac is None:
-            jac = self.jacobian_matrix(dshp=dshp)
-        return strain_displacement_matrix(dshp, jac)
-
-    @classmethod
-    def HMH(cls, stresses: ndarray) -> ndarray:
-        """
-        Evaluates the Huber-Mises-Hencky stress at multiple points
-        of multiple cells.
-
-        s11, s22, s33, s12, s13, s23
-
-        Parameters
-        ----------
-        stresses : numpy.ndarray, Optional
-            Array of shape (nE, nP, nSTRE), where nE, nP and nSTRE
-            are the number of elements, evaulation points and stress
-            components. The stresses are expected in the order
-            s11, s22, s33, s12, s13, s23.
-
-        Returns
-        -------
-        numpy.ndarray
-            An array of shape (nE, nP), where nE and nP are the
-            number of elements and evaulation points.
-        """
-        return HMH_3d_bulk_multi(stresses)
+# -*- coding: utf-8 -*-
+from numba import njit, prange
+import numpy as np
+from numpy import ndarray
+from typing import Union
+
+from .solid import Solid
+
+__cache = True
+
+ArrayOrFloat = Union[ndarray, float]
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def strain_displacement_matrix(gdshp: ndarray):
+    """
+    Returns the matrix expressing the relationship of generalized strains
+        0 : strain along x
+        1 : curvature around x
+        2 : curvature around y
+        3 : curvature around z
+    and generalized displacements of a Bernoulli beam element.
+
+    Parameters
+    ----------
+    gdshp : numpy float array of shape (N, 6, 3)  
+        First, second and third derivatives for every dof(6) of every node(N).
+
+    Returns
+    -------
+    numpy array of shape (4, N * 6) 
+        Apprpximation coefficients for every generalized strain and every 
+        shape function.
+    """
+    nNE = gdshp.shape[0]
+    B = np.zeros((4, nNE * 6), dtype=gdshp.dtype)
+    for i in prange(nNE):
+        di = i * 6
+        # \epsilon_x
+        B[0, 0 + di] = gdshp[i, 0, 0]
+        # \kappa_x
+        B[1, 3 + di] = gdshp[i, 3, 0]
+        # \kappa_y
+        B[2, 2 + di] = -gdshp[i, 2, 1]
+        B[2, 4 + di] = -gdshp[i, 4, 1]
+        # \kappa_z
+        B[3, 1 + di] = gdshp[i, 1, 1]
+        B[3, 5 + di] = gdshp[i, 5, 1]
+    return B
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def strain_displacement_matrix_bulk(gdshp: ndarray):
+    """
+    Parameters
+    ----------
+    gdshp : numpy.ndarray
+        Numpy float array of shape (nE, nP, nNE, nDOF=6, 3)
+
+    Returns
+    -------
+    numpy.ndarray
+        NumPy float array of shape (nE, nP, 4, nNODE * 6)
+
+    """
+    nE, nP, nNE = gdshp.shape[:3]
+    B = np.zeros((nE, nP, 4, nNE * 6), dtype=gdshp.dtype)
+    for iE in prange(nE):
+        for iP in prange(nP):
+            B[iE, iP] = strain_displacement_matrix(gdshp[iE, iP])
+    return B
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def calculate_shear_forces(dofsol: ndarray, forces: ndarray,
+                           D: ndarray, gdshp: ndarray):
+    # dofsol (nE, nNE, nDOF=6, nRHS)
+    # forces (nE, nP, 4, nRHS)
+    # gdshp (nE, nP, nNE=2, nDOF=6, 3)
+    nE, nP, _, nRHS = forces.shape
+    nNE = dofsol.shape[1]
+    res = np.zeros((nE, nP, 6, nRHS), dtype=forces.dtype)
+    res[:, :, 0, :] = forces[:, :, 0, :]
+    res[:, :, 3, :] = forces[:, :, 1, :]
+    res[:, :, 4, :] = forces[:, :, 2, :]
+    res[:, :, 5, :] = forces[:, :, 3, :]
+    for i in prange(nE):
+        for j in prange(nP):
+            for k in prange(nRHS):
+                for m in range(nNE):
+                    # Vy
+                    res[i, j, 1, k] += - D[i, 3, 3] * (
+                        gdshp[i, j, m, 1, 2] * dofsol[i, m, 1, k] +
+                        gdshp[i, j, m, 5, 2] * dofsol[i, m, 5, k])
+                    # Vz
+                    res[i, j, 2, k] += - D[i, 2, 2] * (
+                        gdshp[i, j, m, 2, 2] * dofsol[i, m, 2, k] +
+                        gdshp[i, j, m, 4, 2] * dofsol[i, m, 4, k])
+    return res
+
+
+class BernoulliBeam(Solid):
+
+    dofs = ('UX', 'UY', 'UZ', 'ROTX', 'ROTY', 'ROTZ')
+
+    NDOFN = 6
+    NSTRE = 4
+
+    def model_stiffness_matrix(self, *args, **kwargs):
+        return self.material_stiffness_matrix()
+
+    def strain_displacement_matrix(self, pcoords: ArrayOrFloat = None, *args,
+                                   jac=None, rng=None, dshp=None, **kwargs):
+        rng = np.array([-1, 1]) if rng is None else np.array(rng)
+        gdshp = self.shape_function_derivatives(
+            pcoords, rng=rng, jac=jac, dshp=dshp)
+        return strain_displacement_matrix_bulk(gdshp)
+
+    def masses(self, *args, values=None, **kwargs):
+        if isinstance(values, np.ndarray):
+            dens = values
+        else:
+            dens = self.db.density
+        try:
+            areas = self.areas()
+        except Exception:
+            areas = np.ones_like(dens)
+        lengths = self.lengths()
+        return areas * dens * lengths
+
+    def mass(self, *args, **kwargs):
+        return np.sum(self.masses(*args, **kwargs))
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/fem/material/surface.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/surface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,71 @@
-from neumann import atleast2d, atleastnd
-
-from ...utils.material import stresses_from_strains
-from ...utils.fem.fem import topo_to_gnum
-from .solid import Solid
-
-
-class Surface(Solid):
-    strn = ("exx", "eyy", "exy", "kxx", "kyy", "kxy", "exz", "eyz")
-
-    def model_stiffness_matrix(self, *args, **kwargs):
-        C = self.material_stiffness_matrix()
-        t = self.thickness()
-        return self.model_stiffness_matrix_iso_homg(C, t)
-
-    @classmethod
-    def model_stiffness_matrix_iso_homg(cls, *args, **kwargs):
-        raise NotImplementedError
-
-    @classmethod
-    def material_strains(cls, *args, **kwargs):
-        raise NotImplementedError
-
-    def ABDS(self, *args, **kwargs):
-        return self.model_stiffness_matrix(*args, **kwargs)
-
-    def strains_at(self, lcoords, *args, z=None, topo=None, **kwargs):
-        if topo is None:
-            topo = self.topology().to_numpy()
-        lcoords = atleast2d(lcoords)
-        dshp = self.shape_function_derivatives(lcoords)
-        ecoords = self.local_coordinates(topo=topo)
-        jac = self.jacobian_matrix(dshp, ecoords)
-        gnum = topo_to_gnum(topo, self.NDOFN)
-
-        dofsol1d = self.pointdata.dofsol.to_numpy().flatten()
-
-        dofsol = self.pointdata.dofsol
-        dofsol = atleastnd(dofsol, 3, back=True)
-        nP, nDOF, nRHS = dofsol.shape
-        dofsol = dofsol.reshape(nP * nDOF, nRHS)
-
-        B = self.strain_displacement_matrix(dshp, jac)
-        if z is None:
-            # return generalized model strains
-            return self.model_strains(dofsol1d, gnum, B)
-        else:
-            # returns material strains
-            t = self.thickness()
-            model_strains = self.model_strains(dofsol1d, gnum, B)
-            return self.material_strains(model_strains, z, t)
-
-    def stresses_at(self, *args, z=None, topo=None, **kwargs):
-        """
-        Returns stresses for every node of every element.
-        """
-        # The next code line returns either generalized strains
-        # or material strains, depending on the value of z
-        strns = self.strains_at(*args, z=z, topo=topo, **kwargs)
-        if z is None:
-            C = self.model_stiffness_matrix()
-        else:
-            C = self.material_stiffness_matrix()
-        if "HMH" in args:
-            return self.HMH(stresses_from_strains(C, strns))
-        return stresses_from_strains(C, strns)
+# -*- coding: utf-8 -*-
+from neumann.array import atleast2d, atleastnd
+
+from ..utils import topo_to_gnum
+
+from .solid import Solid
+from .utils import stresses_from_strains
+
+
+class Surface(Solid):
+    
+    strn = ('exx', 'eyy', 'exy', 'kxx', 'kyy', 'kxy', 'exz', 'eyz')
+
+    def model_stiffness_matrix(self, *args, **kwargs):
+        C = self.material_stiffness_matrix()
+        t = self.thickness()
+        return self.model_stiffness_matrix_iso_homg(C, t)
+
+    @classmethod
+    def model_stiffness_matrix_iso_homg(cls, *args,  **kwargs):
+        raise NotImplementedError
+
+    @classmethod
+    def material_strains(cls, *args, **kwargs):
+        raise NotImplementedError
+
+    def ABDS(self, *args, **kwargs):
+        return self.model_stiffness_matrix(*args, **kwargs)
+
+    def strains_at(self, lcoords, *args,  z=None, topo=None, **kwargs):
+        if topo is None:
+            topo = self.topology().to_numpy()
+        lcoords = atleast2d(lcoords)
+        dshp = self.shape_function_derivatives(lcoords)
+        ecoords = self.local_coordinates(topo=topo)
+        jac = self.jacobian_matrix(dshp, ecoords)
+        gnum = topo_to_gnum(topo, self.NDOFN)
+        
+        
+        dofsol1d = self.pointdata.dofsol.to_numpy().flatten()
+        
+        dofsol = self.pointdata.dofsol
+        dofsol = atleastnd(dofsol, 3, back=True)
+        nP, nDOF, nRHS = dofsol.shape
+        dofsol = dofsol.reshape(nP * nDOF, nRHS)
+        
+        
+        B = self.strain_displacement_matrix(dshp, jac)
+        if z is None:
+            # return generalized model strains
+            return self.model_strains(dofsol1d, gnum, B)
+        else:
+            # returns material strains
+            t = self.thickness()
+            model_strains = self.model_strains(dofsol1d, gnum, B)
+            return self.material_strains(model_strains, z, t)
+
+    def stresses_at(self, *args, z=None, topo=None, **kwargs):
+        """
+        Returns stresses for every node of every element.
+        """
+        # The next code line returns either generalized strains
+        # or material strains, depending on the value of z
+        strns = self.strains_at(*args, z=z, topo=topo, **kwargs)
+        if z is None:
+            C = self.model_stiffness_matrix()
+        else:
+            C = self.material_stiffness_matrix()
+        if 'HMH' in args:
+            return self.HMH(stresses_from_strains(C, strns))
+        return stresses_from_strains(C, strns)
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/fem/pointdata.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/pointdata.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,229 +1,192 @@
-from typing import Callable
-
-import numpy as np
-from numpy import ndarray
-
-from neumann import atleastnd
-from polymesh.pointdata import PointData as MeshPointData
-
-
-class PointData(MeshPointData):
-    """
-    A subclass of :class:`polymesh.pointdata.PointData` to handle data related
-    to the pointcloud of a finite element mesh.
-
-    Parameters
-    ----------
-    fixity : numpy.ndarray, Optional
-        A 2d boolean or float array describing essential boundary conditions.
-        Default is None.
-    loads : numpy.ndarray, Optional
-        A 2d or 3d float array of nodal loads.
-        Default is None.
-    mass : numpy.ndarray, Optional
-        2d array of nodal masses for each degree of freedom of a node.
-        Default is None.
-    fields : dict, Optional
-        Every value of this dictionary is added to the dataset. Default is `None`.
-    **kwargs : dict, Optional
-        For every key and value pair where the value is a numpy array
-        with a matching shape (has entries for all points), the key
-        is considered as a field and the value is added to the database.
-
-    Examples
-    --------
-    We will define the point-related data of a simple linear console. At the
-    moment this means the specification of cordinates, nodal loads, and boundary
-    conditions. The common properties of these attributes is that each of these
-    can be best described by arrays having the same length as the pointcloud itself.
-    Import the necessary stuff:
-
-    >>> from sigmaepsilon import Structure, LineMesh, PointData
-    >>> from neumann.linalg import linspace, Vector
-    >>> from polymesh.space import StandardFrame, PointCloud, frames_of_lines
-    >>> import numpy as np
-
-    Define a coordinate frame, and a coordinate array,
-
-    >>> GlobalFrame = StandardFrame(dim=3)
-    >>> nElem = 20  # number of finite elements to use
-    >>> p0 = np.array([0., 0., 0.])
-    >>> p1 = np.array([L, 0., 0.])
-    >>> coords = linspace(p0, p1, nElem+1)
-    >>> coords = PointCloud(coords, frame=GlobalFrame).show()
-
-    two numpy arrays resembling the boundary conditions,
-
-    >>> # support at the leftmost, load at the rightmost node
-    >>> loads = np.zeros((coords.shape[0], 6))
-    >>> fixity = np.zeros((coords.shape[0], 6)).astype(bool)
-    >>> global_load_vector = Vector([0., 0, F], frame=GlobalFrame).show()
-    >>> loads[-1, :3] = global_load_vector
-    >>> fixity[0, :] = True
-
-    and finally we can define our dataset.
-
-    >>> pd = PointData(coords=coords, frame=GlobalFrame,
-    >>>                loads=loads, fixity=fixity)
-
-    See also
-    --------
-    :class:`sigmaepsilon.fem.cells.celldata.CellData`
-    :class:`polymesh.PolyData`
-    :class:`polymesh.CellData`
-    :class:`awkward.Record`
-    """
-
-    _attr_map_ = {
-        "loads": "loads",
-        "mass": "mass",
-        "fixity": "fixity",
-        "dofsol": "dofsol",
-        "shapes": "_shapes_",
-        "reactions": "reactions",
-        "forces": "forces",
-    }
-    NDOFN = 6
-
-    def __init__(
-        self,
-        *args,
-        fixity: ndarray = None,
-        loads: ndarray = None,
-        mass: ndarray = None,
-        fields: dict = None,
-        **kwargs
-    ):
-        amap = self.__class__._attr_map_
-
-        if fields is not None:
-            fixity = fields.pop(amap["fixity"], fixity)
-            loads = fields.pop(amap["loads"], loads)
-            mass = fields.pop(amap["mass"], mass)
-
-        super().__init__(*args, fields=fields, **kwargs)
-
-        if self.db is not None:
-            nP = len(self)
-            NDOFN = self.__class__.NDOFN
-
-            if fixity is None:
-                fixity = np.zeros((nP, NDOFN), dtype=bool)
-            else:
-                assert isinstance(fixity, np.ndarray) and len(fixity.shape) == 2
-            self.fixity = fixity
-
-            if loads is None:
-                loads = np.zeros((nP, NDOFN, 1))
-            if loads is not None:
-                assert isinstance(loads, np.ndarray)
-                if loads.shape[0] == nP:
-                    self.loads = loads
-                elif loads.shape[0] == nP * NDOFN:
-                    loads = atleastnd(loads, 2, back=True)
-                    self.loads = loads.reshape(nP, NDOFN, loads.shape[-1])
-
-            if mass is not None:
-                if isinstance(mass, float) or isinstance(mass, int):
-                    raise NotImplementedError
-                elif isinstance(mass, np.ndarray):
-                    self.mass = mass
-
-    @property
-    def _dbkey_fixity_(self) -> str:
-        return self.__class__._attr_map_["fixity"]
-
-    @property
-    def has_fixity(self):
-        return self._dbkey_fixity_ in self._wrapped.fields
-
-    @property
-    def fixity(self) -> ndarray:
-        """Returns fixity information as a 2d numpy array."""
-        return self._wrapped[self.__class__._attr_map_["fixity"]].to_numpy()
-
-    @fixity.setter
-    def fixity(self, value: ndarray):
-        """Sets essential boundary conditions."""
-        assert isinstance(value, ndarray)
-        self._wrapped[self.__class__._attr_map_["fixity"]] = value
-
-    @property
-    def loads(self) -> ndarray:
-        """Returns the nodal load vector."""
-        return self._wrapped[self.__class__._attr_map_["loads"]].to_numpy()
-
-    @loads.setter
-    def loads(self, value: ndarray):
-        """Sets the nodal load vector."""
-        assert isinstance(value, ndarray)
-        self._wrapped[self.__class__._attr_map_["loads"]] = value
-
-    @property
-    def mass(self) -> ndarray:
-        """Retruns nodal masses."""
-        return self._wrapped[self.__class__._attr_map_["mass"]].to_numpy()
-
-    @mass.setter
-    def mass(self, value: ndarray):
-        """Sets nodal masses."""
-        assert isinstance(value, ndarray)
-        self._wrapped[self.__class__._attr_map_["mass"]] = value
-
-    @property
-    def dofsol(self) -> ndarray:
-        """Returns the displacement vector."""
-        return self._wrapped[self.__class__._attr_map_["dofsol"]].to_numpy()
-
-    @dofsol.setter
-    def dofsol(self, value: ndarray):
-        assert isinstance(value, ndarray)
-        self._wrapped[self.__class__._attr_map_["dofsol"]] = value
-
-    @property
-    def vshapes(self) -> ndarray:
-        """Returns the modal shapes."""
-        return self._wrapped[self.__class__._attr_map_["shapes"]].to_numpy()
-
-    @vshapes.setter
-    def vshapes(self, value: ndarray):
-        assert isinstance(value, ndarray)
-        self._wrapped[self.__class__._attr_map_["shapes"]] = value
-
-    @property
-    def reactions(self) -> ndarray:
-        """Returns the vector of reaction forces."""
-        return self._wrapped[self.__class__._attr_map_["reactions"]].to_numpy()
-
-    @reactions.setter
-    def reactions(self, value: ndarray):
-        assert isinstance(value, ndarray)
-        self._wrapped[self.__class__._attr_map_["reactions"]] = value
-
-    @property
-    def forces(self) -> ndarray:
-        return self._wrapped[self.__class__._attr_map_["forces"]].to_numpy()
-
-    @forces.setter
-    def forces(self, value: ndarray):
-        assert isinstance(value, ndarray)
-        self._wrapped[self.__class__._attr_map_["forces"]] = value
-
-
-def flatten_pd(default=True):
-    def decorator(fnc: Callable):
-        def inner(*args, flatten: bool = default, **kwargs):
-            if flatten:
-                x = fnc(*args, **kwargs)
-                if len(x.shape) == 2:
-                    return x.flatten()
-                else:
-                    nN, nDOFN, nRHS = x.shape
-                    return x.reshape((nN * nDOFN, nRHS))
-            else:
-                return fnc(*args, **kwargs)
-
-        inner.__doc__ = fnc.__doc__
-        return inner
-
-    return decorator
+# -*- coding: utf-8 -*-
+import numpy as np
+from numpy import ndarray
+
+from neumann.array import atleastnd
+
+from polymesh.pointdata import PointData as MeshPointData
+
+
+class PointData(MeshPointData):
+    """
+    A subclass of :class:`polymesh.pointdata.PointData` to handle data related 
+    to the pointcloud of a finite element mesh.
+
+    Parameters
+    ----------
+    fixity : :class:`numpy.ndarray`, Optional
+        A 2d boolean or float array describing essential boundary conditions.
+        Default is None.
+        
+    loads : :class:`numpy.ndarray`, Optional
+        A 2d or 3d float array of nodal loads.
+        Default is None.
+        
+    mass : :class:`numpy.ndarray`, Optional
+        2d array of nodal masses for each degree of freedom of a node.
+        Default is None.
+        
+    fields : `dict`, Optional
+        Every value of this dictionary is added to the dataset. Default is `None`.
+        
+    **kwargs : dict, Optional
+        For every key and value pair where the value is a numpy array
+        with a matching shape (has entries for all points), the key
+        is considered as a field and the value is added to the database.
+        
+    Examples
+    --------
+    
+    We will define the point-related data of a simple linear console. At the
+    moment this means the specification of cordinates, nodal loads, and boundary 
+    conditions. The common properties of these attributes is that each of these
+    can be best described by arrays having the same length as the pointcloud itself.
+    Import the necessary stuff:
+    
+    >>> from sigmaepsilon.solid import Structure, LineMesh, PointData
+    >>> from neumann.linalg import linspace, Vector
+    >>> from polymesh.space import StandardFrame, PointCloud, frames_of_lines
+    >>> import numpy as np
+    
+    Define a coordinate frame, and a coordinate array,
+
+    >>> GlobalFrame = StandardFrame(dim=3)
+    >>> nElem = 20  # number of finite elements to use
+    >>> p0 = np.array([0., 0., 0.])
+    >>> p1 = np.array([L, 0., 0.])
+    >>> coords = linspace(p0, p1, nElem+1)
+    >>> coords = PointCloud(coords, frame=GlobalFrame).show()
+
+    two numpy arrays resembling the boundary conditions,
+
+    >>> # support at the leftmost, load at the rightmost node
+    >>> loads = np.zeros((coords.shape[0], 6))
+    >>> fixity = np.zeros((coords.shape[0], 6)).astype(bool)
+    >>> global_load_vector = Vector([0., 0, F], frame=GlobalFrame).show()
+    >>> loads[-1, :3] = global_load_vector
+    >>> fixity[0, :] = True
+
+    and finally we can define our dataset.  
+
+    >>> pd = PointData(coords=coords, frame=GlobalFrame, 
+    >>>                loads=loads, fixity=fixity)
+
+    See also
+    --------
+    :class:`sigmaepsilon.solid.fem.cells.celldata.CellData`
+    :class:`polymesh.PolyData`
+    :class:`polymesh.CellData`
+    :class:`awkward.Record`
+    
+    """
+
+    _attr_map_ = {
+        'loads': 'loads',
+        'mass': 'mass',
+        'fixity': 'fixity',
+        'dofsol' : 'dofsol',
+        'reactions' : 'reactions',
+        'forces' : 'forces',
+    }
+    NDOFN = 6
+
+    def __init__(self, *args, fixity=None, loads=None, mass=None,
+                 fields=None, **kwargs):
+        amap = self.__class__._attr_map_
+
+        if fields is not None:
+            fixity = fields.pop(amap['fixity'], fixity)
+            loads = fields.pop(amap['loads'], loads)
+            mass = fields.pop(amap['mass'], mass)
+
+        super().__init__(*args, fields=fields, **kwargs)
+
+        if self.db is not None:
+            nP = len(self)
+            NDOFN = self.__class__.NDOFN
+
+            if fixity is None:
+                fixity = np.zeros((nP, NDOFN), dtype=bool)
+            else:
+                assert isinstance(fixity, np.ndarray) and len(
+                    fixity.shape) == 2
+            self.fixity = fixity
+
+            if loads is None:
+                loads = np.zeros((nP, NDOFN, 1))
+            if loads is not None:
+                assert isinstance(loads, np.ndarray)
+                if loads.shape[0] == nP:
+                    self.loads = loads
+                elif loads.shape[0] == nP * NDOFN:
+                    loads = atleastnd(loads, 2, back=True)
+                    self.loads = loads.reshape(nP, NDOFN, loads.shape[-1])
+
+            if mass is not None:
+                if isinstance(mass, float) or isinstance(mass, int):
+                    raise NotImplementedError
+                elif isinstance(mass, np.ndarray):
+                    self.mass = mass
+
+    @property
+    def fixity(self) -> ndarray:
+        """Returns fixity information as a 2d numpy array."""
+        return self._wrapped[self.__class__._attr_map_['fixity']].to_numpy()
+
+    @fixity.setter
+    def fixity(self, value: ndarray):
+        """Sets essential boundary conditions."""
+        assert isinstance(value, ndarray)
+        self._wrapped[self.__class__._attr_map_['fixity']] = value
+
+    @property
+    def loads(self) -> ndarray:
+        """Returns the nodal load vector."""
+        return self._wrapped[self.__class__._attr_map_['loads']].to_numpy()
+
+    @loads.setter
+    def loads(self, value: ndarray):
+        """Sets the nodal load vector."""
+        assert isinstance(value, ndarray)
+        self._wrapped[self.__class__._attr_map_['loads']] = value
+        
+    @property
+    def mass(self) -> ndarray:
+        """Retruns nodal masses."""
+        return self._wrapped[self.__class__._attr_map_['mass']].to_numpy()
+
+    @mass.setter
+    def mass(self, value: ndarray):
+        """Sets nodal masses."""
+        assert isinstance(value, ndarray)
+        self._wrapped[self.__class__._attr_map_['mass']] = value
+        
+    @property
+    def dofsol(self) -> ndarray:
+        """Returns the displacement vector."""
+        return self._wrapped[self.__class__._attr_map_['dofsol']].to_numpy()
+
+    @dofsol.setter
+    def dofsol(self, value: ndarray):
+        assert isinstance(value, ndarray)
+        self._wrapped[self.__class__._attr_map_['dofsol']] = value 
+        
+    @property
+    def reactions(self) -> ndarray:
+        """Returns the vector of reaction forces."""
+        return self._wrapped[self.__class__._attr_map_['reactions']].to_numpy()
+
+    @reactions.setter
+    def reactions(self, value: ndarray):
+        assert isinstance(value, ndarray)
+        self._wrapped[self.__class__._attr_map_['reactions']] = value   
+        
+    @property
+    def forces(self) -> ndarray:
+        return self._wrapped[self.__class__._attr_map_['forces']].to_numpy()
+
+    @forces.setter
+    def forces(self, value: ndarray):
+        assert isinstance(value, ndarray)
+        self._wrapped[self.__class__._attr_map_['forces']] = value    
+
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/fem/structure.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/mesh.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,601 +1,495 @@
-from typing import Tuple, Union, List
-
-import numpy as np
-from numpy import ndarray
-from scipy.sparse import coo_matrix
-
-from neumann import repeat
-
-from .mesh import FemMesh
-from .ebc import EssentialBoundaryCondition as EBC
-from .femsolver import StaticSolver, DynamicSolver
-from ..utils.fem.preproc import assemble_load_vector
-from ..utils.fem.tr import tr_element_matrices_bulk, tr_nodal_loads_bulk
-from ..utils.fem.dyn import effective_modal_masses, Rayleigh_quotient
-from .pointdata import flatten_pd
-from .constants import DEFAULT_DIRICHLET_PENALTY, DEFAULT_MASS_PENALTY_RATIO
-
-
-__all__ = ["Structure"]
-
-
-class Structure:
-    """
-    A higher level class to manage solid structures.
-
-    Parameters
-    ----------
-    mesh : FemMesh, Optional
-        A finite element mesh.
-    essential_penalty : float, Optional
-        Penalty parameter for the Courant penalty function used to enforce
-        Dirichlet (essential) boundary conditions. If not provided, a default
-        value of `~sigmaepsilon.fem.constants.DEFAULT_DIRICHLET_PENALTY`
-        is used.
-    mass_penalty_ratio : float, Optional
-        Ratio of the penalty factors applied to the stiffness matrix (pK) and
-        the mass matrix (pM) as pM/pK. If not provided, a default
-        value of `~sigmaepsilon.fem.constants.DEFAULT_MASS_PENALTY_RATIO`
-        is used.
-    """
-
-    def __init__(
-        self,
-        mesh: FemMesh,
-        essential_penalty: float = DEFAULT_DIRICHLET_PENALTY,
-        mass_penalty_ratio: float = DEFAULT_MASS_PENALTY_RATIO,
-    ):
-        if not isinstance(mesh, FemMesh):
-            raise TypeError(
-                "The type of 'mesh' is {},"
-                " which is not a subclass "
-                "of 'FemMesh'".format(type(mesh))
-            )
-        if not mesh.locked:
-            mesh.lock(create_mappers=True)
-        super().__init__()
-        self._mesh = mesh
-        self._static_solver = None
-        self._dynamic_solver_ = None
-        self._natural_circular_frequencies = None
-        self._essential_penalty = essential_penalty
-        self._mass_penalty_ratio = mass_penalty_ratio
-        self.clear_constraints()
-
-    @property
-    def mesh(self) -> FemMesh:
-        """
-        Returns the underlying mesh object.
-        """
-        return self._mesh
-
-    @mesh.setter
-    def mesh(self, value: FemMesh):
-        """
-        Sets the underlying mesh object.
-        """
-        if not isinstance(value, FemMesh):
-            raise TypeError(
-                "The type of 'value' is {},"
-                " which is not a subclass "
-                "of 'FemMesh'".format(type(value))
-            )
-        if not value.locked:
-            value.lock(create_mappers=True)
-        self._mesh = value
-
-    @property
-    def constraints(self) -> List[EBC]:
-        """
-        Returns the constraints of the structure as a list. Note that
-        this is an independent mechanism from the 'fixity' data defined
-        for the :class:`~sigmaepsilon.fem.pointdata.PointData` object
-        of the underlying mesh instance.
-        """
-        if self._constraints is None:
-            self._constraints = []
-        return self._constraints
-
-    def clear_constraints(self):
-        """
-        Clears up the constraints. This does not affect the 'fixity'
-        definitions in the pointdata of the mesh.
-
-        Note
-        ----
-        You can also use the `clear` method of the constrain list to get
-        rid of previously defined constraints.
-
-        Examples
-        --------
-        >>> structure.clear_constraints()
-
-        is equivalent to
-
-        >>> structure.constraints.clear()
-        """
-        self._constraints = None
-
-    @flatten_pd(False)
-    def natural_modes_of_vibration(self, *, flatten: bool = False, **kwargs) -> ndarray:
-        """
-        Returns natural modes of vibration.
-
-        Parameters
-        ----------
-        flatten : bool, Optional
-            If True, the result is a 1d array, otherwise 2d. Default is False.
-
-        Returns
-        -------
-        numpy.ndarray
-        """
-        return self.mesh.pd.vshapes
-
-    def natural_circular_frequencies(
-        self, *args, return_vectors: bool = False, **kwargs
-    ) -> Union[Tuple[ndarray], ndarray]:
-        """
-        Returns natural circular frequencies. The call forwards all parameters
-        to :func:`sigmaepslion.solid.fem.dyn.natural_circular_frequencies`,
-        see the docs there for the details.
-
-        Parameters
-        ----------
-        return_vectors : bool, Optional
-            To return eigenvectors or not. Default is False.
-
-        Returns
-        -------
-        numpy.ndarray
-            The natural circular frequencies.
-        numpy.ndarray
-            The eigenvectors, only if 'return_vectors' is True.
-
-        See also
-        --------
-        :func:`sigmaepslion.solid.fem.dyn.natural_circular_frequencies`
-        """
-        f = self._dynamic_solver_.natural_circular_frequencies(*args, **kwargs)
-        if return_vectors:
-            v = self.natural_modes_of_vibration(flatten=True)
-            return f, v
-        return f
-
-    def elastic_stiffness_matrix(
-        self,
-        *args,
-        penalize: bool = False,
-        sparse: bool = False,
-        transform: bool = False,
-        **kwargs
-    ) -> Union[ndarray, coo_matrix]:
-        """
-        Returns the elastic stiffness matrix of the structure with dense or
-        sparse layout.
-
-        Parameters
-        ----------
-        penalize : bool, Optional
-            If True, the result is the sum of the stiffness matrix and the
-            penalty matrix of the essential boundary conditions.
-        sparse : bool, Optional
-            If True, the result is a sparse matrix. Default is False.
-        transform : bool, Optional
-            If True, local matrices are transformed to the global frame.
-            Default is True.
-
-        Returns
-        -------
-        numpy.ndarray or scipy.sparse.coo_matrix
-        """
-        if penalize:
-            assert transform, "Must transform to penalize."
-            assert sparse, "Penalization is only available for sparse results."
-        if sparse:
-            assert transform, "Must transform for a sparse output."
-        params = dict(sparse=sparse, transform=transform)
-        params.update(**kwargs)
-        M_sparse = self.mesh.elastic_stiffness_matrix(**params)
-        if penalize:
-            M_sparse += self.mesh.essential_penalty_matrix()
-        return M_sparse.tocoo()
-
-    def essential_penalty_matrix(self, *args, **kwargs) -> coo_matrix:
-        """
-        Returns the penalty stiffness matrix of the structure.
-
-        Returns
-        -------
-        scipy.sparse.coo_matrix
-        """
-        return self.mesh.essential_penalty_matrix(*args, **kwargs).tocoo()
-
-    def consistent_mass_matrix(
-        self,
-        *,
-        penalize: bool = False,
-        sparse: bool = False,
-        transform: bool = False,
-        **kwargs
-    ) -> Union[coo_matrix, ndarray]:
-        """
-        Returns the stiffness-consistent mass matrix of the structure.
-
-        Parameters
-        ----------
-        penalize : bool, Optional
-            If True, the result is the sum of the mass matrix and the
-            penalty matrix of the essential boundary conditions.
-        sparse : bool, Optional
-            If True, the result is a sparse matrix. Default is False.
-        transform : bool, Optional
-            If True, local matrices are transformed to the global frame.
-            Default is True.
-
-        Returns
-        -------
-        numpy.ndarray or scipy.sparse.coo_matrix
-        """
-        if penalize:
-            assert transform, "Must transform to penalize."
-            assert sparse, "Penalization is only available for sparse results."
-        if sparse:
-            assert transform, "Must transform for a sparse output."
-        params = dict(sparse=sparse, transform=transform)
-        params.update(**kwargs)
-        return self.mesh.consistent_mass_matrix(**params)
-
-    def nodal_mass_matrix(self) -> coo_matrix:
-        """
-        Returns the nodal mass matrix of the structure.
-
-        Returns
-        -------
-        scipy.sparse.coo_matrix
-        """
-        return self.mesh.nodal_mass_matrix().tocoo()
-
-    def mass_matrix(self, penalize: bool = False) -> coo_matrix:
-        """
-        Returns the total mass matrix of the structure, which is the
-        sum of the stiffness-consistent mass matrix derived from the
-        densities of the cells and the nodal masses.
-
-        Parameters
-        ----------
-        penalize : bool, Optional
-            If True, the result is the sum of the mass matrix and the
-            penalty matrix emenating from the enforcing of the essential
-            boundary conditions using a Courant penalty function.
-
-        Returns
-        -------
-        scipy.sparse.coo_matrix
-        """
-        M_sparse = self.mesh.mass_matrix()
-        if penalize:
-            M_sparse += self.mesh.essential_penalty_matrix()
-        return M_sparse.tocoo()
-
-    @flatten_pd(False)
-    def nodal_dof_solution(self, *, flatten: bool = False, **__) -> ndarray:
-        """
-        Returns the vector of nodal displacements and optionally stores the result
-        with a specified key.
-
-        Parameters
-        ----------
-        flatten : bool, Optional
-            If True, the result is a 1d array, otherwise 2d. Default is False.
-
-        Returns
-        -------
-        numpy.ndarray
-        """
-        return self.mesh.pd.dofsol
-
-    @flatten_pd(False)
-    def reaction_forces(self, *, flatten: bool = False, **__) -> ndarray:
-        """
-        Returns the vector of reaction forces.
-
-        Parameters
-        ----------
-        flatten : bool, Optional
-            If True, the result is a 1d array, otherwise 2d. Default is False.
-
-        Returns
-        -------
-        numpy.ndarray
-        """
-        return self.mesh.pd.reactions
-
-    @flatten_pd(False)
-    def nodal_forces(self, *_, flatten: bool = False, **__) -> ndarray:
-        """
-        Returns the vector of nodal forces from all sources. This is calculated
-        during static analysis.
-
-        Parameters
-        ----------
-        flatten : bool, Optional
-            If True, the result is a 1d array, otherwise 2d. Default is False.
-        """
-        return self.mesh.pd.forces
-
-    def internal_forces(self, *args, flatten: bool = False, **kwargs) -> ndarray:
-        """
-        Returns the internal forces for one or more elements.
-        """
-        return self.mesh.internal_forces(*args, flatten=flatten, **kwargs)
-
-    def external_forces(self, *args, flatten: bool = False, **kwargs) -> ndarray:
-        """
-        Returns the external forces for one or more elements.
-        """
-        return self.mesh.external_forces(*args, flatten=flatten, **kwargs)
-
-    def linsolve(self, *args, **kwargs) -> "Structure":
-        """
-        Performs a linear elastostatic calculation with pre- and
-        post-processing.
-        """
-        return self.linear_static_analysis(*args, **kwargs)
-
-    def linear_static_analysis(self, *args, **kwargs) -> "Structure":
-        """
-        Performs a linear elastostatic calculation with pre- and
-        post-processing.
-        """
-        self._preproc_linstat_(*args, **kwargs)
-        self._proc_linstat_(*args, **kwargs)
-        return self._postproc_linstat_(*args, **kwargs)
-
-    def free_vibration_analysis(self, *args, **kwargs) -> "Structure":
-        """
-        Performs a linear elastostatic calculation with pre- and
-        post-processing.
-        """
-        self._preproc_free_vib_(*args, **kwargs)
-        self._proc_free_vib_(*args, **kwargs)
-        return self._postproc_free_vib_(*args, **kwargs)
-
-    def effective_modal_masses(self, actions: ndarray, modes: ndarray) -> ndarray:
-        """
-        Returns effective modal masses of several modes of vibration.
-        The call forwards all parameters to
-        :func:`sigmaepslion.solid.fem.dyn.effective_modal_masses`, see the
-        docs there for the details.
-
-        Parameters
-        ----------
-        actions : numpy.ndarray
-            One or more nodal displacement vectors representing rigid
-            body motions.
-        modes : numpy.ndarray
-            Modes of vibration.
-
-        Returns
-        -------
-        numpy.ndarray
-            An array of effective mass values.
-
-        See also
-        --------
-        :func:`~sigmaepslion.solid.fem.dyn.effective_modal_masses`
-        """
-        M_sparse = self.mesh.mass_matrix(penalize=False)
-        return effective_modal_masses(M_sparse, actions, modes)
-
-    def Rayleigh_quotient(self, u: ndarray, f: ndarray) -> ndarray:
-        """
-        Returns Rayleigh's quotient. The call forwards all parameters
-        to :func:`~sigmaepslion.solid.fem.dyn.Rayleigh_quotient`, see the
-        docs there for the details. If there are no actions specified,
-        the function feeds it with the results from a linear elastic solution.
-
-        Parameters
-        ----------
-        u : numpy.ndarray
-            One or more nodal displacement vectors.
-        f : numpy.ndarray
-            One or more nodal load vectors.
-
-        Returns
-        -------
-        float or numpy.ndarray
-            One or more floats, depending on the input.
-
-        See also
-        --------
-        :func:`~sigmaepslion.solid.fem.dyn.Rayleigh_quotient`
-        """
-        M_sparse = self.mass_matrix(penalize=True)
-        return Rayleigh_quotient(M_sparse, u, f=f)
-
-    def _initialize_(self, *_, **__) -> "Structure":
-        """
-        Initializes the structure. This includes data initialization
-        for the cells and happens during the preprocessor. Returns the object
-        for continuation.
-
-        See also
-        --------
-        :func:`preprocess`
-        """
-        blocks = self.mesh.cellblocks(inclusive=True)
-        for block in blocks:
-            nE = len(block.celldata)
-            # populate frames
-            if not block.celldata.has_frames:
-                frames = repeat(block.frame.show(), nE)
-                block.celldata.frames = frames
-        return self
-
-    def _assemble_linstat_(self, *_, **__):
-        mesh = self.mesh
-        jagged = mesh.is_jagged()
-
-        gnum = mesh.element_dof_numbering()
-        # get raw data
-        mesh.nodal_load_vector()
-        if jagged:
-            mesh.cell_load_vector(assemble=True, transform=True)
-        else:
-            mesh.cell_load_vector(assemble=False, transform=False)
-        mesh.elastic_stiffness_matrix(sparse=False, transform=False, _jagged=jagged)
-        # condensate
-        mesh.condensate_cell_fixity()
-        # get condensated data
-        f_nodal = mesh.nodal_load_vector()
-        if jagged:
-            f_bulk = mesh.cell_load_vector(assemble=True, transform=True)
-            K_bulk = mesh.elastic_stiffness_matrix(
-                sparse=False,
-                transform=True,
-                _jagged=jagged,
-            )
-        else:
-            f_bulk = mesh.cell_load_vector(assemble=False, transform=False)
-            K_bulk = mesh.elastic_stiffness_matrix(
-                sparse=False, transform=False, _jagged=jagged
-            )
-
-        if not jagged:
-            # transform to global
-            dcm = mesh.direction_cosine_matrix(target="global")
-            K_bulk = tr_element_matrices_bulk(K_bulk, dcm)
-            f_bulk = tr_nodal_loads_bulk(f_bulk, dcm)
-            # assemble nodal load vector, the stiffness matrix gets assembled
-            # in the solver
-            nX = len(mesh.pd) * mesh.NDOFN
-            f_bulk = assemble_load_vector(f_bulk, gnum, nX)
-        f = f_nodal + f_bulk
-        # penalize essential boundary conditions
-        penalty = self._essential_penalty
-        Kp = mesh.essential_penalty_matrix(penalty=penalty)
-        fp = np.zeros(f.shape[0], dtype=float)
-        for c in self.constraints:
-            Kpc, fpc = c.assemble(mesh)
-            Kp += Kpc
-            fp += fpc
-        if len(f.shape) == 1:
-            f[:] += fp
-        else:
-            for i in range(f.shape[1]):
-                f[:, i] += fp
-        # create solver
-        self._static_solver_ = StaticSolver(K_bulk, Kp.tocoo(), f, gnum, mesh=mesh)
-        return self
-
-    def _assemble_free_vib_(self, *_, **__):
-        mesh = self.mesh
-        gnum = mesh.element_dof_numbering()
-        # get raw data
-        mesh.nodal_load_vector()
-        mesh.cell_load_vector(assemble=False, transform=False)
-        mesh.elastic_stiffness_matrix(sparse=False, transform=False)
-        mesh.consistent_mass_matrix(sparse=False, transform=False)
-        # condensate
-        mesh.condensate_cell_fixity()
-        # get condensated data
-        M_sparse = mesh.mass_matrix()
-        K_bulk = mesh.elastic_stiffness_matrix(sparse=False, transform=False)
-        # transform to global
-        dcm = mesh.direction_cosine_matrix(target="global")
-        K_bulk = tr_element_matrices_bulk(K_bulk, dcm)
-        # penalize essential boundary conditions
-        penalty = self._essential_penalty
-        Kp = mesh.essential_penalty_matrix(penalty=penalty)
-        for c in self.constraints:
-            Kpc, _ = c.assemble(mesh)
-            Kp += Kpc
-        # create solver
-        penalty_ratio = self._mass_penalty_ratio
-        self._dynamic_solver_ = DynamicSolver(
-            K_bulk,
-            Kp.tocoo(),
-            M_sparse,
-            gnum,
-            regular=False,
-            mesh=mesh,
-            penalty_ratio=penalty_ratio,
-        )
-        return self
-
-    def _preproc_linstat_(self, *args, **kwargs) -> "Structure":
-        self._initialize_(*args, **kwargs)
-        self._assemble_linstat_(*args, **kwargs)
-        return self
-
-    def _preproc_free_vib_(self, *args, **kwargs) -> "Structure":
-        self._initialize_(*args, **kwargs)
-        self._assemble_free_vib_(*args, **kwargs)
-        return self
-
-    def _proc_linstat_(self, *args, **kwargs) -> "Structure":
-        self._static_solver_.solve(*args, **kwargs)
-        return self
-
-    def _proc_free_vib_(self, *args, **kwargs) -> "Structure":
-        self._dynamic_solver_.natural_circular_frequencies(*args, **kwargs)
-        return self
-
-    def _postproc_linstat_(self, *args, cleanup: bool = False, **kwargs) -> "Structure":
-        solver = self._static_solver_
-        mesh = self.mesh
-        nDOFN = mesh.NDOFN
-        nN = len(mesh.pd)
-        # dof solution
-        u = solver.u
-        nRHS = 1 if len(u.shape) == 1 else u.shape[-1]
-        if nRHS == 1:
-            u = np.reshape(u, (nN, nDOFN))
-        else:
-            u = np.reshape(u, (nN, nDOFN, nRHS))
-        self.mesh.pd.dofsol = u
-        # reaction forces
-        r = solver.r
-        if nRHS == 1:
-            r = np.reshape(r, (nN, nDOFN))
-        else:
-            r = np.reshape(r, (nN, nDOFN, nRHS))
-        self.mesh.pd.reactions = r
-        # nodal loads
-        f = solver.f
-        if nRHS == 1:
-            f = np.reshape(f, (nN, nDOFN))
-        else:
-            f = np.reshape(f, (nN, nDOFN, nRHS))
-        self.mesh.pd.forces = f
-        # postproc block results
-        self.mesh.postprocess(*args, **kwargs)
-        if cleanup:
-            self.cleanup()
-        return self
-
-    def _postproc_free_vib_(self, *, cleanup: bool = False, **__) -> "Structure":
-        mesh = self.mesh
-        solver = self._dynamic_solver_
-        self._natural_circular_frequencies = solver.frequencies
-        vshapes = solver.modal_shapes
-        nN = len(mesh.pd)
-        nDOF = mesh.__class__.NDOFN
-        nS = vshapes.shape[-1]
-        mesh.pd.vshapes = vshapes.reshape(nN, nDOF, nS)
-        if cleanup:
-            self.cleanup()
-        return self
-
-    def cleanup(self) -> "Structure":
-        """
-        Destroys the solver and returns the object for continuation.
-
-        Returns
-        -------
-        Structure
-        """
-        self._static_solver_ = None
-        self._dynamic_solver_ = None
-        return self
+# -*- coding: utf-8 -*-
+from typing import Union, List
+
+from scipy.sparse import coo_matrix
+import numpy as np
+
+from neumann import squeeze
+from neumann.array import atleast3d
+
+from polymesh import PolyData
+
+from .pointdata import PointData
+from .cells.celldata import CellData
+from .preproc import fem_load_vector, fem_penalty_matrix_coo, fem_nodal_mass_matrix_coo
+from .cells import TET4, TET10, H8, H27
+
+
+class FemMesh(PolyData):
+    """
+    A descendant of :class:`polymesh.PolyData` to handle polygonal meshes for the **Finite Element Method**.
+
+    Parameters
+    ----------
+    pd : :class:`polymesh.PolyData` or :class:`polymesh.CellData`, Optional
+        A PolyData or a CellData instance. Dafault is None.
+
+    cd : :class:`polymesh.CellData`, Optional
+        A CellData instance, if the first argument is provided. Dafault is None.
+
+    coords : :class:`numpy.ndarray`, Optional
+        2d numpy array of floats, describing a pointcloud. Default is None.
+
+    topo : :class:`numpy.ndarray`, Optional
+        2d numpy array of integers, describing the topology of a polygonal mesh. 
+        Default is None.
+
+    celltype : int, Optional
+        An integer spcifying a valid celltype.
+
+    Note
+    ----
+    The suggested way of usage is to create the pointdata and celldata
+    objects in advance, and provide them as the firts argument when building the model.
+    See below for how it works!
+
+    Examples
+    --------
+    >>> from sigmaepsilon.solid import FemMesh
+    >>> from polymesh.grid import grid
+    >>> size = Lx, Ly, Lz = 100, 100, 100
+    >>> shape = nx, ny, nz = 10, 10, 10
+    >>> coords, topo = grid(size=size, shape=shape, eshape='H27')
+    >>> pd = FemMesh(coords=coords)
+    >>> pd['A']['Part1'] = FemMesh(topo=topo[:10])
+    >>> pd['B']['Part2'] = FemMesh(topo=topo[10:-10])
+    >>> pd['C']['Part3'] = FemMesh(topo=topo[-10:])
+
+    See also
+    --------
+    :class:`polymesh.PolyData`
+    :class:`polymesh.CellData`
+
+    """
+
+    dofs = ('UX', 'UY', 'UZ', 'ROTX', 'ROTY', 'ROTZ')
+    NDOFN = 6
+    _point_class_ = PointData
+
+    def __init__(self, *args, model=None, fixity=None, loads=None, body_loads=None,
+                 strain_loads=None, t=None, density=None, mass=None,
+                 cell_fields=None, point_fields=None, activity=None,
+                 connectivity=None, **kwargs):
+        # fill up data objects with obvious data
+        pkeys = self.__class__._point_class_._attr_map_
+        point_fields = {} if point_fields is None else point_fields
+        point_fields[pkeys['loads']] = loads
+        point_fields[pkeys['mass']] = mass
+        point_fields[pkeys['fixity']] = fixity
+        point_fields[pkeys['loads']] = loads
+        ckeys = CellData._attr_map_
+        cell_fields = {} if cell_fields is None else cell_fields
+        cell_fields[ckeys['loads']] = body_loads
+        cell_fields[ckeys['strain-loads']] = strain_loads
+        cell_fields[ckeys['density']] = density
+        cell_fields[ckeys['t']] = t
+        cell_fields[ckeys['connectivity']] = connectivity
+        super().__init__(*args, point_fields=point_fields,
+                         cell_fields=cell_fields, **kwargs)
+        # nodal data can only be provided for the root object
+        if not self.is_root():
+            assert loads is None, "At object creation, nodal loads can only \
+                be provided at the top level."
+            assert fixity is None, "At object creation, fixity information \
+                can only be provided at the top level."
+            assert mass is None, "At object creation, nodal masses can only \
+                be provided at the top level."
+        # it is determined by the size of `activity` whether it refers to
+        # cells or points
+        if isinstance(activity, np.ndarray):
+            nA = activity.shape[0]
+            if self.celldata is not None:
+                N = len(self.celldata)
+                if nA == N:
+                    self.celldata.activity = activity
+                    nA = -1
+            if nA > 0 and self.pointdata is not None:
+                N = len(self.pointdata)
+                if nA == N:
+                    self.pointdata.activity = activity
+                    nA = -1
+            assert nA < 0
+        self._model = model
+
+    def cells_coords(self, *args, points=None, cells=None, **kwargs) \
+            -> Union[np.ndarray, List[np.ndarray]]:
+        """
+        Returns the coordinates of the cells as a 3d numpy array if the 
+        subblocks form a regular mesh, or a list of such arrays.
+        """
+        if points is None and cells is None:
+            return super().cells_coords(*args, **kwargs)
+        else:
+            blocks = self.cellblocks(inclusive=True)
+            kwargs.update(points=points, squeeze=False)
+            if cells is not None:
+                kwargs.update(cells=cells)
+                res = {}
+                def foo(b): return b.celldata.coords(*args, **kwargs)
+                [res.update(d) for d in map(foo, blocks)]
+                return res
+            else:
+                def foo(b): return b.celldata.coords(*args, **kwargs)
+                return np.vstack(list(map(foo, blocks)))
+
+    def element_dof_numbering(self, *args, **kwargs) -> np.ndarray:
+        """
+        Returns global ids of the local degrees of freedoms for each cell.
+        """
+        blocks = self.cellblocks(inclusive=True)
+        def foo(b): return b.celldata.global_dof_numbering()
+        return np.vstack(list(map(foo, blocks)))
+
+    def elastic_stiffness_matrix(self, *args, sparse=True, **kwargs) -> Union[np.ndarray, coo_matrix]:
+        """
+        Returns the elastic stiffness matrix in dense or sparse format.
+
+        Parameters
+        ----------
+        sparse : bool, Optional
+            Returns the matrix in a sparse format. Default is True.
+
+        Returns
+        -------
+        :class:`numpy.ndarray` or :class:`scipy.sparse.coo_matrix`
+
+        """
+        if sparse:
+            return self.elastic_stiffness_matrix_coo(*args, **kwargs)
+        blocks = self.cellblocks(inclusive=True)
+        def foo(b): return b.celldata.elastic_stiffness_matrix()
+        return np.vstack(list(map(foo, blocks)))
+
+    def elastic_stiffness_matrix_coo(self, *args, eliminate_zeros=True,
+                                     sum_duplicates=True, **kwargs):
+        """
+        Elastic stiffness matrix in coo format.
+
+        Parameters
+        ----------
+        eliminate_zeros : bool, Optional
+            Eliminates zero entries. Default is True.
+
+        sum_duplicates : bool, Optional
+            Sums duplicate entries. Default is True.
+
+        Returns
+        -------
+        :class:`scipy.sparse.coo_matrix`
+            The stiffness matrix in sparse COO format.
+
+        """
+        blocks = self.cellblocks(inclusive=True)
+        def foo(b): return b.celldata.elastic_stiffness_matrix_coo()
+        K = np.sum(list(map(foo, blocks))).tocoo()
+        if eliminate_zeros:
+            K.eliminate_zeros()
+        if sum_duplicates:
+            K.sum_duplicates()
+        return K
+
+    def masses(self, *args, **kwargs) -> np.ndarray:
+        """
+        Returns cell masses of the cells as a 1d numpy array.
+        """
+        blocks = self.cellblocks(*args, inclusive=True, **kwargs)
+        vmap = map(lambda b: b.celldata.masses(), blocks)
+        return np.concatenate(list(vmap))
+
+    def mass(self, *args, **kwargs) -> float:
+        """
+        Returns the total mass as a float.
+        """
+        return np.sum(self.masses(*args, **kwargs))
+
+    def consistent_mass_matrix(self, *args, sparse=True, **kwargs):
+        """
+        Returns the consistent mass matrix of the mesh with either dense 
+        or sparse layout.
+
+        Parameters
+        ----------
+        sparse : bool, Optional
+            Returns the matrix in a sparse format. Default is True.
+
+        Notes
+        -----
+        If there are nodal masses defined, only sparse output is 
+        available at the moment.
+
+        """
+        if sparse:
+            return self.consistent_mass_matrix_coo(*args, **kwargs)
+        else:
+            dbkey = self.__class__._point_class_._attr_map_['mass']
+            if dbkey in self.root().pointdata.fields:
+                return self.consistent_mass_matrix_coo(*args, **kwargs)
+        # distributed masses (cells)
+        blocks = self.cellblocks(inclusive=True)
+        def foo(b): return b.celldata.consistent_mass_matrix()
+        return np.vstack(list(map(foo, blocks)))
+
+    def consistent_mass_matrix_coo(self, *args, eliminate_zeros=True,
+                                   sum_duplicates=True, distribute=False, **kwargs):
+        """
+        Returns the mass matrix in coo format. If `distribute` is set 
+        to `True`, nodal masses are distributed over neighbouring cells 
+        and handled as self-weight is.
+
+        Parameters
+        ----------
+        eliminate_zeros : bool, Optional
+            Eliminates zero entries. Default is True.
+
+        sum_duplicates : bool, Optional
+            Sums duplicate entries. Default is True.
+
+        distribute : bool, Optional
+            If True, nodal masses are distributed over neighbouring cells 
+            and are handled as self-weight is. Default is True.
+
+        Returns
+        -------
+        scipy.sparse.coo_matrix
+            The mass matrix in sparse COO format.
+
+        """
+        # distributed masses (cells)
+        blocks = list(self.cellblocks(inclusive=True))
+        def foo(b): return b.celldata.consistent_mass_matrix_coo()
+        M = np.sum(list(map(foo, blocks))).tocoo()
+        # nodal masses
+        pd = self.root().pointdata
+        dbkey = self.__class__._point_class_._attr_map_['mass']
+        if dbkey in pd.fields:
+            d = pd.mass
+            if distribute:
+                v = self.volumes()
+                edata = list(
+                    map(lambda b: b.celldata.pull(data=d, avg=v), blocks))
+
+                def foo(bv): return bv[0].celldata.consistent_mass_matrix_coo(
+                    values=bv[1])
+                moo = map(lambda i: (blocks[i], edata[i]), range(len(blocks)))
+                M += np.sum(list(map(foo, moo))).tocoo()
+            else:
+                ndof = self.__class__.NDOFN
+                M += fem_nodal_mass_matrix_coo(values=d, eliminate_zeros=eliminate_zeros,
+                                               sum_duplicates=sum_duplicates, ndof=ndof)
+        if eliminate_zeros:
+            M.eliminate_zeros()
+        if sum_duplicates:
+            M.sum_duplicates()
+        return M
+
+    def penalty_matrix_coo(self, *args, eliminate_zeros=True,
+                           sum_duplicates=True, ensure_comp=False,
+                           distribute=False, **kwargs) -> coo_matrix:
+        """
+        A penalty matrix that enforces Dirichlet boundary conditions. 
+        Returns a scipy sparse matrix in coo format.
+        """
+        fixity = self.root().pointdata.fixity
+        K_coo = fem_penalty_matrix_coo(values=fixity, eliminate_zeros=eliminate_zeros,
+                                       sum_duplicates=sum_duplicates)
+        return K_coo.tocoo()
+
+    def approximation_matrix_coo(self, *args, eliminate_zeros=True, **kwargs) -> coo_matrix:
+        blocks = self.cellblocks(inclusive=True)
+        def foo(b): return b.celldata.approximation_matrix_coo()
+        res = np.sum(list(map(foo, blocks))).tocoo()
+        if eliminate_zeros:
+            res.eliminate_zeros()
+        return res
+
+    def nodal_approximation_matrix_coo(self, *args, eliminate_zeros=True, **kwargs) -> coo_matrix:
+        blocks = self.cellblocks(inclusive=True)
+        def foo(b): return b.celldata.nodal_approximation_matrix_coo()
+        res = np.sum(list(map(foo, blocks))).tocoo()
+        if eliminate_zeros:
+            res.eliminate_zeros()
+        return res
+
+    @squeeze(True)
+    def load_vector(self, *args, **kwargs) -> np.ndarray:
+        """
+        Returns the nodal load vector.
+
+        """
+        # concentrated nodal loads
+        nodal_data = self.root().pointdata.loads
+        nodal_data = atleast3d(nodal_data, back=True)  # (nP, nDOF, nRHS)
+        res = fem_load_vector(values=nodal_data, squeeze=False)
+        # cells
+        blocks = list(self.cellblocks(inclusive=True))
+        # body loads
+        def foo(b): return b.celldata.body_load_vector(squeeze=False)
+        try:
+            m = filter(lambda i : i is not None, map(foo, blocks))
+            res += np.sum(list(m), axis=0)
+        except Exception:
+            pass
+        # strain loads
+        def foo(b): return b.celldata.strain_load_vector(squeeze=False)
+        try:
+            m = filter(lambda i : i is not None, map(foo, blocks))
+            res += np.sum(list(m), axis=0)
+        except Exception:
+            pass
+        return res
+
+    def prostproc_dof_solution(self, *args, **kwargs):
+        """
+        Calculates approximate solution of the primary variables as a list of arrays
+        for each block in the mesh.
+        """
+        blocks = self.cellblocks(inclusive=True)
+        dofsol = self.root().pointdata.dofsol
+        def foo(b): return b.celldata.prostproc_dof_solution(dofsol=dofsol)
+        list(map(foo, blocks))
+
+    @squeeze(True)
+    def nodal_dof_solution(self, *args, flatten=False, **kwargs) -> np.ndarray:
+        """
+        Returns nodal degree of freedom solution.
+        """
+        dofsol = self.root().pointdata.dofsol
+        if flatten:
+            if len(dofsol.shape) == 2:
+                return dofsol.flatten()
+            else:
+                nN, nDOFN, nRHS = dofsol.shape
+                return dofsol.reshape((nN * nDOFN, nRHS))
+        else:
+            return dofsol
+
+    @squeeze(True)
+    def cell_dof_solution(self, *args, cells=None, flatten=True,
+                          squeeze=True, **kwargs) -> np.ndarray:
+        """
+        Returns degree of freedom solution for each cell.
+        """
+        blocks = self.cellblocks(inclusive=True)
+        kwargs.update(flatten=flatten, squeeze=False)
+        if cells is not None:
+            kwargs.update(cells=cells)
+            res = {}
+            def foo(b): return b.celldata.dof_solution(*args, **kwargs)
+            [res.update(d) for d in map(foo, blocks)]
+            return res
+        else:
+            def foo(b): return b.celldata.dof_solution(*args, **kwargs)
+            return np.vstack(list(map(foo, blocks)))
+
+    @squeeze(True)
+    def strains(self, *args, cells=None, squeeze=True, **kwargs) -> np.ndarray:
+        """
+        Returns strain solution for each cell.
+        """
+        blocks = self.cellblocks(inclusive=True)
+        kwargs.update(squeeze=False)
+        if cells is not None:
+            kwargs.update(cells=cells)
+            res = {}
+            def foo(b): return b.celldata.strains(*args, **kwargs)
+            [res.update(d) for d in map(foo, blocks)]
+            return res
+        else:
+            def foo(b): return b.celldata.strains(*args, **kwargs)
+            return np.vstack(list(map(foo, blocks)))
+
+    @squeeze(True)
+    def internal_forces(self, *args, cells=None, flatten=True, squeeze=True, **kwargs) -> np.ndarray:
+        """
+        Returns internal force solution for each cell.
+        """
+        blocks = self.cellblocks(inclusive=True)
+        kwargs.update(flatten=flatten, squeeze=False)
+        if cells is not None:
+            kwargs.update(cells=cells)
+            res = {}
+            def foo(b): return b.celldata.internal_forces(*args, **kwargs)
+            [res.update(d) for d in map(foo, blocks)]
+            return res
+        else:
+            def foo(b): return b.celldata.internal_forces(*args, **kwargs)
+            return np.vstack(list(map(foo, blocks)))
+
+    def stresses_at_cells_nodes(self, *args, **kwargs) -> np.ndarray:
+        """
+        Returns stresses at all nodes of all cells.
+        """
+        blocks = self.cellblocks(inclusive=True)
+        def foo(b): return b.celldata.stresses_at_nodes(*args, **kwargs)
+        return np.vstack(list(map(foo, blocks)))
+
+    def stresses_at_centers(self, *args, **kwargs) -> np.ndarray:
+        """
+        Returns stresses at the centers of all cells.
+        """
+        blocks = self.cellblocks(inclusive=True)
+        def foo(b): return b.celldata.stresses_at_centers(*args, **kwargs)
+        return np.squeeze(np.vstack(list(map(foo, blocks))))
+
+    @property
+    def model(self):
+        """
+        Returns the attached model object if there is any.
+        """
+        if self._model is not None:
+            return self._model
+        else:
+            if self.is_root():
+                return self._model
+            else:
+                return self.parent.model
+
+    def material_stiffness_matrix(self):
+        """
+        Returns the model of the mesh if there is any.
+        This is not important if all the celldata in the mesh
+        are filled up with appropriate model stiffness matrices.
+        Otherwise, the model stiffness matrix is calcualated on the 
+        mesh level during the initialization stage and is spread 
+        among the subblocks.
+        """
+        m = self.model
+        if isinstance(m, np.ndarray):
+            return m
+        else:
+            try:
+                return m.stiffness_matrix()
+            except Exception:
+                raise RuntimeError("Invalid model type {}".format(type(m)))
+
+    def postprocess(self, *args, **kwargs):
+        """
+        General postprocessing. This may be reimplemented in subclasses,
+        currently nothing happens here.
+        """
+        pass
+    
+    
+class SolidMesh(FemMesh):
+    """
+    A data class dedicated to simple 3d solid cells with 3 degrees of freedom per node.    
+    
+    See also
+    --------
+    :class:`TET4`
+    :class:`TET10`
+    :class:`H8`
+    :class:`H27`
+    """
+
+    dofs = ('UX', 'UY', 'UZ')
+    NDOFN = 3
+    
+    _cell_classes_ = {
+        4: TET4,
+        10: TET10,
+        8: H8,
+        27: H27,
+    }
+
+
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/fourier/proc.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fourier/proc.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,85 +1,40 @@
-import numpy as np
-from numpy import ndarray
-from numba import njit, prange
-
-from neumann.linalg import inv2x2, inv3x3
-
-
-def linsolve(LHS: ndarray, RHS: ndarray, *args, **kwarg):
-    if len(LHS.shape) > 2:
-        return linsolve2d(LHS, RHS)
-    else:
-        raise NotImplementedError
-
-
-@njit(nogil=True, parallel=True, cache=True)
-def linsolve_Bernoulli(A: ndarray, B: ndarray):
-    """
-    Calculates unknowns for Bernoulli Beams.
-    """
-    nLHS, N = A.shape
-    nRHS = B.shape[0]
-    res = np.zeros((nLHS, nRHS, N))
-    for i in prange(nRHS):
-        for j in prange(nLHS):
-            for n in prange(N):
-                res[j, i, n] = B[i, n] / A[j, n]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=True)
-def linsolve_Timoshenko(A: ndarray, B: ndarray):
-    """
-    Calculates unknowns for Timoshenko Beams.
-    """
-    nLHS, nMN = A.shape[:2]
-    nRHS = B.shape[0]
-    res = np.zeros((nLHS, nRHS, nMN, 2))
-    for i in prange(nRHS):
-        for j in prange(nLHS):
-            for k in prange(nMN):
-                res[j, i, k] = inv2x2(A[j, k]) @ B[i, k]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=True)
-def linsolve2d(A: ndarray, B: ndarray):
-    nLHS, nMN = A.shape[:2]
-    nV = A.shape[-1]
-    nRHS = B.shape[0]
-    res = np.zeros((nLHS, nRHS, nMN, nV))
-    if nV == 3:
-        for i in prange(nRHS):
-            for j in prange(nLHS):
-                for k in prange(nMN):
-                    res[j, i, k] = inv3x3(A[j, k]) @ B[i, k]
-    else:
-        for i in prange(nRHS):
-            for j in prange(nLHS):
-                for k in prange(nMN):
-                    res[j, i, k] = inv2x2(A[j, k]) @ B[i, k]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=True)
-def linsolve_Mindlin(A: ndarray, B: ndarray):
-    nLHS, nMN = A.shape[:2]
-    nRHS = B.shape[0]
-    res = np.zeros((nLHS, nRHS, nMN, 3))
-    for i in prange(nRHS):
-        for j in prange(nLHS):
-            for k in prange(nMN):
-                res[j, i, k] = inv3x3(A[j, k]) @ B[i, k]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=True)
-def linsolve_Kirchhoff(A: ndarray, B: ndarray):
-    nLHS, nMN = A.shape[:2]
-    nRHS = B.shape[0]
-    res = np.zeros((nLHS, nRHS, nMN))
-    for i in prange(nRHS):
-        for j in prange(nLHS):
-            for k in prange(nMN):
-                res[j, i, k] = inv2x2(A[j, k]) @ B[i, k]
-    return res
+# -*- coding: utf-8 -*-
+import numpy as np
+from numpy import ndarray
+from numba import njit, prange
+
+from neumann import squeeze
+from neumann.linalg.solve import npsolve
+
+
+@squeeze(True)
+def linsolve(LHS: ndarray, RHS: ndarray, *args, **kwarg):
+    if len(LHS.shape) > 2:
+        return linsolve_Mindlin(LHS, RHS)
+    else:
+        return linsolve_Kirchhoff(LHS, RHS)
+
+
+@njit(nogil=True, parallel=True, cache=True)
+def linsolve_Kirchhoff(A: ndarray, B: ndarray):
+    nLHS, nMN = A.shape
+    nRHS = B.shape[0]
+    res = np.zeros((nRHS, nLHS, nMN))
+    for i in prange(nRHS):
+        for j in prange(nLHS):
+            for k in prange(nMN):
+                res[i, j, k] = B[i, k] / A[j, k]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=True)
+def linsolve_Mindlin(A: ndarray, B: ndarray):
+    nLHS, nMN = A.shape[:2]
+    nRHS = B.shape[0]
+    res = np.zeros((nRHS, nLHS, nMN, 3))
+    for i in prange(nRHS):
+        for j in prange(nLHS):
+            for k in prange(nMN):
+                #res[i, j, k] = inv3x3(A[j, k]) @ B[i, k]
+                res[i, j, k] = npsolve(A[j, k], B[i, k]) 
+    return res
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/material/surface/meta.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/metashell.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,190 +1,183 @@
-from typing import Iterable
-import numpy as np
-from abc import abstractmethod, abstractclassmethod
-
-from linkeddeepdict import LinkedDeepDict
-from linkeddeepdict.tools.kwargtools import getasany, allinkwargs, anyinkwargs
-from linkeddeepdict.tools.dtk import parsedicts_addr
-
-from ...core.material import MaterialLike
-
-
-class MetaSurface(MaterialLike, LinkedDeepDict):
-    """
-    Base object implementing methods that both a folder (a shell) and a
-    file (a layer) can posess.
-    """
-
-    __layerclass__ = None
-
-    @property
-    def angle(self):
-        """Returns the angle of a layer or a laminate."""
-        _angle = self.get("angle", None)
-        if _angle is None:
-            return None if self.is_root() else self.parent.angle
-        else:
-            return _angle
-
-    @angle.setter
-    def angle(self, value):
-        """Sets the angle of a layer or a laminate."""
-        if self.__layerclass__ is None:
-            self["angle"] = value
-        else:
-            for layer in self.containers(dtype=self.__layerclass__):
-                layer["angle"] = value
-            self["angle"] = 0
-            del self["angle"]
-
-    @property
-    def hooke(self):
-        """Returns the Hooke model of a layer or a laminate."""
-        _hooke = self.get("hooke", None)
-        if _hooke is None:
-            return None if self.is_root() else self.parent.hooke
-        else:
-            return _hooke
-
-    @hooke.setter
-    def hooke(self, value):
-        """Sets the Hooke model of a layer or a laminate."""
-        if self.__layerclass__ is None:
-            self["hooke"] = value
-        else:
-            for layer in self.containers(dtype=self.__layerclass__):
-                layer["hooke"] = value
-            self["hooke"] = 0
-            del self["hooke"]
-
-    @property
-    def t(self):
-        """Returns the thickness of a layer."""
-        return self.get("thickness", None)
-
-    @t.setter
-    def t(self, value):
-        """Sets the thickness of a layer."""
-        if self.__layerclass__ is None:
-            self["thickness"] = value
-        else:
-            raise RuntimeError
-
-
-class SurfaceLayer(MetaSurface):
-    """
-    Helper base class for layers of a laminate.
-    """
-
-    __loc__ = [-1.0, 0.0, 1.0]
-    __shape__ = (8, 8)
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.hooke = getasany(["material", "m", "hooke"], **kwargs)
-        # set thickness
-        self.tmin = None
-        self.tmax = None
-        self.t = None
-        if allinkwargs(["tmin", "tmax"], **kwargs):
-            self.tmin = kwargs.get("tmin", None)
-            self.tmax = kwargs.get("tmax", None)
-            self.t = self.tmax - self.tmin
-        elif anyinkwargs(["t", "thickness"], **kwargs):
-            self.t = getasany(["t", "thickness"], **kwargs)
-            if "tmin" in kwargs:
-                self.tmin = kwargs["tmin"]
-                self.tmax = self.tmin + self.t
-            elif "tmax" in kwargs:
-                self.tmax = kwargs["tmax"]
-                self.tmin = self.tmax - self.t
-            else:
-                self.tmin = (-1) * self.t / 2
-                self.tmax = self.t / 2
-
-    def loc_to_z(self, loc) -> float:
-        """
-        Returns height of a local point by linear interpolation.
-        Local coordinate is expected between -1 and 1.
-        """
-        return 0.5 * ((self.tmax + self.tmin) + loc * (self.tmax - self.tmin))
-
-    @abstractmethod
-    def elastic_stiffness_matrix(self):
-        raise NotImplementedError
-
-
-class Surface(MetaSurface):
-    """
-    Helper base class for laminates.
-    """
-
-    __layerclass__ = SurfaceLayer
-
-    @abstractclassmethod
-    def Hooke(cls):
-        raise NotImplementedError
-
-    def Layer(self, *args, **kwargs) -> SurfaceLayer:
-        """
-        Returns a Layer compatible with the model.
-        """
-        return self.__layerclass__(*args, **kwargs)
-
-    def layers(self) -> Iterable[SurfaceLayer]:
-        """
-        Returns the layers of the laminate.
-        """
-        return [layer for layer in self.containers(dtype=self.__layerclass__)]
-
-    def iterlayers(self) -> Iterable[SurfaceLayer]:
-        """
-        Returns the layers of the laminate as a generator.
-        """
-        return self.containers(dtype=self.__layerclass__)
-
-    def elastic_stiffness_matrix(self) -> np.ndarray:
-        """
-        Assembles and returns the stiffness matrix.
-        """
-        self._set_layers()
-        res = np.zeros(self.__layerclass__.__shape__)
-        for layer in self.iterlayers():
-            res += layer.elastic_stiffness_matrix()
-        return res
-
-    def _set_layers(self):
-        """
-        Sets thickness ranges for the layers.
-        """
-        layers = self.layers()
-        t = sum([layer.t for layer in layers])
-        layers[0].tmin = -t / 2
-        nLayers = len(layers)
-        for i in range(nLayers - 1):
-            layers[i].tmax = layers[i].tmin + layers[i].t
-            layers[i + 1].tmin = layers[i].tmax
-        layers[-1].tmax = t / 2
-        for layer in layers:
-            layer.zi = [layer.loc_to_z(l_) for l_ in layer.__loc__]
-        return True
-
-    @classmethod
-    def from_dict(cls, d: dict = None, **kwargs) -> "Surface":
-        """
-        Returns a material model from a dictionary.
-        """
-        if d is None:
-            d = {}
-        d.update(**kwargs)
-        res = cls(**d)
-        for addr, value in parsedicts_addr(d, inclusive=True):
-            if len(addr) == 0:
-                continue
-            if "hooke" in value:
-                subcls = cls.__layerclass__
-            else:
-                continue
-            value["key"] = addr[-1]
-            res[addr] = subcls(**value)
-        return res
+# -*- coding: utf-8 -*-
+from typing import Iterable
+import numpy as np
+from numpy import ndarray
+from abc import abstractmethod
+
+from linkeddeepdict import LinkedDeepDict
+from linkeddeepdict.tools.kwargtools import getasany, allinkwargs, anyinkwargs
+from linkeddeepdict.tools.dtk import parsedicts_addr
+
+
+class MetaSurface(LinkedDeepDict):
+    """
+    Base object implementing methods that both a folder (a shell) and a
+    file (a layer) can posess.
+    """
+    
+    __layerclass__ = None
+    
+    @property
+    def angle(self):
+        """Returns the angle of a layer or a laminate."""
+        _angle = self.get('angle', None)
+        if _angle is None:
+            return None if self.is_root() else self.parent.angle
+        else:
+            return _angle
+
+    @angle.setter
+    def angle(self, value):
+        """Sets the angle of a layer or a laminate."""
+        if self.__layerclass__ is None:
+            self['angle'] = value
+        else:
+            for layer in self.containers(dtype=self.__layerclass__):
+                layer['angle'] = value
+            self['angle'] = 0
+            del self['angle']
+            
+    @property
+    def hooke(self):
+        """Returns the Hooke model of a layer or a laminate."""
+        _hooke = self.get('hooke', None)
+        if _hooke is None:
+            return None if self.is_root() else self.parent.hooke
+        else:
+            return _hooke
+
+    @hooke.setter
+    def hooke(self, value):
+        """Sets the Hooke model of a layer or a laminate."""
+        if self.__layerclass__ is None:
+            self['hooke'] = value
+        else:
+            for layer in self.containers(dtype=self.__layerclass__):
+                layer['hooke'] = value
+            self['hooke'] = 0
+            del self['hooke']
+    
+    @property
+    def t(self):
+        """Returns the thickness of a layer."""
+        return self.get('thickness', None)
+    
+    @t.setter
+    def t(self, value):
+        """Sets the thickness of a layer."""
+        if self.__layerclass__ is None:
+            self['thickness'] = value
+        else:
+            raise RuntimeError
+        
+
+class Layer(MetaSurface):
+    """
+    Helper base class for layers of a laminate.
+    """
+
+    __loc__ = [-1., 0., 1.]
+    __shape__ = (8, 8)
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.hooke = getasany(['material', 'm', 'hooke'], **kwargs)
+        # set thickness
+        self.tmin = None
+        self.tmax = None
+        self.t = None
+        if allinkwargs(['tmin', 'tmax'], **kwargs):
+            self.tmin = kwargs.get('tmin', None)
+            self.tmax = kwargs.get('tmax', None)
+            self.t = self.tmax-self.tmin
+        elif anyinkwargs(['t', 'thickness'], **kwargs):
+            self.t = getasany(['t', 'thickness'], **kwargs)
+            if 'tmin' in kwargs:
+                self.tmin = kwargs['tmin']
+                self.tmax = self.tmin + self.t
+            elif 'tmax' in kwargs:
+                self.tmax = kwargs['tmax']
+                self.tmin = self.tmax - self.t
+            else:
+                self.tmin = (-1) * self.t / 2
+                self.tmax = self.t / 2
+                
+    def loc_to_z(self, loc) -> float:
+        """
+        Returns height of a local point by linear interpolation.
+        Local coordinate is expected between -1 and 1.
+        """
+        return 0.5 * ((self.tmax + self.tmin) + loc * (self.tmax - self.tmin))
+
+    @abstractmethod
+    def stiffness_matrix(self):
+        raise NotImplementedError
+    
+    
+class Surface(MetaSurface):
+    """
+    Helper base class for laminates.
+    """
+
+    __layerclass__ = Layer
+
+    def Layer(self, *args, **kwargs):
+        """
+        Returns a Layer compatible with the model.
+        """
+        return self.__layerclass__(*args, **kwargs)
+    
+    def Hooke(self):
+        raise NotImplementedError
+
+    def layers(self) -> Iterable:
+        """
+        Returns the layers of the laminate.
+        """
+        return [layer for layer in self.containers(dtype=self.__layerclass__)]
+
+    def iterlayers(self):
+        """
+        Returns the layers of the laminate as a generator.
+        """
+        return self.containers(dtype=self.__layerclass__)
+
+    def stiffness_matrix(self) -> np.ndarray:
+        """
+        Assembles and returns the stiffness matrix.
+        """
+        self._set_layers()
+        res = np.zeros(self.__layerclass__.__shape__)
+        for layer in self.iterlayers():
+            res += layer.stiffness_matrix()
+        return res
+
+    def _set_layers(self):
+        """
+        Sets thickness ranges for the layers.
+        """
+        layers = self.layers()
+        t = sum([layer.t for layer in layers])
+        layers[0].tmin = -t/2
+        nLayers = len(layers)
+        for i in range(nLayers-1):
+            layers[i].tmax = layers[i].tmin + layers[i].t
+            layers[i+1].tmin = layers[i].tmax
+        layers[-1].tmax = t/2
+        for layer in layers:
+            layer.zi = [layer.loc_to_z(l_) for l_ in layer.__loc__]
+        return True
+    
+    @classmethod
+    def from_dict(cls, d: dict = None, **kwargs) -> 'Surface':  
+        res = cls(**d)
+        for addr, value in parsedicts_addr(d, inclusive=True):
+            if len(addr) == 0:
+                continue
+            if 'hooke' in value:
+                subcls = cls.__layerclass__
+            else: 
+                continue
+            value['key'] = addr[-1]
+            res[addr] = subcls(**value)
+        return res
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/material/surface/mindlin.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/mindlin/mindlin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,323 +1,330 @@
-from typing import Tuple, Union, Callable
-import numpy as np
-from numpy import ndarray
-from numpy.linalg import inv
-import sympy as sy
-
-from ..hooke.utils import _get_elastic_params
-from ..hooke.sym import smat_sym_ortho_3d
-
-from .meta import Surface, SurfaceLayer
-
-
-__all__ = ["MindlinShell", "MindlinPlate", "MindlinShellLayer", "MindlinPlateLayer"]
-
-
-class MindlinShellLayer(SurfaceLayer):
-    """
-    Helper object for the stress analysis of a layer of a shell.
-    """
-
-    __loc__ = [-1.0, 0.0, 1.0]
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        # locations of discrete points along the thickness
-        self.zi = [self.loc_to_z(loc) for loc in MindlinShellLayer.__loc__]
-
-        # Shear factors have to be multiplied by shear force to obtain shear
-        # stress. They are determined externaly at discrete points, which
-        # are later used for interpolation.
-        self.shear_factors_x = np.array([0.0, 0.0, 0.0])
-        self.shear_factors_y = np.array([0.0, 0.0, 0.0])
-
-        # polinomial coefficients for shear factor interpoaltion
-        self.sfx = None
-        self.sfy = None
-
-    def material_elastic_stiffness_matrices(self) -> Tuple[ndarray, ndarray]:
-        """
-        Returns and stores transformed material stiffness matrices.
-        """
-        Cm = self.hooke
-        Cm_126 = Cm[0:3, 0:3]
-        Cm_45 = Cm[3:, 3:]
-        T_126, T_45 = self.rotation_matrices()
-        R_126 = np.diag([1, 1, 2])
-        R_45 = np.diag([2, 2])
-        C_126 = T_126 @ Cm_126 @ inv(R_126) @ T_126.T @ R_126
-        C_45 = T_45 @ Cm_45 @ inv(R_45) @ T_45.T @ R_45
-        C_126[np.abs(C_126) < 1e-12] = 0.0
-        C_45[np.abs(C_45) < 1e-12] = 0.0
-        self.C_126 = C_126
-        self.C_45 = C_45
-        return C_126, C_45
-
-    def rotation_matrices(self) -> Tuple[ndarray, ndarray]:
-        """
-        Produces transformation matrices T_126 and T_45.
-        """
-        T_126 = np.zeros([3, 3])
-        T_45 = np.zeros([2, 2])
-        angle = self.angle * np.pi / 180
-        #
-        T_126[0, 0] = np.cos(angle) ** 2
-        T_126[0, 1] = np.sin(angle) ** 2
-        T_126[0, 2] = -np.sin(2 * angle)
-        T_126[1, 0] = T_126[0, 1]
-        T_126[1, 1] = T_126[0, 0]
-        T_126[1, 2] = -T_126[0, 2]
-        T_126[2, 0] = np.cos(angle) * np.sin(angle)
-        T_126[2, 1] = -T_126[2, 0]
-        T_126[2, 2] = np.cos(angle) ** 2 - np.sin(angle) ** 2
-        #
-        T_45[0, 0] = np.cos(angle)
-        T_45[0, 1] = -np.sin(angle)
-        T_45[1, 1] = T_45[0, 0]
-        T_45[1, 0] = -T_45[0, 1]
-        #
-        return T_126, T_45
-
-    def elastic_stiffness_matrix(self) -> ndarray:
-        """
-        Returns the uncorrected stiffness contribution to the layer.
-        """
-        C_126, C_45 = self.material_elastic_stiffness_matrices()
-        tmin = self.tmin
-        tmax = self.tmax
-        A = C_126 * (tmax - tmin)
-        B = (1 / 2) * C_126 * (tmax**2 - tmin**2)
-        D = (1 / 3) * C_126 * (tmax**3 - tmin**3)
-        S = C_45 * (tmax - tmin)
-        ABDS = np.zeros([8, 8])
-        ABDS[0:3, 0:3] = A
-        ABDS[0:3, 3:6] = B
-        ABDS[3:6, 0:3] = B
-        ABDS[3:6, 3:6] = D
-        ABDS[6:8, 6:8] = S
-        return ABDS
-
-    def compile_shear_factors(self):
-        """
-        Prepares data for continuous interpolation of shear factors. Should
-        be called if shear factors are already set.
-        """
-        coeff_inv = np.linalg.inv(np.array([[1, z, z**2] for z in self.zi]))
-        self.sfx = np.matmul(coeff_inv, self.shear_factors_x)
-        self.sfy = np.matmul(coeff_inv, self.shear_factors_y)
-
-    def loc_to_shear_factors(self, loc: float):
-        """
-        Returns shear factor for local z direction by quadratic interpolation.
-        Local coordinate is expected between -1 and 1.
-        """
-        z = self.loc_to_z(loc)
-        monoms = np.array([1, z, z**2])
-        return np.dot(monoms, self.sfx), np.dot(monoms, self.sfy)
-
-    def approxfunc(self, data) -> Callable:
-        z0, z1, z2 = self.zi
-        z = np.array([[1, z0, z0**2], [1, z1, z1**2], [1, z2, z2**2]])
-        a, b, c = np.linalg.inv(z) @ np.array(data)
-        return lambda z: a + b * z + c * z**2
-
-
-class MindlinPlateLayer(MindlinShellLayer):
-    """
-    Helper object for the stress analysis of a layer of a plate.
-    """
-
-    def elastic_stiffness_matrix(self) -> ndarray:
-        """
-        Returns the uncorrected stiffness contribution to the layer.
-        """
-        C_126, C_45 = self.material_elastic_stiffness_matrices()
-        tmin = self.tmin
-        tmax = self.tmax
-        D = (1 / 3) * C_126 * (tmax**3 - tmin**3)
-        S = C_45 * (tmax - tmin)
-        ABDS = np.zeros([5, 5])
-        ABDS[:3, :3] = D
-        ABDS[3:, 3:] = S
-        return ABDS
-
-
-class MindlinShell(Surface):
-    """
-    Helper object for the stress analysis of a shell.
-
-    Example
-    -------
-    >>> from sigmaepsilon.material import MindlinShell
-    >>> model = {
-    >>>     '0' : {
-    >>>         'hooke' : MindlinShell.Hooke(E=2100000, nu=0.3),
-    >>>         'angle' : 0.,
-    >>>         'thickness' : 0.1
-    >>>         },
-    >>>     }
-    >>> C = MindlinShell.from_dict(model).elastic_stiffness_matrix()
-    """
-
-    __layerclass__ = MindlinShellLayer
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    @classmethod
-    def Hooke(cls, symbolic: bool = False, **kwargs) -> Union[sy.Matrix, np.ndarray]:
-        """
-        Returns a Hooke matrix appropriate for shells.
-
-        Parameters
-        ----------
-        symbolic : bool, Optional
-            If Truem a symbolic matrix is returned.
-
-        Returns
-        -------
-        Union[sympy.Matrix, numpy.ndarray]
-            The matrix in symbolic or numeric form.
-
-        Examples
-        --------
-        >>> from sigmaepsilon.material import MindlinShell
-        >>> MindlinShell.Hooke(E=2100000, nu=0.3)
-        >>> MindlinShell.Hooke(symbolic=True)
-        """
-        S = smat_sym_ortho_3d()
-        S.row_del(2)
-        S.col_del(2)
-
-        if symbolic:
-            return S.inv()
-
-        constants = _get_elastic_params(**kwargs)
-        subs = {s: constants[str(s)] for s in S.free_symbols}
-        S = S.subs([(sym, val) for sym, val in subs.items()])
-        S = np.array(S, dtype=float)
-        return np.linalg.inv(S)
-
-    def elastic_stiffness_matrix(self) -> ndarray:
-        """
-        Returns the stiffness matrix of the shell.
-
-        Returns
-        -------
-        numpy.ndarray
-            The ABDS matrix of the shell.
-        """
-        ABDS = super().elastic_stiffness_matrix()
-        layers = self.layers()
-        A11 = ABDS[0, 0]
-        B11 = ABDS[0, 3]
-        D11 = ABDS[3, 3]
-        S55 = ABDS[6, 6]
-        A22 = ABDS[1, 1]
-        B22 = ABDS[1, 4]
-        D22 = ABDS[4, 4]
-        S44 = ABDS[7, 7]
-        eta_x = 1 / (A11 * D11 - B11**2)
-        eta_y = 1 / (A22 * D22 - B22**2)
-
-        # Create shear factors. These need to be multiplied with the shear
-        # force in order to obtain shear stress at a given height. Since the
-        # shear stress distribution is of 2nd order, the factors are
-        # determined at 3 locations per layer.
-        for i, layer in enumerate(layers):
-            zi = layer.zi
-            Exi = layer.C_126[0, 0]
-            Eyi = layer.C_126[1, 1]
-
-            # first point through the thickness
-            layer.shear_factors_x[0] = layers[i - 1].shear_factors_x[-1]
-            layer.shear_factors_y[0] = layers[i - 1].shear_factors_y[-1]
-
-            # second point through the thickness
-            layer.shear_factors_x[1] = layer.shear_factors_x[0] - eta_x * Exi * (
-                0.5 * (zi[1] ** 2 - zi[0] ** 2) * A11 - (zi[1] - zi[0]) * B11
-            )
-            layer.shear_factors_y[1] = layer.shear_factors_y[0] - eta_y * Eyi * (
-                0.5 * (zi[1] ** 2 - zi[0] ** 2) * A22 - (zi[1] - zi[0]) * B22
-            )
-
-            # third point through the thickness
-            layer.shear_factors_x[2] = layer.shear_factors_x[0] - eta_x * Exi * (
-                0.5 * (zi[2] ** 2 - zi[0] ** 2) * A11 - (zi[2] - zi[0]) * B11
-            )
-            layer.shear_factors_y[2] = layer.shear_factors_y[0] - eta_y * Eyi * (
-                0.5 * (zi[2] ** 2 - zi[0] ** 2) * A22 - (zi[2] - zi[0]) * B22
-            )
-
-        # remove numerical junk from the end
-        layers[-1].shear_factors_x[-1] = 0.0
-        layers[-1].shear_factors_y[-1] = 0.0
-
-        # prepare data for interpolation of shear stresses in a layer
-        for layer in layers:
-            layer.compile_shear_factors()
-
-        # potential energy using constant stress distribution
-        # and unit shear force
-        pot_c_x = 0.5 / S55
-        pot_c_y = 0.5 / S44
-
-        # positions and weights of Gauss-points
-        gP = np.array([-np.sqrt(3 / 5), 0, np.sqrt(3 / 5)])
-        gW = np.array([5 / 9, 8 / 9, 5 / 9])
-
-        # potential energy using parabolic stress distribution
-        # and unit shear force
-        pot_p_x, pot_p_y = 0.0, 0.0
-        for layer in layers:
-            dJ = 0.5 * (layer.tmax - layer.tmin)
-            Gxi = layer.C_45[0, 0]
-            Gyi = layer.C_45[1, 1]
-            for loc, weight in zip(gP, gW):
-                sfx, sfy = layer.loc_to_shear_factors(loc)
-                pot_p_x += 0.5 * (sfx**2) * dJ * weight / Gxi
-                pot_p_y += 0.5 * (sfy**2) * dJ * weight / Gyi
-        kx = pot_c_x / pot_p_x
-        ky = pot_c_y / pot_p_y
-
-        ABDS[6, 6] = kx * S55
-        ABDS[7, 7] = ky * S44
-        self.kx = kx
-        self.ky = ky
-        self.ABDS = ABDS
-        self.SDBA = np.linalg.inv(ABDS)
-        return ABDS
-
-
-class MindlinPlate(MindlinShell):
-    """
-    Helper object for the stress analysis of a membrane.
-
-    Example
-    -------
-    >>> from sigmaepsilon.model import MindlinPlate
-    >>> model = {
-    >>>     '0' : {
-    >>>         'hooke' : MindlinPlate.Hooke(E=2100000, nu=0.3),
-    >>>         'angle' : 0.,
-    >>>         'thickness' : 0.1
-    >>>         },
-    >>>     }
-    >>> C = MindlinPlate.from_dict(model).elastic_stiffness_matrix()
-    """
-
-    def elastic_stiffness_matrix(self) -> ndarray:
-        """
-        Returns the stiffness matrix of the plate.
-
-        Returns
-        -------
-        numpy.ndarray
-            The ABDS matrix of the plate.
-        """
-        ABDS_ = super().elastic_stiffness_matrix()
-        ABDS = np.zeros([5, 5])
-        ABDS[:3, :3] = ABDS_[3:6, 3:6]
-        ABDS[3:, 3:] = ABDS_[6:8, 6:8]
-        return ABDS
+# -*- coding: utf-8 -*-
+from typing import Tuple, Union, Callable
+import numpy as np
+from numpy import ndarray
+from numpy.linalg import inv
+import sympy as sy
+
+from ...material.hooke.utils import group_mat_params, get_iso_params
+from ...material.hooke.sym import smat_sym_ortho_3d
+
+from ..metashell import Surface, Layer
+
+
+__all__ = ['MindlinShell']
+
+
+class MindlinShellLayer(Layer):
+    """
+    Helper object for the stress analysis of a layer of a shell.
+    """
+
+    __loc__ = [-1., 0., 1.]
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # locations of discrete points along the thickness
+        self.zi = [self.loc_to_z(loc) for loc in MindlinShellLayer.__loc__]
+
+        # Shear factors have to be multiplied by shear force to obtain shear
+        # stress. They are determined externaly at discrete points, which
+        # are later used for interpolation.
+        self.shear_factors_x = np.array([0., 0., 0.])
+        self.shear_factors_y = np.array([0., 0., 0.])
+
+        # polinomial coefficients for shear factor interpoaltion
+        self.sfx = None
+        self.sfy = None
+
+    def material_stiffness_matrices(self) -> Tuple[ndarray, ndarray]:
+        """
+        Returns and stores transformed material stiffness matrices.
+        """
+        Cm = self.hooke
+        Cm_126 = Cm[0:3, 0:3]
+        Cm_45 = Cm[3:, 3:]
+        T_126, T_45 = self.rotation_matrices()
+        R_126 = np.diag([1, 1, 2])
+        R_45 = np.diag([2, 2])  
+        C_126 = T_126 @ Cm_126 @ inv(R_126) @ T_126.T @ R_126
+        C_45 = T_45 @ Cm_45 @ inv(R_45) @ T_45.T @ R_45    
+        C_126[np.abs(C_126) < 1e-12] = 0.0
+        C_45[np.abs(C_45) < 1e-12] = 0.0
+        self.C_126 = C_126
+        self.C_45 = C_45
+        return C_126, C_45
+
+    def rotation_matrices(self) -> Tuple[ndarray, ndarray]:
+        """
+        Produces transformation matrices T_126 and T_45.
+        """
+        T_126 = np.zeros([3, 3])
+        T_45 = np.zeros([2, 2])
+        angle = self.angle * np.pi/180
+        #
+        T_126[0, 0] = np.cos(angle)**2
+        T_126[0, 1] = np.sin(angle)**2
+        T_126[0, 2] = -np.sin(2*angle)
+        T_126[1, 0] = T_126[0, 1]
+        T_126[1, 1] = T_126[0, 0]
+        T_126[1, 2] = -T_126[0, 2]
+        T_126[2, 0] = np.cos(angle)*np.sin(angle)
+        T_126[2, 1] = -T_126[2, 0]
+        T_126[2, 2] = np.cos(angle)**2 - np.sin(angle)**2
+        #
+        T_45[0, 0] = np.cos(angle)
+        T_45[0, 1] = -np.sin(angle)
+        T_45[1, 1] = T_45[0, 0]
+        T_45[1, 0] = -T_45[0, 1]
+        #
+        return T_126, T_45
+
+    def stiffness_matrix(self) -> ndarray:
+        """
+        Returns the uncorrected stiffness contribution to the layer.
+        """
+        C_126, C_45 = self.material_stiffness_matrices()
+        tmin = self.tmin
+        tmax = self.tmax
+        A = C_126*(tmax - tmin)
+        B = (1/2)*C_126*(tmax**2 - tmin**2)
+        D = (1/3)*C_126*(tmax**3 - tmin**3)
+        S = C_45*(tmax - tmin)
+        ABDS = np.zeros([8, 8])
+        ABDS[0:3, 0:3] = A
+        ABDS[0:3, 3:6] = B
+        ABDS[3:6, 0:3] = B
+        ABDS[3:6, 3:6] = D
+        ABDS[6:8, 6:8] = S
+        return ABDS
+
+    def compile_shear_factors(self):
+        """
+        Prepares data for continuous interpolation of shear factors. Should
+        be called if shear factors are already set.
+        """
+        coeff_inv = np.linalg.inv(np.array([[1, z, z**2] for z in self.zi]))
+        self.sfx = np.matmul(coeff_inv, self.shear_factors_x)
+        self.sfy = np.matmul(coeff_inv, self.shear_factors_y)
+
+    def loc_to_shear_factors(self, loc: float):
+        """
+        Returns shear factor for local z direction by quadratic interpolation.
+        Local coordinate is expected between -1 and 1.
+        """
+        z = self.loc_to_z(loc)
+        monoms = np.array([1, z, z**2])
+        return np.dot(monoms, self.sfx), np.dot(monoms, self.sfy)
+
+    def approxfunc(self, data) -> Callable:
+        z0, z1, z2 = self.zi
+        z = np.array([[1, z0, z0**2], [1, z1, z1**2], [1, z2, z2**2]])
+        a, b, c = np.linalg.inv(z) @ np.array(data)
+        return lambda z: a + b*z + c*z**2
+
+
+class MindlinPlateLayer(MindlinShellLayer):
+    """
+    Helper object for the stress analysis of a layer of a plate.
+    """
+
+    def stiffness_matrix(self) -> ndarray:
+        """
+        Returns the uncorrected stiffness contribution to the layer.
+        """
+        C_126, C_45 = self.material_stiffness_matrices()
+        tmin = self.tmin
+        tmax = self.tmax
+        D = (1/3)*C_126*(tmax**3 - tmin**3)
+        S = C_45*(tmax - tmin)
+        ABDS = np.zeros([5, 5])
+        ABDS[:3, :3] = D
+        ABDS[3:, 3:] = S
+        return ABDS
+
+
+class MindlinShell(Surface):
+    """
+    Helper object for the stress analysis of a shell.
+    
+    Example
+    -------
+    >>> from sigmaepsilon.solid.model import MindlinShell as Model
+    >>> model = {
+    >>>     '0' : {
+    >>>         'hooke' : Model.Hooke(E=2100000, nu=0.3),
+    >>>         'angle' : 0., 
+    >>>         'thickness' : 0.1
+    >>>         },
+    >>>     }
+    >>> C = Model.from_dict(model).stiffness_matrix()
+    
+    """
+    
+    __layerclass__ = MindlinShellLayer
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        
+    @classmethod    
+    def Hooke(cls, *args, symbolic=False, **kwargs) -> Union[sy.Matrix, np.ndarray]:
+        """
+        Returns a Hooke matrix appropriate for shells.
+        
+        Parameters
+        ----------
+        symbolic : bool, Optional
+            If Truem a symbolic matrix is returned.
+        
+        Returns
+        -------
+        Union[sympy.Matrix, numpy.ndarray]
+            The matrix in symbolic or numeric form.
+            
+        Examples
+        --------
+        >>> from sigmaepsilon.solid.model import MindlinShell as Model
+        >>> Model.Hooke(E=2100000, nu=0.3)
+        
+        >>> Model.Hooke(symbolic=True)
+        
+        """
+        if symbolic:
+            S = smat_sym_ortho_3d()
+            S.row_del(2)
+            S.col_del(2) 
+            return S
+        else:
+            E, NU, G = group_mat_params(**kwargs)
+            nE, nNU, nG = len(E), len(NU), len(G)
+            nParams = sum([nE, nNU, nG])
+            if nParams == 2:
+                constants = get_iso_params(**E, **NU, **G)
+            S = cls.Hooke(symbolic=True)
+            subs = {s : constants[str(s)] for s in S.free_symbols}
+            S = S.subs([(sym, val) for sym, val in subs.items()])
+            S = np.array(S, dtype=float)
+            return np.linalg.inv(S)
+
+    def stiffness_matrix(self) -> ndarray:
+        """
+        Returns the stiffness matrix of the shell.
+                
+        Returns
+        -------
+        numpy.ndarray
+            The ABDS matrix of the shell.
+            
+        """
+        ABDS = super().stiffness_matrix()
+        layers = self.layers()
+        A11 = ABDS[0, 0]
+        B11 = ABDS[0, 3]
+        D11 = ABDS[3, 3]
+        S55 = ABDS[6, 6]
+        A22 = ABDS[1, 1]
+        B22 = ABDS[1, 4]
+        D22 = ABDS[4, 4]
+        S44 = ABDS[7, 7]
+        eta_x = 1/(A11*D11-B11**2)
+        eta_y = 1/(A22*D22-B22**2)
+
+        # Create shear factors. These need to be multiplied with the shear
+        # force in order to obtain shear stress at a given height. Since the
+        # shear stress distribution is of 2nd order, the factors are
+        # determined at 3 locations per layer.
+        for i, layer in enumerate(layers):
+            zi = layer.zi
+            Exi = layer.C_126[0, 0]
+            Eyi = layer.C_126[1, 1]
+
+            # first point through the thickness
+            layer.shear_factors_x[0] = layers[i-1].shear_factors_x[-1]
+            layer.shear_factors_y[0] = layers[i-1].shear_factors_y[-1]
+
+            # second point through the thickness
+            layer.shear_factors_x[1] = layer.shear_factors_x[0] - \
+                eta_x*Exi*(0.5*(zi[1]**2-zi[0]**2)*A11-(zi[1]-zi[0])*B11)
+            layer.shear_factors_y[1] = layer.shear_factors_y[0] - \
+                eta_y*Eyi*(0.5*(zi[1]**2-zi[0]**2)*A22-(zi[1]-zi[0])*B22)
+
+            # third point through the thickness
+            layer.shear_factors_x[2] = layer.shear_factors_x[0] - \
+                eta_x*Exi*(0.5*(zi[2]**2-zi[0]**2)*A11-(zi[2]-zi[0])*B11)
+            layer.shear_factors_y[2] = layer.shear_factors_y[0] - \
+                eta_y*Eyi*(0.5*(zi[2]**2-zi[0]**2)*A22-(zi[2]-zi[0])*B22)
+
+        # remove numerical junk from the end
+        layers[-1].shear_factors_x[-1] = 0.
+        layers[-1].shear_factors_y[-1] = 0.
+
+        # prepare data for interpolation of shear stresses in a layer
+        for layer in layers:
+            layer.compile_shear_factors()
+
+        # potential energy using constant stress distribution
+        # and unit shear force
+        pot_c_x = 0.5/S55
+        pot_c_y = 0.5/S44
+
+        # positions and weights of Gauss-points
+        gP = np.array([-np.sqrt(3/5), 0, np.sqrt(3/5)])
+        gW = np.array([5/9, 8/9, 5/9])
+
+        # potential energy using parabolic stress distribution
+        # and unit shear force
+        pot_p_x, pot_p_y = 0., 0.
+        for layer in layers:
+            dJ = 0.5*(layer.tmax - layer.tmin)
+            Gxi = layer.C_45[0, 0]
+            Gyi = layer.C_45[1, 1]
+            for loc, weight in zip(gP, gW):
+                sfx, sfy = layer.loc_to_shear_factors(loc)
+                pot_p_x += 0.5*(sfx**2)*dJ*weight/Gxi
+                pot_p_y += 0.5*(sfy**2)*dJ*weight/Gyi
+        kx = pot_c_x/pot_p_x
+        ky = pot_c_y/pot_p_y
+
+        ABDS[6, 6] = kx * S55
+        ABDS[7, 7] = ky * S44
+        self.kx = kx
+        self.ky = ky
+        self.ABDS = ABDS
+        self.SDBA = np.linalg.inv(ABDS)
+        return ABDS
+
+
+class MindlinPlate(MindlinShell):
+    """
+    Helper object for the stress analysis of a membrane.
+    
+    Example
+    -------
+    >>> from sigmaepsilon.solid.model import MindlinPlate as Model
+    >>> model = {
+    >>>     '0' : {
+    >>>         'hooke' : Model.Hooke(E=2100000, nu=0.3),
+    >>>         'angle' : 0., 
+    >>>         'thickness' : 0.1
+    >>>         },
+    >>>     }
+    >>> C = Model.from_dict(model).stiffness_matrix()
+    
+    """
+    
+    def stiffness_matrix(self) -> ndarray:
+        """
+        Returns the stiffness matrix of the plate.
+                
+        Returns
+        -------
+        numpy.ndarray
+            The ABDS matrix of the plate.
+            
+        """
+        ABDS_ = super().stiffness_matrix()
+        ABDS = np.zeros([5, 5])
+        ABDS[:3, :3] = ABDS_[3:6, 3:6]
+        ABDS[3:, 3:] = ABDS_[6:8, 6:8]
+        return ABDS
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/topopt/oc/filter.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/oc/filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,33 @@
-from numba import njit, prange
-import numpy as np
-from numba.typed import Dict as nbDict
-
-from neumann.linalg.sparse.csr import csr_matrix as csr
-
-__cache = True
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def sensitivity_filter(
-    sens: np.ndarray, dens: np.ndarray, neighbours: nbDict, factors: dict
-):
-    nE = len(dens)
-    res = np.zeros_like(sens)
-    inds = np.arange(nE).astype(np.int64)
-    for iE in prange(nE):
-        adj = neighbours[inds[iE]]
-        res[inds[iE]] = np.sum(factors[inds[iE]] * dens[adj] * sens[adj]) / (
-            dens[inds[iE]] * np.sum(factors[inds[iE]])
-        )
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def sensitivity_filter_csr(
-    sens: np.ndarray, dens: np.ndarray, neighbours: csr, factors: dict
-):
-    nE = len(dens)
-    res = np.zeros_like(sens)
-    for iE in prange(nE):
-        adj, _ = neighbours.row(iE)
-        res[iE] = np.sum(factors[iE] * dens[adj] * sens[adj]) / (
-            dens[iE] * np.sum(factors[iE])
-        )
-    return res
+# -*- coding: utf-8 -*-
+from numba import njit, prange
+import numpy as np
+from numba.typed import Dict as nbDict
+
+from neumann.linalg.sparse.csr import csr_matrix as csr
+
+__cache = True
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def sensitivity_filter(sens: np.ndarray, dens: np.ndarray,
+                       neighbours: nbDict, factors: dict):
+    nE = len(dens)
+    res = np.zeros_like(sens)
+    inds = np.arange(nE).astype(np.int64)
+    for iE in prange(nE):
+        adj = neighbours[inds[iE]] 
+        res[inds[iE]] = np.sum(factors[inds[iE]] * dens[adj] * sens[adj]) / \
+            (dens[inds[iE]] * np.sum(factors[inds[iE]]))
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def sensitivity_filter_csr(sens: np.ndarray, dens: np.ndarray,
+                           neighbours: csr, factors: dict):
+    nE = len(dens)
+    res = np.zeros_like(sens)
+    for iE in prange(nE):
+        adj, _ = neighbours.row(iE)
+        res[iE] = np.sum(factors[iE] * dens[adj] * sens[adj]) / \
+            (dens[iE] * np.sum(factors[iE]))
+    return res
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/topopt/oc/oc.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/topopt/oc/oc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,255 +1,259 @@
-import numpy as np
-from numpy import ndarray
-from copy import deepcopy
-from typing import NamedTuple, Iterable
-
-from neumann.linalg.sparse import csr_matrix as csr
-from polymesh.utils import cells_around
-from sigmaepsilon.fem.structure import Structure
-from sigmaepsilon.fem.femsolver import StaticSolver
-
-from .filter import sensitivity_filter, sensitivity_filter_csr
-from .utils import (
-    get_filter_factors,
-    get_filter_factors_csr,
-    weighted_stiffness_flat as weighted_stiffness,
-    element_stiffness_ranges,
-)
-from ...utils.fem.postproc import element_compliances_flat as element_compliances
-
-
-class OptRes(NamedTuple):
-    x: Iterable  # the design variables
-    obj: float  # the actual value of the objective function
-    vol: float  # the actual volume
-    pen: float  # the actual value of the penalty
-    n: int  # the number of iterations completed
-
-
-def maximize_stiffness(
-    structure: Structure,
-    *_,
-    miniter: int = 50,
-    maxiter: int = 100,
-    p_start: float = 1.0,
-    p_stop: float = 3.0,
-    p_inc: float = 0.2,
-    p_step: int = 5,
-    q: float = 0.5,
-    vfrac: float = 0.6,
-    dtol: float = 0.1,
-    r_max: float = None,
-    penalty: float = None,
-    nostop: bool = True,
-    neighbours: Iterable = None,
-    guess: Iterable = None,
-    i_start: int = 0,
-    **__
-) -> OptRes:
-    """
-    Performs topology optimization using an Optimality Criteria Method to
-    maximize the stiffness of a structure, given a design space and a certain 
-    amount of material to distribute.
-    
-    .. math::
-        :nowrap:
-        
-        \\begin{equation}
-            \\begin{array}{rrclcl}
-            \\displaystyle \\min_{\\boldsymbol{\\rho}} & \\mathbf{u(\\boldsymbol{\\rho})}^T \\mathbf{f} \\\\
-            \\textrm{s. t.} \\\\
-            & \\mathbf{K}(\\boldsymbol{\\rho}) \\mathbf{u(\\boldsymbol{\\rho})} & = & \\mathbf{f} \\\\
-            & V(\\boldsymbol{\\rho}) - \\eta V_0 & \\leq & 0 & & \\\\
-            & \\rho_i \\in \\{0, 1\\} & & & & \\forall i \\in N
-            \\end{array}
-        \\end{equation}
-    
-    Parameters
-    ----------
-    structure : Structure
-        An instance of sigmaepsilon.fem.Structure.
-    miniter : int, Optional
-        The minimum number of iterations to perform. Default is 50.
-    maxiter : int, Optional
-        The maximum number of iterations to perform. Default is 100.
-    p_start : float, Optional
-        Initial value of the penalty on intermediate densities. Default is 1.
-    p_stop : float, Optional
-        Final value of the penalty on intermediate densities. Default is 3.
-    p_inc : float, Optional
-        Increment of the penalty on intermediate densities. Default is 0.2
-    p_step : int, Optional
-        The number of interations it takes to increment the penalty on intermediate
-        density values. Default is 5.
-    q : float, Optional
-        Smoothing factor. Defaul is 0.5. 
-    vfrac : float, Optional
-        The fraction of available volume and the volume of the virgin structure.
-        Default is 0.6. 
-    dtol : float, Optional
-        This controls the maximum change in the value of a design variable. 
-        Default is 0.1. 
-    r_max : float, Optional
-        Radius for filtering. Default is None.
-    neighbours : float, Optional
-        The neighbours of the cells for filtering. Default is None.
-    guess : numpy.ndarray, Optional
-        A guess on the solution. This parameter can be used to contiue
-        a workflow. Default is None.  
-    i_start : int, Optional
-        Starting index for iterations. This parameter can be used to contiue
-        a workflow. Default is 0.
-    summary : bool, Optional
-        If True, a short summary about execution time and the number of iterations
-        is available after execution as `structure.summary['topopt']`. Default is False.
-    nostop : bool, Optional
-        If True, iterations neglect all stopping criteria, those govern by 
-        mniniter and maxiter included.
-        Default is False.
-    
-    Yields
-    ------
-    OptRes
-        The results of the actual iteration.
-        
-    Notes
-    -----
-    - The function returns a generator expression.
-    - This function can be used for both size and topology optimization,
-      depending on the inputs.
-    """
-    do_filter = r_max is not None
-
-    if structure._static_solver_ is None:
-        structure.linear_static_analysis()
-    femsolver: StaticSolver = structure._static_solver_.core
-    assert femsolver.regular
-    krows, kcols = femsolver.krows, femsolver.kcols
-    kshape = femsolver.kshape
-    kranges = element_stiffness_ranges(kshape)
-    K_virgin = np.copy(femsolver.K_bulk.flatten())
-    mesh = structure.mesh
-    vols = mesh.volumes()
-    centers = mesh.centers()
-
-    # initial solution to set up parameters
-    dens = np.zeros_like(vols)
-    dens_tmp = np.zeros_like(dens)
-    dens_tmp_ = np.zeros_like(dens)
-    dCdx = np.zeros_like(dens)
-    comps = np.zeros_like(dens)
-
-    def get_dof_solution():
-        U = femsolver.u
-        dU = len(U.shape)
-        if dU == 2:
-            # multiple load cases
-            return U[:, 0]
-        return U
-
-    def compliance(update_stiffness: bool = False) -> ndarray:
-        if update_stiffness:
-            femsolver.update_stiffness(weighted_stiffness(K_virgin, dens, kranges))
-        femsolver._proc_()
-        U = get_dof_solution()
-        comps[:] = element_compliances(K_virgin, U, krows, kcols, kranges)
-        np.clip(comps, 1e-7, None, out=comps)
-        return np.sum(comps)
-
-    # ------------------ INITIAL SOLUTION ---------------
-    comp = compliance()
-    vol = np.sum(vols)
-    vol_start = vol
-    vol_min = vfrac * vol_start
-
-    # initialite filter
-    if do_filter:
-        if neighbours is None:
-            neighbours = cells_around(centers, r_max, frmt="dict")
-        if isinstance(neighbours, csr):
-            factors = get_filter_factors_csr(centers, neighbours, r_max)
-            fltr = sensitivity_filter_csr
-        else:
-            factors = get_filter_factors(centers, neighbours, r_max)
-            fltr = sensitivity_filter
-
-    # initialize penalty parameters
-    if penalty is not None:
-        p_start = penalty
-        p_stop = penalty + 1
-        p_step = maxiter + 1
-
-    # ------------- INITIAL FEASIBLE SOLUTION ------------
-    if guess is None:
-        dens[:] = vfrac
-    else:
-        dens = deepcopy(guess)
-    vol = np.sum(dens * vols)
-    comp = compliance(update_stiffness=True)
-    cIter = i_start
-    p = p_start
-    yield OptRes(dens, comp, vol, p, cIter)
-
-    # ------------------- ITERATION -------------------
-    terminate = False
-    while not terminate:
-        if (p < p_stop) and (np.mod(cIter, p_step) == 0):
-            p += p_inc
-
-        # estimate lagrangian
-        lagr = p * comp / vol
-
-        # set up boundaries of change
-        _dens = dens * (1 - dtol)
-        np.clip(_dens, 1e-5, 1.0, out=_dens)
-        dens_ = dens * (1 + dtol)
-        np.clip(dens_, 1e-5, 1.0, out=dens_)
-
-        # sensitivity [*(-1)]
-        dCdx[:] = p * comps * dens ** (p - 1)
-
-        # sensitivity filter
-        if do_filter:
-            dCdx[:] = fltr(dCdx, dens, neighbours, factors)
-
-        # calculate new densities and lagrangian
-        dens_tmp_[:] = dens * (dCdx / vols) ** q
-        dens_tmp[:] = dens_tmp_
-        _lagr = 0
-        lagr_ = 2 * lagr
-        _maxtries = 200
-        _ntries = 0
-        while (lagr_ - _lagr) > 1e-3:
-            if _ntries == _maxtries:
-                raise RuntimeError("Couldn't find multiplier :(.")
-            _lagr_ = (_lagr + lagr_) / 2
-            dens_tmp[:] = dens_tmp_ / (_lagr_**q)
-            np.clip(dens_tmp, _dens, dens_, out=dens_tmp)
-            vol_tmp = np.sum(dens_tmp * vols)
-            if vol_tmp < vol_min:
-                lagr_ = _lagr_
-            else:
-                _lagr = _lagr_
-            _ntries += 1
-        lagr = lagr_
-        dens[:] = dens_tmp
-
-        # resolve equilibrium equations and calculate compliance
-        comp = compliance(update_stiffness=True)
-        vol = np.sum(dens * vols)
-        cIter += 1
-        res = OptRes(dens, comp, vol, p, cIter)
-        yield res
-
-        if nostop:
-            terminate = False
-        else:
-            if cIter < miniter:
-                terminate = False
-            elif cIter >= maxiter:
-                terminate = True
-            else:
-                terminate = p >= p_stop
-
-    femsolver.update_stiffness(K_virgin)
-    return OptRes(dens, comp, vol, p, cIter)
+# -*- coding: utf-8 -*-
+import numpy as np
+from copy import deepcopy
+from typing import NamedTuple, Iterable
+
+from neumann.linalg.sparse.csr import csr_matrix as csr
+from polymesh.utils import cells_around
+from sigmaepsilon.solid.fem.structure import Structure
+
+from .filter import sensitivity_filter, sensitivity_filter_csr
+from .utils import (compliances_bulk, get_filter_factors,
+                    get_filter_factors_csr,
+                    weighted_stiffness_bulk as weighted_stiffness)
+
+
+class OptRes(NamedTuple):
+    """
+    A tuple collecting information about an iteration block.
+            
+    """
+    x : Iterable
+    obj : float
+    vol : float
+    pen : float
+    n : int
+
+
+def maximize_stiffness(structure: Structure, *args,
+                       miniter:int=50, maxiter:int=100, 
+                       p_start:float=1.0, p_stop:float=3.0, p_inc:float=0.2, p_step:int=5, 
+                       q:float=0.5, vfrac:float=0.6, dtol:float=0.1, r_max:float=None, 
+                       penalty:float=None, nostop:bool=True, 
+                       neighbours:Iterable=None, guess:Iterable=None, i_start:int=0, 
+                       **kwargs) -> OptRes:
+    """
+    Performs topology optimization using an Optimality Criteria Method to
+    maximize the stiffness of a structure, given a design space and a certain 
+    amount of material to distribute.
+    
+    .. math::
+        :nowrap:
+        
+        \\begin{equation}
+            \\begin{array}{rrclcl}
+            \\displaystyle \\min_{\\boldsymbol{\\rho}} & \\mathbf{u(\\boldsymbol{\\rho})}^T \\mathbf{f} \\\\
+            \\textrm{s. t.} \\\\
+            & \\mathbf{K}(\\boldsymbol{\\rho}) \\mathbf{u(\\boldsymbol{\\rho})} & = & \\mathbf{f} \\\\
+            & V(\\boldsymbol{\\rho}) - \\eta V_0 & \\leq & 0 & & \\\\
+            & \\rho_i \\in \\{0, 1\\} & & & & \\forall i \\in N
+            \\end{array}
+        \\end{equation}
+    
+    Parameters
+    ----------
+    structure : Structure
+        An instance of sigmaepsilon.solid.fem.Structure.
+        
+    miniter : int, Optional
+        The minimum number of iterations to perform. Default is 50.
+        
+    maxiter : int, Optional
+        The maximum number of iterations to perform. Default is 100.
+    
+    p_start : float, Optional
+        Initial value of the penalty on intermediate densities. Default is 1.
+        
+    p_stop : float, Optional
+        Final value of the penalty on intermediate densities. Default is 3.
+        
+    p_inc : float, Optional
+        Increment of the penalty on intermediate densities. Default is 0.2
+        
+    p_step : int, Optional
+        The number of interations it takes to increment the penalty on intermediate
+        density values. Default is 5.
+        
+    q : float, Optional
+        Smoothing factor. Defaul is 0.5.
+        
+    vfrac : float, Optional
+        The fraction of available volume and the volume of the virgin structure.
+        Default is 0.6.
+        
+    dtol : float, Optional
+        This controls the maximum change in the value of a design variable. 
+        Default is 0.1.
+        
+    r_max : float, Optional
+        Radius for filtering. Default is None.
+        
+    neighbours : float, Optional
+        The neighbours of the cells for filtering. Default is None.
+    
+    guess : numpy.ndarray, Optional
+        A guess on the solution. This parameter can be used to contiue
+        a workflow. Default is None.
+        
+    i_start : int, Optional
+        Starting index for iterations. This parameter can be used to contiue
+        a workflow. Default is 0.
+        
+    summary : bool, Optional
+        If True, a short summary about execution time and the number of iterations
+        is available after execution as `structure.summary['topopt']`. Default is False.
+        
+    nostop : bool, Optional
+        If True, iterations neglect all stopping criteria, those govern by mniniter and maxiter included.
+        Default is False.
+    
+    Yields
+    ------
+    OptRes
+        The results of the actual iteration.
+        
+    Notes
+    -----
+    - The function returns a generator expression.
+    - This function can be used for both size and topology optimization,
+      depending on the inputs.
+    
+    """
+    do_filter = r_max is not None
+
+    # if i_start==0:
+    if structure.Solver is None:
+        structure.preprocess()
+    femsolver = structure.Solver.core
+    assert femsolver.regular
+    gnum = femsolver.gnum
+    K_bulk_0 = np.copy(femsolver.K)
+    vols = structure.volumes()
+    centers = structure.centers()
+
+    # initial solution to set up parameters
+    dens = np.zeros_like(vols)
+    dens_tmp = np.zeros_like(dens)
+    dens_tmp_ = np.zeros_like(dens)
+    dCdx = np.zeros_like(dens)
+    comps = np.zeros_like(dens)
+
+    def get_dof_solution():
+        U = femsolver.u
+        dU = len(U.shape)
+        if dU == 2:
+            # multiple load cases
+            return U[:,  0]
+        return U
+
+    def compliance(update_stiffness=False):
+        """
+        Init == True means that we are in the initialization phase.
+        """
+        if update_stiffness:
+            femsolver.update_stiffness(weighted_stiffness(K_bulk_0, dens))
+        femsolver.proc()
+        U = get_dof_solution()
+        comps[:] = compliances_bulk(K_bulk_0, U, gnum)
+        np.clip(comps, 1e-7, None, out=comps)
+        return np.sum(comps)
+
+    # ------------------ INITIAL SOLUTION ---------------
+    comp = compliance()
+    vol = np.sum(vols)
+    vol_start = vol
+    vol_min = vfrac * vol_start
+
+    # initialite filter
+    if do_filter:
+        if neighbours is None:
+            neighbours = cells_around(centers, r_max, frmt='dict')
+        if isinstance(neighbours, csr):
+            factors = get_filter_factors_csr(centers, neighbours, r_max)
+            fltr = sensitivity_filter_csr
+        else:
+            factors = get_filter_factors(centers, neighbours, r_max)
+            fltr = sensitivity_filter
+
+    # initialize penalty parameters
+    if penalty is not None:
+        p_start = penalty
+        p_stop = penalty + 1
+        p_step = maxiter + 1
+
+    # ------------- INITIAL FEASIBLE SOLUTION ------------
+    if guess is None:
+        dens[:] = vfrac
+    else:
+        dens = deepcopy(guess)
+    vol = np.sum(dens * vols)
+    comp = compliance(update_stiffness=True)
+    cIter = i_start
+    p = p_start
+    yield OptRes(dens, comp, vol, p, cIter)
+
+    # ------------------- ITERATION -------------------
+    dt = 0
+    terminate = False
+    while not terminate:
+        if (p < p_stop) and (np.mod(cIter, p_step) == 0):
+            p += p_inc
+        
+        # estimate lagrangian
+        lagr = p * comp / vol
+
+        # set up boundaries of change
+        _dens = dens * (1 - dtol)
+        np.clip(_dens, 1e-5, 1.0, out=_dens)
+        dens_ = dens * (1 + dtol)
+        np.clip(dens_, 1e-5, 1.0, out=dens_)
+
+        # sensitivity [*(-1)]
+        dCdx[:] = p * comps * dens ** (p-1)
+
+        # sensitivity filter
+        if do_filter:
+            dCdx[:] = fltr(dCdx, dens, neighbours, factors)
+
+        # calculate new densities and lagrangian
+        dens_tmp_[:] = dens * (dCdx / vols) ** q
+        dens_tmp[:] = dens_tmp_
+        _lagr = 0
+        lagr_ = 2 * lagr
+        _maxtries = 200
+        _ntries = 0
+        while (lagr_ - _lagr) > 1e-3:
+            if _ntries == _maxtries:
+                raise RuntimeError("Couldn't find multiplier :(.")
+            _lagr_ = (_lagr + lagr_) / 2
+            dens_tmp[:] = dens_tmp_ / (_lagr_ ** q)
+            np.clip(dens_tmp, _dens, dens_, out=dens_tmp)
+            vol_tmp = np.sum(dens_tmp * vols)
+            if vol_tmp < vol_min:
+                lagr_ = _lagr_
+            else:
+                _lagr = _lagr_
+            _ntries += 1
+        lagr = lagr_
+        dens[:] = dens_tmp
+
+        # resolve equilibrium equations and calculate compliance
+        comp = compliance(update_stiffness=True)
+        dt += femsolver._summary['proc', 'time']
+        vol = np.sum(dens * vols)
+        cIter += 1
+        res = OptRes(dens, comp, vol, p, cIter)
+        yield res
+
+        if nostop:
+            terminate = False
+        else:
+            if cIter < miniter:
+                terminate = False
+            elif cIter >= maxiter:
+                terminate = True
+            else:
+                terminate = (p >= p_stop)
+        
+    femsolver.K[:, :, :] = K_bulk_0
+    return OptRes(dens, comp, vol, p, cIter)
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/cells/bernoulli.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/utils/bernoulli.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,274 +1,282 @@
-import numpy as np
-from numpy import ndarray
-from numba import njit, prange
-
-__all__ = []
-
-__cache__ = True
-__NDOFN__ = 6
-
-
-@njit(nogil=True, parallel=True, cache=__cache__)
-def global_shape_function_derivatives_Bernoulli_bulk(dshp: ndarray, jac: ndarray):
-    """
-    Calculates derivatives of shape functions w.r.t. the global axes
-    using derivatives along local axes evaulated at some points in
-    the interval [-1, 1], and jacobians of local-to-global mappings.
-
-    Parameters
-    ----------
-    dshp: numpy.ndarray
-        A float array of shape (nE, nP, nNE, nDOF=6, 3)
-        Derivatives of shape functions evaluated at an 'nP' number of
-        points of an 'nE' number of elements.
-    jac: numpy.ndarray
-        A float array of shape (nE, nP, 1, 1)
-        Jacobi determinants, evaluated for each point in each cell.
-
-    Returns
-    -------
-    numpy.ndarray
-        5d float array of shape (nE, nP, nNE, nDOF=6, 3).
-    """
-    nE, nP, nNE = dshp.shape[:3]
-    res = np.zeros((nE, nP, nNE, __NDOFN__, 3), dtype=dshp.dtype)
-    for iE in prange(nE):
-        for jP in prange(nP):
-            J = jac[iE, jP, 0, 0]
-            res[iE, jP, :, :, 0] = dshp[iE, jP, :, :, 0] / J
-            res[iE, jP, :, :, 1] = dshp[iE, jP, :, :, 1] / J**2
-            res[iE, jP, :, :, 2] = dshp[iE, jP, :, :, 2] / J**3
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache__)
-def shape_function_matrix_Bernoulli(shp: ndarray, gdshp: ndarray):
-    """
-    Returns the shape function matrix of a single Bernoulli beam.
-
-    The input contains evaluations of the shape functions and at least
-    the first global derivatives of the shape functions.
-
-    Parameters
-    ----------
-    shp: numpy.ndarray
-        A float array of shape (nNE, nDOF=6), being the shape
-        functions evaluated at a single point of a single cell.
-    gdshp: numpy.ndarray
-        A float array of shape (nNE, nDOF=6, 3), being derivatives of shape
-        functions evaluated at a single point of a single cell.
-
-    Returns
-    -------
-    numpy.ndarray
-        2d float array of shape (nDOF, nDOF * nNODE).
-
-    Notes
-    -----
-    The approximation applies a mixture of Lagrange(L) and Hermite(H)
-    polynomials, in the order [L, H, H, L, H, H].
-
-    See Also
-    --------
-    :func:`shape_function_matrix_bulk`
-    """
-    nNE = shp.shape[0]
-    res = np.zeros((__NDOFN__, nNE * __NDOFN__), dtype=gdshp.dtype)
-    for iN in prange(nNE):
-        di = iN * __NDOFN__
-        # u_s
-        res[0, 0 + di] = shp[iN, 0]
-        # v_s
-        res[1, 1 + di] = shp[iN, 1]
-        res[1, 5 + di] = shp[iN, 5]
-        # w_s
-        res[2, 2 + di] = shp[iN, 2]
-        res[2, 4 + di] = shp[iN, 4]
-        # \heta_x
-        res[3, 3 + di] = shp[iN, 3]
-        # \theta_y
-        res[4, 2 + di] = -gdshp[iN, 2, 0]
-        res[4, 4 + di] = -gdshp[iN, 4, 0]
-        # \theta_z
-        res[5, 1 + di] = gdshp[iN, 1, 0]
-        res[5, 5 + di] = gdshp[iN, 5, 0]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache__)
-def shape_function_matrix_Bernoulli_bulk(shp: ndarray, gdshp: ndarray):
-    """
-    Returns the shape function matrix for several Bernoulli beams.
-
-    The input contains evaluations of the shape functions and at least
-    the first global derivatives of the shape functions.
-
-    Parameters
-    ----------
-    shp: numpy.ndarray
-        A float array of shape (nE, nP, nNE, nDOF=6), being the shape
-        functions evaluated at a nP number of points of several cells.
-    dshp: numpy.ndarray
-        A float array of shape (nE, nP, nNE, nDOF=6, 3), being derivatives
-        of shape functions evaluated at a nP number of points of several cells.
-
-    Returns
-    -------
-    numpy.ndarray
-        2d float array of shape (nE, nP, nDOF, nDOF * nNODE).
-
-    See Also
-    --------
-    :func:`shape_function_matrix`
-    """
-    nE, nP, nNE = gdshp.shape[:3]
-    res = np.zeros((nE, nP, __NDOFN__, nNE * __NDOFN__), dtype=gdshp.dtype)
-    for iE in prange(nE):
-        for iP in prange(nP):
-            res[iE, iP] = shape_function_matrix_Bernoulli(shp[iE, iP], gdshp[iE, iP])
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache__)
-def _shape_function_matrix_Bernoulli_L(shp: ndarray):
-    """
-    Returns the shape function matrix for a line.
-    The input contains evaluations of the shape functions.
-
-    shp (nNE, nDOF=6)
-    ---
-    (nDOF, nDOF * nNODE)
-    """
-    nNE = shp.shape[0]
-    res = np.zeros((__NDOFN__, nNE * __NDOFN__), dtype=shp.dtype)
-    for iN in prange(nNE):
-        di = iN * __NDOFN__
-        res[0, 0 + di] = shp[iN, 0]
-        res[1, 1 + di] = shp[iN, 1]
-        res[2, 2 + di] = shp[iN, 2]
-        res[3, 3 + di] = shp[iN, 3]
-        res[4, 2 + di] = shp[iN, 4]
-        res[5, 1 + di] = shp[iN, 5]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache__)
-def _shape_function_matrix_L_multi(shp: ndarray):
-    """
-    Returns the shape function matrix for a line.
-    The input contains evaluations of the shape functions.
-
-    shp (nP, nNE, nDOF=6)
-    ---
-    (nP, nDOF, nDOF * nNODE)
-    """
-    nP, nNE = shp.shape[:2]
-    res = np.zeros((nP, __NDOFN__, nNE * __NDOFN__), dtype=shp.dtype)
-    for iP in prange(nP):
-        res[iP] = _shape_function_matrix_Bernoulli_L(shp[iP])
-    return res
-
-
-@njit(nogil=True, parallel=True, fastmath=True, cache=__cache__)
-def body_load_vector_Bernoulli(
-    values: ndarray, shp: ndarray, gdshp: ndarray, djac: ndarray, w: ndarray
-):
-    """
-    Input values are assumed to be evaluated at multiple (nG) Gauss points of
-    multiple (nE) cells.
-
-    Parameters
-    ----------
-    values: numpy.ndarray
-        A 3d float array of body loads of shape (nE, nRHS, nNE * 6)
-        for several elements and load cases.
-    shp: numpy.ndarray
-        A float array of shape (nE, nG, nNE, nDOF=6), being the shape
-        functions evaluated at a nG number of Gauss points of several cells.
-    djac: numpy.ndarray
-        A float array of shape (nE, nG), being jacobian determinants
-        evaluated at the Gauss points of several cells.
-    w: numpy.ndarray
-        1d float array of weights for an nG number of Gauss points,
-        with a shape of (nG,).
-
-    Returns
-    -------
-    numpy.ndarray
-        3d float array of shape (nE, nNE * 6, nRHS).
-    """
-    nRHS = values.shape[1]
-    nE, nG, nNE = shp.shape[:3]
-    NH = shape_function_matrix_Bernoulli_bulk(
-        shp, gdshp
-    )  # (nE, nG, nDOF, nDOF * nNODE)
-    NL = _shape_function_matrix_L_multi(shp[0])  # (nG, nDOF, nDOF * nNODE)
-    res = np.zeros((nE, nNE * __NDOFN__, nRHS), dtype=values.dtype)
-    for iG in range(nG):
-        for iRHS in prange(nRHS):
-            for iE in prange(nE):
-                res[iE, :, iRHS] += (
-                    NH[iE, iG].T @ NL[iG] @ values[iE, iRHS, :] * djac[iE, iG] * w[iG]
-                )
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache__)
-def lumped_mass_matrices_direct_Bernoulli(
-    dens: ndarray,
-    lengths: ndarray,
-    areas: ndarray,
-    topo: ndarray,
-    alpha: float = 1 / 20,
-) -> ndarray:
-    """
-    Returns the diagonal values of the directly lumped mass matrix for several
-    Bernoulli beam elements, sharing the total masses equivalently among nodes.
-
-    Implementation is based on the lecture notes of Carlos A. Felippa [1].
-
-    Parameters
-    ----------
-    dens : numpy.ndarray
-        1d numpy float array of material densities.
-    lengths : numpy.ndarray
-        1d numpy float array of element lengths.
-    areas : numpy.ndarray
-        1d numpy float array of element areas.
-    topo : numpy.ndarray
-        2d numpy integer array of node indices referencing the global pointcloud.
-    alpha : float, Optional
-        A nonnegative parameter, typically between 0 and 1/50 (see notes).
-        Default is 1/20.
-
-    Returns
-    -------
-    numpy.ndarray
-        A 2d float array of shape (nE, 6 * nNE), where nE and nNE are the number of
-        elements and nodes per element.
-
-    Notes
-    -----
-    [1] : "The choice of α has been argued in the FEM literature over several decades,
-    but the whole discussion is largely futile. Matching the angular momentum of
-    the beam element gyrating about its midpoint gives α = −1/24. This violates the
-    positivity condition stated in [1, 32.2.4]. It follows that the best possible
-    α — as opposed to possible best — is zero. This choice gives, however, a singular
-    mass matrix, which is undesirable in scenarios where a mass-inverse appears."
-
-    References
-    ----------
-    .. [1] Introduction to Finite Element Methods, Carlos A. Felippa.
-           Department of Aerospace Engineering Sciences and Center for
-           Aerospace Structures, University of Colorado. 2004.
-    """
-    nE, nNE = topo.shape
-    diags = np.zeros((nE, 6 * nNE), dtype=dens.dtype)
-    for iE in prange(nE):
-        li = lengths[iE]
-        vi = li * areas[iE]
-        di = dens[iE]
-        for jNE in prange(nNE):
-            diags[iE, jNE * 6 : jNE * 6 + 3] = di * vi / nNE
-            diags[iE, jNE * 6 + 3 : jNE * 6 + 6] = di * vi * alpha * li**2
-    return diags
+# -*- coding: utf-8 -*-
+import numpy as np
+from numpy import ndarray
+from numba import njit, prange
+
+__all__ = []
+
+__cache__ = True
+__NDOFN__ = 6
+
+
+@njit(nogil=True, parallel=True, cache=__cache__)
+def global_shape_function_derivatives_bulk(dshp: ndarray, jac: ndarray):
+    """
+    Calculates derivatives of shape functions w.r.t. the global axes
+    using derivatives along local axes evaulated at some points in
+    the interval [-1, 1], and jacobians of local-to-global mappings.
+
+    Parameters
+    ----------
+    dshp: a NumPy float array of shape (nE, nP, nNE, nDOF=6, 3)
+        Derivatives of shape functions evaluated at an 'nP' number of 
+        points of an 'nE' number of elements.
+
+    jac: a NumPy float array of shape (nE, nP, 1, 1)
+        Jacobi determinants, evaluated for each point in each cell.
+
+    Returns
+    -------
+    NumPy array of shape (nE, nP, nNE, nDOF=6, 3)
+
+    """
+    nE, nP, nNE = dshp.shape[:3]
+    res = np.zeros((nE, nP, nNE, __NDOFN__, 3), dtype=dshp.dtype)
+    for iE in prange(nE):
+        for jP in prange(nP):
+            J = jac[iE, jP, 0, 0]
+            res[iE, jP, :, :, 0] = dshp[iE, jP, :, :, 0] / J
+            res[iE, jP, :, :, 1] = dshp[iE, jP, :, :, 1] / J**2
+            res[iE, jP, :, :, 2] = dshp[iE, jP, :, :, 2] / J**3
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache__)
+def shape_function_matrix(shp: ndarray, gdshp: ndarray):
+    """
+    Returns the shape function matrix for a Bernoulli beam.
+
+    The input contains evaluations of the shape functions and at lest 
+    the first global derivatives of the shape functions. 
+
+    shp (nNE, nDOF=6)
+    gdshp (nNE, nDOF=6, 3)
+    ---
+    (nDOF, nDOF * nNODE)
+
+    Notes
+    -----
+    The approximation applies a mixture of Lagrange(L) and Hermite(H) 
+    polynomials, in the order [L, H, H, L, H, H].
+    """
+    nNE = shp.shape[0]
+    res = np.zeros((__NDOFN__, nNE * __NDOFN__), dtype=gdshp.dtype)
+    for iN in prange(nNE):
+        di = iN * __NDOFN__
+        # u_s
+        res[0, 0 + di] = shp[iN, 0]
+        # v_s
+        res[1, 1 + di] = shp[iN, 1]
+        res[1, 5 + di] = shp[iN, 5]
+        # w_s
+        res[2, 2 + di] = shp[iN, 2]
+        res[2, 4 + di] = shp[iN, 4]
+        # \heta_x
+        res[3, 3 + di] = shp[iN, 3]
+        # \theta_y
+        res[4, 2 + di] = - gdshp[iN, 2, 0]
+        res[4, 4 + di] = - gdshp[iN, 4, 0]
+        # \theta_z
+        res[5, 1 + di] = gdshp[iN, 1, 0]
+        res[5, 5 + di] = gdshp[iN, 5, 0]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache__)
+def shape_function_matrix_bulk(shp: ndarray, gdshp: ndarray):
+    """
+    In
+    --
+    shp (nE, nP, nNE, nDOF=6)
+    gdshp (nE, nP, nNE, nDOF=6, 3)
+
+    Out
+    ---
+    (nE, nP, nDOF, nDOF * nNODE)
+    """
+    nE, nP, nNE = gdshp.shape[:3]
+    res = np.zeros((nE, nP, __NDOFN__, nNE * __NDOFN__), dtype=gdshp.dtype)
+    for iE in prange(nE):
+        for iP in prange(nP):
+            res[iE, iP] = shape_function_matrix(shp[iE, iP], gdshp[iE, iP])
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache__)
+def shape_function_matrix_L(shp: ndarray):
+    """
+    Returns the shape function matrix for a line.
+
+    The input contains evaluations of the shape functions. 
+
+    In
+    --
+    shp (nNE, nDOF=6)
+
+    Out
+    ---
+    (nDOF, nDOF * nNODE)
+    """
+    nNE = shp.shape[0]
+    res = np.zeros((__NDOFN__, nNE * __NDOFN__), dtype=shp.dtype)
+    for iN in prange(nNE):
+        di = iN * __NDOFN__
+        res[0, 0 + di] = shp[iN, 0]
+        res[1, 1 + di] = shp[iN, 1]
+        res[2, 2 + di] = shp[iN, 2]
+        res[3, 3 + di] = shp[iN, 3]
+        res[4, 2 + di] = shp[iN, 4]
+        res[5, 1 + di] = shp[iN, 5]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache__)
+def shape_function_matrix_L_multi(shp: ndarray):
+    """
+    Returns the shape function matrix for a line.
+
+    The input contains evaluations of the shape functions. 
+
+    In
+    --
+    shp (nP, nNE, nDOF=6)
+
+    Out
+    ---
+    (nP, nDOF, nDOF * nNODE)
+    """
+    nP, nNE = shp.shape[:2]
+    res = np.zeros((nP, __NDOFN__, nNE * __NDOFN__), dtype=shp.dtype)
+    for iP in prange(nP):
+        res[iP] = shape_function_matrix_L(shp[iP])
+    return res
+
+
+@njit(nogil=True, parallel=True, fastmath=True, cache=__cache__)
+def body_load_vector_bulk(values: ndarray, shp: ndarray, gdshp: ndarray,
+                          djac: ndarray, w: ndarray):
+    """
+    Input values are assumed to be evaluated at multiple (nG) Gauss points of
+    multiple (nE) cells.
+
+    values (nE, nRHS, nNE * 6)
+    djac (nE, nG)
+    shp (nE, nG, nNE=2, nDOF=6)
+    w (nG)
+    ---
+    (nE, nNE * 6, nRHS)
+    """
+    nRHS = values.shape[1]
+    nE, nG, nNE = shp.shape[:3]
+    NH = shape_function_matrix_bulk(shp, gdshp)  # (nE, nG, nDOF, nDOF * nNODE)
+    NL = shape_function_matrix_L_multi(shp[0])  # (nG, nDOF, nDOF * nNODE)
+    res = np.zeros((nE, nNE * __NDOFN__, nRHS), dtype=values.dtype)
+    for iG in range(nG):
+        for iRHS in prange(nRHS):
+            for iE in prange(nE):
+                res[iE, :, iRHS] += NH[iE, iG].T @ NL[iG] @ values[iE,
+                                                                   iRHS, :] * djac[iE, iG] * w[iG]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache__)
+def calculate_element_forces_bulk(dofsol: ndarray, B: ndarray,
+                                  D: ndarray, shp: ndarray,
+                                  gdshp: ndarray, body_forces: ndarray):
+    """
+    Calculates internal forces from dof solution.
+    """
+    nE = dofsol.shape[0]
+    nP = B.shape[1]
+    res = np.zeros((__NDOFN__, nE, nP), dtype=dofsol.dtype)
+    for i in prange(nE):
+        for j in prange(nP):
+            pyy, pzz = body_forces[i, 0, 4:] * shp[j, 0] + \
+                body_forces[i, 1, 4:] * shp[j, 1]
+            N, T, My, Mz = D[i] @ B[i, j] @ dofsol[i]
+            res[0, i, j] = N
+            # Vy
+            res[1, i, j] = -D[i, 3, 3] * (
+                gdshp[i, j, 2, 2] * dofsol[i, 1] +
+                gdshp[i, j, 3, 2] * dofsol[i, 5] +
+                gdshp[i, j, 4, 2] * dofsol[i, 7] +
+                gdshp[i, j, 5, 2] * dofsol[i, 11]) - pzz
+            # Vz
+            res[2, i, j] = -D[i, 2, 2] * (
+                gdshp[i, j, 6, 2] * dofsol[i, 2] +
+                gdshp[i, j, 7, 2] * dofsol[i, 4] +
+                gdshp[i, j, 8, 2] * dofsol[i, 8] +
+                gdshp[i, j, 9, 2] * dofsol[i, 10]) + pyy
+            res[3, i, j] = T
+            res[4, i, j] = My
+            res[5, i, j] = Mz
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache__)
+def interpolate_element_data_bulk(edata: ndarray, N: ndarray):
+    """
+    N (nE, nP, nDOF, nDOF * nNODE)  shape function matrix
+    edata (nE, nDOF * nNODE)  element data
+    """
+    nE, nP = N.shape[:2]
+    res = np.zeros(N.shape[:3], dtype=N.dtype)
+    for iE in prange(nE):
+        for iP in prange(nP):
+            res[iE, iP, :] = N[iE, iP] @ edata[iE]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache__)
+def lumped_mass_matrices_direct(dens: ndarray, lengths: ndarray, areas: ndarray,
+                                topo: ndarray, alpha: float = 1/20) -> ndarray:
+    """
+    Returns the diagonal values of the directly lumped mass matrix for several 
+    Bernoulli beam elements, sharing the total masses equivalently among nodes.
+
+    Implementation is based on the lecture notes of Carlos A. Felippa [1].
+
+    Parameters
+    ----------
+    dens : ndarray
+        1d numpy float array of material densities.
+
+    lengths : ndarray
+        1d numpy float array of element lengths.
+
+    areas : ndarray
+        1d numpy float array of element areas.
+
+    topo : ndarray
+        2d numpy integer array of node indices referencing the global pointcloud.
+
+    alpha : float
+        A nonnegative parameter, typically between 0 and 1/50 (see notes).
+        Default is 1/20.
+
+    Notes
+    -----
+    [1] : "The choice of α has been argued in the FEM literature over several decades, 
+    but the whole discussion is largely futile. Matching the angular momentum of 
+    the beam element gyrating about its midpoint gives α = −1/24. This violates the 
+    positivity condition stated in [1, 32.2.4]. It follows that the best possible 
+    α — as opposed to possible best — is zero. This choice gives, however, a singular 
+    mass matrix, which is undesirable in scenarios where a mass-inverse appears."
+
+    References
+    ----------
+    .. [1] Introduction to Finite Element Methods, Carlos A. Felippa.
+           Department of Aerospace Engineering Sciences and Center for 
+           Aerospace Structures, University of Colorado. 2004.
+
+    """
+    nE, nNE = topo.shape
+    diags = np.zeros((nE, 6 * nNE), dtype=dens.dtype)
+    for iE in prange(nE):
+        li = lengths[iE]
+        vi = li * areas[iE]
+        di = dens[iE]
+        for jNE in prange(nNE):
+            diags[iE, jNE*6: jNE*6 + 3] = di * vi / nNE
+            diags[iE, jNE*6 + 3: jNE*6 + 6] = di * vi * alpha * li**2
+    return diags
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/dyn.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/dyn.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,266 +1,259 @@
-from typing import Union, Tuple
-from numpy import ndarray
-from scipy.sparse import spmatrix
-import numpy as np
-
-from neumann import atleast2d
-
-from .linsolve import solve_standard_form
-from .eigsolve import eig_sparse, eig_dense
-
-
-ArrayLike = Union[ndarray, spmatrix]
-
-
-def effective_modal_mass(M: ArrayLike, action: ndarray, mode: ndarray) -> float:
-    """
-    Returns the effective modal mass for a specific mode.
-
-    Assumes that the modal shapes are normalized to the mass matrix.
-
-    Parameters
-    ----------
-    M : numpy.ndarray
-        2d mass matrix as a NumPy or SciPy 2d float array.
-    action : Iterable
-        1d iterable, with a length matching the dof layout of the structure.
-    mode : numpy.ndarray
-        1d array representing a modal shape.
-
-    Returns
-    -------
-    float
-        The effective modal mass.
-
-    """
-    return (mode.T @ M @ action) ** 2
-
-
-def effective_modal_masses(M: ArrayLike, action: ndarray, modes: ndarray) -> ndarray:
-    """
-    Returns the effective modal mass for several modes.
-
-    Assumes that the modal shapes are normalized to the mass matrix.
-
-    Parameters
-    ----------
-    M : numpy.ndarray
-        Mass matrix as a NumPy or SciPy 2d float array.
-    action : numpy.ndarray
-        1d iterable, with a length matching the dof layout of the structure.
-    modes : numpy.ndarray
-        A matrix, whose columns are eigenmodes of interest.
-
-    Notes
-    -----
-    The sum of all effective masses equals the total mass of the structure.
-
-    Returns
-    -------
-    numpy.ndarray
-        1d float array of effective modal masses
-
-    """
-    res = []
-    for i in range(modes.shape[-1]):
-        m_eff = effective_modal_mass(M, action, modes[:, i])
-        res.append(m_eff)
-    return np.array(res)
-
-
-def Rayleigh_quotient(
-    M: spmatrix, *, K: spmatrix = None, u: ndarray = None, f: ndarray = None, **kw
-) -> ndarray:
-    """
-    Returns Rayleigh's quotient
-
-    .. math::
-        :nowrap:
-
-        \\begin{equation}
-            \\frac{\\mathbf{v}^T \\mathbf{K} \\mathbf{v}}{\\mathbf{v}^T
-            \\mathbf{M} \\mathbf{v}},
-        \\end{equation}
-
-    for a prescribed action :math:`\\mathbf{v}`.
-
-    Parameters
-    ----------
-    M : scipy.linalg.sparse.spmatrix
-        The mass matrix.
-    u : numpy.ndarray, Optional
-        The vector of nodal displacements (1d or 2d).
-    K : scipy.linalg.sparse.spmatrix, Optional
-        The stiffness matrix. It can be omitted, if 'f' is provided.
-    f : numpy.ndarray, Optional
-        The vector of nodal forces (1d or 2d). It can be omitted,
-        if 'K' is provided.
-
-    Notes
-    -----
-    The Rayleigh quotient is
-
-    - higher than, or equal to the square of the smallest natural
-      circular frequency,
-
-    - smaller than, or equal to the square of the highest natural
-      circular frequency.
-
-    Returns
-    -------
-    numpy.ndarray
-        An 1d array of floats.
-
-    """
-    if isinstance(f, ndarray) and u is None:
-        u = atleast2d(solve_standard_form(K, f), back=True)
-    elif isinstance(u, ndarray) and f is None:
-        f = K @ u
-    res = []
-    for i in range(u.shape[-1]):
-        nom = u[:, i].T @ f[:, i]
-        denom = u[:, i].T @ M @ u[:, i]
-        res.append(nom / denom)
-    return np.array(res)
-
-
-def natural_circular_frequencies(
-    K: spmatrix,
-    M: spmatrix,
-    *,
-    k: int = 10,
-    return_vectors: bool = False,
-    maxiter: int = 5000,
-    normalize: bool = True,
-    as_dense: bool = False,
-    around: float = None,
-    nmode: str = "M",
-    which: str = "SM",
-    **kwargs
-) -> Tuple[ndarray]:
-    """
-    Returns the natural circular frequencies :math:`\omega_{0i}` and optionally the
-    corresponding eigenvectors as (not trivial) solutions to the eigenproblem
-
-    .. math::
-        :nowrap:
-
-        \\begin{equation}
-            \\left( \\mathbf{K} - \\omega^2 \\mathbf{M} \\right)
-            \\mathbf{v} = \\mathbf{0}.
-        \\end{equation}
-
-    Parameters
-    ----------
-    K : scipy.linalg.sparse.spmatrix
-        The stiffness matrix in sparse format.
-    M : scipy.linalg.sparse.spmatrix
-        The mass matrix in sparse format.
-    k : int, Optional
-        The number of solutions to return. Only if 'as_dense' is False.
-        Default is 10.
-    return_vectors : bool, Optional
-        To return eigenvectors or not. Default is False.
-    maxiter : int, Optional
-        Maximum number of iterations, if solved using sparse matrices.
-        Only if 'as_dense' is False. Default is 5000.
-    normalize : bool, Optional
-        If True, the returned eigenvectors are normalized to the mass matrix.
-        Only if 'return_vectors' is True. Default is True.
-    as_dense : bool, Optional
-        If True, the stiffness and mass matrices are handled as dense arrays.
-        In this case, if 'return_vectors' is True, all eigenvalues and vectors
-        are returned, regardless of other parameters.
-    around : float, Optional
-        A target (possibly an approximation) value around which eigenvalues
-        are searched. Default is None.
-    which : str, ['LM' | 'SM' | 'LA' | 'SA' | 'BE' | 'LR' | 'SR'
-                 | 'LI' | 'SI'], Optional
-        Which `k` eigenvectors and eigenvalues to find:
-
-            'LM' : largest magnitude
-
-            'SM' : smallest magnitude
-
-            'LA' : Largest (algebraic) eigenvalues.
-
-            'SA' : Smallest (algebraic) eigenvalues.
-
-            'BE' : Half (k/2) from each end of the spectrum.
-
-            'LR' : largest real part
-
-            'SR' : smallest real part
-
-            'LI' : largest imaginary part
-
-            'SI' : smallest imaginary part
-
-        Only if 'as_dense' is False. Default is 'LM'.
-    **kwargs : dict, Optional
-        Keyword arguments are forwarded to the appropriate routine of SciPy.
-
-    Note
-    ----
-    Calculation is done using the relavant routines of Scipy,
-    see its documentation for more control over the parameters.
-
-    See also
-    --------
-    :func:`scipy.linalg.eigs`
-    :func:`scipy.sparse.linalg.eigsh`
-
-    Returns
-    -------
-    numpy.ndarray
-        The natural circular frequencies.
-    numpy.ndarray
-        The eigenvectors, only if 'return_vectors' is True.
-
-    """
-    if around is not None:
-        kwargs["sigma"] = around**2
-
-    if as_dense:
-        vals, vecs = eig_dense(
-            K, M=M, nmode=nmode, normalize=normalize, return_residuals=False, **kwargs
-        )
-    else:
-        vals, vecs = eig_sparse(
-            K,
-            k=k,
-            M=M,
-            which=which,
-            normalize=normalize,
-            maxiter=maxiter,
-            return_residuals=False,
-            nmode=nmode,
-            **kwargs
-        )
-    cfreqs = np.sqrt(vals)
-    if return_vectors:
-        return cfreqs, vecs
-    return cfreqs
-
-
-def estimate_smallest_natural_circular_frequency(*args, **kwargs) -> ndarray:
-    """
-    Returns a lower bound estimation of the smallest natural frequency using
-    Rayleigh's quotient. See :func:`Rayleigh_quotient` for the input.
-
-    Notes
-    -----
-    This relies on the equivalence of elastic internal energy and kinetic
-    energy of undamped conservative systems.
-
-    Returns
-    -------
-    numpy.ndarray
-        An 1d array of floats.
-
-    See also
-    --------
-    :func:`Rayleigh_quotient`
-
-    """
-    return np.sqrt(Rayleigh_quotient(*args, **kwargs))
+# -*- coding: utf-8 -*-
+from typing import Union, Tuple
+from numpy import ndarray
+from scipy.sparse import spmatrix
+import numpy as np
+
+from neumann.array import atleast2d
+
+from .linsolve import solve_standard_form
+from .eigsolve import eig_sparse, eig_dense
+
+
+ArrayLike = Union[ndarray, spmatrix]
+
+
+def effective_modal_mass(M: ArrayLike, action: ndarray, mode: ndarray):
+    """
+    Returns the effective modal mass for a specific mode.
+
+    Assumes that the modal shapes are normalized to the mass matrix.
+
+    Parameters
+    ----------
+    M : numpy.ndarray
+        2d mass matrix as a NumPy or SciPy 2d float array.
+
+    action : Iterable
+        1d iterable, with a length matching the dof layout of the structure. 
+
+    mode : numpy.ndarray
+        1d array representing a modal shape.
+
+    Returns
+    -------
+    float  
+        The effective modal mass.
+
+    """
+    return (mode.T @ M @ action)**2
+
+
+def effective_modal_masses(M: ArrayLike, action: ndarray, modes: ndarray) -> ndarray:
+    """
+    Returns the effective modal mass for several modes.
+
+    Assumes that the modal shapes are normalized to the mass matrix.
+
+    Parameters
+    ----------
+    M : numpy.ndarray
+        Mass matrix as a NumPy or SciPy 2d float array.
+
+    action : numpy.ndarray
+        1d iterable, with a length matching the dof layout of the structure. 
+
+    modes : numpy.ndarray
+        A matrix, whose columns are eigenmodes of interest.
+
+    Notes
+    -----
+    The sum of all effective masses equals the total mass of the structure.
+
+    Returns
+    -------
+    numpy.ndarray  
+        1d float array of effective modal masses
+
+    """
+    res = []
+    for i in range(modes.shape[-1]):
+        m_eff = effective_modal_mass(M, action, modes[:, i])
+        res.append(m_eff)
+    return np.array(res)
+
+
+def Rayleigh_quotient(M: spmatrix, *args, K: spmatrix = None, u: ndarray = None,
+                      f: ndarray = None, **kwargs) -> ndarray:
+    """
+    Returns Rayleigh's quotient
+
+    .. math::
+        :nowrap:
+
+        \\begin{equation}
+            \\frac{\\mathbf{v}^T \\mathbf{K} \\mathbf{v}}{\\mathbf{v}^T \\mathbf{M} \\mathbf{v}},
+        \\end{equation}
+
+    for a prescribed action :math:`\\mathbf{v}`.
+
+    Parameters
+    ----------
+    M : scipy.linalg.sparse.spmatrix
+        The mass matrix.
+
+    u : numpy.ndarray, Optional
+        The vector of nodal displacements (1d or 2d).
+
+    K : scipy.linalg.sparse.spmatrix, Optional
+        The stiffness matrix. It can be omitted, if 'f' is provided.
+
+    f : numpy.ndarray, Optional
+        The vector of nodal forces (1d or 2d). It can be omitted, if 'K' is provided.
+
+    Notes
+    -----
+    The Rayleigh quotient is 
+
+    - higher than, or equal to the square of the smallest natural circular frequency,
+
+    - smaller than, or equal to the square of the highest natural circular frequency.
+
+    Returns
+    -------
+    numpy.ndarray
+        An 1d array of floats.
+
+    """
+    if isinstance(f, ndarray) and u is None:
+        u = atleast2d(solve_standard_form(K, f), back=True)
+    elif isinstance(u, ndarray) and f is None:
+        f = K @ u
+    res = []
+    for i in range(u.shape[-1]):
+        nom = u[:, i].T @ f[:, i]
+        denom = u[:, i].T @ M @ u[:, i]
+        res.append(nom / denom)
+    return np.array(res)
+
+
+def natural_circular_frequencies(K: spmatrix, M: spmatrix, *args, k: int = 10, return_vectors: bool = False,
+                                 maxiter: int = 5000, normalize: bool = True, as_dense: bool = False,
+                                 around: float = None, nmode: str = 'M', which: str = 'LM', **kwargs) -> Tuple[ndarray]:
+    """
+    Returns the natural circular frequencies :math:`\omega_{0i}` and optionally the 
+    corresponding eigenvectors as (not trivial) solutions to the eigenproblem
+
+    .. math::
+        :nowrap:
+
+        \\begin{equation}
+            \\left( \\mathbf{K} - \\omega^2 \\mathbf{M} \\right) \\mathbf{v} = \\mathbf{0}. 
+        \\end{equation}
+
+    Parameters
+    ----------
+    K : scipy.linalg.sparse.spmatrix
+        The stiffness matrix in sparse format. 
+
+    M : scipy.linalg.sparse.spmatrix
+        The mass matrix in sparse format.
+
+    k : int, Optional
+        The number of solutions to return. Only if 'as_dense' is False. 
+        Default is 10.
+
+    return_vectors : bool, Optional
+        To return eigenvectors or not. Default is False.
+
+    maxiter : int, Optional
+        Maximum number of iterations, if solved using sparse matrices.
+        Only if 'as_dense' is False. Default is 5000.
+
+    normalize : bool, Optional
+        If True, the returned eigenvectors are normalized to the mass matrix.
+        Only if 'return_vectors' is True. Default is True.
+
+    as_dense : bool, Optional
+        If True, the stiffness and mass matrices are handled as dense arrays.
+        In this case, if 'return_vectors' is True, all eigenvalues and vectors are
+        returned, regardless of other parameters.
+
+    around : float, Optional
+        A target (possibly an approximation) value around which eigenvalues
+        are searched. Default is None.
+
+    which : str, ['LM' | 'SM' | 'LA' | 'SA' | 'BE' | 'LR' | 'SR' | 'LI' | 'SI'], Optional
+        Which `k` eigenvectors and eigenvalues to find:
+
+            'LM' : largest magnitude
+
+            'SM' : smallest magnitude
+
+            'LA' : Largest (algebraic) eigenvalues.
+
+            'SA' : Smallest (algebraic) eigenvalues.
+
+            'BE' : Half (k/2) from each end of the spectrum.
+
+            'LR' : largest real part
+
+            'SR' : smallest real part
+
+            'LI' : largest imaginary part
+
+            'SI' : smallest imaginary part
+
+        Only if 'as_dense' is False. Default is 'LM'.
+
+    **kwargs : dict, Optional
+        Keyword arguments are forwarded to the appropriate routine of SciPy.
+
+    Note
+    ----
+    Calculation is done using the relavant routines of Scipy,
+    see its documentation for more control over the parameters.
+
+    See also
+    --------
+    :func:`scipy.linalg.eigs`
+    :func:`scipy.sparse.linalg.eigsh`
+
+    Returns
+    -------
+    numpy.ndarray
+        The natural circular frequencies.
+
+    numpy.ndarray
+        The eigenvectors, only if 'return_vectors' is True.
+    
+    """
+    if around is not None:
+        kwargs['sigma'] = around**2
+
+    if as_dense:
+        vals, vecs = eig_dense(K, *args, M=M, nmode=nmode,
+                               normalize=normalize,
+                               return_residuals=False, **kwargs)
+    else:
+        vals, vecs = eig_sparse(K, *args, k=k, M=M, which=which,
+                                normalize=normalize, maxiter=maxiter,
+                                return_residuals=False, nmode=nmode,
+                                **kwargs)
+    cfreqs = np.sqrt(vals)
+    if return_vectors:
+        return cfreqs, vecs
+    return cfreqs
+
+
+def estimate_smallest_natural_circular_frequency(*args, **kwargs) -> ndarray:
+    """
+    Returns a lower bound estimation of the smallest natural frequency using Rayleigh's quotient.
+    See :func:`Rayleigh_quotient` for the input.
+
+    Notes
+    -----
+    This relies on the equivalence of elastic internal energy and kinetic energy of 
+    undamped conservative systems.
+
+    Returns
+    -------
+    numpy.ndarray
+        An 1d array of floats.
+
+    See also
+    --------
+    :func:`Rayleigh_quotient`
+
+    """
+    return np.sqrt(Rayleigh_quotient(*args, **kwargs))
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/fem.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/cells/utils/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,536 +1,537 @@
-from typing import Union, Tuple
-
-from numba import njit, prange
-import numpy as np
-from numpy import ndarray
-from scipy.sparse import spmatrix
-import awkward as ak
-
-from neumann.linalg.sparse import csr_matrix as csr, JaggedArray
-from neumann import find1d, flatten2dC
-
-__cache = True
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def fixity2d_to_dofs1d(fixity2d: np.ndarray, inds: np.ndarray = None):
-    """
-    Returns the indices of the degrees of freedoms
-    being supressed.
-
-    Optionally, global indices of the rows in 'fixity2d'
-    array can be provided by the optional argument 'inds'.
-
-    Parameters
-    ----------
-    fixity2d : numpy.ndarray
-        2d numpy array of booleans. It has as many rows as nodes, and as
-        many columns as derees of freedom per node in the model. A True
-        value means that the corresponding dof is fully supressed.
-    inds : numpy.ndarray, Optional
-        1d numpy array of integers, default is None. If provided, it should
-        list the global indices of the nodes, for which the data is provided
-        by the array 'fixity2d'.
-
-    Returns
-    -------
-    dofinds : np.ndarray
-        1d numpy array of integers.
-    """
-    ndof = fixity2d.shape[1]
-    args = np.argwhere(fixity2d == True)
-    N = args.shape[0]
-    res = np.zeros(N, dtype=args.dtype)
-    for i in prange(N):
-        res[i] = args[i, 0] * ndof + args[i, 1]
-    if inds is None:
-        return res
-    else:
-        dofinds = np.zeros_like(res)
-        for i in prange(len(inds)):
-            for j in prange(ndof):
-                dofinds[i * ndof + j] = inds[i] * ndof + j
-        return dofinds[res]
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def nodes2d_to_dofs1d(inds: np.ndarray, values: np.ndarray):
-    """
-    Returns a tuple of degree of freedom indices and data,
-    based on a nodal definition.
-
-    Parameters
-    ----------
-    inds : numpy.ndarray
-        1d numpy array of integers, listing global node indices.
-    values : numpy.ndarray
-        3d numpy float array of shape (nN, nDOF, nX), listing values
-        for each node in 'inds'. nX is the number of datasets.
-
-    Returns
-    -------
-    dofinds : numpy.ndarray
-        1d numpy array of integers, denoting global dof indices.
-    dofvals : numpy.ndarray
-        2d numpy float array of shape (nN * nDOF, nX), denoting values
-        on dofs in 'dofinds'.
-    """
-    nN, dof_per_node, nRHS = values.shape
-    dofinds = np.zeros((nN * dof_per_node), dtype=inds.dtype)
-    dofvals = np.zeros((nN * dof_per_node, nRHS), dtype=values.dtype)
-    for node in prange(nN):
-        for dof in prange(dof_per_node):
-            i = node * dof_per_node + dof
-            dofinds[i] = inds[node] * dof_per_node + dof
-            for rhs in prange(nRHS):
-                dofvals[i, rhs] = values[node, dof, rhs]
-    return dofinds, dofvals
-
-
-@njit(nogil=True, cache=__cache, parallel=True)
-def weighted_stiffness_bulk(K: np.ndarray, weights: np.ndarray):
-    """
-    Returns a weighted stiffness matrix.
-
-    Parameters
-    ----------
-    K : numpy.ndarray
-        2d numpy array of floats, where the first axis of K runs
-        along the elements.
-    weights : numpy.ndarray
-        1d numpy array of floats.
-
-    Returns
-    -------
-    Kw : numpy.ndarray
-        2d numpy array of floats with the same shape as 'K'.
-    """
-    nE = len(weights)
-    res = np.zeros_like(K)
-    for i in prange(nE):
-        res[i, :] = weights[i] * K[i]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def irows_icols_bulk(edofs: np.ndarray) -> Tuple[ndarray]:
-    """
-    Returns row and column index data for several finite elements.
-
-    Parameters
-    ----------
-    edofs : numpy.ndarray
-        2d numpy array. Each row has the meaning of global degree of
-        freedom numbering for a given finite element.
-
-    Returns
-    -------
-    irows : numpy.ndarray
-        Global indices of the rows of the entries of stiffness matrices
-        of the elements.
-    icols : numpy.ndarray
-        Global indices of the columns of the entries of stiffness matrices
-        of the elements.
-
-    Notes
-    -----
-    The implementation assumes that every cell has the same number of
-    degrees of freedom.
-    """
-    nE, nNE = edofs.shape
-    nTOTV = nNE * nNE
-    irows = np.zeros((nE, nTOTV), dtype=edofs.dtype)
-    icols = np.zeros((nE, nTOTV), dtype=edofs.dtype)
-    for iNE in prange(nNE):
-        for jNE in prange(nNE):
-            i = iNE * nNE + jNE
-            for iE in prange(nE):
-                irows[iE, i] = edofs[iE, iNE]
-                icols[iE, i] = edofs[iE, jNE]
-    return irows, icols
-
-
-@njit(nogil=True, parallel=False, cache=False)
-def irows_icols_jagged(edofs: JaggedArray, irows, icols):
-    """
-    Returns row and column index data for several finite elements of different
-    kinds.
-
-    Parameters
-    ----------
-    edofs : JaggedArray
-        2d jagged array. Each row has the meaning of global degree of
-        freedom numbering for a given finite element.
-    irows, icols
-        Awkward array builders.
-    """
-    for iE in range(len(edofs)):
-        dofs = edofs[iE]
-        irows.begin_list()
-        icols.begin_list()
-        nDOF = len(dofs)
-        for iDOF in range(nDOF):
-            for jDOF in range(nDOF):
-                irows.integer(dofs[iDOF])
-                icols.integer(dofs[jDOF])
-        irows.end_list()
-        icols.end_list()
-
-
-@njit(nogil=True, cache=__cache, parallel=True)
-def irows_icols_bulk_filtered(edofs: np.ndarray, inds: np.ndarray) -> Tuple[ndarray]:
-    """
-    Returns row and column index data for finite elements specified
-    by the index array `inds`.
-
-    Parameters
-    ----------
-    edofs : numpy.ndarray
-        2d numpy array. Each row has the meaning of global degree of
-        freedom numbering for a given finite element.
-    inds: numpy.ndarray
-        1d numpy array of integers specifying active elements in an assembly.
-
-    Returns
-    -------
-    irows : numpy.ndarray
-        Global indices of the rows of the entries of stiffness matrices
-        of the elements.
-    icols : numpy.ndarray
-        Global indices of the columns of the entries of stiffness matrices
-        of the elements.
-
-    Notes
-    -----
-    The implementation assumes that every cell has the same number of
-    degrees of freedom.
-    """
-    nI = len(inds)
-    nNE = edofs.shape[1]
-    nTOTV = nNE * nNE
-    irows = np.zeros((nI, nTOTV), dtype=edofs.dtype)
-    icols = np.zeros((nI, nTOTV), dtype=edofs.dtype)
-    for iNE in prange(nNE):
-        for jNE in prange(nNE):
-            i = iNE * nNE + jNE
-            for iI in prange(nI):
-                irows[iI, i] = edofs[inds[iI], iNE]
-                icols[iI, i] = edofs[inds[iI], jNE]
-    return irows, icols
-
-
-def irows_icols(
-    edofs: Union[JaggedArray, ndarray, ak.Array], inds: ndarray = None
-) -> Tuple[Union[JaggedArray, ndarray]]:
-    """
-    Returns row and column indices for coefficient matrices of several finite
-    elements.
-
-    Parameters
-    ----------
-    edofs : numpy.ndarray or JaggedArray or awkward.Array
-        2d numpy array. Each row has the meaning of coefficient numbering for a
-        given finite element.
-    inds: numpy.ndarray, Optional
-        1d numpy array of integers specifying active elements in an assembly.
-        Default is None.
-
-    Returns
-    -------
-    Tuple[Union[JaggedArray, ndarray]]
-        Two NumPy arrays or two JaggedArrays.
-    """
-    if isinstance(edofs, ndarray):
-        if inds:
-            return irows_icols_bulk_filtered(edofs, inds)
-        else:
-            return irows_icols_bulk(edofs)
-    elif isinstance(edofs, ak.Array):
-        if inds:
-            raise NotImplementedError
-        else:
-            irows = ak.ArrayBuilder()
-            icols = ak.ArrayBuilder()
-            irows_icols_jagged(edofs, irows, icols)
-            return JaggedArray(irows.snapshot()), JaggedArray(icols.snapshot())
-    elif isinstance(edofs, JaggedArray):
-        return irows_icols(edofs.to_ak(), inds)
-
-
-@njit(nogil=True, cache=__cache, parallel=True)
-def topo_to_gnum(topo: np.ndarray, ndofn: int):
-    """
-    Returns global dof numbering based on element
-    topology data.
-
-    Parameters
-    ----------
-    topo : numpy.ndarray
-        2d numpy array of integers. Topology array listing global
-        node numbers for several elements.
-    ndofn : int
-        Number of degrees of freedoms per node.
-
-    Returns
-    -------
-    gnum : numpy.ndarray
-        2d numpy array of integers.
-    """
-    nE, nNE = topo.shape
-    gnum = np.zeros((nE, nNE * ndofn), dtype=topo.dtype)
-    for i in prange(nE):
-        for j in prange(nNE):
-            for k in prange(ndofn):
-                gnum[i, j * ndofn + k] = topo[i, j] * ndofn + k
-    return gnum
-
-
-@njit(nogil=True, cache=__cache, parallel=True)
-def topo_to_gnum_jagged(topo, gnum, ndofn: int):
-    """
-    Returns global dof numbering based on element
-    topology data.
-
-    Parameters
-    ----------
-    topo : numpy.ndarray
-        2d array of integers. Topology array listing global
-        node numbers for several elements.
-    gnum : numpy.ndarray or Awkward array
-        2d buffer array for the results.
-    ndofn : int
-        Number of degrees of freedoms per node.
-
-    Returns
-    -------
-    gnum : numpy.ndarray
-        2d numpy array of integers.
-    """
-    nE, _ = topo.shape
-    for i in prange(nE):
-        for j in prange(len(topo[i])):
-            for k in prange(ndofn):
-                gnum[i, j * ndofn + k] = topo[i, j] * ndofn + k
-    return gnum
-
-
-@njit(nogil=True, parallel=False, fastmath=True, cache=__cache)
-def penalty_factor_matrix(cellfixity: ndarray, shp: ndarray):
-    nE, nNE, nDOF = cellfixity.shape
-    N = nDOF * nNE
-    res = np.zeros((nE, N, N), dtype=shp.dtype)
-    for iE in prange(nE):
-        for iNE in prange(nNE):
-            for iDOF in prange(nDOF):
-                fix = cellfixity[iE, iNE, iDOF]
-                for jNE in prange(nNE):
-                    i = jNE * nDOF + iDOF
-                    for kNE in prange(nNE):
-                        j = kNE * nDOF + iDOF
-                        res[iE, i, j] += fix * shp[iNE, jNE] * shp[iNE, kNE]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def approximation_matrix(ndf: ndarray, NDOFN: int):
-    """
-    Returns a matrix of approximation coefficients
-    for all elements.
-    """
-    nE, nNE = ndf.shape[:2]
-    N = nNE * NDOFN
-    nappr = np.eye(N, dtype=ndf.dtype)
-    res = np.zeros((nE, N, N), dtype=ndf.dtype)
-    for iE in prange(nE):
-        for i in prange(nNE):
-            for j in prange(nNE):
-                for ii in prange(NDOFN):
-                    for jj in prange(NDOFN):
-                        res[iE, i * 2 + ii, j * 2 + jj] = nappr[i, j] * ndf[iE, i]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def nodal_approximation_matrix(ndf: ndarray):
-    """
-    Returns a matrix of nodal approximation coefficients
-    for all elements.
-    """
-    nE, nNE = ndf.shape[:2]
-    nappr = np.eye(nNE, dtype=ndf.dtype)
-    res = np.zeros((nE, nNE, nNE), dtype=ndf.dtype)
-    for iE in prange(nE):
-        for i in prange(nNE):
-            for j in prange(nNE):
-                res[iE, i, j] = nappr[i, j] * ndf[iE, i]
-    return res
-
-
-@njit(nogil=True, cache=__cache)
-def nodal_compatibility_factors(nam_csr_tot: csr, nam: ndarray, topo: ndarray):
-    indptr = nam_csr_tot.indptr
-    indices = nam_csr_tot.indices
-    data = nam_csr_tot.data
-    nN = len(indptr) - 1
-    widths = np.zeros(nN, dtype=indptr.dtype)
-    for iN in range(nN):
-        widths[iN] = indptr[iN + 1] - indptr[iN]
-    factors = dict()
-    nreg = dict()
-    for iN in range(nN):
-        factors[iN] = np.zeros((widths[iN], widths[iN]), dtype=nam.dtype)
-        nreg[iN] = indices[indptr[iN] : indptr[iN + 1]]
-    nE, nNE = topo.shape
-    for iE in range(nE):
-        topoE = topo[iE]
-        for jNE in range(nNE):
-            nID = topo[iE, jNE]
-            dataN = data[indptr[nID] : indptr[nID + 1]]
-            topoN = nreg[nID]
-            dataNE = np.zeros(widths[nID], dtype=nam.dtype)
-            imap = find1d(topoE, topoN)
-            dataNE[imap] = nam[iE, jNE]
-            rNE = dataN - dataNE  # residual
-            factors[nID] += np.outer(rNE, rNE)
-    return factors, nreg
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def compatibility_factors_to_coo(ncf: dict, nreg: dict):
-    """
-    ncf : nodal_compatibility_factors
-    """
-    nN = len(ncf)
-    widths = np.zeros(nN, dtype=np.int32)
-    for iN in prange(nN):
-        widths[iN] = len(nreg[iN])
-    shapes = (widths**2).astype(np.int64)
-    N = np.sum(shapes)
-    data = np.zeros(N, dtype=np.float64)
-    rows = np.zeros(N, dtype=np.int32)
-    cols = np.zeros(N, dtype=np.int32)
-    c = 0
-    for iN in range(nN):
-        data[c : c + shapes[iN]] = flatten2dC(ncf[iN])
-        nNN = widths[iN]
-        for jNN in prange(nNN):
-            for kNN in prange(nNN):
-                rows[c + jNN * nNN + kNN] = nreg[iN][jNN]
-                cols[c + jNN * nNN + kNN] = nreg[iN][kNN]
-        c += shapes[iN]
-    return data, rows, cols
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def topo1d_to_gnum1d(topo1d: ndarray, NDOFN: int):
-    nN = topo1d.shape[0]
-    gnum1d = np.zeros(nN * NDOFN, dtype=topo1d.dtype)
-    for i in prange(nN):
-        for j in prange(NDOFN):
-            gnum1d[i * NDOFN + j] = topo1d[i] * NDOFN + j
-    return gnum1d
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def ncf_to_cf(ncf: ndarray, NDOFN: int):
-    nN = ncf.shape[0]
-    cf = np.zeros((nN * NDOFN, nN * NDOFN), dtype=ncf.dtype)
-    for i in prange(nN):
-        for ii in prange(NDOFN):
-            for j in prange(nN):
-                cf[i * NDOFN + ii, j * NDOFN + ii] = ncf[i, j]
-    return cf
-
-
-@njit(nogil=True, cache=__cache)
-def compatibility_factors(ncf: dict, nreg: dict, NDOFN: int):
-    """ncf : nodal_compatibility_factors"""
-    nN = len(ncf)
-    widths = np.zeros(nN, dtype=np.int32)
-    for iN in prange(nN):
-        widths[iN] = len(nreg[iN])
-    cf = dict()
-    reg = dict()
-    for iN in range(nN):
-        cf[iN] = ncf_to_cf(ncf[iN], NDOFN)
-        reg[iN] = topo1d_to_gnum1d(nreg[iN], NDOFN)
-    return cf, reg
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def element_dofmap_bulk(dofmap: ndarray, nDOF: int, nNODE: int):
-    nDOF_ = dofmap.shape[0]
-    res = np.zeros(nNODE * nDOF_, dtype=dofmap.dtype)
-    for i in prange(nNODE):
-        for j in prange(nDOF_):
-            res[i * nDOF_ + j] = i * nDOF + dofmap[j]
-    return res
-
-
-@njit(nogil=True, parallel=False, cache=__cache)
-def expand_shape_function_matrix_bulk(
-    A_in: ndarray, A_out: ndarray, dofmap: ndarray
-) -> ndarray:
-    """
-    Expands the shape function matrices into a standard form.
-    """
-    # nE, nP, nV, nX_in
-    nX = A_in.shape[-1]
-    for iX in prange(nX):
-        A_out[:, :, :, dofmap[iX]] = A_in[:, :, :, iX]
-    return A_out
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def expand_coeff_matrix_bulk(A_in: ndarray, A_out: ndarray, dofmap: ndarray) -> ndarray:
-    """
-    Expands the local coefficient matrices into a standard form. It is used
-    for instance when the total matrix is built up of smaller parts.
-    """
-    nDOF = dofmap.shape[0]
-    nV = A_in.shape[0]
-    for i in prange(nDOF):
-        for j in prange(nDOF):
-            for k in prange(nV):
-                A_out[k, dofmap[i], dofmap[j]] = A_in[k, i, j]
-    return A_out
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def expand_load_vector_bulk(v_in: ndarray, v_out: ndarray, dofmap: ndarray) -> ndarray:
-    """
-    Expands the local load vectors into a standard form.
-    """
-    nDOF = dofmap.shape[0]
-    nV0 = v_out.shape[0]
-    nV1 = v_out.shape[2]
-    for i in prange(nDOF):
-        for j in prange(nV0):
-            for k in prange(nV1):
-                v_out[j, dofmap[i], k] = v_in[j, i, k]
-    return v_out
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def nodal_mass_matrix_data(nodal_masses: ndarray, ndof: int = 6):
-    N = nodal_masses.shape[0]
-    res = np.zeros((N * ndof))
-    for i in prange(N):
-        res[i * ndof : i * ndof + 3] = nodal_masses[i]
-    return res
-
-
-def min_stiffness_diagonal(K: Union[ndarray, spmatrix]) -> float:
-    """
-    Returns the minimum diagonal entry of the stiffness matrix.
-
-    Parameters
-    ----------
-    K : Union[ndarray, spmatrix]
-        The stiffness matrix as a dense or a sparse array.
-    """
-    if isinstance(K, spmatrix):
-        return np.min(K.diagonal())
-    else:
-        i = np.arange(K.shape[-1])
-        return np.min(K[:, i, i])
+# -*- coding: utf-8 -*-
+from typing import Callable
+from numba import njit, prange
+import numpy as np
+from numpy import ndarray
+
+from neumann.linalg import inv
+
+from polymesh.utils import cells_coords
+
+__cache = True
+
+
+@njit(nogil=True, cache=__cache)
+def element_coordinates(coords: ndarray, topo: np.ndarray):
+    return cells_coords(coords, topo)
+
+
+def element_centers(ecoords: np.ndarray):
+    return np.mean(ecoords, axis=1)
+
+
+@njit(nogil=True, cache=__cache)
+def loc_to_glob(pcoord: np.ndarray, gcoords: np.ndarray, shpfnc: Callable):
+    """Local to global transformation for a single cell and point.
+
+    Returns global coordinates of a point in an element, provided the global
+    corodinates of the points of the element, an array of parametric
+    coordinates and a function to evaluate the shape functions.
+
+    Parameters
+    ----------
+    gcoords : (nNE, nD) ndarray
+        2D array containing coordinates for every node of a single element.
+            nNE : number of vertices of the element
+            nD : number of dimensions of the model space
+
+    pcoords : (nDP, ) ndarray
+        1D array of parametric coordinates for a single point.
+            nDP : number of dimensions of the parametric space
+
+    shpfnc : Callable
+        A function that evaluates shape function values at a point,
+        specified with parametric coordinates.
+
+    Returns
+    -------
+    (nD, ) ndarray
+        Global cooridnates of the specified point.
+
+    Notes
+    -----
+    'shpfnc' must be a numba-jitted function, that accepts a 1D array of
+    exactly nDP number of components.
+    """
+    return gcoords.T @ shpfnc(pcoord)
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def loc_to_glob_bulk(pcoords: np.ndarray, gcoords: np.ndarray,
+                     shpfnc: Callable):
+    """Local to global transformation for multiple cells and points.
+
+    Returns global coordinates of points expressed in parametric coordinates.
+
+    Parameters
+    ----------
+    gcoords : (nE, nNE, nD) ndarray
+        3D array containing coordinates for every node of every element.
+            nE : number of elements
+            nNE : number of vertices of the element
+            nD : number of dimensions of the model space
+
+    pcoords : (nP, nDP) ndarray
+        2D array of parametric coordinates for several points.
+            nP : number of points
+            nDP : number of dimensions of the parametric space
+
+    shpfnc : Callable
+        A function that evaluates shape function values at a point,
+        specified with parametric coordinates.
+
+    Returns
+    -------
+    (nE, nP, nD) ndarray
+        Global cooridnates of the specified points in the specified elements.
+        Dummy axes are collapsed, so the result may be 1, 2 or 3 dimensional,
+        depending on the shapes of the input arrays.
+
+    Notes
+    -----
+    'shpfnc' must be a numba-jitted function, that accepts a 1D array of
+    exactly nDP number of components.
+    """
+    nE, nNE, nD = gcoords.shape
+    nP, _ = pcoords.shape
+    res = np.zeros((nE, nP, nD), dtype=gcoords.dtype)
+    for iP in prange(nP):
+        shp = shpfnc(pcoords[iP])
+        for iE in prange(nE):
+            for iD in prange(nD):
+                for iNE in prange(nNE):
+                    res[iE, iP, iD] += gcoords[iE, iNE, iD] * shp[iNE]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def glob_to_loc(coord: np.ndarray, gcoords: np.ndarray, lcoords: np.ndarray,
+                monomsfnc: Callable):
+    """Global to local transformation for a single point and cell.
+
+    Returns local coordinates of a point in an element, provided the global
+    corodinates of the points of the element, an array of global
+    coordinates and a function to evaluate the monomials of the shape
+    functions.
+
+    Parameters
+    ----------
+    gcoords : (nNE, nD) ndarray
+        2D array containing coordinates for every node of a single element.
+            nNE : number of vertices of the element
+            nD : number of dimensions of the model space
+
+    coord : (nD, ) ndarray
+        1D array of global coordinates for a single point.
+            nD : number of dimensions of the model space
+
+    lcoords : (nNE, nDP) ndarray
+        2D array of local coordinates of the parametric element.
+            nNE : number of vertices of the element
+            nDP : number of dimensions of the parametric space
+
+    monomsfnc : Callable
+        A function that evaluates monomials of the shape functions at a point
+        specified with parametric coordinates.
+
+    Returns
+    -------
+    (nDP, ) ndarray
+        Parametric cooridnates of the specified point.
+
+    Notes
+    -----
+    'shpfnc' must be a numba-jitted function, that accepts a 1D array of
+    exactly nDP number of components.
+    """
+    nNE = gcoords.shape[0]
+    monoms = np.zeros((nNE, nNE), dtype=coord.dtype)
+    for i in prange(nNE):
+        monoms[:, i] = monomsfnc(gcoords[i])
+    coeffs = inv(monoms)
+    shp = coeffs @ monomsfnc(coord)
+    return lcoords.T @ shp
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def glob_to_loc_bulk(coords: np.ndarray, gcoords: np.ndarray,
+                     lcoords: np.ndarray, monomsfnc: Callable):
+    """Global to local transformation for multiple cells and points.
+
+    Returns local coordinates of a point in an element, provided the global
+    corodinates of the points of the element, an array of global
+    coordinates and a function to evaluate the monomials of the shape
+    functions.
+
+    Parameters
+    ----------
+    gcoords : (nE, nNE, nD) ndarray
+        3D array containing coordinates for every node of several elements.
+            nE : number of elements
+            nNE : number of vertices of the element
+            nD : number of dimensions of the model space
+
+    coords : (nP, nD) ndarray
+        2D array of global coordinates for several points.
+            nP : number of points
+            nD : number of dimensions of the model space
+
+    lcoords : (nNE, nDP) ndarray
+        2D array of local coordinates of the parametric element.
+            nNE : number of vertices of the element
+            nDP : number of dimensions of the parametric space
+
+    monomsfnc : Callable
+        A function that evaluates monomials of the shape functions at a point
+        specified with parametric coordinates.
+
+    Returns
+    -------
+    (nP, nE, nDP) ndarray
+        Parametric cooridnates of the specified points in all elements.
+
+    Notes
+    -----
+    'shpfnc' must be a numba-jitted function, that accepts a 1D array of
+    exactly nDP number of components, where nDP is the number
+    of paramatric cooridnate dimensions.
+    """
+    nE, nNE, _ = gcoords.shape
+    nP = len(coords)
+    nDP = lcoords.shape[1]
+    lcoords = lcoords.T
+    res = np.zeros((nP, nE, nDP), dtype=gcoords.dtype)
+    monoms = np.zeros((nNE, nNE), dtype=gcoords.dtype)
+    shp = np.zeros(nNE, dtype=gcoords.dtype)
+    coeffs = np.zeros_like(monoms)
+    for iE in prange(nE):
+        for iNE in prange(nNE):
+            monoms[:, iNE] = monomsfnc(gcoords[iE, iNE])
+        coeffs[:, :] = inv(monoms)
+        for iP in prange(nP):
+            shp[:] = coeffs @ monomsfnc(coords[iP])
+            res[iP, iE, :] = lcoords @ shp
+    return res
+
+
+@njit(nogil=True, cache=__cache)
+def pip(coord: np.ndarray, gcoords: np.ndarray, lcoords: np.ndarray,
+        monomsfnc: Callable, shpfnc: Callable, tol=1e-12):
+    """Point-in-polygon test for a single cell and point.
+
+    Performs the point-in-poligon test for a single point and cell.
+    False means that the point is outside of the cell, True means the point
+    is either inside, or on the boundary of the cell.
+
+    Parameters
+    ----------
+    gcoords : (nNE, nD) ndarray
+        2D array containing coordinates for every node of a single element.
+            nNE : number of vertices of the element
+            nD : number of dimensions of the model space
+
+    coord : (nD, ) ndarray
+        1D array of global coordinates for a single point.
+            nD : number of dimensions of the model space
+
+    lcoords : (nNE, nDP) ndarray
+        2D array of local coordinates of the parametric element.
+            nNE : number of vertices of the element
+            nDP : number of dimensions of the parametric space
+
+    monomsfnc : Callable
+        A function that evaluates monomials of the shape functions at a point
+        specified with parametric coordinates.
+
+    shpfnc : Callable
+        A function that evaluates shape function values at a point,
+        specified with parametric coordinates.
+
+    Returns
+    -------
+    bool
+        False if points is outside of the cell, True otherwise.
+
+    Notes
+    -----
+    'shpfnc'  and 'monomsfnc' must be numba-jitted functions, that accept
+    a 1D array of exactly nDP number of components, where nDP is the number
+    of paramatric cooridnate dimensions.
+    """
+    limit = 1 + tol
+    loc = glob_to_loc(coord, gcoords, lcoords, monomsfnc)
+    return np.all(shpfnc(loc) <= limit)
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def int_domain(points: np.ndarray, qpos: np.ndarray, qweight: np.ndarray,
+               dshpfnc: Callable, weight: float = 1.0):
+    """
+    Returns the measure (length, area or volume in 1d, 2d and 3d) of a 
+    single domain.
+    """
+    volume = 0.
+    points = np.transpose(points)
+    nG = len(qweight)
+    for iG in prange(nG):
+        jac = points @ dshpfnc(qpos[iG])
+        djac = np.linalg.det(jac)
+        volume += qweight[iG] * djac
+    return volume * weight
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def int_domains(ecoords: np.ndarray, qpos: np.ndarray,
+                qweight: np.ndarray, dshpfnc: Callable):
+    """
+    Returns the measure (length, area or volume in 1d, 2d and 3d) of 
+    several domains.
+    """
+    nE = ecoords.shape[0]
+    res = np.zeros(nE, dtype=ecoords.dtype)
+    nG = len(qweight)
+    for iG in prange(nG):
+        dshp = dshpfnc(qpos[iG])
+        for i in prange(nE):
+            jac = ecoords[i].T @ dshp
+            djac = np.linalg.det(jac)
+            res[i] += qweight[iG] * djac
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def stiffness_matrix(C: np.ndarray, ecoords: np.ndarray, qpos: np.ndarray,
+                     qweight: np.ndarray, dshpfnc: Callable,
+                     sdmfnc: Callable, nDOFN=3):
+    nTOTV = len(ecoords) * nDOFN
+    res = np.zeros((nTOTV, nTOTV), dtype=C.dtype)
+    points = np.transpose(ecoords)
+    nG = len(qweight)
+    for iG in prange(nG):
+        dshp = dshpfnc(qpos[iG])
+        jac = points @ dshp
+        djac = np.linalg.det(jac) * qweight[iG]
+        B = sdmfnc(jac, dshp)
+        res += B.T @ C @ B * djac
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def stiffness_matrix_bulk(C: np.ndarray, ecoords: np.ndarray,
+                          qpos: np.ndarray, qweight: np.ndarray,
+                          dshpfnc: Callable, sdmfnc: Callable, nDOFN=3):
+    nE, nNODE, _ = ecoords.shape
+    nTOTV = nNODE * nDOFN
+    res = np.zeros((nE, nTOTV, nTOTV), dtype=C.dtype)
+    nG = len(qweight)
+    for iG in prange(nG):
+        dshp = dshpfnc(qpos[iG])
+        for iE in prange(nE):
+            jac = np.transpose(ecoords[iE]) @ dshp
+            djac = np.linalg.det(jac) * qweight[iG]
+            B = sdmfnc(jac, dshp)
+            res[iE] += B.T @ C[iE] @ B * djac
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def strain_displacement_matrix_bulk2(B: ndarray, djac: ndarray, w: ndarray):
+    nE, nG, nSTRE, nTOTV = B.shape
+    res = np.zeros((nE, nSTRE, nTOTV), dtype=B.dtype)
+    for iG in range(nG):
+        for iE in prange(nE):
+            res[iE] += B[iE, iG] * djac[iE, iG] * w[iG]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def unit_strain_load_vector_bulk(D: ndarray, B: ndarray):
+    nE, nSTRE, nTOTV = B.shape
+    res = np.zeros((nE, nTOTV, nSTRE), dtype=D.dtype)
+    for iE in prange(nE):
+        res[iE] = B[iE].T @ D[iE]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def strain_load_vector_bulk(BTD: ndarray, strains: ndarray):
+    nE, nTOTV, nSTRE = BTD.shape
+    nE, nRHS, nSTRE = strains.shape
+    res = np.zeros((nE, nTOTV, nRHS), dtype=BTD.dtype)
+    for iE in prange(nE):
+        for iRHS in prange(nRHS):
+            res[iE, :, iRHS] = BTD[iE] @ strains[iE, iRHS, :]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def stiffness_matrix_bulk2(D: ndarray, B: ndarray, djac: ndarray, w: ndarray):
+    nE, nG = djac.shape
+    nTOTV = B.shape[-1]
+    res = np.zeros((nE, nTOTV, nTOTV), dtype=D.dtype)
+    for iG in range(nG):
+        for iE in prange(nE):
+            res[iE] += B[iE, iG].T @ D[iE] @ B[iE, iG] * djac[iE, iG] * w[iG]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def mass_matrix_bulk(N: ndarray, dens: ndarray, weights: ndarray,
+                     djac: ndarray, w: ndarray):
+    """
+    Evaluates the mass matrix of several elements from evaluations at the
+    Gauss points of the elements. The densities are assumed to be constant
+    over the elements, and be represented by the 1d float numpy array 'dens'.
+
+    Parameters
+    ----------
+    N : 4d numpy float array
+        Evaluations of the shape function matrix according to the type of 
+        the element for every cell and Gauss point.
+
+    dens : 1d numpy float array
+        1d float array of densities of several elements.
+
+    weights : 1d numpy float array
+        Array of weighting factors for the cells (eg. areas, volumes) with 
+        the same shape as 'dens'. 
+
+    w : 1d numpy float array
+        Weights of the Gauss points
+
+    djac : 2d numpy float array
+        Jacobi determinants for every element and Gauss point.
+
+    nE : number of elements
+    nG : number of Gauss points
+    nNE : number of nodes per element
+    nDOF : number of dofs per node
+
+    """
+    nE, nG = djac.shape
+    nTOTV = N.shape[-1]
+    res = np.zeros((nE, nTOTV, nTOTV), dtype=N.dtype)
+    for iG in range(nG):
+        for iE in prange(nE):
+            res[iE] += dens[iE] * weights[iE] * \
+                N[iE, iG].T @ N[iE, iG] * djac[iE, iG] * w[iG]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def compliance_bulk(K_bulk: np.ndarray, dofsol1d: np.ndarray,
+                    gnum: np.ndarray):
+    """
+    Returns the total compliance of the structure, that is
+        u.T @ K @ u
+    """
+    nE, nTOTV, _ = K_bulk.shape
+    res = np.zeros(nE, dtype=K_bulk.dtype)
+    for iE in prange(nE):
+        for i in prange(nTOTV):
+            for j in prange(nTOTV):
+                res[iE] += K_bulk[iE, i, j] * \
+                    dofsol1d[gnum[iE, i]] * dofsol1d[gnum[iE, j]]
+    return res
+
+
+@njit(nogil=True, cache=__cache)
+def elastic_strain_energy_bulk(K_bulk: np.ndarray, dofsol1d: np.ndarray,
+                               gnum: np.ndarray):
+    """
+    Returns the total elastic strain energy of the structure, that is 
+        0.5 * u.T @ K @ u
+    """
+    return compliance_bulk(K_bulk, dofsol1d, gnum) / 2
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def approx_dof_solution(dofsol1d: np.ndarray, gnum: np.ndarray,
+                        shpmat: np.ndarray):
+    nDOFN, nTOTV = shpmat.shape
+    res = np.zeros((nDOFN), dtype=dofsol1d.dtype)
+    for j in prange(nDOFN):
+        for k in prange(nTOTV):
+            res[j] += shpmat[j, k] * dofsol1d[gnum[k]]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def approx_dof_solution_bulk(dofsol1d: np.ndarray, gnum: np.ndarray,
+                             shpmat: np.ndarray):
+    nE = len(gnum)
+    nDOFN, nTOTV = shpmat.shape
+    res = np.zeros((nE, nDOFN), dtype=dofsol1d.dtype)
+    for i in prange(nE):
+        for j in prange(nDOFN):
+            for k in prange(nTOTV):
+                res[i, j] += shpmat[j, k] * dofsol1d[gnum[i, k]]
+    return res
+
+
+@njit(nogil=True, cache=__cache)
+def element_dof_solution(dofsol1d: np.ndarray, gnum: np.ndarray):
+    return dofsol1d[gnum]
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def element_dof_solution_bulk(dofsol1d: ndarray, gnum: ndarray):
+    nE, nEVAB = gnum.shape
+    res = np.zeros((nE, nEVAB), dtype=dofsol1d.dtype)
+    for i in prange(nE):
+        res[i, :] = dofsol1d[gnum[i, :]]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def element_dof_solution_bulk_multi(dofsol: ndarray, gnum: ndarray):
+    nRHS = dofsol.shape[-1]
+    nE, nEVAB = gnum.shape
+    res = np.zeros((nRHS, nE, nEVAB), dtype=dofsol.dtype)
+    for i in prange(nE):
+        for j in prange(nRHS):
+            res[j, i, :] = dofsol[gnum[i, :], j]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def avg_nodal_data_bulk(data: np.ndarray, topo: np.ndarray):
+    nE, nNE, nD = data.shape
+    nP = np.max(topo) + 1
+    res = np.zeros((nP, nD), dtype=data.dtype)
+    count = np.zeros((nP), dtype=topo.dtype)
+    for iE in prange(nE):
+        for jNE in prange(nNE):
+            res[topo[iE, jNE]] += data[iE, jNE]
+            count[topo[iE, jNE]] += 1
+    for iP in prange(nP):
+        res[iP] = res[iP] / count[iP]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def stresses_at_point_bulk(C: np.ndarray, dofsol1d: np.ndarray,
+                           ecoords: np.ndarray, gnum: np.ndarray,
+                           dshp: np.ndarray, sdmfnc: Callable):
+    nE = len(gnum)  # number of elements
+    nSTRE = C.shape[-1]  # number of generalized forces
+    esol = element_dof_solution_bulk(dofsol1d, gnum)
+    res = np.zeros((nE, nSTRE), dtype=C.dtype)
+    for i in prange(nE):
+        jac = ecoords[i].T @ dshp
+        B = sdmfnc(jac, dshp)
+        res[i] = C[i] @ B @ esol[i]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def stresses_at_cells_nodes(C: np.ndarray, dofsol1d: np.ndarray,
+                            ecoords: np.ndarray, gnum: np.ndarray,
+                            dshp: np.ndarray, sdmfnc: Callable):
+    nE, nNODE, _ = ecoords.shape  # numbers of elements and element nodes
+    nSTRE = C.shape[-1]  # number of generalized forces
+    res = np.zeros((nE, nNODE, nSTRE), dtype=C.dtype)
+    for i in prange(nNODE):
+        res[:, i, :] = stresses_at_point_bulk(C, dofsol1d, ecoords, gnum,
+                                              dshp[i], sdmfnc)
+    return res
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/preproc.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,536 +1,654 @@
-from typing import Union, Tuple
-
-from scipy.sparse import coo_matrix
-from scipy.sparse import spmatrix
-import numpy as np
-from numpy import ndarray
-from numba import njit, prange
-
-from neumann.logical import isintegerarray, isfloatarray, isboolarray
-from neumann import bool_to_float, atleastnd, matrixform
-from neumann.linalg.sparse.utils import lower_spdata, upper_spdata
-
-from .fem import (
-    nodes2d_to_dofs1d,
-    irows_icols_bulk,
-    nodal_mass_matrix_data,
-    min_stiffness_diagonal,
-)
-from .imap import index_mappers, box_spmatrix, box_rhs, box_dof_numbering
-from ...fem.constants import DEFAULT_DIRICHLET_PENALTY
-
-__cache = True
-
-
-def fem_coeff_matrix_coo(
-    A: ndarray,
-    *args,
-    inds: ndarray = None,
-    rows: ndarray = None,
-    cols: ndarray = None,
-    N: int = None
-):
-    """
-    Returns the coefficient matrix in sparse 'coo' format.
-    Index mapping is either specified with `inds` or with
-    both `rows` and `cols`.
-
-    If `lower` or `upper` is provided as a positional argument,
-    the result is returned as a lower- or upper-triangular matrix,
-    respectively.
-
-    Parameters
-    ----------
-    A : np.ndarray
-        Element coefficient matrices as a 3d array. The lengths if the last
-        two axes must be the same.
-    inds : np.ndarray, Optional
-        Global indices of all quantities of an element as a 2d integer array.
-        Length of the second axis must match the lengths of the 2nd and 3rd
-        axes of 'A'.
-        Default is None.
-    rows : np.ndarray, Optional
-        Global numbering of the rows as an 1d integer array. Length must
-        equal the flattened length of 'A'. Default is None.
-    cols : np.ndarray, Optional
-        Global numbering of the columns as an 1d integer array. Length must
-        equal the flattened length of 'A'. Default is None.
-    N : int, Optional
-        Total number of coefficients in the system. If not provided,
-        it is inferred from index data.
-
-    Returns
-    -------
-    scipy.sparse.coo_matrix
-        Coefficient matrix in sparse coo format (see scipy doc for the details).
-    """
-    if N is None:
-        assert inds is not None, "shape or `inds` must be provided!."
-        N = inds.max() + 1
-    if rows is None:
-        assert inds is not None, (
-            "Row and column indices (`rows` and `cols`) "
-            "or global index numbering array (inds) must be provided!"
-        )
-        rows, cols = irows_icols_bulk(inds)
-
-    data, rows, cols = A.flatten(), rows.flatten(), cols.flatten()
-
-    if len(args) > 0:
-        if "lower" in args:
-            data, rows, cols = lower_spdata(data, rows, cols)
-        elif "upper" in args:
-            data, rows, cols = upper_spdata(data, rows, cols)
-
-    return coo_matrix((data, (rows, cols)), shape=(N, N))
-
-
-def _build_nodal_data(values: ndarray, *, inds: ndarray = None, N: int = None):
-    """
-    Returns nodal data of any sort in standard form.
-
-    The data is given with 'values' and applies to the node indices specified
-    by 'inds'. At all times, the function must be informed about the total number of
-    nodes in the model, to return an output with a correct shape. If 'inds' is None, it
-    is assumed that 'values' contains data for each node in the model, and therefore
-    the length of 'values' is the number of nodes in the model. Otherwise, the number of
-    nodes is inferred from 'inds' and 'N' (see the doc).
-
-    Parameters
-    ----------
-    values : numpy.ndarray
-        2d or 3d numpy array of floats, that specify some sort of data
-        imposed on nodes for one or several datasets. If it is a 3d array, the length
-        of the third axis equals the number of datasets.
-    inds : numpy.ndarray, Optional
-        1d numpy integer array specifying global indices for the rows of 'values'.
-    N : int, Optional
-        The overall number of nodes in the model. If not provided, we assume that
-        it equals the highest index in 'inds' + 1 (this assumes zero-based indexing).
-
-    Notes
-    -----
-    The function returns the values as a 2d array, even if the input array was only
-    2 dimensional, which suggests a single load case.
-
-    Returns
-    -------
-    indices : numpy.ndarray
-        1d numpy integer array of npde indices
-    nodal_loads : numpy.ndarray
-        2d numpy float array of shape (nN * nDOF, nX), where nN, nDOF and nX
-        are the number of nodes, degrees of freedom and datasets.
-    N : int
-        The overall size of the equation system, as derived from the input.
-    """
-    assert isfloatarray(values)
-
-    # node based definition with multiple RHS (at least 1)
-    values = atleastnd(values, 3, back=True)  # (nP, nDOF, nRHS)
-    if inds is None:
-        inds = np.arange(len(values))  # node indices
-    else:
-        assert isintegerarray(inds)
-        assert len(values) == len(inds)
-
-    # transform to nodal defintion
-    inds, values = nodes2d_to_dofs1d(inds, values)
-
-    N = inds.max() + 1 if N is None else N
-    return inds, values, N
-
-
-def nodal_load_vector(values: ndarray, **kwargs) -> ndarray:
-    """
-    Assembles the right-hand-side of the global equation system.
-
-    Parameters
-    ----------
-    values : numpy.ndarray, Optional
-        2d or 3d numpy array of floats. If 3d, it is assumed that
-        the last axis runs along load cases.
-
-    Returns
-    -------
-    numpy.ndarray
-        The load vector as a 1d or 2d numpy array of floats.
-    """
-    inds, values, N = _build_nodal_data(values, **kwargs)
-    nRHS = values.shape[-1]
-    f = np.zeros((N, nRHS))
-    f[inds] = values
-    return f
-
-
-@njit(nogil=True, parallel=False, fastmath=True, cache=__cache)
-def assemble_load_vector(values: ndarray, gnum: ndarray, N: int = -1):
-    """
-    Returns global dof numbering based on element topology data.
-
-    Parameters
-    ----------
-    values : numpy.ndarray
-        3d numpy float array of shape (nE, nEVAB, nRHS), representing
-        element data. The length of the second axis matches the the number of
-        degrees of freedom per cell.
-    gnum : int
-        Global indices of local degrees of freedoms of elements.
-    N : int, Optional
-        The number of total unknowns in the system. Must be specified correcly,
-        to get a vector the same size of the global system. If not specified, it is
-        inherited from 'gnum' (as 'gnum.max() + 1'), but this can lead to a chopped
-        array.
-
-    Returns
-    -------
-    numpy.ndarray
-        2d numpy array of integers with a shape of (N, nRHS), where nRHS is the number
-        if right hand sizes (load cases).
-    """
-    nE, nEVAB, nRHS = values.shape
-    if N < 0:
-        N = gnum.max() + 1
-    res = np.zeros((N, nRHS), dtype=values.dtype)
-    for i in range(nE):
-        for j in range(nEVAB):
-            for k in range(nRHS):
-                res[gnum[i, j], k] += values[i, j, k]
-    return res
-
-
-def essential_penalty_factor_matrix(
-    fixity: ndarray = None,
-    *,
-    inds: ndarray = None,
-    N: int = None,
-    eliminate_zeros: bool = True,
-    sum_duplicates: bool = True
-) -> coo_matrix:
-    """
-    Returns the penalty factor matrix. This matrix is the basis of several penalty
-    matrices used to enforce constraints on the primary variables.
-
-    At all times, the function must be informed about the total number of nodes in the
-    model, to return an output with a correct shape. If 'inds' is None, it is assumed that
-    'fixity' contains data for each node in the model, and therefore the length of 'fixity'
-    is the number of nodes in the model. You can also use 'N' to indicate the number of
-    nodes, in which case entries according to 'inds' are marked as constrained.
-
-    Parameters
-    ----------
-    fixity : numpy.ndarray, Optional
-        Fixity information as a 2d boolean array.
-    inds : numpy.ndarray, Optional
-        1d numpy integer array specifying node indices.
-    N : int, Optional
-        The overall number of nodes in the model. If not provided, we assume that
-        it equals the highest index in 'inds' + 1 (this assumes zero-based indexing).
-    """
-    if fixity is not None:
-        assert isboolarray(fixity)
-    else:
-        if isintegerarray(inds):
-            if not isinstance(N, int):
-                N = inds.max() + 1  # assumes zero based indexing
-            fixity = np.zeros(N, dtype=bool)
-            fixity[inds] = True
-    assert isboolarray(fixity), "Invalid input!"
-    fixity = bool_to_float(fixity, 1.0, 0.0)
-    fixity = atleastnd(fixity, 3, back=True)
-    inds, fixity, N = _build_nodal_data(fixity, inds=inds, N=N)
-    K = coo_matrix((fixity[:, 0], (inds, inds)), shape=(N, N))
-    if eliminate_zeros:
-        K.eliminate_zeros()
-    if sum_duplicates:
-        K.sum_duplicates()
-    return K
-
-
-def essential_penalty_matrix(
-    fixity: ndarray = None,
-    *,
-    inds: ndarray = None,
-    pfix: float = DEFAULT_DIRICHLET_PENALTY,
-    eliminate_zeros: bool = True,
-    sum_duplicates: bool = True
-) -> coo_matrix:
-    """
-    Returns the sparse, COO format penalty matrix, equivalent of
-    a Courant-type penalization of the essential boundary conditions.
-
-    Parameters
-    ----------
-    fixity : numpy.ndarray, Optional
-        Fixity information as a 2d float or boolean array.
-    inds : numpy.ndarray, Optional
-        1d integer array specifying global indices for the rows of 'values'.
-    pfix : float, Optional
-        Penalty value for fixed dofs. It is used to transform boolean penalty
-        data, or to make up for missing values (e.g. only indices are provided).
-        Default is `sigmaepsilon.fem.constants.DEFAULT_DIRICHLET_PENALTY`.
-    eliminate_zeros : bool, Optional
-        Eliminates zeros from the matrix. Default is True.
-    eliminate_zeros : bool, Optional
-        Summs duplicate entries in the matrix. Default is True.
-
-    Returns
-    -------
-    scipy.sparse.coo_matrix
-        The penalty matrix in sparse COO format.
-    """
-    if fixity is not None:
-        assert isinstance(fixity, np.ndarray)
-    else:
-        if isintegerarray(inds):
-            if not isinstance(N, int):
-                N = inds.max() + 1  # assumes zero based indexing
-            fixity = np.zeros(N, dtype=bool)
-            fixity[inds] = True
-    if isboolarray(fixity):
-        fixity = bool_to_float(fixity, pfix)
-    assert isfloatarray(fixity)
-    fixity = atleastnd(fixity, 3, back=True)  # (nP, nDOF, nX)
-    inds, fixity, N = _build_nodal_data(fixity, inds=inds)
-    K = coo_matrix((fixity[:, 0], (inds, inds)), shape=(N, N))
-    if eliminate_zeros:
-        K.eliminate_zeros()
-    if sum_duplicates:
-        K.sum_duplicates()
-    return K
-
-
-def nodal_mass_matrix(
-    *args,
-    values: ndarray = None,
-    eliminate_zeros: bool = True,
-    sum_duplicates: bool = True,
-    ndof: int = 6,
-    **kwargs
-) -> coo_matrix:
-    """
-    Returns the diagonal mass matrix resulting form nodal masses in scipy
-    COO format.
-
-    Parameters
-    ----------
-    See the documentation of 'build_fem_ebc_data' for the discription
-    of the possible arguments.
-
-    Returns
-    -------
-    scipy.sparse.coo_matrix
-        The mass matrix in sparse COO format.
-    """
-    values = nodal_mass_matrix_data(values, ndof)
-    inds, vals, N = _build_nodal_data(values, **kwargs)
-    M = coo_matrix((vals[:, 0], (inds, inds)), shape=(N, N))
-    if eliminate_zeros:
-        M.eliminate_zeros()
-    if sum_duplicates:
-        M.sum_duplicates()
-    return M
-
-
-def estimate_stiffness_penalty(K: Union[ndarray, spmatrix], fixity: ndarray, N: int):
-    """
-    Returns a sugegsted value for the stiffness penalty, to account
-    for essential boundary conditions.
-
-    :math:`\\mathbf{M}`
-
-    .. math::
-        :nowrap:
-
-        \\begin{equation}
-            \\mathbf{A} \\mathbf{x} = \\lambda \\mathbf{x},
-        \\end{equation}
-
-    Parameters
-    ----------
-    K : Union[ndarray, spmatrix]
-        The stiffness matrix as a dense or a sparse array.
-    N : int
-        The number of degrees of freedom in the model.
-
-    References
-    ----------
-    .. [1] B. Nour-Omid, P. Wriggers "A two-level iteration method for
-       solution of contact problems." Computer Methods in Applied Mechanics
-       and Engineering, vol. 54, pp. 131-144, 1986.
-    """
-    eps = np.finfo(float).eps
-    kmin = min_stiffness_diagonal(K)
-    return kmin / np.sqrt(N * eps)
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def _pull_submatrix(A: ndarray, r: ndarray, c: ndarray) -> ndarray:
-    nR = r.shape[0]
-    nC = c.shape[0]
-    res = np.zeros((nR, nC), dtype=A.dtype)
-    for i in prange(nR):
-        for j in prange(nC):
-            res[i, j] = A[r[i], c[j]]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def _pull_subvector(v: ndarray, i: ndarray) -> ndarray:
-    nI = i.shape[0]
-    res = np.zeros((nI, v.shape[-1]), dtype=v.dtype)
-    for j in prange(nI):
-        res[j, :] = v[i[j], :]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def _push_submatrix(A: ndarray, Asub: ndarray, r: ndarray, c: ndarray):
-    nR = r.shape[0]
-    nC = c.shape[0]
-    for i in prange(nR):
-        for j in prange(nC):
-            A[r[i], c[j]] = Asub[i, j]
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def _push_subvector(v: ndarray, vsub: ndarray, i: ndarray):
-    nI = i.shape[0]
-    for j in prange(nI):
-        v[i[j], :] = vsub[j, :]
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def condensate_Kf_bulk(
-    K: ndarray, f: ndarray, fixity: ndarray
-) -> Tuple[ndarray, ndarray]:
-    """
-    Returns the condensed coefficient matrices representing constraints
-    on the internal forces of the elements (eg. hinges).
-
-    Currently this solution is only able to handle two states, being totally free
-    and being fully constrained. The fixity values are expected to be numbers between
-    0 and 1, where dofs with a factor > 0.5 are assumed to be the constrained ones.
-
-    Parameters
-    ----------
-    K : numpy.ndarray
-        3d float array, the stiffness matrices of several elements of the same kind.
-    factors: numpy.ndarray
-        2d boolean array of connectivity factors for each dof of several elements.
-
-    Returns
-    -------
-    numpy.ndarray
-        The condensed stiffness matrices with the same shape as `K`.
-    numpy.ndarray
-        The condensed load vectors with the same shape as `f`.
-    """
-    nE = K.shape[0]
-    K_out = np.zeros_like(K)
-    f_out = np.zeros_like(f)
-    for iE in prange(nE):
-        b = np.where(fixity[iE])[0]
-        i = np.where(~fixity[iE])[0]
-        # stiffness matrix
-        Kbb = _pull_submatrix(K[iE], b, b)
-        Kbi = _pull_submatrix(K[iE], b, i)
-        Kib = _pull_submatrix(K[iE], i, b)
-        Kii = _pull_submatrix(K[iE], i, i)
-        Kii_inv = np.linalg.inv(Kii)
-        Kbb -= Kbi @ Kii_inv @ Kib
-        _push_submatrix(K_out[iE], Kbb, b, b)
-        # load vector
-        fb = _pull_subvector(f[iE], b)
-        fi = _pull_subvector(f[iE], i)
-        fb -= Kbi @ Kii_inv @ fi
-        _push_subvector(f_out[iE], fb, b)
-    return K_out, f_out
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def condensate_M_bulk(M: ndarray, fixity: ndarray) -> ndarray:
-    """
-    Returns the condensed coefficient matrices representing constraints
-    on the internal forces of the elements (eg. hinges).
-
-    Parameters
-    ----------
-    M : numpy.ndarray
-        3d float array, the mass matrices of several elements of the same kind.
-    fixity: numpy.ndarray
-        2d float boolean of connectivity factors for each dof of several elements.
-
-    Returns
-    -------
-    numpy.ndarray
-        The condensed mass matrices with the same shape as `M`.
-    """
-    nE = M.shape[0]
-    M_out = np.zeros_like(M)
-    for iE in prange(nE):
-        b = np.where(fixity[iE])[0]
-        i = np.where(~fixity[iE])[0]
-        Mbb = _pull_submatrix(M[iE], b, b)
-        Mbi = _pull_submatrix(M[iE], b, i)
-        Mib = _pull_submatrix(M[iE], i, b)
-        Mii = _pull_submatrix(M[iE], i, i)
-        Mbb -= Mbi @ np.linalg.inv(Mii) @ Mib
-        _push_submatrix(M_out[iE], Mbb, b, b)
-    return M_out
-
-
-def assert_min_diagonals_bulk(K: ndarray, minval: float = 1e-12):
-    """
-    Guarantees, that the values in the diagonal are larger
-    a prescribed minimum value.
-
-    Parameters
-    ----------
-    A : numpy.ndarray
-        The coefficient matrix of several elements as a 3d
-        array, where elements run along the first axis.
-    minval : float, Optional
-        The minimum value. Default is 1e-12.
-
-    Returns
-    -------
-    numpy.ndarray
-        The modified coefficient matrix, with the same shape as 'K'.
-    """
-    inds = np.arange(K.shape[-1])
-    d = K[:, inds, inds]
-    eid, vid = np.where(d < minval)
-    K[eid, vid, vid] = minval
-    return K
-
-
-def box_fem_data_sparse(K_coo: coo_matrix, Kp_coo: coo_matrix, f: ndarray):
-    """
-    Notes
-    -----
-    If the load vector 'f' is dense, it must contain values for all
-    nodes, even the passive ones.
-    """
-    # data for boxing and unboxing
-    loc_to_glob, glob_to_loc = index_mappers(K_coo, return_inverse=True)
-    # boxing
-    K = box_spmatrix(K_coo, glob_to_loc) + box_spmatrix(Kp_coo, glob_to_loc)
-    f = box_rhs(matrixform(f), loc_to_glob)
-    return K, f, loc_to_glob
-
-
-def box_fem_data_bulk(Kp_coo: coo_matrix, gnum: ndarray, f: ndarray):
-    """
-    Notes
-    -----
-    If the load vector 'f' is dense, it must contain values for all
-    nodes, even the passive ones.
-    """
-    # data for boxing and unboxing
-    N = f.shape[0]
-    loc_to_glob, glob_to_loc = index_mappers(gnum, N=N, return_inverse=True)
-    # boxing
-    gnum = box_dof_numbering(gnum, glob_to_loc)
-    Kp_coo = box_spmatrix(Kp_coo, glob_to_loc)
-    f = box_rhs(matrixform(f), loc_to_glob)
-    return Kp_coo, gnum, f, loc_to_glob
+# -*- coding: utf-8 -*-
+from numba import njit, prange
+import numpy as np
+from numpy import ndarray
+
+from neumann.linalg.sparse.csr import csr_matrix as csr
+from neumann.array import find1d, flatten2dC
+
+__cache = True
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def fixity2d_to_dofs1d(fixity2d: np.ndarray, inds: np.ndarray = None):
+    """
+    Returns the indices of the degrees of freedoms
+    being supressed. 
+
+    Optionally, global indices of the rows in 'fixity2d' 
+    array can be provided by the optional argument 'inds'.
+
+    Parameters
+    ----------
+    fixity2d : np.ndarray(bool)[:, :]
+        2d numpy array of booleans. It has as many rows as nodes, and as 
+        many columns as derees of freedom per node in the model. A True
+        value means that the corresponding dof is fully supressed.
+
+    inds : np.ndarray, optional
+        1d numpy array of integers, default is None. If provided, it should
+        list the global indices of the nodes, for which the data is provided
+        by the array 'fixity2d'.
+
+    Returns
+    -------
+    dofinds : np.ndarray
+        1d numpy array of integers. 
+
+    """
+    ndof = fixity2d.shape[1]
+    args = np.argwhere(fixity2d == True)
+    N = args.shape[0]
+    res = np.zeros(N, dtype=args.dtype)
+    for i in prange(N):
+        res[i] = args[i, 0]*ndof + args[i, 1]
+    if inds is None:
+        return res
+    else:
+        dofinds = np.zeros_like(res)
+        for i in prange(len(inds)):
+            for j in prange(ndof):
+                dofinds[i*ndof + j] = inds[i]*ndof + j
+        return dofinds[res]
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def nodes2d_to_dofs1d(inds: np.ndarray, values: np.ndarray):
+    """
+    Returns a tuple of degree of freedom indices and data, 
+    based on a nodal definition.
+
+    Parameters
+    ----------
+    inds : np.ndarray
+        1d numpy array of integers, listing global node indices.
+
+    values : int of shape (nN, nDOF, nRHS)
+        3d numpy array of floats, listing values for each node
+        in 'inds'.
+
+    Returns
+    -------
+    dofinds : np.ndarray
+        1d numpy array of integers, denoting global dof indices.
+
+    dofvals : np.ndarray of shape (nN * nDOF, nRHS)
+        2d numpy array of floats, denoting values on dofs in 'dofinds'.
+
+    """
+    nN, dof_per_node, nRHS = values.shape
+    dofinds = np.zeros((nN * dof_per_node), dtype=inds.dtype)
+    dofvals = np.zeros((nN * dof_per_node, nRHS), dtype=values.dtype)
+    for node in prange(nN):
+        for dof in prange(dof_per_node):
+            i = node * dof_per_node + dof
+            dofinds[i] = inds[node] * dof_per_node + dof
+            for rhs in prange(nRHS):
+                dofvals[i, rhs] = values[node, dof, rhs]
+    return dofinds, dofvals
+
+
+@njit(nogil=True, cache=__cache, parallel=True)
+def weighted_stiffness_bulk(K: np.ndarray, weights: np.ndarray):
+    """
+    Returns a weighted stiffness matrix.
+
+    Parameters
+    ----------
+    K : np.ndarray
+        2d numpy array of floats
+
+    weights : np.ndarray
+        1d numpy array of floats
+
+    Returns
+    -------
+    Kw : np.ndarray
+        2d numpy array of floats
+
+    Notes
+    -----
+    (1) It is assumed that the first axis of K runs
+        along the elements.
+
+    """
+    nE = len(weights)
+    res = np.zeros_like(K)
+    for i in prange(nE):
+        res[i, :] = weights[i] * K[i]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def irows_icols_bulk(edofs: np.ndarray):
+    """
+    Returns row and column index data for several finite elements.
+
+    Parameters
+    ----------
+    edofs : np.ndarray
+        2d numpy array. Each row has the meaning of global degree of 
+        freedom numbering for a given finite element.
+
+    Returns
+    -------
+    irows, icols : np.ndarray, np.ndarray
+        Global indices of the rows and columns of the stiffness matrices
+        of the elements.
+
+    Notes
+    -----
+    The implementation assumes that every cell has the same number of
+    degrees of freedom.
+
+    """
+    nE, nNE = edofs.shape
+    nTOTV = nNE * nNE
+    irows = np.zeros((nE, nTOTV), dtype=edofs.dtype)
+    icols = np.zeros((nE, nTOTV), dtype=edofs.dtype)
+    for iNE in prange(nNE):
+        for jNE in prange(nNE):
+            i = iNE * nNE + jNE
+            for iE in prange(nE):
+                irows[iE, i] = edofs[iE, iNE]
+                icols[iE, i] = edofs[iE, jNE]
+    return irows, icols
+
+
+@njit(nogil=True, cache=__cache, parallel=True)
+def irows_icols_bulk_filtered(edofs: np.ndarray, inds: np.ndarray):
+    """
+    Returns row and column index data for finite elements specified
+    by the index array `inds`.
+
+    Parameters
+    ----------
+    edofs : np.ndarray
+        2d numpy array. Each row has the meaning of global degree of 
+        freedom numbering for a given finite element.
+
+    inds: np.ndarray
+        1d numpy array of integers specifying active elements in an assembly.
+
+    Returns
+    -------
+    irows, icols : np.ndarray, np.ndarray
+        Global indices of the rows and columns of the stiffness matrices
+        of the elements.
+
+    Notes
+    -----
+    The implementation assumes that every cell has the same number of
+    degrees of freedom.
+
+    """
+    nI = len(inds)
+    nNE = edofs.shape[1]
+    nTOTV = nNE * nNE
+    irows = np.zeros((nI, nTOTV), dtype=edofs.dtype)
+    icols = np.zeros((nI, nTOTV), dtype=edofs.dtype)
+    for iNE in prange(nNE):
+        for jNE in prange(nNE):
+            i = iNE * nNE + jNE
+            for iI in prange(nI):
+                irows[iI, i] = edofs[inds[iI], iNE]
+                icols[iI, i] = edofs[inds[iI], jNE]
+    return irows, icols
+
+
+@njit(nogil=True, cache=__cache, parallel=True)
+def topo_to_gnum(topo: np.ndarray, ndofn: int):
+    """
+    Returns global dof numbering based on element 
+    topology data.
+
+    Parameters
+    ----------
+    topo : np.ndarray
+        2d numpy array of integers. Topology array listing global
+        node numbers for several elements.
+
+    ndofn : int
+        Number of degrees of freedoms per node.
+
+    Returns
+    -------
+    gnum : np.ndarray
+        2d numpy array of integers.
+
+    """
+    nE, nNE = topo.shape
+    gnum = np.zeros((nE, nNE*ndofn), dtype=topo.dtype)
+    for i in prange(nE):
+        for j in prange(nNE):
+            for k in prange(ndofn):
+                gnum[i, j*ndofn + k] = topo[i, j]*ndofn + k
+    return gnum
+
+
+@njit(nogil=True, cache=__cache, parallel=True)
+def topo_to_gnum_jagged(topo, gnum, ndofn: int):
+    """
+    Returns global dof numbering based on element 
+    topology data.
+
+    Parameters
+    ----------
+    topo : np.ndarray
+        2d array of integers. Topology array listing global
+        node numbers for several elements.
+        
+    gnum : np.ndarray
+        2d buffer array for the results.
+
+    ndofn : int
+        Number of degrees of freedoms per node.
+
+    Returns
+    -------
+    gnum : np.ndarray
+        2d numpy array of integers.
+
+    """
+    nE, _ = topo.shape
+    for i in prange(nE):
+        for j in prange(len(topo[i])):
+            for k in prange(ndofn):
+                gnum[i, j*ndofn + k] = topo[i, j]*ndofn + k
+    return gnum
+
+
+@njit(nogil=True, parallel=True, fastmath=True, cache=__cache)
+def assemble_load_vector(values: ndarray, gnum: ndarray, N: int = -1):
+    """
+    Returns global dof numbering based on element 
+    topology data.
+
+    Parameters
+    ----------
+    values : np.ndarray of shape (nE, nEVAB, nRHS)
+        3d numpy array of floats, representing element data.
+        The length of the second axis matches the the number of
+        degrees of freedom per cell.
+
+    gnum : int
+        Global indices of local degrees of freedoms of elements.
+
+    N : int, Optional.
+        The number of total unknowns in the system. Must be specified correcly,
+        to get a vector the same size of the global system. If not specified, it is
+        inherited from 'gnum' (as 'gnum.max() + 1'), but this can lead to a chopped 
+        array.
+
+    Returns
+    -------
+    np.ndarray
+        2d numpy array of integers with a shape of (N, nRHS), where nRHS is the number
+        if right hand sizes (load cases).
+
+    """
+    nE, nEVAB, nRHS = values.shape 
+    if N < 0:
+        N = gnum.max() + 1
+    res = np.zeros((N, nRHS), dtype=values.dtype)
+    for i in range(nE):
+        for j in range(nEVAB):
+            for k in prange(nRHS):
+                res[gnum[i, j], k] += values[i, j, k]
+    return res
+
+
+@njit(nogil=True, parallel=False, fastmath=True, cache=__cache)
+def penalty_factor_matrix(cellfixity: ndarray, shp: ndarray):
+    nE, nNE, nDOF = cellfixity.shape
+    N = nDOF * nNE
+    res = np.zeros((nE, N, N), dtype=shp.dtype)
+    for iE in prange(nE):
+        for iNE in prange(nNE):
+            for iDOF in prange(nDOF):
+                fix = cellfixity[iE, iNE, iDOF]
+                for jNE in prange(nNE):
+                    i = jNE * nDOF + iDOF
+                    for kNE in prange(nNE):
+                        j = kNE * nDOF + iDOF
+                        res[iE, i, j] += fix * shp[iNE, jNE] * shp[iNE, kNE]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def approximation_matrix(ndf: ndarray, NDOFN: int):
+    """Returns a matrix of approximation coefficients 
+    for all elements."""
+    nE, nNE = ndf.shape[:2]
+    N = nNE * NDOFN
+    nappr = np.eye(N, dtype=ndf.dtype)
+    res = np.zeros((nE, N, N), dtype=ndf.dtype)
+    for iE in prange(nE):
+        for i in prange(nNE):
+            for j in prange(nNE):
+                for ii in prange(NDOFN):
+                    for jj in prange(NDOFN):
+                        res[iE, i*2 + ii, j*2 + jj] = nappr[i, j] * ndf[iE, i]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def nodal_approximation_matrix(ndf: ndarray):
+    """Returns a matrix of nodal approximation coefficients 
+    for all elements."""
+    nE, nNE = ndf.shape[:2]
+    nappr = np.eye(nNE, dtype=ndf.dtype)
+    res = np.zeros((nE, nNE, nNE), dtype=ndf.dtype)
+    for iE in prange(nE):
+        for i in prange(nNE):
+            for j in prange(nNE):
+                res[iE, i, j] = nappr[i, j] * ndf[iE, i]
+    return res
+
+
+@njit(nogil=True, cache=__cache)
+def nodal_compatibility_factors(nam_csr_tot: csr, nam: ndarray, topo: ndarray):
+    indptr = nam_csr_tot.indptr
+    indices = nam_csr_tot.indices
+    data = nam_csr_tot.data
+    nN = len(indptr)-1
+    widths = np.zeros(nN, dtype=indptr.dtype)
+    for iN in range(nN):
+        widths[iN] = indptr[iN+1] - indptr[iN]
+    factors = dict()
+    nreg = dict()
+    for iN in range(nN):
+        factors[iN] = np.zeros((widths[iN], widths[iN]), dtype=nam.dtype)
+        nreg[iN] = indices[indptr[iN]: indptr[iN+1]]
+    nE, nNE = topo.shape
+    for iE in range(nE):
+        topoE = topo[iE]
+        for jNE in range(nNE):
+            nID = topo[iE, jNE]
+            dataN = data[indptr[nID]: indptr[nID+1]]
+            topoN = nreg[nID]
+            dataNE = np.zeros(widths[nID], dtype=nam.dtype)
+            imap = find1d(topoE, topoN)
+            dataNE[imap] = nam[iE, jNE]
+            rNE = dataN - dataNE  # residual
+            factors[nID] += np.outer(rNE, rNE)
+    return factors, nreg
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def compatibility_factors_to_coo(ncf: dict, nreg: dict):
+    """
+    ncf : nodal_compatibility_factors
+    """
+    nN = len(ncf)
+    widths = np.zeros(nN, dtype=np.int32)
+    for iN in prange(nN):
+        widths[iN] = len(nreg[iN])
+    shapes = (widths**2).astype(np.int64)
+    N = np.sum(shapes)
+    data = np.zeros(N, dtype=np.float64)
+    rows = np.zeros(N, dtype=np.int32)
+    cols = np.zeros(N, dtype=np.int32)
+    c = 0
+    for iN in range(nN):
+        data[c: c + shapes[iN]] = flatten2dC(ncf[iN])
+        nNN = widths[iN]
+        for jNN in prange(nNN):
+            for kNN in prange(nNN):
+                rows[c + jNN*nNN + kNN] = nreg[iN][jNN]
+                cols[c + jNN*nNN + kNN] = nreg[iN][kNN]
+        c += shapes[iN]
+    return data, rows, cols
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def topo1d_to_gnum1d(topo1d: ndarray, NDOFN: int):
+    nN = topo1d.shape[0]
+    gnum1d = np.zeros(nN * NDOFN, dtype=topo1d.dtype)
+    for i in prange(nN):
+        for j in prange(NDOFN):
+            gnum1d[i*NDOFN + j] = topo1d[i] * NDOFN + j
+    return gnum1d
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def ncf_to_cf(ncf: ndarray, NDOFN: int):
+    nN = ncf.shape[0]
+    cf = np.zeros((nN * NDOFN, nN * NDOFN), dtype=ncf.dtype)
+    for i in prange(nN):
+        for ii in prange(NDOFN):
+            for j in prange(nN):
+                cf[i*NDOFN + ii, j*NDOFN + ii] = ncf[i, j]
+    return cf
+
+
+@njit(nogil=True, cache=__cache)
+def compatibility_factors(ncf: dict, nreg: dict, NDOFN: int):
+    """ncf : nodal_compatibility_factors"""
+    nN = len(ncf)
+    widths = np.zeros(nN, dtype=np.int32)
+    for iN in prange(nN):
+        widths[iN] = len(nreg[iN])
+    cf = dict()
+    reg = dict()
+    for iN in range(nN):
+        cf[iN] = ncf_to_cf(ncf[iN], NDOFN)
+        reg[iN] = topo1d_to_gnum1d(nreg[iN], NDOFN)
+    return cf, reg
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def tr_cells_1d_in(A: ndarray, Q: ndarray):
+    """
+    Transforms element vectors (like the load vector) from global to local.
+    
+    Parameters
+    ----------
+    A : 3d NumPy float array of shape (nE, nEVAB)
+        Array of coefficients to transform.
+        
+    Q : 3d NumPy float array of shape (nE, nEVAB, nEVAB)
+        Transformation matrices.
+        
+    Returns
+    -------
+    numpy array
+        NumPy array with the same shape as 'A'
+    """
+    res = np.zeros_like(A)
+    for iE in prange(res.shape[0]):
+        res[iE] = Q[iE] @ A[iE]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def tr_cells_1d_out(A: ndarray, Q: ndarray):
+    """
+    Transforms element vectors (like the load vector) from local to global.
+    (nE, nNE * nDOF)
+    """
+    res = np.zeros_like(A)
+    for iE in prange(res.shape[0]):
+        res[iE] = Q[iE].T @ A[iE]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def tr_cells_1d_in_multi(A: ndarray, Q: ndarray):
+    """
+    Transforms element vectors (like the load vector) from local to global
+    for multiple cases.
+    (nE, nRHS, nNE * nDOF)
+    """
+    res = np.zeros_like(A)
+    for iE in prange(res.shape[0]):
+        for jRHS in prange(res.shape[1]):
+            res[iE, jRHS] = Q[iE] @ A[iE, jRHS]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def tr_cells_1d_out_multi(A: ndarray, Q: ndarray):
+    """
+    Transforms element vectors (like the load vector) from local to global
+    for multiple cases.
+    A (nE, nRHS, nP * nDOF)
+    Q (nE, nP * nDOF)
+    """
+    res = np.zeros_like(A)
+    for iE in prange(res.shape[0]):
+        for jRHS in prange(res.shape[1]):
+            res[iE, jRHS] = Q[iE].T @ A[iE, jRHS]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def element_dof_solution_bulk(dofsol1d: ndarray, gnum: ndarray):
+    """
+    dofsol (nN * nDOF, nRHS)
+    gnum (nE, nEVAB)
+    ---
+    (nE, nEVAB, nRHS)
+    """
+    nRHS = dofsol1d.shape[1]
+    nE, nEVAB = gnum.shape
+    res = np.zeros((nE, nEVAB, nRHS), dtype=dofsol1d.dtype)
+    for i in prange(nE):
+        for j in prange(nRHS):
+            res[i, :, j] = dofsol1d[gnum[i, :], j]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def transform_stiffness(K: ndarray, dcm: ndarray):
+    """
+    Transforms element stiffness matrices from local to global.
+    """
+    res = np.zeros_like(K)
+    for iE in prange(res.shape[0]):
+        res[iE] = dcm[iE].T @ K[iE] @ dcm[iE]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def element_dofmap_bulk(dofmap: ndarray, nDOF: int, nNODE: int):
+    nDOF_ = dofmap.shape[0]
+    res = np.zeros(nNODE * nDOF_, dtype=dofmap.dtype)
+    for i in prange(nNODE):
+        for j in prange(nDOF_):
+            res[i*nDOF_ + j] = i*nDOF + dofmap[j]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def expand_stiffness_bulk(K_in: ndarray, K_out: ndarray, dofmap: ndarray):
+    """
+    Expands the local stiffness matrix into a standard form.
+    """
+    nDOF = dofmap.shape[0]    
+    for i in prange(nDOF):
+        for j in prange(nDOF):
+            K_out[:, dofmap[i], dofmap[j]] = K_in[:, i, j]
+    return K_out
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def pull_submatrix(A, r, c):
+    nR = r.shape[0]
+    nC = c.shape[0]
+    res = np.zeros((nR, nC), dtype=A.dtype)
+    for i in prange(nR):
+        for j in prange(nC):
+            res[i, j] = A[r[i], c[j]]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def push_submatrix(A, Asub, r, c, new=True):
+    nR = r.shape[0]
+    nC = c.shape[0]
+    res = np.zeros_like(A)
+    if not new:
+        res[:, :] = A
+    for i in prange(nR):
+        for j in prange(nC):
+            res[r[i], c[j]] = Asub[i, j]
+    return res
+    
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def constrain_local_stiffness_bulk(K: ndarray, factors: ndarray):
+    """
+    Returns the condensed stiffness matrices representing constraints
+    on the internal forces of the elements (eg. hinges).
+        
+    Currently this solution is only able to handle two states, being totally free 
+    and being fully constrained. The factors are expected to be numbers between
+    0 and 1, where dofs with a factor > 0.5 are assumed to be the constrained ones.
+    
+    Note
+    ----
+    numba-jitted in nopython mode
+    
+    Parameters
+    ----------
+    K : numpy.ndarray
+        3d float array, the stiffness matrices of several elements of the same kind.
+        
+    factors: numpy.ndarray
+        2d float array of connectivity facotors for each dof of every element.
+                    
+    Note
+    ----
+    This solution applies the idea of static condensation.
+    
+    Returns
+    -------
+    numpy.ndarray
+        The constrained stiffness matrices with the same shape as `K`.
+        
+    """
+    nE, _, _ = K.shape
+    res = np.zeros_like(K)
+    for iE in prange(nE):
+        b = np.where(factors[iE] > 0.5)[0]
+        i = np.where(factors[iE] <= 0.5)[0]
+        Kbb = pull_submatrix(K[iE], b, b)
+        Kii = pull_submatrix(K[iE], i, i)
+        Kib = pull_submatrix(K[iE], i, b)
+        Kbi = pull_submatrix(K[iE], b, i)
+        Kbb -= Kbi @ np.linalg.inv(Kii) @ Kib
+        res[iE] = push_submatrix(K[iE], Kbb, b, b, True)
+    return res
+
+
+def assert_min_stiffness_bulk(K: ndarray, minval = 1e-12):
+    inds = np.arange(K.shape[-1])
+    d = K[:, inds, inds]
+    eid, vid = np.where(d < minval)
+    K[eid, vid, vid] = minval
+    return K
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def internal_forces(K: ndarray, dofsol: ndarray):
+    """
+    Transforms element stiffness matrices from local to global.
+    ---
+    (nE, nRHS, nEVAB)
+    """
+    nE, nRHS, nEVAB  = dofsol.shape
+    res = np.zeros_like(dofsol)
+    for i in prange(nE):
+        for j in prange(nRHS):
+            res[i, j] = K[i] @ dofsol[i, j]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def nodal_mass_matrix_data(nodal_masses: ndarray, ndof:int=6):
+    N = nodal_masses.shape[0]
+    res = np.zeros((N*ndof))
+    for i in prange(N):
+        res[i*ndof : i*ndof + 3] = nodal_masses[i]
+    return res
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/utils/fem/tr.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/tr.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,162 +1,174 @@
-import numpy as np
-from numpy import ndarray
-from numba import njit, prange
-
-from neumann import repeat_diagonal_2d, ascont
-
-__cache = True
-
-
-@njit(nogil=True, cache=__cache)
-def nodal_dcm(dcm: ndarray, N: int = 2) -> ndarray:
-    """
-    Assembles the nodal direction cosine matrix of a single node.
-
-    Parameters
-    ----------
-    dcm : numpy.ndarray
-        A 3x3 direction cosine matrix.
-    N : int, Optional
-        The number of triplets that make up a nodal vector.
-        Default is 2, which means 6 dofs per node.
-
-    Returns
-    -------
-    numpy.ndarray
-        A 2d numpy float array.
-
-    Note
-    ----
-    The template 'dcm' should be the matrix you would use to transform a
-    position vector in 3d Euclidean space.
-    """
-    return repeat_diagonal_2d(dcm, N)
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def nodal_dcm_bulk(dcm: ndarray, N: int = 2) -> ndarray:
-    """
-    Assembles the nodal direction cosine matrices of several cells.
-
-    Parameters
-    ----------
-    dcm : numpy.ndarray
-        A 3x3 direction cosine matrix for each element (4d).
-    N : int, Optional
-        The number of triplets that make up a nodal vector.
-        Default is 2, which means 6 dofs per node.
-
-    Returns
-    -------
-    numpy.ndarray
-        A 3d numpy float array.
-
-    Note
-    ----
-    Typically, 'dcm' should be the matrix you would use to transform a
-    position vector in 3d Euclidean space.
-    """
-    nE = dcm.shape[0]
-    res = np.zeros((nE, 3 * N, 3 * N), dtype=dcm.dtype)
-    for i in prange(N):
-        _i = i * 3
-        i_ = _i + 3
-        res[:, _i:i_, _i:i_] = dcm
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def element_dcm(nodal_dcm: ndarray, nNE: int = 2, nDOF: int = 6):
-    nEVAB = nNE * nDOF
-    res = np.zeros((nEVAB, nEVAB), dtype=nodal_dcm.dtype)
-    for iNE in prange(nNE):
-        i0, i1 = nDOF * iNE, nDOF * (iNE + 1)
-        res[i0:i1, i0:i1] = nodal_dcm
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def element_dcm_bulk(nodal_dcm: ndarray, nNE: int = 2, nDOF: int = 6):
-    nE = nodal_dcm.shape[0]
-    nEVAB = nNE * nDOF
-    res = np.zeros((nE, nEVAB, nEVAB), dtype=nodal_dcm.dtype)
-    for iNE in prange(nNE):
-        i0, i1 = nDOF * iNE, nDOF * (iNE + 1)
-        for iE in prange(nE):
-            res[iE, i0:i1, i0:i1] = nodal_dcm[iE]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def tr_element_vectors_bulk_multi(
-    values: ndarray, dcm: ndarray, invert: bool = False
-) -> ndarray:
-    """
-    Transforms element vectors for multiple cases.
-
-    Parameters
-    ----------
-    values : numpy.ndarray
-        The values to transform as an array of shape (nE, nRHS, nX).
-    dcm : numpy.ndarray
-        The direct cosine matrix of the transformation as an
-        array of shape (nE, nX).
-    invert : bool, Optional
-        If True, the DCM matrices are transposed before transformation.
-        This makes this function usable in both directions.
-        Default is False.
-
-    Returns
-    -------
-    numpy.ndarray
-        An array with the same shape as 'values'.
-    """
-    res = np.zeros_like(values)
-    if not invert:
-        for iE in prange(res.shape[0]):
-            for jRHS in prange(res.shape[1]):
-                res[iE, jRHS] = dcm[iE] @ values[iE, jRHS]
-    else:
-        for iE in prange(res.shape[0]):
-            for jRHS in prange(res.shape[1]):
-                res[iE, jRHS] = dcm[iE].T @ values[iE, jRHS]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def tr_element_matrices_bulk(K: ndarray, dcm: ndarray, invert: bool = False):
-    """
-    Transforms element stiffness matrices.
-    """
-    res = np.zeros_like(K)
-    if not invert:
-        for iE in prange(res.shape[0]):
-            res[iE] = dcm[iE] @ K[iE] @ dcm[iE].T
-    else:
-        for iE in prange(res.shape[0]):
-            res[iE] = dcm[iE].T @ K[iE] @ dcm[iE]
-    return res
-
-
-def tr_nodal_loads_bulk(nodal_loads: ndarray, dcm: ndarray) -> ndarray:
-    """
-    Transforms discrete nodal loads to the global frame.
-
-    Parameters
-    ----------
-    nodal_loads : numpy.ndarray
-        A 3d array of shape (nE, nEVAB, nRHS).
-
-    Returns
-    -------
-    numpy.ndarray
-        A numpy array of shape (nE, nEVAB, nRHS).
-
-    """
-    nodal_loads = np.swapaxes(nodal_loads, 1, 2)
-    # (nE, nNE * nDOF, nRHS) -> (nE, nRHS, nNE * nDOF)
-    nodal_loads = ascont(nodal_loads)
-    nodal_loads = tr_element_vectors_bulk_multi(nodal_loads, dcm)
-    nodal_loads = np.swapaxes(nodal_loads, 1, 2)
-    # (nE, nRHS, nNE * nDOF) -> (nE, nNE * nDOF, nRHS)
-    return nodal_loads
+import numpy as np
+from numpy import ndarray
+from numba import njit, prange
+__cache = True
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def nodal_dcm(dcm: ndarray, N=2) -> ndarray:
+    """
+    Returns a direction cosine matrix for a node, 
+    if the number of nodal degrees of freedom is a
+    multiple of 3. 
+    
+    Parameters
+    ----------
+    dcm : numpy.ndarray
+        A 3x3 direction cosine matrix for many elements.
+    
+    N : int, Optional
+        The number of triplets that make up a nodal vector.
+        Default is 2, which means 6 dofs per node.
+        
+    Returns
+    -------
+    numpy.ndarray
+        A 3d numpy float array.
+                 
+    """
+    nE = dcm.shape[0]
+    res = np.zeros((nE, 3 * N, 3 * N), dtype=dcm.dtype)
+    for i in prange(N):
+        _i = i * 3
+        i_ = _i + 3
+        res[:, _i:i_, _i:i_] = dcm
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def element_dcm(nodal_dcm: ndarray, nNE: int = 2, nDOF: int=6):
+    nE = nodal_dcm.shape[0]
+    nEVAB = nNE * nDOF
+    res = np.zeros((nE, nEVAB, nEVAB), dtype=nodal_dcm.dtype)
+    for iNE in prange(nNE):
+        i0, i1 = nDOF*iNE, nDOF * (iNE+1)
+        for iE in prange(nE):
+            res[iE, i0: i1, i0: i1] = nodal_dcm[iE]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def element_transformation_matrices(Q: ndarray, nNE: int=2):
+    nE = Q.shape[0]
+    nEVAB = nNE * 6
+    res = np.zeros((nE, nEVAB, nEVAB), dtype=Q.dtype)
+    for iE in prange(nE):
+        for j in prange(2*nNE):
+            res[iE, 3*j : 3*(j+1), 3*j : 3*(j+1)] = Q[iE]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def nodal_transformation_matrices(Q: ndarray):
+    nE = Q.shape[0]
+    res = np.zeros((nE, 6, 6), dtype=Q.dtype)
+    for iE in prange(nE):
+        for j in prange(2):
+            res[iE, 3*j : 3*(j+1), 3*j : 3*(j+1)] = Q[iE]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def transform_element_matrices_out(A: ndarray, Q: ndarray):
+    res = np.zeros_like(A)
+    for iE in prange(res.shape[0]):
+        res[iE] = Q[iE].T @ A[iE] @ Q[iE]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def transform_element_vectors_out(A: ndarray, Q: ndarray):
+    """
+    Transforms element load vectors from local to global.
+    """
+    res = np.zeros_like(A)
+    for iE in prange(res.shape[0]):
+        res[iE] = Q[iE].T @ A[iE]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def transform_element_vectors_out_multi(A: ndarray, Q: ndarray):
+    """
+    Transforms multiple element load vectors from 
+    local to global.
+    """
+    nE, nP = A.shape[:2]
+    res = np.zeros_like(A)
+    for iE in prange(nE):
+        for iP in prange(nP):
+            res[iE, iP] = Q[iE].T @ A[iE, iP]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def transform_element_vectors_in(dofsol: ndarray, Q: ndarray):
+    """
+    Transforms element dof solutions from global to local.
+    """
+    res = np.zeros_like(dofsol)
+    for i in prange(res.shape[0]):
+        res[i] = Q[i] @ dofsol[i]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def transform_numint_forces_out(data: ndarray, dcm_G_L: ndarray):
+    """
+    Transforms internal forces of several elements
+    and evaluation points from local frames
+    to one global frame.
+    
+    Parameters
+    ----------
+    data: (nE, nP, nRHS, nDOFN) numpy.ndarray
+        nE : number of elements
+        nP : number of sampling points
+        nRHS : number of datasets (eg. load cases)
+        nDOFN : number of dofs of a node
+        
+    dcm_G_L : (nE, 3, 3) numpy array
+        Array of DCM matrices from global to local.
+    
+    Returns
+    -------
+    (nE, nP, nRHS, nDOFN) numpy.ndarray
+    """
+    nE, nP, nC = data.shape[:3]
+    res = np.zeros_like(data)
+    for iE in prange(nE):
+        for iP in prange(nP):
+            for iC in prange(nC):
+                res[iE, iP, iC, :] = dcm_G_L[iE].T @ data[iE, iP, iC, :]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def transform_numint_forces_in(data: ndarray, dcm_G_L: ndarray):
+    """
+    Transforms internal forces of several elements
+    and numerical integration points form one global frame
+    to several local frames.
+    
+    Parameters
+    ----------
+    data: (nE, nP, nRHS, nDOF) numpy.ndarray
+        nE : number of elements
+        nP : number of sampling points
+        nRHS : number of datasets (eg. load cases)
+        nDOFN : number of dofs of a node
+        
+    dcm_G_L : (nE, 3, 3) numpy array
+        Array of DCM matrices from global to local.
+    
+    Returns
+    -------
+    (nE, nP, nRHS, nDOFN) numpy.ndarray   
+    """
+    nE, nP, nC = data.shape[:3]
+    res = np.zeros_like(data)
+    for i in prange(nE):
+        for j in prange(nP):
+            for k in prange(nC):
+                res[i, j, k, :] = dcm_G_L[i] @ data[i, j, k, :]
+    return res
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/utils/material/hmh.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/material/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,85 +1,66 @@
-import numpy as np
-from numpy import ndarray
-from numba import njit, vectorize, prange
-
-__cache = True
-
-
-@njit(nogil=True, cache=__cache)
-def HMH_M(strs: ndarray):
-    """
-    Evaluates the Huber-Mises-Hencky formula for membranes.
-
-    Parameters
-    ----------
-    strs : numpy.ndarray
-        The stresses s11, s22, s12.
-    """
-    s11, s22, s12 = strs
-    return np.sqrt(s11**2 - s11 * s22 + s22**2 + 3 * s12**2)
-
-
-@njit(nogil=True, cache=__cache)
-def HMH_S(strs: ndarray):
-    """
-    Evaluates the Huber-Mises-Hencky formula for shells.
-
-    Parameters
-    ----------
-    strs : numpy.ndarray
-        The stresses s11, s22, s12, s13, s23.
-    """
-    s11, s22, s12, s13, s23 = strs
-    return np.sqrt(
-        s11**2 - s11 * s22 + s22**2 + 3 * s12**2 + 3 * s13**2 + 3 * s23**2
-    )
-
-
-@njit(nogil=True, cache=__cache)
-def HMH_3d(strs: ndarray):
-    """
-    Evaluates the Huber-Mises-Hencky formula for 3d solids.
-
-    Parameters
-    ----------
-    strs : numpy.ndarray
-        The stresses s11, s22, s33, s23, s13, s12.
-    """
-    s11, s22, s33, s23, s13, s12 = strs
-    return np.sqrt(
-        0.5 * ((s11 - s22) ** 2 + (s22 - s33) ** 2 + (s33 - s11) ** 2)
-        + 3 * (s12**2 + s13**2 + s23**2)
-    )
-
-
-@njit(nogil=True, cache=__cache)
-def HMH_3d_multi(strs: ndarray):
-    """
-    Evaluates the Huber-Mises-Hencky formula for 3d solids for
-    multiple points.
-
-    Parameters
-    ----------
-    strs : numpy.ndarray
-        2d array of stresses for several points. The stresses are
-        expected in the order s11, s22, s33, s23, s13, s12.
-    """
-    nP = strs.shape[0]
-    res = np.zeros(nP, dtype=strs.dtype)
-    for i in prange(nP):
-        res[i] = HMH_3d(strs[i])
-    return res
-
-
-@vectorize("f8(f8, f8, f8, f8, f8, f8)", target="parallel", cache=__cache)
-def HMH_3d_v(s11, s22, s33, s23, s13, s12):
-    """
-    Vectorized evaluation of the HMH failure criterion.
-
-    The input values s11, s22, s33, s23, s13, s12 can be
-    arbitrary dimensional arrays.
-    """
-    return np.sqrt(
-        0.5 * ((s11 - s22) ** 2 + (s22 - s33) ** 2 + (s33 - s11) ** 2)
-        + 3 * (s12**2 + s13**2 + s23**2)
-    )
+# -*- coding: utf-8 -*-
+import numpy as np
+from numpy import ndarray
+from numba import njit, vectorize
+
+__cache = True
+
+
+@njit(nogil=True, cache=__cache)
+def HMH_M(strs: ndarray):
+    """
+    Evaluates the Huber-Mises-Hencky formula for membranes.
+
+    Parameters
+    ----------
+    strs : numpy.ndarray
+        The stresses s11, s22, s12
+
+    """
+    s11, s22, s12 = strs
+    return np.sqrt(s11**2 - s11*s22 + s22**2 + 3*s12**2)
+
+
+@njit(nogil=True, cache=__cache)
+def HMH_S(strs: ndarray):
+    """
+    Evaluates the Huber-Mises-Hencky formula for shells.
+
+    Parameters
+    ----------
+    strs : numpy.ndarray
+        The stresses s11, s22, s12, s13, s23
+
+    """
+    s11, s22, s12, s13, s23 = strs
+    return np.sqrt(s11**2 - s11*s22 + s22**2 +
+                   3*s12**2 + 3*s13**2 + 3*s23**2)
+
+
+@njit(nogil=True, cache=__cache)
+def HMH_3d(strs: ndarray):
+    """
+    Evaluates the Huber-Mises-Hencky formula for 3d solids.
+
+    Parameters
+    ----------
+    strs : numpy.ndarray
+        The stresses s11, s22, s33, s12, s13, s23
+
+    """
+    s11, s22, s33, s12, s13, s23 = strs
+    return np.sqrt(0.5*((s11-s22)**2 + (s22-s33)**2 + (s33-s11)**2) +
+                   3*(s12**2 + s13**2 + s23**2))
+
+
+@vectorize("f8(f8, f8, f8, f8, f8, f8)", target='parallel', cache=__cache)
+def HMH_3d_v(s11, s22, s33, s12, s13, s23):
+    """
+    Vectorized evaluation of the HMH failure criterion.
+
+    The input values s11, s22, s33, s12, s13, s23 can be
+    arbitrary dimensional arrays. 
+
+    """
+    return np.sqrt(0.5*((s11-s22)**2 + (s22-s33)**2 + (s33-s11)**2) +
+                   3*(s12**2 + s13**2 + s23**2))
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/utils/material/material.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/fem/model/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from numba import njit, prange
-import numpy as np
-from numpy import ndarray
-
-
-from ..fem.cells import element_dof_solution_bulk, element_dof_solution_bulk_multi
-
-__cache = True
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def model_strains(dofsol1d: ndarray, gnum: ndarray, B: ndarray):
-    nE, nP, NSTRE = B.shape[:3]
-    esol = element_dof_solution_bulk(dofsol1d, gnum)
-    res = np.zeros((nE, nP, NSTRE), dtype=dofsol1d.dtype)
-    for iE in prange(nE):
-        for iP in prange(nP):
-            res[iE, iP, :] = B[iE, iP] @ esol[iE]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def model_strains_multi(data: ndarray, gnum: ndarray, B: ndarray):
-    nE, nP, NSTRE = B.shape[:3]
-    esol = element_dof_solution_bulk_multi(data, gnum)
-    nRHS = esol.shape[0]
-    res = np.zeros((nRHS, nE, nP, NSTRE), dtype=data.dtype)
-    for iE in prange(nE):
-        for iP in prange(nP):
-            for j in prange(nRHS):
-                res[j, iE, iP, :] = B[iE, iP] @ esol[j, iE]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def stresses_from_strains(C: ndarray, strains: ndarray):
-    nE, nP, _ = strains.shape
-    res = np.zeros_like(strains)
-    for iE in prange(nE):
-        for iP in prange(nP):
-            res[iE, iP, :] = C[iE] @ strains[iE, iP]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def stresses_from_strains_multi(C: ndarray, strains: ndarray):
-    nR, nE, nP, _ = strains.shape
-    res = np.zeros_like(strains)
-    for iR in prange(nR):
-        for iE in prange(nE):
-            for iP in prange(nP):
-                res[iR, iE, iP, :] = C[iE] @ strains[iR, iE, iP]
-    return res
+# -*- coding: utf-8 -*-
+from numba import njit, prange
+import numpy as np
+from numpy import ndarray
+
+from ..cells.utils import element_dof_solution_bulk, element_dof_solution_bulk_multi
+
+__cache = True
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def model_strains(dofsol1d: ndarray, gnum: ndarray, B: ndarray):
+    nE, nP, NSTRE = B.shape[:3]
+    esol = element_dof_solution_bulk(dofsol1d, gnum)
+    res = np.zeros((nE, nP, NSTRE), dtype=dofsol1d.dtype)
+    for iE in prange(nE):
+        for iP in prange(nP):
+            res[iE, iP, :] = B[iE, iP] @ esol[iE]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def model_strains_multi(data: ndarray, gnum: ndarray, B: ndarray):
+    nE, nP, NSTRE = B.shape[:3]
+    esol = element_dof_solution_bulk_multi(data, gnum)
+    nRHS = esol.shape[0]
+    res = np.zeros((nRHS, nE, nP, NSTRE), dtype=data.dtype)
+    for iE in prange(nE):
+        for iP in prange(nP):
+            for j in prange(nRHS):
+                res[j, iE, iP, :] = B[iE, iP] @ esol[j, iE]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def stresses_from_strains(C: ndarray, strains: ndarray):
+    nE, nP, _ = strains.shape
+    res = np.zeros_like(strains)
+    for iE in prange(nE):
+        for iP in prange(nP):
+            res[iE, iP, :] = C[iE] @ strains[iE, iP]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def stresses_from_strains_multi(C: ndarray, strains: ndarray):
+    nR, nE, nP, _ = strains.shape
+    res = np.zeros_like(strains)
+    for iR in prange(nR):
+        for iE in prange(nE):
+            for iP in prange(nP):
+                res[iR, iE, iP, :] = C[iE] @ strains[iR, iE, iP]
+    return res
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon/utils/material/surface.py` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon/solid/model/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,134 +1,131 @@
-import numpy as np
-from numpy import ndarray
-from numpy.linalg import inv
-from numba import njit, prange
-
-from neumann.linalg import linspace1d
-from neumann import clip1d
-
-__cache = True
-
-
-@njit(nogil=True, cache=__cache)
-def layers_of_points(points: np.ndarray, bounds: np.ndarray):
-    nL = bounds.shape[0]
-    bins = np.zeros((nL + 1,), dtype=points.dtype)
-    bins[0] = bounds[0, 0]
-    bins[1:] = bounds[:, 1]
-    return clip1d(np.digitize(points[:, 2], bins) - 1, 0, nL - 1)
-
-
-@njit(
-    ["f8[:, :](f8[:, :], i8)", "f4[:, :](f4[:, :], i8)"],
-    nogil=True,
-    parallel=True,
-    cache=__cache,
-)
-def points_of_layers(bounds: np.ndarray, nppl=3):
-    nL = bounds.shape[0]
-    res = np.zeros((nL, nppl), dtype=bounds.dtype)
-    for iL in prange(nL):
-        res[iL] = linspace1d(bounds[iL, 0], bounds[iL, 1], nppl)
-    return res
-
-
-@njit(nogil=True, cache=__cache)
-def glob_to_loc_layer(point: np.ndarray, bounds: np.ndarray):
-    return (point[2] - bounds[0]) / (bounds[1] - bounds[0])
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def iso_mindlin_plate_bulk(C: ndarray, t: ndarray, k: float = 5 / 6):
-    res = np.zeros((C.shape[0], 5, 5))
-    for i in prange(res.shape[0]):
-        res[i, :3, :3] = C[i, :3, :3] * (t[i] ** 3 / 12)
-        res[i, 3:, 3:] = C[i, 3:, 3:] * t[i]
-    res[:, 3:, 3:] *= k
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def iso_membrane_bulk(C: ndarray, t: ndarray):
-    res = np.zeros((C.shape[0], 3, 3))
-    for i in prange(res.shape[0]):
-        res[i, :, :] = C[i, :, :] * t[i]
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def iso_mindlin_shell_bulk(C: ndarray, t: ndarray, k: float = 5 / 6):
-    res = np.zeros((C.shape[0], 8, 8))
-    res[:, :3, :3] = iso_membrane_bulk(C, t)
-    res[:, 3:, 3:] = iso_mindlin_plate_bulk(C, t, k)
-    return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def rotation_matrices_126(angles: np.ndarray):
-    """
-    Returns transformation matrmatrixices T_126 for each angle.
-    Angles are expected in radians.
-    """
-    nL = len(angles)
-    T_126 = np.zeros((nL, 3, 3), dtype=angles.dtype)
-    for iL in prange(nL):
-        a = angles[iL] * np.pi / 180
-        T_126[iL, 0, 0] = np.cos(a) ** 2
-        T_126[iL, 0, 1] = np.sin(a) ** 2
-        T_126[iL, 0, 2] = -np.sin(2 * a)
-        T_126[iL, 1, 0] = T_126[iL, 0, 1]
-        T_126[iL, 1, 1] = T_126[iL, 0, 0]
-        T_126[iL, 1, 2] = -T_126[iL, 0, 2]
-        T_126[iL, 2, 0] = np.cos(a) * np.sin(a)
-        T_126[iL, 2, 1] = -T_126[iL, 2, 0]
-        T_126[iL, 2, 2] = np.cos(a) ** 2 - np.sin(a) ** 2
-    return T_126
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def rotation_matrices_45(angles: np.ndarray):
-    """
-    Returns transformation matrix T_45 for each angle.
-    Angles are expected in radians.
-    """
-    nL = len(angles)
-    T_45 = np.zeros((nL, 2, 2), dtype=angles.dtype)
-    for iL in prange(nL):
-        a = angles[iL] * np.pi / 180
-        T_45[iL, 0, 0] = np.cos(a)
-        T_45[iL, 0, 1] = -np.sin(a)
-        T_45[iL, 1, 1] = T_45[iL, 0, 0]
-        T_45[iL, 1, 0] = -T_45[iL, 0, 1]
-    return T_45
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def material_stiffness_matrices_126(C_126: np.ndarray, angles: np.ndarray):
-    """
-    Returns the components of the material stiffness matrix C_126
-    in the global system.
-    """
-    nL = len(C_126)
-    C_126_g = np.zeros_like(C_126)
-    R_126 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 2]], dtype=C_126_g.dtype)
-    R_126_inv = inv(R_126)
-    T_126 = rotation_matrices_126(angles)
-    for iL in prange(nL):
-        C_126_g[iL] = T_126[iL] @ C_126[iL] @ R_126_inv @ T_126[iL].T @ R_126
-    return C_126_g
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def material_stiffness_matrices_45(C_45: np.ndarray, angles: np.ndarray):
-    """
-    Returns the components of the material stiffness matrix C_45
-    in the global system.
-    """
-    nL = len(C_45)
-    C_45_g = np.zeros_like(C_45)
-    R_45 = np.array([[2, 0], [0, 2]], dtype=C_45_g.dtype)
-    R_45_inv = inv(R_45)
-    T_45 = rotation_matrices_45(angles)
-    for iL in prange(nL):
-        C_45_g[iL] = T_45[iL] @ C_45[iL] @ R_45_inv @ T_45[iL].T @ R_45
-    return C_45_g
+# -*- coding: utf-8 -*-
+import numpy as np
+from numpy import ndarray
+from numpy.linalg import inv
+from numba import njit, prange
+
+from neumann.linalg import linspace1d
+from neumann.array import clip1d
+
+__cache = True
+
+
+@njit(nogil=True, cache=__cache)
+def layers_of_points(points: np.ndarray, bounds: np.ndarray):
+    nL = bounds.shape[0]
+    bins = np.zeros((nL+1,), dtype=points.dtype)
+    bins[0] = bounds[0, 0]
+    bins[1:] = bounds[:, 1]
+    return clip1d(np.digitize(points[:, 2], bins) - 1, 0, nL-1)
+
+
+@njit(['f8[:, :](f8[:, :], i8)', 'f4[:, :](f4[:, :], i8)'],
+      nogil=True, parallel=True, cache=__cache)
+def points_of_layers(bounds: np.ndarray, nppl=3):
+    nL = bounds.shape[0]
+    res = np.zeros((nL, nppl), dtype=bounds.dtype)
+    for iL in prange(nL):
+        res[iL] = linspace1d(bounds[iL, 0], bounds[iL, 1], nppl)
+    return res
+
+
+@njit(nogil=True, cache=__cache)
+def glob_to_loc_layer(point: np.ndarray, bounds: np.ndarray):
+    return (point[2] - bounds[0]) / (bounds[1] - bounds[0])
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def iso_mindlin_plate_bulk(C: ndarray, t: ndarray, k=5/6):
+    res = np.zeros((C.shape[0], 5, 5))
+    for i in prange(res.shape[0]):
+        res[i, :3, :3] = C[i, :3, :3] * (t[i]**3 / 12)
+        res[i, 3:, 3:] = C[i, 3:, 3:] * t[i]
+    res[:, 3:, 3:] *= k
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def iso_membrane_bulk(C: ndarray, t: ndarray):
+    res = np.zeros((C.shape[0], 3, 3))
+    for i in prange(res.shape[0]):
+        res[i, :, :] = C[i, :, :] * t[i]
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def iso_mindlin_shell_bulk(C: ndarray, t: ndarray, k=5/6):
+    res = np.zeros((C.shape[0], 8, 8))
+    res[:, :3, :3] = iso_membrane_bulk(C, t)
+    res[:, 3:, 3:] = iso_mindlin_plate_bulk(C, t, k)
+    return res
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def rotation_matrices_126(angles: np.ndarray):
+    """
+    Returns transformation matrmatrixices T_126 for each angle.
+    Angles are expected in radians.
+    """
+    nL = len(angles)
+    T_126 = np.zeros((nL, 3, 3), dtype=angles.dtype)
+    for iL in prange(nL):
+        a = angles[iL] * np.pi / 180
+        T_126[iL, 0, 0] = np.cos(a)**2
+        T_126[iL, 0, 1] = np.sin(a)**2
+        T_126[iL, 0, 2] = -np.sin(2 * a)
+        T_126[iL, 1, 0] = T_126[iL, 0, 1]
+        T_126[iL, 1, 1] = T_126[iL, 0, 0]
+        T_126[iL, 1, 2] = -T_126[iL, 0, 2]
+        T_126[iL, 2, 0] = np.cos(a) * np.sin(a)
+        T_126[iL, 2, 1] = -T_126[iL, 2, 0]
+        T_126[iL, 2, 2] = np.cos(a)**2 - np.sin(a)**2
+    return T_126
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def rotation_matrices_45(angles: np.ndarray):
+    """
+    Returns transformation matrix T_45 for each angle.
+    Angles are expected in radians.
+    """
+    nL = len(angles)
+    T_45 = np.zeros((nL, 2, 2), dtype=angles.dtype)
+    for iL in prange(nL):
+        a = angles[iL] * np.pi / 180
+        T_45[iL, 0, 0] = np.cos(a)
+        T_45[iL, 0, 1] = -np.sin(a)
+        T_45[iL, 1, 1] = T_45[iL, 0, 0]
+        T_45[iL, 1, 0] = -T_45[iL, 0, 1]
+    return T_45
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def material_stiffness_matrices_126(C_126: np.ndarray, angles: np.ndarray):
+    """
+    Returns the components of the material stiffness matrix C_126
+    in the global system.
+    """
+    nL = len(C_126)
+    C_126_g = np.zeros_like(C_126)
+    R_126 = np.array([[1, 0, 0], [0, 1, 0], [0, 0, 2]], dtype=C_126_g.dtype)
+    R_126_inv = inv(R_126)
+    T_126 = rotation_matrices_126(angles)
+    for iL in prange(nL):
+        C_126_g[iL] = T_126[iL] @ C_126[iL] @ R_126_inv @ T_126[iL].T @ R_126
+    return C_126_g
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def material_stiffness_matrices_45(C_45: np.ndarray, angles: np.ndarray):
+    """
+    Returns the components of the material stiffness matrix C_45
+    in the global system.
+    """
+    nL = len(C_45)
+    C_45_g = np.zeros_like(C_45)
+    R_45 = np.array([[2, 0], [0, 2]], dtype=C_45_g.dtype)
+    R_45_inv = inv(R_45)
+    T_126, T_45 = rotation_matrices_45(angles)
+    for iL in prange(nL):
+        C_45_g[iL] = T_45[iL] @ C_45[iL] @ R_45_inv @ T_45[iL].T @ R_45
+    return C_45_g
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon.egg-info/PKG-INFO` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,104 +1,99 @@
-Metadata-Version: 2.1
-Name: sigmaepsilon
-Version: 0.0.29
-Summary: High-Performance Computational Mechanics in Python.
-Home-page: https://github.com/dewloosh/sigmaepsilon
-Download-URL: https://github.com/dewloosh/sigmaepsilon/archive/refs/tags/0.0.29.zip
-Author: Bence Balogh
-Author-email: benceeok@gmail.com
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: Free for non-commercial use
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.6, <3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **SigmaEpsilon** - High-Performance Computational Solid Mechanics in Python
-
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dewloosh/SigmaEpsilon/main?labpath=notebooksnotebooks%2Flpp.ipynb?urlpath=lab)
-[![CircleCI](https://circleci.com/gh/dewloosh/SigmaEpsilon.svg?style=shield)](https://circleci.com/gh/dewloosh/SigmaEpsilon) 
-[![Documentation Status](https://readthedocs.org/projects/sigmaepsilon/badge/?version=latest)](https://sigmaepsilon.readthedocs.io/en/latest/?badge=latest) 
-[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![PyPI](https://badge.fury.io/py/sigmaepsilon.svg)](https://pypi.org/project/sigmaepsilon)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-> **Warning**
-> This package is under active development and in an **alpha stage**. Come back later, or star the repo to make sure you don’t miss the first stable release!
-
-## Highlights
-
-Head over to the Quick Examples page in the docs to explore our gallery of examples showcasing what SigmaEpsilon can do! Want to test-drive SigmaEpsilon? All of the examples from the gallery are live on MyBinder for you to test drive without installing anything locally: Launch on Binder.
-
-### Overview
-
-* A `solid` submodule to analyze and optimize solid structures of all kinds with the **Finite Element Method**. The implementations so far only cover linear behaviour, but with practically no limits on the complexity of the shape and topology of the domain under investigation.
-
-## Installation
-
-This is optional, but we suggest you to create a dedicated virtual enviroment at all times to avoid conflicts with your other projects. Create a folder, open a command shell in that folder and use the following command
-
-```console
->>> python -m venv venv_name
-```
-
-Once the enviroment is created, activate it via typing
-
-```console
->>> .\venv_name\Scripts\activate
-```
-
-`sigmaepsilon` can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.6:
-
-```console
->>> pip install sigmaepsilon
-```
-
-## **Documentation**
-
-Refer to the [docs](https://sigmaepsilon.readthedocs.io/en/latest/) for further details on installation and usage.
-
-## **Testing**
-
-To run all tests, open up a console in the root directory of the project and type the following
-
-```console
->>> python -m unittest
-```
-
-## **Dependencies**
-
-We use Numba's JIT compiler to speed up heavy computations, and it relies on the C++ redistributable package. It is likely already installed on your system, but if it is not, you can download it from Microsoft's website under "Other Tools, Frameworks, and Redistributables".
-
-must have
-
-* `Numba`, `NumPy`, `SciPy`, `SymPy`, `awkward`
-
-strongly suggested
-
-* `PyVista`, `Plotly`, `matplotlib`, `sectionproperties`
-
-optional
-
-* `networkx`
-
-## **License**
-
-SigmaEpsilon is Copyright(C) 2022: Bence Balogh
-
-All rights reserved.
-
-This program is dual-licensed as follows:
-
-(1) You may use SigmaEpsilon as free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
-
-In this case the program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License at http://www.gnu.org/licenses/gpl.txt or in the LICENSE file of this repository for more details.
-
-(2) You may use SigmaEpsilon as part of a commercial software. In this case a proper agreement must be reached with the Authors based on a proper licensing contract.
+Metadata-Version: 2.1
+Name: sigmaepsilon
+Version: 0.0.2b0
+Summary: High-Performance Computational Mechanics in Python.
+Home-page: https://github.com/dewloosh/sigmaepsilon
+Author: Bence Balogh
+Author-email: benceeok@gmail.com
+License: UNKNOWN
+Download-URL: https://github.com/dewloosh/sigmaepsilon/archive/refs/tags/0.0.2b.zip
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6, <3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **SigmaEpsilon** - High-Performance Computational Solid Mechanics in Python
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dewloosh/SigmaEpsilon/main?labpath=notebooksnotebooks%2Flpp.ipynb?urlpath=lab)
+[![CircleCI](https://circleci.com/gh/dewloosh/SigmaEpsilon.svg?style=shield)](https://circleci.com/gh/dewloosh/SigmaEpsilon) 
+[![Documentation Status](https://readthedocs.org/projects/sigmaepsilon/badge/?version=latest)](https://sigmaepsilon.readthedocs.io/en/latest/?badge=latest) 
+[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI](https://badge.fury.io/py/sigmaepsilon.svg)](https://pypi.org/project/sigmaepsilon) 
+
+> **Warning**
+> This package is under active development and in an **alpha stage**. Come back later, or star the repo to make sure you donâ€™t miss the first stable release!
+
+## Highlights
+
+Head over to the Quick Examples page in the docs to explore our gallery of examples showcasing what SigmaEpsilon can do! Want to test-drive SigmaEpsilon? All of the examples from the gallery are live on MyBinder for you to test drive without installing anything locally: Launch on Binder.
+
+### Overview
+
+* A `solid` submodule to analyze and optimize solid structures of all kinds with the **Finite Element Method**. The implementations so far only cover linear behaviour, but with practically no limits on the complexity of the shape and topology of the domain under investigation.
+
+## **Installation**
+This is optional, but we suggest you to create a dedicated virtual enviroment at all times to avoid conflicts with your other projects. Create a folder, open a command shell in that folder and use the following command
+
+```console
+>>> python -m venv venv_name
+```
+
+Once the enviroment is created, activate it via typing
+
+```console
+>>> .\venv_name\Scripts\activate
+```
+
+`sigmaepsilon` can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.6:
+
+```console
+>>> pip install sigmaepsilon
+```
+
+## **Documentation**
+
+Refer to the [docs](https://sigmaepsilon.readthedocs.io/en/latest/) for further details on installation and usage.
+
+## **Testing**
+
+To run all tests, open up a console in the root directory of the project and type the following
+
+```console
+>>> python -m unittest
+```
+
+## **Dependencies**
+
+We use Numba's JIT compiler to speed up heavy computations, and it relies on the C++ redistributable package. It is likely already installed on your system, but if it is not, you can download it from Microsoft's website under "Other Tools, Frameworks, and Redistributables".
+
+must have 
+  * `Numba`, `NumPy`, `SciPy`, `SymPy`, `awkward`
+
+strongly suggested
+  * `PyVista`, `Plotly`, `matplotlib`, `sectionproperties`
+
+optional 
+  * `networkx`
+
+## **License**
+
+SigmaEpsilon is Copyright(C) 2022: Bence Balogh
+
+All rights reserved.
+
+This program is dual-licensed as follows:
+
+(1) You may use SigmaEpsilon as free software; you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; either version 3 of the License, or (at your option) any later version.
+
+In this case the program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License (http://www.gnu.org/licenses/gpl.txt) for more details.
+
+(2) You may use SigmaEpsilon as part of a commercial software. In this case a proper agreement must be reached with the Authors based on a proper licensing contract.
+
```

### Comparing `sigmaepsilon-0.0.29/src/sigmaepsilon.egg-info/SOURCES.txt` & `sigmaepsilon-0.0.2b0/src/sigmaepsilon.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -2,112 +2,106 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
 test-requirements.txt
 src/sigmaepsilon/__init__.py
-src/sigmaepsilon/config.py
+src/sigmaepsilon/io.py
 src/sigmaepsilon.egg-info/PKG-INFO
 src/sigmaepsilon.egg-info/SOURCES.txt
 src/sigmaepsilon.egg-info/dependency_links.txt
 src/sigmaepsilon.egg-info/not-zip-safe
 src/sigmaepsilon.egg-info/requires.txt
 src/sigmaepsilon.egg-info/top_level.txt
-src/sigmaepsilon/core/__init__.py
-src/sigmaepsilon/core/material.py
 src/sigmaepsilon/examples/__init__.py
 src/sigmaepsilon/examples/downloads.py
 src/sigmaepsilon/examples/examples.py
-src/sigmaepsilon/fem/__init__.py
-src/sigmaepsilon/fem/constants.py
-src/sigmaepsilon/fem/dofmap.py
-src/sigmaepsilon/fem/ebc.py
-src/sigmaepsilon/fem/femsolver.py
-src/sigmaepsilon/fem/linemesh.py
-src/sigmaepsilon/fem/mesh.py
-src/sigmaepsilon/fem/metamesh.py
-src/sigmaepsilon/fem/pointdata.py
-src/sigmaepsilon/fem/structure.py
-src/sigmaepsilon/fem/surfacemesh.py
-src/sigmaepsilon/fem/cells/Q5V.py
-src/sigmaepsilon/fem/cells/__init__.py
-src/sigmaepsilon/fem/cells/andes.py
-src/sigmaepsilon/fem/cells/bernoulli.py
-src/sigmaepsilon/fem/cells/bernoulli2.py
-src/sigmaepsilon/fem/cells/bernoulli3.py
-src/sigmaepsilon/fem/cells/celldata.py
-src/sigmaepsilon/fem/cells/cst.py
-src/sigmaepsilon/fem/cells/elem.py
-src/sigmaepsilon/fem/cells/h27.py
-src/sigmaepsilon/fem/cells/h8.py
-src/sigmaepsilon/fem/cells/lst.py
-src/sigmaepsilon/fem/cells/meta.py
-src/sigmaepsilon/fem/cells/q4.py
-src/sigmaepsilon/fem/cells/q9.py
-src/sigmaepsilon/fem/cells/tet10.py
-src/sigmaepsilon/fem/cells/tet4.py
-src/sigmaepsilon/fem/cells/wedge.py
-src/sigmaepsilon/fem/cells/gen/__init__.py
-src/sigmaepsilon/fem/cells/gen/b2.py
-src/sigmaepsilon/fem/cells/gen/b3.py
-src/sigmaepsilon/fem/material/__init__.py
-src/sigmaepsilon/fem/material/beam.py
-src/sigmaepsilon/fem/material/membrane.py
-src/sigmaepsilon/fem/material/mindlinplate.py
-src/sigmaepsilon/fem/material/mindlinshell.py
-src/sigmaepsilon/fem/material/solid.py
-src/sigmaepsilon/fem/material/solid3d.py
-src/sigmaepsilon/fem/material/surface.py
-src/sigmaepsilon/fourier/__init__.py
-src/sigmaepsilon/fourier/beam.py
-src/sigmaepsilon/fourier/loads.py
-src/sigmaepsilon/fourier/plate.py
-src/sigmaepsilon/fourier/postproc.py
-src/sigmaepsilon/fourier/preproc.py
-src/sigmaepsilon/fourier/problem.py
-src/sigmaepsilon/fourier/proc.py
-src/sigmaepsilon/fourier/utils.py
-src/sigmaepsilon/material/__init__.py
-src/sigmaepsilon/material/beam/__init__.py
-src/sigmaepsilon/material/beam/bernoulli/__init__.py
-src/sigmaepsilon/material/beam/bernoulli/section.py
-src/sigmaepsilon/material/homg/__init__.py
-src/sigmaepsilon/material/homg/ebc.py
-src/sigmaepsilon/material/homg/rvs.py
-src/sigmaepsilon/material/homg/utils.py
-src/sigmaepsilon/material/hooke/__init__.py
-src/sigmaepsilon/material/hooke/sym.py
-src/sigmaepsilon/material/hooke/tensor.py
-src/sigmaepsilon/material/hooke/utils.py
-src/sigmaepsilon/material/surface/__init__.py
-src/sigmaepsilon/material/surface/membrane.py
-src/sigmaepsilon/material/surface/meta.py
-src/sigmaepsilon/material/surface/mindlin.py
+src/sigmaepsilon/solid/__init__.py
+src/sigmaepsilon/solid/config.py
+src/sigmaepsilon/solid/fem/__init__.py
+src/sigmaepsilon/solid/fem/config.py
+src/sigmaepsilon/solid/fem/dyn.py
+src/sigmaepsilon/solid/fem/eigsolve.py
+src/sigmaepsilon/solid/fem/femsolver.py
+src/sigmaepsilon/solid/fem/imap.py
+src/sigmaepsilon/solid/fem/io.py
+src/sigmaepsilon/solid/fem/linemesh.py
+src/sigmaepsilon/solid/fem/linsolve.py
+src/sigmaepsilon/solid/fem/mesh.py
+src/sigmaepsilon/solid/fem/pointdata.py
+src/sigmaepsilon/solid/fem/postproc.py
+src/sigmaepsilon/solid/fem/preproc.py
+src/sigmaepsilon/solid/fem/structure.py
+src/sigmaepsilon/solid/fem/surfacemesh.py
+src/sigmaepsilon/solid/fem/tr.py
+src/sigmaepsilon/solid/fem/utils.py
+src/sigmaepsilon/solid/fem/cells/__init__.py
+src/sigmaepsilon/solid/fem/cells/bernoulli.py
+src/sigmaepsilon/solid/fem/cells/bernoulli2.py
+src/sigmaepsilon/solid/fem/cells/bernoulli3.py
+src/sigmaepsilon/solid/fem/cells/celldata.py
+src/sigmaepsilon/solid/fem/cells/cst.py
+src/sigmaepsilon/solid/fem/cells/elem.py
+src/sigmaepsilon/solid/fem/cells/felippa.py
+src/sigmaepsilon/solid/fem/cells/h27.py
+src/sigmaepsilon/solid/fem/cells/h8.py
+src/sigmaepsilon/solid/fem/cells/lst.py
+src/sigmaepsilon/solid/fem/cells/meta.py
+src/sigmaepsilon/solid/fem/cells/q4.py
+src/sigmaepsilon/solid/fem/cells/q9.py
+src/sigmaepsilon/solid/fem/cells/tet10.py
+src/sigmaepsilon/solid/fem/cells/tet4.py
+src/sigmaepsilon/solid/fem/cells/gen/__init__.py
+src/sigmaepsilon/solid/fem/cells/gen/b2.py
+src/sigmaepsilon/solid/fem/cells/gen/b3.py
+src/sigmaepsilon/solid/fem/cells/utils/__init__.py
+src/sigmaepsilon/solid/fem/cells/utils/bernoulli.py
+src/sigmaepsilon/solid/fem/cells/utils/utils.py
+src/sigmaepsilon/solid/fem/model/__init__.py
+src/sigmaepsilon/solid/fem/model/beam.py
+src/sigmaepsilon/solid/fem/model/membrane.py
+src/sigmaepsilon/solid/fem/model/plate.py
+src/sigmaepsilon/solid/fem/model/solid.py
+src/sigmaepsilon/solid/fem/model/solid3d.py
+src/sigmaepsilon/solid/fem/model/surface.py
+src/sigmaepsilon/solid/fem/model/utils.py
+src/sigmaepsilon/solid/fourier/__init__.py
+src/sigmaepsilon/solid/fourier/doc.py
+src/sigmaepsilon/solid/fourier/latex.py
+src/sigmaepsilon/solid/fourier/loads.py
+src/sigmaepsilon/solid/fourier/plate.py
+src/sigmaepsilon/solid/fourier/plot.py
+src/sigmaepsilon/solid/fourier/postproc.py
+src/sigmaepsilon/solid/fourier/preproc.py
+src/sigmaepsilon/solid/fourier/proc.py
+src/sigmaepsilon/solid/fourier/symtools.py
+src/sigmaepsilon/solid/material/__init__.py
+src/sigmaepsilon/solid/material/utils.py
+src/sigmaepsilon/solid/material/hooke/sym.py
+src/sigmaepsilon/solid/material/hooke/utils.py
+src/sigmaepsilon/solid/model/__init__.py
+src/sigmaepsilon/solid/model/membrane.py
+src/sigmaepsilon/solid/model/metashell.py
+src/sigmaepsilon/solid/model/utils.py
+src/sigmaepsilon/solid/model/bernoulli/__init__.py
+src/sigmaepsilon/solid/model/bernoulli/section.py
+src/sigmaepsilon/solid/model/bernoulli/utils.py
+src/sigmaepsilon/solid/model/mindlin/__init__.py
+src/sigmaepsilon/solid/model/mindlin/mindlin.py
+src/sigmaepsilon/solid/model/mindlin/postproc.py
+src/sigmaepsilon/solid/model/mindlin/utils.py
 src/sigmaepsilon/topopt/__init__.py
+src/sigmaepsilon/topopt/fem/__init__.py
+src/sigmaepsilon/topopt/fem/mesh.py
+src/sigmaepsilon/topopt/fem/cells/Q5V.py
+src/sigmaepsilon/topopt/fem/cells/__init__.py
+src/sigmaepsilon/topopt/fem/structure/__init__.py
+src/sigmaepsilon/topopt/fem/structure/domain.py
+src/sigmaepsilon/topopt/fem/structure/structure.py
 src/sigmaepsilon/topopt/joint/__init__.py
 src/sigmaepsilon/topopt/joint/cubejoint.py
+src/sigmaepsilon/topopt/oc/SIMP_OC_FEM_old.py
 src/sigmaepsilon/topopt/oc/__init__.py
 src/sigmaepsilon/topopt/oc/filter.py
 src/sigmaepsilon/topopt/oc/oc.py
-src/sigmaepsilon/topopt/oc/utils.py
-src/sigmaepsilon/utils/__init__.py
-src/sigmaepsilon/utils/fem/__init__.py
-src/sigmaepsilon/utils/fem/dyn.py
-src/sigmaepsilon/utils/fem/ebc.py
-src/sigmaepsilon/utils/fem/eigsolve.py
-src/sigmaepsilon/utils/fem/fem.py
-src/sigmaepsilon/utils/fem/imap.py
-src/sigmaepsilon/utils/fem/linsolve.py
-src/sigmaepsilon/utils/fem/postproc.py
-src/sigmaepsilon/utils/fem/preproc.py
-src/sigmaepsilon/utils/fem/tr.py
-src/sigmaepsilon/utils/fem/cells/__init__.py
-src/sigmaepsilon/utils/fem/cells/bernoulli.py
-src/sigmaepsilon/utils/fem/cells/cells.py
-src/sigmaepsilon/utils/material/__init__.py
-src/sigmaepsilon/utils/material/bernoulli.py
-src/sigmaepsilon/utils/material/hmh.py
-src/sigmaepsilon/utils/material/material.py
-src/sigmaepsilon/utils/material/mindlin.py
-src/sigmaepsilon/utils/material/postproc.py
-src/sigmaepsilon/utils/material/surface.py
+src/sigmaepsilon/topopt/oc/utils.py
```

