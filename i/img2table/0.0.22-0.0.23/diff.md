# Comparing `tmp/img2table-0.0.22.tar.gz` & `tmp/img2table-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/img2table-0.0.22.tar", last modified: Fri Apr  7 15:10:32 2023, max compression
+gzip compressed data, was "dist/img2table-0.0.23.tar", last modified: Sat Apr  8 17:40:15 2023, max compression
```

## Comparing `img2table-0.0.22.tar` & `img2table-0.0.23.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-07 15:08:38.000000 img2table-0.0.22/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-07 15:08:38.000000 img2table-0.0.22/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-07 15:08:38.000000 img2table-0.0.22/.github/workflows/test_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-07 15:08:38.000000 img2table-0.0.22/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-07 15:08:38.000000 img2table-0.0.22/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-04-07 15:10:32.000000 img2table-0.0.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-04-07 15:08:38.000000 img2table-0.0.22/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-07 15:08:38.000000 img2table-0.0.22/activate_venv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    46045 2023-04-07 15:08:38.000000 img2table-0.0.22/examples/Basic_usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    32897 2023-04-07 15:08:38.000000 img2table-0.0.22/examples/Implicit_rows.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-04-07 15:08:38.000000 img2table-0.0.22/examples/borderless.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)    71022 2023-04-07 15:08:38.000000 img2table-0.0.22/examples/data/borderless_aws.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-04-07 15:08:38.000000 img2table-0.0.22/examples/data/borderless_ocr.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-07 15:08:38.000000 img2table-0.0.22/examples/data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-07 15:08:38.000000 img2table-0.0.22/examples/data/tables.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-07 15:08:38.000000 img2table-0.0.22/examples/data/tables.png
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-07 15:08:38.000000 img2table-0.0.22/examples/data/tables.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-07 15:08:38.000000 img2table-0.0.22/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-07 15:08:38.000000 img2table-0.0.22/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-07 15:08:38.000000 img2table-0.0.22/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-07 15:08:38.000000 img2table-0.0.22/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-07 15:10:32.000000 img2table-0.0.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-07 15:08:38.000000 img2table-0.0.22/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table/document/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/document/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/document/base/rotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/document/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/document/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/ocr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/ocr/aws_textract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/ocr/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/ocr/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/ocr/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/ocr/google_vision.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/ocr/paddle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/ocr/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/ocr/tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/objects/cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/objects/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/objects/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/objects/row.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/objects/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/bordered_tables/cells/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/bordered_tables/lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/borderless_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/borderless_tables/column_delimiters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/borderless_tables/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/borderless_tables/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/borderless_tables/segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/borderless_tables/table/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/borderless_tables/table/table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-07 15:08:38.000000 img2table-0.0.22/src/img2table/tables/processing/text/titles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-04-07 15:10:31.000000 img2table-0.0.22/src/img2table.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-07 15:10:32.000000 img2table-0.0.22/src/img2table.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:10:31.000000 img2table-0.0.22/src/img2table.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 15:10:31.000000 img2table-0.0.22/src/img2table.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-07 15:10:31.000000 img2table-0.0.22/src/img2table.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-07 15:10:31.000000 img2table-0.0.22/src/img2table.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 15:10:31.000000 img2table-0.0.22/src/img2table.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/_mock_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/_mock_data/azure.pkl
--rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/_mock_data/tesseract_hocr.html
--rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/_mock_data/textract.json
--rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/_mock_data/vision.json
--rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/_mock_data/vision.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/document/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/document/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/document/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/document/base/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/document/base/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/document/base/test_rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/document/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/document/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/document/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/document/image/test_data/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/document/image/test_data/expected.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/document/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/document/image/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/document/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/document/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/document/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/document/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/document/pdf/test_pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/aws_textract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/aws_textract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/aws_textract/test_aws_textract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/aws_textract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/aws_textract/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/aws_textract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/aws_textract/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/azure/test_azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/azure/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/azure/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/azure/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/data/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/data/test_data/expected_table.json
--rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/data/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/data/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/data/test_ocr_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/google_vision/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/google_vision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/google_vision/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/google_vision/test_data/expected_content.json
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/google_vision/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/google_vision/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/google_vision/test_google_vision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/paddle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/paddle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/paddle/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/paddle/test_data/hocr.json
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/paddle/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/paddle/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/paddle/test_paddle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/pdf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/pdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/pdf/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    35369 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/pdf/test_data/content.json
--rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/pdf/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/pdf/test_data/test.pdf
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/pdf/test_pdf_ocr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/tesseract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/tesseract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/ocr/tesseract/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/tesseract/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/tesseract/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/ocr/tesseract/test_tesseract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/image/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/image/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/image/test_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/objects/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/objects/test_data/expected_tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/objects/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/objects/test_data/tables.json
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/objects/test_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/objects/test_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/objects/test_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/objects/test_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/cells/test_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/cells/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/cells/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/lines/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/lines/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/lines/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/cells.json
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/expected.json
--rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/implicit_ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_table_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/borderless_table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/borderless_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/borderless_table/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/borderless_table/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/column_delimiters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/lines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/lines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/lines/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/lines/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/lines/test_lines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/segment_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/segment_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/segment_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/segment_image/test_data/ocr_df.csv
--rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/table/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/table/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/borderless_tables/table/test_table_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/common/test_common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/common/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/common/test_data/test.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/prepare_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/prepare_image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/prepare_image/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/prepare_image/test_data/test.png
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/prepare_image/test_prepare_image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/text/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 15:10:32.000000 img2table-0.0.22/tests/tables/processing/text/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/text/test_data/ocr.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/text/test_data/table.json
--rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/text/test_data/test.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-07 15:08:38.000000 img2table-0.0.22/tests/tables/processing/text/test_titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-08 17:38:27.000000 img2table-0.0.23/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-08 17:38:27.000000 img2table-0.0.23/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-08 17:38:27.000000 img2table-0.0.23/.github/workflows/test_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-08 17:38:27.000000 img2table-0.0.23/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-08 17:38:27.000000 img2table-0.0.23/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-04-08 17:40:15.000000 img2table-0.0.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-04-08 17:38:27.000000 img2table-0.0.23/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-08 17:38:27.000000 img2table-0.0.23/activate_venv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    46045 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/Basic_usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    32897 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/Implicit_rows.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    18565 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/borderless.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    71022 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/data/borderless_aws.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   690012 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/data/borderless_ocr.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/data/tables.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/data/tables.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-04-08 17:38:27.000000 img2table-0.0.23/examples/data/tables.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-08 17:38:27.000000 img2table-0.0.23/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-08 17:38:27.000000 img2table-0.0.23/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-08 17:38:27.000000 img2table-0.0.23/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-08 17:38:27.000000 img2table-0.0.23/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-08 17:40:15.000000 img2table-0.0.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-08 17:38:27.000000 img2table-0.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/document/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/document/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/document/base/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/document/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/document/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/aws_textract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/google_vision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/paddle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/ocr/tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/objects/cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/objects/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/objects/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/objects/row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/objects/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/cells/deduplication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/cells/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8978 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/column_delimiters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5976 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/table/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/borderless_tables/table/table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-08 17:38:27.000000 img2table-0.0.23/src/img2table/tables/processing/text/titles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-08 17:40:15.000000 img2table-0.0.23/src/img2table.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/_mock_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11590 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/_mock_data/azure.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)    12108 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/_mock_data/tesseract_hocr.html
+-rw-r--r--   0 runner    (1001) docker     (123)    48862 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/_mock_data/textract.json
+-rw-r--r--   0 runner    (1001) docker     (123)    61360 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/_mock_data/vision.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/_mock_data/vision.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/document/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/document/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/document/base/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/base/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/base/test_rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/document/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/document/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/image/test_data/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6176 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/image/test_data/expected.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/image/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/document/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/document/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/document/pdf/test_pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/aws_textract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/aws_textract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/aws_textract/test_aws_textract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/aws_textract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/aws_textract/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/aws_textract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/aws_textract/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/azure/test_azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/azure/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/azure/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/azure/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/data/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/data/test_data/expected_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53989 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/data/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/data/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/data/test_ocr_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/google_vision/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/google_vision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/google_vision/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/google_vision/test_data/expected_content.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/google_vision/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/google_vision/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/google_vision/test_google_vision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/paddle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/paddle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/paddle/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/paddle/test_data/hocr.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/paddle/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/paddle/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/paddle/test_paddle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/pdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/pdf/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    35369 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/pdf/test_data/content.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/pdf/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   170804 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/pdf/test_data/test.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/pdf/test_pdf_ocr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/tesseract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/tesseract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/ocr/tesseract/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/tesseract/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/tesseract/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/ocr/tesseract/test_tesseract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/image/test_data/expected_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/image/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/image/test_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/objects/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/test_data/expected_tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/test_data/tables.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/test_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/test_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/test_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/objects/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/expected_ident_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/expected_potential_cells.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/expected_vertical_dedup.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_identification_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)    16285 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/implicit.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/implicit_ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/implicit_table.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/word_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_table_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/column_delimiters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/column_delimiters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/lines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/lines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/lines/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/lines/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/lines/test_lines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_data/ocr_df.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    20129 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/table/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/table/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/borderless_tables/table/test_table_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/common/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/common/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    29496 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/common/test_data/test.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/prepare_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/prepare_image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/prepare_image/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    20769 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/prepare_image/test_data/test.png
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/prepare_image/test_prepare_image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/text/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 17:40:15.000000 img2table-0.0.23/tests/tables/processing/text/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17822 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/text/test_data/ocr.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/text/test_data/table.json
+-rw-r--r--   0 runner    (1001) docker     (123)   219573 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/text/test_data/test.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-08 17:38:27.000000 img2table-0.0.23/tests/tables/processing/text/test_titles.py
```

### Comparing `img2table-0.0.22/LICENSE.txt` & `img2table-0.0.23/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/Makefile` & `img2table-0.0.23/Makefile`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/PKG-INFO` & `img2table-0.0.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 0.0.22
+Version: 0.0.23
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 0.0.22 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 0.0.23 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
```

### Comparing `img2table-0.0.22/README.md` & `img2table-0.0.23/README.md`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/examples/Basic_usage.ipynb` & `img2table-0.0.23/examples/Basic_usage.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/examples/Implicit_rows.ipynb` & `img2table-0.0.23/examples/Implicit_rows.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/examples/borderless.ipynb` & `img2table-0.0.23/examples/borderless.ipynb`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/examples/data/borderless_aws.jpg` & `img2table-0.0.23/examples/data/borderless_aws.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/examples/data/borderless_ocr.jpg` & `img2table-0.0.23/examples/data/borderless_ocr.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/examples/data/implicit.png` & `img2table-0.0.23/examples/data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/examples/data/tables.pdf` & `img2table-0.0.23/examples/data/tables.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/examples/data/tables.png` & `img2table-0.0.23/examples/data/tables.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/examples/data/tables.xlsx` & `img2table-0.0.23/examples/data/tables.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/setup.cfg` & `img2table-0.0.23/setup.cfg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/__init__.py` & `img2table-0.0.23/src/img2table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/document/base/__init__.py` & `img2table-0.0.23/src/img2table/document/base/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/document/base/rotation.py` & `img2table-0.0.23/src/img2table/document/base/rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/document/image.py` & `img2table-0.0.23/src/img2table/document/image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/document/pdf.py` & `img2table-0.0.23/src/img2table/document/pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/ocr/aws_textract.py` & `img2table-0.0.23/src/img2table/ocr/aws_textract.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,10 +93,10 @@
         Convert list of OCR elements by page to OCRDataframe object
         :param content: list of OCR elements by page
         :return: OCRDataframe object corresponding to content
         """
         list_dfs = list()
         for page_elements in content:
             if page_elements:
-                list_dfs.append(pl.from_dicts(page_elements))
+                list_dfs.append(pl.LazyFrame(data=page_elements))
 
-        return OCRDataframe(df=pl.concat(list_dfs).lazy()) if list_dfs else None
+        return OCRDataframe(df=pl.concat(list_dfs)) if list_dfs else None
```

### Comparing `img2table-0.0.22/src/img2table/ocr/azure.py` & `img2table-0.0.23/src/img2table/ocr/azure.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,10 +103,10 @@
                             "y1": min(bbox[1::2]),
                             "y2": max(bbox[1::2])
                         }
 
                         word_elements.append(d_word)
 
             if word_elements:
-                list_dfs.append(pl.from_dicts(word_elements))
+                list_dfs.append(pl.LazyFrame(data=word_elements))
 
-        return OCRDataframe(df=pl.concat(list_dfs).lazy()) if list_dfs else None
+        return OCRDataframe(df=pl.concat(list_dfs)) if list_dfs else None
```

### Comparing `img2table-0.0.22/src/img2table/ocr/base.py` & `img2table-0.0.23/src/img2table/ocr/base.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/ocr/data.py` & `img2table-0.0.23/src/img2table/ocr/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         # Filter dataframe on relevant words
         df_words = df_words.filter(pl.col('value').is_not_null() & (pl.col('confidence') >= min_confidence))
 
         # Create dataframe containing all coordinates of Cell objects
         list_cells = [{"row": id_row, "col": id_col, "x1_w": cell.x1, "x2_w": cell.x2, "y1_w": cell.y1, "y2_w": cell.y2}
                       for id_row, row in enumerate(table.items)
                       for id_col, cell in enumerate(row.items)]
-        df_cells = pl.from_dicts(dicts=list_cells).lazy()
+        df_cells = pl.LazyFrame(data=list_cells)
 
         # Cartesian product between two dataframes
         df_word_cells = df_words.join(other=df_cells, how="cross")
 
         # Compute coordinates of intersection
         df_word_cells = df_word_cells.with_columns([pl.max([pl.col('x1'), pl.col('x1_w')]).alias('x_left'),
                                                     pl.max([pl.col('y1'), pl.col('y1_w')]).alias('y_top'),
```

### Comparing `img2table-0.0.22/src/img2table/ocr/google_vision.py` & `img2table-0.0.23/src/img2table/ocr/google_vision.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,10 +242,10 @@
         Convert list of OCR elements by page to OCRDataframe object
         :param content: list of OCR elements by page
         :return: OCRDataframe object corresponding to content
         """
         list_dfs = list()
         for page_elements in content:
             if page_elements:
-                list_dfs.append(pl.from_dicts(page_elements))
+                list_dfs.append(pl.LazyFrame(data=page_elements))
 
-        return OCRDataframe(df=pl.concat(list_dfs).lazy()) if list_dfs else None
+        return OCRDataframe(df=pl.concat(list_dfs)) if list_dfs else None
```

### Comparing `img2table-0.0.22/src/img2table/ocr/paddle.py` & `img2table-0.0.23/src/img2table/ocr/paddle.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,8 +87,8 @@
                     "y1": round(min([edge[1] for edge in bbox])),
                     "x2": round(max([edge[0] for edge in bbox])),
                     "y2": round(max([edge[1] for edge in bbox]))
                 }
 
                 list_elements.append(dict_word)
 
-        return OCRDataframe(df=pl.from_dicts(list_elements).lazy()) if list_elements else None
+        return OCRDataframe(df=pl.LazyFrame(list_elements)) if list_elements else None
```

### Comparing `img2table-0.0.22/src/img2table/ocr/pdf.py` & `img2table-0.0.23/src/img2table/ocr/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,10 +67,10 @@
         if min(map(len, content)) == 0:
             return None
 
         # Create OCRDataframe
         list_dfs = list()
         for page_elements in content:
             if page_elements:
-                list_dfs.append(pl.from_dicts(page_elements))
+                list_dfs.append(pl.LazyFrame(data=page_elements))
 
-        return OCRDataframe(df=pl.concat(list_dfs).lazy()) if list_dfs else None
+        return OCRDataframe(df=pl.concat(list_dfs)) if list_dfs else None
```

### Comparing `img2table-0.0.22/src/img2table/ocr/tesseract.py` & `img2table-0.0.23/src/img2table/ocr/tesseract.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,10 +133,10 @@
                 d_el["x1"], d_el["y1"], d_el["x2"], d_el["y2"] = tuple(
                     int(element) for element in re.sub(r"^bbox\s", "", bbox).split())
 
                 list_elements.append(d_el)
 
             # Create dataframe
             if list_elements:
-                list_dfs.append(pl.from_dicts(list_elements))
+                list_dfs.append(pl.LazyFrame(data=list_elements))
 
-        return OCRDataframe(df=pl.concat(list_dfs).lazy()) if list_dfs else None
+        return OCRDataframe(df=pl.concat(list_dfs)) if list_dfs else None
```

### Comparing `img2table-0.0.22/src/img2table/tables/image.py` & `img2table-0.0.23/src/img2table/tables/image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/objects/__init__.py` & `img2table-0.0.23/src/img2table/tables/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/objects/extraction.py` & `img2table-0.0.23/src/img2table/tables/objects/extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/objects/line.py` & `img2table-0.0.23/src/img2table/tables/objects/line.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/objects/row.py` & `img2table-0.0.23/src/img2table/tables/objects/row.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/objects/table.py` & `img2table-0.0.23/src/img2table/tables/objects/table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/bordered_tables/cells/__init__.py` & `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/cells/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/bordered_tables/cells/deduplication.py` & `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/cells/deduplication.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/bordered_tables/cells/identification.py` & `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/cells/identification.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,16 +72,16 @@
     :return: dataframe containing all cells
     """
     # Check for empty lines
     if len(horizontal_lines) * len(vertical_lines) == 0:
         return pl.DataFrame().lazy()
 
     # Create dataframe from horizontal and vertical lines
-    df_h_lines = pl.from_dicts([l.dict for l in horizontal_lines]).lazy()
-    df_v_lines = pl.from_dicts([l.dict for l in vertical_lines]).lazy()
+    df_h_lines = pl.LazyFrame(data=[l.dict for l in horizontal_lines])
+    df_v_lines = pl.LazyFrame(data=[l.dict for l in vertical_lines])
 
     # Identify potential cells bboxes from horizontal lines
     df_bbox = get_potential_cells_from_h_lines(df_h_lines=df_h_lines)
 
     # Cross join with vertical lines
     df_bbox = df_bbox.with_columns(pl.max([(pl.col('x2_bbox') - pl.col('x1_bbox')) * 0.025,
                                            pl.lit(5.0)]).round(0).alias('h_margin')
```

### Comparing `img2table-0.0.22/src/img2table/tables/processing/bordered_tables/lines.py` & `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,16 +126,15 @@
                 )
 
     # If there are no lines or no words, do nothing
     if len(lines) == 0 or df_words.collect().height == 0:
         return lines
 
     # Create dataframe containing lines
-    df_lines = (pl.from_dicts(dicts=[line.dict for line in lines])
-                .lazy()
+    df_lines = (pl.LazyFrame(data=[line.dict for line in lines])
                 .with_columns([pl.max([pl.col('width'), pl.col('height')]).alias('length'),
                                (pl.col('x1') == pl.col('x2')).alias('vertical')]
                               )
                 .with_row_count(name="line_id")
                 .rename({"x1": "x1_line", "x2": "x2_line", "y1": "y1_line", "y2": "y2_line"})
                 )
```

### Comparing `img2table-0.0.22/src/img2table/tables/processing/bordered_tables/tables/__init__.py` & `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py` & `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py` & `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/implicit_rows.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/bordered_tables/tables/table_creation.py` & `img2table-0.0.23/src/img2table/tables/processing/bordered_tables/tables/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/borderless_tables/__init__.py` & `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/borderless_tables/column_delimiters.py` & `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/borderless_tables/lines.py` & `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/lines.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/borderless_tables/model.py` & `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/model.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/borderless_tables/segment_image.py` & `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/segment_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/borderless_tables/table/__init__.py` & `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/table/__init__.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/borderless_tables/table/headers.py` & `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/table/headers.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/borderless_tables/table/table_creation.py` & `img2table-0.0.23/src/img2table/tables/processing/borderless_tables/table/table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/common.py` & `img2table-0.0.23/src/img2table/tables/processing/common.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/prepare_image.py` & `img2table-0.0.23/src/img2table/tables/processing/prepare_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table/tables/processing/text/titles.py` & `img2table-0.0.23/src/img2table/tables/processing/text/titles.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/src/img2table.egg-info/PKG-INFO` & `img2table-0.0.23/src/img2table.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: img2table
-Version: 0.0.22
+Version: 0.0.23
 Summary: img2table is a table identification and extraction Python Library for PDF and images, based on OpenCV image processing
 Home-page: https://github.com/xavctn/img2table
 Author: Xavier Canton
 License: MIT
 Description: # img2table
         
         `img2table` is a simple, easy to use, table identification and extraction Python Library based on [OpenCV](https://opencv.org/) image
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: img2table Version: 0.0.22 Summary: img2table is a
+Metadata-Version: 2.1 Name: img2table Version: 0.0.23 Summary: img2table is a
 table identification and extraction Python Library for PDF and images, based on
 OpenCV image processing Home-page: https://github.com/xavctn/img2table Author:
 Xavier Canton License: MIT Description: # img2table `img2table` is a simple,
 easy to use, table identification and extraction Python Library based on
 [OpenCV](https://opencv.org/) image processing that supports most common image
 file formats as well as PDF files. Thanks to its design, it provides a
 practical and lighter alternative to Neural Networks based solutions,
```

### Comparing `img2table-0.0.22/src/img2table.egg-info/SOURCES.txt` & `img2table-0.0.23/src/img2table.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/_mock_data/azure.pkl` & `img2table-0.0.23/tests/_mock_data/azure.pkl`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/_mock_data/tesseract_hocr.html` & `img2table-0.0.23/tests/_mock_data/tesseract_hocr.html`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/_mock_data/textract.json` & `img2table-0.0.23/tests/_mock_data/textract.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/_mock_data/vision.json` & `img2table-0.0.23/tests/_mock_data/vision.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/_mock_data/vision.pkl` & `img2table-0.0.23/tests/_mock_data/vision.pkl`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/conftest.py` & `img2table-0.0.23/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/document/base/test_data/test.png` & `img2table-0.0.23/tests/document/base/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/document/base/test_rotation.py` & `img2table-0.0.23/tests/document/base/test_rotation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/document/image/test_data/blank.png` & `img2table-0.0.23/tests/document/image/test_data/blank.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/document/image/test_data/expected.xlsx` & `img2table-0.0.23/tests/document/image/test_data/expected.xlsx`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/document/image/test_data/test.png` & `img2table-0.0.23/tests/document/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/document/image/test_image.py` & `img2table-0.0.23/tests/document/image/test_image.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/document/pdf/test_data/test.pdf` & `img2table-0.0.23/tests/document/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/document/pdf/test_pdf.py` & `img2table-0.0.23/tests/document/pdf/test_pdf.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/aws_textract/test_aws_textract.py` & `img2table-0.0.23/tests/ocr/aws_textract/test_aws_textract.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,24 +41,24 @@
 def test_to_ocr_df(mock_textract):
     ocr = TextractOCR()
     with open("test_data/content.json", "r") as f:
         content = json.load(f)
 
     result = ocr.to_ocr_dataframe(content=[content])
 
-    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     assert result == expected
 
 
 def test_textract_ocr(mock_textract):
     img = Image("test_data/test.png")
     ocr = TextractOCR(aws_access_key_id="aws_access_key_id",
                       aws_secret_access_key="aws_secret_access_key",
                       aws_session_token="aws_session_token",
                       region="eu-west-1")
 
     result = ocr.of(document=img)
 
-    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     assert result == expected
```

### Comparing `img2table-0.0.22/tests/ocr/aws_textract/test_data/content.json` & `img2table-0.0.23/tests/ocr/aws_textract/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/aws_textract/test_data/ocr_df.csv` & `img2table-0.0.23/tests/ocr/aws_textract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/aws_textract/test_data/test.png` & `img2table-0.0.23/tests/ocr/aws_textract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/azure/test_azure.py` & `img2table-0.0.23/tests/ocr/azure/test_azure.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 def test_to_ocr_df(mock_azure):
     ocr = AzureOCR(endpoint="aa", subscription_key="bb")
     with open(os.path.join(MOCK_DIR, "azure.pkl"), "rb") as f:
         content = pickle.load(f)
 
     result = ocr.to_ocr_dataframe(content=[content])
 
-    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     assert result == expected
 
 
 def test_azure_ocr(mock_azure):
     # Test init error
     with pytest.raises(TypeError) as e_info:
@@ -50,10 +50,10 @@
         AzureOCR(subscription_key="a")
 
     img = Image("test_data/test.png")
     ocr = AzureOCR(endpoint="aa", subscription_key="bb")
 
     result = ocr.of(document=img)
 
-    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     assert result == expected
```

### Comparing `img2table-0.0.22/tests/ocr/azure/test_data/ocr_df.csv` & `img2table-0.0.23/tests/ocr/azure/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/azure/test_data/test.png` & `img2table-0.0.23/tests/ocr/azure/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/data/test_data/expected_table.json` & `img2table-0.0.23/tests/ocr/data/test_data/expected_table.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/data/test_data/ocr_df.csv` & `img2table-0.0.23/tests/ocr/data/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/data/test_ocr_data.py` & `img2table-0.0.23/tests/ocr/data/test_ocr_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,46 +6,46 @@
 from img2table.ocr.data import OCRDataframe
 from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.row import Row
 from img2table.tables.objects.table import Table
 
 
 def test_text_sizes():
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     assert round(ocr_df.median_line_sep, 2) == 51.0
     assert round(ocr_df.char_length, 2) == 24.2
 
 
 def test_pages():
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     ocr_df_page_0 = ocr_df.page(page_number=0)
     ocr_df_page_1 = ocr_df.page(page_number=1)
 
     assert isinstance(ocr_df_page_0, OCRDataframe)
     assert isinstance(ocr_df_page_1, OCRDataframe)
 
     assert not ocr_df_page_0 == ocr_df_page_1
     assert len(ocr_df_page_0.df.collect()) + len(ocr_df_page_1.df.collect()) == len(ocr_df.df.collect())
 
 
 def test_get_text_cell():
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
     cell = Cell(x1=200, x2=800, y1=700, y2=850)
 
     result = ocr_df.get_text_cell(cell=cell,
                                   min_confidence=50,
                                   page_number=0)
 
     assert result == "Use these data to create\nChecklist for a Data Table."
 
 
 def test_get_text_table():
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     with open("test_data/table.json", "r") as f:
         table = Table(rows=[Row(cells=[Cell(**el) for el in row]) for row in json.load(f)])
 
     result = ocr_df.get_text_table(table=table,
                                    page_number=0,
                                    min_confidence=50)
```

### Comparing `img2table-0.0.22/tests/ocr/google_vision/test_data/expected_content.json` & `img2table-0.0.23/tests/ocr/google_vision/test_data/expected_content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/google_vision/test_data/ocr_df.csv` & `img2table-0.0.23/tests/ocr/google_vision/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/google_vision/test_data/test.png` & `img2table-0.0.23/tests/ocr/google_vision/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/google_vision/test_google_vision.py` & `img2table-0.0.23/tests/ocr/google_vision/test_google_vision.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 def test_vision_ocr(mock_vision):
     image = Image("test_data/test.png")
 
     with open("test_data/expected_content.json", "r") as f:
         content = json.load(f)
 
-    expected_ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    expected_ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     # Test init error
     with pytest.raises(TypeError) as e_info:
         VisionOCR(api_key=8)
 
     with pytest.raises(ValueError) as e_info:
         VisionOCR()
```

### Comparing `img2table-0.0.22/tests/ocr/paddle/test_data/hocr.json` & `img2table-0.0.23/tests/ocr/paddle/test_data/hocr.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/paddle/test_data/ocr_df.csv` & `img2table-0.0.23/tests/ocr/paddle/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/paddle/test_data/test.png` & `img2table-0.0.23/tests/ocr/paddle/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/paddle/test_paddle.py` & `img2table-0.0.23/tests/ocr/paddle/test_paddle.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,24 +56,24 @@
     instance = PaddleOCR()
 
     with open("test_data/hocr.json", "r") as f:
         content = [[[element[0], tuple(element[1])] for element in json.load(f)]]
 
     result = instance.to_ocr_dataframe(content=content)
 
-    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     assert result == expected
 
 
 @pytest.mark.skipif(sys.version_info >= (3, 11), reason="No support for PaddleOCR")
 def test_paddle_document():
     from img2table.ocr import PaddleOCR
 
     instance = PaddleOCR()
     doc = Image(src="test_data/test.png")
 
     result = instance.of(document=doc)
 
-    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     assert result == expected
```

### Comparing `img2table-0.0.22/tests/ocr/pdf/test_data/content.json` & `img2table-0.0.23/tests/ocr/pdf/test_data/content.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/pdf/test_data/ocr_df.csv` & `img2table-0.0.23/tests/ocr/pdf/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/pdf/test_data/test.pdf` & `img2table-0.0.23/tests/ocr/pdf/test_data/test.pdf`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/pdf/test_pdf_ocr.py` & `img2table-0.0.23/tests/ocr/pdf/test_pdf_ocr.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,23 +24,23 @@
     instance = PdfOCR()
 
     with open("test_data/content.json", "r") as f:
         content = json.load(f)
 
     result = instance.to_ocr_dataframe(content=content)
 
-    df_expected = pl.read_csv("test_data/ocr_df.csv", sep=";").lazy()
+    df_expected = pl.read_csv("test_data/ocr_df.csv", separator=";").lazy()
     expected = OCRDataframe(df=df_expected)
 
     assert result == expected
 
 
 def test_pdf_document():
     instance = PdfOCR()
     doc = PDF(src="test_data/test.pdf", dpi=300)
 
     result = instance.of(document=doc)
 
-    df_expected = pl.read_csv("test_data/ocr_df.csv", sep=";").lazy()
+    df_expected = pl.read_csv("test_data/ocr_df.csv", separator=";").lazy()
     expected = OCRDataframe(df=df_expected)
 
     assert result == expected
```

### Comparing `img2table-0.0.22/tests/ocr/tesseract/test_data/ocr_df.csv` & `img2table-0.0.23/tests/ocr/tesseract/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/tesseract/test_data/test.png` & `img2table-0.0.23/tests/ocr/tesseract/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/ocr/tesseract/test_tesseract.py` & `img2table-0.0.23/tests/ocr/tesseract/test_tesseract.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,21 +57,21 @@
     instance = TesseractOCR()
 
     with open(os.path.join(MOCK_DIR, "tesseract_hocr.html"), 'r') as f:
         content = [f.read()]
 
     result = instance.to_ocr_dataframe(content=content)
 
-    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     assert result == expected
 
 
 def test_tesseract_document(mock_tesseract):
     instance = TesseractOCR()
     doc = Image(src="test_data/test.png")
 
     result = instance.of(document=doc)
 
-    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    expected = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     assert result == expected
```

### Comparing `img2table-0.0.22/tests/tables/image/test_data/expected_tables.json` & `img2table-0.0.23/tests/tables/image/test_data/expected_tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/image/test_data/ocr.csv` & `img2table-0.0.23/tests/tables/image/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/image/test_data/test.png` & `img2table-0.0.23/tests/tables/image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/image/test_image.py` & `img2table-0.0.23/tests/tables/image/test_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from img2table.tables.objects.cell import Cell
 from img2table.tables.objects.row import Row
 from img2table.tables.objects.table import Table
 
 
 def test_table_image():
     image = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(pl.read_csv("test_data/ocr.csv", sep=";", encoding="utf-8").lazy())
+    ocr_df = OCRDataframe(pl.read_csv("test_data/ocr.csv", separator=";", encoding="utf-8").lazy())
 
     tb_image = TableImage(img=image,
                           dpi=200,
                           ocr_df=ocr_df,
                           min_confidence=50)
 
     result = tb_image.extract_tables(implicit_rows=True)
```

### Comparing `img2table-0.0.22/tests/tables/objects/test_data/expected_tables.json` & `img2table-0.0.23/tests/tables/objects/test_data/expected_tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/objects/test_data/ocr.csv` & `img2table-0.0.23/tests/tables/objects/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/objects/test_data/tables.json` & `img2table-0.0.23/tests/tables/objects/test_data/tables.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/objects/test_extraction.py` & `img2table-0.0.23/tests/tables/objects/test_extraction.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/objects/test_line.py` & `img2table-0.0.23/tests/tables/objects/test_line.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/objects/test_row.py` & `img2table-0.0.23/tests/tables/objects/test_row.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/objects/test_table.py` & `img2table-0.0.23/tests/tables/objects/test_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 def test_get_table_content():
     with open("test_data/tables.json", "r") as f:
         tables = [Table(rows=[Row(cells=[Cell(**el) for el in row]) for row in tb])
                   for tb in json.load(f)]
 
     # Load OCR
-    ocr_df = OCRDataframe(pl.read_csv("test_data/ocr.csv", sep=";", encoding="utf-8").lazy())
+    ocr_df = OCRDataframe(pl.read_csv("test_data/ocr.csv", separator=";", encoding="utf-8").lazy())
 
     result = [table.get_content(ocr_df=ocr_df, min_confidence=50) for table in tables]
 
     with open("test_data/expected_tables.json", "r") as f:
         expected = [Table(rows=[Row(cells=[Cell(**el) for el in row]) for row in tb])
                     for tb in json.load(f)]
```

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/cells/test_cells.py` & `img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_cells.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,12 +13,12 @@
         data = json.load(f)
     h_lines = [Line(**el) for el in data.get('h_lines')]
     v_lines = [Line(**el) for el in data.get('v_lines')]
 
     result = get_cells(horizontal_lines=h_lines,
                        vertical_lines=v_lines)
 
-    df_expected = pl.read_csv("test_data/expected.csv", sep=";", encoding="utf-8")
+    df_expected = pl.read_csv("test_data/expected.csv", separator=";", encoding="utf-8")
     expected = [Cell(x1=row["x1"], x2=row["x2"], y1=row["y1"], y2=row["y2"])
                 for row in df_expected.to_dicts()]
 
     assert result == expected
```

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/cells/test_data/expected.csv` & `img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/expected.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/cells/test_data/lines.json` & `img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py` & `img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_deduplication_cells.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import polars as pl
 
 from img2table.tables.processing.bordered_tables.cells.deduplication import deduplicate_nested_cells, \
     deduplicate_cells
 
 
 def test_deduplicate_nested_cells():
-    df_cells = pl.read_csv("test_data/expected_ident_cells.csv", sep=";", encoding="utf-8").lazy()
+    df_cells = pl.read_csv("test_data/expected_ident_cells.csv", separator=";", encoding="utf-8").lazy()
 
     result = deduplicate_nested_cells(df_cells=df_cells).collect()
-    expected = pl.read_csv("test_data/expected.csv", sep=";", encoding="utf-8")
+    expected = pl.read_csv("test_data/expected.csv", separator=";", encoding="utf-8")
 
     assert result.frame_equal(expected)
 
 
 def test_deduplicate_cells():
-    df_cells = pl.read_csv("test_data/expected_ident_cells.csv", sep=";", encoding="utf-8").lazy()
+    df_cells = pl.read_csv("test_data/expected_ident_cells.csv", separator=";", encoding="utf-8").lazy()
 
     result = deduplicate_cells(df_cells=df_cells).collect()
-    expected = pl.read_csv("test_data/expected.csv", sep=";", encoding="utf-8")
+    expected = pl.read_csv("test_data/expected.csv", separator=";", encoding="utf-8")
 
     assert result.frame_equal(expected)
```

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/cells/test_identification_cells.py` & `img2table-0.0.23/tests/tables/processing/bordered_tables/cells/test_identification_cells.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,23 +13,23 @@
         data = json.load(f)
     h_lines = [Line(**el) for el in data.get('h_lines')]
 
     df_h_lines = pl.from_dicts([l.dict for l in h_lines]).lazy()
 
     result = get_potential_cells_from_h_lines(df_h_lines=df_h_lines).collect()
 
-    expected = pl.read_csv("test_data/expected_potential_cells.csv", sep=";", encoding="utf-8")
+    expected = pl.read_csv("test_data/expected_potential_cells.csv", separator=";", encoding="utf-8")
 
     assert result.frame_equal(expected)
 
 
 def test_get_cells_dataframe():
     with open("test_data/lines.json", 'r') as f:
         data = json.load(f)
     h_lines = [Line(**el) for el in data.get('h_lines')]
     v_lines = [Line(**el) for el in data.get('v_lines')]
 
     result = get_cells_dataframe(horizontal_lines=h_lines,
                                  vertical_lines=v_lines).collect()
-    expected = pl.read_csv("test_data/expected_ident_cells.csv", sep=";", encoding="utf-8")
+    expected = pl.read_csv("test_data/expected_ident_cells.csv", separator=";", encoding="utf-8")
 
     assert result.frame_equal(expected.sort(['x1', 'y1', 'x2', 'y2']))
```

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/lines/test_data/expected.json` & `img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/lines/test_data/ocr.csv` & `img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/lines/test_data/test.png` & `img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/lines/test_lines.py` & `img2table-0.0.23/tests/tables/processing/bordered_tables/lines/test_lines.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,26 +22,26 @@
                 Line(x1=12, x2=12, y1=210, y2=255, thickness=1),
                 Line(x1=20, x2=20, y1=10, y2=100, thickness=1)]
 
     assert result == expected
 
 
 def test_remove_word_lines():
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr.csv", separator=";").lazy())
     lines = [Line(x1=10, x2=10, y1=10, y2=100),
              Line(x1=975, x2=975, y1=40, y2=60)]
 
     result = remove_word_lines(lines=lines, ocr_df=ocr_df)
 
     assert result == [Line(x1=10, x2=10, y1=10, y2=100)]
 
 
 def test_detect_lines():
     img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr.csv", separator=";").lazy())
 
     h_lines, v_lines = detect_lines(image=img,
                                     rho=0.3,
                                     threshold=10,
                                     minLinLength=10,
                                     maxLineGap=10,
                                     ocr_df=ocr_df)
```

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py` & `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_cell_clustering.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json` & `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/cell_clusters_normalized.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/cells.json` & `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/cells.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json` & `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/cells_clustered.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/expected.json` & `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/expected.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/implicit.png` & `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/implicit.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/implicit_ocr_df.csv` & `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/implicit_ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json` & `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/tables_from_cells.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_data/word_image.png` & `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_data/word_image.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py` & `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_implicit_rows.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from img2table.tables.objects.table import Table
 from img2table.tables.processing.bordered_tables.tables.implicit_rows import create_word_image, \
     handle_implicit_rows_table, handle_implicit_rows
 
 
 def test_create_word_image():
     img = cv2.imread("test_data/implicit.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/implicit_ocr_df.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/implicit_ocr_df.csv", separator=";").lazy())
 
     result = create_word_image(img=img, ocr_df=ocr_df)
 
     expected = cv2.imread("test_data/word_image.png", cv2.IMREAD_GRAYSCALE)
 
     assert np.array_equal(result, expected)
 
@@ -34,15 +34,15 @@
 
     # Check that 2 more lines have been created
     assert result.nb_rows == table.nb_rows + 2
 
 
 def test_handle_implicit_rows():
     img = cv2.imread("test_data/implicit.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/implicit_ocr_df.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/implicit_ocr_df.csv", separator=";").lazy())
 
     with open("test_data/implicit_table.json", 'r') as f:
         table = Table(rows=[Row(cells=[Cell(**el) for el in row]) for row in json.load(f)])
 
     result = handle_implicit_rows(img=img, tables=[table], ocr_df=ocr_df)
 
     # Check that 2 more lines have been created
```

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_table_creation.py` & `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/bordered_tables/tables/test_tables.py` & `img2table-0.0.23/tests/tables/processing/bordered_tables/tables/test_tables.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py` & `img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_borderless_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from img2table.ocr.data import OCRDataframe
 from img2table.tables.objects.line import Line
 from img2table.tables.processing.borderless_tables import identify_borderless_tables
 
 
 def test_identify_borderless_tables():
     img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     with open("test_data/lines.json", 'r') as f:
         data = json.load(f)
     lines = [Line(**el) for el in data.get('h_lines') + data.get('v_lines')]
 
     result = identify_borderless_tables(img=img,
                                         ocr_df=ocr_df,
```

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json` & `img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/borderless_table/test_data/ocr_df.csv` & `img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png` & `img2table-0.0.23/tests/tables/processing/borderless_tables/borderless_table/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py` & `img2table-0.0.23/tests/tables/processing/borderless_tables/column_delimiters/test_column_delimiters.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json` & `img2table-0.0.23/tests/tables/processing/borderless_tables/lines/test_data/image_segment.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/lines/test_data/ocr_df.csv` & `img2table-0.0.23/tests/tables/processing/borderless_tables/lines/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/lines/test_lines.py` & `img2table-0.0.23/tests/tables/processing/borderless_tables/lines/test_lines.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,27 +63,27 @@
                          TableLine(cells=[Cell(x1=0, x2=20, y1=63, y2=73), Cell(x1=20, x2=40, y1=63, y2=73)])])
     ]
 
     assert result == expected
 
 
 def test_is_text_block():
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     line_group = LineGroup(lines=[TableLine(cells=[Cell(x1=0, x2=20, y1=0, y2=10), Cell(x1=20, x2=40, y1=0, y2=10)]),
                                   TableLine(cells=[Cell(x1=0, x2=20, y1=13, y2=23), Cell(x1=20, x2=40, y1=13, y2=23)])])
     assert is_text_block(line_group=line_group, ocr_df=ocr_df)
 
     line_group = LineGroup(lines=[TableLine(cells=[Cell(x1=0, x2=20, y1=0, y2=10), Cell(x1=40, x2=60, y1=0, y2=10)]),
                                   TableLine(cells=[Cell(x1=0, x2=20, y1=13, y2=23), Cell(x1=40, x2=60, y1=13, y2=23)])])
     assert not is_text_block(line_group=line_group, ocr_df=ocr_df)
 
 
 def test_identify_line_groups():
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     with open("test_data/image_segment.json", "r") as f:
         data = json.load(f)
     img_segment = ImageSegment(x1=data.get('x1'),
                                y1=data.get('y1'),
                                x2=data.get('x2'),
                                y2=data.get('y2'),
```

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json` & `img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_data/lines.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/segment_image/test_data/ocr_df.csv` & `img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_data/ocr_df.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/segment_image/test_data/test.png` & `img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py` & `img2table-0.0.23/tests/tables/processing/borderless_tables/segment_image/test_segment_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 from img2table.tables.processing.borderless_tables.model import ImageSegment
 from img2table.tables.processing.borderless_tables.segment_image import create_image_segments, get_segment_elements, \
     segment_image
 
 
 def test_create_image_segments():
     img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
 
     result = create_image_segments(img=img, ocr_df=ocr_df)
 
     assert result == [ImageSegment(x1=2, y1=0, x2=804, y2=361), ImageSegment(x1=928, y1=0, x2=1188, y2=157)]
 
 
 def test_get_segment_elements():
     img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
     img_segments = [ImageSegment(x1=2, y1=0, x2=804, y2=361),
                     ImageSegment(x1=928, y1=0, x2=1188, y2=157)]
 
     with open("test_data/lines.json", 'r') as f:
         data = json.load(f)
     lines = [Line(**el) for el in data.get('h_lines') + data.get('v_lines')]
 
@@ -38,15 +38,15 @@
 
     assert len(result[0].elements) == 14
     assert len(result[1].elements) == 4
 
 
 def test_segment_image():
     img = cv2.imread("test_data/test.png", cv2.IMREAD_GRAYSCALE)
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr_df.csv", separator=";").lazy())
     with open("test_data/lines.json", 'r') as f:
         data = json.load(f)
     lines = [Line(**el) for el in data.get('h_lines') + data.get('v_lines')]
 
     result = segment_image(img=img,
                            ocr_df=ocr_df,
                            lines=lines)
```

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/table/test_headers.py` & `img2table-0.0.23/tests/tables/processing/borderless_tables/table/test_headers.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/table/test_table.py` & `img2table-0.0.23/tests/tables/processing/borderless_tables/table/test_table.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/borderless_tables/table/test_table_creation.py` & `img2table-0.0.23/tests/tables/processing/borderless_tables/table/test_table_creation.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/common/test_common.py` & `img2table-0.0.23/tests/tables/processing/common/test_common.py`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/common/test_data/test.jpg` & `img2table-0.0.23/tests/tables/processing/common/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/prepare_image/test_data/test.png` & `img2table-0.0.23/tests/tables/processing/prepare_image/test_data/test.png`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/text/test_data/ocr.csv` & `img2table-0.0.23/tests/tables/processing/text/test_data/ocr.csv`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/text/test_data/table.json` & `img2table-0.0.23/tests/tables/processing/text/test_data/table.json`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/text/test_data/test.jpg` & `img2table-0.0.23/tests/tables/processing/text/test_data/test.jpg`

 * *Files identical despite different names*

### Comparing `img2table-0.0.22/tests/tables/processing/text/test_titles.py` & `img2table-0.0.23/tests/tables/processing/text/test_titles.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 from img2table.tables.processing.text.titles import get_title_tables
 
 
 def test_get_title_tables():
     img = cv2.imread("test_data/test.jpg", cv2.IMREAD_GRAYSCALE)
     with open("test_data/table.json", "r") as f:
         table = Table(rows=[Row(cells=[Cell(**el) for el in row]) for row in json.load(f)])
-    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr.csv", sep=";").lazy())
+    ocr_df = OCRDataframe(df=pl.read_csv("test_data/ocr.csv", separator=";").lazy())
 
     result = get_title_tables(img=img, tables=[table], ocr_df=ocr_df)
 
     assert result[0].title == "10 most populous countries"
     assert get_title_tables(img=img, tables=[], ocr_df=ocr_df) == []
```

