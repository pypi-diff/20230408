# Comparing `tmp/torch_choice-0.0.6.tar.gz` & `tmp/torch_choice-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_choice-0.0.6.tar", last modified: Thu Sep 29 19:43:22 2022, max compression
+gzip compressed data, was "torch_choice-1.0.0.tar", last modified: Sat Apr  8 20:07:23 2023, max compression
```

## Comparing `torch_choice-0.0.6.tar` & `torch_choice-1.0.0.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 19:43:22.646531 torch_choice-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)    10296 2022-09-29 19:43:22.646531 torch_choice-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9915 2022-09-29 19:43:13.000000 torch_choice-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-29 19:43:22.646531 torch_choice-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-09-29 19:43:13.000000 torch_choice-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 19:43:22.646531 torch_choice-0.0.6/torch_choice/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-29 19:43:13.000000 torch_choice-0.0.6/torch_choice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 19:43:22.646531 torch_choice-0.0.6/torch_choice/data/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-29 19:43:13.000000 torch_choice-0.0.6/torch_choice/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21600 2022-09-29 19:43:13.000000 torch_choice-0.0.6/torch_choice/data/choice_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     4402 2022-09-29 19:43:13.000000 torch_choice-0.0.6/torch_choice/data/joint_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2022 2022-09-29 19:43:13.000000 torch_choice-0.0.6/torch_choice/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 19:43:22.646531 torch_choice-0.0.6/torch_choice/model/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-09-29 19:43:13.000000 torch_choice-0.0.6/torch_choice/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9029 2022-09-29 19:43:13.000000 torch_choice-0.0.6/torch_choice/model/coefficient.py
--rw-r--r--   0 runner    (1001) docker     (121)    17069 2022-09-29 19:43:13.000000 torch_choice-0.0.6/torch_choice/model/conditional_logit_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    18955 2022-09-29 19:43:13.000000 torch_choice-0.0.6/torch_choice/model/nested_logit_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 19:43:22.646531 torch_choice-0.0.6/torch_choice/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-29 19:43:13.000000 torch_choice-0.0.6/torch_choice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21455 2022-09-29 19:43:13.000000 torch_choice-0.0.6/torch_choice/utils/easy_data_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     4335 2022-09-29 19:43:13.000000 torch_choice-0.0.6/torch_choice/utils/run_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2336 2022-09-29 19:43:13.000000 torch_choice-0.0.6/torch_choice/utils/std.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-29 19:43:22.646531 torch_choice-0.0.6/torch_choice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10296 2022-09-29 19:43:22.000000 torch_choice-0.0.6/torch_choice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-09-29 19:43:22.000000 torch_choice-0.0.6/torch_choice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-29 19:43:22.000000 torch_choice-0.0.6/torch_choice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-29 19:43:22.000000 torch_choice-0.0.6/torch_choice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:07:23.225548 torch_choice-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-04-08 20:07:23.225548 torch_choice-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-04-08 20:07:08.000000 torch_choice-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-08 20:07:23.225548 torch_choice-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-08 20:07:08.000000 torch_choice-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:07:23.221548 torch_choice-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-04-08 20:07:08.000000 torch_choice-1.0.0/tests/test_choice_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-08 20:07:08.000000 torch_choice-1.0.0/tests/test_conditional_logit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7750 2023-04-08 20:07:08.000000 torch_choice-1.0.0/tests/test_nested_logit_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:07:23.221548 torch_choice-1.0.0/torch_choice/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:07:23.221548 torch_choice-1.0.0/torch_choice/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22241 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/data/choice_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4402 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/data/joint_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:07:23.221548 torch_choice-1.0.0/torch_choice/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/model/coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18805 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/model/conditional_logit_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/model/formula_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21452 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/model/nested_logit_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:07:23.221548 torch_choice-1.0.0/torch_choice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22785 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/utils/easy_data_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/utils/run_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13678 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/utils/run_helper_temp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-04-08 20:07:08.000000 torch_choice-1.0.0/torch_choice/utils/std.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-08 20:07:23.221548 torch_choice-1.0.0/torch_choice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-04-08 20:07:23.000000 torch_choice-1.0.0/torch_choice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-08 20:07:23.000000 torch_choice-1.0.0/torch_choice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-08 20:07:23.000000 torch_choice-1.0.0/torch_choice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-08 20:07:23.000000 torch_choice-1.0.0/torch_choice.egg-info/top_level.txt
```

### Comparing `torch_choice-0.0.6/PKG-INFO` & `torch_choice-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_choice
-Version: 0.0.6
+Version: 1.0.0
 Summary: A Pytorch Backend Library for Choice Modelling
 Home-page: 
 Author: Tianyu Du
 Author-email: tianyudu@stanford.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,15 @@
 
 [Logistic Regression](https://en.wikipedia.org/wiki/Logistic_regression) models the probability that user $u$ chooses item $i$ in session $s$ by the logistic function
 
 $$
 P_{uis} = \frac{e^{\mu_{uis}}}{\Sigma_{j \in A_{us}}e^{\mu_{ujs}}}
 $$
 
-where, 
+where,
 
 $$\mu_{uis} = \alpha + \beta X + \gamma W + \dots$$
 
 here $X$, $W$ are predictors (independent variables) for users and items respectively (these can be constant or can vary across session), and greek letters $\alpha$, $\beta$ and $\gamma$ are learned parameters. $A_{us}$ is the set of items available for user $u$ in session $s$.
 
 When users are choosing over items, we can write utility $U_{uis}$ that user $u$ derives from item $i$ in session $s$, as
 
@@ -48,15 +48,15 @@
 $$
 
 where $\epsilon$ is an unobserved random error term.
 
 If we assume iid extreme value type 1 errors for $\epsilon_{uis}$, this leads to the above logistic probabilities of user $u$ choosing item $i$ in session $s$, as shown by [McFadden](https://en.wikipedia.org/wiki/Choice_modelling), and as often studied in Econometrics.
 
 ## Package
-We implement a fully flexible setup, where we allow 
+We implement a fully flexible setup, where we allow
 1. coefficients ($\alpha$, $\beta$, $\gamma$, $\dots$) to be constant, user-specific (i.e., $\alpha=\alpha_u$), item-specific (i.e., $\alpha=\alpha_i$), session-specific (i.e., $\alpha=\alpha_t$), or (session, item)-specific (i.e., $\alpha=\alpha_{ti}$). For example, specifying $\alpha$ to be item-specific is equivalent to adding an item-level fixed effect.
 2. Observables ($X$, $Y$, $\dots$) to be constant, user-specific, item-specific, session-specific, or (session, item) (such as price) and (session, user) (such as income) specific as well.
 3. Specifying availability sets $A_{us}$
 
 This flexibility in coefficients and features allows for more than 20 types of additive terms to $U_{uis}$, which enables modelling rich structures.
 
 As such, this package can be used to learn such models for
@@ -88,14 +88,21 @@
 - $X^{session:pixelvalues}_{t}$ is a matrix of size (S) x (H x W) where H x W are the dimensions of the image being classified; its coefficient $\beta_i$ has item level vartiation and is of size (I) x (1)
 
 This is a classic problem used for exposition in Computer Science to motivate various Machine Learning models. There is no concept of a user in this setup. Our package allows for models of this nature and is fully usable for Machine Learning problems with added flexibility over [scikit-learn logistic regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)
 
 We highly recommend users to go through [tutorials](https://github.com/gsbDBI/torch-choice/blob/main/tutorials) we prepared to get a better understanding of what the package offers. We present multiple examples, and for each case we specify the utility form.
 
 ## Installation
+We offer two ways to install the package.
+### Installation from Pip
+Simply run `pip install torch-choice` to install the package. This will install the latest *stable* version of the package.
+
+### Installation from Source
+For those wish to leverage the latest feature, you can install `torch-choice` from Github source.
+
 1. Clone the repository to your local machine or server.
 2. Install required dependencies using: `pip3 install -r requirements.txt`.
 3. Run `pip3 install torch-choice`.
 4. Check installation by running `python3 -c 'import torch_choice; print(torch_choice.__version__)'`.
 
 [The installation page](https://gsbdbi.github.io/torch-choice/install/) provides more details on installation.
```

### Comparing `torch_choice-0.0.6/README.md` & `torch_choice-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 [Logistic Regression](https://en.wikipedia.org/wiki/Logistic_regression) models the probability that user $u$ chooses item $i$ in session $s$ by the logistic function
 
 $$
 P_{uis} = \frac{e^{\mu_{uis}}}{\Sigma_{j \in A_{us}}e^{\mu_{ujs}}}
 $$
 
-where, 
+where,
 
 $$\mu_{uis} = \alpha + \beta X + \gamma W + \dots$$
 
 here $X$, $W$ are predictors (independent variables) for users and items respectively (these can be constant or can vary across session), and greek letters $\alpha$, $\beta$ and $\gamma$ are learned parameters. $A_{us}$ is the set of items available for user $u$ in session $s$.
 
 When users are choosing over items, we can write utility $U_{uis}$ that user $u$ derives from item $i$ in session $s$, as
 
@@ -35,15 +35,15 @@
 $$
 
 where $\epsilon$ is an unobserved random error term.
 
 If we assume iid extreme value type 1 errors for $\epsilon_{uis}$, this leads to the above logistic probabilities of user $u$ choosing item $i$ in session $s$, as shown by [McFadden](https://en.wikipedia.org/wiki/Choice_modelling), and as often studied in Econometrics.
 
 ## Package
-We implement a fully flexible setup, where we allow 
+We implement a fully flexible setup, where we allow
 1. coefficients ($\alpha$, $\beta$, $\gamma$, $\dots$) to be constant, user-specific (i.e., $\alpha=\alpha_u$), item-specific (i.e., $\alpha=\alpha_i$), session-specific (i.e., $\alpha=\alpha_t$), or (session, item)-specific (i.e., $\alpha=\alpha_{ti}$). For example, specifying $\alpha$ to be item-specific is equivalent to adding an item-level fixed effect.
 2. Observables ($X$, $Y$, $\dots$) to be constant, user-specific, item-specific, session-specific, or (session, item) (such as price) and (session, user) (such as income) specific as well.
 3. Specifying availability sets $A_{us}$
 
 This flexibility in coefficients and features allows for more than 20 types of additive terms to $U_{uis}$, which enables modelling rich structures.
 
 As such, this package can be used to learn such models for
@@ -75,14 +75,21 @@
 - $X^{session:pixelvalues}_{t}$ is a matrix of size (S) x (H x W) where H x W are the dimensions of the image being classified; its coefficient $\beta_i$ has item level vartiation and is of size (I) x (1)
 
 This is a classic problem used for exposition in Computer Science to motivate various Machine Learning models. There is no concept of a user in this setup. Our package allows for models of this nature and is fully usable for Machine Learning problems with added flexibility over [scikit-learn logistic regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)
 
 We highly recommend users to go through [tutorials](https://github.com/gsbDBI/torch-choice/blob/main/tutorials) we prepared to get a better understanding of what the package offers. We present multiple examples, and for each case we specify the utility form.
 
 ## Installation
+We offer two ways to install the package.
+### Installation from Pip
+Simply run `pip install torch-choice` to install the package. This will install the latest *stable* version of the package.
+
+### Installation from Source
+For those wish to leverage the latest feature, you can install `torch-choice` from Github source.
+
 1. Clone the repository to your local machine or server.
 2. Install required dependencies using: `pip3 install -r requirements.txt`.
 3. Run `pip3 install torch-choice`.
 4. Check installation by running `python3 -c 'import torch_choice; print(torch_choice.__version__)'`.
 
 [The installation page](https://gsbdbi.github.io/torch-choice/install/) provides more details on installation.
```

### Comparing `torch_choice-0.0.6/setup.py` & `torch_choice-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="torch_choice",
-    version="0.0.6",
+    version="1.0.0",
     description="A Pytorch Backend Library for Choice Modelling",
     long_description=README,
     long_description_content_type="text/markdown",
     url="",
     author="Tianyu Du",
     author_email="tianyudu@stanford.edu",
     license="MIT",
```

### Comparing `torch_choice-0.0.6/torch_choice/data/choice_dataset.py` & `torch_choice-1.0.0/torch_choice/data/choice_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """
 The dataset object for management large scale consumer choice datasets.
 Please refer to the documentation and tutorials for more details on using `ChoiceDataset`.
 
 Author: Tianyu Du
-Update: Apr. 27, 2022
+Update: Jan. 2, 2023
 """
 import copy
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import torch
 
 
 class ChoiceDataset(torch.utils.data.Dataset):
     def __init__(self,
                  item_index: torch.LongTensor,
+                 num_items: int = None,
                  label: Optional[torch.LongTensor] = None,
                  user_index: Optional[torch.LongTensor] = None,
                  session_index: Optional[torch.LongTensor] = None,
                  item_availability: Optional[torch.BoolTensor] = None,
                  **kwargs) -> None:
         """
         Initialization methods for the dataset object, researchers should supply all information about the dataset
@@ -78,33 +79,42 @@
             2. item observables must start with 'item_' and have shape (num_items, *)
             3. session observables must start with 'session_' and have shape (num_sessions, *)
             4. taste observables (those vary by user and item) must start with `taste_` and have shape
                 (num_users, num_items, *).
             NOTE: we don't recommend using taste observables, because num_users * num_items is potentially large.
             5. price observables (those vary by session and item) must start with `price_` and have
                 shape (num_sessions, num_items, *)
+            6. itemsession observables starting with `itemsession_`, this is a more intuitive alias to the price
+                observable.
         """
         # ENHANCEMENT(Tianyu): add item_names for summary.
         super(ChoiceDataset, self).__init__()
         self.label = label
         self.item_index = item_index
+        if num_items is not None:
+            self.provided_num_items = num_items
+        else:
+            self.provided_num_items = None
         self.user_index = user_index
         self.session_index = session_index
 
         if self.session_index is None:
             # if any([x.startswith('session_') or x.startswith('price_') for x in kwargs.keys()]):
             # if any session sensitive observable is provided, but session index is not,
             # infer each row in the dataset to be a session.
             # TODO: (design choice) should we assign unique session index to each choice instance or the same session index.
             print('No `session_index` is provided, assume each choice instance is in its own session.')
             self.session_index = torch.arange(len(self.item_index)).long()
 
         self.item_availability = item_availability
 
         for key, item in kwargs.items():
+            if self._is_attribute(key):
+                # all observable should be float.
+                item = item.float()
             setattr(self, key, item)
 
         # TODO: add a validation procedure to check the consistency of the dataset.
 
     def __getitem__(self, indices: Union[int, torch.LongTensor]) -> "ChoiceDataset":
         """Retrieves samples corresponding to the provided index or list of indices.
 
@@ -194,15 +204,19 @@
     @property
     def num_items(self) -> int:
         """Returns the number of items involved in this dataset.
 
         Returns:
             int: the number of items involved in this dataset.
         """
-        return len(torch.unique(self.item_index))
+        if self.provided_num_items is None:
+            # infer the number of items from item_index.
+            return len(torch.unique(self.item_index))
+        else:
+            return self.provided_num_items
 
         # for key, val in self.__dict__.items():
         #     if torch.is_tensor(val):
         #         if self._is_item_attribute(key):
         #             return val.shape[0]
         #         elif self._is_taste_attribute(key) or self._is_price_attribute(key):
         #             return val.shape[1]
@@ -361,15 +375,15 @@
 
     @staticmethod
     def _is_taste_attribute(key: str) -> bool:
         return key.startswith('taste_')
 
     @staticmethod
     def _is_price_attribute(key: str) -> bool:
-        return key.startswith('price_')
+        return key.startswith('price_') or key.startswith('itemsession_')
 
     def _is_attribute(self, key: str) -> bool:
         return self._is_item_attribute(key) \
             or self._is_user_attribute(key) \
             or self._is_session_attribute(key) \
             or self._is_taste_attribute(key) \
             or self._is_price_attribute(key)
```

### Comparing `torch_choice-0.0.6/torch_choice/data/joint_dataset.py` & `torch_choice-1.0.0/torch_choice/data/joint_dataset.py`

 * *Files identical despite different names*

### Comparing `torch_choice-0.0.6/torch_choice/data/utils.py` & `torch_choice-1.0.0/torch_choice/data/utils.py`

 * *Files identical despite different names*

### Comparing `torch_choice-0.0.6/torch_choice/model/coefficient.py` & `torch_choice-1.0.0/torch_choice/model/coefficient.py`

 * *Files identical despite different names*

### Comparing `torch_choice-0.0.6/torch_choice/model/conditional_logit_model.py` & `torch_choice-1.0.0/torch_choice/model/conditional_logit_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 import warnings
 from copy import deepcopy
 from typing import Dict, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
+
 from torch_choice.data.choice_dataset import ChoiceDataset
 from torch_choice.model.coefficient import Coefficient
+from torch_choice.model.formula_parser import parse_formula
 
 
 class ConditionalLogitModel(nn.Module):
     """The more generalized version of conditional logit model, the model allows for research specific
     variable types(groups) and different levels of variations for coefficient.
 
     The model allows for the following levels for variable variations:
@@ -36,27 +38,37 @@
 
     - user-item: parameters that are specific to both user and item, parameter for the first item
         for all users are forced to be zero.
     - user-item-full: parameters that are specific to both user and item, explicitly model for all items.
     """
 
     def __init__(self,
-                 coef_variation_dict: Dict[str, str],
+                 formula: Optional[str]=None,
+                 dataset: Optional[ChoiceDataset]=None,
+                 coef_variation_dict: Optional[Dict[str, str]]=None,
                  num_param_dict: Optional[Dict[str, int]]=None,
                  num_items: Optional[int]=None,
                  num_users: Optional[int]=None,
                  regularization: Optional[str]=None,
                  regularization_weight: Optional[float]=None
                  ) -> None:
         """
         Args:
-            num_items (int): number of items in the dataset.
-            num_users (int): number of users in the dataset.
+            formula (str): a string representing the utility formula.
+                The formula consists of '(variable_name|variation)'s separated by '+', for example:
+                "(var1|item) + (var2|user) + (var3|constant)"
+                where the first part of each term is the name of the variable
+                and the second part is the variation of the coefficient.
+                The variation can be one of the following:
+                'constant', 'item', 'item-full', 'user', 'user-item', 'user-item-full'.
+                All spaces in the formula will be ignored, hence please do not use spaces in variable/observable names.
+            data (ChoiceDataset): a ChoiceDataset object for training the model, the parser will infer dimensions of variables
+                and sizes of coefficients from the ChoiceDataset.
             coef_variation_dict (Dict[str, str]): variable type to variation level dictionary. Keys of this dictionary
-                should be variable names in the dataset (i.e., these starting with `price_`, `user_`, etc), or `intercept`
+                should be variable names in the dataset (i.e., these starting with `itemsession_`, `price_`, `user_`, etc), or `intercept`
                 if the researcher requires an intercept term.
                 For each variable name X_var (e.g., `user_income`) or `intercept`, the corresponding dictionary key should
                 be one of the following values, this value specifies the "level of variation" of the coefficient.
 
                 - `constant`: the coefficient constant over all users and items: $X \beta$.
 
                 - `user`: user-specific parameters but constant across all items: $X \beta_{u}$.
@@ -70,30 +82,44 @@
 
                 The following configurations are supported by the package, but we don't recommend using them due to the
                     large number of parameters.
                 - `user-item`: parameters that are specific to both user and item, parameter for the first item
                     for all users are forced to be zero.
 
                 - `user-item-full`: parameters that are specific to both user and item, explicitly model for all items.
-
             num_param_dict (Optional[Dict[str, int]]): variable type to number of parameters dictionary with keys exactly the same
                 as the `coef_variation_dict`. Values of `num_param_dict` records numbers of features in each kind of variable.
                 If None is supplied, num_param_dict will be a dictionary with the same keys as the `coef_variation_dict` dictionary
                 and values of all ones. Default to be None.
+            num_items (int): number of items in the dataset.
+            num_users (int): number of users in the dataset.
             regularization (Optional[str]): this argument takes values from {'L1', 'L2', None}, which specifies the type of
                 regularization added to the log-likelihood.
                 - 'L1' will subtract regularization_weight * 1-norm of parameters from the log-likelihood.
                 - 'L2' will subtract regularization_weight * 2-norm of parameters from the log-likelihood.
                 - None does not modify the log-likelihood.
                 Defaults to None.
             regularization_weight (Optional[float]): the weight of parameter norm subtracted from the log-likelihood.
                 This term controls the strength of regularization. This argument is required if and only if regularization
                 is not None.
                 Defaults to None.
         """
+        if coef_variation_dict is None and formula is None:
+            raise ValueError("Either coef_variation_dict or formula should be provided to specify the model.")
+
+        if (coef_variation_dict is not None) and (formula is not None):
+            raise ValueError("Only one of coef_variation_dict or formula should be provided to specify the model.")
+
+        if (formula is not None) and (dataset is None):
+            raise ValueError("If formula is provided, data should be provided to specify the model.")
+
+        # Use the formula to infer model, override dictionaries.
+        if formula is not None:
+            coef_variation_dict, num_param_dict = parse_formula(formula, dataset)
+
         super(ConditionalLogitModel, self).__init__()
 
         if num_param_dict is None:
             num_param_dict = {key:1 for key in coef_variation_dict.keys()}
 
         assert coef_variation_dict.keys() == num_param_dict.keys()
```

### Comparing `torch_choice-0.0.6/torch_choice/utils/easy_data_wrapper.py` & `torch_choice-1.0.0/torch_choice/utils/easy_data_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,21 @@
                  user_index_column: Optional[str] = None,
                  session_index_column: Optional[str] = None,
                  # Option 1: feed in data-frames of observables.
                  user_observable_data: Optional[Dict[str, pd.DataFrame]] = None,
                  item_observable_data: Optional[Dict[str, pd.DataFrame]] = None,
                  session_observable_data: Optional[Dict[str, pd.DataFrame]] = None,
                  price_observable_data: Optional[Dict[str, pd.DataFrame]] = None,
+                 itemsession_observable_data: Optional[Dict[str, pd.DataFrame]] = None,
                  # Option 2: derive observables from columns of main_data.
                  user_observable_columns: Optional[List[str]] = None,
                  item_observable_columns: Optional[List[str]] = None,
                  session_observable_columns: Optional[List[str]] = None,
                  price_observable_columns: Optional[List[str]] = None,
+                 itemsession_observable_columns: Optional[List[str]] = None,
                  device: str = 'cpu'):
         """The initialization method of EasyDatasetWrapper.
 
         Args:
             main_data (pd.DataFrame): the main dataset holding all purchase records in a "long-format", each row of the
                 dataset is an item in a purchase record.
                 The main_data data-frame should contains the following columns:
@@ -67,20 +69,25 @@
                 and consisting of values from `main_data[session_index_column]`. Defaults to dict().
 
             price_observable_data (Optional[Dict[str, pd.DataFrame]], optional): a dictionary with keys as the name of each
                 observable. The values should be a pandas data-frame contains (1) a column named by the value of `session_index_column`
                 and consists of values from `main_data[session_index_column]` and (2) a column named by the value of `item_name_column`
                 and consisting of values from `main_data[item_name_column]`. Defaults to dict().
 
+            itemsession_observable_data (Optional[Dict[str, pd.DataFrame]], optional) is an alias for the
+                price_observable_data argument for backward compatibility. All items of itemsession_observable_data
+                will be added to price_observable_data. Defaults to dict().
+
             Another method to include observables is via *_observable_columns keywords, which takes column name(s) of the main_data
                 data-frame. The data wrapper will derive observable data from the main_data data-frame.
                 For example, with `user_observable_columns = ['feature_A', 'feature_B']`, this wrapper will create two user-specific
                 observable tensors derived from main_data['feature_A'] and main_data['feature_B'].
 
-            # format (str, optional): the input format of the dataset. Defaults to 'stata'.
+            The itemsession_observable_column is an alias for the `price_observable_column` argument for backward compatibility,
+                all elements of `itemsession_observable_columns` will be appended to `price_observable_column`.
 
         Raises:
             ValueError: _description_
         """
         # read in data.
         self.main_data = main_data
         self.purchase_record_column = purchase_record_column
@@ -92,20 +99,34 @@
         self.user_index_column = user_index_column
         self.session_index_column = session_index_column
         self.device = device
 
         # encode item name, user index, session index.
         self.encode()
 
+        # adding alias itemsession_observable_data to price_observable_data.
+        if itemsession_observable_data is not None:
+            if price_observable_data is None:
+                price_observable_data = itemsession_observable_data
+            else:
+                price_observable_data.extend(itemsession_observable_data)
+
         # re-format observable data-frames and set correct index.
         self.align_observable_data(item_observable_data,
                                    user_observable_data,
                                    session_observable_data,
                                    price_observable_data)
 
+        if itemsession_observable_columns is not None:
+            # merge the item-session observable columns to price_observable_columns.
+            if price_observable_columns is None:
+                price_observable_columns = itemsession_observable_columns
+            else:
+                price_observable_columns.extend(itemsession_observable_columns)
+
         # derive observables from columns of the main data-frame.
         self.derive_observable_from_main_data(item_observable_columns,
                                               user_observable_columns,
                                               session_observable_columns,
                                               price_observable_columns)
 
         self.observable_data_to_observable_tensors()
@@ -147,15 +168,15 @@
         self.item_observable_data = dict()
         if item_observable_data is not None:
             for key, val in item_observable_data.items():
                 # key: observable name.
                 # val: data-frame of observable data.
                 assert self.item_name_column in val.columns, f"{self.item_name_column} is not a column of provided item observable data-frame."
                 for item in self.item_name_encoder.classes_:
-                    assert item in val[self.item_name_column], f"item {item} is not in the {self.item_name_column} column of the item observable data-frame."
+                    assert item in val[self.item_name_column].values, f"item {item} is not in the {self.item_name_column} column of the item observable data-frame."
 
                 self.item_observable_data['item_' + key] = val.set_index(self.item_name_column).loc[self.item_name_encoder.classes_]
 
         self.user_observable_data = dict()
         if user_observable_data is not None:
             for key, val in user_observable_data.items():
                 # key: observable name.
@@ -194,15 +215,15 @@
                 for item in self.item_name_encoder.classes_:
                     assert item in val[self.item_name_column].values, f"item {item} is not in the {self.item_name_column} column of the price observable data-frame."
 
                 # need to re-index since some (session, item) pairs are allowed to be unavailable.
                 # complete index = Cartesian product of all sessions and all items.
                 complete_index = pd.MultiIndex.from_product([self.session_name_encoder.classes_, self.item_name_encoder.classes_],
                                                             names=[self.session_index_column, self.item_name_column])
-                self.price_observable_data['price_' + key] = val.set_index([self.session_index_column, self.item_name_column]).reindex(complete_index)
+                self.price_observable_data['itemsession_' + key] = val.set_index([self.session_index_column, self.item_name_column]).reindex(complete_index)
 
     def derive_observable_from_main_data(self,
                                          item_observable_columns: Optional[List[str]],
                                          user_observable_columns: Optional[List[str]],
                                          session_observable_columns: Optional[List[str]],
                                          price_observable_columns: Optional[List[str]]) -> None:
         """
@@ -225,15 +246,15 @@
                 self.session_observable_data['session_' + obs_col] = self.main_data.groupby(self.session_index_column).first()[[obs_col]].loc[self.session_name_encoder.classes_]
 
         if price_observable_columns is not None:
             for obs_col in price_observable_columns:
                 val = self.main_data.groupby([self.session_index_column, self.item_name_column]).first()[[obs_col]]
                 complete_index = pd.MultiIndex.from_product([self.session_name_encoder.classes_, self.item_name_encoder.classes_],
                                                             names=[self.session_index_column, self.item_name_column])
-                self.price_observable_data['price_' + obs_col] = val.reindex(complete_index)
+                self.price_observable_data['itemsession_' + obs_col] = val.reindex(complete_index)
 
     def observable_data_to_observable_tensors(self) -> None:
         """Convert all self.*_observable_data to self.*_observable_tensors for PyTorch."""
         self.item_observable_tensors = dict()
         for key, val in self.item_observable_data.items():
             assert all(val.index == self.item_name_encoder.classes_), "item observable data is not alighted with user name encoder."
             self.item_observable_tensors[key] = torch.tensor(val.values, dtype=torch.float32)
```

### Comparing `torch_choice-0.0.6/torch_choice/utils/run_helper.py` & `torch_choice-1.0.0/torch_choice/utils/run_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 import torch.nn.functional as F
 from torch_choice.data import utils as data_utils
 from torch_choice.utils.std import parameter_std
 from torch_choice.model.conditional_logit_model import ConditionalLogitModel
 from torch_choice.model.nested_logit_model import NestedLogitModel
 
 
-def run(model, dataset, dataset_test=None, batch_size=-1, learning_rate=0.01, num_epochs=5000):
+def run(model, dataset, dataset_test=None, batch_size=-1, learning_rate=0.01, num_epochs=5000, report_frequency=None, compute_std=True, return_final_training_log_likelihood=False):
     """All in one script for the model training and result presentation."""
+    if report_frequency is None:
+        report_frequency = (num_epochs // 10)
+
     assert isinstance(model, ConditionalLogitModel) or isinstance(model, NestedLogitModel), \
         f'A model of type {type(model)} is not supported by this runner.'
     model = deepcopy(model)  # do not modify the model outside.
     trained_model = deepcopy(model)  # create another copy for returning.
     data_loader = data_utils.create_data_loader(dataset, batch_size=batch_size, shuffle=True)
     optimizer = torch.optim.Adam(model.parameters(), lr=learning_rate)
     print('=' * 20, 'received model', '=' * 20)
@@ -32,63 +35,72 @@
         # track the log-likelihood to minimize.
         ll, count = 0.0, 0.0
         for batch in data_loader:
             item_index = batch['item'].item_index if isinstance(model, NestedLogitModel) else batch.item_index
             # the model.loss returns negative log-likelihood + regularization term.
             loss = model.loss(batch, item_index)
 
-            if e % (num_epochs // 10) == 0:
+            if (e % report_frequency) == 0:
                 # record log-likelihood.
                 ll -= model.negative_log_likelihood(batch, item_index).detach().item() # * len(batch)
                 count += len(batch)
 
             optimizer.zero_grad()
             loss.backward()
             optimizer.step()
 
         # ll /= count
-        if e % (num_epochs // 10) == 0:
+        if (e % report_frequency) == 0:
             print(f'Epoch {e}: Log-likelihood={ll}')
 
     if dataset_test is not None:
         test_ll = - model.negative_log_likelihood(dataset_test, dataset_test.item_index).detach().item()
         print('Test set log-likelihood: ', test_ll)
 
-    # current methods of computing standard deviation will corrupt the model, load weights into another model for returning.
-    state_dict = deepcopy(model.state_dict())
-    trained_model.load_state_dict(state_dict)
-
-    # get mean of estimation.
-    mean_dict = dict()
-    for k, v in model.named_parameters():
-        mean_dict[k] = v.clone()
-
-    # estimate the standard error of the model.
-    if isinstance(model, ConditionalLogitModel):
-        def nll_loss(model):
-            y_pred = model(dataset)
-            return F.cross_entropy(y_pred, dataset.item_index, reduction='sum')
-    elif isinstance(model, NestedLogitModel):
-        def nll_loss(model):
-            d = dataset[torch.arange(len(dataset))]
-            return model.negative_log_likelihood(d, d['item'].item_index)
-
-    std_dict = parameter_std(model, nll_loss)
-
-    print('=' * 20, 'model results', '=' * 20)
-    report = list()
-    for coef_name, std in std_dict.items():
-        std = std.cpu().detach().numpy()
-        mean = mean_dict[coef_name].cpu().detach().numpy()
-        coef_name = coef_name.replace('coef_dict.', '').replace('.coef', '')
-        for i in range(mean.size):
-            report.append({'Coefficient': coef_name + f'_{i}',
-                           'Estimation': float(mean[i]),
-                           'Std. Err.': float(std[i])})
-    report = pd.DataFrame(report).set_index('Coefficient')
-    print(f'Training Epochs: {num_epochs}\n')
-    print(f'Learning Rate: {learning_rate}\n')
-    print(f'Batch Size: {batch_size if batch_size != -1 else len(dataset)} out of {len(dataset)} observations in total\n')
-    print(f'Final Log-likelihood: {ll}\n')
-    print('Coefficients:\n')
-    print(report.to_markdown())
-    return trained_model
+    if not compute_std:
+        if return_final_training_log_likelihood:
+            return model, ll
+        else:
+            return model
+    else:
+        # current methods of computing standard deviation will corrupt the model, load weights into another model for returning.
+        state_dict = deepcopy(model.state_dict())
+        trained_model.load_state_dict(state_dict)
+
+        # get mean of estimation.
+        mean_dict = dict()
+        for k, v in model.named_parameters():
+            mean_dict[k] = v.clone()
+
+        # estimate the standard error of the model.
+        if isinstance(model, ConditionalLogitModel):
+            def nll_loss(model):
+                y_pred = model(dataset)
+                return F.cross_entropy(y_pred, dataset.item_index, reduction='sum')
+        elif isinstance(model, NestedLogitModel):
+            def nll_loss(model):
+                d = dataset[torch.arange(len(dataset))]
+                return model.negative_log_likelihood(d, d['item'].item_index)
+
+        std_dict = parameter_std(model, nll_loss)
+
+        print('=' * 20, 'model results', '=' * 20)
+        report = list()
+        for coef_name, std in std_dict.items():
+            std = std.cpu().detach().numpy()
+            mean = mean_dict[coef_name].cpu().detach().numpy()
+            coef_name = coef_name.replace('coef_dict.', '').replace('.coef', '')
+            for i in range(mean.size):
+                report.append({'Coefficient': coef_name + f'_{i}',
+                            'Estimation': float(mean[i]),
+                            'Std. Err.': float(std[i])})
+        report = pd.DataFrame(report).set_index('Coefficient')
+        print(f'Training Epochs: {num_epochs}\n')
+        print(f'Learning Rate: {learning_rate}\n')
+        print(f'Batch Size: {batch_size if batch_size != -1 else len(dataset)} out of {len(dataset)} observations in total\n')
+        print(f'Final Log-likelihood: {ll}\n')
+        print('Coefficients:\n')
+        print(report.to_markdown())
+        if return_final_training_log_likelihood:
+            return trained_model, ll
+        else:
+            return trained_model
```

### Comparing `torch_choice-0.0.6/torch_choice/utils/std.py` & `torch_choice-1.0.0/torch_choice/utils/std.py`

 * *Files identical despite different names*

### Comparing `torch_choice-0.0.6/torch_choice.egg-info/PKG-INFO` & `torch_choice-1.0.0/torch_choice.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-choice
-Version: 0.0.6
+Version: 1.0.0
 Summary: A Pytorch Backend Library for Choice Modelling
 Home-page: 
 Author: Tianyu Du
 Author-email: tianyudu@stanford.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,15 @@
 
 [Logistic Regression](https://en.wikipedia.org/wiki/Logistic_regression) models the probability that user $u$ chooses item $i$ in session $s$ by the logistic function
 
 $$
 P_{uis} = \frac{e^{\mu_{uis}}}{\Sigma_{j \in A_{us}}e^{\mu_{ujs}}}
 $$
 
-where, 
+where,
 
 $$\mu_{uis} = \alpha + \beta X + \gamma W + \dots$$
 
 here $X$, $W$ are predictors (independent variables) for users and items respectively (these can be constant or can vary across session), and greek letters $\alpha$, $\beta$ and $\gamma$ are learned parameters. $A_{us}$ is the set of items available for user $u$ in session $s$.
 
 When users are choosing over items, we can write utility $U_{uis}$ that user $u$ derives from item $i$ in session $s$, as
 
@@ -48,15 +48,15 @@
 $$
 
 where $\epsilon$ is an unobserved random error term.
 
 If we assume iid extreme value type 1 errors for $\epsilon_{uis}$, this leads to the above logistic probabilities of user $u$ choosing item $i$ in session $s$, as shown by [McFadden](https://en.wikipedia.org/wiki/Choice_modelling), and as often studied in Econometrics.
 
 ## Package
-We implement a fully flexible setup, where we allow 
+We implement a fully flexible setup, where we allow
 1. coefficients ($\alpha$, $\beta$, $\gamma$, $\dots$) to be constant, user-specific (i.e., $\alpha=\alpha_u$), item-specific (i.e., $\alpha=\alpha_i$), session-specific (i.e., $\alpha=\alpha_t$), or (session, item)-specific (i.e., $\alpha=\alpha_{ti}$). For example, specifying $\alpha$ to be item-specific is equivalent to adding an item-level fixed effect.
 2. Observables ($X$, $Y$, $\dots$) to be constant, user-specific, item-specific, session-specific, or (session, item) (such as price) and (session, user) (such as income) specific as well.
 3. Specifying availability sets $A_{us}$
 
 This flexibility in coefficients and features allows for more than 20 types of additive terms to $U_{uis}$, which enables modelling rich structures.
 
 As such, this package can be used to learn such models for
@@ -88,14 +88,21 @@
 - $X^{session:pixelvalues}_{t}$ is a matrix of size (S) x (H x W) where H x W are the dimensions of the image being classified; its coefficient $\beta_i$ has item level vartiation and is of size (I) x (1)
 
 This is a classic problem used for exposition in Computer Science to motivate various Machine Learning models. There is no concept of a user in this setup. Our package allows for models of this nature and is fully usable for Machine Learning problems with added flexibility over [scikit-learn logistic regression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html)
 
 We highly recommend users to go through [tutorials](https://github.com/gsbDBI/torch-choice/blob/main/tutorials) we prepared to get a better understanding of what the package offers. We present multiple examples, and for each case we specify the utility form.
 
 ## Installation
+We offer two ways to install the package.
+### Installation from Pip
+Simply run `pip install torch-choice` to install the package. This will install the latest *stable* version of the package.
+
+### Installation from Source
+For those wish to leverage the latest feature, you can install `torch-choice` from Github source.
+
 1. Clone the repository to your local machine or server.
 2. Install required dependencies using: `pip3 install -r requirements.txt`.
 3. Run `pip3 install torch-choice`.
 4. Check installation by running `python3 -c 'import torch_choice; print(torch_choice.__version__)'`.
 
 [The installation page](https://gsbdbi.github.io/torch-choice/install/) provides more details on installation.
```

### Comparing `torch_choice-0.0.6/torch_choice.egg-info/SOURCES.txt` & `torch_choice-1.0.0/torch_choice.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 README.md
 setup.py
+tests/test_choice_dataset.py
+tests/test_conditional_logit_model.py
+tests/test_nested_logit_model.py
 torch_choice/__init__.py
 torch_choice.egg-info/PKG-INFO
 torch_choice.egg-info/SOURCES.txt
 torch_choice.egg-info/dependency_links.txt
 torch_choice.egg-info/top_level.txt
 torch_choice/data/__init__.py
 torch_choice/data/choice_dataset.py
 torch_choice/data/joint_dataset.py
 torch_choice/data/utils.py
 torch_choice/model/__init__.py
 torch_choice/model/coefficient.py
 torch_choice/model/conditional_logit_model.py
+torch_choice/model/formula_parser.py
 torch_choice/model/nested_logit_model.py
 torch_choice/utils/__init__.py
 torch_choice/utils/easy_data_wrapper.py
 torch_choice/utils/run_helper.py
+torch_choice/utils/run_helper_temp.py
 torch_choice/utils/std.py
```

