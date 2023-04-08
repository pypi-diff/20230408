# Comparing `tmp/datarobot_bosun-9.0.7-py3-none-any.whl.zip` & `tmp/datarobot_bosun-9.1.1b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,58 +1,71 @@
-Zip file size: 92235 bytes, number of entries: 56
--rw-r--r--  2.0 unx      583 b- defN 23-Apr-07 22:16 bosun/model_connector/__init__.py
--rw-rw-r--  2.0 unx      399 b- defN 23-Apr-07 22:16 bosun/model_connector/config_external.json
--rw-r--r--  2.0 unx     1507 b- defN 23-Apr-07 22:16 bosun/model_connector/constants.py
--rw-r--r--  2.0 unx     1419 b- defN 23-Apr-07 22:16 bosun/model_connector/file_uri_fetcher.py
--rw-r--r--  2.0 unx     7328 b- defN 23-Apr-07 22:16 bosun/model_connector/mc_bosun.py
--rw-r--r--  2.0 unx     5310 b- defN 23-Apr-07 22:16 bosun/model_connector/mc_runner.py
--rw-r--r--  2.0 unx     5526 b- defN 23-Apr-07 22:16 bosun/model_connector/model_connector_base.py
--rw-r--r--  2.0 unx     2373 b- defN 23-Apr-07 22:16 bosun/model_connector/s3_uri_fetcher.py
--rw-r--r--  2.0 unx      894 b- defN 23-Apr-07 22:16 bosun/model_connector/uri_fetcher_base.py
--rw-r--r--  2.0 unx      583 b- defN 23-Apr-07 22:16 bosun/plugin/__init__.py
--rw-r--r--  2.0 unx     2270 b- defN 23-Apr-07 22:16 bosun/plugin/action_status.py
--rw-r--r--  2.0 unx     5513 b- defN 23-Apr-07 22:16 bosun/plugin/bosun_plugin_base.py
--rw-r--r--  2.0 unx    11655 b- defN 23-Apr-07 22:16 bosun/plugin/bosun_test_plugin.py
--rw-r--r--  2.0 unx     2707 b- defN 23-Apr-07 22:16 bosun/plugin/constants.py
--rw-r--r--  2.0 unx     3066 b- defN 23-Apr-07 22:16 bosun/plugin/deployment_info.py
--rw-r--r--  2.0 unx     1047 b- defN 23-Apr-07 22:16 bosun/plugin/exceptions.py
--rw-r--r--  2.0 unx     2109 b- defN 23-Apr-07 22:16 bosun/plugin/pe_info.py
--rw-r--r--  2.0 unx    17074 b- defN 23-Apr-07 22:16 bosun/plugin/plugin_runner.py
--rw-r--r--  2.0 unx      702 b- defN 23-Apr-07 22:16 bosun/plugin/config_samples/__init__.py
--rw-r--r--  2.0 unx      757 b- defN 23-Apr-07 22:16 bosun/plugin/docker/__init__.py
--rw-r--r--  2.0 unx    15366 b- defN 23-Apr-07 22:16 bosun/plugin/docker/docker_helper.py
--rw-r--r--  2.0 unx    23613 b- defN 23-Apr-07 22:16 bosun/plugin/docker/docker_plugin.py
--rw-r--r--  2.0 unx     5439 b- defN 23-Apr-07 22:16 bosun/plugin/docker/docker_plugin_config.py
--rw-r--r--  2.0 unx     7945 b- defN 23-Apr-07 22:16 bosun/plugin/docker/mlops_monitoring.py
--rw-r--r--  2.0 unx      646 b- defN 23-Apr-07 22:16 bosun/plugin/filesystem/__init__.py
--rw-r--r--  2.0 unx    14203 b- defN 23-Apr-07 22:16 bosun/plugin/filesystem/filesystem_plugin.py
--rw-r--r--  2.0 unx      646 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/__init__.py
--rw-r--r--  2.0 unx    36684 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/client.py
--rw-r--r--  2.0 unx    19957 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/config.py
--rw-r--r--  2.0 unx    27946 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/kubernetes_plugin.py
--rw-r--r--  2.0 unx     9182 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/manifests.py
--rw-rw-r--  2.0 unx      303 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/templates/Dockerfile.pps-model.j2
--rw-rw-r--  2.0 unx     2263 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/templates/_helpers.j2
--rw-rw-r--  2.0 unx     4603 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/templates/cm_pps_installer.sh.j2
--rw-rw-r--  2.0 unx     1393 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/templates/image-builder.yaml.j2
--rw-rw-r--  2.0 unx      356 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/templates/mlops-api-secret.yaml.j2
--rw-rw-r--  2.0 unx     1106 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/templates/model-resources.yaml.j2
--rw-rw-r--  2.0 unx     4929 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/templates/model-resources/deployment.yaml.j2
--rw-rw-r--  2.0 unx      119 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/templates/model-resources/extra.yaml.j2
--rw-rw-r--  2.0 unx      842 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/templates/model-resources/hpa.yaml.j2
--rw-rw-r--  2.0 unx     1253 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/templates/model-resources/ingress.yaml.j2
--rw-rw-r--  2.0 unx      554 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/templates/model-resources/pdb.yaml.j2
--rw-rw-r--  2.0 unx      547 b- defN 23-Apr-07 22:16 bosun/plugin/k8s/templates/model-resources/service.yaml.j2
--rw-r--r--  2.0 unx      630 b- defN 23-Apr-07 22:16 bosun/plugin/s3/__init__.py
--rw-r--r--  2.0 unx    11310 b- defN 23-Apr-07 22:16 bosun/plugin/s3/s3_plugin.py
--rw-r--r--  2.0 unx     2735 b- defN 23-Apr-07 22:16 bosun/plugin/s3/s3_plugin_config.py
--rw-r--r--  2.0 unx      644 b- defN 23-Apr-07 22:16 bosun/plugin/snowflake/__init__.py
--rw-r--r--  2.0 unx    10353 b- defN 23-Apr-07 22:16 bosun/plugin/snowflake/snowflake_plugin.py
--rw-r--r--  2.0 unx     5583 b- defN 23-Apr-07 22:16 bosun/plugin/snowflake/snowflake_plugin_config.py
--rwxr-xr-x  2.0 unx      671 b- defN 23-Apr-07 22:24 datarobot_bosun-9.0.7.data/scripts/bosun-plugin-runner
--rwxr-xr-x  2.0 unx      676 b- defN 23-Apr-07 22:24 datarobot_bosun-9.0.7.data/scripts/mcrunner
--rwxr-xr-x  2.0 unx      671 b- defN 23-Apr-07 22:24 datarobot_bosun-9.0.7.data/scripts/plugin-runner
--rw-r--r--  2.0 unx     4246 b- defN 23-Apr-07 22:24 datarobot_bosun-9.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-07 22:24 datarobot_bosun-9.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Apr-07 22:24 datarobot_bosun-9.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     5315 b- defN 23-Apr-07 22:24 datarobot_bosun-9.0.7.dist-info/RECORD
-56 files, 295649 bytes uncompressed, 83575 bytes compressed:  71.7%
+Zip file size: 114437 bytes, number of entries: 69
+-rw-r--r--  2.0 unx      583 b- defN 23-Mar-27 23:33 bosun/model_connector/__init__.py
+-rw-rw-r--  2.0 unx      399 b- defN 23-Mar-27 23:33 bosun/model_connector/config_external.json
+-rw-r--r--  2.0 unx     1507 b- defN 23-Mar-27 23:33 bosun/model_connector/constants.py
+-rw-r--r--  2.0 unx     1395 b- defN 23-Mar-27 23:33 bosun/model_connector/file_uri_fetcher.py
+-rw-r--r--  2.0 unx     7190 b- defN 23-Mar-27 23:33 bosun/model_connector/mc_bosun.py
+-rw-r--r--  2.0 unx     5269 b- defN 23-Mar-27 23:33 bosun/model_connector/mc_runner.py
+-rw-r--r--  2.0 unx     5433 b- defN 23-Mar-27 23:33 bosun/model_connector/model_connector_base.py
+-rw-r--r--  2.0 unx     2334 b- defN 23-Mar-27 23:33 bosun/model_connector/s3_uri_fetcher.py
+-rw-r--r--  2.0 unx      894 b- defN 23-Mar-27 23:33 bosun/model_connector/uri_fetcher_base.py
+-rw-r--r--  2.0 unx      583 b- defN 23-Mar-27 23:33 bosun/plugin/__init__.py
+-rw-r--r--  2.0 unx     2225 b- defN 23-Mar-27 23:33 bosun/plugin/action_status.py
+-rw-r--r--  2.0 unx     5957 b- defN 23-Mar-27 23:33 bosun/plugin/bosun_plugin_base.py
+-rw-r--r--  2.0 unx    11466 b- defN 23-Mar-27 23:33 bosun/plugin/bosun_test_plugin.py
+-rw-r--r--  2.0 unx     2735 b- defN 23-Mar-27 23:33 bosun/plugin/constants.py
+-rw-r--r--  2.0 unx     3354 b- defN 23-Mar-27 23:33 bosun/plugin/deployment_info.py
+-rw-r--r--  2.0 unx     1047 b- defN 23-Mar-27 23:33 bosun/plugin/exceptions.py
+-rw-r--r--  2.0 unx     2493 b- defN 23-Mar-27 23:33 bosun/plugin/pe_info.py
+-rw-r--r--  2.0 unx    16631 b- defN 23-Mar-27 23:33 bosun/plugin/plugin_runner.py
+-rw-r--r--  2.0 unx      640 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/__init__.py
+-rw-r--r--  2.0 unx     8275 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/azureml_plugin.py
+-rw-r--r--  2.0 unx     3058 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/azureml_status_reporter.py
+-rw-r--r--  2.0 unx     1504 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/template_renderer.py
+-rw-r--r--  2.0 unx    10060 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/client/base_endpoint_client.py
+-rw-r--r--  2.0 unx     5885 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/client/batch_endpoint_client.py
+-rw-r--r--  2.0 unx    12088 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/client/online_endpoint_client.py
+-rw-r--r--  2.0 unx     1680 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/client/scoring_snippets.py
+-rw-r--r--  2.0 unx      583 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/config/__init__.py
+-rw-r--r--  2.0 unx     8036 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/config/azureml_client_config.py
+-rw-r--r--  2.0 unx     3059 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/config/config_keys.py
+-rw-r--r--  2.0 unx     3368 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/templates/azureml_batch_endpoint_score.py
+-rw-r--r--  2.0 unx     4814 b- defN 23-Mar-27 23:33 bosun/plugin/azureml/templates/azureml_online_endpoint_score.py
+-rw-r--r--  2.0 unx      702 b- defN 23-Mar-27 23:33 bosun/plugin/config_samples/__init__.py
+-rw-r--r--  2.0 unx      757 b- defN 23-Mar-27 23:33 bosun/plugin/docker/__init__.py
+-rw-r--r--  2.0 unx    14934 b- defN 23-Mar-27 23:33 bosun/plugin/docker/docker_helper.py
+-rw-r--r--  2.0 unx    23290 b- defN 23-Mar-27 23:33 bosun/plugin/docker/docker_plugin.py
+-rw-r--r--  2.0 unx     5419 b- defN 23-Mar-27 23:33 bosun/plugin/docker/docker_plugin_config.py
+-rw-r--r--  2.0 unx     7897 b- defN 23-Mar-27 23:33 bosun/plugin/docker/mlops_monitoring.py
+-rw-r--r--  2.0 unx      646 b- defN 23-Mar-27 23:33 bosun/plugin/filesystem/__init__.py
+-rw-r--r--  2.0 unx    14021 b- defN 23-Mar-27 23:33 bosun/plugin/filesystem/filesystem_plugin.py
+-rw-r--r--  2.0 unx      646 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/__init__.py
+-rw-r--r--  2.0 unx    37071 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/client.py
+-rw-r--r--  2.0 unx    19918 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/config.py
+-rw-r--r--  2.0 unx    28164 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/kubernetes_plugin.py
+-rw-r--r--  2.0 unx     9170 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/manifests.py
+-rw-rw-r--  2.0 unx      303 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/Dockerfile.pps-model.j2
+-rw-rw-r--  2.0 unx     2263 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/_helpers.j2
+-rw-rw-r--  2.0 unx     4603 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/cm_pps_installer.sh.j2
+-rw-rw-r--  2.0 unx     1393 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/image-builder.yaml.j2
+-rw-rw-r--  2.0 unx      356 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/mlops-api-secret.yaml.j2
+-rw-rw-r--  2.0 unx     1106 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/model-resources.yaml.j2
+-rw-rw-r--  2.0 unx     4929 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/model-resources/deployment.yaml.j2
+-rw-rw-r--  2.0 unx      119 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/model-resources/extra.yaml.j2
+-rw-rw-r--  2.0 unx      842 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/model-resources/hpa.yaml.j2
+-rw-rw-r--  2.0 unx     1253 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/model-resources/ingress.yaml.j2
+-rw-rw-r--  2.0 unx      484 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/model-resources/pdb.yaml.j2
+-rw-rw-r--  2.0 unx      547 b- defN 23-Mar-27 23:33 bosun/plugin/k8s/templates/model-resources/service.yaml.j2
+-rw-r--r--  2.0 unx      630 b- defN 23-Mar-27 23:33 bosun/plugin/s3/__init__.py
+-rw-r--r--  2.0 unx    11175 b- defN 23-Mar-27 23:33 bosun/plugin/s3/s3_plugin.py
+-rw-r--r--  2.0 unx     2705 b- defN 23-Mar-27 23:33 bosun/plugin/s3/s3_plugin_config.py
+-rw-r--r--  2.0 unx      644 b- defN 23-Mar-27 23:33 bosun/plugin/snowflake/__init__.py
+-rw-r--r--  2.0 unx    10034 b- defN 23-Mar-27 23:33 bosun/plugin/snowflake/snowflake_plugin.py
+-rw-r--r--  2.0 unx     5491 b- defN 23-Mar-27 23:33 bosun/plugin/snowflake/snowflake_plugin_config.py
+-rwxr-xr-x  2.0 unx      671 b- defN 23-Mar-27 23:41 datarobot_bosun-9.1.1b1.data/scripts/bosun-plugin-runner
+-rwxr-xr-x  2.0 unx      676 b- defN 23-Mar-27 23:41 datarobot_bosun-9.1.1b1.data/scripts/mcrunner
+-rwxr-xr-x  2.0 unx      671 b- defN 23-Mar-27 23:41 datarobot_bosun-9.1.1b1.data/scripts/plugin-runner
+-rw-r--r--  2.0 unx     4470 b- defN 23-Mar-27 23:41 datarobot_bosun-9.1.1b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-27 23:41 datarobot_bosun-9.1.1b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Mar-27 23:41 datarobot_bosun-9.1.1b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     6689 b- defN 23-Mar-27 23:41 datarobot_bosun-9.1.1b1.dist-info/RECORD
+69 files, 359332 bytes uncompressed, 103523 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -48,14 +48,53 @@
 
 Filename: bosun/plugin/pe_info.py
 Comment: 
 
 Filename: bosun/plugin/plugin_runner.py
 Comment: 
 
+Filename: bosun/plugin/azureml/__init__.py
+Comment: 
+
+Filename: bosun/plugin/azureml/azureml_plugin.py
+Comment: 
+
+Filename: bosun/plugin/azureml/azureml_status_reporter.py
+Comment: 
+
+Filename: bosun/plugin/azureml/template_renderer.py
+Comment: 
+
+Filename: bosun/plugin/azureml/client/base_endpoint_client.py
+Comment: 
+
+Filename: bosun/plugin/azureml/client/batch_endpoint_client.py
+Comment: 
+
+Filename: bosun/plugin/azureml/client/online_endpoint_client.py
+Comment: 
+
+Filename: bosun/plugin/azureml/client/scoring_snippets.py
+Comment: 
+
+Filename: bosun/plugin/azureml/config/__init__.py
+Comment: 
+
+Filename: bosun/plugin/azureml/config/azureml_client_config.py
+Comment: 
+
+Filename: bosun/plugin/azureml/config/config_keys.py
+Comment: 
+
+Filename: bosun/plugin/azureml/templates/azureml_batch_endpoint_score.py
+Comment: 
+
+Filename: bosun/plugin/azureml/templates/azureml_online_endpoint_score.py
+Comment: 
+
 Filename: bosun/plugin/config_samples/__init__.py
 Comment: 
 
 Filename: bosun/plugin/docker/__init__.py
 Comment: 
 
 Filename: bosun/plugin/docker/docker_helper.py
@@ -141,29 +180,29 @@
 
 Filename: bosun/plugin/snowflake/snowflake_plugin.py
 Comment: 
 
 Filename: bosun/plugin/snowflake/snowflake_plugin_config.py
 Comment: 
 
-Filename: datarobot_bosun-9.0.7.data/scripts/bosun-plugin-runner
+Filename: datarobot_bosun-9.1.1b1.data/scripts/bosun-plugin-runner
 Comment: 
 
-Filename: datarobot_bosun-9.0.7.data/scripts/mcrunner
+Filename: datarobot_bosun-9.1.1b1.data/scripts/mcrunner
 Comment: 
 
-Filename: datarobot_bosun-9.0.7.data/scripts/plugin-runner
+Filename: datarobot_bosun-9.1.1b1.data/scripts/plugin-runner
 Comment: 
 
-Filename: datarobot_bosun-9.0.7.dist-info/METADATA
+Filename: datarobot_bosun-9.1.1b1.dist-info/METADATA
 Comment: 
 
-Filename: datarobot_bosun-9.0.7.dist-info/WHEEL
+Filename: datarobot_bosun-9.1.1b1.dist-info/WHEEL
 Comment: 
 
-Filename: datarobot_bosun-9.0.7.dist-info/top_level.txt
+Filename: datarobot_bosun-9.1.1b1.dist-info/top_level.txt
 Comment: 
 
-Filename: datarobot_bosun-9.0.7.dist-info/RECORD
+Filename: datarobot_bosun-9.1.1b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bosun/model_connector/file_uri_fetcher.py

```diff
@@ -28,12 +28,12 @@
         super().__init__("file", base_dir)
 
     def fetch_artifact(self, uri):
         orig_file_path = unquote(urlparse(uri).path)
         priv_file_path = os.path.join(
             self._base_dir, os.path.basename(orig_file_path) + "_" + str(uuid.uuid4())
         )
-        logger.info("uri:            {}".format(uri))
-        logger.info("orig_file_path: {}".format(orig_file_path))
-        logger.info("priv_file_path: {}".format(priv_file_path))
+        logger.info(f"uri:            {uri}")
+        logger.info(f"orig_file_path: {orig_file_path}")
+        logger.info(f"priv_file_path: {priv_file_path}")
         shutil.copyfile(orig_file_path, priv_file_path)
         return priv_file_path
```

## bosun/model_connector/mc_bosun.py

```diff
@@ -48,58 +48,54 @@
         """
         The base class constructor.
         :type config: configuration dictionary
         :param config: The plugin config dict
         """
         super().__init__(
             config,
-            logging.getLogger("{}.{}".format(self.__class__.__module__, self.__class__.__name__)),
+            logging.getLogger(f"{self.__class__.__module__}.{self.__class__.__name__}"),
         )
         file_fetcher = FileURIFetcher(config[ModelConnectorConstants.TMP_DIR_KEY])
         self._external_model_fetchers = {file_fetcher.get_prefix(): file_fetcher}
 
         try:
             from bosun.model_connector.s3_uri_fetcher import S3Fetcher
 
             s3 = S3Fetcher(config[ModelConnectorConstants.TMP_DIR_KEY])
             self._external_model_fetchers[s3.get_prefix()] = s3
         except ImportError:
             self._logger.info("S3 support is not available")
 
     def _handle_external_model(self, config):
         url = config[ModelPackageConstants.MODEL_LOCATION_KEY]
-        self._logger.info("Found external model .. handling via location: {}".format(url))
+        self._logger.info(f"Found external model .. handling via location: {url}")
 
         result = urlparse(url)
         if result.scheme not in self._external_model_fetchers:
-            raise Exception(
-                "URL Scheme is not supported: {} (for uri: {})".format(result.scheme, url)
-            )
+            raise Exception(f"URL Scheme is not supported: {result.scheme} (for uri: {url})")
 
         fetcher = self._external_model_fetchers[result.scheme]
         try:
             local_path = fetcher.fetch_artifact(url)
         except Exception as e:
-            raise Exception("Error fetching external uri: {} {}".format(url, str(e)))
-        self._logger.info("Model is in: {}".format(local_path))
+            raise Exception(f"Error fetching external uri: {url} {str(e)}")
+        self._logger.info(f"Model is in: {local_path}")
         return local_path
 
     def _handle_custom_models(self, config):
         return self._handle_model(config, download_scoring_code=False, download_pps_installer=True)
 
     def _handle_dr_native_model(self, config):
         model_format = config.get(ModelPackageConstants.MODEL_FORMAT_KEY)
 
         if model_format not in [
             ModelPackageConstants.MODEL_FORMAT_SCORING_CODE,
             ModelPackageConstants.MODEL_FORMAT_MLPKG,
         ]:
-            raise Exception(
-                "Model format '{}' is not supported for DataRobot models".format(model_format)
-            )
+            raise Exception(f"Model format '{model_format}' is not supported for DataRobot models")
         download_scoring_code = False
         scoring_code_binary = False
         if model_format == ModelPackageConstants.MODEL_FORMAT_SCORING_CODE:
             download_scoring_code = True
             # model with PE support should be built prior to download
             scoring_code_binary = not config[ModelPackageConstants.MODEL_PREDICTION_EXPLANATIONS]
 
@@ -128,38 +124,38 @@
             download_scoring_code=download_scoring_code,
             scoring_code_binary=scoring_code_binary,
             download_pps_installer=download_pps_installer,
             is_prediction_explanations_supported=is_prediction_explanations,
             timeout=600,
         )
 
-        self._logger.info("Model download complete. Model at {}".format(model_artifact_path))
+        self._logger.info(f"Model download complete. Model at {model_artifact_path}")
         return model_artifact_path
 
     def get_model(self, config):
         """
         :param config: configuration dictionary
         """
         if self._logger.isEnabledFor(logging.INFO):
-            self._logger.info("get_model: {}".format(self.get_sanitized_config(config)))
+            self._logger.info(f"get_model: {self.get_sanitized_config(config)}")
         et = config[ModelPackageConstants.MODEL_EXECUTION_TYPE_KEY]
 
         if et == ModelPackageConstants.MODEL_EXECUTION_EXTERNAL:
             model_path = self._handle_external_model(config)
             return ActionStatusInfo(ActionStatus.OK, model_path=model_path)
         elif et == ModelPackageConstants.MODEL_EXECUTION_DEDICATED:
             self._logger.info("Found dedicated model .. downloading")
             model_path = self._handle_dr_native_model(config)
             return ActionStatusInfo(ActionStatus.OK, model_path=model_path)
         elif et == ModelPackageConstants.MODEL_EXECUTION_CUSTOM_INFERENCE:
             self._logger.info("Found custom model .. downloading")
             model_path = self._handle_custom_models(config)
             return ActionStatusInfo(ActionStatus.OK, model_path=model_path)
         else:
-            raise Exception("Model execution type: {} is not recognized".format(et))
+            raise Exception(f"Model execution type: {et} is not recognized")
 
     @staticmethod
     def get_sanitized_config(parsed_config):
         sanitized = parsed_config.copy()
         if ModelConnectorConstants.DR_TOKEN_KEY in sanitized:
             masked = sanitized[ModelConnectorConstants.DR_TOKEN_KEY][:12] + "*******"
             sanitized[ModelConnectorConstants.DR_TOKEN_KEY] = masked
```

## bosun/model_connector/mc_runner.py

```diff
@@ -14,14 +14,15 @@
 import argparse
 import logging
 import os
 import sys
 from pprint import pformat
 
 import yaml
+
 from bosun.model_connector.constants import ModelConnectorConstants
 from bosun.model_connector.mc_bosun import MCBosun
 from bosun.model_connector.model_connector_base import ActionStatus
 from bosun.model_connector.model_connector_base import ActionStatusInfo
 
 
 class MCRunner:
@@ -32,17 +33,15 @@
         "modelId": "5eaa29d511bf057c2147fe6d",
         "id": "5eaa29d511bf057c2147fe6d",
         "modelExecutionType": "external",
         "location": "file:///opt/model/my_model.zip",
     }
 
     def __init__(self, config_file, action, status_file):
-        self._logger = logging.getLogger(
-            "{}.{}".format(self.__class__.__module__, self.__class__.__name__)
-        )
+        self._logger = logging.getLogger(f"{self.__class__.__module__}.{self.__class__.__name__}")
         self._config_file = config_file
         self._action = action
         self._status_file = status_file
 
     @staticmethod
     def parse_args():
         parser = argparse.ArgumentParser()
@@ -99,15 +98,15 @@
         logger = logging.getLogger("main")
 
         try:
             config = self.get_config(self._config_file, logger)
             mc = MCBosun(config)
             action_status = mc.run_action(self._action, config)
         except Exception as e:
-            msg = "Exception occurred while running action {} : error {}".format(self._action, e)
+            msg = f"Exception occurred while running action {self._action} : error {e}"
             self._logger.exception(msg)
             action_status = ActionStatusInfo(ActionStatus.ERROR, msg=msg)
 
         if self._status_file:
             with open(self._status_file, "w") as status_fh:
                 status_fh.write(action_status.to_yaml())
```

## bosun/model_connector/model_connector_base.py

```diff
@@ -13,14 +13,15 @@
 
 import datetime
 from abc import ABC
 from abc import abstractmethod
 
 import pytz
 import yaml
+
 from bosun.model_connector.constants import ModelConnectorConstants
 from bosun.model_connector.constants import ModelPackageConstants
 
 
 class ActionStatus:
     OK = "passing"
     WARN = "warning"
@@ -34,15 +35,15 @@
 
 
 class ActionStatusInfo:
     def __init__(self, status, model_path=None, msg=None, duration=None):
         if ActionStatus.is_valid(status):
             self.status = status
         else:
-            raise Exception("Bad Status: {}".format(status))
+            raise Exception(f"Bad Status: {status}")
         self.msg = msg
         self.duration = duration
         d = datetime.datetime.utcnow()
         d_with_timezone = d.replace(tzinfo=pytz.UTC)
         d_with_timezone.isoformat()
         self.timestamp = str(d_with_timezone)
 
@@ -52,15 +53,15 @@
         return yaml.dump(self.__dict__, indent=4)
 
 
 def find_or_throw(info, item, parent_item):
     if item in info:
         return info[item]
 
-    err_msg = "Could not find {} in {} information".format(item, parent_item)
+    err_msg = f"Could not find {item} in {parent_item} information"
     raise Exception(err_msg)
 
 
 class ModelPackage:
     def __init__(self, info):
         self._info = info
 
@@ -131,15 +132,15 @@
     def set_mlops_url(self, url):
         self.dr_url = url
 
     def set_mlops_token(self, token):
         self.dr_token = token
 
     def __str__(self):
-        return "tmp_dir: {} url: {} token: {}".format(self.tmp_dir, self.dr_url, self.dr_token[-4:])
+        return f"tmp_dir: {self.tmp_dir} url: {self.dr_url} token: {self.dr_token[-4:]}"
 
 
 class ModelConnectorBase(ABC):
     def __init__(self, config, logger):
         """
         The base class constructor.
         :param config:  The plugin config dict
@@ -160,18 +161,16 @@
 
                 if action_status.model_path is None:
                     raise Exception(
                         "get_model operation should return a model_path " "field in status"
                     )
 
             else:
-                raise Exception("Action is not supported: {}".format(action))
+                raise Exception(f"Action is not supported: {action}")
             if not isinstance(action_status, ActionStatusInfo):
-                raise Exception(
-                    "Action {} provide - did not return ActionStatusInfo object".format(action)
-                )
+                raise Exception(f"Action {action} provide - did not return ActionStatusInfo object")
         except Exception as e:
-            msg = "Exception occurred while running action {} : error {}".format(action, e)
+            msg = f"Exception occurred while running action {action} : error {e}"
             self._logger.error(msg)
             action_status = ActionStatusInfo(ActionStatus.ERROR, msg=msg)
 
         return action_status
```

## bosun/model_connector/s3_uri_fetcher.py

```diff
@@ -13,20 +13,21 @@
 
 import logging
 import os
 import uuid
 from urllib.parse import urlparse
 
 import boto3
+
 from bosun.model_connector.uri_fetcher_base import URIFetcherBase
 
 logger = logging.getLogger(__name__)
 
 
-class S3Url(object):
+class S3Url:
     """
     >>> s = S3Url("s3://bucket/hello/world")
     >>> s.bucket
     'bucket'
     >>> s.key
     'hello/world'
     >>> s.url
@@ -72,13 +73,13 @@
 
     def fetch_artifact(self, uri):
         client = boto3.client("s3")
         s3_url = S3Url(uri)
         file_name = os.path.join(
             self._base_dir, os.path.basename(s3_url.key) + "_" + str(uuid.uuid4())
         )
-        logger.info("uri:    {}".format(uri))
-        logger.info("bucket: {}".format(s3_url.bucket))
-        logger.info("key:    {}".format(s3_url.key))
-        logger.info("local:  {}".format(file_name))
+        logger.info(f"uri:    {uri}")
+        logger.info(f"bucket: {s3_url.bucket}")
+        logger.info(f"key:    {s3_url.key}")
+        logger.info(f"local:  {file_name}")
         client.download_file(s3_url.bucket, s3_url.key, file_name)
         return file_name
```

## bosun/plugin/action_status.py

```diff
@@ -38,31 +38,31 @@
         OK: 0,
         ERROR: 1,
         WARN: 2,
         UNKNOWN: 3,
     }
 
     @classmethod
-    def is_valid(self, status_string):
+    def is_valid(cls, status_string):
         if status_string in (
-            ActionStatus.OK,
-            ActionStatus.WARN,
-            ActionStatus.ERROR,
-            ActionStatus.UNKNOWN,
+            cls.OK,
+            cls.WARN,
+            cls.ERROR,
+            cls.UNKNOWN,
         ):
             return True
         return False
 
 
 class ActionStatusInfo:
     def __init__(self, status, msg=None, state=None, duration=None, data=None):
         if ActionStatus.is_valid(status):
             self.status = status
         else:
-            raise Exception("Bad Status: {}".format(status))
+            raise Exception(f"Bad Status: {status}")
         self.msg = msg
         self.duration = duration
         self.timestamp = int(time.time() * 1000)
         self.state = state
         self.data = data
 
     def set_duration(self, duration):
```

## bosun/plugin/bosun_plugin_base.py

```diff
@@ -12,123 +12,126 @@
 #  --------------------------------------------------------------------------------
 
 import logging
 import time
 import traceback
 from abc import ABC
 from abc import abstractmethod
+from typing import Optional
 
 from bosun.plugin.action_status import ActionStatus
 from bosun.plugin.action_status import ActionStatusInfo
 from bosun.plugin.constants import BosunPluginActions
 from bosun.plugin.constants import BosunPluginConfigConstants
+from bosun.plugin.deployment_info import DeploymentInfo
 from bosun.plugin.pe_info import PEInfo
 
 
 class BosunPluginBase(ABC):
-    def __init__(self, plugin_config, private_config_file, pe_info, dry_run):
+    def __init__(
+        self,
+        plugin_config,
+        private_config_file,
+        pe_info: Optional[dict] = None,
+        dry_run: bool = False,
+    ):
         """
         The baseclass constructor.
         :param plugin_config:  The plugin config dict
         :param pe_info: The PE info dict
         """
         self._plugin_config = plugin_config
         self._private_config_file = private_config_file
-        if pe_info:
-            self._pe_info = PEInfo(pe_info)
-        else:
-            self._pe_info = pe_info
-        self._logger = logging.getLogger(
-            "{}.{}".format(self.__class__.__module__, self.__class__.__name__)
-        )
+        self._pe_info = PEInfo(pe_info) if pe_info else None
+        self._logger = logging.getLogger(f"{self.__class__.__module__}.{self.__class__.__name__}")
         self._dry_run = dry_run
 
     @abstractmethod
-    def plugin_start(self):
+    def plugin_start(self) -> ActionStatusInfo:
         pass
 
     @abstractmethod
-    def plugin_stop(self):
+    def plugin_stop(self) -> ActionStatusInfo:
         pass
 
     @abstractmethod
-    def deployment_list(self):
+    def deployment_list(self) -> ActionStatusInfo:
         pass
 
     @abstractmethod
-    def deployment_start(self, deployment_info):
+    def deployment_start(self, deployment_info: DeploymentInfo) -> ActionStatusInfo:
         pass
 
     @abstractmethod
-    def deployment_stop(self, deployment_info):
+    def deployment_stop(self, deployment_id: str) -> ActionStatusInfo:
         pass
 
     @abstractmethod
-    def deployment_replace_model(self, deployment_info):
+    def deployment_replace_model(self, deployment_info: DeploymentInfo) -> ActionStatusInfo:
         pass
 
     @abstractmethod
-    def pe_status(self):
+    def pe_status(self) -> ActionStatusInfo:
         """
         Check status of PE - possibly also reporting status on each deployment in this pe.
         :return:
         """
         pass
 
     @abstractmethod
-    def deployment_status(self, deployment_info):
+    def deployment_status(self, deployment_info: DeploymentInfo) -> ActionStatusInfo:
         pass
 
-    def deployment_relaunch(self, deployment_info):
+    def deployment_relaunch(self, deployment_info: DeploymentInfo) -> ActionStatusInfo:
         """
         Default relaunch implementation for now is "stop" + "start", but if any plugin
         wants to implement a different logic, it should implement its own relaunch mechanism
 
+        The default implementation ignores any errors during the "stop" action.
+
         :param deployment_info:
         :return:
         """
         self._logger.info("Processing deployment relaunch")
-        status = self.deployment_stop(deployment_info)
-        self._logger.info("Deployment stop status: {}".format(status))
+        status = self.deployment_stop(deployment_info.id)
+        self._logger.info("Deployment stop status: %s", status)
         # Default processing ignores any stop errors, because deployment is going to be launched
         # again soon.  But, if plugin wants to handle the stop error, then it will need its own
         # deployment_relaunch implementation
         return self.deployment_start(deployment_info)
 
-    def run_action(self, action, deployment_info, status_file=None):
+    def run_action(self, action: str, deployment_info: dict, status_file=None) -> ActionStatusInfo:
 
         action_start = time.time()
         try:
 
             if action == BosunPluginActions.PLUGIN_START:
                 action_status = self.plugin_start()
             elif action == BosunPluginActions.PLUGIN_STOP:
                 action_status = self.plugin_stop()
             elif action == BosunPluginActions.DEPLOYMENT_START:
-                action_status = self.deployment_start(deployment_info)
+                action_status = self.deployment_start(DeploymentInfo(deployment_info))
             elif action == BosunPluginActions.DEPLOYMENT_STOP:
-                action_status = self.deployment_stop(deployment_info)
+                action_status = self.deployment_stop(deployment_info["id"])
             elif action == BosunPluginActions.DEPLOYMENT_REPLACE_MODEL:
-                action_status = self.deployment_replace_model(deployment_info)
+                action_status = self.deployment_replace_model(DeploymentInfo(deployment_info))
             elif action == BosunPluginActions.DEPLOYMENT_STATUS:
-                action_status = self.deployment_status(deployment_info)
+                action_status = self.deployment_status(DeploymentInfo(deployment_info))
             elif action == BosunPluginActions.PE_STATUS:
                 action_status = self.pe_status()
             elif action == BosunPluginActions.DEPLOYMENT_LIST:
                 action_status = self.deployment_list()
             elif action == BosunPluginActions.DEPLOYMENT_RELAUNCH:
-                action_status = self.deployment_relaunch(deployment_info)
+                action_status = self.deployment_relaunch(DeploymentInfo(deployment_info))
             else:
-                raise Exception("Action is not supported: {}".format(action))
+                raise Exception(f"Action is not supported: {action}")
             if not isinstance(action_status, ActionStatusInfo):
-                raise Exception(
-                    "Action {} provide - did not return ActionStatusInfo object".format(action)
-                )
+                raise Exception(f"Action {action} provide - did not return ActionStatusInfo object")
         except Exception as e:
-            msg = "Exception occurred while running action {} : error {}".format(action, e)
+            msg = f"Exception occurred while running action {action} : error {e}"
             self._logger.error(msg)
             traceback.print_exc()
             action_status = ActionStatusInfo(ActionStatus.ERROR, msg=msg, state="errored")
 
         action_end = time.time()
         action_status.set_duration(round(action_end - action_start, 4))
         action_status.write_to_file(status_file=status_file)
```

## bosun/plugin/bosun_test_plugin.py

```diff
@@ -15,14 +15,15 @@
 import glob
 import json
 import logging
 import os
 import time
 
 import yaml
+
 from bosun.plugin.action_status import ActionDataFields
 from bosun.plugin.action_status import ActionStatus
 from bosun.plugin.action_status import ActionStatusInfo
 from bosun.plugin.bosun_plugin_base import BosunPluginBase
 from bosun.plugin.constants import DeploymentState
 from bosun.plugin.deployment_info import DeploymentInfo
 
@@ -33,19 +34,19 @@
     any "real" action, but will call time.sleep instead and will print some information about the
     action being called into the logs.
     """
 
     CONFIG_FILE_ENTRY = "config_file"
 
     def __init__(
-        self, plugin_config: object, private_config_file: str, pe_info: object, dry_run: bool
-    ) -> object:
+        self, plugin_config: object, private_config_file: str, pe_info: dict, dry_run: bool
+    ):
         super().__init__(plugin_config, private_config_file, pe_info, False)
         if self._logger.isEnabledFor(logging.DEBUG):
-            self._logger.debug("plugin config: {}".format(self.get_sanitized_config(plugin_config)))
+            self._logger.debug(f"plugin config: {self.get_sanitized_config(plugin_config)}")
 
         # The plugin config dictionary can contain a pointer to a private config file for this
         # specific plugin script. So we can get specific config in any format known only to this
         # implementation of the plugin.
         if private_config_file:
             with open(private_config_file) as config_fh:
                 private_config = json.load(config_fh)
@@ -68,32 +69,32 @@
             raise Exception("Bosun Test plugin is raising an exception")
 
     def _get_pe_filename(self):
         return os.path.join(
             self._plugin_tmp_dir, "pe_" + self._plugin_config["MLOPS_BOSUN_PRED_ENV_ID"] + ".yaml"
         )
 
-    def _get_deployment_filename(self, deployment_info):
-        return self._get_deployment_filename_from_id(deployment_info["id"])
+    def _get_deployment_filename(self, deployment_info: DeploymentInfo):
+        return self._get_deployment_filename_from_id(deployment_info.id)
 
     def _get_deployment_filename_from_id(self, deployment_id):
         return os.path.join(self._plugin_tmp_dir, "deployment_" + deployment_id + ".yaml")
 
     @staticmethod
-    def _get_deployment_content(deployment_info):
+    def _get_deployment_content(deployment_info: DeploymentInfo):
         content = {
-            "name": deployment_info["name"],
-            "model_id": deployment_info["modelId"],
-            "key_value_config": deployment_info["keyValueConfig"],
-            "model_execution_type": deployment_info["modelExecutionType"],
-            "model_artifact": deployment_info["modelArtifact"],
+            "name": deployment_info.name,
+            "model_id": deployment_info.model_id,
+            "key_value_config": deployment_info.kv_config,
+            "model_execution_type": deployment_info.model_execution_type,
+            "model_artifact": str(deployment_info.model_artifact),
             "state": "running",
         }
-        if "newModelId" in deployment_info:
-            content["new_model_id"] = deployment_info["newModelId"]
+        if deployment_info.new_model_id:
+            content["new_model_id"] = deployment_info.new_model_id
         return content
 
     def plugin_start(self):
         self._logger.info("Plugin start for Test plugin- nothing to do")
         self._raise_exception_if_set()
         time.sleep(self._plugin_start_time)
         self._logger.info("Done plugin start for Test plugin")
@@ -107,80 +108,80 @@
         time.sleep(self._plugin_stop_time)
         self._logger.info("Done plugin stop for Test plugin")
         pe_file = self._get_pe_filename()
         if os.path.exists(pe_file):
             os.remove(pe_file)
         return ActionStatusInfo(ActionStatus.OK)
 
-    def deployment_start(self, deployment_info):
+    def deployment_start(self, di: DeploymentInfo):
         """
         Add a cron job per deployment
         :return:
         """
         self._logger.info("start deployment_launch")
         self._raise_exception_if_set()
         time.sleep(self._launch_time_sec)
-        with open(self._get_deployment_filename(deployment_info), "w") as deployment_file:
-            content = self._get_deployment_content(deployment_info)
+        with open(self._get_deployment_filename(di), "w") as deployment_file:
+            content = self._get_deployment_content(di)
             deployment_file.write(yaml.safe_dump(content))
 
         self._logger.info("done  deployment_launch")
         return ActionStatusInfo(ActionStatus.OK, msg="Launch successful", state="ready")
 
-    def deployment_stop(self, deployment_data):
+    def deployment_stop(self, deployment_id: str):
         """
         Stop the cron job and delete it
         :return:
         """
         self._logger.info("start deployment_stop")
         self._raise_exception_if_set()
-        deployment_path = self._get_deployment_filename_from_id(deployment_data["id"])
+        deployment_path = self._get_deployment_filename_from_id(deployment_id)
         if os.path.exists(deployment_path):
             os.remove(deployment_path)
 
         time.sleep(self._stop_time_sec)
         self._logger.info("done  deployment_stop")
         return ActionStatusInfo(ActionStatus.OK, msg="Stop Successful", state="stopped")
 
-    def deployment_replace_model(self, deployment_info):
+    def deployment_replace_model(self, di: DeploymentInfo):
         """
         Will put a model artifact in a place the cronjob can consume it
         :param deployment_info: Info about the deployment
         :param model_artifact_path:
         :return:
         """
-        model_artifact_path = deployment_info["modelArtifact"]
-        self._logger.info("start replacing model: {}".format(model_artifact_path))
+        model_artifact_path = di.model_artifact
+        self._logger.info(f"start replacing model: {model_artifact_path}")
         time.sleep(self._replace_model_time)
-        deployment_path = self._get_deployment_filename(deployment_info)
+        deployment_path = self._get_deployment_filename(di)
         try:
             self._raise_exception_if_set()
             with open(deployment_path, "w") as deployment_file:
-                content = self._get_deployment_content(deployment_info)
+                content = self._get_deployment_content(di)
                 if "new_model_id" in content:
                     content["model_id"] = content["new_model_id"]
                 deployment_file.write(yaml.safe_dump(content))
         except Exception as ex:
             if os.path.exists(deployment_path):
-                with open(deployment_path, "r") as deployment_file:
+                with open(deployment_path) as deployment_file:
                     content = yaml.safe_load(deployment_file.read())
-                    if content["model_id"] != deployment_info["modelId"]:
+                    if content["model_id"] != di.model_id:
                         return ActionStatusInfo(
                             ActionStatus.ERROR,
                             msg="Failed to replace model, continuing with old one",
                             state=DeploymentState.ERROR,
                             data={ActionDataFields.OLD_MODEL_IN_USE: True},
                         )
                     else:
                         raise ex
 
-        self._logger.info("done  replacing model: {}".format(model_artifact_path))
+        self._logger.info(f"done  replacing model: {model_artifact_path}")
         return ActionStatusInfo(
             ActionStatus.OK,
-            msg="Model replaced successfully Path: {}".format(model_artifact_path),
+            msg=f"Model replaced successfully Path: {model_artifact_path}",
             state="ready",
         )
 
     def pe_status(self):
         """
         Do status check
         :return:
@@ -195,41 +196,40 @@
                 content["status_timestamp"] = datetime.datetime.utcnow().isoformat()
                 pe_file.seek(0)
                 pe_file.write(yaml.safe_dump(content))
                 pe_file.truncate()
 
             all_deployments_status = {}
 
+            assert self._pe_info is not None
             print(self._pe_info)
-            for deployment in self._pe_info.deployments:
-                di = DeploymentInfo(deployment)
-                self._logger.info("Checking status of deployment: {}".format(di.id))
+            for di in self._pe_info.deployments:
+                self._logger.info(f"Checking status of deployment: {di.id}")
                 deployment_status = self._deployment_status(di.id)
                 self._logger.info(deployment_status)
                 all_deployments_status[di.id] = deployment_status.to_dict()
             data = {ActionDataFields.DEPLOYMENTS_STATUS: all_deployments_status}
             action_status = ActionStatusInfo(
                 ActionStatus.OK, msg="PE Health looks awesome", data=data
             )
 
         else:
             action_status = ActionStatusInfo(ActionStatus.ERROR, msg="PE not found")
-        self._logger.info("done  pe_status: {}".format(action_status))
+        self._logger.info(f"done  pe_status: {action_status}")
         return action_status
 
-    def deployment_status(self, deployment_info):
+    def deployment_status(self, di: DeploymentInfo):
         """
         :param deployment_info: Info about the deployment to check
         Do status check
         :return:
         """
         self._logger.info("start deployment_status")
         self._raise_exception_if_set()
         time.sleep(self._deployment_status_time)
-        di = DeploymentInfo(deployment_info)
         return self._deployment_status(di.id)
 
     def _deployment_status(self, deployment_id):
         deployment_path = self._get_deployment_filename_from_id(deployment_id)
         if os.path.exists(deployment_path):
             with open(deployment_path, "r+") as deployment_file:
                 content = yaml.safe_load(deployment_file.read())
@@ -261,12 +261,12 @@
         current_deployment_files = glob.glob(
             os.path.join(self._plugin_tmp_dir, "deployment_*.yaml")
         )
 
         deployments_map = {}
         for file in current_deployment_files:
             deployment_id = os.path.basename(file).split("_")[1].split(".")[0]
-            with open(file, "r") as f:
+            with open(file) as f:
                 deployment_info = yaml.safe_load(f.read())
                 deployments_map[deployment_id] = deployment_info
 
         return ActionStatusInfo(ActionStatus.OK, msg="Deployment list", data=deployments_map)
```

## bosun/plugin/constants.py

```diff
@@ -74,7 +74,8 @@
         return model_suffix_for_format.get(model_format, "")
 
 
 class DeploymentState:
     READY = "ready"
     STOPPED = "stopped"
     ERROR = "errored"
+    LAUNCHING = "launching"
```

## bosun/plugin/deployment_info.py

```diff
@@ -8,32 +8,33 @@
 #  This file and its contents are subject to DataRobot Tool and Utility Agreement.
 #  For details, see
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
 #
 #  --------------------------------------------------------------------------------
 
 from pathlib import Path
+from typing import Any
+from typing import Dict
+from typing import Optional as Nullable
 
 import yaml
 from schema import And
 from schema import Optional
 from schema import Or
 from schema import Schema
 from schema import Use
 
 
 class DeploymentInfo:
     """
     A wrapper for the deployment info dict (from the deployment info YAML)
     """
 
-    BASE_IMAGE_KEY = "baseImage"
-
     # TODO: the kev_value_config should be all optional and validated by the specific plugin
-    def __init__(self, deployment_info):
+    def __init__(self, deployment_info: Dict[str, Any]):
         schema = Schema(
             {
                 "id": And(str, len),
                 "modelId": And(str, len),
                 "modelExecutionType": And(str, len),
                 Optional("keyValueConfig", default={}): dict,
                 Optional("name"): str,
@@ -44,56 +45,59 @@
                 Optional("isPredictionExplanationsSupported"): Or(None, bool),
             },
             ignore_extra_keys=True,
         )
 
         self._deployment_info = schema.validate(deployment_info)
 
-    def to_yaml(self):
+    def to_dict(self) -> Dict[str, Any]:
         tmp = self._deployment_info.copy()
         if "modelArtifact" in tmp:
             # convert Path to str if present in the data
             tmp["modelArtifact"] = str(tmp["modelArtifact"])
-        return yaml.safe_dump(tmp, indent=4)
+        return tmp
+
+    def to_yaml(self) -> str:
+        return yaml.safe_dump(self.to_dict(), indent=4)
 
     def __str__(self):
         return self.to_yaml()
 
     @property
-    def id(self):
+    def id(self) -> str:
         return self._deployment_info["id"]
 
     @property
-    def name(self):
+    def name(self) -> Nullable[str]:
         return self._deployment_info.get("name")
 
     @property
-    def description(self):
+    def description(self) -> Nullable[str]:
         return self._deployment_info.get("description")
 
     @property
-    def model_id(self):
+    def model_id(self) -> str:
         return self._deployment_info["modelId"]
 
     @property
-    def model_artifact(self):
+    def model_artifact(self) -> Nullable[Path]:
         return self._deployment_info.get("modelArtifact")
 
     @property
-    def model_format(self):
+    def model_format(self) -> Nullable[str]:
         return self._deployment_info.get("modelFormat")
 
     @property
-    def model_execution_type(self):
+    def model_execution_type(self) -> str:
         return self._deployment_info["modelExecutionType"]
 
     @property
-    def kv_config(self):
+    def kv_config(self) -> Dict[str, Any]:
         return self._deployment_info["keyValueConfig"]
 
     @property
-    def new_model_id(self):
+    def new_model_id(self) -> Nullable[str]:
         return self._deployment_info.get("newModelId")
 
     @property
-    def is_prediction_explanations_supported(self):
-        return self._deployment_info.get("isPredictionExplanationsSupported")
+    def is_prediction_explanations_supported(self) -> bool:
+        return self._deployment_info.get("isPredictionExplanationsSupported", False)
```

## bosun/plugin/pe_info.py

```diff
@@ -7,70 +7,78 @@
 #
 #  This file and its contents are subject to DataRobot Tool and Utility Agreement.
 #  For details, see
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
 #
 #  --------------------------------------------------------------------------------
 
+from datetime import datetime
+from typing import Any
+from typing import Dict
+from typing import List
+from typing import Optional as Nullable
+
 import dateutil.parser
 import yaml
 from schema import And
 from schema import Optional
 from schema import Or
 from schema import Schema
 from schema import Use
 
+from bosun.plugin.deployment_info import DeploymentInfo
+
 
 class PEInfo:
     """
     A wrapper for the PE info dict (from the PE info YAML)
     """
 
-    def __init__(self, pe_info):
+    def __init__(self, pe_info: Dict[str, Any]):
         schema = Schema(
             {
-                Optional("name"): str,
                 "id": And(str, len),
+                Optional("name"): Or(None, str),
                 Optional("description"): Or(None, str),
                 Optional("createdOn"): Or(None, Use(dateutil.parser.isoparse)),
                 Optional("createdBy"): Or(None, str),
-                Optional("deployments"): list,
-                Optional("keyValueConfig"): dict,
+                Optional("deployments", default=[]): list,
+                Optional("keyValueConfig", default={}): dict,
             },
             ignore_extra_keys=True,
         )
 
         self._pe_info = schema.validate(pe_info)
 
     def to_yaml(self):
         return yaml.safe_dump(self._pe_info, indent=4)
 
     def __str__(self):
         return self.to_yaml()
 
     @property
-    def id(self):
+    def id(self) -> str:
         return self._pe_info["id"]
 
     @property
-    def name(self):
+    def name(self) -> Nullable[str]:
         return self._pe_info.get("name")
 
     @property
-    def description(self):
+    def description(self) -> Nullable[str]:
         return self._pe_info.get("description")
 
     @property
-    def deployments(self):
-        return self._pe_info.get("deployments")
+    def deployments(self) -> List[DeploymentInfo]:
+        return [DeploymentInfo(d) for d in self._pe_info["deployments"]]
 
     @property
-    def created_on(self):
+    def created_on(self) -> Nullable[datetime]:
         return self._pe_info.get("createdOn")
 
     @property
-    def created_by(self):
+    def created_by(self) -> Nullable[str]:
         return self._pe_info.get("createdBy")
 
     @property
-    def kv_config(self):
-        return self._deployment_info.get("keyValueConfig")
+    def kv_config(self) -> Dict[str, Any]:
+        return self._pe_info["keyValueConfig"]
```

## bosun/plugin/plugin_runner.py

```diff
@@ -9,32 +9,26 @@
 #  For details, see
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
 #
 #  --------------------------------------------------------------------------------
 
 import argparse
 import importlib
+import importlib.resources as pkg_resources
 import inspect
 import logging
 import logging.config
 import os
 import pprint
 import signal
 import sys
 import textwrap
-from collections import OrderedDict
 
 import yaml
 
-try:
-    import importlib.resources as pkg_resources
-except ImportError:
-    # Try backported to PY<37 `importlib_resources`.
-    import importlib_resources as pkg_resources
-
 from bosun.plugin.action_status import ActionStatus
 from bosun.plugin.action_status import ActionStatusInfo
 from bosun.plugin.bosun_plugin_base import BosunPluginBase
 from bosun.plugin.constants import BosunPluginActions
 from bosun.plugin.constants import BosunPluginConfigConstants
 from bosun.plugin.constants import DeploymentInfoConfigConstants
 from bosun.plugin.constants import PeInfoConfigConstants
@@ -67,59 +61,49 @@
         If your plugin was installed as a python module (using pip), you can provide the name
         of the module that contains the plugin class. For example --plugin sample_plugin.my_plugin
 
         If your plugin is in a directory, you can provide the name of the plugin as the path to the
         file that contains your plugin class. For example:  --plugin sample_plugin/my_plugin.py
     """
 
-    builtin_plugins = OrderedDict(
-        [
-            ("test", {"module": "bosun.plugin.bosun_test_plugin", "names": ["test"]}),
-            (
-                "filesystem",
-                {
-                    "module": "bosun.plugin.filesystem.filesystem_plugin",
-                    "names": ["filesystem_plugin", "filesystem"],
-                },
-            ),
-            (
-                "docker",
-                {
-                    "module": "bosun.plugin.docker.docker_plugin",
-                    "names": ["docker-plugin", "docker"],
-                },
-            ),
-            ("s3", {"module": "bosun.plugin.s3.s3_plugin", "names": ["s3_plugin", "s3"]}),
-            (
-                "k8s",
-                {
-                    "module": "bosun.plugin.k8s.kubernetes_plugin",
-                    "names": ["k8s-plugin", "k8s", "kubernetes"],
-                },
-            ),
-            (
-                "snowflake",
-                {
-                    "module": "bosun.plugin.snowflake.snowflake_plugin",
-                    "names": ["snowflake_plugin", "snowflake"],
-                },
-            ),
-        ]
-    )
-
-    def __init__(self, plugin, config_file, private_config_file, action, status_file, dry_run):
+    builtin_plugins = {
+        "test": {"module": "bosun.plugin.bosun_test_plugin", "names": ["test"]},
+        "filesystem": {
+            "module": "bosun.plugin.filesystem.filesystem_plugin",
+            "names": ["filesystem_plugin", "filesystem"],
+        },
+        "docker": {
+            "module": "bosun.plugin.docker.docker_plugin",
+            "names": ["docker-plugin", "docker"],
+        },
+        "s3": {"module": "bosun.plugin.s3.s3_plugin", "names": ["s3_plugin", "s3"]},
+        "k8s": {
+            "module": "bosun.plugin.k8s.kubernetes_plugin",
+            "names": ["k8s-plugin", "k8s", "kubernetes"],
+        },
+        "snowflake": {
+            "module": "bosun.plugin.snowflake.snowflake_plugin",
+            "names": ["snowflake_plugin", "snowflake"],
+        },
+        "azureml": {
+            "module": "bosun.plugin.azureml.azureml_plugin",
+            "names": ["azureml_plugin", "azureml"],
+        },
+    }
+
+    def __init__(
+        self, plugin, config_file, action, private_config_file=None, status_file=None, dry_run=False
+    ):
         self._plugin = plugin
         self._config_file = config_file
         self._private_config_file = private_config_file
         self._action = action
         self._status_file = status_file
         self._dry_run = dry_run
-        self._logger = logging.getLogger(
-            "{}.{}".format(self.__class__.__module__, self.__class__.__name__)
-        )
+        self._logger = logging.getLogger(f"{self.__class__.__module__}.{self.__class__.__name__}")
 
     @staticmethod
     def parse_args():
         parser = argparse.ArgumentParser(
             formatter_class=argparse.RawDescriptionHelpFormatter,
             description=textwrap.dedent(PluginRunner.description),
         )
@@ -255,30 +239,30 @@
     def _load_plugin_from_file(self, plugin_file_path):
 
         plugin_file_path = os.path.splitext(plugin_file_path)[0]
         module_dir = os.path.dirname(plugin_file_path)
         orig_module_name = plugin_file_path
         module_name = os.path.basename(plugin_file_path)
 
-        self._logger.debug("Trying to load plugin from directory: {}".format(module_dir))
+        self._logger.debug(f"Trying to load plugin from directory: {module_dir}")
         if len(module_dir) > 0:
             sys.path.insert(0, module_dir)
             self._logger.debug(
                 "Added {} to path. Trying to import {}".format(
                     module_dir, os.path.basename(module_name)
                 )
             )
             plugin_module = importlib.import_module(module_name)
             self._logger.debug("Module successfully loaded")
             return plugin_module, module_name
         else:
-            self._logger.error("Failed to load module: {}".format(orig_module_name))
+            self._logger.error(f"Failed to load module: {orig_module_name}")
 
             self._logger.error(
-                "And no directory structure was detected in module name {}".format(orig_module_name)
+                f"And no directory structure was detected in module name {orig_module_name}"
             )
             sys.exit(1)
 
     def load_plugin_object(self, module_name, plugin_config, private_config_file, pe_info):
         try:
             plugin_module = importlib.import_module(module_name)
             self._logger.debug("Plugin was loaded using import statement")
@@ -287,31 +271,29 @@
                 raise
             plugin_module, module_name = self._load_plugin_from_file(module_name)
 
         possible_plugins = []
         for name, obj in inspect.getmembers(plugin_module):
             self._logger.debug(name)
             if inspect.isclass(obj):
-                self._logger.debug("Class: {}  module: {}".format(obj, obj.__module__))
+                self._logger.debug(f"Class: {obj}  module: {obj.__module__}")
                 if issubclass(obj, BosunPluginBase) and obj.__module__ == module_name:
-                    self._logger.debug("Plugin class: {}".format(obj))
+                    self._logger.debug(f"Plugin class: {obj}")
                     possible_plugins.append(obj)
         if len(possible_plugins) == 0:
-            raise Exception(
-                "No plugin implementation was detected in module: {}".format(module_name)
-            )
+            raise Exception(f"No plugin implementation was detected in module: {module_name}")
 
         if len(possible_plugins) > 1:
             raise Exception(
-                "Too many implementations of bosun plugin detected: {}".format(possible_plugins)
+                f"Too many implementations of bosun plugin detected: {possible_plugins}"
             )
 
         return possible_plugins[0](plugin_config, private_config_file, pe_info, self._dry_run)
 
-    def run(self):
+    def run(self) -> ActionStatusInfo:
 
         logger = logging.getLogger("main")
 
         require_deployment_info = (
             True if self._action in BosunPluginActions.require_deployment_info() else False
         )
         plugin_config, pe_info, deployment_info = self.get_configs(
@@ -327,17 +309,17 @@
             msg = "Exception occurred while loading plugin object for action {}: error {}".format(
                 self._action, e
             )
             logger.exception(msg)
             action_status = ActionStatusInfo(ActionStatus.ERROR, msg=msg, state="errored")
 
             action_status.write_to_file(status_file=self._status_file)
-            return
+            return action_status
 
-        pbe.run_action(self._action, deployment_info, status_file=self._status_file)
+        return pbe.run_action(self._action, deployment_info, status_file=self._status_file)
 
 
 action_to_config = {
     BosunPluginActions.PLUGIN_START: "plugin_start_config.yaml",
     BosunPluginActions.PLUGIN_STOP: "plugin_stop_config.yaml",
     BosunPluginActions.PE_STATUS: "pe_status_config.yaml",
     BosunPluginActions.DEPLOYMENT_START: "deployment_start_config.yaml",
@@ -350,31 +332,31 @@
 
 def gen_config_sample(config_file, action):
     of = sys.stdout
     if config_file != "-":
         of = open(config_file, "w")
 
     if action not in action_to_config:
-        print("Unable to generate a sample config file for action: {}".format(action))
+        print(f"Unable to generate a sample config file for action: {action}")
         raise SystemExit(1)
 
     print("# The following is an example of plugin configuration file", file=of)
-    print("# for action: {}".format(action), file=of)
+    print(f"# for action: {action}", file=of)
     print("#----------------------------------------------------------", file=of)
     print("", file=of)
 
     from . import config_samples  # relative-import the *package* containing the templates
 
     sample_content = pkg_resources.read_text(config_samples, action_to_config[action])
     print(textwrap.dedent(sample_content), file=of)
 
 
 def set_logging(options):
     if options.log_config:
-        with open(options.log_config, "r") as f:
+        with open(options.log_config) as f:
             config = yaml.safe_load(f.read())
             logging.config.dictConfig(config)
     else:
         logging.root.setLevel(options.log_level)
         if options.logfile:
             handler = logging.FileHandler(options.logfile)
         else:
```

## bosun/plugin/docker/docker_helper.py

```diff
@@ -17,14 +17,15 @@
 import tempfile
 import time
 import zipfile
 from contextlib import suppress
 from pathlib import Path
 
 import requests
+
 from bosun.model_connector.constants import ModelPackageConstants
 
 
 class DockerLabels:
     MLOPS_LABEL = "mlops"
     AGENT_LABEL = "mlops.agent"
     RABBITMQ_LABEL = "mlops.rabbitmq"
@@ -59,21 +60,19 @@
 class DockerHelper:
     # Need to use /tmp for now because it is the easiest way so we can run both natively on the host
     # OS and also in a docker container (with /tmp from the host OS mounted in).
     MODEL_ARCHIVE_DIR = Path("/tmp/bosun-docker_plugin-model_archives")
 
     def __init__(self, docker_client, config):
         self._client = docker_client
-        self._logger = logging.getLogger(
-            "{}.{}".format(self.__class__.__module__, self.__class__.__name__)
-        )
+        self._logger = logging.getLogger(f"{self.__class__.__module__}.{self.__class__.__name__}")
         self._config = config
 
     def _container_name(self, deployment_id, model_id):
-        return "{}{}_{}".format(self._config.container_name_prefix, deployment_id, model_id)
+        return f"{self._config.container_name_prefix}{deployment_id}_{model_id}"
 
     def get_running_deployment_containers(self, deployment_id=None, force_one=False, model_id=None):
         container_list = self._client.containers.list()
         cm_containers = []
         for c in container_list:
             found = False
             if DockerLabels.DEPLOYMENT_ID_LABEL in c.labels:
@@ -117,38 +116,38 @@
             port_str = internal_port + "/tcp"
             if port == port_str:
                 host_port = container.ports[port][0]["HostPort"]
                 return host_port
         return None
 
     def stop_container(self, container, remove=False):
-        self._logger.info("Stopping container: {}".format(container.name))
+        self._logger.info(f"Stopping container: {container.name}")
         container.stop()
         if remove:
-            self._logger.info("Removing container: {}".format(container.name))
+            self._logger.info(f"Removing container: {container.name}")
             container.remove()
             self.remove_model_archive(container.name)
 
     def save_model_archive(self, archive_path, container_name):
         # Saves the model archive to a location we control so we can maintain the lifecycle of
         # th file based on the lifecycle of the deployment.
         self.MODEL_ARCHIVE_DIR.mkdir(parents=True, exist_ok=True)
-        dest = self.MODEL_ARCHIVE_DIR / "{}.mlpkg".format(container_name)
+        dest = self.MODEL_ARCHIVE_DIR / f"{container_name}.mlpkg"
         with suppress(shutil.SameFileError):
             shutil.copyfile(archive_path, dest)
         # Make sure to give read access to everyone since we share the file between containers
         # that can be running as completely different users (i.e. root and datarobot-service).
         dest.chmod(0o644)
         return dest
 
     def remove_model_archive(self, container_name):
         # Model replacements in DR result in new containers so it should be safe to remove the
         # .mlpkg file finally when this occurs.
         with suppress(FileNotFoundError):
-            pkg_name = "{}.mlpkg".format(container_name)
+            pkg_name = f"{container_name}.mlpkg"
             (self.MODEL_ARCHIVE_DIR / pkg_name).unlink()
 
     @staticmethod
     def _container_labels(
         container_name,
         deployment_id,
         deployment_predict_path,
@@ -159,19 +158,19 @@
         container_predict_path,
         container_ping_path="/ping",
     ):
         # The rule that send the request with the specific deployment id to this container
         predict_router = container_name + "_predict"
         ping_router = container_name + "_ping"
 
-        predict_router_rule_label = "traefik.http.routers.{}.rule".format(predict_router)
-        predict_router_rule_label_value = "Path(`{}`)".format(deployment_predict_path)
+        predict_router_rule_label = f"traefik.http.routers.{predict_router}.rule"
+        predict_router_rule_label_value = f"Path(`{deployment_predict_path}`)"
 
-        ping_router_rule_label = "traefik.http.routers.{}.rule".format(ping_router)
-        ping_router_rule_label_value = "Path(`{}`)".format(deployment_ping_path)
+        ping_router_rule_label = f"traefik.http.routers.{ping_router}.rule"
+        ping_router_rule_label_value = f"Path(`{deployment_ping_path}`)"
 
         predict_middleware = container_name + "_predict"
         ping_middleware = container_name + "_ping"
 
         predict_middleware_label = "traefik.http.middlewares.{}.replacepath.path".format(
             predict_middleware
         )
@@ -182,22 +181,22 @@
         )
         ping_middleware_value = container_ping_path
 
         # Attaching the middleware to the router (which has the rule)
         predict_router_middleware_label = "traefik.http.routers.{}.middlewares".format(
             predict_router
         )
-        predict_router_middleware_label_value = "{}@docker".format(predict_middleware)
+        predict_router_middleware_label_value = f"{predict_middleware}@docker"
 
-        ping_router_middleware_label = "traefik.http.routers.{}.middlewares".format(ping_router)
-        ping_router_middleware_label_value = "{}@docker".format(ping_middleware)
+        ping_router_middleware_label = f"traefik.http.routers.{ping_router}.middlewares"
+        ping_router_middleware_label_value = f"{ping_middleware}@docker"
 
         return {
             DockerLabels.MLOPS_LABEL: None,
-            DockerLabels.PREDICTION_PORT: "{}".format(host_port),
+            DockerLabels.PREDICTION_PORT: f"{host_port}",
             DockerLabels.DEPLOYMENT_ID_LABEL: deployment_id,
             DockerLabels.MODEL_ID_LABEL: model_id,
             DockerLabels.MODEL_EXECUTION_TYPE_LABEL: model_execution_type,
             predict_router_rule_label: predict_router_rule_label_value,
             predict_middleware_label: predict_middleware_value,
             predict_router_middleware_label: predict_router_middleware_label_value,
             ping_router_rule_label: ping_router_rule_label_value,
@@ -206,41 +205,39 @@
         }
 
 
 class CMDockerHelper(DockerHelper):
     CM_SERVER_INTERNAL_PORT = "6788"
 
     def __init__(self, docker_client, config):
-        super(CMDockerHelper, self).__init__(docker_client, config)
+        super().__init__(docker_client, config)
 
     def ping_prediction_server(self, deployment_id, container, count=10, sleep_time=1):
         if self.running_in_container:
-            url = "http://{}:{}/".format(container.name, self.CM_SERVER_INTERNAL_PORT)
+            url = f"http://{container.name}:{self.CM_SERVER_INTERNAL_PORT}/"
         else:
             host_port = self.find_port(container, self.CM_SERVER_INTERNAL_PORT)
             if not host_port:
-                raise Exception(
-                    "Could not find container host port (deployment: {})".format(deployment_id)
-                )
-
-            self._logger.debug("Found server port, host port: {}".format(host_port))
-            url = "http://0.0.0.0:{}/".format(host_port)
-        self._logger.info("Checking deployment: {} status, url: {}".format(deployment_id, url))
+                raise Exception(f"Could not find container host port (deployment: {deployment_id})")
+
+            self._logger.debug(f"Found server port, host port: {host_port}")
+            url = f"http://0.0.0.0:{host_port}/"
+        self._logger.info(f"Checking deployment: {deployment_id} status, url: {url}")
         last_error = None
         for ii in range(0, count):
             try:
                 res = requests.get(url)
                 if res.status_code == 200:
                     return True, ""
                 else:
-                    last_error = "request status: {}".format(res.status_code)
+                    last_error = f"request status: {res.status_code}"
             except Exception as e:
                 self._logger.info("Failed sending request... will try again")
                 last_error = e
-            self._logger.info("ping: count {} going to sleep".format(ii))
+            self._logger.info(f"ping: count {ii} going to sleep")
             time.sleep(sleep_time)
 
         raise Exception(
             "Could not ping cm server deployment_id: {} : error {}".format(
                 deployment_id, last_error
             )
         )
@@ -248,25 +245,25 @@
     def build_cm_container(self, di):
         with tempfile.TemporaryDirectory() as tmp_dir:
             with zipfile.ZipFile(di.model_artifact, "r") as zip_ref:
                 zip_ref.extractall(tmp_dir)
 
             installer = os.path.join(tmp_dir, "cm_pps_installer.sh")
             if not os.path.exists(installer):
-                raise Exception("Missing custom model installer: {}".format(installer))
+                raise Exception(f"Missing custom model installer: {installer}")
 
             # Build docker image
             cmd = ["bash", installer, "--skip-agent-install"]
             build_process = subprocess.Popen(cmd, cwd=tmp_dir, stdout=subprocess.PIPE)
             exit_code = build_process.wait()
-            self._logger.info("Building docker image complete with exit code: {}".format(exit_code))
+            self._logger.info(f"Building docker image complete with exit code: {exit_code}")
 
-        image_tag = "cm_pps_{}".format(di.model_id)
+        image_tag = f"cm_pps_{di.model_id}"
         if not self._client.images.list(name=image_tag):
-            raise Exception("Image {} was not created successfully".format(image_tag))
+            raise Exception(f"Image {image_tag} was not created successfully")
 
         return image_tag
 
     def run_cm_container(
         self,
         image_tag,
         host_port,
@@ -284,17 +281,17 @@
             deployment_predict_path,
             deployment_ping_path,
             model_id,
             ModelPackageConstants.MODEL_EXECUTION_CUSTOM_INFERENCE,
             host_port,
             "/predict/",
         )
-        ports = {"{}/tcp".format(self.CM_SERVER_INTERNAL_PORT): host_port}
+        ports = {f"{self.CM_SERVER_INTERNAL_PORT}/tcp": host_port}
         env = {
-            "ADDRESS": "0.0.0.0:{}".format(self.CM_SERVER_INTERNAL_PORT),
+            "ADDRESS": f"0.0.0.0:{self.CM_SERVER_INTERNAL_PORT}",
             "MODEL_ID": model_id,
             "DEPLOYMENT_ID": deployment_id,
             "MONITOR": str(self._config.do_mlops_monitoring),
             "MONITOR_SETTINGS": monitor_settings,
         }
         self._client.containers.run(
             image_tag,
@@ -307,15 +304,15 @@
         )
 
 
 class PPSDockerHelper(DockerHelper):
     SERVER_INTERNAL_PORT = "8080"
 
     def __init__(self, docker_client, base_image, config):
-        super(PPSDockerHelper, self).__init__(docker_client, config)
+        super().__init__(docker_client, config)
         self._base_image = base_image
 
     def run_pps_container(
         self,
         deployment_id,
         model_id,
         model_artifact,
@@ -344,15 +341,15 @@
             "PREDICTION_API_MONITORING_ENABLED": str(self._config.do_mlops_monitoring),
             "MONITORING_AGENT": "False",
             "PREDICTION_API_MONITORING_SETTINGS": monitor_settings,
             "PORTABLE_PREDICTION_API_MONITORING_SETTINGS": monitor_settings,
             "MLOPS_DEPLOYMENT_ID": deployment_id,
             "MLOPS_MODEL_ID": model_id,
         }
-        ports = {"{}/tcp".format(self.SERVER_INTERNAL_PORT): "0"}
+        ports = {f"{self.SERVER_INTERNAL_PORT}/tcp": "0"}
 
         volumes = {
             str(persisted_archive_path.absolute()): {"bind": str(pps_artifact_path), "mode": "ro"}
         }
 
         self._client.containers.run(
             self._base_image,
@@ -363,37 +360,35 @@
             labels=labels,
             volumes=volumes,
             network=self._config.docker_network,
         )
 
     def ping_prediction_server(self, deployment_id, container, count=60, sleep_time=1):
         if self.running_in_container:
-            url = "http://{}:{}/ping".format(container.name, self.SERVER_INTERNAL_PORT)
+            url = f"http://{container.name}:{self.SERVER_INTERNAL_PORT}/ping"
         else:
             host_port = self.find_port(container, self.SERVER_INTERNAL_PORT)
             if not host_port:
-                raise Exception(
-                    "Could not find container host port (deployment: {})".format(deployment_id)
-                )
-
-            self._logger.debug("Found server port, host port: {}".format(host_port))
-            url = "http://0.0.0.0:{}/ping".format(host_port)
-        self._logger.info("Checking deployment: {} status, url: {}".format(deployment_id, url))
+                raise Exception(f"Could not find container host port (deployment: {deployment_id})")
+
+            self._logger.debug(f"Found server port, host port: {host_port}")
+            url = f"http://0.0.0.0:{host_port}/ping"
+        self._logger.info(f"Checking deployment: {deployment_id} status, url: {url}")
         last_error = None
         for ii in range(0, count):
             try:
                 res = requests.get(url)
                 if res.status_code == 200:
                     return True, ""
                 else:
-                    last_error = "request status: {}".format(res.status_code)
+                    last_error = f"request status: {res.status_code}"
             except Exception as e:
                 self._logger.info("Failed sending request... will try again")
                 last_error = e
-            self._logger.info("ping: count {} going to sleep".format(ii))
+            self._logger.info(f"ping: count {ii} going to sleep")
             time.sleep(sleep_time)
 
         raise Exception(
             "Could not ping pps server deployment_id: {} : error {}".format(
                 deployment_id, last_error
             )
         )
```

## bosun/plugin/docker/docker_plugin.py

```diff
@@ -13,14 +13,15 @@
 import logging
 import pprint
 import time
 import traceback
 
 import docker
 import yaml
+
 from bosun.model_connector.constants import ModelPackageConstants
 from bosun.plugin.action_status import ActionDataFields
 from bosun.plugin.action_status import ActionStatus
 from bosun.plugin.action_status import ActionStatusInfo
 from bosun.plugin.bosun_plugin_base import BosunPluginBase
 from bosun.plugin.constants import DeploymentState
 from bosun.plugin.deployment_info import DeploymentInfo
@@ -69,34 +70,34 @@
     def _monitor_settings(self):
         return "spooler_type=rabbitmq;rabbitmq_queue_url={};rabbitmq_queue_name={}".format(
             self._rabbitmq_queue_url, self._rabbitmq_queue_name
         )
 
     @staticmethod
     def _deployment_base_path(di):
-        return "/deployments/{}".format(di.id)
+        return f"/deployments/{di.id}"
 
     @staticmethod
     def _deployment_predict_path(di):
-        return "{}/predictions".format(DockerPlugin._deployment_base_path(di))
+        return f"{DockerPlugin._deployment_base_path(di)}/predictions"
 
     @staticmethod
     def _deployment_ping_path(di):
-        return "{}/ping".format(DockerPlugin._deployment_base_path(di))
+        return f"{DockerPlugin._deployment_base_path(di)}/ping"
 
     def _read_config_file(self):
         """
         Reading the plugin specific config file is such is provided. And overriding this plugin
         configuration
         :return:
         """
         if not self._private_config_file:
             return
 
-        self._logger.info("Docker plugin private config file: {}".format(self._private_config_file))
+        self._logger.info(f"Docker plugin private config file: {self._private_config_file}")
         with open(self._private_config_file) as conf_file:
             config = yaml.safe_load(conf_file)
         self._logger.info(config)
         self._plugin_config.update(config)
         if self._logger.isEnabledFor(logging.DEBUG):
             self._logger.debug(self.get_sanitized_config(self._plugin_config))
 
@@ -114,15 +115,15 @@
         self.clean_stopped_reverse_proxy_container_if_any()
         self._logger.info("Starting reverse proxy container")
 
         if self._config.traefik_port_mapping:
             ports = {str(k): str(v) for k, v in self._config.traefik_port_mapping.items()}
         else:
             ports = {"80": "80", "8080": "8080"}
-        self._logger.info("Reverse proxy port mapping: '{}'".format(ports))
+        self._logger.info(f"Reverse proxy port mapping: '{ports}'")
         labels = {DockerLabels.REVERSE_PROXY_LABEL: "reverse_proxy", DockerLabels.MLOPS_LABEL: None}
         volumes = {"/var/run/docker.sock": {"bind": "/var/run/docker.sock", "mode": "ro"}}
 
         if self._is_reverse_proxy_running():
             self._logger.info("Reverse Proxy container is already running skipping")
             return
 
@@ -170,23 +171,23 @@
         return ActionStatusInfo(ActionStatus.OK)
 
     def plugin_stop(self):
         self._logger.info("Docker plugin stop called")
         cm_helper = DockerHelper(self._client, self._config)
         container_list = cm_helper.get_running_deployment_containers()
         for c in container_list:
-            self._logger.info("Container {} is still running".format(c))
+            self._logger.info(f"Container {c} is still running")
 
         # Taking down the MLOps monitoring containers.
         if self._config.do_mlops_monitoring:
             self._mlops_helper.stop()
         self._stop_reverse_proxy()
         return ActionStatusInfo(ActionStatus.OK)
 
-    def _deploy_cm_model(self, di):
+    def _deploy_cm_model(self, di: DeploymentInfo):
         port = int(di.kv_config.get("port", "0"))
         model_id = di.new_model_id if di.new_model_id is not None else di.model_id
         cm_helper = CMDockerHelper(self._client, self._config)
         image_tag = cm_helper.build_cm_container(di)
 
         cm_helper.run_cm_container(
             image_tag=image_tag,
@@ -209,15 +210,15 @@
         cm_helper.ping_prediction_server(di.id, container)
 
         msg = "Deployment {} launched, image tag: {} container id {}".format(
             di.id, image_tag, container.id
         )
         return msg
 
-    def _deploy_dr_model(self, di):
+    def _deploy_dr_model(self, di: DeploymentInfo):
         base_image = di.kv_config.get(DeploymentInfo.BASE_IMAGE_KEY, self._config.pps_base_image)
         pps_helper = PPSDockerHelper(self._client, base_image, self._config)
         model_id = di.new_model_id if di.new_model_id is not None else di.model_id
         pps_helper.run_pps_container(
             deployment_id=di.id,
             model_id=model_id,
             model_artifact=di.model_artifact,
@@ -236,30 +237,30 @@
         pps_helper.ping_prediction_server(di.id, container)
 
         msg = "Deployment {} launched, image tag: {} container id {}".format(
             di.id, self._config.pps_base_image, container.id
         )
         return msg
 
-    def _deploy_model(self, di):
+    def _deploy_model(self, di: DeploymentInfo):
         # According to the model type we decide how to run the container
         # We have 2 options - DataRobot models using PPS and User Models using DRUM
         if di.model_execution_type == ModelPackageConstants.MODEL_EXECUTION_DEDICATED:
             self._logger.info("Got a DataRobot Native model to deploy")
             msg = self._deploy_dr_model(di)
         elif di.model_execution_type == ModelPackageConstants.MODEL_EXECUTION_CUSTOM_INFERENCE:
             self._logger.info("Got a User Custom Inference model to deploy")
             msg = self._deploy_cm_model(di)
         else:
             raise Exception(
-                "This plugin does not support model of type: {}".format(di.model_execution_type)
+                f"This plugin does not support model of type: {di.model_execution_type}"
             )
         return msg
 
-    def _apply_deployment(self, di):
+    def _apply_deployment(self, di: DeploymentInfo):
         """
         Making sure the deployment is correctly applied. This means, taking down containers serving
         old models, and creating containers serving new models
         :param di:
         :return:
         """
         # Find existing containers
@@ -269,16 +270,16 @@
         containers_to_keep = []
         for container in containers:
             model_id = helper.get_model_id(container)
             if model_id == di.model_id and di.new_model_id is None:
                 containers_to_keep.append(container)
             else:
                 containers_to_stop.append(container)
-        self._logger.info("Containers to stop: {}".format(len(containers_to_stop)))
-        self._logger.info("Containers to keep: {}".format(len(containers_to_keep)))
+        self._logger.info(f"Containers to stop: {len(containers_to_stop)}")
+        self._logger.info(f"Containers to keep: {len(containers_to_keep)}")
 
         # Check if we need to deploy new containers, and if so deploy one
         if len(containers_to_keep) > 0:
             msg = "Not deploying any new container"
             self._logger.info(msg)
         else:
             if self._dry_run:
@@ -290,50 +291,47 @@
                     msg = self._deploy_model(di)
                 except Exception as ex:
                     raise DeploymentLaunchException(ex, "Failed to launch container")
 
         # Take down the original container(s)
         if len(containers_to_stop) > 0:
             for c in containers_to_stop:
-                m = "Stopping container: {}".format(c.name)
+                m = f"Stopping container: {c.name}"
                 if self._dry_run:
                     self._logger.info("DRYRUN: " + m)
                 else:
                     self._logger.info(m)
                     try:
                         helper.stop_container(c, remove=True)
                     except Exception as ex:
                         raise DeploymentStopException(ex, "Failed to stop container")
 
         return msg
 
-    def deployment_start(self, deployment_info):
+    def deployment_start(self, di: DeploymentInfo):
         """
         Add a cron job per deployment
         :return:
         """
-        di = DeploymentInfo(deployment_info)
-        self._logger.info("Launching deployment {}".format(di.id))
+        self._logger.info(f"Launching deployment {di.id}")
 
         msg = self._apply_deployment(di)
 
         prediction_url = (
             self._config.outfacing_prediction_url_prefix + self._deployment_predict_path(di)
         )
         data = {ActionDataFields.PREDICTION_URL: prediction_url}
         return ActionStatusInfo(ActionStatus.OK, msg, state=DeploymentState.READY, data=data)
 
-    def deployment_stop(self, deployment_data):
+    def deployment_stop(self, deployment_id: str):
         """
         Stop the cron job and delete it
         :return:
         """
         self._logger.info("Stopping cm container - this action will take down the model !!!")
-        deployment_id = deployment_data["id"]
-
         helper = DockerHelper(self._client, self._config)
         container_list = helper.get_running_deployment_containers(deployment_id=deployment_id)
         if len(container_list) == 0:
             status = ActionStatus.OK
             status_msg = "No container for deployment {} was found - skipping stop".format(
                 deployment_id
             )
@@ -351,25 +349,22 @@
             helper.stop_container(container_list[0], remove=True)
             status = ActionStatus.OK
             status_msg = "Container stopped"
 
         self._logger.info(status_msg)
         return ActionStatusInfo(status=status, msg=status_msg, state=DeploymentState.STOPPED)
 
-    def deployment_replace_model(self, deployment_info):
+    def deployment_replace_model(self, di: DeploymentInfo):
         """
         Will put a model artifact in a place the cronjob can consume it
         :param deployment_info: Info about the deployment
         :param model_artifact_path:
         :return:
         """
-        di = DeploymentInfo(deployment_info)
-        self._logger.info(
-            "-- Replacing model for deployment: {} dry_run: {}".format(di.id, self._dry_run)
-        )
+        self._logger.info(f"-- Replacing model for deployment: {di.id} dry_run: {self._dry_run}")
         try:
             msg = self._apply_deployment(di)
         except DeploymentLaunchException:
             # In case of launch failure, plugin did not stop the old container, so indicate
             # that in the status response
             msg = "Failed to replace model -\n{}\nContinuing with old model".format(
                 traceback.format_exc()
@@ -378,31 +373,32 @@
                 ActionStatus.ERROR,
                 msg=msg,
                 state=DeploymentState.ERROR,
                 data={ActionDataFields.OLD_MODEL_IN_USE: True},
             )
         return ActionStatusInfo(
             ActionStatus.OK,
-            msg="Model replaced successfully: {}".format(msg),
+            msg=f"Model replaced successfully: {msg}",
             state=DeploymentState.READY,
         )
 
     def pe_status(self):
         """
         Do status check
         :return:
         """
         self._logger.info("Getting status of docker environment")
+        assert self._pe_info is not None
         try:
             helper = DockerHelper(self._client, self._config)
             container_list = helper.get_running_deployment_containers()
-            status_msg = "Number of containers: {}".format(len(container_list))
+            status_msg = f"Number of containers: {len(container_list)}"
             status = ActionStatus.OK
         except Exception as e:
-            status_msg = "Error checking PE status: {}".format(e)
+            status_msg = f"Error checking PE status: {e}"
             status = ActionStatus.ERROR
 
         if self._config.do_mlops_monitoring:
             mlops_status = self._mlops_helper.status()
             if mlops_status is False and status == ActionStatus.OK:
                 status = ActionStatus.WARN
                 status_msg = "Error - mlops monitoring is not functioning properly"
@@ -410,63 +406,62 @@
         reverse_proxy_status = self._is_reverse_proxy_running()
         if reverse_proxy_status is False:
             status = ActionStatus.ERROR
             status_msg += "Reverse proxy is not running"
 
         pe_status = ActionStatusInfo(status=status, msg=status_msg)
         all_deployments_status = {}
-        for deployment in self._pe_info.deployments:
-            deployment_id = deployment["id"]
-            self._logger.info("Checking status for deployment: {}".format(deployment_id))
-            d_status = self.deployment_status(deployment)
+        for di in self._pe_info.deployments:
+            deployment_id = di.id
+            self._logger.info(f"Checking status for deployment: {deployment_id}")
+            d_status = self.deployment_status(di)
             all_deployments_status[deployment_id] = d_status.to_dict()
             self._logger.info(d_status.to_yaml())
         if bool(all_deployments_status):
             pe_status.data = {ActionDataFields.DEPLOYMENTS_STATUS: all_deployments_status}
-        self._logger.info("pe_status: {} {}".format(pe_status.status, pe_status.msg))
+        self._logger.info(f"pe_status: {pe_status.status} {pe_status.msg}")
         return pe_status
 
-    def deployment_status(self, deployment_info):
+    def deployment_status(self, di: DeploymentInfo):
         """
         :param deployment_info: Info about the deployment to check
         Do status check
         :return:
         """
         self._logger.info("Getting status for python batch deployment")
-        di = DeploymentInfo(deployment_info)
 
         # TODO: create a DockerHelperFactory
         if di.model_execution_type == ModelPackageConstants.MODEL_EXECUTION_DEDICATED:
             docker_helper = PPSDockerHelper(self._client, self._config.pps_base_image, self._config)
         elif di.model_execution_type == ModelPackageConstants.MODEL_EXECUTION_CUSTOM_INFERENCE:
             docker_helper = CMDockerHelper(self._client, self._config)
         else:
             raise Exception(
-                "This plugin does not support model of type: {}".format(di.model_execution_type)
+                f"This plugin does not support model of type: {di.model_execution_type}"
             )
 
         containers = docker_helper.get_running_deployment_containers(deployment_id=di.id)
 
         if len(containers) == 0:
             final_status = ActionStatusInfo(
                 ActionStatus.ERROR,
-                msg="Error: could not find a container for deployment {}".format(di.id),
+                msg=f"Error: could not find a container for deployment {di.id}",
                 state="errored",
             )
         elif len(containers) > 1:
             # In case of model replacement it is possible that more than 1 containers are
             # running for the same deployment.  As long as at least one container is in OK
             # state, we will return that status.  It is possible that model replacement may
             # fail, and that status will be captured in the subsequent status request
             found_one_good_container = False
             status_data = None
-            msg = "Found {} containers for deployment {} ".format(len(containers), di.id)
+            msg = f"Found {len(containers)} containers for deployment {di.id} "
             for index, container in enumerate(containers):
                 cont_status = self._get_deployment_status(docker_helper, di.id, container)
-                msg += " - Container {} id {}: {}".format(index, container.id, cont_status.msg)
+                msg += f" - Container {index} id {container.id}: {cont_status.msg}"
                 if cont_status.status == ActionStatus.OK:
                     found_one_good_container = True
                     status_data = cont_status.data
             if not found_one_good_container:
                 final_status = ActionStatusInfo(ActionStatus.ERROR, msg=msg, state="errored")
             else:
                 final_status = ActionStatusInfo(
@@ -479,15 +474,15 @@
 
     def _get_deployment_status(self, docker_helper, deployment_id, container):
         result = docker_helper.ping_prediction_server(
             deployment_id=deployment_id, container=container
         )
         if result:
             status = ActionStatus.OK
-            status_msg = "Deployment {} is doing well".format(deployment_id)
+            status_msg = f"Deployment {deployment_id} is doing well"
             state = "ready"
             current_model_id = container.labels[DockerLabels.MODEL_ID_LABEL]
             data = {ActionDataFields.CURRENT_MODEL_ID: current_model_id}
         else:
             status = ActionStatus.ERROR
             status_msg = "Could not ping prediction server"
             state = "errored"
@@ -496,18 +491,18 @@
         return ActionStatusInfo(status, msg=status_msg, state=state, data=data)
 
     def deployment_list(self):
         self._logger.info("Getting the list of running deployments")
         try:
             helper = DockerHelper(self._client, self._config)
             container_list = helper.get_running_deployment_containers()
-            status_msg = "Number of cm containers: {}".format(len(container_list))
+            status_msg = f"Number of cm containers: {len(container_list)}"
             status = ActionStatus.OK
         except Exception as e:
-            status_msg = "Error checking PE status: {}".format(e)
+            status_msg = f"Error checking PE status: {e}"
             status = ActionStatus.ERROR
             return ActionStatusInfo(status=status, msg=status_msg)
 
         if len(container_list) == 0:
             status_msg = "No containers running"
             self._logger.info(status_msg)
             return ActionStatusInfo(status, msg=status_msg)
@@ -529,15 +524,15 @@
                 docker_helper = PPSDockerHelper(
                     self._client, self._config.pps_base_image, self._config
                 )
             elif model_execution_type == ModelPackageConstants.MODEL_EXECUTION_CUSTOM_INFERENCE:
                 docker_helper = CMDockerHelper(self._client, self._config)
             else:
                 self._logger.warn(
-                    "This plugin does not support model of type: {}".format(model_execution_type)
+                    f"This plugin does not support model of type: {model_execution_type}"
                 )
                 continue
 
             deployments_map[deployment_id] = self._get_deployment_status(
                 docker_helper, deployment_id, deployment_container
             ).__dict__
```

## bosun/plugin/docker/docker_plugin_config.py

```diff
@@ -45,17 +45,17 @@
             DockerPluginConfig.GENERATED_IMAGE_PREFIX: str,
             DockerPluginConfig.CONTAINER_NAME_PREFIX: str,
             DockerPluginConfig.TRAEFIK_PORT_MAPPING: dict,
             DockerPluginConfig.RABBITMQ_PORT_MAPPING: dict,
         }
         for f in schema:
             if f not in self._config:
-                raise Exception("Field {} is missing in plugin config {}".format(f, self._config))
+                raise Exception(f"Field {f} is missing in plugin config {self._config}")
 
-            logger.debug("self._config[f]: {} {}".format(self._config[f], type(self._config[f])))
+            logger.debug(f"self._config[f]: {self._config[f]} {type(self._config[f])}")
             if type(self._config[f]) != schema[f]:
                 raise Exception(
                     "Field {} type: {} is not as expected: {}".format(
                         f, type(self._config[f]), schema[f]
                     )
                 )
             if f in [
```

## bosun/plugin/docker/mlops_monitoring.py

```diff
@@ -41,17 +41,15 @@
         self._rabbitmq_queue_url = rabbitmq_queue_url
         self._rabbitmq_queue_name = rabbitmq_queue_name
         self._datarobot_url = datarobot_url
         self._datarobot_api_token = datarobot_api_token
         self._docker_network = docker_network
         self._dry_run = dry_run
         self._nr_agents = 1
-        self._logger = logging.getLogger(
-            "{}.{}".format(self.__class__.__module__, self.__class__.__name__)
-        )
+        self._logger = logging.getLogger(f"{self.__class__.__module__}.{self.__class__.__name__}")
 
     def _get_running_agent_containers(self):
         return get_containers_with_label(self._client, label=DockerLabels.AGENT_LABEL)
 
     def _get_running_rabbit_containers(self):
         return get_containers_with_label(self._client, label=DockerLabels.RABBITMQ_LABEL)
 
@@ -67,15 +65,15 @@
         )
         return self._clean_stopped_containers(rabbit_containers, "rabbit")
 
     def _clean_stopped_containers(self, containers, name):
         if len(containers) == 0:
             return
         if containers[0].status == "exited":
-            self._logger.info("Removing stopped {} container".format(name))
+            self._logger.info(f"Removing stopped {name} container")
             containers[0].remove()
 
     def is_agent_running(self):
         cl = self._get_running_agent_containers()
         if len(cl) == 0:
             return False
         else:
@@ -94,15 +92,15 @@
             "RABBITMQ_DEFAULT_USER": parsed_url.username,
             "RABBITMQ_DEFAULT_PASS": parsed_url.password,
         }
         if rabbitmq_port_mapping:
             ports = {str(k): str(v) for k, v in rabbitmq_port_mapping.items()}
         else:
             ports = {"15672": "15672", "5672": "5672"}
-        self._logger.info("RabbitMQ port mapping: '{}'".format(ports))
+        self._logger.info(f"RabbitMQ port mapping: '{ports}'")
         labels = {DockerLabels.RABBITMQ_LABEL: "rabbit", DockerLabels.MLOPS_LABEL: None}
 
         if self._dry_run:
             self._logger.info("DRYRUN: running rabbit container")
         else:
             self._client.containers.run(
                 self._rabbitmq_image,
```

## bosun/plugin/filesystem/filesystem_plugin.py

```diff
@@ -12,38 +12,39 @@
 
 import glob
 import logging
 import os
 import shutil
 
 import yaml
+from schema import And
+from schema import Optional
+from schema import Schema
+from schema import Use
+
 from bosun.model_connector.constants import ModelPackageConstants
 from bosun.plugin.action_status import ActionDataFields
 from bosun.plugin.action_status import ActionStatus
 from bosun.plugin.action_status import ActionStatusInfo
 from bosun.plugin.bosun_plugin_base import BosunPluginBase
 from bosun.plugin.constants import BosunPluginConfigConstants
 from bosun.plugin.constants import DeploymentInfoConfigConstants
 from bosun.plugin.constants import DeploymentState
 from bosun.plugin.deployment_info import DeploymentInfo
-from schema import And
-from schema import Optional
-from schema import Schema
-from schema import Use
 
 
 class FSPluginConfig:
     BASE_DIR_KEY = "baseDir"
     DEPLOYMENT_DIR_PREFIX_KEY = "deploymentDirPrefix"
     DEPLOYMENT_INFO_FILE = "deploymentInfoFile"
     DEPLOYMENT_PREDICTION_BASE_URL = "deploymentPredictionBaseUrl"
     DEPLOYMENT_KV_FILE = "deploymentKVFile"
 
     def __init__(self, plugin_config):
-        log = logging.getLogger("{}.{}".format(self.__class__.__module__, self.__class__.__name__))
+        log = logging.getLogger(f"{self.__class__.__module__}.{self.__class__.__name__}")
         self._config = plugin_config
 
         schema = Schema(
             {
                 FSPluginConfig.BASE_DIR_KEY: And(str, len),
                 FSPluginConfig.DEPLOYMENT_DIR_PREFIX_KEY: And(str, len),
                 FSPluginConfig.DEPLOYMENT_INFO_FILE: And(str, len),
@@ -86,16 +87,17 @@
 class FilesystemPlugin(BosunPluginBase):
     def __init__(self, plugin_config, private_config_file, pe_info, dry_run):
         super().__init__(plugin_config, private_config_file, pe_info, dry_run)
         self._read_config_file()
         self._config = FSPluginConfig(self._plugin_config)
 
     #  =====  Plugin Internal functions ==========
-    def _create_deployment_structure(self, di):
-        self._logger.info("Creating deployment structure for: {}".format(di.id))
+    def _create_deployment_structure(self, di: DeploymentInfo):
+        self._logger.info(f"Creating deployment structure for: {di.id}")
+        assert di.model_artifact is not None
 
         deployment_dir = self._deployment_dir(di)
         model_base_path = os.path.basename(di.model_artifact)
         model_path = os.path.join(deployment_dir, model_base_path)
 
         self._logger.info(
             "Copying model artifact: {}, size: {}".format(
@@ -105,112 +107,110 @@
         os.makedirs(deployment_dir, exist_ok=True)
         shutil.copyfile(di.model_artifact, model_path)
 
         self._logger.info("Updating deployment info file")
         self._write_deployment_info_file(di)
         self._write_deployment_kv_file(di)
 
-    def _deployment_dir(self, di):
+    def _deployment_dir(self, di: DeploymentInfo):
         return self._deployment_dir_from_id(di.id)
 
     def _deployment_dir_from_id(self, deployment_id):
         return (
             os.path.join(self._config.base_dir, self._config.deployment_dir_prefix + deployment_id)
             + os.path.sep
         )
 
-    def _deployment_info_file(self, di):
+    def _deployment_info_file(self, di: DeploymentInfo):
         return os.path.join(self._deployment_dir(di), self._config.deployment_info_file)
 
-    def _deployment_kv_file(self, di):
+    def _deployment_kv_file(self, di: DeploymentInfo):
         return os.path.join(self._deployment_dir(di), self._config.deployment_kv_file)
 
-    def _write_deployment_info_file(self, di):
+    def _write_deployment_info_file(self, di: DeploymentInfo):
         model_id = di.new_model_id if di.new_model_id is not None else di.model_id
         data = {
             "deployment_id": di.id,
             "model_id": model_id,
         }
         with open(self._deployment_info_file(di), "w+") as fd:
             yaml.dump(data, fd, default_flow_style=False)
 
-    def _write_deployment_kv_file(self, di):
+    def _write_deployment_kv_file(self, di: DeploymentInfo):
 
         # If file is not created if deployment
         if not self._config.deployment_kv_file:
             self._logger.debug("Skipping writing kv file")
             return
-        self._logger.debug("writing deployment kv file {}".format(self._deployment_kv_file(di)))
+        self._logger.debug(f"writing deployment kv file {self._deployment_kv_file(di)}")
         with open(self._deployment_kv_file(di), "w") as fd:
             yaml.dump(di.kv_config, fd, default_flow_style=False)
 
     def _check_base_dir(self):
         if not os.path.exists(self._config.base_dir):
             return ActionStatusInfo(
-                ActionStatus.ERROR, msg="Unable to detect folder: {}".format(self._config.base_dir)
+                ActionStatus.ERROR, msg=f"Unable to detect folder: {self._config.base_dir}"
             )
         if not os.path.isdir(self._config.base_dir):
             return ActionStatusInfo(
                 ActionStatus.ERROR,
-                msg="Provided folder '{}' - is not a directory".format(self._config.base_dir),
+                msg=f"Provided folder '{self._config.base_dir}' - is not a directory",
             )
         if not os.access(self._config.base_dir, os.W_OK):
             return ActionStatusInfo(
                 ActionStatus.ERROR,
-                msg="Provided folder '{}' - is not write accessible".format(self._config.base_dir),
+                msg=f"Provided folder '{self._config.base_dir}' - is not write accessible",
             )
 
         return ActionStatusInfo(ActionStatus.OK, msg="all ok")
 
     def _read_config_file(self):
         if self._private_config_file is None:
             return
 
-        self._logger.info(
-            "Filesystem plugin private config file: {}".format(self._private_config_file)
-        )
+        self._logger.info(f"Filesystem plugin private config file: {self._private_config_file}")
 
         with open(self._private_config_file) as conf_file:
             config = yaml.safe_load(conf_file)
         self._logger.debug(config)
         self._plugin_config.update(config)
         if self._logger.isEnabledFor(logging.DEBUG):
             self._logger.debug(self.get_sanitized_config(self._plugin_config))
 
     def _deployment_status(self, deployment_dir, model_format=None, model_execution_type=None):
         if not os.path.exists(deployment_dir):
             return ActionStatusInfo(
                 ActionStatus.ERROR,
-                msg="No deployment dir: {}".format(deployment_dir),
+                msg=f"No deployment dir: {deployment_dir}",
                 state=DeploymentState.ERROR,
             )
 
         if model_format and model_execution_type == ModelPackageConstants.MODEL_EXECUTION_DEDICATED:
             suffix = DeploymentInfoConfigConstants.model_artifact_suffix(model_format)
-            model_files = glob.glob(os.path.join(deployment_dir, "*.{}".format(suffix)))
+            model_files = glob.glob(os.path.join(deployment_dir, f"*.{suffix}"))
             if len(model_files) != 1:
                 return ActionStatusInfo(
                     ActionStatus.ERROR, msg="Missing model artifact", state=DeploymentState.ERROR
                 )
 
         deployment_info = os.path.join(deployment_dir, self._config.deployment_info_file)
         if not os.path.exists(deployment_info):
             return ActionStatusInfo(
                 ActionStatus.ERROR,
-                msg="No deployment info file: {}".format(deployment_info),
+                msg=f"No deployment info file: {deployment_info}",
                 state=DeploymentState.ERROR,
             )
 
         with open(deployment_info) as info:
             config = yaml.safe_load(info)
             missing_fields = [f for f in self._config.deployment_info_fields if f not in config]
             if len(missing_fields) > 0:
                 return ActionStatusInfo(
                     ActionStatus.ERROR,
-                    msg="Invalid config file, missing fields: {}".format(missing_fields),
+                    msg=f"Invalid config file, missing fields: {missing_fields}",
                     state=DeploymentState.ERROR,
                 )
 
         return ActionStatusInfo(
             ActionStatus.OK,
             state=DeploymentState.READY,
             data={ActionDataFields.CURRENT_MODEL_ID: config["model_id"]},
@@ -234,116 +234,111 @@
         return ActionStatusInfo(ActionStatus.OK)
 
     def deployment_list(self):
         self._logger.info("-------> deployment_list called")
 
         deployments_map = {}
         list_deployment = glob.glob(
-            os.path.join(self._config.base_dir, "{}*".format(self._config.deployment_dir_prefix))
+            os.path.join(self._config.base_dir, f"{self._config.deployment_dir_prefix}*")
         )
 
         for deployment_dir in list_deployment:
             deployments_status = self._deployment_status(deployment_dir)
             deployment_id = os.path.basename(deployment_dir).replace(
                 self._config.deployment_dir_prefix, ""
             )
             deployments_map[deployment_id] = deployments_status.__dict__
 
         if len(list_deployment) == 0:
             status_msg = "No containers running"
         else:
-            status_msg = "Number of deployments: {}".format(len(list_deployment))
+            status_msg = f"Number of deployments: {len(list_deployment)}"
 
         self._logger.info(status_msg)
         self._logger.info("Deployments: " + str(deployments_map))
         return ActionStatusInfo(ActionStatus.OK, msg=status_msg, data=deployments_map)
 
-    def deployment_start(self, deployment_info):
+    def deployment_start(self, di: DeploymentInfo):
         """
         Create a directory structure for deployment
         :param deployment_info: deployment information
         :return:
         """
         self._logger.info("-------> deployment_start called")
-        di = DeploymentInfo(deployment_info)
 
         self._create_deployment_structure(di)
         self._logger.info("Filesystem deployment_start completed successfully")
         prediction_url = "{}/deployments/{}{}/predictions".format(
             self._config.prediction_base_url, self._config.deployment_dir_prefix, di.id
         )
         data = {ActionDataFields.PREDICTION_URL: prediction_url}
         return ActionStatusInfo(ActionStatus.OK, state=DeploymentState.READY, data=data)
 
-    def deployment_stop(self, deployment_data):
+    def deployment_stop(self, deployment_id: str):
         """
         Removes deployment directory under base dir
         :param deployment_info: deployment information
         :return:
         """
         self._logger.info("-------> deployment_stop called")
-        deployment_dir = self._deployment_dir_from_id(deployment_data["id"])
+        deployment_dir = self._deployment_dir_from_id(deployment_id)
 
-        self._logger.info("Stopping deployment - removing deployment dir {}".format(deployment_dir))
+        self._logger.info(f"Stopping deployment - removing deployment dir {deployment_dir}")
         try:
             if os.path.exists(deployment_dir):
                 shutil.rmtree(deployment_dir)
             self._logger.info("Filesystem deployment_stop completed successfully")
             return ActionStatusInfo(status=ActionStatus.OK, state=DeploymentState.STOPPED)
         except OSError:
             return ActionStatusInfo(status=ActionStatus.ERROR, state=DeploymentState.ERROR)
 
-    def deployment_replace_model(self, deployment_info):
+    def deployment_replace_model(self, di: DeploymentInfo):
         """
         Update directory content for current deployment
         :param deployment_info: deployment information
         :return:
         """
         self._logger.info("-------> deployment_replace_model called")
-        di = DeploymentInfo(deployment_info)
         try:
             shutil.rmtree(self._deployment_dir(di))
         except OSError:
             return ActionStatusInfo(status=ActionStatus.ERROR, state=DeploymentState.ERROR)
 
-        self._logger.info("Replacing deployment {}".format(di.id))
+        self._logger.info(f"Replacing deployment {di.id}")
         self._create_deployment_structure(di)
         self._logger.info("Filesystem deployment_replace_model completed successfully")
         return ActionStatusInfo(ActionStatus.OK, state=DeploymentState.READY)
 
-    def deployment_status(self, deployment_info):
+    def deployment_status(self, di: DeploymentInfo):
         """
         Check that deployment directory exists and has correct content
         :param deployment_info: deployment information
         :return:
         """
         self._logger.info("-------> deployment_status called")
-        di = DeploymentInfo(deployment_info)
         deployment_dir = self._deployment_dir(di)
 
         return self._deployment_status(deployment_dir, di.model_format, di.model_execution_type)
 
     def pe_status(self):
         """
         Verify that base directory exists and is a directory
         :return:
         """
         self._logger.info("---------> pe_status called")
         pe_status = self._check_base_dir()
         if pe_status.status != ActionStatus.OK:
             return pe_status
 
-        self._logger.info(
-            "PE is ok .. checking deployments [{}]".format(len(self._pe_info.deployments))
-        )
+        assert self._pe_info is not None
+        self._logger.info(f"PE is ok .. checking deployments [{len(self._pe_info.deployments)}]")
         # TODO: Add logic for orphaned deployments, as k8s plugin
         all_deployments_status = {}
-        for deployment in self._pe_info.deployments:
-            di = DeploymentInfo(deployment)
-            self._logger.info("Checking status for deployment: {}".format(di.id))
+        for di in self._pe_info.deployments:
+            self._logger.info(f"Checking status for deployment: {di.id}")
             deployment_dir = self._deployment_dir(di)
             d_status = self._deployment_status(
                 deployment_dir, di.model_format, di.model_execution_type
             )
 
             all_deployments_status[di.id] = d_status.to_dict()
             self._logger.info(d_status.to_yaml())
```

## bosun/plugin/k8s/client.py

```diff
@@ -19,14 +19,17 @@
 from itertools import chain
 
 import yaml
 from kubernetes import client
 from kubernetes import config
 from kubernetes import utils
 from kubernetes import watch
+from kubernetes.client.models.v1_deployment import V1Deployment
+from kubernetes.client.models.v1_deployment_list import V1DeploymentList
+from kubernetes.client.models.version_info import VersionInfo
 from kubernetes.config.kube_config import list_kube_config_contexts
 from kubernetes.dynamic import DynamicClient
 from kubernetes.dynamic.resource import ResourceList
 from kubernetes.stream import stream
 from requests import codes
 
 DEPLOYMENT_CHECK_DELAY = 3
@@ -36,25 +39,26 @@
 log = logging.getLogger(__name__)
 logd = logging.getLogger(__name__ + ".dedupe")
 
 # Wrap Kubernetes exceptions so callers of our client don't need to be aware that we are just a thin
 # wrapper.
 ClientError = client.rest.ApiException
 ClientErrorList = utils.FailToCreateError
+K8sDeployment = V1Deployment
 
 
 class FailToDeleteError(ClientErrorList):
     pass
 
 
 class _SimpleDedupe(logging.Filter):
     """Simple log filter to hush consecutive duplicate log messages."""
 
     def __init__(self):
-        self.last_sent = None
+        self.last_sent = float("-inf")
         self.last_message = None
 
     def filter(self, record):
         # Only display duplicate logs every so often
         if record.msg == self.last_message and (time.time() - self.last_sent) < 240:
             return False
         else:
@@ -67,15 +71,15 @@
 
 
 # TODO there is a lot of use for wait_for that we should look at and try to use a watcher (with
 # retries and use of resourceVersion) more intelligently to be lighter on the API. This is what
 # kubectl does.
 def wait_for(
     checker,
-    timeout=60,
+    timeout=60.0,
     exception=TimeoutError,
     max_retry_delay=DEFAULT_MAX_RETRY_DELAY,
     initial_delay=0,
 ):
     """
     Sometimes it just doesn't make sense to use a watcher and we need to fall back to polling.
     This is a generic function that takes a user defined condition and waits for it to return
@@ -89,15 +93,15 @@
         success = checker(i, start_time)
         if success:
             # Return the value back from the checker() in case it isn't just a True/False
             # value and the caller can do something useful with it.
             return success
         elapsed = time.monotonic() - start_time
         if elapsed > timeout:
-            raise exception("Timed out after {}s".format(elapsed))
+            raise exception(f"Timed out after {elapsed}s")
 
         # Randomize the actual wait to get even spread as illustrated here:
         # https://aws.amazon.com/blogs/architecture/exponential-backoff-and-jitter It is prudent to
         # have a sleep in here because most checkers() are going to be calling into the k8s API and
         # while it can handle a lot of load, it is a finite resource so we need some sleeps before
         # checks.
         wait = random.uniform(1, min(max_retry_delay, 2 ** i))  # nosec
@@ -129,15 +133,15 @@
 
 
 def make_selector(mapping):
     """
     Given a mapping of label names and values, generate a selector expression to use in API
     requests.
     """
-    return ",".join("{}={}".format(k, v) for k, v in mapping.items())
+    return ",".join(f"{k}={v}" for k, v in mapping.items())
 
 
 def json_pointer(value):
     """
     Correctly escapes values for use as JSON Pointers
     http://jsonpatch.com/#json-pointer
     """
@@ -217,15 +221,15 @@
         self.__dynamic_client = DynamicClient(api_client)
         self.namespace = namespace or "default"  # "default" namespace is a k8s convention
         self.config_file = config_file
         self.context = context
         self.__version_info = None
 
     @classmethod
-    def from_config(cls, context=None, config_file=None, namespace=None):
+    def from_config(cls, context=None, config_file=None, namespace=None) -> "K8sClient":
         """
         Returns a new API Client that is configured from loading the normal kubectl config files. We
         also support a special 'IN_CLUSTER' context which means we are running *inside* a Kubernetes
         cluster so no extra configuration is necessary.
         """
         api_client, default_namespace = cls.load_settings(context, config_file)
 
@@ -284,21 +288,17 @@
         return client.VersionApi(self.api)
 
     @property
     def apps_api(self):
         return client.AppsV1Api(self.api)
 
     @property
-    def extensions_api(self):
-        return client.ExtensionsV1beta1Api(self.api)
-
-    @property
-    def version_info(self):
+    def version_info(self) -> VersionInfo:
         if self.__version_info is None:
-            self.__version_info = self.version_api.get_code()
+            self.__version_info: VersionInfo = self.version_api.get_code()
         return self.__version_info
 
     def create_from_dict(self, data):
         """Simple wrapper around the kubernetes-lib function of the same name. Pass it a dict-like
         manifest of a k8s *List kind.
         """
         return utils.create_from_dict(self.api, data, namespace=self.namespace)
@@ -329,19 +329,21 @@
                     log.debug("permission denied when listing %s items; skipping...", resource)
                     continue
                 log.error("Failed searching for resources of type: %s", resource)
                 raise
 
             for item in resp.items:
                 try:
+                    log.debug("deleting %s: %s", item.kind, item.metadata.name)
                     resp = resource.delete(namespace=self.namespace, name=item.metadata.name)
-                    log.debug(
-                        "deleted %s: %s", item.kind, item.metadata.name, extra=dict(response=resp)
-                    )
-                    k8s_objects.append(resp)
+                    log.debug("response post delete: %s", resp)
+                    # Append the original item and not the response because K8s sometimes returns
+                    # the deleted object and sometimes returns a Status object so this makes our
+                    # response consistent.
+                    k8s_objects.append(item)
                 except ClientError as err:
                     api_exceptions.append(err)
         if api_exceptions:
             raise FailToDeleteError(api_exceptions)
         return k8s_objects
 
     def delete_from_dict(self, data):
@@ -453,19 +455,18 @@
         # TODO we should probably be managing the `resource_version` for the caller during retries
         # so we don't miss events.
         api = self.resources.get(api_version=api_version, kind=kind)
         if api.namespaced:
             kwargs["namespace"] = self.namespace
         if sub:
             api = getattr(api, sub)
-        for e in api.watch(**kwargs):
-            yield e
+        yield from api.watch(**kwargs)
 
     @contextmanager
-    def run(self, manifest, cleanup=True, start_timeout=1200):
+    def run(self, manifest, cleanup=True, start_timeout=1200.0):
         """
         This is a context manager that takes a dict-like object of a Pod v1 API `manifest`. It
         is up to the caller to make sure the name of the pod is unique. The function will wait until
         the pod is running and then yield a websocket stream attached to stdin, stdout, and stderr
         to the caller. Upon exiting of the context, we will wait for the pod to terminate and
         optionally delete it if `cleanup` is set. The context manager will wait `start_timeout`
         seconds for the pod to be ready before aborting.
@@ -484,15 +485,15 @@
             def pod_is_running(_, start_time):
                 resp = self.get_pod(name)
                 log.debug("Pod status: %s", resp.status)
                 if resp.status.phase == "Running":
                     return True
 
                 if resp.status.phase != "Pending":
-                    raise RuntimeError("Pod '{}' bypassed 'Running' state".format(name))
+                    raise RuntimeError(f"Pod '{name}' bypassed 'Running' state")
 
                 elapsed = time.monotonic() - start_time
                 if elapsed < 180:  # wait at least a few minutes before short-circuit
                     return False
 
                 # Some conditions aren't worth waiting the full amount of time.
                 if resp.status.container_statuses is not None:
@@ -587,24 +588,24 @@
         # given a chance to terminate gracefully. However, we want a synchronous call that will
         # return when the resource is actually gone in the event we want to turn around and
         # re-create it.
         watcher = watch.Watch()
         for event in watcher.stream(
             self.core_api.list_namespaced_pod,
             self.namespace,
-            field_selector="metadata.name={}".format(name),
+            field_selector=f"metadata.name={name}",
             resource_version=response.metadata.resource_version,
             timeout_seconds=420,
         ):
             log.debug("got event: %s", event)
             if event["type"] == "DELETED":
                 return response  # it has been completely deleted
-        raise TimeoutError("Timed out deleting Pod: {}/{}".format(self.namespace, name))
+        raise TimeoutError(f"Timed out deleting Pod: {self.namespace}/{name}")
 
-    def wait_for_pod_completion(self, name, timeout=60, poll_interval=3, raise_on_failure=False):
+    def wait_for_pod_completion(self, name, timeout=60.0, poll_interval=3, raise_on_failure=False):
         """
         Waits `timeout` seconds for the pod with `name to reach a terminal state by checking its
         status every `poll_interval` seconds. `Unknown` is considered a terminal state by this
         function. If `raise_on_failure` is set, we will raise an error if the pod terminated but not
         with a successful status.
 
         Raises: TimeoutError if the pod does not complete in `timeout` seconds
@@ -625,15 +626,15 @@
                 pod = self.get_pod(name)
                 log.debug("%s/pod/%s status: %s", self.namespace, name, pod.status)
                 self.check_successful_run(pod)
 
     def wait_for_deployment_rollout(
         self,
         name,
-        timeout=900,
+        timeout=900.0,
         max_retry_delay=DEFAULT_MAX_RETRY_DELAY,
     ):
         # https://github.com/kubernetes/kubectl/blob/7b01e2757cc74b1145976726b05cc1108ad2911d/pkg/cmd/rollout/rollout_status.go
         @retry_kubernetes(retry_on_timeout=True)
         def checker(*args):
             try:
                 deployment = self.apps_api.read_namespaced_deployment_status(name, self.namespace)
@@ -746,27 +747,27 @@
             checker,
             timeout=timeout,
             initial_delay=DEPLOYMENT_CHECK_DELAY,
             max_retry_delay=max_retry_delay,
         )
 
     @retry_kubernetes(retry_on_timeout=True)
-    def get_deployments(self, label_selector):
+    def get_deployments(self, label_selector) -> V1DeploymentList:
         response = self.apps_api.list_namespaced_deployment(
             namespace=self.namespace, label_selector=label_selector
         )
         return response
 
     @retry_kubernetes(retry_on_timeout=True)
-    def get_deployment(self, name):
+    def get_deployment(self, name) -> V1Deployment:
         response = self.apps_api.read_namespaced_deployment(name, self.namespace)
         return response
 
     @retry_kubernetes()
-    def update_deployment(self, name, body, timeout=900):
+    def update_deployment(self, name, body, timeout=900.0):
         """Update a deployment."""
         response = self.apps_api.patch_namespaced_deployment(name, self.namespace, body=body)
         log.debug("updated deployment", extra=dict(response=response))
         try:
             self.wait_for_deployment_rollout(
                 # We want to be a little more responsive so half the max wait time
                 name,
@@ -821,15 +822,15 @@
             {
                 "op": "replace",
                 "path": "/spec/template",
                 "value": rollback_replica_set.spec.template,
             },
             {
                 "op": "replace",
-                "path": "/metadata/annotations/{}".format(json_pointer(revision_key)),
+                "path": f"/metadata/annotations/{json_pointer(revision_key)}",
                 "value": rollback_revision_number,
             },
         ]
 
         log.debug("rolling back deployment %s:\n%s", name, patch)
         self.apps_api.patch_namespaced_deployment(body=patch, name=name, namespace=self.namespace)
```

## bosun/plugin/k8s/config.py

```diff
@@ -11,22 +11,23 @@
 #  ---------------------------------------------------------------------------------
 
 import logging
 import re
 from urllib.parse import urlparse
 
 import yaml
-from bosun.plugin.bosun_plugin_base import BosunPluginBase
-from bosun.plugin.constants import BosunPluginConfigConstants
 from schema import Optional
 from schema import Or
 from schema import Regex
 from schema import Schema
 from schema import SchemaError
 
+from bosun.plugin.bosun_plugin_base import BosunPluginBase
+from bosun.plugin.constants import BosunPluginConfigConstants
+
 log = logging.getLogger(__name__)
 
 PATTERN_IP_ADDR = re.compile(r"[0-9.:]+")
 
 
 class KubernetesPluginConfig:
     AGENT_IMAGE = "agentImage"
@@ -74,22 +75,22 @@
 
     def __init__(self, plugin_config):
         def validate_repo_no_tag(s):
             parts = s.split(":")
             # If we can split string into 3 parts then we know it has a tag and is invalid, i.e.
             #    docker.io:5000/datarobot/search:stable-1.4.2
             if len(parts) == 3:
-                msg = 'Repo for generated images must not contain a tag: ":{}"'.format(parts[2])
+                msg = f'Repo for generated images must not contain a tag: ":{parts[2]}"'
                 raise SchemaError(msg)
 
             # Otherwise if we split into two parts we need to make sure it is
             #    this -> docker.io:5000/datarobot/search
             #    not  -> docker.io/datarobot/search:stable-1.4.2
             elif len(parts) == 2 and parts[1].find("/") == -1:
-                msg = 'Repo for generated images must not contain a tag: ":{}"'.format(parts[1])
+                msg = f'Repo for generated images must not contain a tag: ":{parts[1]}"'
                 raise SchemaError(msg)
             return True
 
         schema = Schema(
             {
                 # You need to use a versioned PPS image tag (e.g. not latest) so we can track what
                 # env version was baked with the .mlpkg file.
@@ -185,15 +186,15 @@
                     KubernetesPluginConfig.KANIKO_CONFIG, KubernetesPluginConfig.KANIKO_SECRET
                 )
             )
 
     @classmethod
     def from_files(cls, bosun_config, extra_config_file=None):
         if extra_config_file:
-            log.info("Kubernetes plugin private config file: {}".format(extra_config_file))
+            log.info(f"Kubernetes plugin private config file: {extra_config_file}")
             with open(extra_config_file) as fp:
                 config = yaml.safe_load(fp)
             bosun_config.update(config)
         if log.isEnabledFor(logging.DEBUG):
             log.debug(BosunPluginBase.get_sanitized_config(bosun_config))
         return cls(bosun_config)
 
@@ -432,19 +433,19 @@
     def image_pull_secrets(self):
         return self._config[KubernetesPluginConfig.IMAGE_PULL_SECRETS]
 
     @property
     def kaniko_args(self):
         return (
             [
-                "--skip-tls-verify-registry={}".format(r)
+                f"--skip-tls-verify-registry={r}"
                 for r in self._config[KubernetesPluginConfig.KANIKO_SKIP_VERIFY_REG]
             ]
             + [
-                "--insecure-registry={}".format(r)
+                f"--insecure-registry={r}"
                 for r in self._config[KubernetesPluginConfig.KANIKO_INSECURE_REG]
             ]
             + self._config[KubernetesPluginConfig.KANIKO_EXTRA_ARGS]
         )
 
     @property
     def kaniko_volumes(self):
```

## bosun/plugin/k8s/kubernetes_plugin.py

```diff
@@ -15,28 +15,30 @@
 import tarfile
 import time
 from contextlib import suppress
 from functools import partial
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from tempfile import TemporaryFile
+from typing import Dict
 from urllib.parse import urljoin
 from zipfile import BadZipFile
 from zipfile import ZipFile
 
 from bosun.model_connector.constants import ModelPackageConstants
 from bosun.plugin.action_status import ActionDataFields
 from bosun.plugin.action_status import ActionStatus
 from bosun.plugin.action_status import ActionStatusInfo
 from bosun.plugin.bosun_plugin_base import BosunPluginBase
 from bosun.plugin.constants import DeploymentState
 from bosun.plugin.deployment_info import DeploymentInfo
 
 from .client import ClientError
 from .client import ClientErrorList
+from .client import K8sDeployment
 from .client import codes
 from .client import get_client
 from .client import make_selector
 from .config import KubernetesPluginConfig
 from .manifests import COMPONENT_LABEL_NAME
 from .manifests import DEPLOYMENT_LABEL_NAME
 from .manifests import MODEL_LABEL_NAME
@@ -119,53 +121,54 @@
         """
         self._logger.info("Getting the list of running deployments")
         deployments_map = self._list_deployments()
         if len(deployments_map) == 0:
             status_msg = "No Deployments running"
             self._logger.info(status_msg)
             return ActionStatusInfo(ActionStatus.OK, msg=status_msg)
-        status_msg = "Number of deployments: {}".format(len(deployments_map))
+        status_msg = f"Number of deployments: {len(deployments_map)}"
         self._logger.info(status_msg)
         return ActionStatusInfo(ActionStatus.OK, msg=status_msg, data=deployments_map)
 
     def pe_status(self):
         """
         Checks to see that the K8s API is still functioning correctly. We also implement the
         the extended health check functionality by returning the status of the managed deployments.
         """
         self._logger.info("Getting status of k8s environment")
+        assert self._pe_info is not None
         try:
             self._client.version_api.get_code()  # sanity check to confirm we can talk to k8s API
         except ClientError as err:
-            return ActionStatusInfo(ActionStatus.ERROR, msg="Kubernetes API Issue: {}".format(err))
+            return ActionStatusInfo(ActionStatus.ERROR, msg=f"Kubernetes API Issue: {err}")
 
         k8s_deployments = self._list_deployments()
         pe_deployments = {}
         data = None
-        for di in (DeploymentInfo(deployment) for deployment in self._pe_info.deployments):
+        for di in self._pe_info.deployments:
             if di.id in k8s_deployments:
                 pe_deployments[di.id] = k8s_deployments[di.id]
             else:
                 status_msg = "No record of deployment running in Kubernetes."
                 pe_deployments[di.id] = ActionStatusInfo(
                     ActionStatus.UNKNOWN, msg=status_msg, state=DeploymentState.STOPPED
                 ).to_dict()
 
         expected_vs_reality = set(k8s_deployments) - set(pe_deployments)
         if expected_vs_reality:
             status = ActionStatus.WARN
-            status_msg = "Orphaned deployments exist: {}".format(expected_vs_reality)
+            status_msg = f"Orphaned deployments exist: {expected_vs_reality}"
         else:
             status = ActionStatus.OK
             status_msg = "Cluster is Healthy"
         if bool(pe_deployments):
             data = {ActionDataFields.DEPLOYMENTS_STATUS: pe_deployments}
         return ActionStatusInfo(status, msg=status_msg, data=data)
 
-    def deployment_status(self, deployment_info):
+    def deployment_status(self, di: DeploymentInfo):
         """
         Return the health status of a MLOps deployment. We rely on the liveness/readiness probes
         setup on the Deployment resource to determine its health. We **do not** send traffic through
         the Ingress.
 
         The returned ActionStatusInfo can have the following (status, state) values:
             - status=UNKNOWN, state=STOPPED: if the Deployment does not exist in namespace
@@ -173,35 +176,33 @@
             - status=WARN, state=READY: if the Deployment has at least one ready Pod but less than
               desired
             - status=OK, state=READY: if the Deployment has all desired Pods ready
         """
         # TODO: we should have an optional status mode that checks health E2E (e.g. through external
         # ingress URL)
         self._logger.debug("Getting status for model deployment")
-        di = DeploymentInfo(deployment_info)
         try:
             deployment = self._find_deployment(di)
             return self._deployment_status(deployment)
         except DeploymentNotFound as err:
             return ActionStatusInfo(
                 ActionStatus.UNKNOWN, msg=str(err), state=DeploymentState.STOPPED
             )
 
-    def deployment_start(self, deployment_info):
+    def deployment_start(self, di: DeploymentInfo):
         """
         Create a new deployment. This function is idempotent so it can be called on an existing
         deployment (note, a new image will be built but any existing Deployment, Ingress, etc.
         resources will be left as-is).
 
         The action will wait for at least one replica is reporting ready to serve predictions
         before returning (status=OK, state=READY). Otherwise it will return an (ERROR, ERROR)
         ActionStatus.
         """
         start_time = time.time()
-        di = DeploymentInfo(deployment_info)
         # Render the manifests first so we can make sure everything is valid before starting the
         # _long_ image building process. But it doesn't make sense to actually create them in K8s
         # until after we have a successful image build.
         rendered = self._renderer.get_pps_manifest(di)
         rendered["items"].insert(0, self._renderer.get_mlops_secret_manifest(di))
 
         self._build_pps_image(di)
@@ -250,19 +251,19 @@
             " We will continue to monitor its status and report any changes. We recommend you"
             " examine the cluster or you can attempt to relaunch the deployment to try again."
         )
         return ActionStatusInfo(
             ActionStatus.ERROR, state=DeploymentState.ERROR, msg=status_msg, data=data
         )
 
-    def deployment_stop(self, deployment_data):
+    def deployment_stop(self, deployment_id: str):
         """
         Delete Deployment (and all related) resources from the cluster.
         """
-        deployment_id = deployment_data["id"]
+        assert self._pe_info is not None
         labels = {
             DEPLOYMENT_LABEL_NAME: deployment_id,
             PRED_ENV_LABEL_NAME: self._pe_info.id,
             "app.kubernetes.io/managed-by": "Bosun",
         }
         selector = make_selector(labels)
         self._logger.info(
@@ -272,30 +273,27 @@
         # and this method will attempt to walk the full K8s API which is likely to generate a few
         # permission denied errors that are safe to ignore.
         items = self._client.delete_everything(selector, ignore_auth_errors=True)
         if items:
             self._logger.info(
                 "Deleted resources (%s):\n\t%s",
                 len(items),
-                "\n\t".join(
-                    "Kind: {}; Name: {}".format(i.details.kind, i.details.name) for i in items
-                ),
+                "\n\t".join(f"Kind: {i.kind}; Name: {i.metadata.name}" for i in items),
             )
         return ActionStatusInfo(ActionStatus.OK, state=DeploymentState.STOPPED)
 
-    def deployment_replace_model(self, deployment_info):
+    def deployment_replace_model(self, di: DeploymentInfo):
         """
         Replace the model of an existing deployment with a new one. Updates are done in a rolling
         fashion to cause minimal service disruption.
         """
         # XXX hack until we cleanup `new_model_id` upstream. K8s is declarative so we don't care
         # about old vs. new model IDs -- just tell us what the end result should be.
-        deployment_info["modelId"] = deployment_info.pop("newModelId")
+        di._deployment_info["modelId"] = di._deployment_info.pop("newModelId")
         start_time = time.time()
-        di = DeploymentInfo(deployment_info)
         self._build_pps_image(di)
 
         existing_deployment = self._find_deployment(di)
         name = existing_deployment.metadata.name
         current_model = existing_deployment.metadata.labels[MODEL_LABEL_NAME]
 
         new_spec = self._renderer.get_deployment_for_update(existing_deployment, di)
@@ -308,15 +306,15 @@
             elapsed = time.time() - start_time
             adjusted_deadline = ACTION_TIMEOUT_SECONDS - elapsed
             self._client.update_deployment(name, new_spec, timeout=adjusted_deadline)
         except (ClientError, TimeoutError) as err:
             # In case of launch failure, k8s did not stop the old container, so indicate
             # that in the status response
             self._logger.exception("Deployment update failed")
-            status_msg = "Failed to replace model -\n{}\nContinuing with old model".format(err)
+            status_msg = f"Failed to replace model -\n{err}\nContinuing with old model"
             return ActionStatusInfo(
                 ActionStatus.ERROR,
                 msg=status_msg,
                 state=DeploymentState.ERROR,
                 data={ActionDataFields.OLD_MODEL_IN_USE: True},
             )
 
@@ -325,45 +323,50 @@
         self._logger.info("Recording that %s is now running model %s", di.id, di.model_id)
         new_spec["metadata"]["labels"][MODEL_LABEL_NAME] = di.model_id
         self._client.update_deployment(name, new_spec, timeout=120)
         return ActionStatusInfo(
             ActionStatus.OK, msg="Model replaced successfully", state=DeploymentState.READY
         )
 
-    def _list_deployments(self):
+    def _list_deployments(self) -> Dict[str, dict]:
         """
         Fetches all deployments associated with our Prediction Environment. Returns
         a mapping of {deployment_id: ActionStatusInfo}.
         """
+        assert self._pe_info is not None
         deployments = {}
         # We use a labels to discover all the resources we _own_.
-        selector = "{}={}".format(PRED_ENV_LABEL_NAME, self._pe_info.id)
-        for item in self._client.get_deployments(selector).items:
+        selector = f"{PRED_ENV_LABEL_NAME}={self._pe_info.id}"
+        k8s_deployments = self._client.get_deployments(selector).items
+        assert k8s_deployments is not None
+        for item in k8s_deployments:
             deployment_id = item.metadata.labels[DEPLOYMENT_LABEL_NAME]
             deployments[deployment_id] = self._deployment_status(item).to_dict()
         return deployments
 
-    def _find_deployment(self, di):
+    def _find_deployment(self, di) -> K8sDeployment:
+        assert self._pe_info is not None
         labels = {
             COMPONENT_LABEL_NAME: "predictionServer",
             DEPLOYMENT_LABEL_NAME: di.id,
             PRED_ENV_LABEL_NAME: self._pe_info.id,
         }
         deployments = self._client.get_deployments(make_selector(labels)).items
+        assert deployments is not None
         if len(deployments) == 1:
             return deployments[0]
         elif len(deployments) == 0:
-            raise DeploymentNotFound("No Kubernetes deployment found for: {}".format(di.id))
+            raise DeploymentNotFound(f"No Kubernetes deployment found for: {di.id}")
         else:
             msg = "Got back too many resources associated with deployment {}: {}".format(
                 di.id, [i.metadata.name for i in deployments]
             )
             raise RuntimeError(msg)
 
-    def _deployment_status(self, deployment):
+    def _deployment_status(self, deployment: K8sDeployment):
         """
         The workhorse of deployment_status(), see semantics of that method for details.
         """
         # For now this is just checking the health of the deployment resource (and assumes all
         # supporting infra such as the Service and Ingress are up and working. This is a good
         # minimum bar because checking the health E2E could end up being blocked by things outside
         # our control:
@@ -381,34 +384,34 @@
                     )
             return ActionStatusInfo(ActionStatus.ERROR, msg=status_msg, state=DeploymentState.ERROR)
 
         # We will consider the deployment state still ready if there is at least one replica but it
         # will be a warning if available is less than requested because capacity/redundancy is
         # degraded.
         status = ActionStatus.WARN if available_replicas < requested_replicas else ActionStatus.OK
-        status_msg = "{}/{} Pods are ready.".format(available_replicas, requested_replicas)
+        status_msg = f"{available_replicas}/{requested_replicas} Pods are ready."
         current_model_id = deployment.metadata.labels[MODEL_LABEL_NAME]
         return ActionStatusInfo(
             status,
             msg=status_msg,
             state=DeploymentState.READY,
             data={ActionDataFields.CURRENT_MODEL_ID: current_model_id},
         )
 
-    def _get_prediction_url(self, di):
+    def _get_prediction_url(self, di: DeploymentInfo):
         """
         Based on model type, generate an appropriate URL based on the prefix the user configured.
         """
         if di.model_execution_type == ModelPackageConstants.MODEL_EXECUTION_DEDICATED:
-            predict_path = "{}/predictions".format(di.id)
+            predict_path = f"{di.id}/predictions"
         else:
-            predict_path = "{}/predict/".format(di.id)
+            predict_path = f"{di.id}/predict/"
         return urljoin(self._config.outfacing_prediction_url_prefix, predict_path)
 
-    def _build_pps_image(self, di):
+    def _build_pps_image(self, di: DeploymentInfo):
         """
         Build either a custom-model or native PPS image to serve predictions. We use a tool called
         Kaniko which is single use so for every new build request, we launch a new build Pod. The
         is left for K8s to garbage collect it until either the associated deployment in MLOps is
         stopped or a new build request is submitted (in which case we delete and recreate).
         """
         rendered = self._renderer.get_builder_manifest(di)
@@ -422,15 +425,15 @@
                 raise
             # TODO: add optimization to reuse successful pods that match model_id and pps_version
             pod_name = rendered["metadata"]["name"]
             self._logger.info("Cleaning existing pod (%s) and retrying image build", pod_name)
             self._client.delete_pod(pod_name)
             self._start_new_image_builder(di, rendered)
 
-    def _start_new_image_builder(self, di, rendered):
+    def _start_new_image_builder(self, di: DeploymentInfo, rendered: dict):
         """
         Starts a Kaniko Pod in a way that this plugin can attach to it and send it the Docker build
         context we generated to build either the Custom Model or the frozen native model + PPS
         environment. This method will wait for Kaniko to finish and raise an error if it failed.
         """
         pod_name = rendered["metadata"]["name"]
         # It is safer to just always cleanup this pod on exit to allow the cluster to reclaim
@@ -456,48 +459,50 @@
                     pod_name, partial(self._logger.debug, "%s OUTPUT: %s", pod_name)
                 )
 
             elapsed = time.time() - start_time
             adjusted_deadline = IMAGE_BUILD_DEADLINE_SECONDS - elapsed
             self._client.wait_for_pod_completion(pod_name, timeout=adjusted_deadline)
 
-    def _send_pps_docker_context(self, socket, di):
+    def _send_pps_docker_context(self, socket, di: DeploymentInfo):
         """
         Build and send a Docker context over the socket that will bake a frozen DataRobot Portable
         Prediction API that includes the deployment's mlpkg ready to serve.
         """
+        assert di.model_artifact is not None
         with TemporaryFile() as buff:
             tar = tarfile.open(mode="w:gz", fileobj=buff)
             self._logger.info("Preparing Docker context for image builder...")
             t = self._renderer.get_template("Dockerfile.pps-model.j2")
             content = t.render(di=di, config=self._config)
             self._logger.debug("Writing Dockerfile:\n%s", content)
             with TemporaryFile() as dockerfile:
                 dockerfile.write(content.encode("utf8"))
                 dockerfile.seek(0)
                 tarinfo = tar.gettarinfo(arcname="Dockerfile", fileobj=dockerfile)
                 self._logger.debug("adding to context: %s", tarinfo.get_info())
                 tar.addfile(tarinfo, fileobj=dockerfile)
             with open(di.model_artifact, mode="rb") as fh:
-                tarinfo = tar.gettarinfo(arcname="model_{}.mlpkg".format(di.model_id), fileobj=fh)
+                tarinfo = tar.gettarinfo(arcname=f"model_{di.model_id}.mlpkg", fileobj=fh)
                 self._logger.debug("adding to context: %s", tarinfo.get_info())
                 tar.addfile(tarinfo, fileobj=fh)
             tar.close()
 
             total_size = buff.tell()
             buff.seek(0)
             _send_chunked_data(socket, buff, total_size)
             socket.close()
 
-    def _send_cm_docker_context(self, socket, di):
+    def _send_cm_docker_context(self, socket, di: DeploymentInfo):
         """
         Using the provided install script from the Custom Model model package, build and send a
         Docker context over the socket.
         """
-        cm_pps_image_name = "cm_pps_{}".format(di.model_id)
+        assert di.model_artifact is not None
+        cm_pps_image_name = f"cm_pps_{di.model_id}"
         with TemporaryDirectory() as tmp_dir:
             tmp_dir = Path(tmp_dir)
             try:
                 with ZipFile(di.model_artifact, "r") as zip_ref:
                     zip_ref.extractall(tmp_dir)
             except BadZipFile:
                 stats = "(file does not exist)"
```

## bosun/plugin/k8s/manifests.py

```diff
@@ -92,15 +92,15 @@
 
 def _truncate_middle(s, max_length):
     if len(s) <= max_length:
         return s
     # half of the size, minus the 3 .'s
     n_2 = floor(max_length / 2) - 3
     n_1 = max_length - n_2 - 3  # whatever's left
-    return "{}...{}".format(s[:n_1], s[-n_2:])
+    return f"{s[:n_1]}...{s[-n_2:]}"
 
 
 def clean_as_kubernetes_name(value):
     """
     Kubernetes name can consist of lowercase alphanumeric characters, '-', or '.'.
     It must start and end with an an alphanumeric characters.
     There is also a max length of 253 characters.
@@ -228,10 +228,10 @@
     def validate_k8s_version(version_info):
         """
         Our manifests are only designed to support specific versions of K8s.
 
         Raises ValueError if provided an unsupported version of K8s.
         """
         # .minor isn't always a pure number so use a regexp to validate
-        if version_info.major != "1" or not re.match(r"(19|2[0-4]).*", version_info.minor):
-            status_msg = "K8s server version must be 1.19 to 1.24"
+        if version_info.major != "1" or not re.match(r"(2[1-9]|[3-9]\d).*", version_info.minor):
+            status_msg = "K8s server version must be 1.21+"
             raise ValueError(status_msg)
```

## bosun/plugin/k8s/templates/model-resources/pdb.yaml.j2

```diff
@@ -1,10 +1,9 @@
 {% import '_helpers.j2' as helpers %}
-{# TODO update apiVersion when v1.21 is min supported version #}
-- apiVersion: policy/v1beta1
+- apiVersion: policy/v1
   kind: PodDisruptionBudget
   metadata:
     name: "{{ helpers.name(di) }}"
     labels:
       {{ COMPONENT_LABEL_NAME }}: predictionServer
       {{ helpers.default_labels(di) | indent(6) }}
     annotations:
```

## bosun/plugin/s3/s3_plugin.py

```diff
@@ -13,14 +13,15 @@
 import logging
 import os
 import pprint
 from pathlib import Path
 
 import boto3
 import yaml
+
 from bosun.model_connector.constants import ModelPackageConstants
 from bosun.plugin.action_status import ActionStatus
 from bosun.plugin.action_status import ActionStatusInfo
 from bosun.plugin.bosun_plugin_base import BosunPluginBase
 from bosun.plugin.constants import DeploymentInfoConfigConstants
 from bosun.plugin.constants import DeploymentState
 from bosun.plugin.deployment_info import DeploymentInfo
@@ -42,15 +43,15 @@
         Reading the plugin specific config file if such is provided. And overriding this plugin
         configuration
         :return:
         """
         if self._private_config_file is None:
             return
 
-        self._logger.info("S3 plugin private config file: {}".format(self._private_config_file))
+        self._logger.info(f"S3 plugin private config file: {self._private_config_file}")
 
         with open(self._private_config_file) as conf_file:
             config = yaml.safe_load(conf_file)
         self._logger.info(config)
         self._plugin_config.update(config)
         if self._logger.isEnabledFor(logging.DEBUG):
             self._logger.debug(self.get_sanitized_config(self._plugin_config))
@@ -69,27 +70,27 @@
         objects = []
         for obj in response.get(S3Plugin.CONTENTS_KEY, []):
             key = obj["Key"]
             if key.endswith(suffix):
                 objects.append(key)
         return objects
 
-    def _deployment_dir(self, di):
+    def _deployment_dir(self, di: DeploymentInfo):
         return self._deployment_dir_from_id(di.id)
 
     def _deployment_dir_from_id(self, deployment_id):
         return (
             os.path.join(self._config.base_dir, self._config.deployment_dir_prefix + deployment_id)
             + os.path.sep
         )
 
-    def _deployment_info_file(self, di):
+    def _deployment_info_file(self, di: DeploymentInfo):
         return os.path.join(self._deployment_dir(di), self._config.deployment_info_file)
 
-    def _write_deployment_info_file(self, di):
+    def _write_deployment_info_file(self, di: DeploymentInfo):
         model_id = di.new_model_id if di.new_model_id is not None else di.model_id
         data = {
             "deployment_id": di.id,
             "model_id": model_id,
         }
 
         self._s3.put_object(
@@ -112,15 +113,15 @@
 
     def _deployment_status(self, deployment_dir, model_format=None, model_execution_type=None):
         obj_list = self._s3.list_objects(Bucket=self._config.bucket_name, Prefix=deployment_dir)
         self._logger.debug(pprint.pformat(obj_list))
         if not self._is_path_exists(obj_list, deployment_dir):
             return ActionStatusInfo(
                 ActionStatus.ERROR,
-                msg="No deployment dir: {}".format(deployment_dir),
+                msg=f"No deployment dir: {deployment_dir}",
                 state=DeploymentState.ERROR,
             )
         if model_format and model_execution_type == ModelPackageConstants.MODEL_EXECUTION_DEDICATED:
             model_files = self._list_objects_matching(
                 prefix=deployment_dir,
                 suffix=DeploymentInfoConfigConstants.model_artifact_suffix(model_format),
             )
@@ -130,15 +131,15 @@
                     ActionStatus.ERROR, msg="Missing model artifact", state=DeploymentState.ERROR
                 )
 
         deployment_info = os.path.join(deployment_dir, self._config.deployment_info_file)
         if not self._is_path_exists(obj_list, deployment_info):
             return ActionStatusInfo(
                 ActionStatus.ERROR,
-                msg="Deployment info file is missing: {}".format(deployment_info),
+                msg=f"Deployment info file is missing: {deployment_info}",
                 state=DeploymentState.ERROR,
             )
 
         return ActionStatusInfo(ActionStatus.OK, state=DeploymentState.READY)
 
     def _delete_deployment(self, deployment_dir):
         obj_list = self._s3.list_objects(Bucket=self._config.bucket_name, Prefix=deployment_dir)
@@ -163,23 +164,24 @@
             msg = "all ok"
         return ActionStatusInfo(status, msg=msg)
 
     def plugin_stop(self):
         self._logger.info("S3 plugin_stop called")
         return ActionStatusInfo(ActionStatus.OK)
 
-    def _create_deployment_structure(self, di):
-        self._logger.info("Applying deployment: {}".format(di.id))
+    def _create_deployment_structure(self, di: DeploymentInfo):
+        self._logger.info(f"Applying deployment: {di.id}")
+        assert di.model_artifact is not None
 
         deployment_dir = self._deployment_dir(di)
         obj_list = self._s3.list_objects(Bucket=self._config.bucket_name, Prefix=deployment_dir)
         self._logger.debug(pprint.pformat(obj_list))
 
         if not self._is_path_exists(obj_list, deployment_dir):
-            self._logger.info("Deployment directory does not exist: {}".format(deployment_dir))
+            self._logger.info(f"Deployment directory does not exist: {deployment_dir}")
 
         model_base_path = os.path.basename(di.model_artifact)
         model_path = os.path.join(deployment_dir, model_base_path)
 
         self._logger.info(
             "Uploading model artifact: {}, size: {}".format(
                 di.model_artifact, os.path.getsize(di.model_artifact)
@@ -188,51 +190,47 @@
         self._s3.upload_file(
             Bucket=self._config.bucket_name, Key=model_path, Filename=str(di.model_artifact)
         )
 
         self._logger.info("Updating deployment info file")
         self._write_deployment_info_file(di)
 
-    def deployment_start(self, deployment_info):
-        di = DeploymentInfo(deployment_info)
-        self._logger.info("Starting deployment {}".format(di.id))
+    def deployment_start(self, di: DeploymentInfo):
+        self._logger.info(f"Starting deployment {di.id}")
 
         self._create_deployment_structure(di)
         return ActionStatusInfo(ActionStatus.OK, state=DeploymentState.READY)
 
-    def deployment_stop(self, deployment_data):
+    def deployment_stop(self, deployment_id: str):
         """
         Stop the cron job and delete it
         :return:
         """
         self._logger.info("Stopping deployment - doing nothing - no file will be deleted")
-        deployment_dir = self._deployment_dir_from_id(deployment_data["id"])
+        deployment_dir = self._deployment_dir_from_id(deployment_id)
         self._delete_deployment(deployment_dir)
 
         status = ActionStatus.OK
         return ActionStatusInfo(status=status, state=DeploymentState.STOPPED)
 
-    def deployment_replace_model(self, deployment_info):
+    def deployment_replace_model(self, di: DeploymentInfo):
         """
         Will put a model artifact in a place the prediction job can consume it
         :param deployment_info: Info about the deployment
         :param model_artifact_path:
         :return:
         """
-        di = DeploymentInfo(deployment_info)
-        self._logger.info(
-            "-- Replacing model for deployment: {} dry_run: {}".format(di.id, self._dry_run)
-        )
+        self._logger.info(f"-- Replacing model for deployment: {di.id} dry_run: {self._dry_run}")
         deployment_dir = self._deployment_dir(di)
         self._delete_deployment(deployment_dir)
 
         self._create_deployment_structure(di)
         return ActionStatusInfo(
             ActionStatus.OK,
-            msg="Model replaced successfully, new model id: {}".format(di.new_model_id),
+            msg=f"Model replaced successfully, new model id: {di.new_model_id}",
             state=DeploymentState.READY,
         )
 
     def pe_status(self):
         """
         Do status check
         :return:
@@ -242,27 +240,26 @@
             Bucket=self._config.bucket_name, Prefix=self._config.base_dir
         )
         if self._is_path_exists(obj_list, self._config.base_dir):
             status = ActionStatus.OK
             status_msg = None
         else:
             status = ActionStatus.ERROR
-            status_msg = "Error: no base dir: {}".format(self._config.base_dir)
+            status_msg = f"Error: no base dir: {self._config.base_dir}"
 
-        self._logger.info("pe_status: {} {}".format(status, status_msg))
+        self._logger.info(f"pe_status: {status} {status_msg}")
         return ActionStatusInfo(status=status, msg=status_msg)
 
-    def deployment_status(self, deployment_info):
+    def deployment_status(self, di: DeploymentInfo):
         """
         :param deployment_info: Info about the deployment to check
         Do status check
         :return:
         """
         self._logger.info("Getting status for python batch deployment")
-        di = DeploymentInfo(deployment_info)
         deployment_dir = self._deployment_dir(di)
 
         return self._deployment_status(deployment_dir, di.model_format, di.model_execution_type)
 
     def deployment_list(self):
         self._logger.info("Getting the list of running deployments")
 
@@ -275,12 +272,12 @@
                 self._config.deployment_dir_prefix, ""
             )
             deployments_map[deployment_id] = deployments_status.__dict__
 
         if len(deployment_set) == 0:
             status_msg = "No containers running"
         else:
-            status_msg = "Number of deployments: {}".format(len(deployment_set))
+            status_msg = f"Number of deployments: {len(deployment_set)}"
 
         self._logger.info(status_msg)
         self._logger.info("Deployments: " + str(deployments_map))
         return ActionStatusInfo(ActionStatus.OK, msg=status_msg, data=deployments_map)
```

## bosun/plugin/s3/s3_plugin_config.py

```diff
@@ -18,29 +18,29 @@
 class S3PluginConfig:
     BUCKET_NAME_KEY = "bucketName"
     BASE_DIR_KEY = "baseDir"
     DEPLOYMENT_DIR_PREFIX_KEY = "deploymentDirPrefix"
     DEPLOYMENT_INFO_FILE = "deploymentInfoFile"
 
     def __init__(self, plugin_config):
-        log = logging.getLogger("{}.{}".format(self.__class__.__module__, self.__class__.__name__))
+        log = logging.getLogger(f"{self.__class__.__module__}.{self.__class__.__name__}")
         self._config = plugin_config
 
         schema = {
             S3PluginConfig.BUCKET_NAME_KEY: str,
             S3PluginConfig.BASE_DIR_KEY: str,
             S3PluginConfig.DEPLOYMENT_DIR_PREFIX_KEY: str,
             S3PluginConfig.DEPLOYMENT_INFO_FILE: str,
             BosunPluginConfigConstants.MLOPS_BOSUN_PRED_ENV_ENABLE_MONITORING_KEY: bool,
         }
         for f in schema:
             if f not in self._config:
-                raise Exception("Field {} is missing in plugin config {}".format(f, self._config))
+                raise Exception(f"Field {f} is missing in plugin config {self._config}")
 
-            log.debug("self._config[f]: {} {}".format(self._config[f], type(self._config[f])))
+            log.debug(f"self._config[f]: {self._config[f]} {type(self._config[f])}")
             if type(self._config[f]) != schema[f]:
                 raise Exception(
                     "Field {} type: {} is not as expected: {}".format(
                         f, type(self._config[f]), schema[f]
                     )
                 )
```

## bosun/plugin/snowflake/snowflake_plugin.py

```diff
@@ -11,38 +11,34 @@
 #  ---------------------------------------------------------------------------------
 import os
 import textwrap
 from typing import Optional
 from typing import Union
 
 import snowflake.connector
+from snowflake.connector import DatabaseError
+from snowflake.connector import ProgrammingError
+
 from bosun.plugin.action_status import ActionStatus
 from bosun.plugin.action_status import ActionStatusInfo
 from bosun.plugin.bosun_plugin_base import BosunPluginBase
 from bosun.plugin.constants import DeploymentState
 from bosun.plugin.deployment_info import DeploymentInfo
-from bosun.plugin.pe_info import PEInfo
 from bosun.plugin.snowflake.snowflake_plugin_config import SnowflakePluginConfig
-from snowflake.connector import DatabaseError
-from snowflake.connector import ProgrammingError
 
 
 class SnowflakePlugin(BosunPluginBase):
-    EMPTY_MODEL_LOCATION = "<No Location>"
-
     def __init__(self, plugin_config, private_config_file, pe_info, dry_run):
         super().__init__(plugin_config, private_config_file, pe_info, dry_run)
-        self._private_config_file = private_config_file
-        self._pe_info = PEInfo(pe_info) if pe_info else None
         self._conn = None
 
     def get_config(
         self, deployment: Optional[Union[DeploymentInfo, str]] = None
     ) -> SnowflakePluginConfig:
-        self._logger.info("Snowflake plugin config file: {}".format(self._private_config_file))
+        self._logger.info(f"Snowflake plugin config file: {self._private_config_file}")
         config = SnowflakePluginConfig.read_config(
             self._pe_info, self._private_config_file, deployment
         )
         config.validate_config()
         return config
 
     def _snowflake_connect(self):
@@ -64,14 +60,15 @@
                 connection_properties["user"] = config.user
                 connection_properties["password"] = config.password
 
             self._conn = snowflake.connector.connect(**connection_properties)
 
     def _execute_query(self, query, fetch_all=True):
         self._snowflake_connect()
+        assert self._conn is not None
         cur = self._conn.cursor()
         try:
             cur.execute(query)
             result = cur.fetchall() if fetch_all else cur.sfqid
         finally:
             cur.close()
 
@@ -88,29 +85,30 @@
                 udf_function_prefix=config.udf_function_prefix,
                 db=config.database,
                 schema=config.schema,
             )
 
             last_query_id = self._execute_query(get_all_deployed_udfs, fetch_all=False)
             filter_udf_by_prediction_env_id = (
-                "SELECT \"name\", \"description\" FROM TABLE(RESULT_SCAN('{last_query_id}')) "
+                'SELECT "name", "description" FROM TABLE(RESULT_SCAN(\'{last_query_id}\')) '
                 "WHERE \"description\" = '{prediction_env_id}'".format(
                     prediction_env_id=config.prediction_environment_id, last_query_id=last_query_id
                 )
             )
 
             deployment_udfs = self._execute_query(filter_udf_by_prediction_env_id)
         except (DatabaseError, ProgrammingError) as e:
             self._logger.error(e)
             return ActionStatusInfo(ActionStatus.ERROR, msg=str(e))
 
         if deployment_udfs is not None and len(deployment_udfs) > 0:
-            status_msg = "Number of scoring code UDFs deployed: {}".format(len(deployment_udfs))
+            status_msg = f"Number of scoring code UDFs deployed: {len(deployment_udfs)}"
         else:
             status_msg = "No scoring code UDFs deployed"
+            deployment_udfs = []
 
         self._logger.info(status_msg)
         self._logger.info("Deployed Scoring Code UDFs: " + str(deployment_udfs))
 
         deployments_map = {}
         deployment_ready = ActionStatusInfo(ActionStatus.OK, state=DeploymentState.READY).__dict__
 
@@ -119,25 +117,24 @@
             deployment_id = udf_name.split("_")[-1].lower()
             # A UDF in Snowflake either exists or doesn't, so if it's there, then it is ready
             deployments_map[deployment_id] = deployment_ready
 
         self._logger.info("Deployments: " + str(deployments_map))
         return ActionStatusInfo(ActionStatus.OK, msg=status_msg, data=deployments_map)
 
-    def deployment_start(self, deployment: dict):
-        di = DeploymentInfo(deployment)
+    def deployment_start(self, di: DeploymentInfo):
         config = self.get_config(di)
 
-        if di.model_artifact == self.EMPTY_MODEL_LOCATION:
+        if di.model_artifact is None or not di.model_artifact.exists():
             return ActionStatusInfo(
                 ActionStatus.ERROR,
                 "Model must be pulled from DataRobot deployment, before pushing it to Snowflake.",
             )
 
-        self._logger.info("Starting deployment {}".format(di.id))
+        self._logger.info(f"Starting deployment {di.id}")
         udf_scoring_jar = os.path.basename(di.model_artifact)
 
         try:
             self._logger.info(
                 "Uploading model artifact: %s, size: %s",
                 udf_scoring_jar,
                 os.path.getsize(di.model_artifact),
@@ -177,53 +174,50 @@
         except (DatabaseError, ProgrammingError) as e:
             self._logger.error(e)
             return ActionStatusInfo(ActionStatus.ERROR, msg=str(e))
 
         self._logger.info("Scoring Code UDF deployed successfully.")
         return ActionStatusInfo(ActionStatus.OK, state=DeploymentState.READY)
 
-    def deployment_stop(self, deployment: dict):
-        deployment_id = deployment["id"]
-        config = self.get_config(deployment_id)
+    def deployment_stop(self, deployment_id: str):
         self._logger.info("Stopping deployment %s", deployment_id)
+        config = self.get_config(deployment_id)
         self._logger.info("Deleting Scoring Code UDF: %s", config.udf_function_name)
         query = "DROP FUNCTION IF EXISTS {udf_name} (OBJECT)".format(
             udf_name=config.udf_function_name
         )
         try:
             self._execute_query(query, fetch_all=False)
         except (DatabaseError, ProgrammingError) as e:
             self._logger.error(e)
             return ActionStatusInfo(ActionStatus.ERROR, msg=str(e))
 
         self._logger.info("Scoring Code UDF removed")
         return ActionStatusInfo(ActionStatus.OK, state=DeploymentState.STOPPED)
 
-    def deployment_replace_model(self, deployment: dict):
-        di = DeploymentInfo(deployment)
-        self._logger.info("Replacing model for deployment: {}".format(di.id))
-        return self.deployment_start(deployment)
+    def deployment_replace_model(self, di: DeploymentInfo):
+        self._logger.info(f"Replacing model for deployment: {di.id}")
+        return self.deployment_start(di)
 
     def pe_status(self):
         try:
             self._execute_query("SELECT 1")
             status = ActionStatus.OK
             status_msg = "Snowflake connection successful"
         except (DatabaseError, ProgrammingError):
             status = ActionStatus.ERROR
             status_msg = "Failed to connect to Snowflake"
             self._logger.error(status_msg, exc_info=True)
 
         self._logger.info(status_msg)
         return ActionStatusInfo(status=status, msg=status_msg)
 
-    def deployment_status(self, deployment: dict):
-        di = DeploymentInfo(deployment)
+    def deployment_status(self, di: DeploymentInfo):
         config = self.get_config(di)
-        self._logger.info("Getting status for deployment: {}".format(di.id))
+        self._logger.info(f"Getting status for deployment: {di.id}")
         check_udf_function_deployed = "SHOW USER FUNCTIONS LIKE '{udf_name}'".format(
             udf_name=config.udf_function_name
         )
 
         try:
             udf_functions_deployed = self._execute_query(check_udf_function_deployed)
         except (DatabaseError, ProgrammingError) as e:
```

## bosun/plugin/snowflake/snowflake_plugin_config.py

```diff
@@ -10,20 +10,21 @@
 #  https://www.datarobot.com/wp-content/uploads/2021/07/DataRobot-Tool-and-Utility-Agreement.pdf.
 #  ---------------------------------------------------------------------------------
 import os
 from typing import Optional as Nullable
 from typing import Union
 
 import yaml
-from bosun.plugin.deployment_info import DeploymentInfo
-from bosun.plugin.pe_info import PEInfo
 from schema import Optional
 from schema import Or
 from schema import Schema
 
+from bosun.plugin.deployment_info import DeploymentInfo
+from bosun.plugin.pe_info import PEInfo
+
 
 class SnowflakePluginConfig:
     AUTH_TYPE = "authType"
     OAUTH_TOKEN = "oauthToken"
     ACCOUNT = "account"
     WAREHOUSE = "warehouse"
     DATABASE = "database"
@@ -111,15 +112,14 @@
 
             # Set configuration from Deployment KV config
             if deployment.kv_config:
                 for key in cls.config_keys:
                     if key in deployment.kv_config:
                         config[key] = deployment.kv_config[key]
         elif deployment:
-            # If deployment wasn't a DeploymentInfo object then it is just the deployment ID
             config[cls.DEPLOYMENT_ID] = deployment
 
         return SnowflakePluginConfig(config)
 
     @property
     def account(self):
         return self._config.get(SnowflakePluginConfig.ACCOUNT)
```

## Comparing `datarobot_bosun-9.0.7.data/scripts/bosun-plugin-runner` & `datarobot_bosun-9.1.1b1.data/scripts/bosun-plugin-runner`

 * *Files identical despite different names*

## Comparing `datarobot_bosun-9.0.7.data/scripts/mcrunner` & `datarobot_bosun-9.1.1b1.data/scripts/mcrunner`

 * *Files identical despite different names*

## Comparing `datarobot_bosun-9.0.7.data/scripts/plugin-runner` & `datarobot_bosun-9.1.1b1.data/scripts/plugin-runner`

 * *Files identical despite different names*

## Comparing `datarobot_bosun-9.0.7.dist-info/METADATA` & `datarobot_bosun-9.1.1b1.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: datarobot-bosun
-Version: 9.0.7
+Version: 9.1.1b1
 Summary: datarobot-bosun module providing MLOps Management framework and plug-ins
 Home-page: http://datarobot.com
 Author: DataRobot
 Author-email: info@datarobot.com
 License: DataRobot
 Project-URL: Documentation, https://docs.datarobot.com/en/docs/release/public-preview/mlops-preview/mgmt-agent.html#mlops-management-agent
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: MacOS
@@ -19,22 +20,25 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: pyyaml
 Requires-Dist: pytz
 Requires-Dist: python-dateutil
 Requires-Dist: schema
 Requires-Dist: datarobot-mlops-connected-client (>=7.1)
-Requires-Dist: importlib-resources ; python_version < "3.7"
+Provides-Extra: azureml
+Requires-Dist: azure-ai-ml (>=1.3) ; extra == 'azureml'
+Requires-Dist: azure-identity (>=1.12) ; extra == 'azureml'
 Provides-Extra: docker
 Requires-Dist: requests ; extra == 'docker'
 Requires-Dist: docker ; extra == 'docker'
 Provides-Extra: kubernetes
 Requires-Dist: jinja2 ; extra == 'kubernetes'
 Requires-Dist: requests ; extra == 'kubernetes'
-Requires-Dist: kubernetes (>=19.15.0b1) ; extra == 'kubernetes'
+Requires-Dist: kubernetes (!=25.*,>=19.15) ; (python_version < "3.9") and extra == 'kubernetes'
+Requires-Dist: kubernetes (>=19.15) ; (python_version >= "3.9") and extra == 'kubernetes'
 Provides-Extra: s3
 Requires-Dist: boto3 (<2,>=1.11.4) ; extra == 's3'
 Provides-Extra: snowflake
 Requires-Dist: snowflake-connector-python (>=2.7.12) ; extra == 'snowflake'
 
 # Bosun - DataRobot's MLOps event manager
 
@@ -81,7 +85,9 @@
 ```
 
 The example above will invoke the `plugin-runner` program which in turn will load and run the test plugin. The `my_config.yaml` file will be loaded and the configuration will be provided to the plugin. The action to run is `pe_status` which is supposed to return the status of the prediction environment. The `--status-file` argument is the path to the status file that should contain the plugin result of running the action.
 
 ## The Bosun Model Connector Framework
 
 This framework provides a simple way to develop and test model connectors. A model connector is a program that fetches the model artifact given the model metadata. This framework provides some built-in support for models stored on S3 and local file systems.
+
+
```

## Comparing `datarobot_bosun-9.0.7.dist-info/RECORD` & `datarobot_bosun-9.1.1b1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,69 @@
 bosun/model_connector/__init__.py,sha256=DkDcTr72Blt8vM8naGFt7uhMdGjy_hwr7mq73bGRbLw,583
 bosun/model_connector/config_external.json,sha256=q_aj-Hz6UUl5YByy26DyrB4Pzz0V-SYbRCmiDckSZHY,399
 bosun/model_connector/constants.py,sha256=rTgnedPFzr9o0vPFV3q9iNh0gZcYBrCWTfB_z4w-q7U,1507
-bosun/model_connector/file_uri_fetcher.py,sha256=AC3IOHM8nS6RDsE5Ar37S4BgxCEz5bqs38PvfAzfZqs,1419
-bosun/model_connector/mc_bosun.py,sha256=LBYODbVx0lZ7dOq7DR_JdjXoe9gHYkFZFEntdFqeSIM,7328
-bosun/model_connector/mc_runner.py,sha256=xS2OJz9NHCqYeA2RfhclYaoUYQOCuxju-9sTKqm8cTI,5310
-bosun/model_connector/model_connector_base.py,sha256=NZhEO_eHjzHoO-ja8rMWbURf6wIYRYL8T20xedyapQY,5526
-bosun/model_connector/s3_uri_fetcher.py,sha256=8ab_8w1C-y-X-EkWD3L4v1mAVAxJAK4GO0UYIsX5ozw,2373
+bosun/model_connector/file_uri_fetcher.py,sha256=voMRhzmZEY23uRh0LqL5w5aZCZxaAmWfgT_O3TBW1QQ,1395
+bosun/model_connector/mc_bosun.py,sha256=lCo6xyXg6YfwsP8Oh2UmFVQgusLwUpDcD98qyEFHACA,7190
+bosun/model_connector/mc_runner.py,sha256=xFxhvllb0W--AoP7m1aN0GyCY2eOQBk4e9D0heKm5R8,5269
+bosun/model_connector/model_connector_base.py,sha256=DSV1DI9n6bPk0J5dzQjQQCRHsIpawGF5miBX3f2hRMY,5433
+bosun/model_connector/s3_uri_fetcher.py,sha256=MAhtLIBhy8T-ACUFQ_-OyRl-Dm4UEpyq2ZlXO210dS4,2334
 bosun/model_connector/uri_fetcher_base.py,sha256=03RVfWSkb_jIa6EpIIwmIOfcw-6EMcW5wzwmIHnvB0Y,894
 bosun/plugin/__init__.py,sha256=jpqAqC1Ils82n2QssUt_W0fcKI6z6JUz4KJ-tyMWTro,583
-bosun/plugin/action_status.py,sha256=tD8APWM1--cLlW43rqFGQ2MgkfSX_6rSbYeivcBLhl0,2270
-bosun/plugin/bosun_plugin_base.py,sha256=8xqll7foSWuzTdzL66HpXsEuGJ_GL09irH2wOujSJ6w,5513
-bosun/plugin/bosun_test_plugin.py,sha256=JacgPX3HPm2Y8UZnxxEPvQLj75hF5b799xgkKzELvmY,11655
-bosun/plugin/constants.py,sha256=QqaHp1cAR3oHgdRRZE2uikXne1tVIhXxiRjrc0D4J78,2707
-bosun/plugin/deployment_info.py,sha256=W6X_iut2rEfIIPNQ01cSZznm_PLyb3xzvpaHw27Zjpw,3066
+bosun/plugin/action_status.py,sha256=3WAqo1_pSw5KzIzvNbhvmgChiC_lX2ViRAGEsl8yUG8,2225
+bosun/plugin/bosun_plugin_base.py,sha256=X2wtg6Zn4QxZEvB7WsnDkweKb2KyaRBrEJzZaixF9_g,5957
+bosun/plugin/bosun_test_plugin.py,sha256=W97oxU9Y__d5e_LGkPV6f2UtZvj3cuyHkZ1AKq1D7Mw,11466
+bosun/plugin/constants.py,sha256=QDr7g31LPrxk5ToCTW129XrWJ1od11hiP0kK1W_GI_Y,2735
+bosun/plugin/deployment_info.py,sha256=lJOP2S9sQC-bw-X5rMHw3IZbBV4-DcKH2vvGe9OF4QE,3354
 bosun/plugin/exceptions.py,sha256=XiPxJWyRd50MBAO3Ztu4KrlL5oSBjcPBK8IDD1sWHo0,1047
-bosun/plugin/pe_info.py,sha256=qxm2vgKcbqnomLcCgoah-B4HCgHTGHaKM97KX5pVNJA,2109
-bosun/plugin/plugin_runner.py,sha256=019XjgjE-En32u_Lo9YVogYCnP2h1houDsC9PXvdnOQ,17074
+bosun/plugin/pe_info.py,sha256=ey2Ef1zzK1jHO705xlpZo3jmdA5UW2S6e99mf_Xy4YI,2493
+bosun/plugin/plugin_runner.py,sha256=fvjuJASX6wXNyGROVwUM-SY1CYqbRgQB5mHQZ1f3Wmw,16631
+bosun/plugin/azureml/__init__.py,sha256=w0FppK0OReL18im5hlOAeWB_NYCFPFaSmnbqIxIspj4,640
+bosun/plugin/azureml/azureml_plugin.py,sha256=QKjTRB4ybxj4E6zYd01Yq7qaLFr0RxmRqnS7vDecJoY,8275
+bosun/plugin/azureml/azureml_status_reporter.py,sha256=z5fSZy1xGfx7eFkR7wcWOlbbwgM2rnfKGI_cvepPax4,3058
+bosun/plugin/azureml/template_renderer.py,sha256=8y5kt4asrvtykNCu7SU-d4_HXJHc_8Nkt6PN-DzpM6I,1504
+bosun/plugin/azureml/client/base_endpoint_client.py,sha256=Iydk78rg395b6xf5skGWb_egNHoxG8GsPZI95tuDI8Q,10060
+bosun/plugin/azureml/client/batch_endpoint_client.py,sha256=prciD-GZ3VrqHSBvPw3puN-ptbXiG28P4jIC-sDqmiA,5885
+bosun/plugin/azureml/client/online_endpoint_client.py,sha256=4sgQmsRKaRsPLGofaoiwzQia_OUiVekPSjLgHUYwOLI,12088
+bosun/plugin/azureml/client/scoring_snippets.py,sha256=kboJhrumqNhJvwTV_LHzkkSel1WONvhuoOx4FS3lWPw,1680
+bosun/plugin/azureml/config/__init__.py,sha256=5LKBu0qgbs3MEvPz1MWIyivQ_LsncJV9bDTFdIEqoJk,583
+bosun/plugin/azureml/config/azureml_client_config.py,sha256=f70E3E_qdtB1EtohQ3BPYYKpBd1CrMpK-HY0oRIoZk4,8036
+bosun/plugin/azureml/config/config_keys.py,sha256=LK8HBTgCmGlHa3FjypcNLN77hehb5dj1bZniIpI6gxQ,3059
+bosun/plugin/azureml/templates/azureml_batch_endpoint_score.py,sha256=cpg30f2gjntk6lDhUvZaHv29m-ZhKXzW-F3fDN6pAz4,3368
+bosun/plugin/azureml/templates/azureml_online_endpoint_score.py,sha256=hl0-GjpuW8QiUfqD8AfaO6Hn4nRpPgHrydK5dXOfn6A,4814
 bosun/plugin/config_samples/__init__.py,sha256=sAc8oDBMnbrQI82jZrO-TKBO4JwXaMPLnO7cZw6GkxM,702
 bosun/plugin/docker/__init__.py,sha256=HBnE1c15RavjXjjlGCEqQm7PgKETJl1cLW3othCfBPU,757
-bosun/plugin/docker/docker_helper.py,sha256=rH0b-wXIGjD21JeVppcUwMv2ONdlcIXwQYMMh1zQYsM,15366
-bosun/plugin/docker/docker_plugin.py,sha256=OzwF7DnjDfcDXhYAAwH5eK24JHKSdHB9Fj7fxHUGa2M,23613
-bosun/plugin/docker/docker_plugin_config.py,sha256=Y0GgLUqlJxjzB_PFKoiybmdTvY70fZdPP2z2eothW00,5439
-bosun/plugin/docker/mlops_monitoring.py,sha256=vYLk6erAW84_zQ0qeh91BLRPebeaTFGkON25Axhb52M,7945
+bosun/plugin/docker/docker_helper.py,sha256=fubvtoFhsJihzazfLk2gsfD_1YgxE0B_aJSoacQEcKU,14934
+bosun/plugin/docker/docker_plugin.py,sha256=LCoEkUCfaVKf4VcGrSM7wWVnRcWMazNBCj2tKPNzFek,23290
+bosun/plugin/docker/docker_plugin_config.py,sha256=haxXV6dkolVNXXxy1uG7e3O7xV32ALibwDVwye2234U,5419
+bosun/plugin/docker/mlops_monitoring.py,sha256=UXtIj4Uybr9SY4m1uFZAoiRpsOAii343rYPpVt2trZ0,7897
 bosun/plugin/filesystem/__init__.py,sha256=DS_gsVTXiCIXCKL6eJe14Jye0Q08EvJoQaFagwvzTJI,646
-bosun/plugin/filesystem/filesystem_plugin.py,sha256=cC92cjuLZuDC2R2PUUWLZlb_TAv_auh_u3rEOM5D4j4,14203
+bosun/plugin/filesystem/filesystem_plugin.py,sha256=PB675cG9e59i1qSzEd2CbCjXXHRYZrp08X9p-bFXKk0,14021
 bosun/plugin/k8s/__init__.py,sha256=AfSBWxZWkUluB4pI2V6dlvZ1znEdTT8wDx4QHxSQIZ8,646
-bosun/plugin/k8s/client.py,sha256=YuEE0yQBzzSvf6JNICIh4VG-x_wh-ABZoR_pI3IdTJo,36684
-bosun/plugin/k8s/config.py,sha256=iJVMhF-kvrCrapVtLQMWYWmZXioXdqPbmiLDpUtUtW4,19957
-bosun/plugin/k8s/kubernetes_plugin.py,sha256=aByXUlseokOo4pShwbg8EUgRpIUSXbl8eI0O7OoEsTs,27946
-bosun/plugin/k8s/manifests.py,sha256=Ovv1MNvLS1t95Z1bBOKVIl8otZ2IYkGxba0JD6w8l3k,9182
+bosun/plugin/k8s/client.py,sha256=TX0Zz3z6VPypQLeh5nyIwWF9AjJ2rlMHzRq6XQ2uPSU,37071
+bosun/plugin/k8s/config.py,sha256=RYoz9P034IZXw-CTn4oFxCYgVkbcQA0-P--sZSY1khY,19918
+bosun/plugin/k8s/kubernetes_plugin.py,sha256=nerEx-jAYOap7qMq_m0vSGG3liBU8ToTc3R4aSqqb3k,28164
+bosun/plugin/k8s/manifests.py,sha256=j0IesWl7nnOAvwphIIYSACrzM6JoGNqBK4tteQxInKg,9170
 bosun/plugin/k8s/templates/Dockerfile.pps-model.j2,sha256=i9mZbUArvs1q4N6z9vtB5CHqya3USqRzK17Zwl-6w1k,303
 bosun/plugin/k8s/templates/_helpers.j2,sha256=arpcrQvzhk-ZH7pyIpNXPqIf1NZ2RlrZxfyuY3DAfZs,2263
 bosun/plugin/k8s/templates/cm_pps_installer.sh.j2,sha256=L5F7pP4M_HqsNP2wTqMMiNDbWB5pndHQi2vHlr4mCDo,4603
 bosun/plugin/k8s/templates/image-builder.yaml.j2,sha256=DjYTQSHq2uSxC0bOPr-fp6nrZEFi1tcmTVIkwpt2dRM,1393
 bosun/plugin/k8s/templates/mlops-api-secret.yaml.j2,sha256=RgnvF5CGVBsq3ThtKU3MjjlALUqD-w1xjkEjZ0sR14g,356
 bosun/plugin/k8s/templates/model-resources.yaml.j2,sha256=A1SW1aNFSswwsHXhh89u4L9p2Bd10jTJItjNFJpRcWA,1106
 bosun/plugin/k8s/templates/model-resources/deployment.yaml.j2,sha256=xWJR6dxoL-_-_BwpVdv9WDqqw4X8v97tymUi5nJrQRo,4929
 bosun/plugin/k8s/templates/model-resources/extra.yaml.j2,sha256=1LRvU1g2owLignZ9bjefrVkrzk_Tlap5yVX8evk2Kz4,119
 bosun/plugin/k8s/templates/model-resources/hpa.yaml.j2,sha256=6qlsvgIUeV7GcMjEPWpPKPrVCETSTmUcq184O_NiKGU,842
 bosun/plugin/k8s/templates/model-resources/ingress.yaml.j2,sha256=b3K54nLIDeeHJp2mn9VzMM45Z8x0NVGRrhm0YTz3PT0,1253
-bosun/plugin/k8s/templates/model-resources/pdb.yaml.j2,sha256=rGHJbliASUZbCMdoatTXw_-GN_7O1pnekjzx6GOqYcc,554
+bosun/plugin/k8s/templates/model-resources/pdb.yaml.j2,sha256=Uu_JR1FDrMOSgdROcaDpDkfSQzVaSYrrVxJfV6-LtPk,484
 bosun/plugin/k8s/templates/model-resources/service.yaml.j2,sha256=uvp3IeGLMR1slrY9S5jlPH8lm4tRwm1lD3HnAm36jU0,547
 bosun/plugin/s3/__init__.py,sha256=K1whUFDQfXk5zzO_B7cdIf5rFBhBXkKveGb2utt5OAo,630
-bosun/plugin/s3/s3_plugin.py,sha256=9fJoKombdPj6RFJ1EQMgNJIX5Y6cL1HPsEveDgebq8Q,11310
-bosun/plugin/s3/s3_plugin_config.py,sha256=8rFJGVVO3c3gNnKtqIKtI-Bg4SomQ63z3FGXLYD7TLs,2735
+bosun/plugin/s3/s3_plugin.py,sha256=EF-orhokbNFCev9P1liSroojc6TdT3A-2wdPGO79CEI,11175
+bosun/plugin/s3/s3_plugin_config.py,sha256=bDKpMgdCEXSiLiAmKlEcw5DP0ShrTZmUbJuA3U6VbRs,2705
 bosun/plugin/snowflake/__init__.py,sha256=DP4zjkZvK-kb975NTxg1HF_UTQYbwQPszpI2QJUbdR8,644
-bosun/plugin/snowflake/snowflake_plugin.py,sha256=ly7pmEfuwK21Qh1B7haUJFQZl_b6r0GNPQXwRweIiAk,10353
-bosun/plugin/snowflake/snowflake_plugin_config.py,sha256=ioY5My79eInfJnJS-vwEV33EGsyBRHas3e9rXdmV0zw,5583
-datarobot_bosun-9.0.7.data/scripts/bosun-plugin-runner,sha256=e8YQBceK8QeD8EFh1q5Vb-jlAYxlrzvZllDq3LNnVPg,671
-datarobot_bosun-9.0.7.data/scripts/mcrunner,sha256=FPqMPz123TVvMrWf1bBsu17RSoJJwXA0-M9EG5IdpXg,676
-datarobot_bosun-9.0.7.data/scripts/plugin-runner,sha256=pe1lGnDyvW82cBjewuRhb6ad6q3j4TYEJLurzG6GNdk,671
-datarobot_bosun-9.0.7.dist-info/METADATA,sha256=ehmZPa6encogt_DdHweGCmoAgL5cSbD2gfWxHaWZrK0,4246
-datarobot_bosun-9.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-datarobot_bosun-9.0.7.dist-info/top_level.txt,sha256=zNJvGsG32_zF72Xl_00PTybDZE3u5FXDSxJiFEekRd4,6
-datarobot_bosun-9.0.7.dist-info/RECORD,,
+bosun/plugin/snowflake/snowflake_plugin.py,sha256=HE308wrkeS5Ie1kMrDTKx7KbsRNuDX1qjPapozdaYck,10034
+bosun/plugin/snowflake/snowflake_plugin_config.py,sha256=KclEb3I9xEkJPf-0ZZcH2QCNI1bCRKhmYWy9-aW-GmE,5491
+datarobot_bosun-9.1.1b1.data/scripts/bosun-plugin-runner,sha256=e8YQBceK8QeD8EFh1q5Vb-jlAYxlrzvZllDq3LNnVPg,671
+datarobot_bosun-9.1.1b1.data/scripts/mcrunner,sha256=FPqMPz123TVvMrWf1bBsu17RSoJJwXA0-M9EG5IdpXg,676
+datarobot_bosun-9.1.1b1.data/scripts/plugin-runner,sha256=pe1lGnDyvW82cBjewuRhb6ad6q3j4TYEJLurzG6GNdk,671
+datarobot_bosun-9.1.1b1.dist-info/METADATA,sha256=8h0qjHtlBCZ4xuso6V3HoluqKOoGb74fcE1YWti3vkI,4470
+datarobot_bosun-9.1.1b1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+datarobot_bosun-9.1.1b1.dist-info/top_level.txt,sha256=zNJvGsG32_zF72Xl_00PTybDZE3u5FXDSxJiFEekRd4,6
+datarobot_bosun-9.1.1b1.dist-info/RECORD,,
```

