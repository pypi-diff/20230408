# Comparing `tmp/rexify-0.1.4.tar.gz` & `tmp/rexify-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rexify-0.1.4.tar", max compression
+gzip compressed data, was "rexify-0.1.5.tar", max compression
```

## Comparing `rexify-0.1.4.tar` & `rexify-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1071 2023-04-07 23:32:59.495901 rexify-0.1.4/LICENSE
--rw-r--r--   0        0        0     4845 2023-04-07 23:32:59.495901 rexify-0.1.4/README.md
--rw-r--r--   0        0        0     2831 2023-04-07 23:33:01.939907 rexify-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      136 2023-04-07 23:32:59.495901 rexify-0.1.4/rexify/__init__.py
--rw-r--r--   0        0        0     3231 2023-04-07 23:32:59.495901 rexify-0.1.4/rexify/data.py
--rw-r--r--   0        0        0        0 2023-04-07 23:32:59.495901 rexify-0.1.4/rexify/features/__init__.py
--rw-r--r--   0        0        0     2565 2023-04-07 23:32:59.495901 rexify-0.1.4/rexify/features/base.py
--rw-r--r--   0        0        0     4165 2023-04-07 23:32:59.495901 rexify-0.1.4/rexify/features/extractor.py
--rw-r--r--   0        0        0      206 2023-04-07 23:32:59.495901 rexify-0.1.4/rexify/features/transform/__init__.py
--rw-r--r--   0        0        0      399 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/features/transform/category.py
--rw-r--r--   0        0        0      346 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/features/transform/custom.py
--rw-r--r--   0        0        0     3988 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/features/transform/entity.py
--rw-r--r--   0        0        0     1130 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/features/transform/event.py
--rw-r--r--   0        0        0     1809 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/features/transform/id.py
--rw-r--r--   0        0        0      402 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/features/transform/number.py
--rw-r--r--   0        0        0     4398 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/features/transform/sequence.py
--rw-r--r--   0        0        0       37 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/__init__.py
--rw-r--r--   0        0        0      807 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/base.py
--rw-r--r--   0        0        0       38 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/callbacks/__init__.py
--rw-r--r--   0        0        0     1310 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/callbacks/index.py
--rw-r--r--   0        0        0      721 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/index.py
--rw-r--r--   0        0        0     1358 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/lookup.py
--rw-r--r--   0        0        0       34 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/ranking/__init__.py
--rw-r--r--   0        0        0      624 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/ranking/base.py
--rw-r--r--   0        0        0      619 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/ranking/event.py
--rw-r--r--   0        0        0     1778 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/ranking/ranking.py
--rw-r--r--   0        0        0     4850 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/recommender.py
--rw-r--r--   0        0        0       38 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/retrieval/__init__.py
--rw-r--r--   0        0        0     1838 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/retrieval/candidate.py
--rw-r--r--   0        0        0     3032 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/retrieval/query.py
--rw-r--r--   0        0        0     2131 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/retrieval/retrieval.py
--rw-r--r--   0        0        0     2293 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/retrieval/tower.py
--rw-r--r--   0        0        0     2011 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/models/sequential.py
--rw-r--r--   0        0        0     2686 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/schema.py
--rw-r--r--   0        0        0      676 2023-04-07 23:32:59.499901 rexify-0.1.4/rexify/utils.py
--rw-r--r--   0        0        0     6150 1970-01-01 00:00:00.000000 rexify-0.1.4/setup.py
--rw-r--r--   0        0        0     6528 1970-01-01 00:00:00.000000 rexify-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-08 21:51:51.982510 rexify-0.1.5/LICENSE
+-rw-r--r--   0        0        0     4845 2023-04-08 21:51:51.982510 rexify-0.1.5/README.md
+-rw-r--r--   0        0        0     2831 2023-04-08 21:51:54.082506 rexify-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      136 2023-04-08 21:51:51.982510 rexify-0.1.5/rexify/__init__.py
+-rw-r--r--   0        0        0     3641 2023-04-08 21:51:51.982510 rexify-0.1.5/rexify/data.py
+-rw-r--r--   0        0        0        0 2023-04-08 21:51:51.982510 rexify-0.1.5/rexify/features/__init__.py
+-rw-r--r--   0        0        0     2565 2023-04-08 21:51:51.982510 rexify-0.1.5/rexify/features/base.py
+-rw-r--r--   0        0        0     4165 2023-04-08 21:51:51.982510 rexify-0.1.5/rexify/features/extractor.py
+-rw-r--r--   0        0        0      206 2023-04-08 21:51:51.982510 rexify-0.1.5/rexify/features/transform/__init__.py
+-rw-r--r--   0        0        0      399 2023-04-08 21:51:51.982510 rexify-0.1.5/rexify/features/transform/category.py
+-rw-r--r--   0        0        0      346 2023-04-08 21:51:51.982510 rexify-0.1.5/rexify/features/transform/custom.py
+-rw-r--r--   0        0        0     3988 2023-04-08 21:51:51.982510 rexify-0.1.5/rexify/features/transform/entity.py
+-rw-r--r--   0        0        0     1130 2023-04-08 21:51:51.982510 rexify-0.1.5/rexify/features/transform/event.py
+-rw-r--r--   0        0        0     1809 2023-04-08 21:51:51.982510 rexify-0.1.5/rexify/features/transform/id.py
+-rw-r--r--   0        0        0      402 2023-04-08 21:51:51.982510 rexify-0.1.5/rexify/features/transform/number.py
+-rw-r--r--   0        0        0     4398 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/features/transform/sequence.py
+-rw-r--r--   0        0        0       37 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/__init__.py
+-rw-r--r--   0        0        0      807 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/base.py
+-rw-r--r--   0        0        0       38 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/callbacks/__init__.py
+-rw-r--r--   0        0        0     1310 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/callbacks/index.py
+-rw-r--r--   0        0        0      721 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/index.py
+-rw-r--r--   0        0        0     1358 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/lookup.py
+-rw-r--r--   0        0        0       34 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/ranking/__init__.py
+-rw-r--r--   0        0        0      624 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/ranking/base.py
+-rw-r--r--   0        0        0      619 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/ranking/event.py
+-rw-r--r--   0        0        0     1778 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/ranking/ranking.py
+-rw-r--r--   0        0        0     4850 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/recommender.py
+-rw-r--r--   0        0        0       38 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/retrieval/__init__.py
+-rw-r--r--   0        0        0     1838 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/retrieval/candidate.py
+-rw-r--r--   0        0        0     3032 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/retrieval/query.py
+-rw-r--r--   0        0        0     2131 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/retrieval/retrieval.py
+-rw-r--r--   0        0        0     2293 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/retrieval/tower.py
+-rw-r--r--   0        0        0     2011 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/models/sequential.py
+-rw-r--r--   0        0        0     2686 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/schema.py
+-rw-r--r--   0        0        0      676 2023-04-08 21:51:51.986510 rexify-0.1.5/rexify/utils.py
+-rw-r--r--   0        0        0     6150 1970-01-01 00:00:00.000000 rexify-0.1.5/setup.py
+-rw-r--r--   0        0        0     6528 1970-01-01 00:00:00.000000 rexify-0.1.5/PKG-INFO
```

### Comparing `rexify-0.1.4/LICENSE` & `rexify-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/README.md` & `rexify-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/pyproject.toml` & `rexify-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rexify"
-version = "0.1.4"
+version = "0.1.5"
 description = "Streamlined Recommender System workflows with TensorFlow and Kubeflow"
 authors = ["José Medeiros <joseprsm@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://rexify.readthedocs.io"
 packages = [{ include = "rexify" }]
 classifiers = [
```

### Comparing `rexify-0.1.4/rexify/data.py` & `rexify-0.1.5/rexify/data.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import tensorflow as tf
+from sklearn.model_selection import train_test_split
 
 from rexify.features.base import HasSchemaMixin
 from rexify.schema import Schema
 from rexify.utils import get_target_id, make_dirs
 
 
 class DataFrame(pd.DataFrame, HasSchemaMixin):
@@ -16,14 +17,18 @@
         data: pd.DataFrame,
         schema: Schema,
         ranking_features: list[str] | None = None,
     ):
         super().__init__(data)
         HasSchemaMixin.__init__(self, schema)
         self._ranking_features = ranking_features
+        self._dataframe_args = {
+            "schema": self._schema,
+            "ranking_features": self._ranking_features,
+        }
 
     def save(self, path: str | Path, name: str = None):
         path = Path(path)
         path = path / name if name else path
 
         history = pd.DataFrame(np.stack(self.loc[:, "history"].values))
 
@@ -47,14 +52,20 @@
 
         schema = Schema.from_json(path / "schema.json")
         with open(path / "ranks.json", "r") as f:
             ranking_features = json.load(f)
 
         return DataFrame(features, schema=schema, ranking_features=ranking_features)
 
+    def split(self, **kwargs):
+        train, val = train_test_split(self, **kwargs)
+        train = DataFrame(train, **self._dataframe_args)
+        val = DataFrame(val, **self._dataframe_args)
+        return train, val
+
     def to_dataset(self) -> tf.data.Dataset:
         return self._make_dataset().map(self._get_header_fn())
 
     def _make_dataset(self) -> tf.data.Dataset:
         return tf.data.Dataset.zip(
             (
                 self._get_target_vector_dataset(self, self._schema, "user"),
```

### Comparing `rexify-0.1.4/rexify/features/base.py` & `rexify-0.1.5/rexify/features/base.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/features/extractor.py` & `rexify-0.1.5/rexify/features/extractor.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/features/transform/entity.py` & `rexify-0.1.5/rexify/features/transform/entity.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/features/transform/event.py` & `rexify-0.1.5/rexify/features/transform/event.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/features/transform/id.py` & `rexify-0.1.5/rexify/features/transform/id.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/features/transform/sequence.py` & `rexify-0.1.5/rexify/features/transform/sequence.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/models/base.py` & `rexify-0.1.5/rexify/models/base.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/models/callbacks/index.py` & `rexify-0.1.5/rexify/models/callbacks/index.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/models/index.py` & `rexify-0.1.5/rexify/models/index.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/models/lookup.py` & `rexify-0.1.5/rexify/models/lookup.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/models/ranking/base.py` & `rexify-0.1.5/rexify/models/ranking/base.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/models/ranking/event.py` & `rexify-0.1.5/rexify/models/ranking/event.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/models/ranking/ranking.py` & `rexify-0.1.5/rexify/models/ranking/ranking.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/models/recommender.py` & `rexify-0.1.5/rexify/models/recommender.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/models/retrieval/candidate.py` & `rexify-0.1.5/rexify/models/retrieval/candidate.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/models/retrieval/query.py` & `rexify-0.1.5/rexify/models/retrieval/query.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/models/retrieval/retrieval.py` & `rexify-0.1.5/rexify/models/retrieval/retrieval.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/models/retrieval/tower.py` & `rexify-0.1.5/rexify/models/retrieval/tower.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/models/sequential.py` & `rexify-0.1.5/rexify/models/sequential.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/schema.py` & `rexify-0.1.5/rexify/schema.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/rexify/utils.py` & `rexify-0.1.5/rexify/utils.py`

 * *Files identical despite different names*

### Comparing `rexify-0.1.4/setup.py` & `rexify-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 extras_require = \
 {':sys_platform != "darwin"': ['tensorflow==2.9.0', 'scann>=1.2.0,<2.0.0'],
  ':sys_platform == "darwin"': ['tensorflow_metal==0.5.0',
                                'tensorflow_macos==2.9.0']}
 
 setup_kwargs = {
     'name': 'rexify',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Streamlined Recommender System workflows with TensorFlow and Kubeflow',
     'long_description': '<p align="center">\n    <br>\n    <img src="https://storage.googleapis.com/rexify/1659986918545.png" height="200"/>\n    <br>\n<p>\n\n<p align="center">\n    <a href="https://circleci.com/gh/joseprsm/rexify">\n        <img alt="Build" src="https://img.shields.io/circleci/build/github/joseprsm/rexify?style=flat-square">\n    </a>\n    <a href="https://github.com/joseprsm/rexify/blob/main/LICENSE">\n        <img alt="License" src="https://img.shields.io/github/license/joseprsm/rexify?style=flat-square">\n    </a>\n    <a href="https://rexify.readthedocs.io">\n        <img alt="Documentation" src="https://img.shields.io/badge/documentation-online-success?style=flat-square">\n    </a>\n    <a href="https://pypi.org/project/rexify/">\n        <img alt="GitHub release" src="https://img.shields.io/github/v/release/joseprsm/rexify?style=flat-square">\n    </a>\n</p>\n\nRexify is a library to streamline recommender systems model development.\n\nIn essence, Rexify adapts dynamically to your data, and outputs high-performing TensorFlow\nmodels that may be used wherever you want, independently of your data. Rexify also includes\nmodules to deal with feature engineering as Scikit-Learn Transformers and Pipelines.\n\nWith Rexify, users may easily train Recommender Systems models, just by specifying what their\ndata looks like. Rexify also comes equipped with pre-built machine learning pipelines which can\nbe used serverlessly. \n\n## What is Rexify?\n\nRexify is a low-code personalization tool, that makes use of traditional machine learning \nframeworks, such as Scikit-Learn and TensorFlow, to create scalable Recommender Systems\nworkflows that anyone can use.\n\n### Who is it for?\n\nRexify is a project that simplifies and standardizes the workflow of recommender systems. It is \nmostly geared towards people with little to no machine learning knowledge, that want to implement\nsomewhat scalable Recommender Systems in their applications.\n\n## Installation\n\nThe easiest way to install Rexify is via `pip`:\n\n```shell\npip install rexify\n```\n\n## Quick Tour\n\nRexify is meant to be usable right out of the box. All you need to set up your model is interaction\ndata - something that kind of looks like this:\n\n| user_id | item_id | timestamp  | event_type  |\n|---------|---------|------------|-------------|\n| 22      | 67      | 2021/05/13 | Purchase    |\n| 37      | 9       | 2021/04/11 | Page View   |\n| 22      | 473     | 2021/04/11 | Add to Cart |\n| ...     | ...     | ...        | ...         |\n| 358     | 51      | 2021/04/11 | Purchase    |\n\nAdditionally, we\'ll have to have configured a schema for the data.\nThis schema is what will allow Rexify to generate a dynamic model and preprocessing steps.\nThe schema should be comprised of two dictionaries (`user`, `ìtem`) and two key-value \npairs: `event_type` (which should point to the column of the event type) and `timestamp` (\nwhich should point to the timestamp column)\n\nEach of these dictionaries should consist of features and internal data types, \nsuch as: `id`, `category`, `number`. More data types will be available \nin the future.\n\n```json\n{\n  "user": {\n    "user_id": "id",\n    "age": "number"\n  },\n  "item": {\n    "item_id": "id",\n    "category": "category"\n  },\n  "timestamp": "timestamp"\n  "event_type": "event_type"\n}\n```\n\nEssentially, what Rexify will do is take the schema, and dynamically adapt to the data.\n\nThere are two main components in Rexify workflows: `FeatureExtractor` and `Recommender`.\n\nThe `FeatureExtractor` is a scikit-learn Transformer that basically takes the schema of \nthe data, and transforms the event data accordingly. Another method `.make_dataset()`, \nconverts the transformed data into a `tf.data.Dataset`, all correctly configured to be fed\nto the `Recommender` model.\n\n`Recommender` is a `tfrs.Model` that basically implements the Query and Candidate towers. \nDuring training, the Query tower will take the user ID, user features, and context, to \nlearn an embedding; the Candidate tower will do the same for the item ID and its features. \n\nMore information about how the `FeatureExtractor` and the `Recommender` works can be found \n[here](https://rexify.readthedocs.io/en/latest/overview/architecture.html). \n\nA sample Rexify workflow should sort of look like this:\n\n````python\n\nimport pandas as pd\n\nfrom rexify import Schema, FeatureExtractor, Recommender\n\nevents = pd.read_csv(\'path/to/events/data\')\n\nschema = Schema.load(\'path/to/schema\')\n\nfeat = FeatureExtractor(schema, users=\'path/to/users/data\', items=\'path/to/events/data\')\nx = feat.fit_transform(events)\nx = feat.make_dataset(x)\n\nmodel = Recommender(**feat.model_params)\nmodel.compile()\nmodel.fit(events, batch_size=512)\n````\n\nWhen training is complete, you\'ll have a trained `tf.keras.Model` ready to be used, as\nyou normally would. \n\n## License\n\n[MIT](https://github.com/joseprsm/rexify/blob/main/LICENSE)\n',
     'author': 'José Medeiros',
     'author_email': 'joseprsm@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 'rexify.features', 'rexify.features.transform', 'rexify.models',
 'rexify.models.callbacks', 'rexify.models.ranking', 'rexify.models.retrieval']
 package_data = \ {'': ['*']} install_requires = \ ['kfp>=1.8.0,<2.0.0',
 'numpy>=1.22.3', 'pandas>=1.4.0,<2.0.0', 'scikit-learn>=1.0.0,<2.0.0',
 'tensorflow_recommenders>=0.7.2'] extras_require = \ {':sys_platform !=
 "darwin"': ['tensorflow==2.9.0', 'scann>=1.2.0,<2.0.0'], ':sys_platform ==
 "darwin"': ['tensorflow_metal==0.5.0', 'tensorflow_macos==2.9.0']} setup_kwargs
-= { 'name': 'rexify', 'version': '0.1.4', 'description': 'Streamlined
+= { 'name': 'rexify', 'version': '0.1.5', 'description': 'Streamlined
 Recommender System workflows with TensorFlow and Kubeflow', 'long_description':
 '
                                       \n
         \n [https://storage.googleapis.com/rexify/1659986918545.png]\n
                                       \n
 \n\n
      \n \n_[Build]\n\n \n_[License]\n\n \n_[Documentation]\n\n \n_[GitHub
```

### Comparing `rexify-0.1.4/PKG-INFO` & `rexify-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rexify
-Version: 0.1.4
+Version: 0.1.5
 Summary: Streamlined Recommender System workflows with TensorFlow and Kubeflow
 License: MIT
 Author: José Medeiros
 Author-email: joseprsm@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rexify Version: 0.1.4 Summary: Streamlined
+Metadata-Version: 2.1 Name: rexify Version: 0.1.5 Summary: Streamlined
 Recommender System workflows with TensorFlow and Kubeflow License: MIT Author:
 JosÃ© Medeiros Author-email: joseprsm@gmail.com Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

