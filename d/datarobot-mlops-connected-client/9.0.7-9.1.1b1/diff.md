# Comparing `tmp/datarobot_mlops_connected_client-9.0.7-py3-none-any.whl.zip` & `tmp/datarobot_mlops_connected_client-9.1.1b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 39875 bytes, number of entries: 13
--rw-r--r--  2.0 unx      597 b- defN 23-Apr-07 22:16 datarobot/mlops/__init__.py
--rw-r--r--  2.0 unx      532 b- defN 23-Apr-07 22:16 datarobot/mlops/connected/__init__.py
--rw-r--r--  2.0 unx    98234 b- defN 23-Apr-07 22:16 datarobot/mlops/connected/client.py
--rw-r--r--  2.0 unx     1231 b- defN 23-Apr-07 22:16 datarobot/mlops/connected/enums.py
--rw-r--r--  2.0 unx      931 b- defN 23-Apr-07 22:16 datarobot/mlops/connected/exception.py
--rw-r--r--  2.0 unx    97624 b- defN 23-Apr-07 22:16 datarobot/mlops/connected/mlops_cli.py
--rw-r--r--  2.0 unx     2694 b- defN 23-Apr-07 22:16 datarobot/mlops/connected/upload_tracker.py
--rw-r--r--  2.0 unx    10281 b- defN 23-Apr-07 22:16 datarobot/mlops/connected/url_helper.py
--rw-r--r--  2.0 unx     1510 b- defN 23-Apr-07 22:22 datarobot_mlops_connected_client-9.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 22:22 datarobot_mlops_connected_client-9.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       71 b- defN 23-Apr-07 22:22 datarobot_mlops_connected_client-9.0.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-07 22:22 datarobot_mlops_connected_client-9.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1265 b- defN 23-Apr-07 22:22 datarobot_mlops_connected_client-9.0.7.dist-info/RECORD
-13 files, 215072 bytes uncompressed, 37697 bytes compressed:  82.5%
+Zip file size: 39453 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      597 b- defN 23-Mar-27 23:33 datarobot/mlops/__init__.py
+-rw-r--r--  2.0 unx      532 b- defN 23-Mar-27 23:33 datarobot/mlops/connected/__init__.py
+-rw-r--r--  2.0 unx    94846 b- defN 23-Mar-27 23:33 datarobot/mlops/connected/client.py
+-rw-r--r--  2.0 unx     1231 b- defN 23-Mar-27 23:33 datarobot/mlops/connected/enums.py
+-rw-r--r--  2.0 unx      900 b- defN 23-Mar-27 23:33 datarobot/mlops/connected/exception.py
+-rw-r--r--  2.0 unx    96728 b- defN 23-Mar-27 23:33 datarobot/mlops/connected/mlops_cli.py
+-rw-r--r--  2.0 unx     2646 b- defN 23-Mar-27 23:33 datarobot/mlops/connected/upload_tracker.py
+-rw-r--r--  2.0 unx    10251 b- defN 23-Mar-27 23:33 datarobot/mlops/connected/url_helper.py
+-rw-r--r--  2.0 unx     1536 b- defN 23-Mar-27 23:38 datarobot_mlops_connected_client-9.1.1b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-27 23:38 datarobot_mlops_connected_client-9.1.1b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Mar-27 23:38 datarobot_mlops_connected_client-9.1.1b1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Mar-27 23:38 datarobot_mlops_connected_client-9.1.1b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1275 b- defN 23-Mar-27 23:38 datarobot_mlops_connected_client-9.1.1b1.dist-info/RECORD
+13 files, 210716 bytes uncompressed, 37255 bytes compressed:  82.3%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: datarobot/mlops/connected/upload_tracker.py
 Comment: 
 
 Filename: datarobot/mlops/connected/url_helper.py
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.0.7.dist-info/METADATA
+Filename: datarobot_mlops_connected_client-9.1.1b1.dist-info/METADATA
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.0.7.dist-info/WHEEL
+Filename: datarobot_mlops_connected_client-9.1.1b1.dist-info/WHEEL
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.0.7.dist-info/entry_points.txt
+Filename: datarobot_mlops_connected_client-9.1.1b1.dist-info/entry_points.txt
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.0.7.dist-info/top_level.txt
+Filename: datarobot_mlops_connected_client-9.1.1b1.dist-info/top_level.txt
 Comment: 
 
-Filename: datarobot_mlops_connected_client-9.0.7.dist-info/RECORD
+Filename: datarobot_mlops_connected_client-9.1.1b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datarobot/mlops/connected/client.py

```diff
@@ -18,27 +18,29 @@
 import tempfile
 import time
 import warnings
 from contextlib import suppress
 
 import aiohttp
 import requests
+
 from datarobot.mlops.common.aggregation_util import convert_aggregated_stats_features_to_dr_format
 from datarobot.mlops.common.aggregation_util import (
     convert_aggregated_stats_predictions_to_dr_format,
 )
 from datarobot.mlops.common.aggregation_util import (
     convert_aggregated_stats_segment_attr_to_dr_format,
 )
 from datarobot.mlops.common.config import ConfigConstants
 from datarobot.mlops.common.config import get_config_default
 from datarobot.mlops.common.enums import DataFormat
 from datarobot.mlops.common.exception import DRNotFoundException
 from datarobot.mlops.common.exception import DRUnsupportedType
 from datarobot.mlops.common.prediction_util import get_predictions
+from datarobot.mlops.common.version_util import DataRobotAppVersion
 from datarobot.mlops.connected.enums import DatasetSourceType
 from datarobot.mlops.connected.enums import HTTPStatus
 from datarobot.mlops.connected.url_helper import MMMEndpoint
 from datarobot.mlops.constants import Constants
 from datarobot.mlops.json_shim import default_serializer
 from datarobot.mlops.json_shim import json_dumps_bytes
 from datarobot.mlops.metric import AggregatedStats
@@ -50,86 +52,28 @@
 from datarobot.mlops.metric import SerializationConstants
 
 from .exception import DRMLOpsConnectedException
 from .url_helper import URLBuilder
 
 logger = logging.getLogger(__name__)
 
-
-class MMMLimits:
-    DATA_REPORTING_MAX_CHUNKS = 100
-    DATA_REPORTING_MAX_LINES_PER_CHUNK = 100
-    ACTUALS_REPORTING_MAX_LINES = 10000
-
-
 agg_stats_data_keys = SerializationConstants.AggregatedStatsConstants
 predictions_data_keys = SerializationConstants.PredictionsDataConstants
 common_fields_keys = SerializationConstants.GeneralConstants
 
-
-class DataRobotAppVersion(object):
-    def __init__(self, string_version=None, major=None, minor=None, patch=None):
-        if string_version is not None:
-            versions = string_version.split(".")
-            if len(versions) < 3:
-                raise ValueError(
-                    "DataRobot App version in string form should have syntax \"x.y.z\" "
-                    "where x, y and z are integers"
-                )
-            major = versions[0]
-            minor = versions[1]
-            patch = versions[2]
-        elif major is None or minor is None or patch is None:
-            raise ValueError(
-                "DataRobot App version needs to be specified either as a string \"x.y.z\" "
-                "or integer values for major, minor, patch"
-            )
-
-        self._major = int(major)
-        self._minor = int(minor)
-        self._patch = int(patch)
-
-    def __str__(self):
-        return "{}.{}.{}".format(self._major, self._minor, self._patch)
-
-    @property
-    def major(self):
-        return self._major
-
-    @property
-    def minor(self):
-        return self._minor
-
-    @property
-    def patch(self):
-        return self._patch
-
-    def is_newer_or_equal(self, datarobot_app_compare_version):
-        """
-        Checks if "this" version is newer or equal to the version input as an argument
-        :param datarobot_app_compare_version:
-        :return:
-        """
-        if self._major > datarobot_app_compare_version.major:
-            return True
-        if self._major < datarobot_app_compare_version.major:
-            return False
-        # At this point major versions are equal
-        if self._minor > datarobot_app_compare_version.minor:
-            return True
-        if self._minor < datarobot_app_compare_version.minor:
-            return False
-        # At this point major and minor versions are equal
-        return self._patch >= datarobot_app_compare_version.patch
+DATAROBOT_APP_VERSION_WITH_SKIP_AGGREGATION_SUPPORT = DataRobotAppVersion(major=8, minor=0, patch=6)
 
 
-DATAROBOT_APP_VERSION_WITH_SKIP_AGGREGATION_SUPPORT = DataRobotAppVersion(major=8, minor=0, patch=6)
+class MMMLimits:
+    DATA_REPORTING_MAX_CHUNKS = 100
+    DATA_REPORTING_MAX_LINES_PER_CHUNK = 100
+    ACTUALS_REPORTING_MAX_LINES = 10000
 
 
-class MLOpsClient(object):
+class MLOpsClient:
     """
     This class provides helper methods to communicate with
     DataRobot MLOps.
     *Note*: These class methods can only be run from a node
     with connectivity to DataRobot MLOps.
 
     :param service_url: DataRobot MLOps URL
@@ -247,15 +191,15 @@
 
         while time.time() < start_time + max_wait:
             response = self._get_url_request_response(async_location, allow_redirects=False)
             if response.status_code == HTTPStatus.SEE_OTHER:
                 return response.headers[MLOpsClient.RESPONSE_LOCATION_KEY]
             if response.status_code != HTTPStatus.OK:
                 raise DRMLOpsConnectedException(
-                    "Call {} failed; text: [{}]".format(async_location, response.text)
+                    f"Call {async_location} failed; text: [{response.text}]"
                 )
             data = response.json()
             if MLOpsClient.RESPONSE_STATUS_KEY in data:
                 async_status = data[MLOpsClient.RESPONSE_STATUS_KEY].lower()
                 if async_status in [
                     MLOpsClient.ASYNC_STATUS_INITIALIZED,
                     MLOpsClient.ASYNC_STATUS_RUNNING,
@@ -265,26 +209,24 @@
                     return True
                 elif async_status in [
                     MLOpsClient.ASYNC_STATUS_ABORT,
                     MLOpsClient.ASYNC_STATUS_ERROR,
                 ]:
                     raise DRMLOpsConnectedException(str(data))
                 else:
-                    raise DRMLOpsConnectedException(
-                        "Task status '{}' is not valid".format(async_status)
-                    )
+                    raise DRMLOpsConnectedException(f"Task status '{async_status}' is not valid")
             else:
                 return True
             logger.debug(
                 "Retrying request to %s in %s seconds.",
                 async_location,
                 MLOpsClient.ASYNC_WAIT_SLEEP_TIME,
             )
             time.sleep(MLOpsClient.ASYNC_WAIT_SLEEP_TIME)
-        raise RuntimeError("Client timed out waiting for {} to resolve".format(async_location))
+        raise RuntimeError(f"Client timed out waiting for {async_location} to resolve")
 
     def update_api_version(self):
         url = self._service_url + "/" + MMMEndpoint.API_VERSION
         headers = dict(self._common_headers)
         try:
             response = requests.get(url, headers=headers, verify=self._verify)
             if response.ok:
@@ -293,20 +235,18 @@
                 self._api_minor_version = response.json()[MLOpsClient.RESPONSE_API_MINOR_VERSION]
             else:
                 if "invalid authorization header" in response.text.lower():
                     raise DRMLOpsConnectedException(
                         "Call {} failed: invalid Authorization header. "
                         "Make sure you have supplied a valid API token.".format(url)
                     )
-                raise DRMLOpsConnectedException(
-                    "Call {} failed; text: [{}]".format(url, response.text)
-                )
+                raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def update_datarobot_app_version(self):
         """
         Placeholder method to query the DataRobot App version if and when it is available
         :return:
         """
@@ -335,35 +275,33 @@
             # GONE when deployment was previously deleted
             # NOT_FOUND if deployment was already deleted or user has no permission to delete
             # 422 if an application is currently associated with the deployment
             if response.status_code in [HTTPStatus.NO_CONTENT]:
                 return
             if response.status_code == HTTPStatus.ACCEPTED:
                 if wait_for_result:
-                    logger.info(
-                        "Waiting up to {} seconds for operation to complete...".format(timeout)
-                    )
+                    logger.info(f"Waiting up to {timeout} seconds for operation to complete...")
                     self._wait_for_async_completion(
                         response.headers[MLOpsClient.RESPONSE_LOCATION_KEY], timeout
                     )
                 return
             if response.status_code == HTTPStatus.NOT_FOUND:
-                raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
             if response.status_code == HTTPStatus.IN_USE:
                 raise DRMLOpsConnectedException(
-                    "Call {} failed; deployment ID {} in use.".format(url, deployment_id)
+                    f"Call {url} failed; deployment ID {deployment_id} in use."
                 )
             raise DRMLOpsConnectedException(
                 "Call {} failed; unexpected status code: {}; text:[{}]".format(
                     url, response.status_code, response.text
                 )
             )
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def upload_dataset(self, dataset_filepath, timeout=180, dry_run=False):
         """
         Upload a dataset (from a CSV file) into DataRobot MLOps
 
         :param dataset_filepath: path to a CSV dataset file
@@ -396,15 +334,15 @@
                     raise DRMLOpsConnectedException(
                         "Call {} with filename {} failed; text:[{}]".format(
                             url, dataset_filepath, response.text
                         )
                     )
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def upload_dataframe(self, df, filename=None, timeout=180, dry_run=False):
         """
         Upload a DataFrame to MLOps.  Internally, a DataFrame is serialized to CSV and then
         uploaded to AI Catalog.  Filename is used just as display name; no actual file is created.
 
@@ -435,19 +373,19 @@
             if response.ok:
                 self._wait_for_async_completion(
                     response.headers[MLOpsClient.RESPONSE_LOCATION_KEY], timeout
                 )
                 return response.json()[MLOpsClient.RESPONSE_CATALOG_ID_KEY]
             else:
                 raise DRMLOpsConnectedException(
-                    "Call {} for DataFrame failed; text:[{}]".format(url, response.text)
+                    f"Call {url} for DataFrame failed; text:[{response.text}]"
                 )
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def _get_url_request_response(self, url, allow_redirects=True, params=None):
         return requests.get(
             url,
             headers=self._common_headers,
             allow_redirects=allow_redirects,
@@ -480,28 +418,24 @@
         :type timeout: int
         :returns: True if association succeeded
         :raises DRUnsupportedType: if data source type is not supported
         :raises DRMLOpsConnectedException: if association failed
         """
 
         if not isinstance(data_source_type, DatasetSourceType):
-            raise DRUnsupportedType(
-                "data_source_type must be of type '{}'".format(DatasetSourceType)
-            )
+            raise DRUnsupportedType(f"data_source_type must be of type '{DatasetSourceType}'")
 
         if data_source_type == DatasetSourceType.TRAINING:
             raise DRMLOpsConnectedException(
                 "Associating training data with deployments is not allowed. "
                 "Instead associate training data with the model package."
             )
 
         if data_source_type != DatasetSourceType.SCORING:
-            raise DRMLOpsConnectedException(
-                "Invalid data source type '{}'".format(data_source_type)
-            )
+            raise DRMLOpsConnectedException(f"Invalid data source type '{data_source_type}'")
 
         payload = {
             "datasetId": dataset_id,
         }
         url = self._url_builder.associate_deployment_dataset(deployment_id)
 
         headers = dict(self._common_headers)
@@ -518,21 +452,21 @@
                         response.headers[MLOpsClient.RESPONSE_LOCATION_KEY], timeout
                     )
                 # API responds with HTTP 202, but no longer provides a location header
                 return True
             # TODO: verify that the NOT_FOUND applies to the deployment_id only,
             #       so as not to confuse if deployment_id is valid but model_package_id is not
             if response.status_code == HTTPStatus.NOT_FOUND:
-                raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
             raise DRMLOpsConnectedException(
-                "Call {} with payload {} failed; text: [{}]".format(url, payload, response.text)
+                f"Call {url} with payload {payload} failed; text: [{response.text}]"
             )
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def get_deployment(self, deployment_id):
         """
         Get deployment
 
         :param deployment_id: deployment ID
@@ -543,19 +477,19 @@
         """
         try:
             url = self._url_builder.deployment(deployment_id)
             response = self._get_url_request_response(url)
             if response.ok:
                 return response.json()
             if response.status_code == HTTPStatus.NOT_FOUND:
-                raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
-            raise DRMLOpsConnectedException("Call {} failed; text: [{}]".format(url, response.text))
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def list_deployments(self, params=None):
         url = self._url_builder.list_deployments()
         return self._make_list_call(url, params)
 
     def get_model_id(self, deployment_id):
@@ -602,19 +536,19 @@
         """
         try:
             url = self._url_builder.get_dataset(dataset_id)
             response = self._get_url_request_response(url)
             if response.ok:
                 return response.json()
             if response.status_code == HTTPStatus.NOT_FOUND:
-                raise DRNotFoundException("Dataset ID {} not found.".format(dataset_id))
-            raise DRMLOpsConnectedException("Call {} failed; text: [{}]".format(url, response.text))
+                raise DRNotFoundException(f"Dataset ID {dataset_id} not found.")
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def list_datasets(self, params=None):
         url = self._url_builder.list_datasets()
         return self._make_list_call(url, params)
 
     def soft_delete_dataset(self, dataset_id):
@@ -635,23 +569,23 @@
             # status code is:
             # NO_CONTENT when dataset was deleted
             # GONE when dataset was previously deleted
             # NOT_FOUND when dataset with provided DIId has never existed
             if response.status_code == HTTPStatus.NO_CONTENT:
                 return
             if response.status_code in [HTTPStatus.GONE, HTTPStatus.NOT_FOUND]:
-                raise DRNotFoundException("Dataset ID {} not found.".format(dataset_id))
+                raise DRNotFoundException(f"Dataset ID {dataset_id} not found.")
             raise DRMLOpsConnectedException(
                 "Call {} failed; unexpected status code: {}; text:[{}]".format(
                     url, response.status_code, response.text
                 )
             )
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def set_scoring_dataset(self, deployment_id, dataset_filepath):
         # TODO: This method is never called. It looks like:
         #           MLOpsCli.upload_dataset calls MLOpsClient.upload_dataset
         #           MLOpsCli.upload_scoring_dataset calls MLOpsClient.associate_deployment_dataset
         #       Should this method exist as a standalone?
@@ -686,30 +620,30 @@
 
         if len(actuals) == 0:
             raise DRMLOpsConnectedException("Empty actuals list to post")
 
         for actual in actuals:
             if Constants.ACTUALS_VALUE_KEY not in actual:
                 raise DRMLOpsConnectedException(
-                    "'{}' missing in '{}'".format(Constants.ACTUALS_VALUE_KEY, str(actual))
+                    f"'{Constants.ACTUALS_VALUE_KEY}' missing in '{str(actual)}'"
                 )
             if (
                 not isinstance(actual[Constants.ACTUALS_VALUE_KEY], float)
                 and not isinstance(actual[Constants.ACTUALS_VALUE_KEY], str)
                 and not isinstance(actual[Constants.ACTUALS_VALUE_KEY], int)
             ):
                 raise DRUnsupportedType(
                     "'{}' must be either string, int or float, '{}'".format(
                         Constants.ACTUALS_VALUE_KEY, str(actual)
                     )
                 )
 
             if Constants.ACTUALS_ASSOCIATION_ID_KEY not in actual:
                 raise DRMLOpsConnectedException(
-                    "'{}' missing in '{}'".format(Constants.ACTUALS_ASSOCIATION_ID_KEY, str(actual))
+                    f"'{Constants.ACTUALS_ASSOCIATION_ID_KEY}' missing in '{str(actual)}'"
                 )
 
             if Constants.ACTUALS_WAS_ACTED_ON_KEY in actual and not isinstance(
                 actual[Constants.ACTUALS_WAS_ACTED_ON_KEY], bool
             ):
                 raise DRUnsupportedType(
                     "'{}' should be bool, '{}'".format(
@@ -721,25 +655,25 @@
         headers = dict(self._common_headers)
         headers.update({"Content-Type": "application/json"})
         data = {"data": actuals}
         response = requests.post(
             url, headers=headers, data=json_dumps_bytes(data), verify=self._verify
         )
         if response.status_code != HTTPStatus.ACCEPTED:
-            raise DRMLOpsConnectedException("Failed to post actuals: {}".format(response.text))
+            raise DRMLOpsConnectedException(f"Failed to post actuals: {response.text}")
         if wait_for_result:
             self._wait_for_async_completion(
                 response.headers[MLOpsClient.RESPONSE_LOCATION_KEY], timeout
             )
         return response
 
     @staticmethod
     def _validate_col_exists(df, col_name):
         if col_name not in df.columns:
-            raise Exception("Data does not include {} column".format(col_name))
+            raise Exception(f"Data does not include {col_name} column")
 
     @staticmethod
     def _get_correct_actual_value(deployment_type, value):
         if deployment_type == "Regression":
             return float(value)
         return str(value)
 
@@ -941,29 +875,29 @@
                 raise DRMLOpsConnectedException(
                     "Call {} with payload {} failed; text: [{}]".format(
                         url, model_info, response.text
                     )
                 )
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def get_features_from_model_package(self, model_package_id, params=None):
         try:
             url = self._url_builder.features_model_package(model_package_id)
             response = self._get_url_request_response(url, params=params)
             if response.ok:
                 return response.json()["data"]
             if response.status_code == HTTPStatus.NOT_FOUND:
-                raise DRNotFoundException("Model package ID {} not found.".format(model_package_id))
-            raise DRMLOpsConnectedException("Call {} failed; text: [{}]".format(url, response.text))
+                raise DRNotFoundException(f"Model package ID {model_package_id} not found.")
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def get_model_package(self, model_package_id):
         """
         Get information about a model package from DataRobot MLOps
 
         :param model_package_id: ID of the model package
@@ -975,19 +909,19 @@
 
         try:
             url = self._url_builder.get_model_package(model_package_id)
             response = self._get_url_request_response(url)
             if response.ok:
                 return response.json()
             if response.status_code == HTTPStatus.NOT_FOUND:
-                raise DRNotFoundException("Model package ID {} not found.".format(model_package_id))
-            raise DRMLOpsConnectedException("Call {} failed; text: [{}]".format(url, response.text))
+                raise DRNotFoundException(f"Model package ID {model_package_id} not found.")
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def list_model_packages(self, params=None):
         url = self._url_builder.list_model_packages()
         return self._make_list_call(url, params)
 
     def archive_model_package(self, model_package_id):
@@ -1009,23 +943,23 @@
             # NO_CONTENT when model package was deleted
             # GONE when model package was previously deleted
             # NOT_FOUND when model package with provided id has never existed
             if response.status_code == HTTPStatus.NO_CONTENT:
                 return
             # treating GONE and NOT_FOUND the same (consistent with deleting other resources)
             if response.status_code in [HTTPStatus.GONE, HTTPStatus.NOT_FOUND]:
-                raise DRNotFoundException("Model package ID {} not found.".format(model_package_id))
+                raise DRNotFoundException(f"Model package ID {model_package_id} not found.")
             raise DRMLOpsConnectedException(
                 "Call {} failed; unexpected status code: {}; text:[{}]".format(
                     url, response.status_code, response.text
                 )
             )
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def deploy_model_package(
         self,
         model_package_id,
         label,
         description="",
@@ -1073,23 +1007,23 @@
                 deployment_id = response.json()[MLOpsClient.RESPONSE_DEPLOYMENT_ID_KEY]
                 if wait_for_result:
                     self._wait_for_async_completion(
                         response.headers[MLOpsClient.RESPONSE_LOCATION_KEY], timeout
                     )
                 return deployment_id
             if response.status_code == HTTPStatus.NOT_FOUND:
-                raise DRNotFoundException("Model package ID {} not found.".format(model_package_id))
+                raise DRNotFoundException(f"Model package ID {model_package_id} not found.")
             raise DRMLOpsConnectedException(
                 "Call {} with payload {} failed; text: [{}]".format(
                     url, deployment_info, response.text
                 )
             )
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def replace_model_package(self, deployment_id, model_package_id, reason, timeout=180):
         """
         Replace the model on the deployment
 
         :param deployment_id: ID of the deployment
@@ -1116,23 +1050,23 @@
             )
             if response.ok:
                 self._wait_for_async_completion(
                     response.headers[MLOpsClient.RESPONSE_LOCATION_KEY], timeout
                 )
                 return
             if response.status_code == HTTPStatus.NOT_FOUND:
-                raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
             raise DRMLOpsConnectedException(
                 "Call {} with deployment ID {} and model package ID {} failed; text:[{}]".format(
                     url, deployment_id, model_package_id, response.text
                 )
             )
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def update_deployment_settings(
         self,
         deployment_id,
         target_drift,
         feature_drift,
@@ -1197,23 +1131,23 @@
             )
             if response.ok:
                 self._wait_for_async_completion(
                     response.headers[MLOpsClient.RESPONSE_LOCATION_KEY], timeout
                 )
                 return
             if response.status_code == HTTPStatus.NOT_FOUND:
-                raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
             raise DRMLOpsConnectedException(
                 "Call {} with deployment ID {} and deployment settings {} failed; text:[{}]".format(
                     url, deployment_id, settings_info, response.text
                 )
             )
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def get_deployment_settings(self, deployment_id):
         """
         Get information about a deployment from DataRobot MLOps.
 
         :param deployment_id: ID of the deployment
@@ -1225,19 +1159,19 @@
 
         try:
             url = self._url_builder.deployment_settings(deployment_id)
             response = self._get_url_request_response(url)
             if response.ok:
                 return response.json()
             if response.status_code == HTTPStatus.NOT_FOUND:
-                raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
-            raise DRMLOpsConnectedException("Call {} failed; text: [{}]".format(url, response.text))
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def create_prediction_environment(self, pe_info):
         """
         Create an external prediction environment in DataRobot MLOps from JSON configuration.
 
         :param pe_info: a JSON object of prediction environment parameters
@@ -1264,33 +1198,33 @@
             for key in ["name", "platform", "supportedModelFormats"]:
                 try:
                     _ = pe_info[key]
                 except KeyError:
                     missing_keys.append(key)
             if len(missing_keys) > 0:
                 raise DRMLOpsConnectedException(
-                    "create_prediction_environment(): payload is missing {}".format(missing_keys)
+                    f"create_prediction_environment(): payload is missing {missing_keys}"
                 )
 
             url = self._url_builder.create_prediction_environment()
 
             headers = dict(self._common_headers)
             headers.update({"Content-Type": "application/json"})
             response = requests.post(
                 url, data=json_dumps_bytes(pe_info), headers=headers, verify=self._verify
             )
             if response.ok:
                 return response.json()[MLOpsClient.RESPONSE_PREDICTION_ENVIRONMENT_ID_KEY]
             else:
                 raise DRMLOpsConnectedException(
-                    "Call {} with payload {} failed; text: [{}]".format(url, pe_info, response.text)
+                    f"Call {url} with payload {pe_info} failed; text: [{response.text}]"
                 )
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def get_prediction_environment(self, prediction_environment_id):
         """
         Get information about a prediction environment from DataRobot MLOps.
 
         :param prediction_environment_id: ID of the prediction environment
@@ -1303,34 +1237,32 @@
         try:
             url = self._url_builder.get_prediction_environment(prediction_environment_id)
             response = self._get_url_request_response(url)
             if response.ok:
                 return response.json()
             if response.status_code == HTTPStatus.NOT_FOUND:
                 raise DRNotFoundException(
-                    "Prediction environment ID {} not found.".format(prediction_environment_id)
+                    f"Prediction environment ID {prediction_environment_id} not found."
                 )
-            raise DRMLOpsConnectedException("Call {} failed; text: [{}]".format(url, response.text))
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def _make_list_call(self, url, params=None):
         try:
             response = self._get_url_request_response(url, params=params)
             if response.ok:
                 return response.json()["data"]
             else:
-                raise DRMLOpsConnectedException(
-                    "Call {} failed; text: [{}]".format(url, response.text)
-                )
+                raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def list_prediction_environments(self, params=None):
         url = self._url_builder.list_prediction_environments()
         return self._make_list_call(url, params)
 
     def delete_prediction_environment(self, prediction_environment_id):
@@ -1354,28 +1286,28 @@
             # GONE if it was previously deleted
             # NOT_FOUND if PE was already deleted or user has no permission to delete
             # 422 if a deployment is currently associated with the PE
             if response.status_code == HTTPStatus.NO_CONTENT:
                 return
             if response.status_code in [HTTPStatus.GONE, HTTPStatus.NOT_FOUND]:
                 raise DRNotFoundException(
-                    "Prediction environment ID {} not found.".format(prediction_environment_id)
+                    f"Prediction environment ID {prediction_environment_id} not found."
                 )
             if response.status_code == HTTPStatus.IN_USE:
                 raise DRMLOpsConnectedException(
-                    "Prediction environment ID {} in use.".format(prediction_environment_id)
+                    f"Prediction environment ID {prediction_environment_id} in use."
                 )
             raise DRMLOpsConnectedException(
                 "Call {} failed; unexpected status code: {}; text:[{}]".format(
                     url, response.status_code, response.text
                 )
             )
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def payload_report_deployment_stats(
         self, model_id, timestamp, num_predictions, execution_time_ms=None, batch_name=None
     ):
         deployment_stats = DeploymentStats(num_predictions, execution_time_ms)
         deployment_stats_container = DeploymentStatsContainer(
@@ -1406,28 +1338,26 @@
             if dry_run:
                 return {"message": "ok"}
             else:
                 response = await self._session.post(
                     url, headers=headers, data=payload, verify_ssl=self._verify
                 )
                 if response.status == HTTPStatus.NOT_FOUND:
-                    raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
+                    raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
                 if response.status != HTTPStatus.ACCEPTED:
                     message = await response.text()
-                    raise DRMLOpsConnectedException(
-                        "Failed to post deployment stats: {}".format(message)
-                    )
+                    raise DRMLOpsConnectedException(f"Failed to post deployment stats: {message}")
                 if response.ok:
                     json_response = await response.json()
                     return json_response
                 message = await response.text()
-                raise DRMLOpsConnectedException("Call {} failed; text: [{}]".format(url, message))
+                raise DRMLOpsConnectedException(f"Call {url} failed; text: [{message}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def payload_report_prediction_data(
         self,
         model_id,
         data,
         association_ids=None,
@@ -1485,17 +1415,15 @@
                 feature_data = data
 
         assoc_id_list = None
         if association_ids is not None:
             assoc_id_list = association_ids
         elif assoc_id:
             if assoc_id not in feature_data.columns:
-                raise Exception(
-                    "Error: assoc_id column '{}' is not present in DataFrame".format(assoc_id)
-                )
+                raise Exception(f"Error: assoc_id column '{assoc_id}' is not present in DataFrame")
             assoc_ids = feature_data[assoc_id].tolist()
             assoc_id_list = list(map(str, assoc_ids))
 
         if assoc_id is not None and assoc_id in feature_data.columns:
             feature_data = feature_data.drop(columns=assoc_id)
 
         nr_lines = len(data)
@@ -1676,38 +1604,34 @@
                 else:
                     response = await self._session.post(
                         url, headers=headers, data=payload, verify_ssl=self._verify
                     )
                     # TODO: verify that the NOT_FOUND applies to the deployment_id only, so as
                     #       not to confuse if deployment_id is valid but model_package_id is not
                     if response.status == HTTPStatus.NOT_FOUND:
-                        raise DRNotFoundException(
-                            "Deployment ID {} not found.".format(deployment_id)
-                        )
+                        raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
                     if response.status != HTTPStatus.ACCEPTED:
                         message = await response.text()
                         raise DRMLOpsConnectedException(
-                            "Failed to post prediction data: {}".format(message)
+                            f"Failed to post prediction data: {message}"
                         )
                     if response.ok:
                         json_response = await response.json()
                         last_response = json_response
                         payload_size = len(payload)
                         aggregate_payload_size += payload_size
                         start = end
                     else:
                         message = await response.text()
-                        raise DRMLOpsConnectedException(
-                            "Call {} failed; text:[{}]".format(url, message)
-                        )
+                        raise DRMLOpsConnectedException(f"Call {url} failed; text:[{message}]")
                 continue
 
             except requests.exceptions.ConnectionError as e:
                 raise DRMLOpsConnectedException(
-                    "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                    f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
                 )
 
         return last_response, aggregate_payload_size
 
     def payload_report_aggregated_prediction_data(
         self,
         model_id,
@@ -1807,31 +1731,27 @@
                 return {"message": "ok"}
             else:
                 response = await self._session.post(
                     url, headers=headers, data=payload, verify_ssl=self._verify
                 )
 
                 if response.status == HTTPStatus.NOT_FOUND:
-                    raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
+                    raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
                 if response.status != HTTPStatus.ACCEPTED:
                     message = await response.text()
-                    raise DRMLOpsConnectedException(
-                        "Failed to post prediction data: {}".format(message)
-                    )
+                    raise DRMLOpsConnectedException(f"Failed to post prediction data: {message}")
                 if response.ok:
                     json_response = await response.json()
                     return json_response
                 else:
                     message = await response.text()
-                    raise DRMLOpsConnectedException(
-                        "Call {} failed; text:[{}]".format(url, message)
-                    )
+                    raise DRMLOpsConnectedException(f"Call {url} failed; text:[{message}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def report_actuals_data(self, deployment_id, actuals, dry_run=False):
         """
         Report actuals data for a given deployment.
 
         :param deployment_id: deployment ID to use for reporting
@@ -1849,15 +1769,15 @@
         try:
             if dry_run:
                 return {"message": "ok"}
             else:
                 self.submit_actuals(deployment_id, actuals)
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def _is_model_package_download_from_registry_supported(self):
         if self._api_major_version > 2:
             return True
 
         if self._api_major_version == 2 and self._api_minor_version >= 25:
@@ -1915,34 +1835,32 @@
         if not self._is_model_package_download_from_registry_supported():
             raise DRMLOpsConnectedException(
                 """Downloading model package from model registry is
                 supported for API version 2.25 and later"""
             )
 
         if not os.path.exists(output_dir):
-            raise DRMLOpsConnectedException(
-                "Provided output_dir '{}' does not exist.".format(output_dir)
-            )
+            raise DRMLOpsConnectedException(f"Provided output_dir '{output_dir}' does not exist.")
 
         if not os.path.isdir(output_dir):
             raise DRMLOpsConnectedException(
-                "Provided output_dir '{}' is not a directory.".format(output_dir)
+                f"Provided output_dir '{output_dir}' is not a directory."
             )
 
         headers = dict(self._common_headers)
         params = {"portablePredictionsServerInstaller": "true"} if download_pps_installer else None
         if download_scoring_code and scoring_code_binary:
             # Download binary scoring code in single request
             scoring_code_url = self._url_builder.scoring_code_download_from_registry(
                 model_package_id
             )
             response = requests.get(scoring_code_url, headers=headers, verify=self._verify)
             if response.status_code != HTTPStatus.OK:
                 raise DRMLOpsConnectedException(
-                    "Failed to download binary scoring code: {}".format(response.text)
+                    f"Failed to download binary scoring code: {response.text}"
                 )
         else:
             # Wait for completion needed
             if download_scoring_code:
                 headers.update({"Content-Type": "application/json"})
                 data = json_dumps_bytes(
                     {"includePredictionExplanations": is_prediction_explanations_supported}
@@ -1957,32 +1875,32 @@
                 model_build_url = self._url_builder.model_package_build_from_registry(
                     model_package_id
                 )
                 response = requests.post(
                     model_build_url, headers=headers, params=params, verify=self._verify
                 )
             if response.status_code == HTTPStatus.NOT_FOUND:
-                raise DRNotFoundException("Model package ID {} not found.".format(model_package_id))
+                raise DRNotFoundException(f"Model package ID {model_package_id} not found.")
             if response.status_code != HTTPStatus.ACCEPTED:
                 raise DRMLOpsConnectedException(
-                    "Failed to download model package: {}".format(response.text)
+                    f"Failed to download model package: {response.text}"
                 )
 
             # wait for completion
             model_retrieve_url = self._wait_for_async_completion(
                 response.headers[MLOpsClient.RESPONSE_LOCATION_KEY], timeout
             )
 
             # Download the model package
             response = requests.get(
                 model_retrieve_url, headers=headers, params=params, stream=True, verify=self._verify
             )
             if response.status_code != HTTPStatus.OK:
                 raise DRMLOpsConnectedException(
-                    "Failed to download model package: {}".format(response.text)
+                    f"Failed to download model package: {response.text}"
                 )
 
         return self._download_model(output_dir, response)
 
     def download_dr_current_model_package(
         self,
         deployment_id,
@@ -1999,65 +1917,63 @@
         :param download_scoring_code: Download the scoring code "jar" or "mlpkg" file, default is
             mlpkg file
         :param scoring_code_binary: Download scoring code as binary if required
         :param timeout: time in seconds to wait for result (default is 120 seconds)
         :return: The path of download model package
         """
         if not os.path.exists(output_dir):
-            raise DRMLOpsConnectedException(
-                "Provided output_dir '{}' does not exist.".format(output_dir)
-            )
+            raise DRMLOpsConnectedException(f"Provided output_dir '{output_dir}' does not exist.")
 
         if not os.path.isdir(output_dir):
             raise DRMLOpsConnectedException(
-                "Provided output_dir '{}' is not a directory.".format(output_dir)
+                f"Provided output_dir '{output_dir}' is not a directory."
             )
 
         headers = dict(self._common_headers)
         if download_scoring_code and scoring_code_binary:
             # Download binary scoring code in single request
             scoring_code_url = self._url_builder.scoring_code_download(deployment_id)
             response = requests.get(scoring_code_url, headers=headers, verify=self._verify)
             if response.status_code == HTTPStatus.NOT_FOUND:
-                raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
             if response.status_code != HTTPStatus.OK:
                 raise DRMLOpsConnectedException(
-                    "Failed to download binary scoring code: {}".format(response.text)
+                    f"Failed to download binary scoring code: {response.text}"
                 )
         else:
             # Wait for completion needed
             if download_scoring_code:
                 headers.update({"Content-Type": "application/json"})
                 data = json_dumps_bytes({"includeAgent": False})
                 model_build_url = self._url_builder.scoring_code_build(deployment_id)
                 response = requests.post(
                     model_build_url, headers=headers, data=data, verify=self._verify
                 )
             else:
                 model_build_url = self._url_builder.model_package_build(deployment_id)
                 response = requests.post(model_build_url, headers=headers, verify=self._verify)
             if response.status_code == HTTPStatus.NOT_FOUND:
-                raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
             if response.status_code != HTTPStatus.ACCEPTED:
                 raise DRMLOpsConnectedException(
-                    "Failed to download model package: {}".format(response.text)
+                    f"Failed to download model package: {response.text}"
                 )
 
             # wait for completion
             model_retrieve_url = self._wait_for_async_completion(
                 response.headers[MLOpsClient.RESPONSE_LOCATION_KEY], timeout
             )
 
             # Download the model package
             response = requests.get(
                 model_retrieve_url, headers=headers, stream=True, verify=self._verify
             )
             if response.status_code != HTTPStatus.OK:
                 raise DRMLOpsConnectedException(
-                    "Failed to download model package: {}".format(response.text)
+                    f"Failed to download model package: {response.text}"
                 )
 
         return self._download_model(output_dir, response)
 
     def get_service_stats(self, deployment_id, model_id=None):
         """
         Get information about a deployment's service stats from DataRobot MLOps.
@@ -2087,19 +2003,19 @@
                     and model_id in response.text
                 ):
                     raise DRNotFoundException(
                         "Model ID {} not found for deployment ID {}.".format(
                             model_id, deployment_id
                         )
                     )
-                raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
-            raise DRMLOpsConnectedException("Call {} failed; text: [{}]".format(url, response.text))
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def get_prediction_stats(self, deployment_id, model_id=None):
         """
         Get information about a deployment's prediction stats from DataRobot MLOps.
 
         :param deployment_id: ID of the deployment
@@ -2132,19 +2048,19 @@
                     and model_id in response.text
                 ):
                     raise DRNotFoundException(
                         "Model ID {} not found for deployment ID {}.".format(
                             model_id, deployment_id
                         )
                     )
-                raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
-            raise DRMLOpsConnectedException("Call {} failed; text: [{}]".format(url, response.text))
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def get_target_drift(self, deployment_id, model_id=None):
         """
         Get deployment target drift information from DataRobot MLOps.
 
         :param deployment_id: ID of the deployment
@@ -2172,19 +2088,19 @@
                     and model_id in response.text
                 ):
                     raise DRNotFoundException(
                         "Model ID {} not found for deployment ID {}.".format(
                             model_id, deployment_id
                         )
                     )
-                raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
-            raise DRMLOpsConnectedException("Call {} failed; text: [{}]".format(url, response.text))
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def get_predictions_and_actuals_stats(self, deployment_id, model_id=None):
         """
         Get information about a deployment's predictions and actuals stats from DataRobot MLOps.
 
         :param deployment_id: ID of the deployment
@@ -2213,19 +2129,19 @@
                     and model_id in response.text
                 ):
                     raise DRNotFoundException(
                         "Model ID {} not found for deployment ID {}.".format(
                             model_id, deployment_id
                         )
                     )
-                raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
-            raise DRMLOpsConnectedException("Call {} failed; text: [{}]".format(url, response.text))
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def get_batch_service_statistics(self, deployment_id, batch_id):
         url = self._url_builder.get_batch_service_statistics(deployment_id, batch_id)
         try:
             response = self._get_url_request_response(url)
             if response.ok:
@@ -2233,19 +2149,19 @@
             if response.status_code == HTTPStatus.NOT_FOUND:
                 if "Monitoring batch not found" in response.text:
                     raise DRNotFoundException(
                         "Batch ID {} not found for deployment ID {}.".format(
                             batch_id, deployment_id
                         )
                     )
-                raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
-            raise DRMLOpsConnectedException("Call {} failed; text: [{}]".format(url, response.text))
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def get_batch_data_drift(self, deployment_id, batch_id):
         url = self._url_builder.get_batch_data_drift(deployment_id, batch_id)
         try:
             response = self._get_url_request_response(url)
             if response.ok:
@@ -2253,28 +2169,28 @@
             if response.status_code == HTTPStatus.NOT_FOUND:
                 if "Monitoring batch not found" in response.text:
                     raise DRNotFoundException(
                         "Batch ID {} not found for deployment ID {}.".format(
                             batch_id, deployment_id
                         )
                     )
-                raise DRNotFoundException("Deployment ID {} not found.".format(deployment_id))
-            raise DRMLOpsConnectedException("Call {} failed; text: [{}]".format(url, response.text))
+                raise DRNotFoundException(f"Deployment ID {deployment_id} not found.")
+            raise DRMLOpsConnectedException(f"Call {url} failed; text: [{response.text}]")
         except requests.exceptions.ConnectionError as e:
             raise DRMLOpsConnectedException(
-                "Connection to DataRobot MLOps [{}] refused: {}".format(self._service_url, e)
+                f"Connection to DataRobot MLOps [{self._service_url}] refused: {e}"
             )
 
     def list_batches(self, deployment_id, params=None):
         url = self._url_builder.list_batches(deployment_id)
         return self._make_list_call(url, params)
 
     async def shutdown(self):
         if self.__session is not None:
             await self.__session.close()
 
     def __del__(self):
         if self.__session is not None and not self.__session.closed:
             warnings.warn(
-                "Client was not properly shutdown() {}".format(repr(self)),
+                f"Client was not properly shutdown() {repr(self)}",
                 ResourceWarning,
             )
```

## datarobot/mlops/connected/exception.py

```diff
@@ -1,10 +1,10 @@
 #  ---------------------------------------------------------------------------------
 #  Copyright (c) 2022 DataRobot, Inc. and its affiliates. All rights reserved.
-#  Last updated 2022.
+#  Last updated 2023.
 #
 #  DataRobot, Inc. Confidential.
 #  This is unpublished proprietary source code of DataRobot, Inc. and its affiliates.
 #  The copyright notice above does not evidence any actual or intended publication of
 #  such source code.
 #
 #  This file and its contents are subject to DataRobot Tool and Utility Agreement.
@@ -13,8 +13,8 @@
 #  ---------------------------------------------------------------------------------
 
 from datarobot.mlops.common.exception import DRCommonException
 
 
 class DRMLOpsConnectedException(DRCommonException):
     def __init__(self, *args, **kwargs):
-        super(DRMLOpsConnectedException, self).__init__(args, kwargs)
+        super().__init__(args, kwargs)
```

## datarobot/mlops/connected/mlops_cli.py

```diff
@@ -19,14 +19,15 @@
 import sys
 import time
 from argparse import RawTextHelpFormatter
 from contextlib import closing
 from enum import Enum
 
 import pandas as pd
+
 from datarobot.mlops.common import config
 from datarobot.mlops.common.enums import DataType
 from datarobot.mlops.common.enums import MLOpsSpoolAction
 from datarobot.mlops.common.enums import SpoolerType
 from datarobot.mlops.common.exception import DRCommonException
 from datarobot.mlops.common.exception import DRNotFoundException
 from datarobot.mlops.constants import Constants
@@ -202,15 +203,15 @@
     SERVICE_STATS = Subjects.SERVICE_STATS
     BATCH = Subjects.BATCH
 
     @staticmethod
     def list_all():
         all_subjects = ""
         for m in RunMode:
-            all_subjects = "{} {}".format(all_subjects, m.value)
+            all_subjects = f"{all_subjects} {m.value}"
         return all_subjects
 
 
 REPLACEMENT_REASONS = [
     "ACCURACY",
     "DATA_DRIFT",
     "ERRORS",
@@ -233,25 +234,25 @@
 
     parser = None
 
     @staticmethod
     def _is_valid_file(arg):
         abs_path = os.path.abspath(arg)
         if not os.path.exists(arg):
-            raise argparse.ArgumentTypeError("The file {} does not exist.".format(arg))
+            raise argparse.ArgumentTypeError(f"The file {arg} does not exist.")
         else:
             return os.path.realpath(abs_path)
 
     @staticmethod
     def _register_arg_version(*parsers):
         for parser in parsers:
             parser.add_argument(
                 "--version",
                 action="version",
-                version="%(prog)s {version}".format(version=Constants.MLOPS_VERSION),
+                version=f"%(prog)s {Constants.MLOPS_VERSION}",
             )
 
     @staticmethod
     def _register_arg_verbose(*parsers):
         for parser in parsers:
             parser.add_argument(
                 ArgumentsOptions.VERBOSE,
@@ -419,25 +420,25 @@
     @staticmethod
     def _register_arg_mlops_service(*parsers):
         for parser in parsers:
             parser.add_argument(
                 ArgumentsOptions.MLOPS_SERVICE,
                 dest="mlops_service_url",
                 default=os.environ.get(EV.MLOPS_SERVICE_URL, None),
-                help="MLOps service URL to use (env: {})".format(EV.MLOPS_SERVICE_URL),
+                help=f"MLOps service URL to use (env: {EV.MLOPS_SERVICE_URL})",
             )
 
     @staticmethod
     def _register_arg_mlops_api_token(*parsers):
         for parser in parsers:
             parser.add_argument(
                 ArgumentsOptions.MLOPS_API_TOKEN,
                 dest="mlops_api_token",
                 default=os.environ.get(EV.MLOPS_API_TOKEN, None),
-                help="MLOps API Token to use for connecting (env: {})".format(EV.MLOPS_API_TOKEN),
+                help=f"MLOps API Token to use for connecting (env: {EV.MLOPS_API_TOKEN})",
             )
 
     @staticmethod
     def _register_arg_no_verify_ssl(*parsers):
         for parser in parsers:
             parser.add_argument(
                 ArgumentsOptions.NO_VERIFY_SSL,
@@ -909,15 +910,15 @@
     def __init__(self, filename, chunk_size, skip_rows=0):
         self.filename = filename
         self.chunk_size = chunk_size
         self.skip_rows = skip_rows
         # Because we want to skip 'n' rows, but still want to keep the header (as it contains the
         # column names), we skip rows from range 1 to that offset)
         self.headers = pd.read_csv(filename, nrows=1).columns.tolist()
-        logger.info("Reading input data after skipping '{}' rows".format(self.skip_rows))
+        logger.info(f"Reading input data after skipping '{self.skip_rows}' rows")
         self.reader = pd.read_csv(
             filename, skiprows=range(1, self.skip_rows), chunksize=self.chunk_size
         )
         self._next_chunk = None
         self._current_row = self.skip_rows
 
     def get_columns(self):
@@ -959,23 +960,23 @@
 
 
 class MLOpsCSVBatchSplitter(MLOpsCSVSplitter):
     # Batch Splitter can chop big, 100K
     BATCH_CHUNK_SIZE = 100 * 1000
 
     def __init__(self, filename, skip_rows=0):
-        super(MLOpsCSVBatchSplitter, self).__init__(filename, self.BATCH_CHUNK_SIZE, skip_rows)
+        super().__init__(filename, self.BATCH_CHUNK_SIZE, skip_rows)
 
 
 class MLOpsCSVJSONSplitter(MLOpsCSVSplitter):
     # JSON Post is 10k at a time
     JSON_CHUNK_SIZE = 10000
 
     def __init__(self, filename, skip_rows=0):
-        super(MLOpsCSVJSONSplitter, self).__init__(filename, self.JSON_CHUNK_SIZE, skip_rows)
+        super().__init__(filename, self.JSON_CHUNK_SIZE, skip_rows)
 
 
 class MLOpsCli:
     def __init__(self, options):
         self.options = options
         # self.logger = CMRunner._config_logger(runtime.options)
         self.run_mode = RunMode(options.subject)
@@ -1012,15 +1013,15 @@
                 self.options.model_id,
                 1,
                 10,
                 batch_name=self.options.batch_name,
             )
             request_end_time = time.time()
             request_elapsed_ms = (request_end_time - request_start_time) * 1000
-            logger.info("request: {} time {:.1f}ms".format(res, request_elapsed_ms))
+            logger.info(f"request: {res} time {request_elapsed_ms:.1f}ms")
 
         end_time = time.time()
         elapsed_time = end_time - start_time
         per_request_ms = (elapsed_time * 1000.0) / request_num
 
         logger.info(
             "report deployment stats: total: {:.3f}sec sec, per request {:.2f}ms".format(
@@ -1079,36 +1080,36 @@
             self.options.model_id, EV.MLOPS_MODEL_ID, ArgumentsOptions.MODEL_ID
         )
         check_required_parameter(self.options.target_col, None, ArgumentsOptions.TARGET_COL)
         check_required_parameter(self.options.class_names, None, ArgumentsOptions.CLASS_NAMES)
 
         self.create_mclient()
         logger.info("Running performance test:")
-        logger.info("MLOps service: {}".format(self.options.mlops_service_url))
-        logger.info("Deployment ID: {}".format(self.options.deployment_id))
-        logger.info("Model ID:      {}".format(self.options.model_id))
-        logger.info("Target:        {}".format(self.options.target_col))
-        logger.info("Classes:       {}".format(self.options.class_names))
-        logger.info("Input:         {}".format(self.options.input))
-        logger.info("Count:         {}".format(self.options.count))
-        logger.info("Rows:          {}".format(self.options.rows))
-        logger.info("Batch Name:    {}".format(self.options.batch_name))
+        logger.info(f"MLOps service: {self.options.mlops_service_url}")
+        logger.info(f"Deployment ID: {self.options.deployment_id}")
+        logger.info(f"Model ID:      {self.options.model_id}")
+        logger.info(f"Target:        {self.options.target_col}")
+        logger.info(f"Classes:       {self.options.class_names}")
+        logger.info(f"Input:         {self.options.input}")
+        logger.info(f"Count:         {self.options.count}")
+        logger.info(f"Rows:          {self.options.rows}")
+        logger.info(f"Batch Name:    {self.options.batch_name}")
 
         self.event_loop.run_until_complete(self._perf_run_async())
         self.delete_mclient()
 
     def _log_report_status(self, input_df, row_offset):
         logger.info("Reporting predictions:")
-        logger.debug("MLOps service: {}".format(self.options.mlops_service_url))
-        logger.debug("Input:         {}".format(self.options.input))
-        logger.info("Input rows:     {}".format(len(input_df)))
-        logger.info("Input cols:     {}".format(len(input_df.columns)))
-        logger.info("Row Offset:     {}".format(row_offset))
-        logger.debug("Dry run:       {}".format(self.options.dry_run))
-        logger.debug("Status File:   {}".format(self.status_tracker.get_status_file()))
+        logger.debug(f"MLOps service: {self.options.mlops_service_url}")
+        logger.debug(f"Input:         {self.options.input}")
+        logger.info(f"Input rows:     {len(input_df)}")
+        logger.info(f"Input cols:     {len(input_df.columns)}")
+        logger.info(f"Row Offset:     {row_offset}")
+        logger.debug(f"Dry run:       {self.options.dry_run}")
+        logger.debug(f"Status File:   {self.status_tracker.get_status_file()}")
 
     async def _report_predictions_connected_lib(self, input_df, row_offset):
         self._log_report_status(input_df, row_offset)
 
         request_start_time = time.time()
         res, payload_size = await self.mclient.report_prediction_data(
             self.options.deployment_id,
@@ -1253,31 +1254,31 @@
                 record.get_deployment_id(),
                 payload[common_fields_keys.MODEL_ID_FIELD_NAME],
                 payload=payload,
                 batch_name=payload.get(common_fields_keys.BATCH_NAME_FIELD_NAME, None),
                 dry_run=self.options.dry_run,
             )
         else:
-            logger.warn("Connected client does not handle data type: '{}'".format(data_type.name))
+            logger.warn(f"Connected client does not handle data type: '{data_type.name}'")
 
         if spooler.enable_dequeue_ack_record:
             spooler.ack_records([record.get_id()])
 
         request_end_time = time.time()
         request_elapsed_ms = (request_end_time - request_start_time) * 1000
         if data_type == DataType.DEPLOYMENT_STATS:
             logger.debug(
                 "Reporting stats predictions: {} execution time: {}".format(
                     payload[deployment_stats_keys.NUM_PREDICTIONS_FIELD_NAME],
                     payload[deployment_stats_keys.EXECUTION_TIME_FIELD_NAME],
                 )
             )
         elif data_type == DataType.PREDICTIONS_DATA:
-            logger.debug("Reporting feature data, row count: {}".format(row_count))
-        logger.debug("Reporting latency: {:.1f}ms".format(request_elapsed_ms))
+            logger.debug(f"Reporting feature data, row count: {row_count}")
+        logger.debug(f"Reporting latency: {request_elapsed_ms:.1f}ms")
 
     def report_predictions_from_spool(self):
         self.create_mclient()
         try:
             spooler_type = config.get_config_default(
                 config.ConfigConstants.SPOOLER_TYPE, SpoolerType.FILESYSTEM.name
             )
@@ -1343,25 +1344,25 @@
         logger.info("Done reporting all data.")
 
     def _check_columns(self, columns):
         if self.options.prediction_cols is not None:
             for prediction_col in self.options.prediction_cols:
                 if prediction_col not in columns:
                     raise DRCommonException(
-                        "Prediction column {} not found in input file.".format(prediction_col)
+                        f"Prediction column {prediction_col} not found in input file."
                     )
             if self.options.class_names is not None:
                 if len(self.options.class_names) != len(self.options.prediction_cols):
                     raise DRCommonException(
                         "The number of class names and prediction columns must match."
                     )
         if self.options.target_col is not None:
             if self.options.target_col not in columns:
                 raise DRCommonException(
-                    "Target column {} not found in input file.".format(self.options.target_col)
+                    f"Target column {self.options.target_col} not found in input file."
                 )
         if self.options.assoc_id_col is not None:
             if self.options.assoc_id_col not in columns:
                 raise DRCommonException(
                     "Association ID column {} not found in input file.".format(
                         self.options.assoc_id_col
                     )
@@ -1373,21 +1374,21 @@
             self.options.deployment_id, EV.MLOPS_DEPLOYMENT_ID, ArgumentsOptions.DEPLOYMENT_ID
         )
         check_required_parameter(
             self.options.model_id, EV.MLOPS_MODEL_ID, ArgumentsOptions.MODEL_ID
         )
 
         logger.debug("Reporting predictions:")
-        logger.debug("MLOps service:         {}".format(self.options.mlops_service_url))
-        logger.debug("Input:                 {}".format(self.options.input))
-        logger.debug("Target column:         {}".format(self.options.target_col))
-        logger.debug("Prediction column(s):  {}".format(self.options.prediction_cols))
-        logger.debug("Classes:               {}".format(self.options.class_names))
-        logger.debug("Assoc Id column:       {}".format(self.options.assoc_id_col))
-        logger.debug("Dry run:               {}".format(self.options.dry_run))
+        logger.debug(f"MLOps service:         {self.options.mlops_service_url}")
+        logger.debug(f"Input:                 {self.options.input}")
+        logger.debug(f"Target column:         {self.options.target_col}")
+        logger.debug(f"Prediction column(s):  {self.options.prediction_cols}")
+        logger.debug(f"Classes:               {self.options.class_names}")
+        logger.debug(f"Assoc Id column:       {self.options.assoc_id_col}")
+        logger.debug(f"Dry run:               {self.options.dry_run}")
 
         if self.options.status_file:
             self.status_tracker = MLOpsUploadTracker(self.options.status_file)
         else:
             self.status_tracker = MLOpsUploadTracker()
         skip_rows, _ = self.status_tracker.get_status()
         try:
@@ -1465,15 +1466,15 @@
         self.create_mclient()
         if self.options.model_id is None:
             self._log_get_action("deployment", self.options.deployment_id, "service stats")
         else:
             self._log_get_action(
                 "deployment",
                 self.options.deployment_id,
-                "service stats for model ID {}".format(self.options.model_id),
+                f"service stats for model ID {self.options.model_id}",
             )
         try:
             stats = self.mclient.get_service_stats(
                 self.options.deployment_id, self.options.model_id
             )
             self._print_resource_received(self.options.deployment_id, stats)
         except DRNotFoundException as e:
@@ -1494,22 +1495,22 @@
         check_required_parameter(self.options.assoc_id_col, None, ArgumentsOptions.ASSOC_ID)
 
         self.create_mclient()
 
         input_df = pd.read_csv(self.options.input)
 
         logger.info("Reporting actuals:")
-        logger.info("MLOps service:         {}".format(self.options.mlops_service_url))
-        logger.info("Deployment ID:         {}".format(self.options.deployment_id))
-        logger.info("Input:                 {}".format(self.options.input))
-        logger.info("Input rows:            {}".format(len(input_df)))
-        logger.info("Actual value column:   {}".format(self.options.actual_value_col))
-        logger.info("Assoc ID column:       {}".format(self.options.assoc_id_col))
-        logger.info("Was-acted-on column:   {}".format(self.options.acted_on_col))
-        logger.info("Timestamp column:      {}".format(self.options.timestamp_col))
+        logger.info(f"MLOps service:         {self.options.mlops_service_url}")
+        logger.info(f"Deployment ID:         {self.options.deployment_id}")
+        logger.info(f"Input:                 {self.options.input}")
+        logger.info(f"Input rows:            {len(input_df)}")
+        logger.info(f"Actual value column:   {self.options.actual_value_col}")
+        logger.info(f"Assoc ID column:       {self.options.assoc_id_col}")
+        logger.info(f"Was-acted-on column:   {self.options.acted_on_col}")
+        logger.info(f"Timestamp column:      {self.options.timestamp_col}")
 
         def progress_callback(total_nr_actuals, nr_actuals_sent, request_time):
             logger.info(
                 "Actuals sent: {} / {} : {:.3f} sec".format(
                     nr_actuals_sent, total_nr_actuals, request_time
                 )
             )
@@ -1524,63 +1525,63 @@
             timestamp_col=self.options.timestamp_col,
             progress_callback=progress_callback,
             wait_for_result=self.options.wait,
             timeout=self.options.timeout,
         )
         request_end_time = time.time()
         request_elapsed_ms = request_end_time - request_start_time
-        logger.debug("request: {} : time {:.2f} sec".format(ret_val, request_elapsed_ms))
+        logger.debug(f"request: {ret_val} : time {request_elapsed_ms:.2f} sec")
         self.delete_mclient()
 
     def _generate_temp_csv_filename(self, iteration):
         prefix = "/tmp/" + os.path.basename(self.options.input).replace(".csv", "")
         return prefix + str(iteration) + ".csv"
 
     async def _upload_scoring_dataset_batch(self, input_df, row_offset, iteration):
         """Upload a scoring dataset and associate it with a deployment."""
         # This is just the filename generated and issued for display in "AI Catalog"; there is no
         # actual file written to disk.  Dataframe is streamed to the MLOps in CSV format.
         csv_file_name = self._generate_temp_csv_filename(iteration)
         logger.info("Set scoring dataset:")
-        logger.debug("MLOps service: {}".format(self.options.mlops_service_url))
-        logger.info("Deployment ID:  {}".format(self.options.deployment_id))
-        logger.info("Model ID:       {}".format(self.options.model_id))
-        logger.info("Target:         {}".format(self.options.target_col))
-        logger.info("Prediction column(s):  {}".format(self.options.prediction_cols))
-        logger.info("Classes:        {}".format(self.options.class_names))
-        logger.debug("Input:         {}".format(self.options.input))
-        logger.info("Input rows:     {}".format(len(input_df)))
-        logger.info("Input cols:     {}".format(len(input_df.columns)))
-        logger.info("Row Offset:     {}".format(row_offset))
-        logger.debug("Dry run:       {}".format(self.options.dry_run))
-        logger.debug("Status File:   {}".format(self.status_tracker.get_status_file()))
-        logger.debug("CSV FileName:  {}".format(csv_file_name))
+        logger.debug(f"MLOps service: {self.options.mlops_service_url}")
+        logger.info(f"Deployment ID:  {self.options.deployment_id}")
+        logger.info(f"Model ID:       {self.options.model_id}")
+        logger.info(f"Target:         {self.options.target_col}")
+        logger.info(f"Prediction column(s):  {self.options.prediction_cols}")
+        logger.info(f"Classes:        {self.options.class_names}")
+        logger.debug(f"Input:         {self.options.input}")
+        logger.info(f"Input rows:     {len(input_df)}")
+        logger.info(f"Input cols:     {len(input_df.columns)}")
+        logger.info(f"Row Offset:     {row_offset}")
+        logger.debug(f"Dry run:       {self.options.dry_run}")
+        logger.debug(f"Status File:   {self.status_tracker.get_status_file()}")
+        logger.debug(f"CSV FileName:  {csv_file_name}")
 
         if len(input_df) < 1:
             logger.debug("All rows already uploaded.")
             return
 
         request_start_time = time.time()
         dataset_id = self.mclient.upload_dataframe(
             input_df, csv_file_name, dry_run=self.options.dry_run
         )
         request_end_time = time.time()
         request_elapsed_ms = (request_end_time - request_start_time) * 1000
-        logger.debug("Upload done: time {:.1f}ms".format(request_elapsed_ms))
+        logger.debug(f"Upload done: time {request_elapsed_ms:.1f}ms")
 
         request_start_time = time.time()
         self.mclient.associate_deployment_dataset(
             self.options.deployment_id,
             dataset_id,
             DatasetSourceType.SCORING,
             dry_run=self.options.dry_run,
         )
         request_end_time = time.time()
         request_elapsed_ms = (request_end_time - request_start_time) * 1000
-        logger.debug("Association done: time {:.1f}ms".format(request_elapsed_ms))
+        logger.debug(f"Association done: time {request_elapsed_ms:.1f}ms")
 
         # Remove the dataset after association is done
         self.mclient.soft_delete_dataset(dataset_id)
 
         request_start_time = time.time()
         res, payload_size = await self.mclient.report_prediction_data(
             self.options.deployment_id,
@@ -1632,22 +1633,22 @@
         finally:
             self.delete_mclient()
 
     def upload_dataset(self):
         check_required_parameter(self.options.input, None, ArgumentsOptions.INPUT)
         self.create_mclient()
         dataset = self.options.input
-        logger.info("Uploading dataset - {}. This may take some time...".format(dataset))
+        logger.info(f"Uploading dataset - {dataset}. This may take some time...")
         try:
             if self.options.timeout:
                 dataset_id = self.mclient.upload_dataset(dataset, timeout=self.options.timeout)
             else:
                 dataset_id = self.mclient.upload_dataset(dataset)
             self._print_resource_generic_action(dataset_id)
-            logger.info("Dataset uploaded. Dataset ID {}.".format(dataset_id))
+            logger.info(f"Dataset uploaded. Dataset ID {dataset_id}.")
         except Exception as e:
             feature_drift_error_message = (
                 "Dataset upload failed. You won't see Feature Drift reports in UI."
             )
             logger.error(feature_drift_error_message)
             self._log_error_and_exit(e, ExitCode.UNSPECIFIED)
         finally:
@@ -1716,23 +1717,23 @@
     def download_model_package(self):
         check_required_parameter(
             self.options.deployment_id, "MLOPS_DEPLOYMENT_ID", ArgumentsOptions.DEPLOYMENT_ID
         )
 
         self.create_mclient()
         logger.debug("Downloading current model package:")
-        logger.debug("MLOps service:          {}".format(self.options.mlops_service_url))
-        logger.debug("Deployment ID:          {}".format(self.options.deployment_id))
-        logger.debug("Output directory:       {}".format(self.options.output_dir))
+        logger.debug(f"MLOps service:          {self.options.mlops_service_url}")
+        logger.debug(f"Deployment ID:          {self.options.deployment_id}")
+        logger.debug(f"Output directory:       {self.options.output_dir}")
 
         mlpkg_path = self.mclient.download_dr_current_model_package(
             self.options.deployment_id, self.options.output_dir
         )
 
-        logger.debug("Model Package path     {}".format(mlpkg_path))
+        logger.debug(f"Model Package path     {mlpkg_path}")
 
         self.delete_mclient()
 
     @staticmethod
     def _convert_feature_format(feature):
         # FeatureType is defined in mlops-stats-aggregator library and are the types
         # currently supported, this mostly correspond to EdaTypeEnum in DR side.
@@ -1838,54 +1839,54 @@
             self._log_error_and_exit(e, ExitCode.UNSPECIFIED.value)
         finally:
             self.delete_mclient()
 
     def _read_json_config(self, config_file):
         config_path = os.path.abspath(config_file)
         try:
-            with open(config_path, "r") as f:
+            with open(config_path) as f:
                 info = json.loads(f.read())
         except FileNotFoundError as e:
             # Effectively, remove the '[Errno 2]' portion of the default FileNotFoundError message
             # so as to not confuse the user, since we exit with a custom error number from ExitCode
-            raise FileNotFoundError("No such file or directory: {}".format(e.filename))
+            raise FileNotFoundError(f"No such file or directory: {e.filename}")
         return info
 
     def create_model_package(self):
         check_required_parameter(self.options.json_config, None, ArgumentsOptions.JSON_CONF)
         self.create_mclient()
         logger.info("Creating model package:")
-        logger.debug("MLOps service:         {}".format(self.options.mlops_service_url))
-        logger.info("Model config:           {}".format(self.options.json_config))
+        logger.debug(f"MLOps service:         {self.options.mlops_service_url}")
+        logger.info(f"Model config:           {self.options.json_config}")
 
         try:
             model_info = self._read_json_config(self.options.json_config)
         except FileNotFoundError as e:
             self._log_error_and_exit(e, ExitCode.FILE_NOT_FOUND.value)
         if self.options.model_id is not None:
             model_info["modelId"] = self.options.model_id
-            logger.debug("Model ID:              {}".format(self.options.model_id))
+            logger.debug(f"Model ID:              {self.options.model_id}")
 
         # if specified, add training_data to model configuration
         if (
             self.options.training_dataset_id is not None
             or self.options.holdout_dataset_id is not None
         ):
             datasets = {}
             if self.options.training_dataset_id is not None:
                 datasets["trainingDataCatalogId"] = self.options.training_dataset_id
-                logger.debug("Training dataset ID:   {}".format(self.options.training_dataset_id))
+                logger.debug(f"Training dataset ID:   {self.options.training_dataset_id}")
             if self.options.holdout_dataset_id is not None:
                 datasets["holdoutDataCatalogId"] = self.options.holdout_dataset_id
-                logger.debug("Holdout dataset ID:    {}".format(self.options.holdout_dataset_id))
+                logger.debug(f"Holdout dataset ID:    {self.options.holdout_dataset_id}")
             model_info["datasets"] = datasets
         try:
             model_pkg_id = self.mclient.create_model_package(model_info)
             self._print_resource_generic_action(model_pkg_id)
-            logger.info("Created model package ID {}.".format(model_pkg_id))
+            logger.info(f"Created model package ID {model_pkg_id}.")
         except DRMLOpsConnectedException as e:
             self._log_error_and_exit(e, ExitCode.DR_CONNECTED.value)
         except Exception as e:
             self._log_error_and_exit(e, ExitCode.UNSPECIFIED.value)
         finally:
             self.delete_mclient()
 
@@ -1893,34 +1894,34 @@
         check_required_parameter(
             self.options.model_package_id,
             EV.MLOPS_MODEL_PACKAGE_ID,
             ArgumentsOptions.MODEL_PACKAGE_ID,
         )
         self.create_mclient()
         logger.info("Deploying model package to prediction environment. This may take some time...")
-        logger.debug("MLOps service:            {}".format(self.options.mlops_service_url))
-        logger.info("Model package ID:          {}".format(self.options.model_package_id))
-        logger.info("Deployment label:          {}".format(self.options.deployment_label))
-        logger.info("Prediction Environment ID: {}".format(self.options.prediction_environment_id))
-        logger.info("Timestamp column name:     {}".format(self.options.timestamp_col))
-        logger.info("Timestamp format:          {}".format(self.options.timestamp_format))
-        logger.info("Enable Batch Monitoring:   {}".format(self.options.enable_batch_monitoring))
+        logger.debug(f"MLOps service:            {self.options.mlops_service_url}")
+        logger.info(f"Model package ID:          {self.options.model_package_id}")
+        logger.info(f"Deployment label:          {self.options.deployment_label}")
+        logger.info(f"Prediction Environment ID: {self.options.prediction_environment_id}")
+        logger.info(f"Timestamp column name:     {self.options.timestamp_col}")
+        logger.info(f"Timestamp format:          {self.options.timestamp_format}")
+        logger.info(f"Enable Batch Monitoring:   {self.options.enable_batch_monitoring}")
         if self.options.segment_attributes:
-            logger.info("Segment attributes:        {}".format(self.options.segment_attributes))
+            logger.info(f"Segment attributes:        {self.options.segment_attributes}")
 
         try:
             deployment_id = self.mclient.deploy_model_package(
                 self.options.model_package_id,
                 self.options.deployment_label,
                 prediction_environment_id=self.options.prediction_environment_id,
             )
             self._print_resource_generic_action(deployment_id)
-            logger.info("Model package deployed. Deployment ID {}.".format(deployment_id))
+            logger.info(f"Model package deployed. Deployment ID {deployment_id}.")
 
-            logger.info("Updating deployment settings for deployment ID {}.".format(deployment_id))
+            logger.info(f"Updating deployment settings for deployment ID {deployment_id}.")
             self.mclient.update_deployment_settings(
                 deployment_id,
                 target_drift=True,
                 feature_drift=True,
                 segment_attributes=self.options.segment_attributes,
                 timeout=600,
                 timestamp_col_name=self.options.timestamp_col,
@@ -1943,25 +1944,23 @@
         check_required_parameter(
             self.options.model_package_id,
             EV.MLOPS_MODEL_PACKAGE_ID,
             ArgumentsOptions.MODEL_PACKAGE_ID,
         )
         self.create_mclient()
         logger.info("Replacing model package in a deployment:")
-        logger.debug("MLOps service:        {}".format(self.options.mlops_service_url))
-        logger.info("Model package ID:      {}".format(self.options.model_package_id))
-        logger.info("Deployment ID:         {}".format(self.options.deployment_id))
-        logger.info("Reason:                {}".format(self.options.reason))
+        logger.debug(f"MLOps service:        {self.options.mlops_service_url}")
+        logger.info(f"Model package ID:      {self.options.model_package_id}")
+        logger.info(f"Deployment ID:         {self.options.deployment_id}")
+        logger.info(f"Reason:                {self.options.reason}")
         try:
             self.mclient.replace_model_package(
                 self.options.deployment_id, self.options.model_package_id, self.options.reason
             )
-            logger.debug(
-                "Model package replaced on deployment {}".format(self.options.deployment_id)
-            )
+            logger.debug(f"Model package replaced on deployment {self.options.deployment_id}")
         except DRNotFoundException as e:
             self._log_error_and_exit(e, ExitCode.DR_NOT_FOUND.value)
         except DRMLOpsConnectedException as e:
             self._log_error_and_exit(e, ExitCode.DR_CONNECTED.value)
         except Exception as e:
             self._log_error_and_exit(e, ExitCode.UNSPECIFIED.value)
         finally:
@@ -2030,15 +2029,15 @@
             info = self._read_json_config(self.options.json_config)
         except FileNotFoundError as e:
             self._log_error_and_exit(e, ExitCode.FILE_NOT_FOUND.value)
         self.create_mclient()
         try:
             pe_id = self.mclient.create_prediction_environment(info)
             self._print_resource_generic_action(pe_id)
-            logger.info("Created prediction environment ID {}.".format(pe_id))
+            logger.info(f"Created prediction environment ID {pe_id}.")
         except DRMLOpsConnectedException as e:
             self._log_error_and_exit(e, ExitCode.DR_CONNECTED.value)
         except Exception as e:
             self._log_error_and_exit(e, ExitCode.UNSPECIFIED.value)
         finally:
             self.delete_mclient()
 
@@ -2095,15 +2094,15 @@
         finally:
             self.delete_mclient()
 
     @staticmethod
     def _print_supported_actions(subject):
         actions = SUPPORTED_ACTIONS[subject]
         if len(actions) == 1:
-            print("Supported {} action is: {}".format(subject, actions[0]))
+            print(f"Supported {subject} action is: {actions[0]}")
         else:
             print("Supported {} actions are: {}".format(subject, ", ".join(actions)))
         raise SystemExit(ExitCode.INVALID_CLI_INPUT.value)
 
     def handle_predictions(self):
         if self.options.action == Actions.GET:
             self.get_prediction_stats()
@@ -2207,15 +2206,15 @@
                 )
             elif self.options.batch_data_drift:
                 stats = self.mclient.get_batch_data_drift(
                     self.options.deployment_id, self.options.batch_id
                 )
             else:
                 raise Exception(
-                    "Please specify either \"--service-stats\" or \"--data-drift\" "
+                    'Please specify either "--service-stats" or "--data-drift" '
                     "to query for the given batch"
                 )
             self._print_resource_received(self.options.deployment_id, stats)
         except DRNotFoundException as e:
             self._log_error_and_exit(e, ExitCode.DR_NOT_FOUND.value)
         except DRMLOpsConnectedException as e:
             self._log_error_and_exit(e, ExitCode.DR_CONNECTED.value)
@@ -2259,44 +2258,44 @@
             if self.options.search:
                 params["search"] = self.options.search
             if self.options.limit:
                 params["limit"] = self.options.limit
         return params
 
     def _log_list_action(self, resource):
-        logger.debug("Listing {} metadata...".format(resource))
-        logger.debug("MLOps service:         {}".format(self.options.mlops_service_url))
+        logger.debug(f"Listing {resource} metadata...")
+        logger.debug(f"MLOps service:         {self.options.mlops_service_url}")
 
     def _print_resources_listed(self, info, key="id"):
         """Print information for resources listed, according to output format."""
         if self.options.terse:
             for id in [result.get(key) for result in info]:
                 print(id)
         elif self.options.json:
             print(json.dumps(info, indent=1))
         else:
             raise ValueError("Something went wrong. Output format not recognized.")
 
     def _log_get_action(self, resource, id, retrieved="metadata"):
-        logger.debug("Retrieving {} for {} ID {}".format(retrieved, resource, id))
-        logger.debug("MLOps service:          {}".format(self.options.mlops_service_url))
+        logger.debug(f"Retrieving {retrieved} for {resource} ID {id}")
+        logger.debug(f"MLOps service:          {self.options.mlops_service_url}")
 
     def _print_resource_received(self, id, info):
         # TODO: this could technically be the same method as _print_list_resources;
         #       maybe just get 'id' from info object, instead of passing 'id' separately
         if self.options.terse:
             print(id)
         elif self.options.json:
             print(json.dumps(info, indent=1))
         else:
             raise ValueError("Something went wrong. Output format not recognized.")
 
     def _log_delete_action(self, resource, id):
-        logger.info("Deleting {} ID {}...".format(resource, id))
-        logger.debug("MLOps service:         {}".format(self.options.mlops_service_url))
+        logger.info(f"Deleting {resource} ID {id}...")
+        logger.debug(f"MLOps service:         {self.options.mlops_service_url}")
 
     def _print_resource_generic_action(self, id):
         """Print information for a single resource, according to output format."""
         if self.options.terse:
             print(id)
         elif self.options.json:
             print(json.dumps({"id": id}, indent=1))
@@ -2332,15 +2331,15 @@
             print("No valid subject provided")
             raise SystemExit(ExitCode.INVALID_CLI_INPUT.value)
 
 
 def check_required_parameter(option, env_name, parameter_name):
     if option is None:
         if env_name is None:
-            print("Missing required parameter {}.".format(parameter_name))
+            print(f"Missing required parameter {parameter_name}.")
         else:
             print(
                 "{} must be set via environment variable or via {} parameter.".format(
                     env_name, parameter_name
                 )
             )
         raise SystemExit(ExitCode.INVALID_CLI_INPUT.value)
```

## datarobot/mlops/connected/upload_tracker.py

```diff
@@ -30,30 +30,28 @@
             with open(self._status_filename) as status_file:
                 status = json.load(status_file)
                 self._row_count_uploaded_successfully = status["row_count"]
                 self._iteration = status["iteration"] + 1
                 if "spooler" in status:
                     self._spooler = status["spooler"]
 
-        logger.info("Using status file: '{}'".format(self._status_filename))
+        logger.info(f"Using status file: '{self._status_filename}'")
         if self._spooler is not None:
             logger.info("Setting spooler configuration found in status file")
             self._setup_spooler()
 
     def _setup_spooler(self):
         # Because we are using the same key names, we can simply loop around the dict
         for key, value in self._spooler.items():
             if value is not None:
-                logger.info("Setting Spooler config '{}' to value '{}'".format(key, value))
+                logger.info(f"Setting Spooler config '{key}' to value '{value}'")
                 os.environ[key] = str(value)
 
     def get_status(self):
-        logger.info(
-            "Returning skipped rows count: {}".format(self._row_count_uploaded_successfully)
-        )
+        logger.info(f"Returning skipped rows count: {self._row_count_uploaded_successfully}")
         return self._row_count_uploaded_successfully, self._iteration
 
     def save_spooler(self, spooler):
         self._spooler = spooler.__dict__()
 
     def update_status(self, row_count, iteration):
         self._row_count_uploaded_successfully = row_count
```

## datarobot/mlops/connected/url_helper.py

```diff
@@ -24,19 +24,19 @@
     :param res: path components
     :param params: REST request parameters.
     """
 
     url = host_base_url.rstrip("/")
     for r in res:
         if r is not None:
-            url = "{}/{}".format(url, r)
+            url = f"{url}/{r}"
     if not url.endswith("/"):
         url += "/"
     if params:
-        url = "{}?{}".format(url, urlencode(params))
+        url = f"{url}?{urlencode(params)}"
 
     return url
 
 
 class MMMEndpointPrefix:
     DEPLOYMENT = "api/v2/deployments"
     DATASET = "api/v2/datasets"
@@ -291,15 +291,15 @@
     def get_batch_service_statistics(self, deployment_id, batch_id):
         url = build_url(
             self._service_url,
             MMMEndpointPrefix.DEPLOYMENT,
             deployment_id,
             MMMEndpoint.MONITORING_BATCHES,
         )
-        return "{}{}/".format(url, batch_id)
+        return f"{url}{batch_id}/"
 
     def get_batch_data_drift(self, deployment_id, batch_id):
         return build_url(
             self._service_url,
             MMMEndpointPrefix.DEPLOYMENT,
             deployment_id,
             MMMEndpoint.PREDICTIONS_OVER_BATCH,
```

## Comparing `datarobot_mlops_connected_client-9.0.7.dist-info/METADATA` & `datarobot_mlops_connected_client-9.1.1b1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: datarobot-mlops-connected-client
-Version: 9.0.7
+Version: 9.1.1b1
 Summary: datarobot-mlops-connected-client client to communicate with DataRobot MLOps service
 Home-page: http://datarobot.com
 Author: DataRobot
 Author-email: support@datarobot.com
 Maintainer: DataRobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
 Project-URL: Documentation, https://docs.datarobot.com/en/docs/mlops/deployment/mlops-agent/agent-use.html#monitor-using-the-mlops-cli
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: pandas
 Requires-Dist: requests
-Requires-Dist: datarobot-mlops (>=7.1)
+Requires-Dist: datarobot-mlops (>=9.1.1b1)
 
 # DataRobot MLOps Connected client (mlops-cli)
 
 This is the Python client used to communicate with the
 DataRobot MLOps service. It can be used to upload datasets,
 create and deploy model packages, report predictions files, etc.
 
@@ -40,7 +41,9 @@
 ## Documentation
 
 Once installed, the `help` parameter provides detailed usage information.
 
 ```shell
 $ mlops-cli --help
 ```
+
+
```

## Comparing `datarobot_mlops_connected_client-9.0.7.dist-info/RECORD` & `datarobot_mlops_connected_client-9.1.1b1.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 datarobot/mlops/__init__.py,sha256=AKjMKTNwSwhUBVbzAe95rrPT428dkII5aszufDWlEYw,597
 datarobot/mlops/connected/__init__.py,sha256=gtaquSkCXoIY93Uy5hmlx-TbK6pSnDoGPwV-KeoM-DU,532
-datarobot/mlops/connected/client.py,sha256=Rqdc7Xdq6wJ-nDAZUdxAd9BagxiZUIDs964Iw7Qw6CY,98234
+datarobot/mlops/connected/client.py,sha256=iviglWayMRAxzDRpcoHrHmmYlSjzbdJRWaFc62-1GJc,94846
 datarobot/mlops/connected/enums.py,sha256=ygJSPeoZjdYGWMBGJ3X18RumXqCEsnEdGQB6yqpI77g,1231
-datarobot/mlops/connected/exception.py,sha256=Vz9e1Au5prIzjny9ylBuHt5-C79EyCPsjYg4QgUAxcE,931
-datarobot/mlops/connected/mlops_cli.py,sha256=rfB_-GgU7WtseXkYKv-MVZbptaejrUuuWUm-bzl5pMw,97624
-datarobot/mlops/connected/upload_tracker.py,sha256=UhiJCTiGYc8JOMufZWjyG3iA-ZQSn-7SWZeg8tbGs7A,2694
-datarobot/mlops/connected/url_helper.py,sha256=t-q2qQNTbYyy7oSGxDz6Qf5xII_3bzh1nwumKrEa9us,10281
-datarobot_mlops_connected_client-9.0.7.dist-info/METADATA,sha256=Dh-Ph6lhFo-XLqc3pZG0ZhTdTLOsZTRyLUwnFuAhoms,1510
-datarobot_mlops_connected_client-9.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-datarobot_mlops_connected_client-9.0.7.dist-info/entry_points.txt,sha256=UwMsqtZYVbjeVQGjVh-FrLqSDIb8Y9iacmNva0ZSC1Q,71
-datarobot_mlops_connected_client-9.0.7.dist-info/top_level.txt,sha256=RTK5ZHErXe7mZUlXWQRjQpqFdWw3qmpF95Lz7ViL2Lc,10
-datarobot_mlops_connected_client-9.0.7.dist-info/RECORD,,
+datarobot/mlops/connected/exception.py,sha256=2Y-nd3Lbo6abhvyS3nTUPwnS8sGTdk29-kl3gsuUihA,900
+datarobot/mlops/connected/mlops_cli.py,sha256=6movxevCTCpDct9bHBUzDb_8_iRUq_G3lS7ze8T-YF4,96728
+datarobot/mlops/connected/upload_tracker.py,sha256=sgMVqBgI7xvXtpLYINqnxaw4AljraDVg5Gg3An8pq3A,2646
+datarobot/mlops/connected/url_helper.py,sha256=AJQKndXVQA5L-yluwXG1-vWKH1ASSo7DzGKjcNGXwh4,10251
+datarobot_mlops_connected_client-9.1.1b1.dist-info/METADATA,sha256=PdplKvXR2gM4C3P_wkw1qZz3tGN4Z-dMTAb1ciao38E,1536
+datarobot_mlops_connected_client-9.1.1b1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+datarobot_mlops_connected_client-9.1.1b1.dist-info/entry_points.txt,sha256=pjOHN_gQuYzuqbf0AL5S5lcGhDfIlOGElQU2Qduh2mg,72
+datarobot_mlops_connected_client-9.1.1b1.dist-info/top_level.txt,sha256=RTK5ZHErXe7mZUlXWQRjQpqFdWw3qmpF95Lz7ViL2Lc,10
+datarobot_mlops_connected_client-9.1.1b1.dist-info/RECORD,,
```

