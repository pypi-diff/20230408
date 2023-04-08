# Comparing `tmp/emmet-api-0.51.8.tar.gz` & `tmp/emmet-api-0.51.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.51.8.tar", last modified: Fri Apr  7 22:34:38 2023, max compression
+gzip compressed data, was "emmet-api-0.51.9.tar", last modified: Fri Apr  7 23:09:39 2023, max compression
```

## Comparing `emmet-api-0.51.8.tar` & `emmet-api-0.51.9.tar`

### file list

```diff
@@ -1,339 +1,339 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.946123 emmet-api-0.51.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-07 22:34:34.000000 emmet-api-0.51.8/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-07 22:34:38.946123 emmet-api-0.51.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-07 22:34:34.000000 emmet-api-0.51.8/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.918124 emmet-api-0.51.8/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.922124 emmet-api-0.51.8/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.922124 emmet-api-0.51.8/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.922124 emmet-api-0.51.8/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.926123 emmet-api-0.51.8/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.926123 emmet-api-0.51.8/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.926123 emmet-api-0.51.8/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.926123 emmet-api-0.51.8/emmet/api/routes/absorption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.926123 emmet-api-0.51.8/emmet/api/routes/alloys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.926123 emmet-api-0.51.8/emmet/api/routes/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.926123 emmet-api-0.51.8/emmet/api/routes/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.926123 emmet-api-0.51.8/emmet/api/routes/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.926123 emmet-api-0.51.8/emmet/api/routes/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.926123 emmet-api-0.51.8/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.926123 emmet-api-0.51.8/emmet/api/routes/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.926123 emmet-api-0.51.8/emmet/api/routes/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.926123 emmet-api-0.51.8/emmet/api/routes/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.926123 emmet-api-0.51.8/emmet/api/routes/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/fermi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/materials/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/mpcules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/mpcules/association/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/mpcules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/mpcules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    17188 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/mpcules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19772 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/mpcules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/mpcules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/mpcules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.930123 emmet-api-0.51.8/emmet/api/routes/mpcules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.934123 emmet-api-0.51.8/emmet/api/routes/mpcules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/tasks/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.934123 emmet-api-0.51.8/emmet/api/routes/mpcules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.934123 emmet-api-0.51.8/emmet/api/routes/mpcules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/mpcules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.934123 emmet-api-0.51.8/emmet/api/routes/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.934123 emmet-api-0.51.8/emmet/api/routes/phonon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.934123 emmet-api-0.51.8/emmet/api/routes/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.934123 emmet-api-0.51.8/emmet/api/routes/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.934123 emmet-api-0.51.8/emmet/api/routes/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.934123 emmet-api-0.51.8/emmet/api/routes/similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.934123 emmet-api-0.51.8/emmet/api/routes/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.934123 emmet-api-0.51.8/emmet/api/routes/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.934123 emmet-api-0.51.8/emmet/api/routes/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.934123 emmet-api-0.51.8/emmet/api/routes/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.938123 emmet-api-0.51.8/emmet/api/routes/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.938123 emmet-api-0.51.8/emmet/api/routes/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.938123 emmet-api-0.51.8/emmet/api/routes/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-07 22:34:34.000000 emmet-api-0.51.8/emmet/api/routes/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.938123 emmet-api-0.51.8/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-07 22:34:38.000000 emmet-api-0.51.8/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-04-07 22:34:38.000000 emmet-api-0.51.8/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 22:34:38.000000 emmet-api-0.51.8/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 22:34:38.000000 emmet-api-0.51.8/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-07 22:34:38.000000 emmet-api-0.51.8/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-07 22:34:38.000000 emmet-api-0.51.8/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-04-07 22:34:34.000000 emmet-api-0.51.8/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-07 22:34:34.000000 emmet-api-0.51.8/mpcule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.938123 emmet-api-0.51.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-04-07 22:34:34.000000 emmet-api-0.51.8/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 22:34:38.946123 emmet-api-0.51.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-07 22:34:34.000000 emmet-api-0.51.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-07 22:34:34.000000 emmet-api-0.51.8/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.938123 emmet-api-0.51.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.938123 emmet-api-0.51.8/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.938123 emmet-api-0.51.8/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/_general_store/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.938123 emmet-api-0.51.8/tests/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.938123 emmet-api-0.51.8/tests/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/chemenv/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/materials/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/mpcules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/mpcules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/mpcules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/mpcules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/mpcules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/mpcules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.942123 emmet-api-0.51.8/tests/mpcules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/tasks/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.946123 emmet-api-0.51.8/tests/mpcules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/mpcules/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.946123 emmet-api-0.51.8/tests/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.946123 emmet-api-0.51.8/tests/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.946123 emmet-api-0.51.8/tests/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.946123 emmet-api-0.51.8/tests/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.946123 emmet-api-0.51.8/tests/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.946123 emmet-api-0.51.8/tests/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.946123 emmet-api-0.51.8/tests/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.946123 emmet-api-0.51.8/tests/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.946123 emmet-api-0.51.8/tests/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:38.946123 emmet-api-0.51.8/tests/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-07 22:34:34.000000 emmet-api-0.51.8/tests/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-07 23:09:30.000000 emmet-api-0.51.9/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-07 23:09:39.466811 emmet-api-0.51.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-07 23:09:30.000000 emmet-api-0.51.9/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.438810 emmet-api-0.51.9/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/absorption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/alloys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.446810 emmet-api-0.51.9/emmet/api/routes/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/fermi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/materials/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10578 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcules/association/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17188 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19772 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.450810 emmet-api-0.51.9/emmet/api/routes/mpcules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/mpcules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/mpcules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/mpcules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/tasks/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/mpcules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/mpcules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/mpcules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/phonon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.454810 emmet-api-0.51.9/emmet/api/routes/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.458810 emmet-api-0.51.9/emmet/api/routes/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.458810 emmet-api-0.51.9/emmet/api/routes/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.458810 emmet-api-0.51.9/emmet/api/routes/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.458810 emmet-api-0.51.9/emmet/api/routes/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-04-07 23:09:30.000000 emmet-api-0.51.9/emmet/api/routes/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.458810 emmet-api-0.51.9/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-07 23:09:38.000000 emmet-api-0.51.9/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-04-07 23:09:39.000000 emmet-api-0.51.9/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:09:38.000000 emmet-api-0.51.9/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:09:38.000000 emmet-api-0.51.9/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-07 23:09:38.000000 emmet-api-0.51.9/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-07 23:09:38.000000 emmet-api-0.51.9/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-04-07 23:09:30.000000 emmet-api-0.51.9/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-07 23:09:30.000000 emmet-api-0.51.9/mpcule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.458810 emmet-api-0.51.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5846 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9082 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6008 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-04-07 23:09:30.000000 emmet-api-0.51.9/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 23:09:39.466811 emmet-api-0.51.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-07 23:09:30.000000 emmet-api-0.51.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-07 23:09:30.000000 emmet-api-0.51.9/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.458810 emmet-api-0.51.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/_general_store/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/chemenv/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/materials/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/mpcules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/mpcules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/mpcules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/mpcules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.462811 emmet-api-0.51.9/tests/mpcules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/mpcules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/mpcules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/tasks/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/mpcules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/mpcules/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:39.466811 emmet-api-0.51.9/tests/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-07 23:09:30.000000 emmet-api-0.51.9/tests/xas/test_query_operators.py
```

### Comparing `emmet-api-0.51.8/Dockerfile` & `emmet-api-0.51.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/core/api.py` & `emmet-api-0.51.9/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.51.9/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.51.9/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/core/documentation.py` & `emmet-api-0.51.9/emmet/api/core/documentation.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/core/global_header.py` & `emmet-api-0.51.9/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/core/settings.py` & `emmet-api-0.51.9/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.51.9/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.51.9/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.51.9/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.51.9/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/absorption/resources.py` & `emmet-api-0.51.9/emmet/api/routes/absorption/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/alloys/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/alloys/resources.py` & `emmet-api-0.51.9/emmet/api/routes/alloys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/bonds/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/bonds/resources.py` & `emmet-api-0.51.9/emmet/api/routes/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/charge_density/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/charge_density/resources.py` & `emmet-api-0.51.9/emmet/api/routes/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/chemenv/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/chemenv/resources.py` & `emmet-api-0.51.9/emmet/api/routes/chemenv/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/dielectric/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/dielectric/resources.py` & `emmet-api-0.51.9/emmet/api/routes/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/dois/resources.py` & `emmet-api-0.51.9/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/elasticity/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/elasticity/resources.py` & `emmet-api-0.51.9/emmet/api/routes/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/electrodes/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/electrodes/resources.py` & `emmet-api-0.51.9/emmet/api/routes/electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/electrodes/utils.py` & `emmet-api-0.51.9/emmet/api/routes/electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/electronic_structure/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/electronic_structure/resources.py` & `emmet-api-0.51.9/emmet/api/routes/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/eos/resources.py` & `emmet-api-0.51.9/emmet/api/routes/eos/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/fermi/resources.py` & `emmet-api-0.51.9/emmet/api/routes/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/grain_boundary/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/grain_boundary/resources.py` & `emmet-api-0.51.9/emmet/api/routes/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/magnetism/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/magnetism/resources.py` & `emmet-api-0.51.9/emmet/api/routes/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/materials/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/materials/resources.py` & `emmet-api-0.51.9/emmet/api/routes/materials/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/materials/utils.py` & `emmet-api-0.51.9/emmet/api/routes/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/molecules/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/molecules/resources.py` & `emmet-api-0.51.9/emmet/api/routes/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcomplete/query_operator.py` & `emmet-api-0.51.9/emmet/api/routes/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcomplete/resources.py` & `emmet-api-0.51.9/emmet/api/routes/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/association/resources.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/association/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/bonds/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/bonds/resources.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/molecules/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/molecules/resources.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/orbitals/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/orbitals/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/orbitals/resources.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/orbitals/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/partial_charges/resources.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/partial_charges/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/partial_spins/resources.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/partial_spins/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/redox/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/redox/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/redox/resources.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/redox/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/summary/hint_scheme.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/summary/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/summary/resources.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/tasks/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/tasks/resources.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/thermo/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/thermo/resources.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/utils.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/mpcules/vibrations/resources.py` & `emmet-api-0.51.9/emmet/api/routes/mpcules/vibrations/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/oxidation_states/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/oxidation_states/resources.py` & `emmet-api-0.51.9/emmet/api/routes/oxidation_states/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/phonon/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/phonon/resources.py` & `emmet-api-0.51.9/emmet/api/routes/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/piezo/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/piezo/resources.py` & `emmet-api-0.51.9/emmet/api/routes/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/provenance/resources.py` & `emmet-api-0.51.9/emmet/api/routes/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/robocrys/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/robocrys/resources.py` & `emmet-api-0.51.9/emmet/api/routes/robocrys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/similarity/resources.py` & `emmet-api-0.51.9/emmet/api/routes/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/substrates/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/substrates/resources.py` & `emmet-api-0.51.9/emmet/api/routes/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/summary/hint_scheme.py` & `emmet-api-0.51.9/emmet/api/routes/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/summary/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/summary/resources.py` & `emmet-api-0.51.9/emmet/api/routes/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/surface_properties/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/surface_properties/resources.py` & `emmet-api-0.51.9/emmet/api/routes/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/synthesis/data_adaptor.py` & `emmet-api-0.51.9/emmet/api/routes/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/synthesis/data_adaptor_synpro.py` & `emmet-api-0.51.9/emmet/api/routes/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/synthesis/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/synthesis/resources.py` & `emmet-api-0.51.9/emmet/api/routes/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/synthesis/utils.py` & `emmet-api-0.51.9/emmet/api/routes/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/tasks/hint_scheme.py` & `emmet-api-0.51.9/emmet/api/routes/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/tasks/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/tasks/resources.py` & `emmet-api-0.51.9/emmet/api/routes/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/tasks/utils.py` & `emmet-api-0.51.9/emmet/api/routes/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/thermo/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/thermo/resources.py` & `emmet-api-0.51.9/emmet/api/routes/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/xas/query_operators.py` & `emmet-api-0.51.9/emmet/api/routes/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet/api/routes/xas/resources.py` & `emmet-api-0.51.9/emmet/api/routes/xas/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/emmet_api.egg-info/SOURCES.txt` & `emmet-api-0.51.9/emmet_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/material_resources.py` & `emmet-api-0.51.9/material_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/mpcule_resources.py` & `emmet-api-0.51.9/mpcule_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/deployment.txt` & `emmet-api-0.51.9/requirements/deployment.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/macos-latest_py3.10.txt` & `emmet-api-0.51.9/requirements/macos-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/macos-latest_py3.10_extras.txt` & `emmet-api-0.51.9/requirements/macos-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/macos-latest_py3.11.txt` & `emmet-api-0.51.9/requirements/macos-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/macos-latest_py3.11_extras.txt` & `emmet-api-0.51.9/requirements/macos-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/macos-latest_py3.8.txt` & `emmet-api-0.51.9/requirements/macos-latest_py3.8.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/macos-latest_py3.8_extras.txt` & `emmet-api-0.51.9/requirements/macos-latest_py3.8_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/macos-latest_py3.9.txt` & `emmet-api-0.51.9/requirements/macos-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/macos-latest_py3.9_extras.txt` & `emmet-api-0.51.9/requirements/macos-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.51.9/requirements/ubuntu-latest_py3.10.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.51.9/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.51.9/requirements/ubuntu-latest_py3.11.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.51.9/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/ubuntu-latest_py3.8.txt` & `emmet-api-0.51.9/requirements/ubuntu-latest_py3.8.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/ubuntu-latest_py3.8_extras.txt` & `emmet-api-0.51.9/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.51.9/requirements/ubuntu-latest_py3.9.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.51.9/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/setup.py` & `emmet-api-0.51.9/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/_consumer/test_query_operators.py` & `emmet-api-0.51.9/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/_general_store/test_query_operators.py` & `emmet-api-0.51.9/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/bonds/test_query_operators.py` & `emmet-api-0.51.9/tests/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/charge_density/test_query_operators.py` & `emmet-api-0.51.9/tests/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/chemenv/test_query_operators.py` & `emmet-api-0.51.9/tests/chemenv/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/core/test_mapi.py` & `emmet-api-0.51.9/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/dielectric/test_query_operators.py` & `emmet-api-0.51.9/tests/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/elasticity/test_query_operators.py` & `emmet-api-0.51.9/tests/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/electrodes/test_query_operators.py` & `emmet-api-0.51.9/tests/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/electrodes/test_utils.py` & `emmet-api-0.51.9/tests/electrodes/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/electronic_structure/test_query_operators.py` & `emmet-api-0.51.9/tests/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/grain_boundary/test_query_operators.py` & `emmet-api-0.51.9/tests/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/magnetism/test_query_operators.py` & `emmet-api-0.51.9/tests/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/materials/test_query_operators.py` & `emmet-api-0.51.9/tests/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/materials/test_utils.py` & `emmet-api-0.51.9/tests/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/molecules/test_query_operators.py` & `emmet-api-0.51.9/tests/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/mpcomplete/test_query_operators.py` & `emmet-api-0.51.9/tests/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/mpcules/bonds/test_query_operators.py` & `emmet-api-0.51.9/tests/mpcules/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/mpcules/molecules/test_query_operators.py` & `emmet-api-0.51.9/tests/mpcules/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/mpcules/orbitals/test_query_operators.py` & `emmet-api-0.51.9/tests/mpcules/orbitals/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/mpcules/redox/test_query_operators.py` & `emmet-api-0.51.9/tests/mpcules/redox/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/mpcules/summary/test_query_operators.py` & `emmet-api-0.51.9/tests/mpcules/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/mpcules/tasks/test_query_operators.py` & `emmet-api-0.51.9/tests/mpcules/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/mpcules/thermo/test_query_operators.py` & `emmet-api-0.51.9/tests/mpcules/thermo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/oxidation_states/test_query_operators.py` & `emmet-api-0.51.9/tests/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/piezo/test_query_operators.py` & `emmet-api-0.51.9/tests/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/robocrys/test_query_operators.py` & `emmet-api-0.51.9/tests/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/substrates/test_query_operators.py` & `emmet-api-0.51.9/tests/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/summary/test_query_operators.py` & `emmet-api-0.51.9/tests/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/surface_properties/test_query_operators.py` & `emmet-api-0.51.9/tests/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/synthesis/test_adaptor.py` & `emmet-api-0.51.9/tests/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/synthesis/test_adaptor_synpro.py` & `emmet-api-0.51.9/tests/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/synthesis/test_query_operators.py` & `emmet-api-0.51.9/tests/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/synthesis/test_utils.py` & `emmet-api-0.51.9/tests/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/tasks/test_query_operators.py` & `emmet-api-0.51.9/tests/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/tasks/test_utils.py` & `emmet-api-0.51.9/tests/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.51.8/tests/xas/test_query_operators.py` & `emmet-api-0.51.9/tests/xas/test_query_operators.py`

 * *Files identical despite different names*

