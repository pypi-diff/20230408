# Comparing `tmp/pandas_dq-1.7.tar.gz` & `tmp/pandas_dq-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_dq-1.7.tar", last modified: Fri Apr  7 17:03:29 2023, max compression
+gzip compressed data, was "pandas_dq-1.8.tar", last modified: Fri Apr  7 22:22:56 2023, max compression
```

## Comparing `pandas_dq-1.7.tar` & `pandas_dq-1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-07 17:03:29.818100 pandas_dq-1.7/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    11357 2023-04-02 23:27:15.000000 pandas_dq-1.7/LICENSE
--rwxrwxrwx   0 ram       (1000) ram       (1000)      610 2022-04-07 23:06:53.000000 pandas_dq-1.7/MANIFEST.in
--rwxrwxrwx   0 ram       (1000) ram       (1000)    11030 2023-04-07 17:03:29.818100 pandas_dq-1.7/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)     9215 2023-04-07 16:58:41.000000 pandas_dq-1.7/README.md
-drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-07 17:03:29.802470 pandas_dq-1.7/pandas_dq.egg-info/
--rwxrwxrwx   0 ram       (1000) ram       (1000)    11030 2023-04-07 17:03:29.000000 pandas_dq-1.7/pandas_dq.egg-info/PKG-INFO
--rwxrwxrwx   0 ram       (1000) ram       (1000)      232 2023-04-07 17:03:29.000000 pandas_dq-1.7/pandas_dq.egg-info/SOURCES.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-04-07 17:03:29.000000 pandas_dq-1.7/pandas_dq.egg-info/dependency_links.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       49 2023-04-07 17:03:29.000000 pandas_dq-1.7/pandas_dq.egg-info/requires.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       10 2023-04-07 17:03:29.000000 pandas_dq-1.7/pandas_dq.egg-info/top_level.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)    43639 2023-04-07 16:46:41.000000 pandas_dq-1.7/pandas_dq.py
--rwxrwxrwx   0 ram       (1000) ram       (1000)       52 2023-04-07 12:15:09.000000 pandas_dq-1.7/requirements.txt
--rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-04-07 17:03:29.833721 pandas_dq-1.7/setup.cfg
--rwxrwxrwx   0 ram       (1000) ram       (1000)      883 2023-04-07 16:47:57.000000 pandas_dq-1.7/setup.py
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-07 22:22:56.949926 pandas_dq-1.8/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    11357 2023-04-02 23:27:15.000000 pandas_dq-1.8/LICENSE
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      610 2022-04-07 23:06:53.000000 pandas_dq-1.8/MANIFEST.in
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    11353 2023-04-07 22:22:56.945937 pandas_dq-1.8/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)     9530 2023-04-07 22:10:48.000000 pandas_dq-1.8/README.md
+drwxrwxrwx   0 ram       (1000) ram       (1000)        0 2023-04-07 22:22:56.913926 pandas_dq-1.8/pandas_dq.egg-info/
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    11353 2023-04-07 22:22:56.000000 pandas_dq-1.8/pandas_dq.egg-info/PKG-INFO
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      232 2023-04-07 22:22:56.000000 pandas_dq-1.8/pandas_dq.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)        1 2023-04-07 22:22:56.000000 pandas_dq-1.8/pandas_dq.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       49 2023-04-07 22:22:56.000000 pandas_dq-1.8/pandas_dq.egg-info/requires.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       10 2023-04-07 22:22:56.000000 pandas_dq-1.8/pandas_dq.egg-info/top_level.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)    44456 2023-04-07 22:17:06.000000 pandas_dq-1.8/pandas_dq.py
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       52 2023-04-07 12:15:09.000000 pandas_dq-1.8/requirements.txt
+-rwxrwxrwx   0 ram       (1000) ram       (1000)       38 2023-04-07 22:22:56.953927 pandas_dq-1.8/setup.cfg
+-rwxrwxrwx   0 ram       (1000) ram       (1000)      883 2023-04-07 21:49:21.000000 pandas_dq-1.8/setup.py
```

### Comparing `pandas_dq-1.7/LICENSE` & `pandas_dq-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_dq-1.7/MANIFEST.in` & `pandas_dq-1.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pandas_dq-1.7/PKG-INFO` & `pandas_dq-1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas_dq
-Version: 1.7
+Version: 1.8
 Summary: Clean your data using a scikit-learn transformer in a single line of code
 Home-page: https://github.com/AutoViML/pandas_dq
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # pandas_dq
         Analyze and clean your data in a single line of code with a Scikit-Learn compatible Transformer.
         
@@ -138,23 +138,24 @@
         ## API
         
         <p>
         pandas_dq has a very simple API with just two modules to import: one will find data quality issues in your data and the other will fix it. Simple!
         
         **Arguments**
         
-        `dq_report` has only 4 arguments:
-        - `data`: You can provide any kind of file format (string) or even a pandas DataFrame (df). It reads parquet, csv, feather, arrow, all kinds of file formats straight from disk. You just have to tell it the path to the file and the name of the file.
+        `dq_report` has only 4 arguments:<br>
+        <b>Caution:</b> For very large data sets, we randomly sample 100K rows from your CSV file to speed up reporting. If you want a larger sample, simply read in your file offline into a pandas dataframe and send it in as input, and we will load it as it is. This is one way to go around our speed limitations.
+        - `data`: You can provide any kind of file format (string) or even a pandas DataFrame (df). It reads parquet, csv, feather, arrow, all kinds of file formats straight from disk. You just have to tell it the path to the file and the name of the file. 
         - `target`: default: `None`. Otherwise, it should be a string name representing the name of a column in df. You can leave it as `None` if you don't want any target related issues.
         - `csv_engine`: default is `pandas`. If you want to load your CSV file using any other backend engine such as `arrow` or `parquet` please specify it here. This option only impacts CSV files.
         - `verbose`: This has 2 possible states:
           - `0` summary report. Prints only the summary level data quality issues in the dataset. Great for managers.
           - `1` detailed report. Prints all the gory details behind each DQ issue in your dataset and what to do about them. Great for engineers.
         
-        `Fix_DQ` has slightly more arguments:
+        `Fix_DQ` has slightly more arguments:<br>
         <b>Caution:</b> X_train and y_train in Fix_DQ must be pandas Dataframes or pandas Series. I have not tested it on numpy arrays. You can try your luck.
         
         - `quantile`: float (0.75): Define a threshold for IQR for outlier detection. Could be any float between 0 and 1. If quantile is set to `None`, then no outlier detection will take place.
         - `cat_fill_value`: string ("missing") or a dictionary: Define a fill value for missing categories in your object or categorical variables. This is a global default for your entire dataset. You can also give a dictionary where you specify different fill values for different columns.
         - `num_fill_value`: integer (99) or float value (999.0) or a dictionary: Define a fill value for missing numbers in your integer or float variables.  This is a global default for your entire dataset. You can also give a dictionary where you specify different fill values for different columns.
         - `rare_threshold`: float (0.05):  Define a threshold for rare categories. If a certain category in a column is less than say 5% (0.05) of samples, then it will be considered rare. All rare categories in that column will be merged under a new category named "Rare". 
         - `correlation_threshold`: float (0.8): Define a correlation limit. Anything above this limit, if two variables are correlated, one of them will be dropped. The program will tell you which variable is being dropped. You can switch the sequence of variables in your dataset if you want the one or other dropped.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pandas_dq Version: 1.7 Summary: Clean your data
+Metadata-Version: 2.1 Name: pandas_dq Version: 1.8 Summary: Clean your data
 using a scikit-learn transformer in a single line of code Home-page: https://
 github.com/AutoViML/pandas_dq Author: Ram Seshadri License: Apache License 2.0
 Description: # pandas_dq Analyze and clean your data in a single line of code
 with a Scikit-Learn compatible Transformer. # Table of Contents
     * What_is_pandas_dq
     * How_to_use_pandas_dq
     * How_to_install_pandas_dq
@@ -97,46 +97,51 @@
 X_test_transformed = fdq.transform(X_test) ``` ### if you are not using the
 Transformer, you can simply call the function, dq_report ``` from pandas_dq
 import dq_report dq_report(data, target=target, csv_engine="pandas", verbose=1)
 ``` It prints out a data quality report like this: ![dq_report](./images/
 dq_report_screenshot.png) ## API
 pandas_dq has a very simple API with just two modules to import: one will find
 data quality issues in your data and the other will fix it. Simple!
-**Arguments** `dq_report` has only 4 arguments: - `data`: You can provide any
-kind of file format (string) or even a pandas DataFrame (df). It reads parquet,
-csv, feather, arrow, all kinds of file formats straight from disk. You just
-have to tell it the path to the file and the name of the file. - `target`:
-default: `None`. Otherwise, it should be a string name representing the name of
-a column in df. You can leave it as `None` if you don't want any target related
-issues. - `csv_engine`: default is `pandas`. If you want to load your CSV file
-using any other backend engine such as `arrow` or `parquet` please specify it
-here. This option only impacts CSV files. - `verbose`: This has 2 possible
-states: - `0` summary report. Prints only the summary level data quality issues
-in the dataset. Great for managers. - `1` detailed report. Prints all the gory
-details behind each DQ issue in your dataset and what to do about them. Great
-for engineers. `Fix_DQ` has slightly more arguments: Caution: X_train and
-y_train in Fix_DQ must be pandas Dataframes or pandas Series. I have not tested
-it on numpy arrays. You can try your luck. - `quantile`: float (0.75): Define a
-threshold for IQR for outlier detection. Could be any float between 0 and 1. If
-quantile is set to `None`, then no outlier detection will take place. -
-`cat_fill_value`: string ("missing") or a dictionary: Define a fill value for
-missing categories in your object or categorical variables. This is a global
-default for your entire dataset. You can also give a dictionary where you
-specify different fill values for different columns. - `num_fill_value`:
-integer (99) or float value (999.0) or a dictionary: Define a fill value for
-missing numbers in your integer or float variables. This is a global default
-for your entire dataset. You can also give a dictionary where you specify
-different fill values for different columns. - `rare_threshold`: float (0.05):
-Define a threshold for rare categories. If a certain category in a column is
-less than say 5% (0.05) of samples, then it will be considered rare. All rare
-categories in that column will be merged under a new category named "Rare". -
-`correlation_threshold`: float (0.8): Define a correlation limit. Anything
-above this limit, if two variables are correlated, one of them will be dropped.
-The program will tell you which variable is being dropped. You can switch the
-sequence of variables in your dataset if you want the one or other dropped.
+**Arguments** `dq_report` has only 4 arguments:
+Caution: For very large data sets, we randomly sample 100K rows from your CSV
+file to speed up reporting. If you want a larger sample, simply read in your
+file offline into a pandas dataframe and send it in as input, and we will load
+it as it is. This is one way to go around our speed limitations. - `data`: You
+can provide any kind of file format (string) or even a pandas DataFrame (df).
+It reads parquet, csv, feather, arrow, all kinds of file formats straight from
+disk. You just have to tell it the path to the file and the name of the file. -
+`target`: default: `None`. Otherwise, it should be a string name representing
+the name of a column in df. You can leave it as `None` if you don't want any
+target related issues. - `csv_engine`: default is `pandas`. If you want to load
+your CSV file using any other backend engine such as `arrow` or `parquet`
+please specify it here. This option only impacts CSV files. - `verbose`: This
+has 2 possible states: - `0` summary report. Prints only the summary level data
+quality issues in the dataset. Great for managers. - `1` detailed report.
+Prints all the gory details behind each DQ issue in your dataset and what to do
+about them. Great for engineers. `Fix_DQ` has slightly more arguments:
+Caution: X_train and y_train in Fix_DQ must be pandas Dataframes or pandas
+Series. I have not tested it on numpy arrays. You can try your luck. -
+`quantile`: float (0.75): Define a threshold for IQR for outlier detection.
+Could be any float between 0 and 1. If quantile is set to `None`, then no
+outlier detection will take place. - `cat_fill_value`: string ("missing") or a
+dictionary: Define a fill value for missing categories in your object or
+categorical variables. This is a global default for your entire dataset. You
+can also give a dictionary where you specify different fill values for
+different columns. - `num_fill_value`: integer (99) or float value (999.0) or a
+dictionary: Define a fill value for missing numbers in your integer or float
+variables. This is a global default for your entire dataset. You can also give
+a dictionary where you specify different fill values for different columns. -
+`rare_threshold`: float (0.05): Define a threshold for rare categories. If a
+certain category in a column is less than say 5% (0.05) of samples, then it
+will be considered rare. All rare categories in that column will be merged
+under a new category named "Rare". - `correlation_threshold`: float (0.8):
+Define a correlation limit. Anything above this limit, if two variables are
+correlated, one of them will be dropped. The program will tell you which
+variable is being dropped. You can switch the sequence of variables in your
+dataset if you want the one or other dropped.
 ## Maintainers * [@AutoViML](https://github.com/AutoViML) ## Contributing See
 [the contributing file](CONTRIBUTING.md)! PRs accepted. ## License Apache
 License 2.0 Â© 2020 Ram Seshadri ## Note of Gratitude This libray would not
 have been possible without the help of ChatGPT and Bard. This library is
 dedicated to the thousands of people who worked to create LLM's. ## DISCLAIMER
 This project is not an official Google project. It is not supported by Google
 and Google specifically disclaims all warranties as to its quality,
```

### Comparing `pandas_dq-1.7/README.md` & `pandas_dq-1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -131,23 +131,24 @@
 ## API
 
 <p>
 pandas_dq has a very simple API with just two modules to import: one will find data quality issues in your data and the other will fix it. Simple!
 
 **Arguments**
 
-`dq_report` has only 4 arguments:
-- `data`: You can provide any kind of file format (string) or even a pandas DataFrame (df). It reads parquet, csv, feather, arrow, all kinds of file formats straight from disk. You just have to tell it the path to the file and the name of the file.
+`dq_report` has only 4 arguments:<br>
+<b>Caution:</b> For very large data sets, we randomly sample 100K rows from your CSV file to speed up reporting. If you want a larger sample, simply read in your file offline into a pandas dataframe and send it in as input, and we will load it as it is. This is one way to go around our speed limitations.
+- `data`: You can provide any kind of file format (string) or even a pandas DataFrame (df). It reads parquet, csv, feather, arrow, all kinds of file formats straight from disk. You just have to tell it the path to the file and the name of the file. 
 - `target`: default: `None`. Otherwise, it should be a string name representing the name of a column in df. You can leave it as `None` if you don't want any target related issues.
 - `csv_engine`: default is `pandas`. If you want to load your CSV file using any other backend engine such as `arrow` or `parquet` please specify it here. This option only impacts CSV files.
 - `verbose`: This has 2 possible states:
   - `0` summary report. Prints only the summary level data quality issues in the dataset. Great for managers.
   - `1` detailed report. Prints all the gory details behind each DQ issue in your dataset and what to do about them. Great for engineers.
 
-`Fix_DQ` has slightly more arguments:
+`Fix_DQ` has slightly more arguments:<br>
 <b>Caution:</b> X_train and y_train in Fix_DQ must be pandas Dataframes or pandas Series. I have not tested it on numpy arrays. You can try your luck.
 
 - `quantile`: float (0.75): Define a threshold for IQR for outlier detection. Could be any float between 0 and 1. If quantile is set to `None`, then no outlier detection will take place.
 - `cat_fill_value`: string ("missing") or a dictionary: Define a fill value for missing categories in your object or categorical variables. This is a global default for your entire dataset. You can also give a dictionary where you specify different fill values for different columns.
 - `num_fill_value`: integer (99) or float value (999.0) or a dictionary: Define a fill value for missing numbers in your integer or float variables.  This is a global default for your entire dataset. You can also give a dictionary where you specify different fill values for different columns.
 - `rare_threshold`: float (0.05):  Define a threshold for rare categories. If a certain category in a column is less than say 5% (0.05) of samples, then it will be considered rare. All rare categories in that column will be merged under a new category named "Rare". 
 - `correlation_threshold`: float (0.8): Define a correlation limit. Anything above this limit, if two variables are correlated, one of them will be dropped. The program will tell you which variable is being dropped. You can switch the sequence of variables in your dataset if you want the one or other dropped.
```

#### html2text {}

```diff
@@ -94,46 +94,51 @@
 X_test_transformed = fdq.transform(X_test) ``` ### if you are not using the
 Transformer, you can simply call the function, dq_report ``` from pandas_dq
 import dq_report dq_report(data, target=target, csv_engine="pandas", verbose=1)
 ``` It prints out a data quality report like this: ![dq_report](./images/
 dq_report_screenshot.png) ## API
 pandas_dq has a very simple API with just two modules to import: one will find
 data quality issues in your data and the other will fix it. Simple!
-**Arguments** `dq_report` has only 4 arguments: - `data`: You can provide any
-kind of file format (string) or even a pandas DataFrame (df). It reads parquet,
-csv, feather, arrow, all kinds of file formats straight from disk. You just
-have to tell it the path to the file and the name of the file. - `target`:
-default: `None`. Otherwise, it should be a string name representing the name of
-a column in df. You can leave it as `None` if you don't want any target related
-issues. - `csv_engine`: default is `pandas`. If you want to load your CSV file
-using any other backend engine such as `arrow` or `parquet` please specify it
-here. This option only impacts CSV files. - `verbose`: This has 2 possible
-states: - `0` summary report. Prints only the summary level data quality issues
-in the dataset. Great for managers. - `1` detailed report. Prints all the gory
-details behind each DQ issue in your dataset and what to do about them. Great
-for engineers. `Fix_DQ` has slightly more arguments: Caution: X_train and
-y_train in Fix_DQ must be pandas Dataframes or pandas Series. I have not tested
-it on numpy arrays. You can try your luck. - `quantile`: float (0.75): Define a
-threshold for IQR for outlier detection. Could be any float between 0 and 1. If
-quantile is set to `None`, then no outlier detection will take place. -
-`cat_fill_value`: string ("missing") or a dictionary: Define a fill value for
-missing categories in your object or categorical variables. This is a global
-default for your entire dataset. You can also give a dictionary where you
-specify different fill values for different columns. - `num_fill_value`:
-integer (99) or float value (999.0) or a dictionary: Define a fill value for
-missing numbers in your integer or float variables. This is a global default
-for your entire dataset. You can also give a dictionary where you specify
-different fill values for different columns. - `rare_threshold`: float (0.05):
-Define a threshold for rare categories. If a certain category in a column is
-less than say 5% (0.05) of samples, then it will be considered rare. All rare
-categories in that column will be merged under a new category named "Rare". -
-`correlation_threshold`: float (0.8): Define a correlation limit. Anything
-above this limit, if two variables are correlated, one of them will be dropped.
-The program will tell you which variable is being dropped. You can switch the
-sequence of variables in your dataset if you want the one or other dropped.
+**Arguments** `dq_report` has only 4 arguments:
+Caution: For very large data sets, we randomly sample 100K rows from your CSV
+file to speed up reporting. If you want a larger sample, simply read in your
+file offline into a pandas dataframe and send it in as input, and we will load
+it as it is. This is one way to go around our speed limitations. - `data`: You
+can provide any kind of file format (string) or even a pandas DataFrame (df).
+It reads parquet, csv, feather, arrow, all kinds of file formats straight from
+disk. You just have to tell it the path to the file and the name of the file. -
+`target`: default: `None`. Otherwise, it should be a string name representing
+the name of a column in df. You can leave it as `None` if you don't want any
+target related issues. - `csv_engine`: default is `pandas`. If you want to load
+your CSV file using any other backend engine such as `arrow` or `parquet`
+please specify it here. This option only impacts CSV files. - `verbose`: This
+has 2 possible states: - `0` summary report. Prints only the summary level data
+quality issues in the dataset. Great for managers. - `1` detailed report.
+Prints all the gory details behind each DQ issue in your dataset and what to do
+about them. Great for engineers. `Fix_DQ` has slightly more arguments:
+Caution: X_train and y_train in Fix_DQ must be pandas Dataframes or pandas
+Series. I have not tested it on numpy arrays. You can try your luck. -
+`quantile`: float (0.75): Define a threshold for IQR for outlier detection.
+Could be any float between 0 and 1. If quantile is set to `None`, then no
+outlier detection will take place. - `cat_fill_value`: string ("missing") or a
+dictionary: Define a fill value for missing categories in your object or
+categorical variables. This is a global default for your entire dataset. You
+can also give a dictionary where you specify different fill values for
+different columns. - `num_fill_value`: integer (99) or float value (999.0) or a
+dictionary: Define a fill value for missing numbers in your integer or float
+variables. This is a global default for your entire dataset. You can also give
+a dictionary where you specify different fill values for different columns. -
+`rare_threshold`: float (0.05): Define a threshold for rare categories. If a
+certain category in a column is less than say 5% (0.05) of samples, then it
+will be considered rare. All rare categories in that column will be merged
+under a new category named "Rare". - `correlation_threshold`: float (0.8):
+Define a correlation limit. Anything above this limit, if two variables are
+correlated, one of them will be dropped. The program will tell you which
+variable is being dropped. You can switch the sequence of variables in your
+dataset if you want the one or other dropped.
 ## Maintainers * [@AutoViML](https://github.com/AutoViML) ## Contributing See
 [the contributing file](CONTRIBUTING.md)! PRs accepted. ## License Apache
 License 2.0 Â© 2020 Ram Seshadri ## Note of Gratitude This libray would not
 have been possible without the help of ChatGPT and Bard. This library is
 dedicated to the thousands of people who worked to create LLM's. ## DISCLAIMER
 This project is not an official Google project. It is not supported by Google
 and Google specifically disclaims all warranties as to its quality,
```

### Comparing `pandas_dq-1.7/pandas_dq.egg-info/PKG-INFO` & `pandas_dq-1.8/pandas_dq.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-dq
-Version: 1.7
+Version: 1.8
 Summary: Clean your data using a scikit-learn transformer in a single line of code
 Home-page: https://github.com/AutoViML/pandas_dq
 Author: Ram Seshadri
 License: Apache License 2.0
 Description: # pandas_dq
         Analyze and clean your data in a single line of code with a Scikit-Learn compatible Transformer.
         
@@ -138,23 +138,24 @@
         ## API
         
         <p>
         pandas_dq has a very simple API with just two modules to import: one will find data quality issues in your data and the other will fix it. Simple!
         
         **Arguments**
         
-        `dq_report` has only 4 arguments:
-        - `data`: You can provide any kind of file format (string) or even a pandas DataFrame (df). It reads parquet, csv, feather, arrow, all kinds of file formats straight from disk. You just have to tell it the path to the file and the name of the file.
+        `dq_report` has only 4 arguments:<br>
+        <b>Caution:</b> For very large data sets, we randomly sample 100K rows from your CSV file to speed up reporting. If you want a larger sample, simply read in your file offline into a pandas dataframe and send it in as input, and we will load it as it is. This is one way to go around our speed limitations.
+        - `data`: You can provide any kind of file format (string) or even a pandas DataFrame (df). It reads parquet, csv, feather, arrow, all kinds of file formats straight from disk. You just have to tell it the path to the file and the name of the file. 
         - `target`: default: `None`. Otherwise, it should be a string name representing the name of a column in df. You can leave it as `None` if you don't want any target related issues.
         - `csv_engine`: default is `pandas`. If you want to load your CSV file using any other backend engine such as `arrow` or `parquet` please specify it here. This option only impacts CSV files.
         - `verbose`: This has 2 possible states:
           - `0` summary report. Prints only the summary level data quality issues in the dataset. Great for managers.
           - `1` detailed report. Prints all the gory details behind each DQ issue in your dataset and what to do about them. Great for engineers.
         
-        `Fix_DQ` has slightly more arguments:
+        `Fix_DQ` has slightly more arguments:<br>
         <b>Caution:</b> X_train and y_train in Fix_DQ must be pandas Dataframes or pandas Series. I have not tested it on numpy arrays. You can try your luck.
         
         - `quantile`: float (0.75): Define a threshold for IQR for outlier detection. Could be any float between 0 and 1. If quantile is set to `None`, then no outlier detection will take place.
         - `cat_fill_value`: string ("missing") or a dictionary: Define a fill value for missing categories in your object or categorical variables. This is a global default for your entire dataset. You can also give a dictionary where you specify different fill values for different columns.
         - `num_fill_value`: integer (99) or float value (999.0) or a dictionary: Define a fill value for missing numbers in your integer or float variables.  This is a global default for your entire dataset. You can also give a dictionary where you specify different fill values for different columns.
         - `rare_threshold`: float (0.05):  Define a threshold for rare categories. If a certain category in a column is less than say 5% (0.05) of samples, then it will be considered rare. All rare categories in that column will be merged under a new category named "Rare". 
         - `correlation_threshold`: float (0.8): Define a correlation limit. Anything above this limit, if two variables are correlated, one of them will be dropped. The program will tell you which variable is being dropped. You can switch the sequence of variables in your dataset if you want the one or other dropped.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pandas-dq Version: 1.7 Summary: Clean your data
+Metadata-Version: 2.1 Name: pandas-dq Version: 1.8 Summary: Clean your data
 using a scikit-learn transformer in a single line of code Home-page: https://
 github.com/AutoViML/pandas_dq Author: Ram Seshadri License: Apache License 2.0
 Description: # pandas_dq Analyze and clean your data in a single line of code
 with a Scikit-Learn compatible Transformer. # Table of Contents
     * What_is_pandas_dq
     * How_to_use_pandas_dq
     * How_to_install_pandas_dq
@@ -97,46 +97,51 @@
 X_test_transformed = fdq.transform(X_test) ``` ### if you are not using the
 Transformer, you can simply call the function, dq_report ``` from pandas_dq
 import dq_report dq_report(data, target=target, csv_engine="pandas", verbose=1)
 ``` It prints out a data quality report like this: ![dq_report](./images/
 dq_report_screenshot.png) ## API
 pandas_dq has a very simple API with just two modules to import: one will find
 data quality issues in your data and the other will fix it. Simple!
-**Arguments** `dq_report` has only 4 arguments: - `data`: You can provide any
-kind of file format (string) or even a pandas DataFrame (df). It reads parquet,
-csv, feather, arrow, all kinds of file formats straight from disk. You just
-have to tell it the path to the file and the name of the file. - `target`:
-default: `None`. Otherwise, it should be a string name representing the name of
-a column in df. You can leave it as `None` if you don't want any target related
-issues. - `csv_engine`: default is `pandas`. If you want to load your CSV file
-using any other backend engine such as `arrow` or `parquet` please specify it
-here. This option only impacts CSV files. - `verbose`: This has 2 possible
-states: - `0` summary report. Prints only the summary level data quality issues
-in the dataset. Great for managers. - `1` detailed report. Prints all the gory
-details behind each DQ issue in your dataset and what to do about them. Great
-for engineers. `Fix_DQ` has slightly more arguments: Caution: X_train and
-y_train in Fix_DQ must be pandas Dataframes or pandas Series. I have not tested
-it on numpy arrays. You can try your luck. - `quantile`: float (0.75): Define a
-threshold for IQR for outlier detection. Could be any float between 0 and 1. If
-quantile is set to `None`, then no outlier detection will take place. -
-`cat_fill_value`: string ("missing") or a dictionary: Define a fill value for
-missing categories in your object or categorical variables. This is a global
-default for your entire dataset. You can also give a dictionary where you
-specify different fill values for different columns. - `num_fill_value`:
-integer (99) or float value (999.0) or a dictionary: Define a fill value for
-missing numbers in your integer or float variables. This is a global default
-for your entire dataset. You can also give a dictionary where you specify
-different fill values for different columns. - `rare_threshold`: float (0.05):
-Define a threshold for rare categories. If a certain category in a column is
-less than say 5% (0.05) of samples, then it will be considered rare. All rare
-categories in that column will be merged under a new category named "Rare". -
-`correlation_threshold`: float (0.8): Define a correlation limit. Anything
-above this limit, if two variables are correlated, one of them will be dropped.
-The program will tell you which variable is being dropped. You can switch the
-sequence of variables in your dataset if you want the one or other dropped.
+**Arguments** `dq_report` has only 4 arguments:
+Caution: For very large data sets, we randomly sample 100K rows from your CSV
+file to speed up reporting. If you want a larger sample, simply read in your
+file offline into a pandas dataframe and send it in as input, and we will load
+it as it is. This is one way to go around our speed limitations. - `data`: You
+can provide any kind of file format (string) or even a pandas DataFrame (df).
+It reads parquet, csv, feather, arrow, all kinds of file formats straight from
+disk. You just have to tell it the path to the file and the name of the file. -
+`target`: default: `None`. Otherwise, it should be a string name representing
+the name of a column in df. You can leave it as `None` if you don't want any
+target related issues. - `csv_engine`: default is `pandas`. If you want to load
+your CSV file using any other backend engine such as `arrow` or `parquet`
+please specify it here. This option only impacts CSV files. - `verbose`: This
+has 2 possible states: - `0` summary report. Prints only the summary level data
+quality issues in the dataset. Great for managers. - `1` detailed report.
+Prints all the gory details behind each DQ issue in your dataset and what to do
+about them. Great for engineers. `Fix_DQ` has slightly more arguments:
+Caution: X_train and y_train in Fix_DQ must be pandas Dataframes or pandas
+Series. I have not tested it on numpy arrays. You can try your luck. -
+`quantile`: float (0.75): Define a threshold for IQR for outlier detection.
+Could be any float between 0 and 1. If quantile is set to `None`, then no
+outlier detection will take place. - `cat_fill_value`: string ("missing") or a
+dictionary: Define a fill value for missing categories in your object or
+categorical variables. This is a global default for your entire dataset. You
+can also give a dictionary where you specify different fill values for
+different columns. - `num_fill_value`: integer (99) or float value (999.0) or a
+dictionary: Define a fill value for missing numbers in your integer or float
+variables. This is a global default for your entire dataset. You can also give
+a dictionary where you specify different fill values for different columns. -
+`rare_threshold`: float (0.05): Define a threshold for rare categories. If a
+certain category in a column is less than say 5% (0.05) of samples, then it
+will be considered rare. All rare categories in that column will be merged
+under a new category named "Rare". - `correlation_threshold`: float (0.8):
+Define a correlation limit. Anything above this limit, if two variables are
+correlated, one of them will be dropped. The program will tell you which
+variable is being dropped. You can switch the sequence of variables in your
+dataset if you want the one or other dropped.
 ## Maintainers * [@AutoViML](https://github.com/AutoViML) ## Contributing See
 [the contributing file](CONTRIBUTING.md)! PRs accepted. ## License Apache
 License 2.0 Â© 2020 Ram Seshadri ## Note of Gratitude This libray would not
 have been possible without the help of ChatGPT and Bard. This library is
 dedicated to the thousands of people who worked to create LLM's. ## DISCLAIMER
 This project is not an official Google project. It is not supported by Google
 and Google specifically disclaims all warranties as to its quality,
```

### Comparing `pandas_dq-1.7/pandas_dq.py` & `pandas_dq-1.8/pandas_dq.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,34 +65,46 @@
         print("This is a summary report. Change verbose to 1 to see more details on each DQ issue.")
     # Check if the input is a string or a dataframe
     if isinstance(data, str):
         # Get the file extension
         ext = os.path.splitext(data)[-1]
         # Load the file into a pandas dataframe based on the extension
         if ext == ".csv":
+            print("If large dataset, we will randomly sample 100K rows to speed up processing...")
             if csv_engine == 'pandas':
                 # Upload the data file into Pandas
-                df = pd.read_csv(data, nrows=1000000)
+                df = pd.read_csv(data)
             elif csv_engine == 'polars':
                 # Upload the data file into Polars
                 import polars as pl
-                df_polars = pl.read_csv(data, nrows=1000000)
+                df = pl.read_csv(data)
             elif csv_engine == 'parquet':
                 # Upload the data file into Parquet
                 import pyarrow as pa
-                df_parquet = pa.read_table(data)
+                df = pa.read_table(data)
+            else :
+                # print the pandas version
+                if str(pd.__version__)[0] == '2':
+                    print(f"pandas version={pd.__version__}. Hence using pyarrow backend.")
+                    df = pd.read_csv(data, engine='pyarrow', dtype_backend='pyarrow')
+                else:
+                    print(f"pandas version={pd.__version__}. Hence using pandas backend.")
+                    df = pd.read_csv(data)
         elif ext == ".parquet":
             df = pd.read_parquet(data)
-        elif ext in [".feather", ".arrow"]:
+        elif ext in [".feather", ".arrow", "ftr"]:
             df = pd.read_feather(data)
         else:
             print("Unsupported file format. Please use CSV, parquet, feather or arrow.")
-            return
+            return data
+        ######## This is to sample the data if it is too large ###
+        if df.shape[0] >= 1000000:
+            df = df.sample(100000)
     elif isinstance(data, pd.DataFrame):
-        # Use the input dataframe as is
+        print("We use the input dataframe as is...")
         df = data
     else:
         print("Invalid input. Please provide a string (filename) or a dataframe.")
         return
 
     ### This is the column that lists our data quality issues
     new_col = 'DQ Issue'
@@ -108,32 +120,33 @@
     # Create an empty dataframe to store the data quality issues
     data_types = pd.DataFrame(
         df.dtypes,
         columns=['Data Type']
     )
 
     missing_values = df.isnull().sum()
+    missing_values_pct = ((df.isnull().sum()/df.shape[0])*100)
     missing_cols = missing_values[missing_values > 0].index.tolist()
     number_cols = df.select_dtypes(include=["integer", "float"]).columns.tolist() # Get numerical columns
     float_cols = df.select_dtypes(include=[ "float"]).columns.tolist() # Get float columns
     id_cols = []
     zero_var_cols = []
 
     missing_data = pd.DataFrame(
-        missing_values,
-        columns=['Missing Values']
+        missing_values_pct,
+        columns=['Missing Values%']
     )
     unique_values = pd.DataFrame(
-        columns=['Unique Values']
+        columns=['Unique Values%']
     )
     for row in list(df.columns.values):
         if row in float_cols:
             unique_values.loc[row] = ["NA"]
         else:
-            unique_values.loc[row] = [df[row].nunique()]
+            unique_values.loc[row] = [int(100*df[row].nunique()/df.shape[0])]
             if df[row].nunique() == df.shape[0]:
                 id_cols.append(row)
             elif df[row].nunique() == 1:
                 zero_var_cols.append(row)
         
     maximum_values = pd.DataFrame(
         columns=['Maximum Value']
@@ -306,15 +319,15 @@
                 outlier_cols.append(col)
                 if first_time:
                     new_string = f"There are {len(num_cols)} numerical columns, some with outliers. Remove them or use robust statistics."
                     dq_df1.loc[bad_col,new_col] += dq_df1.loc[bad_col,'first_comma'] + new_string
                     dq_df1.loc[bad_col,'first_comma'] = ', '
                     first_time =False
                 ### check if there are outlier columns and print them ##
-                new_string = f"has {len(outliers)} outliers greater than upper bound ({upper_bound}) or lower than lower bound: {lower_bound}. Cap them or remove them."
+                new_string = f"has {len(outliers)} outliers greater than upper bound ({upper_bound}) or lower than lower bound({lower_bound}). Cap them or remove them."
                 dq_df2.loc[col,new_col] += dq_df2.loc[col,'first_comma'] + new_string
                 dq_df2.loc[col,'first_comma'] = ', '
         if len(outlier_cols) < 1:
             new_string =  f"There are no numeric columns with outliers in this dataset"
             dq_df1.loc[good_col,new_col] += dq_df1.loc[good_col,'first_comma'] + new_string
             dq_df1.loc[good_col,'first_comma'] = ', '
                 
@@ -323,15 +336,15 @@
     cardinality = df[cat_cols].nunique() # Get the number of unique values in each categorical column
     high_card_cols = cardinality[cardinality > cardinality_threshold].index.tolist() # Get the columns with high cardinality
     if len(high_card_cols) > 0:
         new_string = f"There are {len(high_card_cols)} columns with high cardinality (>{cardinality_threshold} categories) in the dataset. Reduce them using encoding techniques or feature selection methods."
         dq_df1.loc[bad_col,new_col] += dq_df1.loc[bad_col,'first_comma'] + new_string
         dq_df1.loc[bad_col,'first_comma'] = ', '
         for col in high_card_cols:
-            new_string = f"high cardinality with {cardinality[col]} unique values."
+            new_string = f"high cardinality with {cardinality[col]} unique values: Use hash encoding or embedding to reduce dimension."
             dq_df2.loc[col,new_col] += dq_df2.loc[col,'first_comma'] + new_string
             dq_df2.loc[col,'first_comma'] = ', '
     else:
         new_string =  f"There are no high cardinality columns in this dataset"
         dq_df1.loc[good_col,new_col] += dq_df1.loc[good_col,'first_comma'] + new_string
         dq_df1.loc[good_col,'first_comma'] = ', '
 
@@ -802,12 +815,12 @@
         transformed_X = self.transform_skewed(rare_X)
                 
         # Return the transformed DataFrame
         return transformed_X
 
 ############################################################################################
 module_type = 'Running' if  __name__ == "__main__" else 'Imported'
-version_number =  '1.7'
+version_number =  '1.8'
 print(f"""{module_type} pandas_dq ({version_number}). Always upgrade to get latest version.
 from pandas_dq import dq_report, Fix_DQ
 """)
 #################################################################################
```

### Comparing `pandas_dq-1.7/setup.py` & `pandas_dq-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pandas_dq",
-    version="1.7",
+    version="1.8",
     author="Ram Seshadri",
     # author_email="author@example.com",
     description="Clean your data using a scikit-learn transformer in a single line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License 2.0',
     url="https://github.com/AutoViML/pandas_dq",
```

