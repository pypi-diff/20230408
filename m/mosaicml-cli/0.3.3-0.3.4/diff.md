# Comparing `tmp/mosaicml-cli-0.3.3.tar.gz` & `tmp/mosaicml-cli-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosaicml-cli-0.3.3.tar", last modified: Thu Apr  6 21:21:43 2023, max compression
+gzip compressed data, was "mosaicml-cli-0.3.4.tar", last modified: Fri Apr  7 22:51:48 2023, max compression
```

## Comparing `mosaicml-cli-0.3.3.tar` & `mosaicml-cli-0.3.4.tar`

### file list

```diff
@@ -1,268 +1,268 @@
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.508520 mosaicml-cli-0.3.3/
--rw-r--r--   0 anna       (501) staff       (20)      696 2023-04-06 21:21:43.508200 mosaicml-cli-0.3.3/PKG-INFO
--rw-r--r--   0 anna       (501) staff       (20)     7799 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/README.md
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.428429 mosaicml-cli-0.3.3/mcli/
--rw-r--r--   0 anna       (501) staff       (20)       54 2022-12-14 17:51:04.000000 mosaicml-cli-0.3.3/mcli/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.429519 mosaicml-cli-0.3.3/mcli/api/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/api/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.430281 mosaicml-cli-0.3.3/mcli/api/cluster/
--rw-r--r--   0 anna       (501) staff       (20)      134 2022-10-27 22:42:42.000000 mosaicml-cli-0.3.3/mcli/api/cluster/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4058 2023-03-30 22:21:56.000000 mosaicml-cli-0.3.3/mcli/api/cluster/api_get_clusters.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.431671 mosaicml-cli-0.3.3/mcli/api/engine/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/api/engine/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)    22935 2023-04-05 22:41:30.000000 mosaicml-cli-0.3.3/mcli/api/engine/engine.py
--rw-r--r--   0 anna       (501) staff       (20)      787 2022-09-12 18:09:44.000000 mosaicml-cli-0.3.3/mcli/api/engine/utils.py
--rw-r--r--   0 anna       (501) staff       (20)    11677 2023-04-05 22:17:10.000000 mosaicml-cli-0.3.3/mcli/api/exceptions.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.433550 mosaicml-cli-0.3.3/mcli/api/inference_deployments/
--rw-r--r--   0 anna       (501) staff       (20)      858 2023-03-30 22:21:56.000000 mosaicml-cli-0.3.3/mcli/api/inference_deployments/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3388 2023-03-30 22:24:52.000000 mosaicml-cli-0.3.3/mcli/api/inference_deployments/api_create_inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     3278 2023-03-30 22:24:52.000000 mosaicml-cli-0.3.3/mcli/api/inference_deployments/api_delete_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     6091 2023-03-30 22:24:52.000000 mosaicml-cli-0.3.3/mcli/api/inference_deployments/api_get_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     1156 2023-03-30 22:24:52.000000 mosaicml-cli-0.3.3/mcli/api/inference_deployments/api_ping_inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     1276 2023-03-30 22:24:52.000000 mosaicml-cli-0.3.3/mcli/api/inference_deployments/api_predict_inference_deployment.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.433818 mosaicml-cli-0.3.3/mcli/api/kube/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-09-01 16:10:03.000000 mosaicml-cli-0.3.3/mcli/api/kube/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.435990 mosaicml-cli-0.3.3/mcli/api/kube/runs/
--rw-r--r--   0 anna       (501) staff       (20)      856 2022-09-01 16:10:03.000000 mosaicml-cli-0.3.3/mcli/api/kube/runs/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4900 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/api/kube/runs/api_create_run.py
--rw-r--r--   0 anna       (501) staff       (20)     5042 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/api/kube/runs/api_delete_runs.py
--rw-r--r--   0 anna       (501) staff       (20)    14458 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/api/kube/runs/api_get_run_logs.py
--rw-r--r--   0 anna       (501) staff       (20)    16142 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/api/kube/runs/api_get_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     6007 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/api/kube/runs/api_stop_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     6210 2022-12-16 00:52:51.000000 mosaicml-cli-0.3.3/mcli/api/kube/runs/api_watch_run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.436596 mosaicml-cli-0.3.3/mcli/api/mint/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/api/mint/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4987 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/api/mint/shell.py
--rw-r--r--   0 anna       (501) staff       (20)     1530 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/api/mint/tty.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.437555 mosaicml-cli-0.3.3/mcli/api/model/
--rw-r--r--   0 anna       (501) staff       (20)      209 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/api/model/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     5655 2023-03-30 20:02:22.000000 mosaicml-cli-0.3.3/mcli/api/model/cluster_details.py
--rw-r--r--   0 anna       (501) staff       (20)     3015 2023-03-30 22:24:52.000000 mosaicml-cli-0.3.3/mcli/api/model/inference_deployment.py
--rw-r--r--   0 anna       (501) staff       (20)     4050 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/api/model/run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.439335 mosaicml-cli-0.3.3/mcli/api/runs/
--rw-r--r--   0 anna       (501) staff       (20)      828 2023-04-06 21:20:57.000000 mosaicml-cli-0.3.3/mcli/api/runs/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2683 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/api/runs/api_create_run.py
--rw-r--r--   0 anna       (501) staff       (20)     3947 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/api/runs/api_delete_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     9281 2023-03-30 22:21:56.000000 mosaicml-cli-0.3.3/mcli/api/runs/api_get_run_logs.py
--rw-r--r--   0 anna       (501) staff       (20)     6563 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/api/runs/api_get_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     6037 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/api/runs/api_stop_runs.py
--rw-r--r--   0 anna       (501) staff       (20)    10619 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/api/runs/api_watch_run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.439738 mosaicml-cli-0.3.3/mcli/api/schema/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/api/schema/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      636 2022-09-01 16:10:03.000000 mosaicml-cli-0.3.3/mcli/api/schema/generic_model.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.441241 mosaicml-cli-0.3.3/mcli/api/secrets/
--rw-r--r--   0 anna       (501) staff       (20)      309 2022-10-06 23:19:14.000000 mosaicml-cli-0.3.3/mcli/api/secrets/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2365 2023-03-30 23:10:34.000000 mosaicml-cli-0.3.3/mcli/api/secrets/api_create_secret.py
--rw-r--r--   0 anna       (501) staff       (20)     2998 2023-03-30 22:21:56.000000 mosaicml-cli-0.3.3/mcli/api/secrets/api_delete_secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     3697 2023-03-30 22:21:56.000000 mosaicml-cli-0.3.3/mcli/api/secrets/api_get_secrets.py
--rw-r--r--   0 anna       (501) staff       (20)      508 2023-01-12 23:53:10.000000 mosaicml-cli-0.3.3/mcli/api/types.py
--rw-r--r--   0 anna       (501) staff       (20)     2354 2022-08-15 20:43:31.000000 mosaicml-cli-0.3.3/mcli/api/typing_future.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.441995 mosaicml-cli-0.3.3/mcli/api/users/
--rw-r--r--   0 anna       (501) staff       (20)      139 2023-02-22 17:58:38.000000 mosaicml-cli-0.3.3/mcli/api/users/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2694 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/api/users/api_get_users.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.442308 mosaicml-cli-0.3.3/mcli/cli/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/cli/__init__.py
--rwxr-xr-x   0 anna       (501) staff       (20)     7182 2023-03-30 22:21:56.000000 mosaicml-cli-0.3.3/mcli/cli/cli.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.442893 mosaicml-cli-0.3.3/mcli/cli/common/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-02-02 22:26:54.000000 mosaicml-cli-0.3.3/mcli/cli/common/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2670 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/cli/common/deployment_filters.py
--rw-r--r--   0 anna       (501) staff       (20)     7180 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/cli/common/run_filters.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.443349 mosaicml-cli-0.3.3/mcli/cli/m_clean/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/cli/m_clean/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      950 2022-10-27 22:42:42.000000 mosaicml-cli-0.3.3/mcli/cli/m_clean/m_clean.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.443899 mosaicml-cli-0.3.3/mcli/cli/m_connect/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/cli/m_connect/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1541 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/cli/m_connect/m_connect.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.445209 mosaicml-cli-0.3.3/mcli/cli/m_create/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/cli/m_create/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)    11513 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/cli/m_create/cluster.py
--rw-r--r--   0 anna       (501) staff       (20)     7167 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/cli/m_create/env_var.py
--rw-r--r--   0 anna       (501) staff       (20)     4217 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/cli/m_create/m_create.py
--rw-r--r--   0 anna       (501) staff       (20)    24927 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/cli/m_create/secret.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.446005 mosaicml-cli-0.3.3/mcli/cli/m_delete/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/cli/m_delete/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)    14072 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/cli/m_delete/delete.py
--rw-r--r--   0 anna       (501) staff       (20)     8417 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/cli/m_delete/m_delete.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.446453 mosaicml-cli-0.3.3/mcli/cli/m_deploy/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/cli/m_deploy/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3896 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/cli/m_deploy/m_deploy.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.447292 mosaicml-cli-0.3.3/mcli/cli/m_describe/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-02-02 22:26:54.000000 mosaicml-cli-0.3.3/mcli/cli/m_describe/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4409 2023-03-30 22:24:52.000000 mosaicml-cli-0.3.3/mcli/cli/m_describe/describe_inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     7391 2023-04-06 21:20:57.000000 mosaicml-cli-0.3.3/mcli/cli/m_describe/describe_runs.py
--rw-r--r--   0 anna       (501) staff       (20)     1860 2023-03-30 22:24:52.000000 mosaicml-cli-0.3.3/mcli/cli/m_describe/m_describe.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.449472 mosaicml-cli-0.3.3/mcli/cli/m_get/
--rw-r--r--   0 anna       (501) staff       (20)      549 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/cli/m_get/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3909 2023-03-31 01:05:42.000000 mosaicml-cli-0.3.3/mcli/cli/m_get/clusters.py
--rw-r--r--   0 anna       (501) staff       (20)     6452 2023-04-05 17:48:41.000000 mosaicml-cli-0.3.3/mcli/cli/m_get/display.py
--rw-r--r--   0 anna       (501) staff       (20)     1315 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/cli/m_get/envvars.py
--rw-r--r--   0 anna       (501) staff       (20)     5361 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/cli/m_get/inference_deployments.py
--rw-r--r--   0 anna       (501) staff       (20)     4866 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/cli/m_get/m_get.py
--rw-r--r--   0 anna       (501) staff       (20)     6289 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/cli/m_get/runs.py
--rw-r--r--   0 anna       (501) staff       (20)     3567 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/cli/m_get/secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     1580 2023-02-22 17:58:38.000000 mosaicml-cli-0.3.3/mcli/cli/m_get/users.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.450008 mosaicml-cli-0.3.3/mcli/cli/m_init/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/cli/m_init/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4113 2023-03-30 22:21:56.000000 mosaicml-cli-0.3.3/mcli/cli/m_init/m_init.py
--rw-r--r--   0 anna       (501) staff       (20)     9374 2023-03-31 01:05:42.000000 mosaicml-cli-0.3.3/mcli/cli/m_init/m_init_kube.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.450916 mosaicml-cli-0.3.3/mcli/cli/m_interactive/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/cli/m_interactive/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     9005 2023-03-31 20:52:34.000000 mosaicml-cli-0.3.3/mcli/cli/m_interactive/interactive.py
--rw-r--r--   0 anna       (501) staff       (20)    16203 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/cli/m_interactive/m_interactive.py
--rw-r--r--   0 anna       (501) staff       (20)     4571 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/cli/m_interactive/temp_mcloud_interactive.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.451187 mosaicml-cli-0.3.3/mcli/cli/m_log/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/cli/m_log/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     8633 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/cli/m_log/m_log.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.451457 mosaicml-cli-0.3.3/mcli/cli/m_ping/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/cli/m_ping/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     1742 2023-03-30 22:21:56.000000 mosaicml-cli-0.3.3/mcli/cli/m_ping/m_ping.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.451719 mosaicml-cli-0.3.3/mcli/cli/m_predict/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-03-30 22:21:56.000000 mosaicml-cli-0.3.3/mcli/cli/m_predict/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2160 2023-03-30 22:21:56.000000 mosaicml-cli-0.3.3/mcli/cli/m_predict/m_predict.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.451974 mosaicml-cli-0.3.3/mcli/cli/m_root/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/cli/m_root/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      947 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/cli/m_root/m_config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.452371 mosaicml-cli-0.3.3/mcli/cli/m_run/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/cli/m_run/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     9494 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/cli/m_run/m_run.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.453256 mosaicml-cli-0.3.3/mcli/cli/m_set_unset/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-10-06 23:19:14.000000 mosaicml-cli-0.3.3/mcli/cli/m_set_unset/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     2973 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/cli/m_set_unset/api_key.py
--rw-r--r--   0 anna       (501) staff       (20)     1927 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/cli/m_set_unset/m_set.py
--rw-r--r--   0 anna       (501) staff       (20)     1408 2023-02-22 17:58:38.000000 mosaicml-cli-0.3.3/mcli/cli/m_set_unset/m_unset.py
--rw-r--r--   0 anna       (501) staff       (20)      881 2023-02-22 17:58:38.000000 mosaicml-cli-0.3.3/mcli/cli/m_set_unset/user.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.453576 mosaicml-cli-0.3.3/mcli/cli/m_stop/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-10-06 23:19:14.000000 mosaicml-cli-0.3.3/mcli/cli/m_stop/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3847 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/cli/m_stop/m_stop.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.454050 mosaicml-cli-0.3.3/mcli/cli/m_use/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/cli/m_use/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3234 2022-12-21 22:27:10.000000 mosaicml-cli-0.3.3/mcli/cli/m_use/m_use.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.455137 mosaicml-cli-0.3.3/mcli/cli/m_util/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-09-01 16:10:03.000000 mosaicml-cli-0.3.3/mcli/cli/m_util/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     9853 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/cli/m_util/kube_util.py
--rw-r--r--   0 anna       (501) staff       (20)     1147 2022-10-27 22:42:42.000000 mosaicml-cli-0.3.3/mcli/cli/m_util/m_util.py
--rw-r--r--   0 anna       (501) staff       (20)     6515 2023-03-30 22:24:52.000000 mosaicml-cli-0.3.3/mcli/cli/m_util/util.py
--rw-r--r--   0 anna       (501) staff       (20)    16462 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.457062 mosaicml-cli-0.3.3/mcli/models/
--rw-r--r--   0 anna       (501) staff       (20)     1061 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/models/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     7179 2023-03-30 22:24:52.000000 mosaicml-cli-0.3.3/mcli/models/inference_deployment_config.py
--rw-r--r--   0 anna       (501) staff       (20)     3693 2023-03-30 20:02:22.000000 mosaicml-cli-0.3.3/mcli/models/mcli_cluster.py
--rw-r--r--   0 anna       (501) staff       (20)      563 2022-09-12 19:04:53.000000 mosaicml-cli-0.3.3/mcli/models/mcli_envvar.py
--rw-r--r--   0 anna       (501) staff       (20)     3386 2022-10-06 23:19:14.000000 mosaicml-cli-0.3.3/mcli/models/mcli_integration.py
--rw-r--r--   0 anna       (501) staff       (20)     9400 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/models/mcli_secret.py
--rw-r--r--   0 anna       (501) staff       (20)    21114 2023-04-06 21:20:57.000000 mosaicml-cli-0.3.3/mcli/models/run_config.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.457474 mosaicml-cli-0.3.3/mcli/objects/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/objects/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.459561 mosaicml-cli-0.3.3/mcli/objects/integrations/
--rw-r--r--   0 anna       (501) staff       (20)      660 2022-10-06 23:19:14.000000 mosaicml-cli-0.3.3/mcli/objects/integrations/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      671 2022-07-14 18:08:16.000000 mosaicml-cli-0.3.3/mcli/objects/integrations/apt_packages.py
--rw-r--r--   0 anna       (501) staff       (20)     1287 2022-10-06 23:19:14.000000 mosaicml-cli-0.3.3/mcli/objects/integrations/comet.py
--rw-r--r--   0 anna       (501) staff       (20)     2597 2023-02-02 22:26:54.000000 mosaicml-cli-0.3.3/mcli/objects/integrations/git_repo.py
--rw-r--r--   0 anna       (501) staff       (20)     3491 2022-10-06 23:19:14.000000 mosaicml-cli-0.3.3/mcli/objects/integrations/local.py
--rw-r--r--   0 anna       (501) staff       (20)     2126 2022-12-21 22:27:10.000000 mosaicml-cli-0.3.3/mcli/objects/integrations/mosaicml_agent.py
--rw-r--r--   0 anna       (501) staff       (20)      810 2022-07-14 18:08:20.000000 mosaicml-cli-0.3.3/mcli/objects/integrations/pip_packages.py
--rw-r--r--   0 anna       (501) staff       (20)     2742 2022-09-01 16:42:18.000000 mosaicml-cli-0.3.3/mcli/objects/integrations/wandb.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.461402 mosaicml-cli-0.3.3/mcli/objects/secrets/
--rw-r--r--   0 anna       (501) staff       (20)     1090 2022-12-21 22:27:10.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     4913 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/cluster_secret.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.462897 mosaicml-cli-0.3.3/mcli/objects/secrets/create/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/create/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     3953 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/create/base.py
--rw-r--r--   0 anna       (501) staff       (20)     3461 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/create/docker_registry.py
--rw-r--r--   0 anna       (501) staff       (20)     2406 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/create/gcp.py
--rw-r--r--   0 anna       (501) staff       (20)     7554 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/create/generic.py
--rw-r--r--   0 anna       (501) staff       (20)     3855 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/create/oci.py
--rw-r--r--   0 anna       (501) staff       (20)     2998 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/create/s3.py
--rw-r--r--   0 anna       (501) staff       (20)     6701 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/create/ssh.py
--rw-r--r--   0 anna       (501) staff       (20)     3782 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/docker_registry.py
--rw-r--r--   0 anna       (501) staff       (20)     1634 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/env_var.py
--rw-r--r--   0 anna       (501) staff       (20)     1122 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/gcp.py
--rw-r--r--   0 anna       (501) staff       (20)     2893 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/mounted.py
--rw-r--r--   0 anna       (501) staff       (20)     2855 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/oci.py
--rw-r--r--   0 anna       (501) staff       (20)     2577 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/s3.py
--rw-r--r--   0 anna       (501) staff       (20)     3952 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/objects/secrets/ssh.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.463087 mosaicml-cli-0.3.3/mcli/sdk/
--rw-r--r--   0 anna       (501) staff       (20)      586 2023-04-06 21:20:57.000000 mosaicml-cli-0.3.3/mcli/sdk/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.463247 mosaicml-cli-0.3.3/mcli/serverside/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/serverside/__init__.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.465114 mosaicml-cli-0.3.3/mcli/serverside/clusters/
--rw-r--r--   0 anna       (501) staff       (20)      381 2023-03-30 20:02:22.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)    11245 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/cluster.py
--rw-r--r--   0 anna       (501) staff       (20)    23072 2023-03-30 20:02:22.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/cluster_instances.py
--rw-r--r--   0 anna       (501) staff       (20)     4005 2022-10-27 22:42:42.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/cluster_pv_setup.py
--rw-r--r--   0 anna       (501) staff       (20)     2793 2023-03-15 21:04:58.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/gpu_type.py
--rw-r--r--   0 anna       (501) staff       (20)     2824 2023-02-02 22:26:54.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/instance_type.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.476653 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/
--rw-r--r--   0 anna       (501) staff       (20)     1603 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)      548 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/microk8s.py
--rw-r--r--   0 anna       (501) staff       (20)     2219 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r10z1.py
--rw-r--r--   0 anna       (501) staff       (20)     2822 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r1z1.py
--rw-r--r--   0 anna       (501) staff       (20)     2495 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r1z4.py
--rw-r--r--   0 anna       (501) staff       (20)     2759 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r3z1.py
--rw-r--r--   0 anna       (501) staff       (20)     5355 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r4z1.py
--rw-r--r--   0 anna       (501) staff       (20)     1049 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z1.py
--rw-r--r--   0 anna       (501) staff       (20)     1161 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z10.py
--rw-r--r--   0 anna       (501) staff       (20)     2497 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z2.py
--rw-r--r--   0 anna       (501) staff       (20)     1062 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z3.py
--rw-r--r--   0 anna       (501) staff       (20)     1034 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z4.py
--rw-r--r--   0 anna       (501) staff       (20)     1047 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z5.py
--rw-r--r--   0 anna       (501) staff       (20)     1047 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z6.py
--rw-r--r--   0 anna       (501) staff       (20)     1214 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z7.py
--rw-r--r--   0 anna       (501) staff       (20)     1242 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z9.py
--rw-r--r--   0 anna       (501) staff       (20)     1034 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r8z1.py
--rw-r--r--   0 anna       (501) staff       (20)     1071 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r8z2.py
--rw-r--r--   0 anna       (501) staff       (20)     1054 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r8z3.py
--rw-r--r--   0 anna       (501) staff       (20)     1061 2023-03-31 00:39:43.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r99z1.py
--rw-r--r--   0 anna       (501) staff       (20)      310 2022-10-06 23:19:14.000000 mosaicml-cli-0.3.3/mcli/serverside/clusters/volumekind.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.481828 mosaicml-cli-0.3.3/mcli/serverside/job/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/serverside/job/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)    15555 2023-02-02 22:26:54.000000 mosaicml-cli-0.3.3/mcli/serverside/job/mcli_job.py
--rw-r--r--   0 anna       (501) staff       (20)      465 2022-07-14 19:44:13.000000 mosaicml-cli-0.3.3/mcli/serverside/job/mcli_k8s_config_map_typing.py
--rw-r--r--   0 anna       (501) staff       (20)     6471 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/mcli/serverside/job/mcli_k8s_job.py
--rw-r--r--   0 anna       (501) staff       (20)     8090 2022-08-08 20:33:01.000000 mosaicml-cli-0.3.3/mcli/serverside/job/mcli_k8s_job_typing.py
--rw-r--r--   0 anna       (501) staff       (20)     7524 2022-10-06 23:19:14.000000 mosaicml-cli-0.3.3/mcli/serverside/job/mcli_k8s_resource_requirements_typing.py
--rw-r--r--   0 anna       (501) staff       (20)      459 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/serverside/job/mcli_k8s_service_typing.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.483232 mosaicml-cli-0.3.3/mcli/serverside/runners/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/serverside/runners/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     5770 2022-12-21 22:27:10.000000 mosaicml-cli-0.3.3/mcli/serverside/runners/runner.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.499369 mosaicml-cli-0.3.3/mcli/utils/
--rw-r--r--   0 anna       (501) staff       (20)        0 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/utils/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     5306 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/utils/utils_cli.py
--rw-r--r--   0 anna       (501) staff       (20)     2555 2023-04-05 17:17:35.000000 mosaicml-cli-0.3.3/mcli/utils/utils_config.py
--rw-r--r--   0 anna       (501) staff       (20)      740 2022-10-06 23:19:14.000000 mosaicml-cli-0.3.3/mcli/utils/utils_date.py
--rw-r--r--   0 anna       (501) staff       (20)    10453 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/utils/utils_docker.py
--rw-r--r--   0 anna       (501) staff       (20)    12947 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/utils/utils_epilog.py
--rw-r--r--   0 anna       (501) staff       (20)      751 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/utils/utils_file.py
--rw-r--r--   0 anna       (501) staff       (20)    11769 2022-12-21 22:27:10.000000 mosaicml-cli-0.3.3/mcli/utils/utils_interactive.py
--rw-r--r--   0 anna       (501) staff       (20)    49322 2022-11-16 17:00:39.000000 mosaicml-cli-0.3.3/mcli/utils/utils_kube.py
--rw-r--r--   0 anna       (501) staff       (20)     6980 2023-02-02 22:26:54.000000 mosaicml-cli-0.3.3/mcli/utils/utils_kube_labels.py
--rw-r--r--   0 anna       (501) staff       (20)     4741 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/utils/utils_logging.py
--rw-r--r--   0 anna       (501) staff       (20)      359 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/utils/utils_modules.py
--rw-r--r--   0 anna       (501) staff       (20)     6614 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/utils/utils_pypi.py
--rw-r--r--   0 anna       (501) staff       (20)     6513 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/utils/utils_rancher.py
--rw-r--r--   0 anna       (501) staff       (20)     3115 2022-09-12 17:46:33.000000 mosaicml-cli-0.3.3/mcli/utils/utils_rich.py
--rw-r--r--   0 anna       (501) staff       (20)     8533 2023-01-06 22:51:41.000000 mosaicml-cli-0.3.3/mcli/utils/utils_run_status.py
--rw-r--r--   0 anna       (501) staff       (20)     4350 2022-09-12 17:46:33.000000 mosaicml-cli-0.3.3/mcli/utils/utils_serializable_dataclass.py
--rw-r--r--   0 anna       (501) staff       (20)     1103 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/utils/utils_spinner.py
--rw-r--r--   0 anna       (501) staff       (20)    11437 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/mcli/utils/utils_string_functions.py
--rw-r--r--   0 anna       (501) staff       (20)     3954 2022-11-15 18:47:24.000000 mosaicml-cli-0.3.3/mcli/utils/utils_types.py
--rw-r--r--   0 anna       (501) staff       (20)     1001 2022-07-01 20:27:34.000000 mosaicml-cli-0.3.3/mcli/utils/utils_yaml.py
--rw-r--r--   0 anna       (501) staff       (20)     3884 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/mcli/version.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.503145 mosaicml-cli-0.3.3/mosaicml_cli.egg-info/
--rw-r--r--   0 anna       (501) staff       (20)      696 2023-04-06 21:21:43.000000 mosaicml-cli-0.3.3/mosaicml_cli.egg-info/PKG-INFO
--rw-r--r--   0 anna       (501) staff       (20)     7139 2023-04-06 21:21:43.000000 mosaicml-cli-0.3.3/mosaicml_cli.egg-info/SOURCES.txt
--rw-r--r--   0 anna       (501) staff       (20)        1 2023-04-06 21:21:43.000000 mosaicml-cli-0.3.3/mosaicml_cli.egg-info/dependency_links.txt
--rw-r--r--   0 anna       (501) staff       (20)       75 2023-04-06 21:21:43.000000 mosaicml-cli-0.3.3/mosaicml_cli.egg-info/entry_points.txt
--rw-r--r--   0 anna       (501) staff       (20)     1630 2023-04-06 21:21:43.000000 mosaicml-cli-0.3.3/mosaicml_cli.egg-info/requires.txt
--rw-r--r--   0 anna       (501) staff       (20)       11 2023-04-06 21:21:43.000000 mosaicml-cli-0.3.3/mosaicml_cli.egg-info/top_level.txt
--rw-r--r--   0 anna       (501) staff       (20)    30933 2022-12-15 00:57:04.000000 mosaicml-cli-0.3.3/pyproject.toml
--rw-r--r--   0 anna       (501) staff       (20)       38 2023-04-06 21:21:43.508717 mosaicml-cli-0.3.3/setup.cfg
--rw-r--r--   0 anna       (501) staff       (20)     3111 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/setup.py
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.505313 mosaicml-cli-0.3.3/tests/
-drwxr-xr-x   0 anna       (501) staff       (20)        0 2023-04-06 21:21:43.507257 mosaicml-cli-0.3.3/tests/submit/
--rw-r--r--   0 anna       (501) staff       (20)        0 2023-03-17 15:59:14.000000 mosaicml-cli-0.3.3/tests/submit/__init__.py
--rw-r--r--   0 anna       (501) staff       (20)     6393 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/tests/submit/test_cluster.py
--rw-r--r--   0 anna       (501) staff       (20)     9266 2023-03-31 04:06:45.000000 mosaicml-cli-0.3.3/tests/submit/test_cluster_secrets.py
--rw-r--r--   0 anna       (501) staff       (20)     7973 2023-04-06 21:21:07.000000 mosaicml-cli-0.3.3/tests/test_config.py
--rw-r--r--   0 anna       (501) staff       (20)       62 2023-03-17 15:59:14.000000 mosaicml-cli-0.3.3/tests/test_simple.py
--rw-r--r--   0 anna       (501) staff       (20)     6116 2023-03-27 21:07:48.000000 mosaicml-cli-0.3.3/tests/test_upgrade.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.143029 mosaicml-cli-0.3.4/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      696 2023-04-07 22:51:48.142481 mosaicml-cli-0.3.4/PKG-INFO
+-rw-r--r--   0 jeffchen   (501) staff       (20)     7799 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/README.md
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.944867 mosaicml-cli-0.3.4/mcli/
+-rw-r--r--   0 jeffchen   (501) staff       (20)       54 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/__init__.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.951912 mosaicml-cli-0.3.4/mcli/api/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/api/__init__.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.956825 mosaicml-cli-0.3.4/mcli/api/cluster/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      134 2022-10-27 20:22:32.000000 mosaicml-cli-0.3.4/mcli/api/cluster/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4058 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/cluster/api_get_clusters.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.963041 mosaicml-cli-0.3.4/mcli/api/engine/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/api/engine/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    22935 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/engine/engine.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      787 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/api/engine/utils.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    11677 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/exceptions.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.974224 mosaicml-cli-0.3.4/mcli/api/inference_deployments/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      858 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/inference_deployments/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3388 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/inference_deployments/api_create_inference_deployment.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3278 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/inference_deployments/api_delete_inference_deployments.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6091 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/inference_deployments/api_get_inference_deployments.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1156 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/inference_deployments/api_ping_inference_deployment.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1276 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/inference_deployments/api_predict_inference_deployment.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.974957 mosaicml-cli-0.3.4/mcli/api/kube/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/api/kube/__init__.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.980551 mosaicml-cli-0.3.4/mcli/api/kube/runs/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      856 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/api/kube/runs/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4900 2023-04-07 16:42:06.000000 mosaicml-cli-0.3.4/mcli/api/kube/runs/api_create_run.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5042 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/kube/runs/api_delete_runs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    14458 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/kube/runs/api_get_run_logs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    16142 2023-04-07 16:42:06.000000 mosaicml-cli-0.3.4/mcli/api/kube/runs/api_get_runs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6007 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/kube/runs/api_stop_runs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6210 2022-10-27 20:22:32.000000 mosaicml-cli-0.3.4/mcli/api/kube/runs/api_watch_run.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.984355 mosaicml-cli-0.3.4/mcli/api/mint/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/mint/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4987 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/mint/shell.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1530 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/mint/tty.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.988939 mosaicml-cli-0.3.4/mcli/api/model/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      209 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/model/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5655 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/model/cluster_details.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3015 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/model/inference_deployment.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6055 2023-04-07 22:48:37.000000 mosaicml-cli-0.3.4/mcli/api/model/run.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.992321 mosaicml-cli-0.3.4/mcli/api/runs/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      828 2023-01-26 01:45:43.000000 mosaicml-cli-0.3.4/mcli/api/runs/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2683 2023-04-07 16:42:06.000000 mosaicml-cli-0.3.4/mcli/api/runs/api_create_run.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3947 2023-04-07 16:42:06.000000 mosaicml-cli-0.3.4/mcli/api/runs/api_delete_runs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     9281 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/runs/api_get_run_logs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6563 2023-04-07 16:42:06.000000 mosaicml-cli-0.3.4/mcli/api/runs/api_get_runs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6037 2023-04-07 16:42:06.000000 mosaicml-cli-0.3.4/mcli/api/runs/api_stop_runs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    10619 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/runs/api_watch_run.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.992692 mosaicml-cli-0.3.4/mcli/api/schema/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/api/schema/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      636 2022-11-11 00:18:38.000000 mosaicml-cli-0.3.4/mcli/api/schema/generic_model.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.993879 mosaicml-cli-0.3.4/mcli/api/secrets/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      309 2022-09-19 22:17:10.000000 mosaicml-cli-0.3.4/mcli/api/secrets/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2365 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/secrets/api_create_secret.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2998 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/secrets/api_delete_secrets.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3697 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/secrets/api_get_secrets.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      508 2023-01-10 00:19:00.000000 mosaicml-cli-0.3.4/mcli/api/types.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2354 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/api/typing_future.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.994331 mosaicml-cli-0.3.4/mcli/api/users/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      139 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/users/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2694 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/api/users/api_get_users.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.994673 mosaicml-cli-0.3.4/mcli/cli/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/cli/__init__.py
+-rwxr-xr-x   0 jeffchen   (501) staff       (20)     7182 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/cli.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.995417 mosaicml-cli-0.3.4/mcli/cli/common/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-02-01 21:37:29.000000 mosaicml-cli-0.3.4/mcli/cli/common/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2670 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/common/deployment_filters.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     7180 2023-04-07 16:42:06.000000 mosaicml-cli-0.3.4/mcli/cli/common/run_filters.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.995798 mosaicml-cli-0.3.4/mcli/cli/m_clean/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/cli/m_clean/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      950 2022-10-27 20:22:32.000000 mosaicml-cli-0.3.4/mcli/cli/m_clean/m_clean.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.996386 mosaicml-cli-0.3.4/mcli/cli/m_connect/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_connect/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1541 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_connect/m_connect.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.998112 mosaicml-cli-0.3.4/mcli/cli/m_create/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/cli/m_create/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    11513 2022-10-27 20:22:32.000000 mosaicml-cli-0.3.4/mcli/cli/m_create/cluster.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     7167 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_create/env_var.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4217 2023-02-01 21:37:29.000000 mosaicml-cli-0.3.4/mcli/cli/m_create/m_create.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    24927 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_create/secret.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:47.999963 mosaicml-cli-0.3.4/mcli/cli/m_delete/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/cli/m_delete/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    14072 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_delete/delete.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     8417 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_delete/m_delete.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.000452 mosaicml-cli-0.3.4/mcli/cli/m_deploy/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_deploy/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3896 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_deploy/m_deploy.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.001130 mosaicml-cli-0.3.4/mcli/cli/m_describe/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-01-26 01:45:43.000000 mosaicml-cli-0.3.4/mcli/cli/m_describe/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4409 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_describe/describe_inference_deployments.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     7391 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_describe/describe_runs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1860 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_describe/m_describe.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.005600 mosaicml-cli-0.3.4/mcli/cli/m_get/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      549 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_get/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3909 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_get/clusters.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6452 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_get/display.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1315 2022-09-14 20:53:21.000000 mosaicml-cli-0.3.4/mcli/cli/m_get/envvars.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5361 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_get/inference_deployments.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4866 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_get/m_get.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6346 2023-04-07 22:48:37.000000 mosaicml-cli-0.3.4/mcli/cli/m_get/runs.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3567 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_get/secrets.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1580 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_get/users.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.006114 mosaicml-cli-0.3.4/mcli/cli/m_init/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/cli/m_init/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4113 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_init/m_init.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     9374 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_init/m_init_kube.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.009688 mosaicml-cli-0.3.4/mcli/cli/m_interactive/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/cli/m_interactive/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     9005 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_interactive/interactive.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    16203 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_interactive/m_interactive.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4571 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_interactive/temp_mcloud_interactive.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.010099 mosaicml-cli-0.3.4/mcli/cli/m_log/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/cli/m_log/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     8633 2023-04-07 16:42:06.000000 mosaicml-cli-0.3.4/mcli/cli/m_log/m_log.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.010474 mosaicml-cli-0.3.4/mcli/cli/m_ping/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_ping/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1742 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_ping/m_ping.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.010799 mosaicml-cli-0.3.4/mcli/cli/m_predict/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_predict/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2160 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_predict/m_predict.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.011141 mosaicml-cli-0.3.4/mcli/cli/m_root/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/cli/m_root/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      947 2022-10-31 17:33:03.000000 mosaicml-cli-0.3.4/mcli/cli/m_root/m_config.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.012038 mosaicml-cli-0.3.4/mcli/cli/m_run/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/cli/m_run/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    10179 2023-04-07 22:48:37.000000 mosaicml-cli-0.3.4/mcli/cli/m_run/m_run.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.013453 mosaicml-cli-0.3.4/mcli/cli/m_set_unset/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-10-06 23:40:35.000000 mosaicml-cli-0.3.4/mcli/cli/m_set_unset/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2973 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_set_unset/api_key.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1927 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_set_unset/m_set.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1408 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_set_unset/m_unset.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      881 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_set_unset/user.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.013939 mosaicml-cli-0.3.4/mcli/cli/m_stop/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-27 01:04:20.000000 mosaicml-cli-0.3.4/mcli/cli/m_stop/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3847 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_stop/m_stop.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.014357 mosaicml-cli-0.3.4/mcli/cli/m_use/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/cli/m_use/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3234 2022-12-09 18:28:49.000000 mosaicml-cli-0.3.4/mcli/cli/m_use/m_use.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.016670 mosaicml-cli-0.3.4/mcli/cli/m_util/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/cli/m_util/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     9853 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_util/kube_util.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1147 2022-10-27 20:22:32.000000 mosaicml-cli-0.3.4/mcli/cli/m_util/m_util.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6515 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/cli/m_util/util.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    16462 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/config.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.019329 mosaicml-cli-0.3.4/mcli/models/
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1061 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/models/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     8572 2023-04-07 22:48:37.000000 mosaicml-cli-0.3.4/mcli/models/inference_deployment_config.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3693 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/models/mcli_cluster.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      563 2022-09-14 20:53:21.000000 mosaicml-cli-0.3.4/mcli/models/mcli_envvar.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3386 2022-09-14 20:53:21.000000 mosaicml-cli-0.3.4/mcli/models/mcli_integration.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     9400 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/models/mcli_secret.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    17303 2023-04-07 22:48:37.000000 mosaicml-cli-0.3.4/mcli/models/run_config.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.022649 mosaicml-cli-0.3.4/mcli/objects/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/objects/__init__.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.026562 mosaicml-cli-0.3.4/mcli/objects/integrations/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      660 2022-09-14 20:53:21.000000 mosaicml-cli-0.3.4/mcli/objects/integrations/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      671 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/objects/integrations/apt_packages.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1287 2022-09-14 20:53:21.000000 mosaicml-cli-0.3.4/mcli/objects/integrations/comet.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2597 2023-01-26 01:45:43.000000 mosaicml-cli-0.3.4/mcli/objects/integrations/git_repo.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3491 2022-09-23 00:37:17.000000 mosaicml-cli-0.3.4/mcli/objects/integrations/local.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2126 2022-12-01 00:52:00.000000 mosaicml-cli-0.3.4/mcli/objects/integrations/mosaicml_agent.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      810 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/objects/integrations/pip_packages.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2742 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/objects/integrations/wandb.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.031026 mosaicml-cli-0.3.4/mcli/objects/secrets/
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1090 2022-12-09 18:28:49.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4913 2022-10-27 20:22:32.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/cluster_secret.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.036174 mosaicml-cli-0.3.4/mcli/objects/secrets/create/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/create/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3953 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/create/base.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3461 2022-12-09 18:28:49.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/create/docker_registry.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2406 2022-11-30 21:02:34.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/create/gcp.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     7554 2022-11-04 23:17:49.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/create/generic.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3855 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/create/oci.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2998 2022-09-19 22:17:10.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/create/s3.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6701 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/create/ssh.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3782 2022-09-19 22:17:10.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/docker_registry.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1634 2022-09-19 22:17:10.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/env_var.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1122 2022-12-13 00:59:45.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/gcp.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2893 2022-10-03 22:11:44.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/mounted.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2855 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/oci.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2577 2022-09-19 22:17:10.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/s3.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3952 2022-11-30 21:02:34.000000 mosaicml-cli-0.3.4/mcli/objects/secrets/ssh.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.038576 mosaicml-cli-0.3.4/mcli/sdk/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      586 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/sdk/__init__.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.039388 mosaicml-cli-0.3.4/mcli/serverside/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/serverside/__init__.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.044652 mosaicml-cli-0.3.4/mcli/serverside/clusters/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      381 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    11245 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/cluster.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    23072 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/cluster_instances.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4005 2022-10-27 20:22:32.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/cluster_pv_setup.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2793 2022-09-27 00:07:54.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/gpu_type.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2824 2023-01-26 01:45:43.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/instance_type.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.062644 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1603 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      548 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/microk8s.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2219 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r10z1.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2822 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r1z1.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2495 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r1z4.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2759 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r3z1.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5355 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r4z1.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1049 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z1.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1161 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z10.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     2497 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z2.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1062 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z3.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1034 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z4.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1047 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z5.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1047 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z6.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1214 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z7.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1242 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z9.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1034 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r8z1.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1071 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r8z2.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1054 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r8z3.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1061 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r99z1.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      310 2022-09-20 00:08:28.000000 mosaicml-cli-0.3.4/mcli/serverside/clusters/volumekind.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.077676 mosaicml-cli-0.3.4/mcli/serverside/job/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/serverside/job/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    15654 2023-04-07 22:48:37.000000 mosaicml-cli-0.3.4/mcli/serverside/job/mcli_job.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      465 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/serverside/job/mcli_k8s_config_map_typing.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6471 2023-02-01 21:37:29.000000 mosaicml-cli-0.3.4/mcli/serverside/job/mcli_k8s_job.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     8090 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/serverside/job/mcli_k8s_job_typing.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     7524 2022-10-06 23:40:35.000000 mosaicml-cli-0.3.4/mcli/serverside/job/mcli_k8s_resource_requirements_typing.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      459 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/serverside/job/mcli_k8s_service_typing.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.080840 mosaicml-cli-0.3.4/mcli/serverside/runners/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/serverside/runners/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5770 2022-12-13 00:59:45.000000 mosaicml-cli-0.3.4/mcli/serverside/runners/runner.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.120324 mosaicml-cli-0.3.4/mcli/utils/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/utils/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     5306 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/utils/utils_cli.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6066 2023-04-07 22:48:37.000000 mosaicml-cli-0.3.4/mcli/utils/utils_config.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      740 2022-09-23 00:37:17.000000 mosaicml-cli-0.3.4/mcli/utils/utils_date.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    10453 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/utils/utils_docker.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    12947 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/utils/utils_epilog.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      751 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/utils/utils_file.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    11769 2022-12-09 18:28:49.000000 mosaicml-cli-0.3.4/mcli/utils/utils_interactive.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    49322 2022-11-14 21:21:56.000000 mosaicml-cli-0.3.4/mcli/utils/utils_kube.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6980 2023-02-01 21:37:29.000000 mosaicml-cli-0.3.4/mcli/utils/utils_kube_labels.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4741 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/utils/utils_logging.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)      359 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/utils/utils_modules.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6614 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/utils/utils_pypi.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6513 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/utils/utils_rancher.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3115 2022-09-08 17:54:07.000000 mosaicml-cli-0.3.4/mcli/utils/utils_rich.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     8533 2022-12-01 00:52:00.000000 mosaicml-cli-0.3.4/mcli/utils/utils_run_status.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     4350 2022-09-09 21:35:49.000000 mosaicml-cli-0.3.4/mcli/utils/utils_serializable_dataclass.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1103 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/utils/utils_spinner.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)    11437 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/mcli/utils/utils_string_functions.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3954 2022-11-30 21:02:34.000000 mosaicml-cli-0.3.4/mcli/utils/utils_types.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1001 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/mcli/utils/utils_yaml.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3884 2023-04-07 22:49:18.000000 mosaicml-cli-0.3.4/mcli/version.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.126172 mosaicml-cli-0.3.4/mosaicml_cli.egg-info/
+-rw-r--r--   0 jeffchen   (501) staff       (20)      696 2023-04-07 22:51:47.000000 mosaicml-cli-0.3.4/mosaicml_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jeffchen   (501) staff       (20)     7139 2023-04-07 22:51:47.000000 mosaicml-cli-0.3.4/mosaicml_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jeffchen   (501) staff       (20)        1 2023-04-07 22:51:47.000000 mosaicml-cli-0.3.4/mosaicml_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jeffchen   (501) staff       (20)       75 2023-04-07 22:51:47.000000 mosaicml-cli-0.3.4/mosaicml_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jeffchen   (501) staff       (20)     1630 2023-04-07 22:51:47.000000 mosaicml-cli-0.3.4/mosaicml_cli.egg-info/requires.txt
+-rw-r--r--   0 jeffchen   (501) staff       (20)       11 2023-04-07 22:51:47.000000 mosaicml-cli-0.3.4/mosaicml_cli.egg-info/top_level.txt
+-rw-r--r--   0 jeffchen   (501) staff       (20)    30933 2022-12-14 22:12:45.000000 mosaicml-cli-0.3.4/pyproject.toml
+-rw-r--r--   0 jeffchen   (501) staff       (20)       38 2023-04-07 22:51:48.143287 mosaicml-cli-0.3.4/setup.cfg
+-rw-r--r--   0 jeffchen   (501) staff       (20)     3111 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/setup.py
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.134228 mosaicml-cli-0.3.4/tests/
+drwxr-xr-x   0 jeffchen   (501) staff       (20)        0 2023-04-07 22:51:48.139120 mosaicml-cli-0.3.4/tests/submit/
+-rw-r--r--   0 jeffchen   (501) staff       (20)        0 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/tests/submit/__init__.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6393 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/tests/submit/test_cluster.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     9266 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/tests/submit/test_cluster_secrets.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     7973 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/tests/test_config.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)       62 2022-09-07 04:52:30.000000 mosaicml-cli-0.3.4/tests/test_simple.py
+-rw-r--r--   0 jeffchen   (501) staff       (20)     6116 2023-04-05 00:11:39.000000 mosaicml-cli-0.3.4/tests/test_upgrade.py
```

### Comparing `mosaicml-cli-0.3.3/PKG-INFO` & `mosaicml-cli-0.3.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.3.3
+Version: 0.3.4
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.3.3/README.md` & `mosaicml-cli-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/cluster/api_get_clusters.py` & `mosaicml-cli-0.3.4/mcli/api/cluster/api_get_clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/engine/engine.py` & `mosaicml-cli-0.3.4/mcli/api/engine/engine.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/engine/utils.py` & `mosaicml-cli-0.3.4/mcli/api/engine/utils.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/exceptions.py` & `mosaicml-cli-0.3.4/mcli/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/inference_deployments/__init__.py` & `mosaicml-cli-0.3.4/mcli/api/inference_deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/inference_deployments/api_create_inference_deployment.py` & `mosaicml-cli-0.3.4/mcli/api/inference_deployments/api_create_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/inference_deployments/api_delete_inference_deployments.py` & `mosaicml-cli-0.3.4/mcli/api/inference_deployments/api_delete_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/inference_deployments/api_get_inference_deployments.py` & `mosaicml-cli-0.3.4/mcli/api/inference_deployments/api_get_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/inference_deployments/api_ping_inference_deployment.py` & `mosaicml-cli-0.3.4/mcli/api/inference_deployments/api_ping_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/inference_deployments/api_predict_inference_deployment.py` & `mosaicml-cli-0.3.4/mcli/api/inference_deployments/api_predict_inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/kube/runs/__init__.py` & `mosaicml-cli-0.3.4/mcli/api/kube/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/kube/runs/api_create_run.py` & `mosaicml-cli-0.3.4/mcli/api/kube/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/kube/runs/api_delete_runs.py` & `mosaicml-cli-0.3.4/mcli/api/kube/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/kube/runs/api_get_run_logs.py` & `mosaicml-cli-0.3.4/mcli/api/kube/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/kube/runs/api_get_runs.py` & `mosaicml-cli-0.3.4/mcli/api/kube/runs/api_get_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/kube/runs/api_stop_runs.py` & `mosaicml-cli-0.3.4/mcli/api/kube/runs/api_stop_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/kube/runs/api_watch_run.py` & `mosaicml-cli-0.3.4/mcli/api/kube/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/mint/shell.py` & `mosaicml-cli-0.3.4/mcli/api/mint/shell.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/mint/tty.py` & `mosaicml-cli-0.3.4/mcli/api/mint/tty.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/model/cluster_details.py` & `mosaicml-cli-0.3.4/mcli/api/model/cluster_details.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/model/inference_deployment.py` & `mosaicml-cli-0.3.4/mcli/api/model/inference_deployment.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/runs/__init__.py` & `mosaicml-cli-0.3.4/mcli/api/runs/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/runs/api_create_run.py` & `mosaicml-cli-0.3.4/mcli/api/runs/api_create_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/runs/api_delete_runs.py` & `mosaicml-cli-0.3.4/mcli/api/runs/api_delete_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/runs/api_get_run_logs.py` & `mosaicml-cli-0.3.4/mcli/api/runs/api_get_run_logs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/runs/api_get_runs.py` & `mosaicml-cli-0.3.4/mcli/api/runs/api_get_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/runs/api_stop_runs.py` & `mosaicml-cli-0.3.4/mcli/api/runs/api_stop_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/runs/api_watch_run.py` & `mosaicml-cli-0.3.4/mcli/api/runs/api_watch_run.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/schema/generic_model.py` & `mosaicml-cli-0.3.4/mcli/api/schema/generic_model.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/secrets/api_create_secret.py` & `mosaicml-cli-0.3.4/mcli/api/secrets/api_create_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/secrets/api_delete_secrets.py` & `mosaicml-cli-0.3.4/mcli/api/secrets/api_delete_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/secrets/api_get_secrets.py` & `mosaicml-cli-0.3.4/mcli/api/secrets/api_get_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/typing_future.py` & `mosaicml-cli-0.3.4/mcli/api/typing_future.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/api/users/api_get_users.py` & `mosaicml-cli-0.3.4/mcli/api/users/api_get_users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/cli.py` & `mosaicml-cli-0.3.4/mcli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/common/deployment_filters.py` & `mosaicml-cli-0.3.4/mcli/cli/common/deployment_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/common/run_filters.py` & `mosaicml-cli-0.3.4/mcli/cli/common/run_filters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_clean/m_clean.py` & `mosaicml-cli-0.3.4/mcli/cli/m_clean/m_clean.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_connect/m_connect.py` & `mosaicml-cli-0.3.4/mcli/cli/m_connect/m_connect.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_create/cluster.py` & `mosaicml-cli-0.3.4/mcli/cli/m_create/cluster.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_create/env_var.py` & `mosaicml-cli-0.3.4/mcli/cli/m_create/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_create/m_create.py` & `mosaicml-cli-0.3.4/mcli/cli/m_create/m_create.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_create/secret.py` & `mosaicml-cli-0.3.4/mcli/cli/m_create/secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_delete/delete.py` & `mosaicml-cli-0.3.4/mcli/cli/m_delete/delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_delete/m_delete.py` & `mosaicml-cli-0.3.4/mcli/cli/m_delete/m_delete.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_deploy/m_deploy.py` & `mosaicml-cli-0.3.4/mcli/cli/m_deploy/m_deploy.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_describe/describe_inference_deployments.py` & `mosaicml-cli-0.3.4/mcli/cli/m_describe/describe_inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_describe/describe_runs.py` & `mosaicml-cli-0.3.4/mcli/cli/m_describe/describe_runs.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_describe/m_describe.py` & `mosaicml-cli-0.3.4/mcli/cli/m_describe/m_describe.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_get/__init__.py` & `mosaicml-cli-0.3.4/mcli/cli/m_get/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_get/clusters.py` & `mosaicml-cli-0.3.4/mcli/cli/m_get/clusters.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_get/display.py` & `mosaicml-cli-0.3.4/mcli/cli/m_get/display.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_get/envvars.py` & `mosaicml-cli-0.3.4/mcli/cli/m_get/envvars.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_get/inference_deployments.py` & `mosaicml-cli-0.3.4/mcli/cli/m_get/inference_deployments.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_get/m_get.py` & `mosaicml-cli-0.3.4/mcli/cli/m_get/m_get.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_get/runs.py` & `mosaicml-cli-0.3.4/mcli/cli/m_get/runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     def from_run(cls, run: Run, include_ids: bool = False) -> RunDisplayItem:
         display_status = run.status.display_name
         if run.reason:
             display_status = f"{display_status} ({run.reason})"
         extracted: Dict[str, str] = {
             RunColumns.NAME.value: run.name,
             RunColumns.CLUSTER.value: run.config.cluster,
-            RunColumns.GPU_TYPE.value: run.config.gpu_type,
+            RunColumns.GPU_TYPE.value: run.config.gpu_type or run.config.compute.get('gpu_type', None) or 'Unknown',
             RunColumns.GPU_NUM.value: str(run.config.gpu_num),
             RunColumns.CREATED_TIME.value: format_timestamp(run.created_at),
             RunColumns.START_TIME.value: format_timestamp(run.started_at),
             RunColumns.END_TIME.value: format_timestamp(run.completed_at),
             RunColumns.USER.value: run.created_by,
             RunColumns.STATUS.value: display_status
         }
```

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_get/secrets.py` & `mosaicml-cli-0.3.4/mcli/cli/m_get/secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_get/users.py` & `mosaicml-cli-0.3.4/mcli/cli/m_get/users.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_init/m_init.py` & `mosaicml-cli-0.3.4/mcli/cli/m_init/m_init.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_init/m_init_kube.py` & `mosaicml-cli-0.3.4/mcli/cli/m_init/m_init_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_interactive/interactive.py` & `mosaicml-cli-0.3.4/mcli/cli/m_interactive/interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_interactive/m_interactive.py` & `mosaicml-cli-0.3.4/mcli/cli/m_interactive/m_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_interactive/temp_mcloud_interactive.py` & `mosaicml-cli-0.3.4/mcli/cli/m_interactive/temp_mcloud_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_log/m_log.py` & `mosaicml-cli-0.3.4/mcli/cli/m_log/m_log.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_ping/m_ping.py` & `mosaicml-cli-0.3.4/mcli/cli/m_ping/m_ping.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_predict/m_predict.py` & `mosaicml-cli-0.3.4/mcli/cli/m_predict/m_predict.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_root/m_config.py` & `mosaicml-cli-0.3.4/mcli/cli/m_root/m_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_run/m_run.py` & `mosaicml-cli-0.3.4/mcli/cli/m_run/m_run.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,16 @@
     override_cluster: Optional[str] = None,
     override_gpu_type: Optional[str] = None,
     override_gpu_num: Optional[int] = None,
     override_image: Optional[str] = None,
     override_name: Optional[str] = None,
     override_optimization_level: Optional[int] = None,
     override_priority: Optional[str] = None,
+    override_nodes: Optional[int] = None,
+    override_instance: Optional[str] = None,
     **kwargs,
 ) -> int:
     del kwargs
 
     cluster_name: Optional[str] = None
     try:
         if file:
@@ -112,34 +114,40 @@
             run_config = run.submitted_config
         else:
             return print_help()
 
         # command line overrides
         # only supports basic format for now and not structured params
         if override_cluster is not None:
-            run_config.cluster = override_cluster
+            run_config.compute['cluster'] = override_cluster
 
         if override_gpu_type is not None:
-            run_config.gpu_type = override_gpu_type
+            run_config.compute['gpu_type'] = override_gpu_type
 
         if override_gpu_num is not None:
-            run_config.gpu_num = override_gpu_num
+            run_config.compute['gpus'] = override_gpu_num
 
         if override_image is not None:
             run_config.image = override_image
 
         if override_name is not None:
             run_config.name = override_name
 
         if override_optimization_level is not None:
             run_config.optimization_level = override_optimization_level
 
         if override_priority is not None:
             run_config.scheduling['priority'] = override_priority
 
+        if override_instance is not None:
+            run_config.compute['instance'] = override_instance
+
+        if override_nodes is not None:
+            run_config.compute['nodes'] = override_nodes
+
         conf = MCLIConfig.load_config(safe=True)
 
         with console_status('Submitting run...'):
             if conf.feature_enabled(FeatureFlag.USE_MCLOUD):
                 # TODO: Move this out when legacy priority is removed
 
                 run = create_run(run=run_config, timeout=None)
@@ -268,14 +276,28 @@
     parser.add_argument(
         '--name',
         '--run-name',
         dest='override_name',
         help='Optional override for run name',
     )
 
+    parser.add_argument(
+        '--nodes',
+        type=int,
+        dest='override_nodes',
+        help='Optional override for number of nodes. '
+        'Valid node numbers depend on the cluster and instance type',
+    )
+
+    parser.add_argument(
+        '--instance',
+        dest='override_instance',
+        help='Optional override for instance type',
+    )
+
     conf = MCLIConfig.load_config(safe=True)
     if conf.internal:
         parser.add_argument(
             '-o',
             '--optimization_level',
             dest='override_optimization_level',
             choices=VALID_OPTIMIZATION_LEVELS,
```

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_set_unset/api_key.py` & `mosaicml-cli-0.3.4/mcli/cli/m_set_unset/api_key.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_set_unset/m_set.py` & `mosaicml-cli-0.3.4/mcli/cli/m_set_unset/m_set.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_set_unset/m_unset.py` & `mosaicml-cli-0.3.4/mcli/cli/m_set_unset/m_unset.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_set_unset/user.py` & `mosaicml-cli-0.3.4/mcli/cli/m_set_unset/user.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_stop/m_stop.py` & `mosaicml-cli-0.3.4/mcli/cli/m_stop/m_stop.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_use/m_use.py` & `mosaicml-cli-0.3.4/mcli/cli/m_use/m_use.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_util/kube_util.py` & `mosaicml-cli-0.3.4/mcli/cli/m_util/kube_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_util/m_util.py` & `mosaicml-cli-0.3.4/mcli/cli/m_util/m_util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/cli/m_util/util.py` & `mosaicml-cli-0.3.4/mcli/cli/m_util/util.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/config.py` & `mosaicml-cli-0.3.4/mcli/config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/models/__init__.py` & `mosaicml-cli-0.3.4/mcli/models/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/models/inference_deployment_config.py` & `mosaicml-cli-0.3.4/mcli/models/inference_deployment_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """ Deployment Input """
 from __future__ import annotations
 
 import logging
 from dataclasses import asdict, dataclass, field
 from http import HTTPStatus
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 import yaml
 
 from mcli.api.exceptions import MAPIException, MCLIDeploymentConfigValidationError
 from mcli.api.schema.generic_model import DeserializableModel
 from mcli.models.run_config import _clean_run_name, _validate_cluster_exists
-from mcli.utils.utils_config import BaseSubmissionConfig, uuid_generator
+from mcli.utils.utils_config import BaseSubmissionConfig, EnvVarTranslation, IntegrationTranslation, uuid_generator
 from mcli.utils.utils_string_functions import validate_image
 
 logger = logging.getLogger(__name__)
 
 DEPLOYMENT_CONFIG_UID_LENGTH = 6
 
 
@@ -27,14 +27,17 @@
     """
 
     deployment_id: str
     name: str
     gpu_num: int
     image: str
     replicas: int
+    env_variables: List[Dict[str, str]]
+    integrations: List[Dict[str, Any]]
+
     metadata: Dict[str, Any] = field(default_factory=dict)
 
     gpu_type: str = ''
     command: str = ''
 
     cluster: str = ''
 
@@ -44,36 +47,48 @@
         'gpuType': 'gpu_type',
         'gpuNum': 'gpu_num',
         'cluster': 'cluster',
         'image': 'image',
         'command': 'command',
         'replicas': 'replicas',
         'metadata': 'metadata',
+        'envVariables': 'env_variables',
+        'integrations': 'integrations',
     }
 
     def __str__(self) -> str:
         return yaml.safe_dump(asdict(self))
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> FinalInferenceDeploymentConfig:
 
         # Backwards Compatability
         if 'metadata' not in response:
             response['metadata'] = {}
 
+        if 'envVariables' not in response:
+            response['envVariables'] = []
+
+        if 'integrations' not in response:
+            response['integrations'] = []
+
         missing = set(cls._property_translations) - set(response)
         if missing:
             raise MAPIException(
                 status=HTTPStatus.BAD_REQUEST,
                 message=('Missing required key(s) in response to deserialize '
                          f'FinalDeploymentConfig object: {", ".join(missing)}'),
             )
         data = {}
         for k, v in cls._property_translations.items():
             value = response[k]
+            if v == 'env_variables':
+                value = EnvVarTranslation.from_mapi(value)
+            elif v == 'integrations':
+                value = IntegrationTranslation.from_mapi(value)
             data[v] = value
 
         return cls(**data)
 
     @classmethod
     def finalize_config(cls, deployment_config: InferenceDeploymentConfig) -> FinalInferenceDeploymentConfig:
         """Create a :class:`~mcli.models.deployment_config.FinalDeploymentConfig` from the provided
@@ -132,17 +147,21 @@
             Dict[str, Dict[str, Any]]: The deployment configuration as a MAPI deploymentInput JSON
         """
         translations = {v: k for k, v in self._property_translations.items()}
 
         translated_input = {}
         for field_name, value in asdict(self).items():
             translated_name = translations.get(field_name, field_name)
-            if field_name == "gpu_type" and not value:
+            if field_name == 'env_variables':
+                value = EnvVarTranslation.to_mapi(value)
+            elif field_name == 'integrations':
+                value = IntegrationTranslation.to_mapi(value)
+            elif field_name == "gpu_type" and not value:
                 continue
-            if field_name == "cluster" and not value:
+            elif field_name == "cluster" and not value:
                 continue
             translated_input[translated_name] = value
         return {
             'inferenceDeploymentInput': translated_input,
         }
 
 
@@ -154,40 +173,50 @@
         name (`Optional[str]`): User-defined name of the deployment
         gpu_type (`Optional[str]`): GPU type (optional if only one gpu type for your cluster)
         gpu_num (`Optional[int]`): Number of GPUs
         cluster (`Optional[str]`): Cluster to use (optional if you only have one)
         image (`Optional[str]`): Docker image (e.g. `mosaicml/composer`)
         command (`str`): Command to use when a deployment starts
         replicas (`Optional[int]`): Number of replicas to create
+        env_variables (`List[Dict[str, str]]`): List of environment variables
+        integrations (`List[Dict[str, Any]]`): List of integrations
     """
     name: Optional[str] = None
     gpu_type: Optional[str] = None
     gpu_num: Optional[int] = None
     cluster: Optional[str] = None
     image: Optional[str] = None
     replicas: Optional[int] = None
     command: Optional[str] = None
     metadata: Optional[Dict[str, Any]] = None
+    env_variables: List[Dict[str, str]] = field(default_factory=list)
+    integrations: List[Dict[str, Any]] = field(default_factory=list)
 
     _property_translations = {
         'deploymentName': 'name',
         'gpuNum': 'gpu_num',
         'cluster': 'cluster',
         'image': 'image',
         'command': 'command',
         'replicas': 'replicas',
         'metadata': 'metadata',
+        'envVariables': 'env_variables',
+        'integrations': 'integrations',
     }
 
-    _optional_display_properties = {'gpu_type', 'metadata'}
+    _optional_display_properties = {'gpu_type', 'metadata', 'env_variables', 'integrations'}
 
     @classmethod
     def from_mapi_response(cls, response: Dict[str, Any]) -> InferenceDeploymentConfig:
         data = {}
         for k, v in cls._property_translations.items():
             if k not in response:
                 # This must be an optional property, so skip
                 continue
             value = response[k]
+            if v == 'env_variables':
+                value = EnvVarTranslation.from_mapi(value)
+            elif v == 'integrations':
+                value = IntegrationTranslation.from_mapi(value)
             data[v] = value
 
         return cls(**data)
```

### Comparing `mosaicml-cli-0.3.3/mcli/models/mcli_cluster.py` & `mosaicml-cli-0.3.4/mcli/models/mcli_cluster.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/models/mcli_envvar.py` & `mosaicml-cli-0.3.4/mcli/models/mcli_envvar.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/models/mcli_integration.py` & `mosaicml-cli-0.3.4/mcli/models/mcli_integration.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/models/mcli_secret.py` & `mosaicml-cli-0.3.4/mcli/models/mcli_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/models/run_config.py` & `mosaicml-cli-0.3.4/mcli/models/run_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,92 @@
 """ Run Input """
 from __future__ import annotations
 
-import copy
 import logging
-from abc import ABC, abstractmethod
 from dataclasses import asdict, dataclass, field
 from http import HTTPStatus
-from typing import Any, Dict, Generic, List, Optional, Sequence, TypeVar
+from typing import Any, Dict, List, Optional, Sequence
 
 import yaml
 from typing_extensions import TypedDict
 
 from mcli.api.exceptions import MAPIException, MCLIRunConfigValidationError
 from mcli.api.schema.generic_model import DeserializableModel
 from mcli.models.mcli_cluster import Cluster
-from mcli.serverside.clusters.cluster_instances import (IncompleteInstanceRequest, InstanceRequest,
-                                                        UserInstanceRegistry, ValidInstance)
-from mcli.utils.utils_config import BaseSubmissionConfig, uuid_generator
-from mcli.utils.utils_string_functions import (MAX_KUBERNETES_LENGTH, camel_case_to_snake_case,
-                                               ensure_rfc1123_compatibility, snake_case_to_camel_case, validate_image,
+from mcli.utils.utils_config import (BaseSubmissionConfig, EnvVarTranslation, IntegrationTranslation, Translation,
+                                     uuid_generator)
+from mcli.utils.utils_string_functions import (MAX_KUBERNETES_LENGTH, ensure_rfc1123_compatibility, validate_image,
                                                validate_rfc1123_name)
 
 logger = logging.getLogger(__name__)
 RUN_CONFIG_UID_LENGTH = 6
 VALID_OPTIMIZATION_LEVELS = frozenset([0, 1, 2, 3])
 MAX_RUN_NAME_LENGTH = MAX_KUBERNETES_LENGTH - RUN_CONFIG_UID_LENGTH - 1  # -1 for the dash
 
 
 class SchedulingConfig(TypedDict):
     """Typed dictionary for nested scheduling configurations"""
     priority: Optional[str]
 
 
+class ComputeConfig(TypedDict):
+    """Typed dictionary for nested compute requests"""
+    cluster: Optional[str]
+    instance: Optional[str]
+    nodes: Optional[int]
+    gpu_type: Optional[str]
+    gpus: Optional[int]
+    cpus: Optional[int]
+
+
+def strip_nones(d: Dict[str, Any]) -> Dict[str, Any]:
+    """Remove all keys with None values from a dictionary"""
+    return {k: v for k, v in d.items() if v is not None}
+
+
 @dataclass
 class FinalRunConfig(DeserializableModel):
     """A finalized run configuration
 
     This configuration must be complete, with enough details to submit a new run to the
     MosaicML platform.
     """
 
     run_id: str
     name: str
-    gpu_num: int
     cpus: int
     image: str
     integrations: List[Dict[str, Any]]
     env_variables: List[Dict[str, str]]
 
     parameters: Dict[str, Any]
 
-    gpu_type: str = ''
+    gpu_type: Optional[str] = None  # deprecating in favor of compute['gpu_type']
+    gpu_num: Optional[int] = None  # deprecating in favor of compute['gpus']
+
     optimization_level: int = 0
     # Make both optional for initial rollout
     # Eventually make entrypoint required and deprecate command
     command: str = ''
     entrypoint: str = ''
 
     # Platform is deprecated, but not required for backwards compatibility
     cluster: str = ''
     platform: str = ''
 
     # Partition is an optional new keyword
     partitions: Optional[List[str]] = None
 
     # Scheduling parameters - optional for backwards-compatibility
-    scheduling: SchedulingConfig = field(default_factory=lambda: SchedulingConfig(priority=None))
+    # pylint: disable-next=unnecessary-lambda
+    scheduling: SchedulingConfig = field(default_factory=lambda: SchedulingConfig(**{}))
+
+    # Compute parameters - optional for backwards-compatibility
+    # pylint: disable-next=unnecessary-lambda
+    compute: ComputeConfig = field(default_factory=lambda: ComputeConfig(**{}))
 
     _property_translations = {
         'run_id': 'run_id',
         'runName': 'name',
         'gpuType': 'gpu_type',
         'gpuNum': 'gpu_num',
         'cpus': 'cpus',
@@ -78,19 +95,21 @@
         'optimizationLevel': 'optimization_level',
         'integrations': 'integrations',
         'envVariables': 'env_variables',
         'parameters': 'parameters',
         'command': 'command',
         'entrypoint': 'entrypoint',
         'scheduling': 'scheduling',
+        'compute': 'compute',
     }
 
     _optional_properties = {
         'partitions',
         'scheduling',
+        'compute',
     }
 
     def __str__(self) -> str:
         return yaml.safe_dump(asdict(self))
 
     def __post_init__(self):
         self.cluster = self.cluster or self.platform
@@ -112,14 +131,16 @@
             value = response[k]
             if v == 'env_variables':
                 value = EnvVarTranslation.from_mapi(value)
             elif v == 'integrations':
                 value = IntegrationTranslation.from_mapi(value)
             elif v == 'scheduling':
                 value = SchedulingTranslation.from_mapi(value)
+            elif v == 'compute':
+                value = ComputeTranslation.from_mapi(value)
             data[v] = value
 
         return cls(**data)
 
     @classmethod
     def finalize_config(cls, run_config: RunConfig) -> FinalRunConfig:  # pylint: disable=too-many-statements
         """Create a :class:`~mcli.models.run_config.FinalRunConfig` from the provided
@@ -135,15 +156,15 @@
             :class:`~mcli.models.run_config.FinalRunConfig`: The object created using values from the input
 
         Raises:
             :class:`~mcli.api.exceptions.MCLIConfigError`: If MCLI config is not present or is missing information
             :class:`~mcli.api.exceptions.MCLIRunConfigValidationError`: If run_config is not valid
         """
         # pylint: disable-next=import-outside-toplevel
-        from mcli.config import FeatureFlag, MCLIConfig
+        from mcli.config import MCLIConfig
         conf = MCLIConfig.load_config(safe=True)
 
         if run_config.cpus is None:
             run_config.cpus = 0
 
         # MosaicML Agent is disabled for all external users
         if not conf.internal or run_config.optimization_level is None:
@@ -155,68 +176,22 @@
         if run_config.partitions is not None:
             # Validate provided partition is a list of strings
             if not isinstance(run_config.partitions, Sequence):
                 run_config.partitions = [str(run_config.partitions)]
             else:
                 run_config.partitions = [str(p) for p in run_config.partitions]
 
-        if run_config.cluster:
-            _validate_cluster_exists(run_config.cluster)
-
-        # Try to infer values from provided
-        if not all((
-                run_config.cluster,
-                run_config.gpu_type,
-                run_config.gpu_num is not None,
-        )) and not conf.feature_enabled(FeatureFlag.USE_MCLOUD):
-            request = InstanceRequest(cluster=run_config.cluster,
-                                      gpu_type=run_config.gpu_type,
-                                      gpu_num=run_config.gpu_num)
-            logger.debug(f'Incomplete instance request: {request}')
-            user_instances = UserInstanceRegistry()
-            options = user_instances.lookup(request)
-            if len(options) == 1:
-                valid_instance = options[0]
-                logger.debug(f'Inferred a valid instance request: {valid_instance}')
-                run_config.cluster = valid_instance.cluster
-                run_config.gpu_type = valid_instance.gpu_type
-                run_config.gpu_num = valid_instance.gpu_num
-            else:
-                valid_registry = ValidInstance.to_registry(options)
-                incomplete_instance_error = IncompleteInstanceRequest(
-                    requested=request,
-                    options=valid_registry,
-                    registry=user_instances.registry,
-                )
-                raise MCLIRunConfigValidationError(str(incomplete_instance_error))
-
         model_as_dict = asdict(run_config)
 
         # Remove deprecated run_name
         model_as_dict.pop('run_name', None)
 
         # Remove deprecated platform
         model_as_dict.pop('platform', None)
-
-        missing_fields = [
-            field for field, value in model_as_dict.items() if value is None and field not in cls._optional_properties
-        ]
-        if conf.feature_enabled(FeatureFlag.USE_MCLOUD):
-            for missing in missing_fields:
-                model_as_dict.pop(missing, None)
-
-            # required for FinalRunConfig, even though not required for mcloud
-            if not model_as_dict.get("gpu_num"):
-                model_as_dict["gpu_num"] = 0
-
-        elif len(missing_fields) > 0:
-            raise MCLIRunConfigValidationError(
-                f'Cannot construct run because of missing field(s): {", ".join(missing_fields)}'
-                '\nPlease pass the missing fields either through the yaml file or as command line arguments')
-            # TODO: we could give the user what they should add to their yaml file directly
+        model_as_dict = strip_nones(model_as_dict)
 
         # Fill in default initial values for FinalRunConfig
         model_as_dict.update({
             'run_id': uuid_generator(RUN_CONFIG_UID_LENGTH),
         })
 
         model_as_dict['name'] = _clean_run_name(model_as_dict.get('name'))
@@ -258,130 +233,40 @@
         Returns:
             Dict[str, Dict[str, Any]]: The run configuration as a MAPI runInput JSON
         """
         translations = {v: k for k, v in self._property_translations.items()}
 
         translated_input = {}
         for field_name, value in asdict(self).items():
+            if value is None:
+                continue
             translated_name = translations.get(field_name, field_name)
             if field_name == 'env_variables':
                 value = EnvVarTranslation.to_mapi(value)
             elif field_name == 'integrations':
                 value = IntegrationTranslation.to_mapi(value)
             elif field_name == "scheduling":
                 value = SchedulingTranslation.to_mapi(value)
+            elif field_name == "compute":
+                value = ComputeTranslation.to_mapi(value)
             elif field_name == "gpu_type" and not value:
                 continue
             elif field_name == "cluster" and not value:
                 continue
             elif field_name == "platform":
                 continue
+            elif isinstance(value, dict):
+                value = strip_nones(value)
 
             translated_input[translated_name] = value
         return {
             'runInput': translated_input,
         }
 
 
-T = TypeVar('T')  # pylint: disable=invalid-name
-U = TypeVar('U')
-
-
-class Translation(ABC, Generic[T, U]):
-    """ABC for MAPI/MCLI translations"""
-
-    @classmethod
-    @abstractmethod
-    def to_mapi(cls, value: T) -> U:
-        ...
-
-    @classmethod
-    @abstractmethod
-    def from_mapi(cls, value: U) -> T:
-        ...
-
-
-class EnvVarTranslation(Translation[List[Dict[str, str]], List[Dict[str, str]]]):
-    """Translate environment variable configs"""
-
-    MAPI_KEY = 'envKey'
-    MAPI_VALUE = 'envValue'
-
-    MCLI_KEY = 'key'
-    MCLI_VALUE = 'value'
-
-    @classmethod
-    def to_mapi(cls, value: List[Dict[str, str]]) -> List[Dict[str, str]]:
-        env_vars = []
-        for env_var in value:
-            try:
-                key = env_var[cls.MCLI_KEY]
-                val = env_var[cls.MCLI_VALUE]
-            except KeyError as e:
-                raise KeyError('Environment variables should be specified as a list '
-                               f'of dictionaries with keys: "{cls.MCLI_KEY}" and "{cls.MCLI_VALUE}". '
-                               f'Got: {", ".join(list(env_var.keys()))}') from e
-
-            env_vars.append({cls.MAPI_KEY: key, cls.MAPI_VALUE: val})
-        return env_vars
-
-    @classmethod
-    def from_mapi(cls, value: List[Dict[str, str]]) -> List[Dict[str, str]]:
-        env_vars = []
-        for env_var in value:
-            try:
-                key = env_var[cls.MAPI_KEY]
-                val = env_var[cls.MAPI_VALUE]
-            except KeyError:
-                logger.warning(f'Received incompatible environment variable: {env_var}')
-                continue
-            env_vars.append({cls.MCLI_KEY: key, cls.MCLI_VALUE: val})
-        return env_vars
-
-
-class IntegrationTranslation(Translation[List[Dict[str, Any]], List[Dict[str, Any]]]):
-    """Translate integration configs"""
-
-    MAPI_TYPE = 'type'
-    MAPI_PARAMS = 'params'
-
-    MCLI_TYPE = 'integration_type'
-
-    @classmethod
-    def to_mapi(cls, value: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
-        value = copy.deepcopy(value)
-        integrations_list = []
-        for integration in value:
-            integration_type = integration.pop(cls.MCLI_TYPE)
-
-            translated_integration = {}
-            for param, val in integration.items():
-                # Translate keys to camel case for MAPI parameters
-                translated_key = snake_case_to_camel_case(param)
-                translated_integration[translated_key] = val
-
-            integrations_dict = {cls.MAPI_TYPE: integration_type, cls.MAPI_PARAMS: translated_integration}
-            integrations_list.append(integrations_dict)
-        return integrations_list
-
-    @classmethod
-    def from_mapi(cls, value: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
-        integrations_list = []
-        for integration in value:
-            translated_integration = {cls.MCLI_TYPE: integration[cls.MAPI_TYPE]}
-            params = integration.get(cls.MAPI_PARAMS, {})
-            for param, val in params.items():
-                # Translate keys to camel case for MAPI parameters
-                translated_key = camel_case_to_snake_case(param)
-                translated_integration[translated_key] = val
-
-            integrations_list.append(translated_integration)
-        return integrations_list
-
-
 class SchedulingTranslation(Translation[SchedulingConfig, Dict[str, Any]]):
     """Translate scheduling configs to and from MAPI"""
 
     @classmethod
     def from_mapi(cls, value: Dict[str, Any]) -> SchedulingConfig:
         extracted: SchedulingConfig = {'priority': None}
         for k, v in value.items():
@@ -394,14 +279,33 @@
         processed: Dict[str, Any] = {}
         for k, v in value.items():
             if v is not None:
                 processed[k] = v
         return processed
 
 
+class ComputeTranslation(Translation[ComputeConfig, Dict[str, Any]]):
+    """Translate compute configs to and from MAPI"""
+
+    translations = {
+        "gpuType": "gpu_type",
+    }
+
+    @classmethod
+    def from_mapi(cls, value: Dict[str, Any]) -> ComputeConfig:
+        extracted = ComputeConfig(**{cls.translations.get(k, k): v for k, v in value.items()})
+        return extracted
+
+    @classmethod
+    def to_mapi(cls, value: ComputeConfig) -> Dict[str, Any]:
+        inv = {v: k for k, v in cls.translations.items()}
+        processed = {inv.get(k, k): v for k, v in value.items() if v is not None}
+        return processed
+
+
 def _clean_run_name(run_name: Optional[str]) -> str:
     if run_name is None:
         raise MCLIRunConfigValidationError('A run name must be provided using the keyword [bold]name[/]')
 
     name_validation = validate_rfc1123_name(text=run_name)
     if name_validation.valid:
         return run_name
@@ -474,15 +378,18 @@
     platform: Optional[str] = None
     cluster: Optional[str] = None
     image: Optional[str] = None
     partitions: Optional[List[str]] = None
     optimization_level: Optional[int] = None
     integrations: List[Dict[str, Any]] = field(default_factory=list)
     env_variables: List[Dict[str, str]] = field(default_factory=list)
-    scheduling: SchedulingConfig = field(default_factory=lambda: SchedulingConfig(priority=None))
+    # pylint: disable-next=unnecessary-lambda
+    scheduling: SchedulingConfig = field(default_factory=lambda: SchedulingConfig(**{}))
+    # pylint: disable-next=unnecessary-lambda
+    compute: ComputeConfig = field(default_factory=lambda: ComputeConfig(**{}))
 
     command: str = ''
     parameters: Dict[str, Any] = field(default_factory=dict)
     entrypoint: str = ''
 
     _property_translations = {
         'runName': 'name',
@@ -514,14 +421,16 @@
             value = response[k]
             if v == 'env_variables':
                 value = EnvVarTranslation.from_mapi(value)
             elif v == 'integrations':
                 value = IntegrationTranslation.from_mapi(value)
             elif v == 'scheduling':
                 value = SchedulingTranslation.from_mapi(value)
+            elif v == 'compute':
+                value = ComputeConfig(**value)
             data[v] = value
 
         return cls(**data)
 
     def __post_init__(self):
         self.name = self.name or self.run_name
         if self.run_name is not None:
```

### Comparing `mosaicml-cli-0.3.3/mcli/objects/integrations/__init__.py` & `mosaicml-cli-0.3.4/mcli/objects/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/integrations/apt_packages.py` & `mosaicml-cli-0.3.4/mcli/objects/integrations/apt_packages.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/integrations/comet.py` & `mosaicml-cli-0.3.4/mcli/objects/integrations/comet.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/integrations/git_repo.py` & `mosaicml-cli-0.3.4/mcli/objects/integrations/git_repo.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/integrations/local.py` & `mosaicml-cli-0.3.4/mcli/objects/integrations/local.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/integrations/mosaicml_agent.py` & `mosaicml-cli-0.3.4/mcli/objects/integrations/mosaicml_agent.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/integrations/pip_packages.py` & `mosaicml-cli-0.3.4/mcli/objects/integrations/pip_packages.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/integrations/wandb.py` & `mosaicml-cli-0.3.4/mcli/objects/integrations/wandb.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/__init__.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/cluster_secret.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/cluster_secret.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/create/base.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/create/base.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/create/docker_registry.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/create/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/create/gcp.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/create/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/create/generic.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/create/generic.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/create/oci.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/create/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/create/s3.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/create/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/create/ssh.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/create/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/docker_registry.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/docker_registry.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/env_var.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/env_var.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/gcp.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/gcp.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/mounted.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/mounted.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/oci.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/oci.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/s3.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/s3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/objects/secrets/ssh.py` & `mosaicml-cli-0.3.4/mcli/objects/secrets/ssh.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/sdk/__init__.py` & `mosaicml-cli-0.3.4/mcli/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/cluster.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/cluster.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/cluster_instances.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/cluster_instances.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/cluster_pv_setup.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/cluster_pv_setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/gpu_type.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/gpu_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/instance_type.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/instance_type.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/__init__.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/__init__.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/microk8s.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/microk8s.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r10z1.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r10z1.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r1z1.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r1z1.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r1z4.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r1z4.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r3z1.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r3z1.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r4z1.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r4z1.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z1.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z1.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z10.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z10.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z2.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z3.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z4.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z4.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z5.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z5.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z6.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z6.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z7.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z7.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r7z9.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r7z9.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r8z1.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r8z1.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r8z2.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r8z2.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r8z3.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r8z3.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/clusters/overrides/r99z1.py` & `mosaicml-cli-0.3.4/mcli/serverside/clusters/overrides/r99z1.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/job/mcli_job.py` & `mosaicml-cli-0.3.4/mcli/serverside/job/mcli_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,19 +85,19 @@
                 found_cluster = candidate_cluster
                 break
         clusters_available_str = ', '.join([x.name for x in mcli_config.clusters])
         assert found_cluster, (f'Unable to find cluster: {run_config.cluster}'
                                f' in registered clusters: {clusters_available_str}')
         cluster = GenericK8sCluster.from_mcli_cluster(found_cluster)
 
-        gpu_type = GPUType.from_string(run_config.gpu_type)
+        gpu_type = GPUType.from_string(run_config.gpu_type or run_config.compute.get('gpu_type', None) or 'None')
         try:
             instance_type = cluster.get_instance_type(
                 gpu_type=gpu_type,
-                gpu_num=run_config.gpu_num,
+                gpu_num=run_config.gpu_num or run_config.compute.get('gpus', None) or 0,
                 cpus=run_config.cpus,
             )
         except InstanceTypeUnavailable as it_unavailable_exception:
             it_unavailable_exception.current_cluster_name = cluster.mcli_cluster.name
             other_clusters = [
                 GenericK8sCluster.from_mcli_cluster(x) for x in mcli_config.clusters if x.name != run_config.cluster
             ]
```

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/job/mcli_k8s_job.py` & `mosaicml-cli-0.3.4/mcli/serverside/job/mcli_k8s_job.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/job/mcli_k8s_job_typing.py` & `mosaicml-cli-0.3.4/mcli/serverside/job/mcli_k8s_job_typing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/job/mcli_k8s_resource_requirements_typing.py` & `mosaicml-cli-0.3.4/mcli/serverside/job/mcli_k8s_resource_requirements_typing.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/serverside/runners/runner.py` & `mosaicml-cli-0.3.4/mcli/serverside/runners/runner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_cli.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_cli.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_date.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_date.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_docker.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_docker.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_epilog.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_epilog.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_file.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_file.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_interactive.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_interactive.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_kube.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_kube.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_kube_labels.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_kube_labels.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_logging.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_logging.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_pypi.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_pypi.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_rancher.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_rancher.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_rich.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_rich.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_run_status.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_run_status.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_serializable_dataclass.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_spinner.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_spinner.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_string_functions.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_string_functions.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_types.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_types.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/utils/utils_yaml.py` & `mosaicml-cli-0.3.4/mcli/utils/utils_yaml.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mcli/version.py` & `mosaicml-cli-0.3.4/mcli/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,13 +111,13 @@
 
 def print_version(**kwargs) -> None:
     """ Prints version """
     del kwargs
     print(get_formatted_version())
 
 
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 v = Version.from_string(__version__)
 __version_major__ = v.major
 __version_minor__ = v.minor
 __version_patch__ = v.patch
 __version_extras__ = v.extras
```

### Comparing `mosaicml-cli-0.3.3/mosaicml_cli.egg-info/PKG-INFO` & `mosaicml-cli-0.3.4/mosaicml_cli.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosaicml-cli
-Version: 0.3.3
+Version: 0.3.4
 Summary: Interact with the MosaicML platform from python or a command line interface
 Home-page: https://github.com/mosaicml/mosaicml-cli
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `mosaicml-cli-0.3.3/mosaicml_cli.egg-info/SOURCES.txt` & `mosaicml-cli-0.3.4/mosaicml_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/mosaicml_cli.egg-info/requires.txt` & `mosaicml-cli-0.3.4/mosaicml_cli.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -16,43 +16,43 @@
 jinja2
 arrow>=1.2.2
 slack-sdk>=3.17.1
 docker>=5.0.3
 gql[websockets]>=3.4.0
 
 [all]
-pytest-mock>=3.7.0
-sphinx-copybutton>=0.5.0
-pylint>=2.12.2
-pre-commit>=2.17.0
-myst-parser>=0.16.1
-sphinxcontrib-htmlhelp>=2.0.0
-sphinxcontrib-katex>=0.8.6
-pyright>=1.1.256
-sphinx_external_toc>=0.3.0
-sphinx-design
-pytest>=6.2.5
-sphinx-argparse>=0.3.1
-pytest-cov>=4.0.0
+sphinxcontrib-devhelp>=1.0.2
 sphinx-rtd-theme>=1.0.0
-isort>=5.9.3
-sphinxemoji>=0.2.0
+radon>=5.1.0
 sphinxcontrib-applehelp>=1.0.2
-sphinxcontrib-serializinghtml>=1.1.5
-sphinx-panels>=0.6.0
-yapf>=0.32.0
 sphinx-markdown-tables>=0.0.15
 sphinxext-opengraph>=0.6.1
-sphinxcontrib-images>=0.9.4
-sphinxcontrib-jsmath>=1.0.1
+pre-commit>=2.17.0
+sphinx-copybutton>=0.5.0
+sphinxemoji>=0.2.0
+sphinx-panels>=0.6.0
+pytest-mock>=3.7.0
+sphinxcontrib-htmlhelp>=2.0.0
+sphinx-argparse>=0.3.1
+sphinx_external_toc>=0.3.0
+pytest>=6.2.5
 sphinxcontrib-qthelp>=1.0.3
-radon>=5.1.0
-sphinxcontrib-devhelp>=1.0.2
 furo>=2022.3.4
+pytest-cov>=4.0.0
+myst-parser>=0.16.1
+sphinxcontrib-images>=0.9.4
+pylint>=2.12.2
+sphinxcontrib-katex>=0.8.6
 sphinx>=4.4.0
+pyright>=1.1.256
+yapf>=0.32.0
+isort>=5.9.3
+sphinx-design
+sphinxcontrib-jsmath>=1.0.1
+sphinxcontrib-serializinghtml>=1.1.5
 
 [dev]
 isort>=5.9.3
 pre-commit>=2.17.0
 pylint>=2.12.2
 pyright>=1.1.256
 pytest>=6.2.5
```

### Comparing `mosaicml-cli-0.3.3/pyproject.toml` & `mosaicml-cli-0.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/setup.py` & `mosaicml-cli-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/tests/submit/test_cluster.py` & `mosaicml-cli-0.3.4/tests/submit/test_cluster.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/tests/submit/test_cluster_secrets.py` & `mosaicml-cli-0.3.4/tests/submit/test_cluster_secrets.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/tests/test_config.py` & `mosaicml-cli-0.3.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mosaicml-cli-0.3.3/tests/test_upgrade.py` & `mosaicml-cli-0.3.4/tests/test_upgrade.py`

 * *Files identical despite different names*

