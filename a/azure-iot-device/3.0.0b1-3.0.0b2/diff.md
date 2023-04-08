# Comparing `tmp/azure-iot-device-3.0.0b1.tar.gz` & `tmp/azure-iot-device-3.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-iot-device-3.0.0b1.tar", last modified: Sat Nov 19 00:36:10 2022, max compression
+gzip compressed data, was "dist\azure-iot-device-3.0.0b2.tar", last modified: Fri Apr  7 23:04:21 2023, max compression
```

## Comparing `azure-iot-device-3.0.0b1.tar` & `azure-iot-device-3.0.0b2.tar`

### file list

```diff
@@ -1,120 +1,43 @@
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.661176 azure-iot-device-3.0.0b1/
--rw-rw-rw-   0        0        0     1162 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/LICENSE
--rw-rw-rw-   0        0        0       68 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/MANIFEST.in
--rw-rw-rw-   0        0        0    14808 2022-11-19 00:36:10.661176 azure-iot-device-3.0.0b1/PKG-INFO
--rw-rw-rw-   0        0        0    13770 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/README.md
--rw-rw-rw-   0        0        0     2757 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/SECURITY.md
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.117990 azure-iot-device-3.0.0b1/azure-iot-device/
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.102363 azure-iot-device-3.0.0b1/azure-iot-device/azure/
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.102363 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.164865 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/
--rw-rw-rw-   0        0        0     1966 2022-11-16 05:12:05.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.182498 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/aio/
--rw-rw-rw-   0        0        0     1914 2022-11-16 05:14:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/aio/__init__.py
--rw-rw-rw-   0        0        0    14751 2022-11-19 00:35:49.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/aio/patch_documentation.py
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.229383 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/
--rw-rw-rw-   0        0        0      218 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/__init__.py
--rw-rw-rw-   0        0        0     1839 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/alarm.py
--rw-rw-rw-   0        0        0     3715 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/async_adapter.py
--rw-rw-rw-   0        0        0     1974 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/asyncio_compat.py
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.260634 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/auth/
--rw-rw-rw-   0        0        0      317 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/auth/__init__.py
--rw-rw-rw-   0        0        0     3650 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/auth/connection_string.py
--rw-rw-rw-   0        0        0     5661 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/auth/sastoken.py
--rw-rw-rw-   0        0        0     2170 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/auth/signing_mechanism.py
--rw-rw-rw-   0        0        0     2528 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/evented_callback.py
--rw-rw-rw-   0        0        0     2237 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/handle_exceptions.py
--rw-rw-rw-   0        0        0     9408 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/http_transport.py
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.282768 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/models/
--rw-rw-rw-   0        0        0      234 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/models/__init__.py
--rw-rw-rw-   0        0        0     2908 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/models/proxy_options.py
--rw-rw-rw-   0        0        0     1463 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/models/x509.py
--rw-rw-rw-   0        0        0    34348 2022-11-18 20:33:54.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/mqtt_transport.py
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.367068 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/pipeline/
--rw-rw-rw-   0        0        0      398 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/pipeline/__init__.py
--rw-rw-rw-   0        0        0     5215 2022-11-14 18:39:01.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/pipeline/config.py
--rw-rw-rw-   0        0        0     3557 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/pipeline/pipeline_events_base.py
--rw-rw-rw-   0        0        0      860 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/pipeline/pipeline_events_mqtt.py
--rw-rw-rw-   0        0        0      981 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/pipeline/pipeline_exceptions.py
--rw-rw-rw-   0        0        0     1252 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/pipeline/pipeline_nucleus.py
--rw-rw-rw-   0        0        0    19448 2022-11-14 18:39:01.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/pipeline/pipeline_ops_base.py
--rw-rw-rw-   0        0        0     1728 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/pipeline/pipeline_ops_http.py
--rw-rw-rw-   0        0        0     3025 2022-11-18 20:33:54.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/pipeline/pipeline_ops_mqtt.py
--rw-rw-rw-   0        0        0    54315 2022-11-18 20:33:54.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/pipeline/pipeline_stages_base.py
--rw-rw-rw-   0        0        0     4884 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/pipeline/pipeline_stages_http.py
--rw-rw-rw-   0        0        0    21441 2022-11-18 20:33:54.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/pipeline/pipeline_stages_mqtt.py
--rw-rw-rw-   0        0        0     8952 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/pipeline/pipeline_thread.py
--rw-rw-rw-   0        0        0     1249 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/transport_exceptions.py
--rw-rw-rw-   0        0        0     1039 2022-11-19 00:35:49.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/constant.py
--rw-rw-rw-   0        0        0     3883 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/exceptions.py
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.398319 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/
--rw-rw-rw-   0        0        0      364 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/__init__.py
--rw-rw-rw-   0        0        0    38880 2022-11-19 00:35:49.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/abstract_clients.py
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.429569 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/aio/
--rw-rw-rw-   0        0        0      280 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/aio/__init__.py
--rw-rw-rw-   0        0        0    31661 2022-11-19 00:35:49.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/aio/async_clients.py
--rw-rw-rw-   0        0        0    12824 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/aio/async_handler_manager.py
--rw-rw-rw-   0        0        0     3394 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/aio/async_inbox.py
--rw-rw-rw-   0        0        0     2349 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/aio/loop_management.py
--rw-rw-rw-   0        0        0      972 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/client_event.py
--rw-rw-rw-   0        0        0     6070 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/edge_hsm.py
--rw-rw-rw-   0        0        0     4056 2022-11-14 18:39:01.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/inbox_manager.py
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.445195 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/models/
--rw-rw-rw-   0        0        0      230 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/models/__init__.py
--rw-rw-rw-   0        0        0     3710 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/models/message.py
--rw-rw-rw-   0        0        0     2728 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/models/methods.py
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.546628 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/
--rw-rw-rw-   0        0        0      312 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/__init__.py
--rw-rw-rw-   0        0        0     1724 2022-11-14 18:39:01.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/config.py
--rw-rw-rw-   0        0        0      498 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/constant.py
--rw-rw-rw-   0        0        0     1182 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/exceptions.py
--rw-rw-rw-   0        0        0     3302 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/http_map_error.py
--rw-rw-rw-   0        0        0     1813 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/http_path_iothub.py
--rw-rw-rw-   0        0        0     8115 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/http_pipeline.py
--rw-rw-rw-   0        0        0    23191 2022-11-18 20:33:54.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/mqtt_pipeline.py
--rw-rw-rw-   0        0        0    15225 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/mqtt_topic_iothub.py
--rw-rw-rw-   0        0        0     2015 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/pipeline_events_iothub.py
--rw-rw-rw-   0        0        0     4222 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/pipeline_ops_iothub.py
--rw-rw-rw-   0        0        0     3846 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/pipeline_ops_iothub_http.py
--rw-rw-rw-   0        0        0     4024 2022-11-14 18:39:01.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/pipeline_stages_iothub.py
--rw-rw-rw-   0        0        0     7971 2022-11-14 18:39:01.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/pipeline_stages_iothub_http.py
--rw-rw-rw-   0        0        0    10994 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/pipeline_stages_iothub_mqtt.py
--rw-rw-rw-   0        0        0    31027 2022-11-19 00:35:49.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/sync_clients.py
--rw-rw-rw-   0        0        0    20887 2022-11-14 18:39:01.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/sync_handler_manager.py
--rw-rw-rw-   0        0        0     3521 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/sync_inbox.py
--rw-rw-rw-   0        0        0     8965 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/patch.py
--rw-rw-rw-   0        0        0    14442 2022-11-19 00:35:49.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/patch_documentation.py
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.566404 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/
--rw-rw-rw-   0        0        0      440 2022-11-14 17:47:14.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/__init__.py
--rw-rw-rw-   0        0        0    11764 2022-11-15 23:38:04.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/abstract_provisioning_device_client.py
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.566404 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/aio/
--rw-rw-rw-   0        0        0      282 2022-11-14 17:47:15.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/aio/__init__.py
--rw-rw-rw-   0        0        0     7684 2022-11-15 23:38:04.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/aio/async_provisioning_device_client.py
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.583040 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/models/
--rw-rw-rw-   0        0        0      194 2022-11-14 17:47:15.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/models/__init__.py
--rw-rw-rw-   0        0        0     4292 2022-11-14 17:47:15.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/models/registration_result.py
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.645551 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/pipeline/
--rw-rw-rw-   0        0        0      272 2022-11-14 17:47:15.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/pipeline/__init__.py
--rw-rw-rw-   0        0        0     1482 2022-11-14 17:47:15.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/pipeline/config.py
--rw-rw-rw-   0        0        0     1152 2022-11-14 17:47:15.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/pipeline/constant.py
--rw-rw-rw-   0        0        0     1269 2022-11-15 23:38:04.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/pipeline/exceptions.py
--rw-rw-rw-   0        0        0    12164 2022-11-18 20:33:54.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/pipeline/mqtt_pipeline.py
--rw-rw-rw-   0        0        0     4253 2022-11-14 17:47:15.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/pipeline/mqtt_topic_provisioning.py
--rw-rw-rw-   0        0        0     2860 2022-11-14 17:47:15.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/pipeline/pipeline_ops_provisioning.py
--rw-rw-rw-   0        0        0    20946 2022-11-14 17:47:15.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/pipeline/pipeline_stages_provisioning.py
--rw-rw-rw-   0        0        0     6639 2022-11-14 17:47:15.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/pipeline/pipeline_stages_provisioning_mqtt.py
--rw-rw-rw-   0        0        0     7398 2022-11-15 23:38:04.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/provisioning/provisioning_device_client.py
--rw-rw-rw-   0        0        0     1357 2022-11-14 17:47:15.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/user_agent.py
-drwxrwxrwx   0        0        0        0 2022-11-19 00:36:10.661176 azure-iot-device-3.0.0b1/azure-iot-device/azure_iot_device.egg-info/
--rw-rw-rw-   0        0        0    14808 2022-11-19 00:36:09.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure_iot_device.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5964 2022-11-19 00:36:10.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure_iot_device.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-19 00:36:09.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure_iot_device.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2022-11-14 17:47:38.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure_iot_device.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      118 2022-11-19 00:36:09.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure_iot_device.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-11-19 00:36:09.000000 azure-iot-device-3.0.0b1/azure-iot-device/azure_iot_device.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2889 2022-11-14 17:47:15.000000 azure-iot-device-3.0.0b1/devbox_setup.md
--rw-rw-rw-   0        0        0     6701 2022-11-19 00:35:49.000000 azure-iot-device-3.0.0b1/migration_guide.md
--rw-rw-rw-   0        0        0       64 2022-11-14 17:47:15.000000 azure-iot-device-3.0.0b1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-19 00:36:10.661176 azure-iot-device-3.0.0b1/setup.cfg
--rw-rw-rw-   0        0        0     3327 2022-11-19 00:35:49.000000 azure-iot-device-3.0.0b1/setup.py
--rw-rw-rw-   0        0        0      224 2022-11-14 17:47:16.000000 azure-iot-device-3.0.0b1/tls_protocol_version_and_ciphers.md
+drwxrwxrwx   0        0        0        0 2023-04-07 23:04:21.929490 azure-iot-device-3.0.0b2/
+-rw-rw-rw-   0        0        0     1183 2023-03-20 16:56:36.000000 azure-iot-device-3.0.0b2/LICENSE
+-rw-rw-rw-   0        0        0       70 2023-03-20 16:56:36.000000 azure-iot-device-3.0.0b2/MANIFEST.in
+-rw-rw-rw-   0        0        0    10220 2023-04-07 23:04:21.929490 azure-iot-device-3.0.0b2/PKG-INFO
+-rw-rw-rw-   0        0        0     9292 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/README.md
+-rw-rw-rw-   0        0        0     2798 2023-03-20 16:56:36.000000 azure-iot-device-3.0.0b2/SECURITY.md
+drwxrwxrwx   0        0        0        0 2023-04-07 23:04:21.493707 azure-iot-device-3.0.0b2/azure-iot-device/
+drwxrwxrwx   0        0        0        0 2023-04-07 23:04:21.492275 azure-iot-device-3.0.0b2/azure-iot-device/azure/
+drwxrwxrwx   0        0        0        0 2023-04-07 23:04:21.493002 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/
+drwxrwxrwx   0        0        0        0 2023-04-07 23:04:21.849423 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/
+-rw-rw-rw-   0        0        0      557 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/__init__.py
+-rw-rw-rw-   0        0        0     6937 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/config.py
+-rw-rw-rw-   0        0        0     3904 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/connection_string.py
+-rw-rw-rw-   0        0        0      944 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/constant.py
+-rw-rw-rw-   0        0        0     1458 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/custom_typing.py
+-rw-rw-rw-   0        0        0     6659 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/edge_hsm.py
+-rw-rw-rw-   0        0        0     1948 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/http_path_iothub.py
+-rw-rw-rw-   0        0        0      818 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/iot_exceptions.py
+-rw-rw-rw-   0        0        0    12573 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/iothub_http_client.py
+-rw-rw-rw-   0        0        0    31367 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/iothub_mqtt_client.py
+-rw-rw-rw-   0        0        0    20351 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/iothub_session.py
+-rw-rw-rw-   0        0        0     8949 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/models.py
+-rw-rw-rw-   0        0        0    41408 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/mqtt_client.py
+-rw-rw-rw-   0        0        0    10800 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/mqtt_topic_iothub.py
+-rw-rw-rw-   0        0        0     4560 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/mqtt_topic_provisioning.py
+-rw-rw-rw-   0        0        0     2141 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/request_response.py
+-rw-rw-rw-   0        0        0    11271 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/sastoken.py
+-rw-rw-rw-   0        0        0     2746 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/signing_mechanism.py
+-rw-rw-rw-   0        0        0     1403 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/user_agent.py
+drwxrwxrwx   0        0        0        0 2023-04-07 23:04:21.929490 azure-iot-device-3.0.0b2/azure-iot-device/azure_iot_device.egg-info/
+-rw-rw-rw-   0        0        0    10220 2023-04-07 23:04:21.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure_iot_device.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1485 2023-04-07 23:04:21.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure_iot_device.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-07 23:04:21.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure_iot_device.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-05 22:47:28.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure_iot_device.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      126 2023-04-07 23:04:21.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure_iot_device.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-07 23:04:21.000000 azure-iot-device-3.0.0b2/azure-iot-device/azure_iot_device.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2939 2023-03-20 16:56:36.000000 azure-iot-device-3.0.0b2/devbox_setup.md
+-rw-rw-rw-   0        0        0    24944 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/migration_guide_iothub.md
+-rw-rw-rw-   0        0        0     6731 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/migration_guide_provisioning.md
+-rw-rw-rw-   0        0        0       70 2023-03-20 16:56:36.000000 azure-iot-device-3.0.0b2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-07 23:04:21.929490 azure-iot-device-3.0.0b2/setup.cfg
+-rw-rw-rw-   0        0        0     3517 2023-04-07 22:42:45.000000 azure-iot-device-3.0.0b2/setup.py
+-rw-rw-rw-   0        0        0      235 2023-03-20 16:56:36.000000 azure-iot-device-3.0.0b2/tls_protocol_version_and_ciphers.md
```

### Comparing `azure-iot-device-3.0.0b1/LICENSE` & `azure-iot-device-3.0.0b2/LICENSE`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-    MIT License
-
-    Copyright (c) Microsoft Corporation. All rights reserved.
-
-    Permission is hereby granted, free of charge, to any person obtaining a copy
-    of this software and associated documentation files (the "Software"), to deal
-    in the Software without restriction, including without limitation the rights
-    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-    copies of the Software, and to permit persons to whom the Software is
-    furnished to do so, subject to the following conditions:
-
-    The above copyright notice and this permission notice shall be included in all
-    copies or substantial portions of the Software.
-
-    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-    SOFTWARE
+    MIT License
+
+    Copyright (c) Microsoft Corporation. All rights reserved.
+
+    Permission is hereby granted, free of charge, to any person obtaining a copy
+    of this software and associated documentation files (the "Software"), to deal
+    in the Software without restriction, including without limitation the rights
+    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+    copies of the Software, and to permit persons to whom the Software is
+    furnished to do so, subject to the following conditions:
+
+    The above copyright notice and this permission notice shall be included in all
+    copies or substantial portions of the Software.
+
+    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+    SOFTWARE
```

### Comparing `azure-iot-device-3.0.0b1/PKG-INFO` & `azure-iot-device-3.0.0b2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,126 +1,99 @@
 Metadata-Version: 2.1
 Name: azure-iot-device
-Version: 3.0.0b1
+Version: 3.0.0b2
 Summary: Microsoft Azure IoT Device Library
 Home-page: https://github.com/Azure/azure-iot-sdk-python/tree/v3
 Author: Microsoft Corporation
 Author-email: opensource@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6, <4
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #
 <div align=center>
     <img src="./doc/images/azure_iot_sdk_python_banner.png"></img>
     <h1> azure-iot-device </h1>
 </div>
 
 ![Build Status](https://azure-iot-sdks.visualstudio.com/azure-iot-sdks/_apis/build/status/Azure.azure-iot-sdk-python)
 
 The Azure IoT Device SDK for Python enables Python developers to easily create IoT device solutions that seamlessly connect to the Azure IoT Hub ecosystem.
 
-* *If you're looking for the azure-iot-hub library, it is now located in the [azure-iot-hub-python](https://github.com/Azure/azure-iot-hub-python) repository*
+* *If you're migrating v2.x.x code to use v3.x.x check the [IoT Hub Migration Guide](https://github.com/Azure/azure-iot-sdk-python/blob/main/migration_guide_iothub.md) and/or the [Provisioning Migration Guide](https://github.com/Azure/azure-iot-sdk-python/blob/main/migration_guide_provisioning.md)*
+
+* *If you're looking for the v2.x.x client library, it is now preserved in the [v2](https://github.com/Azure/azure-iot-sdk-python/tree/v2) branch*
 
 * *If you're looking for the v1.x.x client library, it is now preserved in the [v1-deprecated](https://github.com/Azure/azure-iot-sdk-python/tree/v1-deprecated) branch.*
 
+* *If you're looking for the azure-iot-hub library, it is now located in the [azure-iot-hub-python](https://github.com/Azure/azure-iot-hub-python) repository*
+
+**NOTE: 3.x.x is still in beta and APIs are subject to change until the release of 3.0.0**
+
 
 ## Installing the library
 
 The Azure IoT Device library is available on PyPI:
 
 ```Shell
-pip install azure-iot-device
+pip install azure-iot-device==3.0.0b2
 ```
 
-Python 3.6 or higher is required in order to use the library
+Python 3.7 or higher is required in order to use the library
 
-## Using the library
-API documentation for this package is available via [**Microsoft Docs**](https://docs.microsoft.com/python/api/azure-iot-device/azure.iot.device?view=azure-python).
-
-See our [**quickstart guide**](https://github.com/Azure/azure-iot-sdk-python/tree/main/samples/README.md) for step by step instructions for setting up and using an IoTHub with devices. 
 
-You can also view the [**samples repository**](https://github.com/Azure/azure-iot-sdk-python/tree/main/samples) to see additional examples of basic client usage.
+## Using the library
+You can view the [**samples repository**](https://github.com/Azure/azure-iot-sdk-python/tree/main/samples) to see examples of SDK usage.
 
-Want to start off on the right foot? Be sure to learn about [**common pitfalls**](https://github.com/Azure/azure-iot-sdk-python/wiki/pitfalls) of using this Python SDK before starting a project.  
+Full API documentation for this package is available via [**Microsoft Docs**](https://docs.microsoft.com/python/api/azure-iot-device/azure.iot.device?view=azure-python). Note that this documentation may currently be out of date as v3.x.x is still in preview at the time of this writing.
 
 
 ## Features
 
 :heavy_check_mark: feature available  :heavy_multiplication_x: feature planned but not yet supported  :heavy_minus_sign: no support planned*
 
 *Features that are not planned may be prioritized in a future release, but are not currently planned
 
-These clients only support the **MQTT protocol**.
+This library primarily uses the **MQTT protocol**.
 
-### IoTHub Device Client
+### IoTHubSession
 
 | Features                                                                                                         | Status                     | Description                                                                                                                                                                                                          |
 |------------------------------------------------------------------------------------------------------------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | [Authentication](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-security-deployment)                     | :heavy_check_mark:         | Connect your device to IoT Hub securely with supported authentication, including symmetric key, X-509 Self Signed, Certificate Authority (CA) Signed, and SASToken                                     |
 | [Send device-to-cloud message](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-d2c)     | :heavy_check_mark:         | Send device-to-cloud messages (max 256KB) to IoT Hub with the option to add custom properties.                                                                                                                       |
 | [Receive cloud-to-device messages](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-c2d) | :heavy_check_mark:         | Receive cloud-to-device messages and read associated custom and system properties from IoT Hub.                                                        |
 | [Device Twins](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-device-twins)                     | :heavy_check_mark:         | IoT Hub persists a device twin for each device that you connect to IoT Hub.  The device can perform operations like get twin tags, subscribe to desired properties.                                                |
 | [Direct Methods](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-direct-methods)                 | :heavy_check_mark:         | IoT Hub gives you the ability to invoke direct methods on devices from the cloud.  The SDK supports handler for method specific and generic operation.                                                            |
-| [Connection Status and Error reporting](https://docs.microsoft.com/en-us/rest/api/iothub/common-error-codes)     | :heavy_check_mark:   | Error reporting for IoT Hub supported error code.                                                                                         |
-| Connection Retry                                                                                                   | :heavy_check_mark:         | Dropped connections will be retried with a fixed 10 second interval by default. This functionality can be disabled if desired, and the interval can be configured   |
-| [Upload file to Blob](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-file-upload)               | :heavy_check_mark:         | A device can initiate a file upload and notifies IoT Hub when the upload is complete.  |
-
-### IoTHub Module Client
-
-**Note:** IoT Edge for Python is scoped to Linux containers & devices only. [Learn more](https://techcommunity.microsoft.com/t5/internet-of-things/linux-modules-with-azure-iot-edge-on-windows-10-iot-enterprise/ba-p/1407066) about using Linux containers for IoT edge on Windows devices. 
-
-| Features                                                                                                         | Status                     | Description                                                                                                                                                                                                          |
-|------------------------------------------------------------------------------------------------------------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| [Authentication](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-security-deployment)                     | :heavy_check_mark:         | Connect your device to IoT Hub securely with supported authentication, including symmetric key, X-509 Self Signed, and Certificate Authority (CA) Signed. SASToken authentication is not currently supported.                                                   |
-| [Send device-to-cloud message](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-d2c)     | :heavy_check_mark:         | Send device-to-cloud messages (max 256KB) to IoT Hub with the option to add custom properties.                                                                                                                       |
-| [Receive cloud-to-device messages](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-c2d) | :heavy_check_mark:         | Receive cloud-to-device messages and read associated custom and system properties from IoT Hub, with the option to complete/reject/abandon C2D messages.                                                        |
-| [Device Twins](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-device-twins)                     | :heavy_check_mark:         | IoT Hub persists a device twin for each device that you connect to IoT Hub.  The device can perform operations like get twin tags, subscribe to desired properties.                                                |
-| [Direct Methods](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-direct-methods)                 | :heavy_check_mark:         | IoT Hub gives you the ability to invoke direct methods on devices from the cloud.  The SDK supports handler for method specific and generic operation.                                                            |
-| [Connection Status and Error reporting](https://docs.microsoft.com/en-us/rest/api/iothub/common-error-codes)     | :heavy_check_mark:   | Error reporting for IoT Hub supported error code.                                                                                         |
-| Connection Retry                                                                                                   | :heavy_check_mark:         | Dropped connections will be retried with a fixed 10 second interval.  TThis functionality can be disabled if desired, and the interval can be configured            |
-| Direct Invocation of Method on Modules                                                                           | :heavy_check_mark:         | Invoke method calls to another module using using the Edge Gateway.                                                                                                                                        |
-
-### Provisioning Device Client
-
-| Features                    | Status             | Description                                                                                                                                                                                                                                                                                                                                        |
-|-----------------------------|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| TPM Individual Enrollment   | :heavy_minus_sign: | Provisioning via [Trusted Platform Module](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#trusted-platform-module-tpm).                                                                                                                                                                                                          |
-| X.509 Individual Enrollment | :heavy_check_mark: | Provisioning via [X.509 root certificate](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#root-certificate).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_x509.py) folder and this [quickstart](https://docs.microsoft.com/en-us/azure/iot-dps/quick-create-simulated-device-x509-python) on how to create a device client.   |
-| X.509 Enrollment Group      | :heavy_check_mark: | Provisioning via [X.509 leaf certificate](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#leaf-certificate)).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_x509.py) folder on how to create a device client.                                                                                                                  |
-| Symmetric Key Enrollment    | :heavy_check_mark: | Provisioning via [Symmetric key attestation](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-symmetric-key-attestation)).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_symmetric_key.py) folder on how to create a device client.                                                                                                               |
-
-## Critical Upcoming Changes Notice
-
-### Certificates
-All Azure IoT SDK users are advised to be aware of upcoming TLS certificate changes for Azure IoT Hub and Device Provisioning Service 
-that will impact the SDK's ability to connect to these services. In October 2022, both services will migrate from the current 
-[Baltimore CyberTrust CA Root](https://baltimore-cybertrust-root.chain-demos.digicert.com/info/index.html) to the 
-[DigiCert Global G2 CA root](https://global-root-g2.chain-demos.digicert.com/info/index.html). There will be a 
-transition period beforehand where your IoT devices must have both the Baltimore and Digicert public certificates 
-installed in their certificate store in order to prevent connectivity issues.
-
-**Devices with only the Baltimore public certificate installed will lose the ability to connect to Azure IoT hub and Device Provisioning Service in October 2022.**
+| [Connection Status and Error reporting](https://docs.microsoft.com/en-us/rest/api/iothub/common-error-codes)     | :heavy_check_mark:         | Error reporting for IoT Hub supported error code.                                                                                         |
+| Connection Retry                                                                                                 | :heavy_check_mark:         | Dropped connections will be retried with a fixed 10 second interval by default. This functionality can be disabled if desired, and the interval can be configured   |
+| [Upload file to Blob](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-file-upload)               | :heavy_multiplication_x:   | A device can initiate a file upload and notifies IoT Hub when the upload is complete.  |
+| Direct Invocation of Method on Modules                                                                           | :heavy_multiplication_x:   | Invoke method calls to another module using using the Edge Gateway.         
 
-To prepare for this change, make sure your device's certificate store has both of these public certificates installed.
 
-For a more in depth explanation as to why the IoT services are doing this, please see
-[this article](https://techcommunity.microsoft.com/t5/internet-of-things/azure-iot-tls-critical-changes-are-almost-here-and-why-you/ba-p/2393169).
+### ProvisioningSession
+
+| Features                    | Status                   | Description                                                                                                                                                                                                                                                                                                                                        |
+|-----------------------------|--------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| TPM Individual Enrollment   | :heavy_multiplication_x: | Provisioning via [Trusted Platform Module](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#trusted-platform-module-tpm).                                                                                                                                                                                                          |
+| X.509 Individual Enrollment | :heavy_check_mark:       | Provisioning via [X.509 root certificate](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#root-certificate).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_x509.py) folder and this [quickstart](https://docs.microsoft.com/en-us/azure/iot-dps/quick-create-simulated-device-x509-python) on how to create a device client.   |
+| X.509 Enrollment Group      | :heavy_check_mark:       | Provisioning via [X.509 leaf certificate](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#leaf-certificate)).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_x509.py) folder on how to create a device client.                                                                                                                  |
+| Symmetric Key Enrollment    | :heavy_check_mark:       | Provisioning via [Symmetric key attestation](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-symmetric-key-attestation)).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_symmetric_key.py) folder on how to create a device client.                                                                                                               |
 
 
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.microsoft.com.
```

### Comparing `azure-iot-device-3.0.0b1/README.md` & `azure-iot-device-3.0.0b2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,84 @@
-#
-<div align=center>
-    <img src="./doc/images/azure_iot_sdk_python_banner.png"></img>
-    <h1> azure-iot-device </h1>
-</div>
-
-![Build Status](https://azure-iot-sdks.visualstudio.com/azure-iot-sdks/_apis/build/status/Azure.azure-iot-sdk-python)
-
-The Azure IoT Device SDK for Python enables Python developers to easily create IoT device solutions that seamlessly connect to the Azure IoT Hub ecosystem.
-
-* *If you're looking for the azure-iot-hub library, it is now located in the [azure-iot-hub-python](https://github.com/Azure/azure-iot-hub-python) repository*
-
-* *If you're looking for the v1.x.x client library, it is now preserved in the [v1-deprecated](https://github.com/Azure/azure-iot-sdk-python/tree/v1-deprecated) branch.*
-
-
-## Installing the library
-
-The Azure IoT Device library is available on PyPI:
-
-```Shell
-pip install azure-iot-device
-```
-
-Python 3.6 or higher is required in order to use the library
-
-## Using the library
-API documentation for this package is available via [**Microsoft Docs**](https://docs.microsoft.com/python/api/azure-iot-device/azure.iot.device?view=azure-python).
-
-See our [**quickstart guide**](https://github.com/Azure/azure-iot-sdk-python/tree/main/samples/README.md) for step by step instructions for setting up and using an IoTHub with devices. 
-
-You can also view the [**samples repository**](https://github.com/Azure/azure-iot-sdk-python/tree/main/samples) to see additional examples of basic client usage.
-
-Want to start off on the right foot? Be sure to learn about [**common pitfalls**](https://github.com/Azure/azure-iot-sdk-python/wiki/pitfalls) of using this Python SDK before starting a project.  
-
-
-## Features
-
-:heavy_check_mark: feature available  :heavy_multiplication_x: feature planned but not yet supported  :heavy_minus_sign: no support planned*
-
-*Features that are not planned may be prioritized in a future release, but are not currently planned
-
-These clients only support the **MQTT protocol**.
-
-### IoTHub Device Client
-
-| Features                                                                                                         | Status                     | Description                                                                                                                                                                                                          |
-|------------------------------------------------------------------------------------------------------------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| [Authentication](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-security-deployment)                     | :heavy_check_mark:         | Connect your device to IoT Hub securely with supported authentication, including symmetric key, X-509 Self Signed, Certificate Authority (CA) Signed, and SASToken                                     |
-| [Send device-to-cloud message](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-d2c)     | :heavy_check_mark:         | Send device-to-cloud messages (max 256KB) to IoT Hub with the option to add custom properties.                                                                                                                       |
-| [Receive cloud-to-device messages](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-c2d) | :heavy_check_mark:         | Receive cloud-to-device messages and read associated custom and system properties from IoT Hub.                                                        |
-| [Device Twins](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-device-twins)                     | :heavy_check_mark:         | IoT Hub persists a device twin for each device that you connect to IoT Hub.  The device can perform operations like get twin tags, subscribe to desired properties.                                                |
-| [Direct Methods](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-direct-methods)                 | :heavy_check_mark:         | IoT Hub gives you the ability to invoke direct methods on devices from the cloud.  The SDK supports handler for method specific and generic operation.                                                            |
-| [Connection Status and Error reporting](https://docs.microsoft.com/en-us/rest/api/iothub/common-error-codes)     | :heavy_check_mark:   | Error reporting for IoT Hub supported error code.                                                                                         |
-| Connection Retry                                                                                                   | :heavy_check_mark:         | Dropped connections will be retried with a fixed 10 second interval by default. This functionality can be disabled if desired, and the interval can be configured   |
-| [Upload file to Blob](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-file-upload)               | :heavy_check_mark:         | A device can initiate a file upload and notifies IoT Hub when the upload is complete.  |
-
-### IoTHub Module Client
-
-**Note:** IoT Edge for Python is scoped to Linux containers & devices only. [Learn more](https://techcommunity.microsoft.com/t5/internet-of-things/linux-modules-with-azure-iot-edge-on-windows-10-iot-enterprise/ba-p/1407066) about using Linux containers for IoT edge on Windows devices. 
-
-| Features                                                                                                         | Status                     | Description                                                                                                                                                                                                          |
-|------------------------------------------------------------------------------------------------------------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| [Authentication](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-security-deployment)                     | :heavy_check_mark:         | Connect your device to IoT Hub securely with supported authentication, including symmetric key, X-509 Self Signed, and Certificate Authority (CA) Signed. SASToken authentication is not currently supported.                                                   |
-| [Send device-to-cloud message](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-d2c)     | :heavy_check_mark:         | Send device-to-cloud messages (max 256KB) to IoT Hub with the option to add custom properties.                                                                                                                       |
-| [Receive cloud-to-device messages](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-c2d) | :heavy_check_mark:         | Receive cloud-to-device messages and read associated custom and system properties from IoT Hub, with the option to complete/reject/abandon C2D messages.                                                        |
-| [Device Twins](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-device-twins)                     | :heavy_check_mark:         | IoT Hub persists a device twin for each device that you connect to IoT Hub.  The device can perform operations like get twin tags, subscribe to desired properties.                                                |
-| [Direct Methods](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-direct-methods)                 | :heavy_check_mark:         | IoT Hub gives you the ability to invoke direct methods on devices from the cloud.  The SDK supports handler for method specific and generic operation.                                                            |
-| [Connection Status and Error reporting](https://docs.microsoft.com/en-us/rest/api/iothub/common-error-codes)     | :heavy_check_mark:   | Error reporting for IoT Hub supported error code.                                                                                         |
-| Connection Retry                                                                                                   | :heavy_check_mark:         | Dropped connections will be retried with a fixed 10 second interval.  TThis functionality can be disabled if desired, and the interval can be configured            |
-| Direct Invocation of Method on Modules                                                                           | :heavy_check_mark:         | Invoke method calls to another module using using the Edge Gateway.                                                                                                                                        |
-
-### Provisioning Device Client
-
-| Features                    | Status             | Description                                                                                                                                                                                                                                                                                                                                        |
-|-----------------------------|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| TPM Individual Enrollment   | :heavy_minus_sign: | Provisioning via [Trusted Platform Module](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#trusted-platform-module-tpm).                                                                                                                                                                                                          |
-| X.509 Individual Enrollment | :heavy_check_mark: | Provisioning via [X.509 root certificate](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#root-certificate).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_x509.py) folder and this [quickstart](https://docs.microsoft.com/en-us/azure/iot-dps/quick-create-simulated-device-x509-python) on how to create a device client.   |
-| X.509 Enrollment Group      | :heavy_check_mark: | Provisioning via [X.509 leaf certificate](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#leaf-certificate)).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_x509.py) folder on how to create a device client.                                                                                                                  |
-| Symmetric Key Enrollment    | :heavy_check_mark: | Provisioning via [Symmetric key attestation](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-symmetric-key-attestation)).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_symmetric_key.py) folder on how to create a device client.                                                                                                               |
-
-## Critical Upcoming Changes Notice
-
-### Certificates
-All Azure IoT SDK users are advised to be aware of upcoming TLS certificate changes for Azure IoT Hub and Device Provisioning Service 
-that will impact the SDK's ability to connect to these services. In October 2022, both services will migrate from the current 
-[Baltimore CyberTrust CA Root](https://baltimore-cybertrust-root.chain-demos.digicert.com/info/index.html) to the 
-[DigiCert Global G2 CA root](https://global-root-g2.chain-demos.digicert.com/info/index.html). There will be a 
-transition period beforehand where your IoT devices must have both the Baltimore and Digicert public certificates 
-installed in their certificate store in order to prevent connectivity issues.
-
-**Devices with only the Baltimore public certificate installed will lose the ability to connect to Azure IoT hub and Device Provisioning Service in October 2022.**
-
-To prepare for this change, make sure your device's certificate store has both of these public certificates installed.
-
-For a more in depth explanation as to why the IoT services are doing this, please see
-[this article](https://techcommunity.microsoft.com/t5/internet-of-things/azure-iot-tls-critical-changes-are-almost-here-and-why-you/ba-p/2393169).
-
-
-## Contributing
-
-This project welcomes contributions and suggestions.  Most contributions require you to agree to a
-Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
-the rights to use your contribution. For details, visit https://cla.microsoft.com.
-
-When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
-a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
-provided by the bot. You will only need to do this once across all repos using our CLA.
-
-This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
-For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
-contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
+#
+<div align=center>
+    <img src="./doc/images/azure_iot_sdk_python_banner.png"></img>
+    <h1> azure-iot-device </h1>
+</div>
+
+![Build Status](https://azure-iot-sdks.visualstudio.com/azure-iot-sdks/_apis/build/status/Azure.azure-iot-sdk-python)
+
+The Azure IoT Device SDK for Python enables Python developers to easily create IoT device solutions that seamlessly connect to the Azure IoT Hub ecosystem.
+
+* *If you're migrating v2.x.x code to use v3.x.x check the [IoT Hub Migration Guide](https://github.com/Azure/azure-iot-sdk-python/blob/main/migration_guide_iothub.md) and/or the [Provisioning Migration Guide](https://github.com/Azure/azure-iot-sdk-python/blob/main/migration_guide_provisioning.md)*
+
+* *If you're looking for the v2.x.x client library, it is now preserved in the [v2](https://github.com/Azure/azure-iot-sdk-python/tree/v2) branch*
+
+* *If you're looking for the v1.x.x client library, it is now preserved in the [v1-deprecated](https://github.com/Azure/azure-iot-sdk-python/tree/v1-deprecated) branch.*
+
+* *If you're looking for the azure-iot-hub library, it is now located in the [azure-iot-hub-python](https://github.com/Azure/azure-iot-hub-python) repository*
+
+**NOTE: 3.x.x is still in beta and APIs are subject to change until the release of 3.0.0**
+
+
+## Installing the library
+
+The Azure IoT Device library is available on PyPI:
+
+```Shell
+pip install azure-iot-device==3.0.0b2
+```
+
+Python 3.7 or higher is required in order to use the library
+
+
+## Using the library
+You can view the [**samples repository**](https://github.com/Azure/azure-iot-sdk-python/tree/main/samples) to see examples of SDK usage.
+
+Full API documentation for this package is available via [**Microsoft Docs**](https://docs.microsoft.com/python/api/azure-iot-device/azure.iot.device?view=azure-python). Note that this documentation may currently be out of date as v3.x.x is still in preview at the time of this writing.
+
+
+## Features
+
+:heavy_check_mark: feature available  :heavy_multiplication_x: feature planned but not yet supported  :heavy_minus_sign: no support planned*
+
+*Features that are not planned may be prioritized in a future release, but are not currently planned
+
+This library primarily uses the **MQTT protocol**.
+
+### IoTHubSession
+
+| Features                                                                                                         | Status                     | Description                                                                                                                                                                                                          |
+|------------------------------------------------------------------------------------------------------------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| [Authentication](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-security-deployment)                     | :heavy_check_mark:         | Connect your device to IoT Hub securely with supported authentication, including symmetric key, X-509 Self Signed, Certificate Authority (CA) Signed, and SASToken                                     |
+| [Send device-to-cloud message](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-d2c)     | :heavy_check_mark:         | Send device-to-cloud messages (max 256KB) to IoT Hub with the option to add custom properties.                                                                                                                       |
+| [Receive cloud-to-device messages](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-c2d) | :heavy_check_mark:         | Receive cloud-to-device messages and read associated custom and system properties from IoT Hub.                                                        |
+| [Device Twins](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-device-twins)                     | :heavy_check_mark:         | IoT Hub persists a device twin for each device that you connect to IoT Hub.  The device can perform operations like get twin tags, subscribe to desired properties.                                                |
+| [Direct Methods](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-direct-methods)                 | :heavy_check_mark:         | IoT Hub gives you the ability to invoke direct methods on devices from the cloud.  The SDK supports handler for method specific and generic operation.                                                            |
+| [Connection Status and Error reporting](https://docs.microsoft.com/en-us/rest/api/iothub/common-error-codes)     | :heavy_check_mark:         | Error reporting for IoT Hub supported error code.                                                                                         |
+| Connection Retry                                                                                                 | :heavy_check_mark:         | Dropped connections will be retried with a fixed 10 second interval by default. This functionality can be disabled if desired, and the interval can be configured   |
+| [Upload file to Blob](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-file-upload)               | :heavy_multiplication_x:   | A device can initiate a file upload and notifies IoT Hub when the upload is complete.  |
+| Direct Invocation of Method on Modules                                                                           | :heavy_multiplication_x:   | Invoke method calls to another module using using the Edge Gateway.         
+
+
+### ProvisioningSession
+
+| Features                    | Status                   | Description                                                                                                                                                                                                                                                                                                                                        |
+|-----------------------------|--------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| TPM Individual Enrollment   | :heavy_multiplication_x: | Provisioning via [Trusted Platform Module](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#trusted-platform-module-tpm).                                                                                                                                                                                                          |
+| X.509 Individual Enrollment | :heavy_check_mark:       | Provisioning via [X.509 root certificate](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#root-certificate).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_x509.py) folder and this [quickstart](https://docs.microsoft.com/en-us/azure/iot-dps/quick-create-simulated-device-x509-python) on how to create a device client.   |
+| X.509 Enrollment Group      | :heavy_check_mark:       | Provisioning via [X.509 leaf certificate](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#leaf-certificate)).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_x509.py) folder on how to create a device client.                                                                                                                  |
+| Symmetric Key Enrollment    | :heavy_check_mark:       | Provisioning via [Symmetric key attestation](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-symmetric-key-attestation)).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_symmetric_key.py) folder on how to create a device client.                                                                                                               |
+
+
+## Contributing
+
+This project welcomes contributions and suggestions.  Most contributions require you to agree to a
+Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
+the rights to use your contribution. For details, visit https://cla.microsoft.com.
+
+When you submit a pull request, a CLA-bot will automatically determine whether you need to provide
+a CLA and decorate the PR appropriately (e.g., label, comment). Simply follow the instructions
+provided by the bot. You will only need to do this once across all repos using our CLA.
+
+This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
+For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
+contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
```

### Comparing `azure-iot-device-3.0.0b1/SECURITY.md` & `azure-iot-device-3.0.0b2/SECURITY.md`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-<!-- BEGIN MICROSOFT SECURITY.MD V0.0.7 BLOCK -->
-
-## Security
-
-Microsoft takes the security of our software products and services seriously, which includes all source code repositories managed through our GitHub organizations, which include [Microsoft](https://github.com/Microsoft), [Azure](https://github.com/Azure), [DotNet](https://github.com/dotnet), [AspNet](https://github.com/aspnet), [Xamarin](https://github.com/xamarin), and [our GitHub organizations](https://opensource.microsoft.com/).
-
-If you believe you have found a security vulnerability in any Microsoft-owned repository that meets [Microsoft's definition of a security vulnerability](https://aka.ms/opensource/security/definition), please report it to us as described below.
-
-## Reporting Security Issues
-
-**Please do not report security vulnerabilities through public GitHub issues.**
-
-Instead, please report them to the Microsoft Security Response Center (MSRC) at [https://msrc.microsoft.com/create-report](https://aka.ms/opensource/security/create-report).
-
-If you prefer to submit without logging in, send email to [secure@microsoft.com](mailto:secure@microsoft.com).  If possible, encrypt your message with our PGP key; please download it from the [Microsoft Security Response Center PGP Key page](https://aka.ms/opensource/security/pgpkey).
-
-You should receive a response within 24 hours. If for some reason you do not, please follow up via email to ensure we received your original message. Additional information can be found at [microsoft.com/msrc](https://aka.ms/opensource/security/msrc). 
-
-Please include the requested information listed below (as much as you can provide) to help us better understand the nature and scope of the possible issue:
-
-  * Type of issue (e.g. buffer overflow, SQL injection, cross-site scripting, etc.)
-  * Full paths of source file(s) related to the manifestation of the issue
-  * The location of the affected source code (tag/branch/commit or direct URL)
-  * Any special configuration required to reproduce the issue
-  * Step-by-step instructions to reproduce the issue
-  * Proof-of-concept or exploit code (if possible)
-  * Impact of the issue, including how an attacker might exploit the issue
-
-This information will help us triage your report more quickly.
-
-If you are reporting for a bug bounty, more complete reports can contribute to a higher bounty award. Please visit our [Microsoft Bug Bounty Program](https://aka.ms/opensource/security/bounty) page for more details about our active programs.
-
-## Preferred Languages
-
-We prefer all communications to be in English.
-
-## Policy
-
-Microsoft follows the principle of [Coordinated Vulnerability Disclosure](https://aka.ms/opensource/security/cvd).
-
-<!-- END MICROSOFT SECURITY.MD BLOCK -->
+<!-- BEGIN MICROSOFT SECURITY.MD V0.0.7 BLOCK -->
+
+## Security
+
+Microsoft takes the security of our software products and services seriously, which includes all source code repositories managed through our GitHub organizations, which include [Microsoft](https://github.com/Microsoft), [Azure](https://github.com/Azure), [DotNet](https://github.com/dotnet), [AspNet](https://github.com/aspnet), [Xamarin](https://github.com/xamarin), and [our GitHub organizations](https://opensource.microsoft.com/).
+
+If you believe you have found a security vulnerability in any Microsoft-owned repository that meets [Microsoft's definition of a security vulnerability](https://aka.ms/opensource/security/definition), please report it to us as described below.
+
+## Reporting Security Issues
+
+**Please do not report security vulnerabilities through public GitHub issues.**
+
+Instead, please report them to the Microsoft Security Response Center (MSRC) at [https://msrc.microsoft.com/create-report](https://aka.ms/opensource/security/create-report).
+
+If you prefer to submit without logging in, send email to [secure@microsoft.com](mailto:secure@microsoft.com).  If possible, encrypt your message with our PGP key; please download it from the [Microsoft Security Response Center PGP Key page](https://aka.ms/opensource/security/pgpkey).
+
+You should receive a response within 24 hours. If for some reason you do not, please follow up via email to ensure we received your original message. Additional information can be found at [microsoft.com/msrc](https://aka.ms/opensource/security/msrc). 
+
+Please include the requested information listed below (as much as you can provide) to help us better understand the nature and scope of the possible issue:
+
+  * Type of issue (e.g. buffer overflow, SQL injection, cross-site scripting, etc.)
+  * Full paths of source file(s) related to the manifestation of the issue
+  * The location of the affected source code (tag/branch/commit or direct URL)
+  * Any special configuration required to reproduce the issue
+  * Step-by-step instructions to reproduce the issue
+  * Proof-of-concept or exploit code (if possible)
+  * Impact of the issue, including how an attacker might exploit the issue
+
+This information will help us triage your report more quickly.
+
+If you are reporting for a bug bounty, more complete reports can contribute to a higher bounty award. Please visit our [Microsoft Bug Bounty Program](https://aka.ms/opensource/security/bounty) page for more details about our active programs.
+
+## Preferred Languages
+
+We prefer all communications to be in English.
+
+## Policy
+
+Microsoft follows the principle of [Coordinated Vulnerability Disclosure](https://aka.ms/opensource/security/cvd).
+
+<!-- END MICROSOFT SECURITY.MD BLOCK -->
```

### Comparing `azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/auth/connection_string.py` & `azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/connection_string.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,105 +1,110 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for
-# license information.
-# --------------------------------------------------------------------------
-"""This module contains tools for working with Connection Strings"""
-
-__all__ = ["ConnectionString"]
-
-CS_DELIMITER = ";"
-CS_VAL_SEPARATOR = "="
-
-HOST_NAME = "HostName"
-SHARED_ACCESS_KEY_NAME = "SharedAccessKeyName"
-SHARED_ACCESS_KEY = "SharedAccessKey"
-SHARED_ACCESS_SIGNATURE = "SharedAccessSignature"
-DEVICE_ID = "DeviceId"
-MODULE_ID = "ModuleId"
-GATEWAY_HOST_NAME = "GatewayHostName"
-X509 = "x509"
-
-_valid_keys = [
-    HOST_NAME,
-    SHARED_ACCESS_KEY_NAME,
-    SHARED_ACCESS_KEY,
-    SHARED_ACCESS_SIGNATURE,
-    DEVICE_ID,
-    MODULE_ID,
-    GATEWAY_HOST_NAME,
-    X509,
-]
-
-
-def _parse_connection_string(connection_string):
-    """Return a dictionary of values contained in a given connection string"""
-    try:
-        cs_args = connection_string.split(CS_DELIMITER)
-    except (AttributeError, TypeError):
-        raise TypeError("Connection String must be of type str")
-    try:
-        d = dict(arg.split(CS_VAL_SEPARATOR, 1) for arg in cs_args)
-    except ValueError:
-        # This occurs in an extreme edge case where a dictionary cannot be formed because there
-        # is only 1 token after the split (dict requires two in order to make a key/value pair)
-        raise ValueError("Invalid Connection String - Unable to parse")
-    if len(cs_args) != len(d):
-        # various errors related to incorrect parsing - duplicate args, bad syntax, etc.
-        raise ValueError("Invalid Connection String - Unable to parse")
-    if not all(key in _valid_keys for key in d.keys()):
-        raise ValueError("Invalid Connection String - Invalid Key")
-    _validate_keys(d)
-    return d
-
-
-def _validate_keys(d):
-    """Raise ValueError if incorrect combination of keys in dict d"""
-    host_name = d.get(HOST_NAME)
-    shared_access_key_name = d.get(SHARED_ACCESS_KEY_NAME)
-    shared_access_key = d.get(SHARED_ACCESS_KEY)
-    device_id = d.get(DEVICE_ID)
-    x509 = d.get(X509)
-
-    if shared_access_key and x509:
-        raise ValueError("Invalid Connection String - Mixed authentication scheme")
-
-    # This logic could be expanded to return the category of ConnectionString
-    if host_name and device_id and (shared_access_key or x509):
-        pass
-    elif host_name and shared_access_key and shared_access_key_name:
-        pass
-    else:
-        raise ValueError("Invalid Connection String - Incomplete")
-
-
-class ConnectionString(object):
-    """Key/value mappings for connection details.
-    Uses the same syntax as dictionary
-    """
-
-    def __init__(self, connection_string):
-        """Initializer for ConnectionString
-
-        :param str connection_string: String with connection details provided by Azure
-        :raises: ValueError if provided connection_string is invalid
-        """
-        self._dict = _parse_connection_string(connection_string)
-        self._strrep = connection_string
-
-    def __getitem__(self, key):
-        return self._dict[key]
-
-    def __repr__(self):
-        return self._strrep
-
-    def get(self, key, default=None):
-        """Return the value for key if key is in the dictionary, else default
-
-        :param str key: The key to retrieve a value for
-        :param str default: The default value returned if a key is not found
-        :returns: The value for the given key
-        """
-        try:
-            return self._dict[key]
-        except KeyError:
-            return default
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License.txt in the project root for
+# license information.
+# --------------------------------------------------------------------------
+"""This module contains tools for working with Connection Strings"""
+
+__all__ = ["ConnectionString"]
+
+CS_DELIMITER = ";"
+CS_VAL_SEPARATOR = "="
+
+HOST_NAME = "HostName"
+SHARED_ACCESS_KEY_NAME = "SharedAccessKeyName"
+SHARED_ACCESS_KEY = "SharedAccessKey"
+SHARED_ACCESS_SIGNATURE = "SharedAccessSignature"
+DEVICE_ID = "DeviceId"
+MODULE_ID = "ModuleId"
+GATEWAY_HOST_NAME = "GatewayHostName"
+X509 = "x509"
+
+_valid_keys = [
+    HOST_NAME,
+    SHARED_ACCESS_KEY_NAME,
+    SHARED_ACCESS_KEY,
+    SHARED_ACCESS_SIGNATURE,
+    DEVICE_ID,
+    MODULE_ID,
+    GATEWAY_HOST_NAME,
+    X509,
+]
+
+# TODO: does this module need revision for V3?
+
+
+class ConnectionString(object):
+    """Key/value mappings for connection details.
+    Uses the same syntax as dictionary
+    """
+
+    def __init__(self, connection_string):
+        """Initializer for ConnectionString
+
+        :param str connection_string: String with connection details provided by Azure
+        :raises: ValueError if provided connection_string is invalid
+        """
+        self._dict = _parse_connection_string(connection_string)
+        self._strrep = connection_string
+
+    def __contains__(self, item):
+        return item in self._dict
+
+    def __getitem__(self, key):
+        return self._dict[key]
+
+    def __repr__(self):
+        return self._strrep
+
+    def get(self, key, default=None):
+        """Return the value for key if key is in the dictionary, else default
+
+        :param str key: The key to retrieve a value for
+        :param str default: The default value returned if a key is not found
+        :returns: The value for the given key
+        """
+        try:
+            return self._dict[key]
+        except KeyError:
+            return default
+
+
+def _parse_connection_string(connection_string):
+    """Return a dictionary of values contained in a given connection string"""
+    try:
+        cs_args = connection_string.split(CS_DELIMITER)
+    except (AttributeError, TypeError):
+        raise TypeError("Connection String must be of type str")
+    try:
+        d = dict(arg.split(CS_VAL_SEPARATOR, 1) for arg in cs_args)
+    except ValueError:
+        # This occurs in an extreme edge case where a dictionary cannot be formed because there
+        # is only 1 token after the split (dict requires two in order to make a key/value pair)
+        raise ValueError("Invalid Connection String - Unable to parse")
+    if len(cs_args) != len(d):
+        # various errors related to incorrect parsing - duplicate args, bad syntax, etc.
+        raise ValueError("Invalid Connection String - Unable to parse")
+    if not all(key in _valid_keys for key in d.keys()):
+        raise ValueError("Invalid Connection String - Invalid Key")
+    _validate_keys(d)
+    return d
+
+
+def _validate_keys(d):
+    """Raise ValueError if incorrect combination of keys in dict d"""
+    host_name = d.get(HOST_NAME)
+    shared_access_key_name = d.get(SHARED_ACCESS_KEY_NAME)
+    shared_access_key = d.get(SHARED_ACCESS_KEY)
+    device_id = d.get(DEVICE_ID)
+    x509 = d.get(X509)
+
+    if shared_access_key and x509 and x509.lower() == "true":
+        raise ValueError("Invalid Connection String - Mixed authentication scheme")
+
+    # This logic could be expanded to return the category of ConnectionString
+    if host_name and device_id and (shared_access_key or x509):
+        pass
+    elif host_name and shared_access_key and shared_access_key_name:
+        pass
+    else:
+        raise ValueError("Invalid Connection String - Incomplete")
```

### Comparing `azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/common/auth/signing_mechanism.py` & `azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/signing_mechanism.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,68 +1,77 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for
-# license information.
-# --------------------------------------------------------------------------
-"""This module defines an abstract SigningMechanism, as well as common child implementations of it
-"""
-import abc
-import hmac
-import hashlib
-import base64
-
-
-class SigningMechanism(abc.ABC):
-    @abc.abstractmethod
-    def sign(self, data_str):
-        pass
-
-
-class SymmetricKeySigningMechanism(SigningMechanism):
-    def __init__(self, key):
-        """
-        A mechanism that signs data using a symmetric key
-
-        :param key: Symmetric Key (base64 encoded)
-        :type key: str or bytes
-        """
-        # Convert key to bytes
-        try:
-            key = key.encode("utf-8")
-        except AttributeError:
-            # If byte string, no need to encode
-            pass
-
-        # Derives the signing key
-        # CT-TODO: is "signing key" the right term?
-        try:
-            self._signing_key = base64.b64decode(key)
-        except (base64.binascii.Error):
-            raise ValueError("Invalid Symmetric Key")
-
-    def sign(self, data_str):
-        """
-        Sign a data string with symmetric key and the HMAC-SHA256 algorithm.
-
-        :param data_str: Data string to be signed
-        :type data_str: str or bytes
-
-        :returns: The signed data
-        :rtype: str
-        """
-        # Convert data_str to bytes
-        try:
-            data_str = data_str.encode("utf-8")
-        except AttributeError:
-            # If byte string, no need to encode
-            pass
-
-        # Derive signature via HMAC-SHA256 algorithm
-        try:
-            hmac_digest = hmac.HMAC(
-                key=self._signing_key, msg=data_str, digestmod=hashlib.sha256
-            ).digest()
-            signed_data = base64.b64encode(hmac_digest)
-        except (TypeError):
-            raise ValueError("Unable to sign string using the provided symmetric key")
-        # Convert from bytes to string
-        return signed_data.decode("utf-8")
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License.txt in the project root for
+# license information.
+# --------------------------------------------------------------------------
+import abc
+import base64
+import binascii
+import hmac
+import hashlib
+from typing import AnyStr
+
+# TODO: remove commented signatures
+
+
+class SigningMechanism(abc.ABC):
+    @abc.abstractmethod
+    async def sign(self, data_str: AnyStr) -> str:
+        # NOTE: This is defined as a coroutine to allow for flexibility of implementation.
+        # Some implementations may not require a coroutine, but others may, so we err on the side
+        # of a coroutine for consistent interface.
+        pass
+
+
+class SymmetricKeySigningMechanism(SigningMechanism):
+    def __init__(self, key: AnyStr) -> None:
+        """
+        A mechanism that signs data using a symmetric key
+
+        :param key: Symmetric Key (base64 encoded)
+        :type key: str or bytes
+
+        :raises: ValueError if provided key is invalid
+        """
+        # Convert key to bytes (if not already)
+        if isinstance(key, str):
+            key_bytes = key.encode("utf-8")
+        else:
+            key_bytes = key
+
+        # Derives the signing key
+        try:
+            self._signing_key = base64.b64decode(key_bytes)
+        except (binascii.Error):
+            raise ValueError("Invalid Symmetric Key")
+
+    async def sign(self, data_str: AnyStr) -> str:
+        """
+        Sign a data string with symmetric key and the HMAC-SHA256 algorithm.
+
+        :param data_str: Data string to be signed
+        :type data_str: str or bytes
+
+        :returns: The signed data
+        :rtype: str
+
+        :raises: ValueError if an invalid data string is provided
+        """
+        # NOTE: This implementation doesn't take advantage of being a coroutine, but this is by
+        # design. See the definition of the abstract base class above.
+
+        # Convert data_str to bytes (if not already)
+        if isinstance(data_str, str):
+            data_bytes = data_str.encode("utf-8")
+        else:
+            data_bytes = data_str
+
+        # Derive signature via HMAC-SHA256 algorithm
+        try:
+            hmac_digest = hmac.HMAC(
+                key=self._signing_key, msg=data_bytes, digestmod=hashlib.sha256
+            ).digest()
+            signed_data = base64.b64encode(hmac_digest)
+        except (TypeError):
+            raise ValueError("Unable to sign string using the provided symmetric key")
+        # Convert from bytes to string
+        return signed_data.decode("utf-8")
```

### Comparing `azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/constant.py` & `azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/constant.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """This module defines constants for use across the azure-iot-device package
 """
 
-VERSION = "3.0.0b1"
+VERSION = "3.0.0b2"
 IOTHUB_IDENTIFIER = "azure-iot-device-iothub-py"
 PROVISIONING_IDENTIFIER = "azure-iot-device-provisioning-py"
-IOTHUB_API_VERSION = "2019-10-01"
+IOTHUB_API_VERSION = "2020-09-30"
 PROVISIONING_API_VERSION = "2019-03-31"
 SECURITY_MESSAGE_INTERFACE_ID = "urn:azureiot:Security:SecurityAgent:1"
+
+# TODO: find somewhere else for this
 TELEMETRY_MESSAGE_SIZE_LIMIT = 262144
-# The max keep alive is determined by the load balancer currently.
-MAX_KEEP_ALIVE_SECS = 1740
+
 # Everything in digital twin is defined here
 # as things are extremely dynamic and subject to sudden changes
 DIGITAL_TWIN_PREFIX = "dtmi"
-DIGITAL_TWIN_API_VERSION = "2020-09-30"
 DIGITAL_TWIN_QUERY_HEADER = "model-id"
```

### Comparing `azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/edge_hsm.py` & `azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/edge_hsm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,160 +1,167 @@
-# --------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-import logging
-import json
-import base64
-import requests
-import requests_unixsocket
-import urllib
-from azure.iot.device.common.auth.signing_mechanism import SigningMechanism
-from azure.iot.device import user_agent
-
-requests_unixsocket.monkeypatch()
-logger = logging.getLogger(__name__)
-
-
-class IoTEdgeError(Exception):
-    pass
-
-
-class IoTEdgeHsm(SigningMechanism):
-    """
-    Constructor for instantiating a iot hsm object.  This is an object that
-    communicates with the Azure IoT Edge HSM in order to get connection credentials
-    for an Azure IoT Edge module.  The credentials that this object return come in
-    two forms:
-
-    1. The trust bundle, which is a certificate that can be used as a trusted cert
-       to authenticate the SSL connection between the IoE Edge module and IoT Edge
-    2. A signing function, which can be used to create the sig field for a
-       SharedAccessSignature string which can be used to authenticate with Iot Edge
-    """
-
-    def __init__(self, module_id, generation_id, workload_uri, api_version):
-        """
-        Constructor for instantiating a Azure IoT Edge HSM object
-
-        :param str module_id: The module id
-        :param str api_version: The API version
-        :param str generation_id: The module generation id
-        :param str workload_uri: The workload uri
-        """
-        self.module_id = urllib.parse.quote(module_id, safe="")
-        self.api_version = api_version
-        self.generation_id = generation_id
-        self.workload_uri = _format_socket_uri(workload_uri)
-
-    def get_certificate(self):
-        """
-        Return the server verification certificate from the trust bundle that can be used to
-        validate the server-side SSL TLS connection that we use to talk to Edge
-
-        :return: The server verification certificate to use for connections to the Azure IoT Edge
-        instance, as a PEM certificate in string form.
-
-        :raises: IoTEdgeError if unable to retrieve the certificate.
-        """
-        r = requests.get(
-            self.workload_uri + "trust-bundle",
-            params={"api-version": self.api_version},
-            headers={"User-Agent": urllib.parse.quote_plus(user_agent.get_iothub_user_agent())},
-        )
-        # Validate that the request was successful
-        try:
-            r.raise_for_status()
-        except requests.exceptions.HTTPError as e:
-            raise IoTEdgeError("Unable to get trust bundle from Edge") from e
-        # Decode the trust bundle
-        try:
-            bundle = r.json()
-        except ValueError as e:
-            raise IoTEdgeError("Unable to decode trust bundle") from e
-        # Retrieve the certificate
-        try:
-            cert = bundle["certificate"]
-        except KeyError as e:
-            raise IoTEdgeError("No certificate in trust bundle") from e
-        return cert
-
-    def sign(self, data_str):
-        """
-        Use the IoTEdge HSM to sign a piece of string data.  The caller should then insert the
-        returned value (the signature) into the 'sig' field of a SharedAccessSignature string.
-
-        :param str data_str: The data string to sign
-
-        :return: The signature, as a URI-encoded and base64-encoded value that is ready to
-        directly insert into the SharedAccessSignature string.
-
-        :raises: IoTEdgeError if unable to sign the data.
-        """
-        encoded_data_str = base64.b64encode(data_str.encode("utf-8")).decode()
-
-        path = "{workload_uri}modules/{module_id}/genid/{gen_id}/sign".format(
-            workload_uri=self.workload_uri, module_id=self.module_id, gen_id=self.generation_id
-        )
-        sign_request = {"keyId": "primary", "algo": "HMACSHA256", "data": encoded_data_str}
-
-        r = requests.post(  # can we use json field instead of data?
-            url=path,
-            params={"api-version": self.api_version},
-            headers={"User-Agent": urllib.parse.quote(user_agent.get_iothub_user_agent(), safe="")},
-            data=json.dumps(sign_request),
-        )
-        try:
-            r.raise_for_status()
-        except requests.exceptions.HTTPError as e:
-            raise IoTEdgeError("Unable to sign data") from e
-        try:
-            sign_response = r.json()
-        except ValueError as e:
-            raise IoTEdgeError("Unable to decode signed data") from e
-        try:
-            signed_data_str = sign_response["digest"]
-        except KeyError as e:
-            raise IoTEdgeError("No signed data received") from e
-
-        return signed_data_str  # what format is this? string? bytes?
-
-
-def _format_socket_uri(old_uri):
-    """
-    This function takes a socket URI in one form and converts it into another form.
-
-    The source form is based on what we receive inside the IOTEDGE_WORKLOADURI
-    environment variable, and it looks like this:
-    "unix:///var/run/iotedge/workload.sock"
-
-    The destination form is based on what the requests_unixsocket library expects
-    and it looks like this:
-    "http+unix://%2Fvar%2Frun%2Fiotedge%2Fworkload.sock/"
-
-    The function changes the prefix, uri-encodes the path, and adds a slash
-    at the end.
-
-    If the socket URI does not start with unix:// this function only adds
-    a slash at the end.
-
-    :param old_uri: The URI in IOTEDGE_WORKLOADURI form
-
-    :return: The URI in requests_unixsocket form
-    """
-    old_prefix = "unix://"
-    new_prefix = "http+unix://"
-
-    if old_uri.startswith(old_prefix):
-        stripped_uri = old_uri[len(old_prefix) :]
-        if stripped_uri.endswith("/"):
-            stripped_uri = stripped_uri[:-1]
-        new_uri = new_prefix + urllib.parse.quote(stripped_uri, safe="")
-    else:
-        new_uri = old_uri
-
-    if not new_uri.endswith("/"):
-        new_uri += "/"
-
-    return new_uri
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License.txt in the project root for
+# license information.
+# --------------------------------------------------------------------------
+import base64
+import logging
+import json
+import requests  # type: ignore
+import requests_unixsocket  # type: ignore
+import urllib.parse
+from typing import Union
+from . import user_agent
+from .iot_exceptions import IoTEdgeError
+from .signing_mechanism import SigningMechanism
+
+requests_unixsocket.monkeypatch()
+logger = logging.getLogger(__name__)
+
+
+class IoTEdgeHsm(SigningMechanism):
+    """
+    Constructor for instantiating a iot hsm object.  This is an object that
+    communicates with the Azure IoT Edge HSM in order to get connection credentials
+    for an Azure IoT Edge module.  The credentials that this object return come in
+    two forms:
+
+    1. The trust bundle, which is a certificate that can be used as a trusted cert
+       to authenticate the SSL connection between the IoE Edge module and IoT Edge
+    2. A signing function, which can be used to create the sig field for a
+       SharedAccessSignature string which can be used to authenticate with Iot Edge
+    """
+
+    def __init__(
+        self, module_id: str, generation_id: str, workload_uri: str, api_version: str
+    ) -> None:
+        """
+        Constructor for instantiating a Azure IoT Edge HSM object
+
+        :param str module_id: The module id
+        :param str api_version: The API version
+        :param str generation_id: The module generation id
+        :param str workload_uri: The workload uri
+        """
+        self.module_id = urllib.parse.quote(module_id, safe="")
+        self.api_version = api_version
+        self.generation_id = generation_id
+        self.workload_uri = _format_socket_uri(workload_uri)
+
+    # TODO: Use async http to make use of this being a coroutine
+    async def get_certificate(self) -> str:
+        """
+        Return the server verification certificate from the trust bundle that can be used to
+        validate the server-side SSL TLS connection that we use to talk to Edge
+
+        :return: The server verification certificate to use for connections to the Azure IoT Edge
+        instance, as a PEM certificate in string form.
+
+        :raises: IoTEdgeError if unable to retrieve the certificate.
+        """
+        r = requests.get(
+            self.workload_uri + "trust-bundle",
+            params={"api-version": self.api_version},
+            headers={"User-Agent": urllib.parse.quote_plus(user_agent.get_iothub_user_agent())},
+        )
+        # Validate that the request was successful
+        try:
+            r.raise_for_status()
+        except requests.exceptions.HTTPError as e:
+            raise IoTEdgeError("Unable to get trust bundle from Edge") from e
+        # Decode the trust bundle
+        try:
+            bundle = r.json()
+        except ValueError as e:
+            raise IoTEdgeError("Unable to decode trust bundle") from e
+        # Retrieve the certificate
+        try:
+            cert = bundle["certificate"]
+        except KeyError as e:
+            raise IoTEdgeError("No certificate in trust bundle") from e
+        return cert
+
+    # TODO: Use async http to make use of this being a coroutine
+    async def sign(self, data_str: Union[str, bytes]) -> str:
+        """
+        Use the IoTEdge HSM to sign a piece of string data.  The caller should then insert the
+        returned value (the signature) into the 'sig' field of a SharedAccessSignature string.
+
+        :param str data_str: The data string to sign
+
+        :return: The signature, as a URI-encoded and base64-encoded value that is ready to
+        directly insert into the SharedAccessSignature string.
+
+        :raises: IoTEdgeError if unable to sign the data.
+        """
+        # Convert data_str to bytes (if not already)
+        if isinstance(data_str, str):
+            data_bytes = data_str.encode("utf-8")
+        else:
+            data_bytes = data_str
+
+        encoded_data_str = base64.b64encode(data_bytes).decode()
+
+        path = "{workload_uri}modules/{module_id}/genid/{gen_id}/sign".format(
+            workload_uri=self.workload_uri, module_id=self.module_id, gen_id=self.generation_id
+        )
+        sign_request = {"keyId": "primary", "algo": "HMACSHA256", "data": encoded_data_str}
+
+        r = requests.post(  # can we use json field instead of data?
+            url=path,
+            params={"api-version": self.api_version},
+            headers={"User-Agent": urllib.parse.quote(user_agent.get_iothub_user_agent(), safe="")},
+            data=json.dumps(sign_request),
+        )
+        try:
+            r.raise_for_status()
+        except requests.exceptions.HTTPError as e:
+            raise IoTEdgeError("Unable to sign data") from e
+        try:
+            sign_response = r.json()
+        except ValueError as e:
+            raise IoTEdgeError("Unable to decode signed data") from e
+        try:
+            signed_data_str = sign_response["digest"]
+        except KeyError as e:
+            raise IoTEdgeError("No signed data received") from e
+
+        return signed_data_str  # what format is this? string? bytes?
+
+
+def _format_socket_uri(old_uri: str) -> str:
+    """
+    This function takes a socket URI in one form and converts it into another form.
+
+    The source form is based on what we receive inside the IOTEDGE_WORKLOADURI
+    environment variable, and it looks like this:
+    "unix:///var/run/iotedge/workload.sock"
+
+    The destination form is based on what the requests_unixsocket library expects
+    and it looks like this:
+    "http+unix://%2Fvar%2Frun%2Fiotedge%2Fworkload.sock/"
+
+    The function changes the prefix, uri-encodes the path, and adds a slash
+    at the end.
+
+    If the socket URI does not start with unix:// this function only adds
+    a slash at the end.
+
+    :param old_uri: The URI in IOTEDGE_WORKLOADURI form
+
+    :return: The URI in requests_unixsocket form
+    """
+    old_prefix = "unix://"
+    new_prefix = "http+unix://"
+
+    if old_uri.startswith(old_prefix):
+        stripped_uri = old_uri[len(old_prefix) :]
+        if stripped_uri.endswith("/"):
+            stripped_uri = stripped_uri[:-1]
+        new_uri = new_prefix + urllib.parse.quote(stripped_uri, safe="")
+    else:
+        new_uri = old_uri
+
+    if not new_uri.endswith("/"):
+        new_uri += "/"
+
+    return new_uri
```

### Comparing `azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/iothub/pipeline/http_path_iothub.py` & `azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/http_path_iothub.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-# --------------------------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-import logging
-import urllib
-
-logger = logging.getLogger(__name__)
-
-
-def get_method_invoke_path(device_id, module_id=None):
-    """
-    :return: The path for invoking methods from one module to a device or module. It is of the format
-    twins/uri_encode($device_id)/modules/uri_encode($module_id)/methods
-    """
-    if module_id:
-        return "twins/{device_id}/modules/{module_id}/methods".format(
-            device_id=urllib.parse.quote_plus(device_id),
-            module_id=urllib.parse.quote_plus(module_id),
-        )
-    else:
-        return "twins/{device_id}/methods".format(device_id=urllib.parse.quote_plus(device_id))
-
-
-def get_storage_info_for_blob_path(device_id):
-    """
-    This does not take a module_id since get_storage_info_for_blob_path should only ever be invoked on device clients.
-
-    :return: The path for getting the storage sdk credential information from IoT Hub. It is of the format
-    devices/uri_encode($device_id)/files
-    """
-    return "devices/{}/files".format(urllib.parse.quote_plus(device_id))
-
-
-def get_notify_blob_upload_status_path(device_id):
-    """
-    This does not take a module_id since get_notify_blob_upload_status_path should only ever be invoked on device clients.
-
-    :return: The path for getting the storage sdk credential information from IoT Hub. It is of the format
-    devices/uri_encode($device_id)/files/notifications
-    """
-    return "devices/{}/files/notifications".format(urllib.parse.quote_plus(device_id))
+# --------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License.txt in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+import logging
+import urllib
+from typing import Optional
+
+logger = logging.getLogger(__name__)
+
+
+def get_direct_method_invoke_path(device_id: str, module_id: Optional[str] = None) -> str:
+    """
+    :return: The relative path for invoking methods from one module to a device or module. It is of the format
+    /twins/uri_encode($device_id)/modules/uri_encode($module_id)/methods
+    """
+    if module_id:
+        return "/twins/{device_id}/modules/{module_id}/methods".format(
+            device_id=urllib.parse.quote_plus(device_id),
+            module_id=urllib.parse.quote_plus(module_id),
+        )
+    else:
+        return "/twins/{device_id}/methods".format(device_id=urllib.parse.quote_plus(device_id))
+
+
+def get_storage_info_for_blob_path(device_id: str):
+    """
+    This does not take a module_id since get_storage_info_for_blob_path should only ever be invoked on device clients.
+
+    :return: The relative path for getting the storage sdk credential information from IoT Hub. It is of the format
+    /devices/uri_encode($device_id)/files
+    """
+    return "/devices/{}/files".format(urllib.parse.quote_plus(device_id))
+
+
+def get_notify_blob_upload_status_path(device_id: str):
+    """
+    This does not take a module_id since get_notify_blob_upload_status_path should only ever be invoked on device clients.
+
+    :return: The relative path for getting the storage sdk credential information from IoT Hub. It is of the format
+    /devices/uri_encode($device_id)/files/notifications
+    """
+    return "/devices/{}/files/notifications".format(urllib.parse.quote_plus(device_id))
```

### Comparing `azure-iot-device-3.0.0b1/azure-iot-device/azure/iot/device/user_agent.py` & `azure-iot-device-3.0.0b2/azure-iot-device/azure/iot/device/user_agent.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for
-# license information.
-# --------------------------------------------------------------------------
-"""This module is for creating agent strings for all clients"""
-
-import platform
-from azure.iot.device.constant import VERSION, IOTHUB_IDENTIFIER, PROVISIONING_IDENTIFIER
-
-python_runtime = platform.python_version()
-os_type = platform.system()
-os_release = platform.version()
-architecture = platform.machine()
-
-
-def _get_common_user_agent():
-    return "({python_runtime};{os_type} {os_release};{architecture})".format(
-        python_runtime=python_runtime,
-        os_type=os_type,
-        os_release=os_release,
-        architecture=architecture,
-    )
-
-
-def get_iothub_user_agent():
-    """
-    Create the user agent for IotHub
-    """
-    return "{iothub_iden}/{version}{common}".format(
-        iothub_iden=IOTHUB_IDENTIFIER, version=VERSION, common=_get_common_user_agent()
-    )
-
-
-def get_provisioning_user_agent():
-    """
-    Create the user agent for Provisioning
-    """
-    return "{provisioning_iden}/{version}{common}".format(
-        provisioning_iden=PROVISIONING_IDENTIFIER, version=VERSION, common=_get_common_user_agent()
-    )
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License.txt in the project root for
+# license information.
+# --------------------------------------------------------------------------
+"""This module is for creating agent strings for all clients"""
+
+import platform
+from .constant import VERSION, IOTHUB_IDENTIFIER, PROVISIONING_IDENTIFIER
+
+python_runtime = platform.python_version()
+os_type = platform.system()
+os_release = platform.version()
+architecture = platform.machine()
+
+
+def _get_common_user_agent() -> str:
+    return "({python_runtime};{os_type} {os_release};{architecture})".format(
+        python_runtime=python_runtime,
+        os_type=os_type,
+        os_release=os_release,
+        architecture=architecture,
+    )
+
+
+def get_iothub_user_agent() -> str:
+    """
+    Create the user agent for IotHub
+    """
+    return "{iothub_iden}/{version}{common}".format(
+        iothub_iden=IOTHUB_IDENTIFIER, version=VERSION, common=_get_common_user_agent()
+    )
+
+
+def get_provisioning_user_agent() -> str:
+    """
+    Create the user agent for Provisioning
+    """
+    return "{provisioning_iden}/{version}{common}".format(
+        provisioning_iden=PROVISIONING_IDENTIFIER, version=VERSION, common=_get_common_user_agent()
+    )
```

### Comparing `azure-iot-device-3.0.0b1/azure-iot-device/azure_iot_device.egg-info/PKG-INFO` & `azure-iot-device-3.0.0b2/azure-iot-device/azure_iot_device.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,126 +1,99 @@
 Metadata-Version: 2.1
 Name: azure-iot-device
-Version: 3.0.0b1
+Version: 3.0.0b2
 Summary: Microsoft Azure IoT Device Library
 Home-page: https://github.com/Azure/azure-iot-sdk-python/tree/v3
 Author: Microsoft Corporation
 Author-email: opensource@microsoft.com
 License: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.6, <4
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 #
 <div align=center>
     <img src="./doc/images/azure_iot_sdk_python_banner.png"></img>
     <h1> azure-iot-device </h1>
 </div>
 
 ![Build Status](https://azure-iot-sdks.visualstudio.com/azure-iot-sdks/_apis/build/status/Azure.azure-iot-sdk-python)
 
 The Azure IoT Device SDK for Python enables Python developers to easily create IoT device solutions that seamlessly connect to the Azure IoT Hub ecosystem.
 
-* *If you're looking for the azure-iot-hub library, it is now located in the [azure-iot-hub-python](https://github.com/Azure/azure-iot-hub-python) repository*
+* *If you're migrating v2.x.x code to use v3.x.x check the [IoT Hub Migration Guide](https://github.com/Azure/azure-iot-sdk-python/blob/main/migration_guide_iothub.md) and/or the [Provisioning Migration Guide](https://github.com/Azure/azure-iot-sdk-python/blob/main/migration_guide_provisioning.md)*
+
+* *If you're looking for the v2.x.x client library, it is now preserved in the [v2](https://github.com/Azure/azure-iot-sdk-python/tree/v2) branch*
 
 * *If you're looking for the v1.x.x client library, it is now preserved in the [v1-deprecated](https://github.com/Azure/azure-iot-sdk-python/tree/v1-deprecated) branch.*
 
+* *If you're looking for the azure-iot-hub library, it is now located in the [azure-iot-hub-python](https://github.com/Azure/azure-iot-hub-python) repository*
+
+**NOTE: 3.x.x is still in beta and APIs are subject to change until the release of 3.0.0**
+
 
 ## Installing the library
 
 The Azure IoT Device library is available on PyPI:
 
 ```Shell
-pip install azure-iot-device
+pip install azure-iot-device==3.0.0b2
 ```
 
-Python 3.6 or higher is required in order to use the library
+Python 3.7 or higher is required in order to use the library
 
-## Using the library
-API documentation for this package is available via [**Microsoft Docs**](https://docs.microsoft.com/python/api/azure-iot-device/azure.iot.device?view=azure-python).
-
-See our [**quickstart guide**](https://github.com/Azure/azure-iot-sdk-python/tree/main/samples/README.md) for step by step instructions for setting up and using an IoTHub with devices. 
 
-You can also view the [**samples repository**](https://github.com/Azure/azure-iot-sdk-python/tree/main/samples) to see additional examples of basic client usage.
+## Using the library
+You can view the [**samples repository**](https://github.com/Azure/azure-iot-sdk-python/tree/main/samples) to see examples of SDK usage.
 
-Want to start off on the right foot? Be sure to learn about [**common pitfalls**](https://github.com/Azure/azure-iot-sdk-python/wiki/pitfalls) of using this Python SDK before starting a project.  
+Full API documentation for this package is available via [**Microsoft Docs**](https://docs.microsoft.com/python/api/azure-iot-device/azure.iot.device?view=azure-python). Note that this documentation may currently be out of date as v3.x.x is still in preview at the time of this writing.
 
 
 ## Features
 
 :heavy_check_mark: feature available  :heavy_multiplication_x: feature planned but not yet supported  :heavy_minus_sign: no support planned*
 
 *Features that are not planned may be prioritized in a future release, but are not currently planned
 
-These clients only support the **MQTT protocol**.
+This library primarily uses the **MQTT protocol**.
 
-### IoTHub Device Client
+### IoTHubSession
 
 | Features                                                                                                         | Status                     | Description                                                                                                                                                                                                          |
 |------------------------------------------------------------------------------------------------------------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | [Authentication](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-security-deployment)                     | :heavy_check_mark:         | Connect your device to IoT Hub securely with supported authentication, including symmetric key, X-509 Self Signed, Certificate Authority (CA) Signed, and SASToken                                     |
 | [Send device-to-cloud message](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-d2c)     | :heavy_check_mark:         | Send device-to-cloud messages (max 256KB) to IoT Hub with the option to add custom properties.                                                                                                                       |
 | [Receive cloud-to-device messages](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-c2d) | :heavy_check_mark:         | Receive cloud-to-device messages and read associated custom and system properties from IoT Hub.                                                        |
 | [Device Twins](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-device-twins)                     | :heavy_check_mark:         | IoT Hub persists a device twin for each device that you connect to IoT Hub.  The device can perform operations like get twin tags, subscribe to desired properties.                                                |
 | [Direct Methods](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-direct-methods)                 | :heavy_check_mark:         | IoT Hub gives you the ability to invoke direct methods on devices from the cloud.  The SDK supports handler for method specific and generic operation.                                                            |
-| [Connection Status and Error reporting](https://docs.microsoft.com/en-us/rest/api/iothub/common-error-codes)     | :heavy_check_mark:   | Error reporting for IoT Hub supported error code.                                                                                         |
-| Connection Retry                                                                                                   | :heavy_check_mark:         | Dropped connections will be retried with a fixed 10 second interval by default. This functionality can be disabled if desired, and the interval can be configured   |
-| [Upload file to Blob](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-file-upload)               | :heavy_check_mark:         | A device can initiate a file upload and notifies IoT Hub when the upload is complete.  |
-
-### IoTHub Module Client
-
-**Note:** IoT Edge for Python is scoped to Linux containers & devices only. [Learn more](https://techcommunity.microsoft.com/t5/internet-of-things/linux-modules-with-azure-iot-edge-on-windows-10-iot-enterprise/ba-p/1407066) about using Linux containers for IoT edge on Windows devices. 
-
-| Features                                                                                                         | Status                     | Description                                                                                                                                                                                                          |
-|------------------------------------------------------------------------------------------------------------------|----------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| [Authentication](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-security-deployment)                     | :heavy_check_mark:         | Connect your device to IoT Hub securely with supported authentication, including symmetric key, X-509 Self Signed, and Certificate Authority (CA) Signed. SASToken authentication is not currently supported.                                                   |
-| [Send device-to-cloud message](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-d2c)     | :heavy_check_mark:         | Send device-to-cloud messages (max 256KB) to IoT Hub with the option to add custom properties.                                                                                                                       |
-| [Receive cloud-to-device messages](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-messages-c2d) | :heavy_check_mark:         | Receive cloud-to-device messages and read associated custom and system properties from IoT Hub, with the option to complete/reject/abandon C2D messages.                                                        |
-| [Device Twins](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-device-twins)                     | :heavy_check_mark:         | IoT Hub persists a device twin for each device that you connect to IoT Hub.  The device can perform operations like get twin tags, subscribe to desired properties.                                                |
-| [Direct Methods](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-direct-methods)                 | :heavy_check_mark:         | IoT Hub gives you the ability to invoke direct methods on devices from the cloud.  The SDK supports handler for method specific and generic operation.                                                            |
-| [Connection Status and Error reporting](https://docs.microsoft.com/en-us/rest/api/iothub/common-error-codes)     | :heavy_check_mark:   | Error reporting for IoT Hub supported error code.                                                                                         |
-| Connection Retry                                                                                                   | :heavy_check_mark:         | Dropped connections will be retried with a fixed 10 second interval.  TThis functionality can be disabled if desired, and the interval can be configured            |
-| Direct Invocation of Method on Modules                                                                           | :heavy_check_mark:         | Invoke method calls to another module using using the Edge Gateway.                                                                                                                                        |
-
-### Provisioning Device Client
-
-| Features                    | Status             | Description                                                                                                                                                                                                                                                                                                                                        |
-|-----------------------------|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| TPM Individual Enrollment   | :heavy_minus_sign: | Provisioning via [Trusted Platform Module](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#trusted-platform-module-tpm).                                                                                                                                                                                                          |
-| X.509 Individual Enrollment | :heavy_check_mark: | Provisioning via [X.509 root certificate](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#root-certificate).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_x509.py) folder and this [quickstart](https://docs.microsoft.com/en-us/azure/iot-dps/quick-create-simulated-device-x509-python) on how to create a device client.   |
-| X.509 Enrollment Group      | :heavy_check_mark: | Provisioning via [X.509 leaf certificate](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#leaf-certificate)).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_x509.py) folder on how to create a device client.                                                                                                                  |
-| Symmetric Key Enrollment    | :heavy_check_mark: | Provisioning via [Symmetric key attestation](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-symmetric-key-attestation)).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_symmetric_key.py) folder on how to create a device client.                                                                                                               |
-
-## Critical Upcoming Changes Notice
-
-### Certificates
-All Azure IoT SDK users are advised to be aware of upcoming TLS certificate changes for Azure IoT Hub and Device Provisioning Service 
-that will impact the SDK's ability to connect to these services. In October 2022, both services will migrate from the current 
-[Baltimore CyberTrust CA Root](https://baltimore-cybertrust-root.chain-demos.digicert.com/info/index.html) to the 
-[DigiCert Global G2 CA root](https://global-root-g2.chain-demos.digicert.com/info/index.html). There will be a 
-transition period beforehand where your IoT devices must have both the Baltimore and Digicert public certificates 
-installed in their certificate store in order to prevent connectivity issues.
-
-**Devices with only the Baltimore public certificate installed will lose the ability to connect to Azure IoT hub and Device Provisioning Service in October 2022.**
+| [Connection Status and Error reporting](https://docs.microsoft.com/en-us/rest/api/iothub/common-error-codes)     | :heavy_check_mark:         | Error reporting for IoT Hub supported error code.                                                                                         |
+| Connection Retry                                                                                                 | :heavy_check_mark:         | Dropped connections will be retried with a fixed 10 second interval by default. This functionality can be disabled if desired, and the interval can be configured   |
+| [Upload file to Blob](https://docs.microsoft.com/en-us/azure/iot-hub/iot-hub-devguide-file-upload)               | :heavy_multiplication_x:   | A device can initiate a file upload and notifies IoT Hub when the upload is complete.  |
+| Direct Invocation of Method on Modules                                                                           | :heavy_multiplication_x:   | Invoke method calls to another module using using the Edge Gateway.         
 
-To prepare for this change, make sure your device's certificate store has both of these public certificates installed.
 
-For a more in depth explanation as to why the IoT services are doing this, please see
-[this article](https://techcommunity.microsoft.com/t5/internet-of-things/azure-iot-tls-critical-changes-are-almost-here-and-why-you/ba-p/2393169).
+### ProvisioningSession
+
+| Features                    | Status                   | Description                                                                                                                                                                                                                                                                                                                                        |
+|-----------------------------|--------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| TPM Individual Enrollment   | :heavy_multiplication_x: | Provisioning via [Trusted Platform Module](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#trusted-platform-module-tpm).                                                                                                                                                                                                          |
+| X.509 Individual Enrollment | :heavy_check_mark:       | Provisioning via [X.509 root certificate](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#root-certificate).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_x509.py) folder and this [quickstart](https://docs.microsoft.com/en-us/azure/iot-dps/quick-create-simulated-device-x509-python) on how to create a device client.   |
+| X.509 Enrollment Group      | :heavy_check_mark:       | Provisioning via [X.509 leaf certificate](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-security#leaf-certificate)).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_x509.py) folder on how to create a device client.                                                                                                                  |
+| Symmetric Key Enrollment    | :heavy_check_mark:       | Provisioning via [Symmetric key attestation](https://docs.microsoft.com/en-us/azure/iot-dps/concepts-symmetric-key-attestation)).  Please review the [samples](azure-iot-device/samples/async-hub-scenarios/provision_symmetric_key.py) folder on how to create a device client.                                                                                                               |
 
 
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.microsoft.com.
```

### Comparing `azure-iot-device-3.0.0b1/devbox_setup.md` & `azure-iot-device-3.0.0b2/devbox_setup.md`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-# Prepare your development environment
-
-This document describes how to prepare your development environment to work with the Microsoft Azure IoT Device SDK for Python
-
-## End User
-If you are simply using the Microsoft Azure IoT SDK for Python as an end user and do not need to modify the code itself, you can simply install the package via `pip` as follows:
-
-```
-pip install azure-iot-device
-```
-
-## IoT Device SDK developer
-If you are going to be modifying the codebase (likely because you are working as a developer on the Microsoft Azure IoT Device SDK for Python) you will need a few extras. Thankfully, you can prepare your development environment simply by running the following command **from the root**:
-
-```
-python scripts/env_setup.py
-```
-
-This will install not only relevant development and test dependencies, but also an editable install of the source code, which can then have any code changes immediately reflected in the install.
-
-It is recommended to use [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/install.html) for Unix-based platforms or [virtualenvwrapper-win](https://github.com/davidmarble/virtualenvwrapper-win) for Windows, in order to easily manage custom environments and switch Python versions, however this is optional.
-
-## Sample Environment Variables (Optional)
-
-If you wish to follow the samples exactly as written, you will need to set some environment variables on your system. These are not required however - if you wish to use different environment variables, or no environment variables at all, simply change the samples to retrieve these values from elsewhere. Additionally, different samples use different variables, so you would only need the ones relevant to samples you intend to use.
-
-### Connection String Device Authentication
-* **IOTHUB_DEVICE_CONNECTION_STRING**: The connection string for your IoTHub Device, which can be found in the Azure Portal
-
-### X509 Authentication
-* **X509_CERT_FILE**: The path to the X509 certificate
-* **X509_KEY_FILE**: The path to the X509 key
-* **X509_PASS_PHRASE**: The pass phrase for the X509 key (Only necessary if cert has a password)
-
-**This is an incomplete list of environment variables**
-
-
-## E2E Testing Setup (Optional - SDK Developer)
-
-If you wish to run end to end tests locally, you'll need to configure some additional environment variables:
-
-* **IOTHUB_CONNECTION_STRING**: The connection string for your IoTHub (ideally iothubowner permissions)
-* **EVENTHUB_CONNECTION_STRING**: The built-in Event Hub compatible endpoint of the above IoTHub
-
-**NOTE**: if you wish to use dedicated E2E resources, you may also prefix the above variables with `IOTHUB_E2E_`
-
-Additionally, you will need to add a messaging route with the following settings to the IoTHub in order for all tests to run correctly:
-* Name: twin
-* Endpoint: events
-* Data Source: Device Twin Change Events
+# Prepare your development environment
+
+This document describes how to prepare your development environment to work with the Microsoft Azure IoT Device SDK for Python
+
+## End User
+If you are simply using the Microsoft Azure IoT SDK for Python as an end user and do not need to modify the code itself, you can simply install the package via `pip` as follows:
+
+```
+pip install azure-iot-device
+```
+
+## IoT Device SDK developer
+If you are going to be modifying the codebase (likely because you are working as a developer on the Microsoft Azure IoT Device SDK for Python) you will need a few extras. Thankfully, you can prepare your development environment simply by running the following command **from the root**:
+
+```
+python scripts/env_setup.py
+```
+
+This will install not only relevant development and test dependencies, but also an editable install of the source code, which can then have any code changes immediately reflected in the install.
+
+It is recommended to use [virtualenvwrapper](https://virtualenvwrapper.readthedocs.io/en/latest/install.html) for Unix-based platforms or [virtualenvwrapper-win](https://github.com/davidmarble/virtualenvwrapper-win) for Windows, in order to easily manage custom environments and switch Python versions, however this is optional.
+
+## Sample Environment Variables (Optional)
+
+If you wish to follow the samples exactly as written, you will need to set some environment variables on your system. These are not required however - if you wish to use different environment variables, or no environment variables at all, simply change the samples to retrieve these values from elsewhere. Additionally, different samples use different variables, so you would only need the ones relevant to samples you intend to use.
+
+### Connection String Device Authentication
+* **IOTHUB_DEVICE_CONNECTION_STRING**: The connection string for your IoTHub Device, which can be found in the Azure Portal
+
+### X509 Authentication
+* **X509_CERT_FILE**: The path to the X509 certificate
+* **X509_KEY_FILE**: The path to the X509 key
+* **X509_PASS_PHRASE**: The pass phrase for the X509 key (Only necessary if cert has a password)
+
+**This is an incomplete list of environment variables**
+
+
+## E2E Testing Setup (Optional - SDK Developer)
+
+If you wish to run end to end tests locally, you'll need to configure some additional environment variables:
+
+* **IOTHUB_CONNECTION_STRING**: The connection string for your IoTHub (ideally iothubowner permissions)
+* **EVENTHUB_CONNECTION_STRING**: The built-in Event Hub compatible endpoint of the above IoTHub
+
+**NOTE**: if you wish to use dedicated E2E resources, you may also prefix the above variables with `IOTHUB_E2E_`
+
+Additionally, you will need to add a messaging route with the following settings to the IoTHub in order for all tests to run correctly:
+* Name: twin
+* Endpoint: events
+* Data Source: Device Twin Change Events
```

### Comparing `azure-iot-device-3.0.0b1/setup.py` & `azure-iot-device-3.0.0b2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,32 +61,34 @@
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     install_requires=[
         # Define sub-dependencies due to pip dependency resolution bug
         # https://github.com/pypa/pip/issues/988
         # ---requests dependencies---
         # requests 2.22+ does not support urllib3 1.25.0 or 1.25.1 (https://github.com/psf/requests/pull/5092)
         # Security issue below 1.26.5
         "urllib3>=1.26.5,<1.27",
         # Actual project dependencies
         "paho-mqtt>=1.6.1,<2.0.0",
-        "requests>=2.20.0,<3.0.0",
         "requests-unixsocket>=0.1.5,<1.0.0",
-        "janus",
+        "typing-extensions>=4.4.0,<5.0",
         "PySocks",
+        # This dependency is needed by some modules, but none that are actually used
+        # in current IoTHubSession design. This can be removed once we settle on a direction.
+        "aiohttp",
     ],
-    python_requires=">=3.6, <4",
+    python_requires=">=3.7, <4",
     packages=find_namespace_packages(where="azure-iot-device"),
     package_dir={"": "azure-iot-device"},
     zip_safe=False,
 )
```

