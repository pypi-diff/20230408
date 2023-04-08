# Comparing `tmp/windmill_api-1.85.0.tar.gz` & `tmp/windmill_api-1.86.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windmill_api-1.85.0.tar", max compression
+gzip compressed data, was "windmill_api-1.86.0.tar", max compression
```

## Comparing `windmill_api-1.85.0.tar` & `windmill_api-1.86.0.tar`

### file list

```diff
@@ -1,1236 +1,1241 @@
--rw-r--r--   0        0        0    11348 2023-04-03 11:32:18.314776 windmill_api-1.85.0/LICENSE
--rw-r--r--   0        0        0     2952 2023-04-03 11:32:18.322777 windmill_api-1.85.0/README.md
--rw-r--r--   0        0        0      717 2023-04-03 11:32:18.318776 windmill_api-1.85.0/pyproject.toml
--rw-r--r--   0        0        0      100 2023-04-03 11:31:41.552699 windmill_api-1.85.0/windmill_api/__init__.py
--rw-r--r--   0        0        0       47 2023-04-03 11:31:42.088730 windmill_api-1.85.0/windmill_api/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.204736 windmill_api-1.85.0/windmill_api/api/app/__init__.py
--rw-r--r--   0        0        0     1999 2023-04-03 11:31:53.845396 windmill_api-1.85.0/windmill_api/api/app/create_app.py
--rw-r--r--   0        0        0     1769 2023-04-03 11:31:53.849396 windmill_api-1.85.0/windmill_api/api/app/delete_app.py
--rw-r--r--   0        0        0     2214 2023-04-03 11:31:53.889398 windmill_api-1.85.0/windmill_api/api/app/execute_component.py
--rw-r--r--   0        0        0     2782 2023-04-03 11:31:53.901399 windmill_api-1.85.0/windmill_api/api/app/exists_app.py
--rw-r--r--   0        0        0     3020 2023-04-03 11:31:53.957402 windmill_api-1.85.0/windmill_api/api/app/get_app_by_path.py
--rw-r--r--   0        0        0     3031 2023-04-03 11:31:53.945402 windmill_api-1.85.0/windmill_api/api/app/get_app_by_version.py
--rw-r--r--   0        0        0     2649 2023-04-03 11:31:54.005405 windmill_api-1.85.0/windmill_api/api/app/get_hub_app_by_id.py
--rw-r--r--   0        0        0     3168 2023-04-03 11:31:54.005405 windmill_api-1.85.0/windmill_api/api/app/get_public_app_by_secret.py
--rw-r--r--   0        0        0     1797 2023-04-03 11:31:54.049407 windmill_api-1.85.0/windmill_api/api/app/get_public_secret_of_app.py
--rw-r--r--   0        0        0     7289 2023-04-03 11:31:54.109411 windmill_api-1.85.0/windmill_api/api/app/list_apps.py
--rw-r--r--   0        0        0     2405 2023-04-03 11:31:54.089410 windmill_api-1.85.0/windmill_api/api/app/list_hub_apps.py
--rw-r--r--   0        0        0     2140 2023-04-03 11:31:54.129412 windmill_api-1.85.0/windmill_api/api/app/update_app.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.128732 windmill_api-1.85.0/windmill_api/api/audit/__init__.py
--rw-r--r--   0        0        0     3065 2023-04-03 11:31:54.157414 windmill_api-1.85.0/windmill_api/api/audit/get_audit_log.py
--rw-r--r--   0        0        0     8723 2023-04-03 11:31:54.257419 windmill_api-1.85.0/windmill_api/api/audit/list_audit_logs.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.260740 windmill_api-1.85.0/windmill_api/api/capture/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-03 11:31:54.189415 windmill_api-1.85.0/windmill_api/api/capture/create_capture.py
--rw-r--r--   0        0        0     1790 2023-04-03 11:31:54.217417 windmill_api-1.85.0/windmill_api/api/capture/get_capture.py
--rw-r--r--   0        0        0     1799 2023-04-03 11:31:54.249419 windmill_api-1.85.0/windmill_api/api/capture/update_capture.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.264740 windmill_api-1.85.0/windmill_api/api/favorite/__init__.py
--rw-r--r--   0        0        0     1964 2023-04-03 11:31:54.289421 windmill_api-1.85.0/windmill_api/api/favorite/star.py
--rw-r--r--   0        0        0     1984 2023-04-03 11:31:54.289421 windmill_api-1.85.0/windmill_api/api/favorite/unstar.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.196736 windmill_api-1.85.0/windmill_api/api/flow/__init__.py
--rw-r--r--   0        0        0     1789 2023-04-03 11:31:54.321423 windmill_api-1.85.0/windmill_api/api/flow/archive_flow_by_path.py
--rw-r--r--   0        0        0     2009 2023-04-03 11:31:54.325423 windmill_api-1.85.0/windmill_api/api/flow/create_flow.py
--rw-r--r--   0        0        0     1788 2023-04-03 11:31:54.353425 windmill_api-1.85.0/windmill_api/api/flow/delete_flow_by_path.py
--rw-r--r--   0        0        0     2755 2023-04-03 11:31:54.369425 windmill_api-1.85.0/windmill_api/api/flow/exists_flow_by_path.py
--rw-r--r--   0        0        0     3036 2023-04-03 11:31:54.421429 windmill_api-1.85.0/windmill_api/api/flow/get_flow_by_path.py
--rw-r--r--   0        0        0     2667 2023-04-03 11:31:54.437429 windmill_api-1.85.0/windmill_api/api/flow/get_hub_flow_by_id.py
--rw-r--r--   0        0        0     1668 2023-04-03 11:31:54.453430 windmill_api-1.85.0/windmill_api/api/flow/list_flow_paths.py
--rw-r--r--   0        0        0     7969 2023-04-03 11:31:54.557436 windmill_api-1.85.0/windmill_api/api/flow/list_flows.py
--rw-r--r--   0        0        0     2423 2023-04-03 11:31:54.489432 windmill_api-1.85.0/windmill_api/api/flow/list_hub_flows.py
--rw-r--r--   0        0        0     2150 2023-04-03 11:31:54.525434 windmill_api-1.85.0/windmill_api/api/flow/update_flow.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.252739 windmill_api-1.85.0/windmill_api/api/folder/__init__.py
--rw-r--r--   0        0        0     2214 2023-04-03 11:31:54.561436 windmill_api-1.85.0/windmill_api/api/folder/add_owner_to_folder.py
--rw-r--r--   0        0        0     2029 2023-04-03 11:31:54.589438 windmill_api-1.85.0/windmill_api/api/folder/create_folder.py
--rw-r--r--   0        0        0     1778 2023-04-03 11:31:54.597438 windmill_api-1.85.0/windmill_api/api/folder/delete_folder.py
--rw-r--r--   0        0        0     2960 2023-04-03 11:31:54.637441 windmill_api-1.85.0/windmill_api/api/folder/get_folder.py
--rw-r--r--   0        0        0     3055 2023-04-03 11:31:54.645441 windmill_api-1.85.0/windmill_api/api/folder/get_folder_usage.py
--rw-r--r--   0        0        0     3405 2023-04-03 11:31:54.693444 windmill_api-1.85.0/windmill_api/api/folder/list_folder_names.py
--rw-r--r--   0        0        0     4251 2023-04-03 11:31:54.713445 windmill_api-1.85.0/windmill_api/api/folder/list_folders.py
--rw-r--r--   0        0        0     2244 2023-04-03 11:31:54.725446 windmill_api-1.85.0/windmill_api/api/folder/remove_owner_to_folder.py
--rw-r--r--   0        0        0     2170 2023-04-03 11:31:54.749447 windmill_api-1.85.0/windmill_api/api/folder/update_folder.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.260740 windmill_api-1.85.0/windmill_api/api/granular_acl/__init__.py
--rw-r--r--   0        0        0     2480 2023-04-03 11:31:54.765448 windmill_api-1.85.0/windmill_api/api/granular_acl/add_granular_acls.py
--rw-r--r--   0        0        0     3526 2023-04-03 11:31:54.825451 windmill_api-1.85.0/windmill_api/api/granular_acl/get_granular_acls.py
--rw-r--r--   0        0        0     2545 2023-04-03 11:31:54.801450 windmill_api-1.85.0/windmill_api/api/granular_acl/remove_granular_acls.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.244739 windmill_api-1.85.0/windmill_api/api/group/__init__.py
--rw-r--r--   0        0        0     2194 2023-04-03 11:31:54.857453 windmill_api-1.85.0/windmill_api/api/group/add_user_to_group.py
--rw-r--r--   0        0        0     2019 2023-04-03 11:31:54.861453 windmill_api-1.85.0/windmill_api/api/group/create_group.py
--rw-r--r--   0        0        0     1775 2023-04-03 11:31:54.885455 windmill_api-1.85.0/windmill_api/api/group/delete_group.py
--rw-r--r--   0        0        0     2942 2023-04-03 11:31:54.905456 windmill_api-1.85.0/windmill_api/api/group/get_group.py
--rw-r--r--   0        0        0     3400 2023-04-03 11:31:54.937458 windmill_api-1.85.0/windmill_api/api/group/list_group_names.py
--rw-r--r--   0        0        0     4233 2023-04-03 11:31:54.969459 windmill_api-1.85.0/windmill_api/api/group/list_groups.py
--rw-r--r--   0        0        0     2224 2023-04-03 11:31:54.973460 windmill_api-1.85.0/windmill_api/api/group/remove_user_to_group.py
--rw-r--r--   0        0        0     2160 2023-04-03 11:31:55.005462 windmill_api-1.85.0/windmill_api/api/group/update_group.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.212737 windmill_api-1.85.0/windmill_api/api/job/__init__.py
--rw-r--r--   0        0        0     2181 2023-04-03 11:31:55.013462 windmill_api-1.85.0/windmill_api/api/job/cancel_queued_job.py
--rw-r--r--   0        0        0     2687 2023-04-03 11:31:55.049464 windmill_api-1.85.0/windmill_api/api/job/cancel_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-04-03 11:31:55.065465 windmill_api-1.85.0/windmill_api/api/job/cancel_suspended_job_post.py
--rw-r--r--   0        0        0     2535 2023-04-03 11:31:55.093467 windmill_api-1.85.0/windmill_api/api/job/create_job_signature.py
--rw-r--r--   0        0        0     3217 2023-04-03 11:31:55.125468 windmill_api-1.85.0/windmill_api/api/job/delete_completed_job.py
--rw-r--r--   0        0        0     2235 2023-04-03 11:31:55.125468 windmill_api-1.85.0/windmill_api/api/job/force_cancel_queued_job.py
--rw-r--r--   0        0        0     3034 2023-04-03 11:31:55.173471 windmill_api-1.85.0/windmill_api/api/job/get_completed_job.py
--rw-r--r--   0        0        0     1784 2023-04-03 11:31:55.157470 windmill_api-1.85.0/windmill_api/api/job/get_completed_job_result.py
--rw-r--r--   0        0        0     2868 2023-04-03 11:31:55.225474 windmill_api-1.85.0/windmill_api/api/job/get_job.py
--rw-r--r--   0        0        0     4305 2023-04-03 11:31:55.257476 windmill_api-1.85.0/windmill_api/api/job/get_job_updates.py
--rw-r--r--   0        0        0     4306 2023-04-03 11:31:55.285477 windmill_api-1.85.0/windmill_api/api/job/get_resume_urls.py
--rw-r--r--   0        0        0     4601 2023-04-03 11:31:55.325480 windmill_api-1.85.0/windmill_api/api/job/get_suspended_job_flow.py
--rw-r--r--   0        0        0    12602 2023-04-03 11:31:55.445486 windmill_api-1.85.0/windmill_api/api/job/list_completed_jobs.py
--rw-r--r--   0        0        0    11829 2023-04-03 11:31:55.481488 windmill_api-1.85.0/windmill_api/api/job/list_jobs.py
--rw-r--r--   0        0        0    12367 2023-04-03 11:31:55.605495 windmill_api-1.85.0/windmill_api/api/job/list_queue.py
--rw-r--r--   0        0        0     2067 2023-04-03 11:31:55.513490 windmill_api-1.85.0/windmill_api/api/job/result_by_id.py
--rw-r--r--   0        0        0     2313 2023-04-03 11:31:55.553492 windmill_api-1.85.0/windmill_api/api/job/resume_suspended_flow_as_owner.py
--rw-r--r--   0        0        0     2687 2023-04-03 11:31:55.597495 windmill_api-1.85.0/windmill_api/api/job/resume_suspended_job_get.py
--rw-r--r--   0        0        0     3154 2023-04-03 11:31:55.649498 windmill_api-1.85.0/windmill_api/api/job/resume_suspended_job_post.py
--rw-r--r--   0        0        0     4566 2023-04-03 11:31:55.705501 windmill_api-1.85.0/windmill_api/api/job/run_flow_by_path.py
--rw-r--r--   0        0        0     3037 2023-04-03 11:31:55.725502 windmill_api-1.85.0/windmill_api/api/job/run_flow_preview.py
--rw-r--r--   0        0        0     4594 2023-04-03 11:31:55.769504 windmill_api-1.85.0/windmill_api/api/job/run_script_by_hash.py
--rw-r--r--   0        0        0     4200 2023-04-03 11:31:55.785505 windmill_api-1.85.0/windmill_api/api/job/run_script_by_path.py
--rw-r--r--   0        0        0     3050 2023-04-03 11:31:55.813507 windmill_api-1.85.0/windmill_api/api/job/run_script_preview.py
--rw-r--r--   0        0        0     4280 2023-04-03 11:31:55.849509 windmill_api-1.85.0/windmill_api/api/job/run_wait_result_flow_by_path.py
--rw-r--r--   0        0        0     4586 2023-04-03 11:31:55.877510 windmill_api-1.85.0/windmill_api/api/job/run_wait_result_script_by_path.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.164734 windmill_api-1.85.0/windmill_api/api/oauth/__init__.py
--rw-r--r--   0        0        0     3506 2023-04-03 11:31:55.897512 windmill_api-1.85.0/windmill_api/api/oauth/connect_callback.py
--rw-r--r--   0        0        0     2118 2023-04-03 11:31:55.905512 windmill_api-1.85.0/windmill_api/api/oauth/connect_slack_callback.py
--rw-r--r--   0        0        0     2056 2023-04-03 11:31:55.933513 windmill_api-1.85.0/windmill_api/api/oauth/create_account.py
--rw-r--r--   0        0        0     1764 2023-04-03 11:31:55.937514 windmill_api-1.85.0/windmill_api/api/oauth/disconnect_account.py
--rw-r--r--   0        0        0     1649 2023-04-03 11:31:55.961515 windmill_api-1.85.0/windmill_api/api/oauth/disconnect_slack.py
--rw-r--r--   0        0        0     1426 2023-04-03 11:31:55.965515 windmill_api-1.85.0/windmill_api/api/oauth/list_o_auth_connects.py
--rw-r--r--   0        0        0     2162 2023-04-03 11:31:56.005518 windmill_api-1.85.0/windmill_api/api/oauth/list_o_auth_logins.py
--rw-r--r--   0        0        0     2151 2023-04-03 11:31:56.001517 windmill_api-1.85.0/windmill_api/api/oauth/refresh_token.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.172735 windmill_api-1.85.0/windmill_api/api/resource/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-03 11:31:56.037519 windmill_api-1.85.0/windmill_api/api/resource/create_resource.py
--rw-r--r--   0        0        0     2093 2023-04-03 11:31:56.041519 windmill_api-1.85.0/windmill_api/api/resource/create_resource_type.py
--rw-r--r--   0        0        0     1784 2023-04-03 11:31:56.069521 windmill_api-1.85.0/windmill_api/api/resource/delete_resource.py
--rw-r--r--   0        0        0     1799 2023-04-03 11:31:56.093522 windmill_api-1.85.0/windmill_api/api/resource/delete_resource_type.py
--rw-r--r--   0        0        0     2763 2023-04-03 11:31:56.137525 windmill_api-1.85.0/windmill_api/api/resource/exists_resource.py
--rw-r--r--   0        0        0     2788 2023-04-03 11:31:56.141525 windmill_api-1.85.0/windmill_api/api/resource/exists_resource_type.py
--rw-r--r--   0        0        0     2996 2023-04-03 11:31:56.181527 windmill_api-1.85.0/windmill_api/api/resource/get_resource.py
--rw-r--r--   0        0        0     3074 2023-04-03 11:31:56.189528 windmill_api-1.85.0/windmill_api/api/resource/get_resource_type.py
--rw-r--r--   0        0        0     1790 2023-04-03 11:31:56.213529 windmill_api-1.85.0/windmill_api/api/resource/get_resource_value.py
--rw-r--r--   0        0        0     5732 2023-04-03 11:31:56.273532 windmill_api-1.85.0/windmill_api/api/resource/list_resource.py
--rw-r--r--   0        0        0     3149 2023-04-03 11:31:56.257532 windmill_api-1.85.0/windmill_api/api/resource/list_resource_type.py
--rw-r--r--   0        0        0     2600 2023-04-03 11:31:56.301534 windmill_api-1.85.0/windmill_api/api/resource/list_resource_type_names.py
--rw-r--r--   0        0        0     2190 2023-04-03 11:31:56.309535 windmill_api-1.85.0/windmill_api/api/resource/update_resource.py
--rw-r--r--   0        0        0     2234 2023-04-03 11:31:56.333536 windmill_api-1.85.0/windmill_api/api/resource/update_resource_type.py
--rw-r--r--   0        0        0     2244 2023-04-03 11:31:56.345537 windmill_api-1.85.0/windmill_api/api/resource/update_resource_value.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.240738 windmill_api-1.85.0/windmill_api/api/schedule/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-03 11:31:56.365538 windmill_api-1.85.0/windmill_api/api/schedule/create_schedule.py
--rw-r--r--   0        0        0     1784 2023-04-03 11:31:56.377538 windmill_api-1.85.0/windmill_api/api/schedule/delete_schedule.py
--rw-r--r--   0        0        0     2763 2023-04-03 11:31:56.409540 windmill_api-1.85.0/windmill_api/api/schedule/exists_schedule.py
--rw-r--r--   0        0        0     2996 2023-04-03 11:31:56.425541 windmill_api-1.85.0/windmill_api/api/schedule/get_schedule.py
--rw-r--r--   0        0        0     4287 2023-04-03 11:31:56.493545 windmill_api-1.85.0/windmill_api/api/schedule/list_schedules.py
--rw-r--r--   0        0        0     3217 2023-04-03 11:31:56.493545 windmill_api-1.85.0/windmill_api/api/schedule/preview_schedule.py
--rw-r--r--   0        0        0     2233 2023-04-03 11:31:56.533547 windmill_api-1.85.0/windmill_api/api/schedule/set_schedule_enabled.py
--rw-r--r--   0        0        0     2190 2023-04-03 11:31:56.529547 windmill_api-1.85.0/windmill_api/api/schedule/update_schedule.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.180735 windmill_api-1.85.0/windmill_api/api/script/__init__.py
--rw-r--r--   0        0        0     3165 2023-04-03 11:31:56.573549 windmill_api-1.85.0/windmill_api/api/script/archive_script_by_hash.py
--rw-r--r--   0        0        0     1797 2023-04-03 11:31:56.565549 windmill_api-1.85.0/windmill_api/api/script/archive_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-04-03 11:31:56.613551 windmill_api-1.85.0/windmill_api/api/script/bash_to_jsonschema.py
--rw-r--r--   0        0        0     2029 2023-04-03 11:31:56.605551 windmill_api-1.85.0/windmill_api/api/script/create_script.py
--rw-r--r--   0        0        0     3327 2023-04-03 11:31:56.653554 windmill_api-1.85.0/windmill_api/api/script/delete_script_by_hash.py
--rw-r--r--   0        0        0     2873 2023-04-03 11:31:56.657554 windmill_api-1.85.0/windmill_api/api/script/delete_script_by_path.py
--rw-r--r--   0        0        0     3003 2023-04-03 11:31:56.697556 windmill_api-1.85.0/windmill_api/api/script/deno_to_jsonschema.py
--rw-r--r--   0        0        0     2767 2023-04-03 11:31:56.705557 windmill_api-1.85.0/windmill_api/api/script/exists_script_by_path.py
--rw-r--r--   0        0        0     2802 2023-04-03 11:31:56.737558 windmill_api-1.85.0/windmill_api/api/script/get_hub_script_by_path.py
--rw-r--r--   0        0        0     1607 2023-04-03 11:31:56.733558 windmill_api-1.85.0/windmill_api/api/script/get_hub_script_content_by_path.py
--rw-r--r--   0        0        0     3092 2023-04-03 11:31:56.793562 windmill_api-1.85.0/windmill_api/api/script/get_script_by_hash.py
--rw-r--r--   0        0        0     3074 2023-04-03 11:31:56.781561 windmill_api-1.85.0/windmill_api/api/script/get_script_by_path.py
--rw-r--r--   0        0        0     3276 2023-04-03 11:31:56.825564 windmill_api-1.85.0/windmill_api/api/script/get_script_deployment_status.py
--rw-r--r--   0        0        0     2967 2023-04-03 11:31:56.837564 windmill_api-1.85.0/windmill_api/api/script/go_to_jsonschema.py
--rw-r--r--   0        0        0     2459 2023-04-03 11:31:56.885567 windmill_api-1.85.0/windmill_api/api/script/list_hub_scripts.py
--rw-r--r--   0        0        0     1676 2023-04-03 11:31:56.885567 windmill_api-1.85.0/windmill_api/api/script/list_script_paths.py
--rw-r--r--   0        0        0    11165 2023-04-03 11:31:57.033575 windmill_api-1.85.0/windmill_api/api/script/list_scripts.py
--rw-r--r--   0        0        0     3039 2023-04-03 11:31:56.933570 windmill_api-1.85.0/windmill_api/api/script/python_to_jsonschema.py
--rw-r--r--   0        0        0     1784 2023-04-03 11:31:56.965571 windmill_api-1.85.0/windmill_api/api/script/raw_script_by_hash.py
--rw-r--r--   0        0        0     1784 2023-04-03 11:31:56.997573 windmill_api-1.85.0/windmill_api/api/script/raw_script_by_path.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.100731 windmill_api-1.85.0/windmill_api/api/settings/__init__.py
--rw-r--r--   0        0        0     1414 2023-04-03 11:31:57.025575 windmill_api-1.85.0/windmill_api/api/settings/backend_version.py
--rw-r--r--   0        0        0     1423 2023-04-03 11:31:57.057577 windmill_api-1.85.0/windmill_api/api/settings/get_open_api_yaml.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.132732 windmill_api-1.85.0/windmill_api/api/user/__init__.py
--rw-r--r--   0        0        0     1857 2023-04-03 11:31:57.061577 windmill_api-1.85.0/windmill_api/api/user/accept_invite.py
--rw-r--r--   0        0        0     1822 2023-04-03 11:31:57.089578 windmill_api-1.85.0/windmill_api/api/user/create_token.py
--rw-r--r--   0        0        0     2058 2023-04-03 11:31:57.093578 windmill_api-1.85.0/windmill_api/api/user/create_user.py
--rw-r--r--   0        0        0     1863 2023-04-03 11:31:57.121580 windmill_api-1.85.0/windmill_api/api/user/create_user_globally.py
--rw-r--r--   0        0        0     1867 2023-04-03 11:31:57.125580 windmill_api-1.85.0/windmill_api/api/user/decline_invite.py
--rw-r--r--   0        0        0     1674 2023-04-03 11:31:57.161582 windmill_api-1.85.0/windmill_api/api/user/delete_token.py
--rw-r--r--   0        0        0     1872 2023-04-03 11:31:57.157582 windmill_api-1.85.0/windmill_api/api/user/delete_user.py
--rw-r--r--   0        0        0     1454 2023-04-03 11:31:57.181583 windmill_api-1.85.0/windmill_api/api/user/get_current_email.py
--rw-r--r--   0        0        0     1474 2023-04-03 11:31:57.189584 windmill_api-1.85.0/windmill_api/api/user/get_usage.py
--rw-r--r--   0        0        0     1639 2023-04-03 11:31:57.213585 windmill_api-1.85.0/windmill_api/api/user/global_user_delete.py
--rw-r--r--   0        0        0     2060 2023-04-03 11:31:57.221586 windmill_api-1.85.0/windmill_api/api/user/global_user_update.py
--rw-r--r--   0        0        0     2468 2023-04-03 11:31:57.273589 windmill_api-1.85.0/windmill_api/api/user/global_whoami.py
--rw-r--r--   0        0        0     2745 2023-04-03 11:31:57.289590 windmill_api-1.85.0/windmill_api/api/user/is_owner_of_path.py
--rw-r--r--   0        0        0     1646 2023-04-03 11:31:57.305590 windmill_api-1.85.0/windmill_api/api/user/leave_workspace.py
--rw-r--r--   0        0        0     2633 2023-04-03 11:31:57.333592 windmill_api-1.85.0/windmill_api/api/user/list_tokens.py
--rw-r--r--   0        0        0     2552 2023-04-03 11:31:57.349593 windmill_api-1.85.0/windmill_api/api/user/list_usernames.py
--rw-r--r--   0        0        0     3012 2023-04-03 11:31:57.381595 windmill_api-1.85.0/windmill_api/api/user/list_users.py
--rw-r--r--   0        0        0     4222 2023-04-03 11:31:57.409596 windmill_api-1.85.0/windmill_api/api/user/list_users_as_super_admin.py
--rw-r--r--   0        0        0     2829 2023-04-03 11:31:57.425597 windmill_api-1.85.0/windmill_api/api/user/list_workspace_invites.py
--rw-r--r--   0        0        0     1784 2023-04-03 11:31:57.441598 windmill_api-1.85.0/windmill_api/api/user/login.py
--rw-r--r--   0        0        0     2116 2023-04-03 11:31:57.461599 windmill_api-1.85.0/windmill_api/api/user/login_with_oauth.py
--rw-r--r--   0        0        0     1393 2023-04-03 11:31:57.469600 windmill_api-1.85.0/windmill_api/api/user/logout.py
--rw-r--r--   0        0        0     1820 2023-04-03 11:31:57.493601 windmill_api-1.85.0/windmill_api/api/user/set_password.py
--rw-r--r--   0        0        0     2250 2023-04-03 11:31:57.501601 windmill_api-1.85.0/windmill_api/api/user/update_user.py
--rw-r--r--   0        0        0     2652 2023-04-03 11:31:57.537603 windmill_api-1.85.0/windmill_api/api/user/whoami.py
--rw-r--r--   0        0        0     2967 2023-04-03 11:31:57.549604 windmill_api-1.85.0/windmill_api/api/user/whois.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.160734 windmill_api-1.85.0/windmill_api/api/variable/__init__.py
--rw-r--r--   0        0        0     2634 2023-04-03 11:31:57.585606 windmill_api-1.85.0/windmill_api/api/variable/create_variable.py
--rw-r--r--   0        0        0     1784 2023-04-03 11:31:57.581606 windmill_api-1.85.0/windmill_api/api/variable/delete_variable.py
--rw-r--r--   0        0        0     2795 2023-04-03 11:31:57.625608 windmill_api-1.85.0/windmill_api/api/variable/exists_variable.py
--rw-r--r--   0        0        0     3840 2023-04-03 11:31:57.645609 windmill_api-1.85.0/windmill_api/api/variable/get_variable.py
--rw-r--r--   0        0        0     3270 2023-04-03 11:31:57.689612 windmill_api-1.85.0/windmill_api/api/variable/list_contextual_variables.py
--rw-r--r--   0        0        0     3071 2023-04-03 11:31:57.713613 windmill_api-1.85.0/windmill_api/api/variable/list_variable.py
--rw-r--r--   0        0        0     2775 2023-04-03 11:31:57.733614 windmill_api-1.85.0/windmill_api/api/variable/update_variable.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.260740 windmill_api-1.85.0/windmill_api/api/worker/__init__.py
--rw-r--r--   0        0        0     3896 2023-04-03 11:31:57.785617 windmill_api-1.85.0/windmill_api/api/worker/list_workers.py
--rw-r--r--   0        0        0        0 2023-04-03 11:31:42.148733 windmill_api-1.85.0/windmill_api/api/workspace/__init__.py
--rw-r--r--   0        0        0     2015 2023-04-03 11:31:57.769616 windmill_api-1.85.0/windmill_api/api/workspace/add_user.py
--rw-r--r--   0        0        0     1647 2023-04-03 11:31:57.797618 windmill_api-1.85.0/windmill_api/api/workspace/archive_workspace.py
--rw-r--r--   0        0        0     1856 2023-04-03 11:31:57.817619 windmill_api-1.85.0/windmill_api/api/workspace/create_workspace.py
--rw-r--r--   0        0        0     2049 2023-04-03 11:31:57.833620 windmill_api-1.85.0/windmill_api/api/workspace/delete_invite.py
--rw-r--r--   0        0        0     1688 2023-04-03 11:31:57.853621 windmill_api-1.85.0/windmill_api/api/workspace/delete_workspace.py
--rw-r--r--   0        0        0     2063 2023-04-03 11:31:57.869622 windmill_api-1.85.0/windmill_api/api/workspace/edit_auto_invite.py
--rw-r--r--   0        0        0     2083 2023-04-03 11:31:57.889623 windmill_api-1.85.0/windmill_api/api/workspace/edit_slack_command.py
--rw-r--r--   0        0        0     2029 2023-04-03 11:31:57.901624 windmill_api-1.85.0/windmill_api/api/workspace/edit_webhook.py
--rw-r--r--   0        0        0     1856 2023-04-03 11:31:57.921625 windmill_api-1.85.0/windmill_api/api/workspace/exists_username.py
--rw-r--r--   0        0        0     1856 2023-04-03 11:31:57.933625 windmill_api-1.85.0/windmill_api/api/workspace/exists_workspace.py
--rw-r--r--   0        0        0     2809 2023-04-03 11:31:57.969627 windmill_api-1.85.0/windmill_api/api/workspace/get_premium_info.py
--rw-r--r--   0        0        0     2753 2023-04-03 11:31:57.985628 windmill_api-1.85.0/windmill_api/api/workspace/get_settings.py
--rw-r--r--   0        0        0     2045 2023-04-03 11:31:58.005629 windmill_api-1.85.0/windmill_api/api/workspace/invite_user.py
--rw-r--r--   0        0        0     2176 2023-04-03 11:31:58.021630 windmill_api-1.85.0/windmill_api/api/workspace/is_domain_allowed.py
--rw-r--r--   0        0        0     3255 2023-04-03 11:31:58.061632 windmill_api-1.85.0/windmill_api/api/workspace/list_pending_invites.py
--rw-r--r--   0        0        0     2583 2023-04-03 11:31:58.081634 windmill_api-1.85.0/windmill_api/api/workspace/list_user_workspaces.py
--rw-r--r--   0        0        0     2775 2023-04-03 11:31:58.137637 windmill_api-1.85.0/windmill_api/api/workspace/list_workspaces.py
--rw-r--r--   0        0        0     4311 2023-04-03 11:31:58.145637 windmill_api-1.85.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py
--rw-r--r--   0        0        0     1651 2023-04-03 11:31:58.169639 windmill_api-1.85.0/windmill_api/api/workspace/unarchive_workspace.py
--rw-r--r--   0        0        0     1821 2023-04-03 11:31:58.177639 windmill_api-1.85.0/windmill_api/client.py
--rw-r--r--   0        0        0        1 2023-04-03 11:32:18.310776 windmill_api-1.85.0/windmill_api/models/__init__.py
--rw-r--r--   0        0        0     1667 2023-04-03 11:31:58.209641 windmill_api-1.85.0/windmill_api/models/accept_invite_json_body.py
--rw-r--r--   0        0        0     1710 2023-04-03 11:31:58.241643 windmill_api-1.85.0/windmill_api/models/add_granular_acls_json_body.py
--rw-r--r--   0        0        0      301 2023-04-03 11:31:52.461317 windmill_api-1.85.0/windmill_api/models/add_granular_acls_kind.py
--rw-r--r--   0        0        0     1529 2023-04-03 11:31:58.273645 windmill_api-1.85.0/windmill_api/models/add_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1940 2023-04-03 11:31:58.305646 windmill_api-1.85.0/windmill_api/models/add_user_json_body.py
--rw-r--r--   0        0        0     1552 2023-04-03 11:31:58.337648 windmill_api-1.85.0/windmill_api/models/add_user_to_group_json_body.py
--rw-r--r--   0        0        0     3940 2023-04-03 11:31:58.377650 windmill_api-1.85.0/windmill_api/models/app_with_last_version.py
--rw-r--r--   0        0        0      214 2023-04-03 11:31:51.969289 windmill_api-1.85.0/windmill_api/models/app_with_last_version_execution_mode.py
--rw-r--r--   0        0        0     1248 2023-04-03 11:31:58.361649 windmill_api-1.85.0/windmill_api/models/app_with_last_version_extra_perms.py
--rw-r--r--   0        0        0     3716 2023-04-03 11:31:58.417652 windmill_api-1.85.0/windmill_api/models/app_with_last_version_policy.py
--rw-r--r--   0        0        0      220 2023-04-03 11:31:52.161300 windmill_api-1.85.0/windmill_api/models/app_with_last_version_policy_execution_mode.py
--rw-r--r--   0        0        0     1946 2023-04-03 11:31:58.409652 windmill_api-1.85.0/windmill_api/models/app_with_last_version_policy_triggerables.py
--rw-r--r--   0        0        0     1381 2023-04-03 11:31:58.437654 windmill_api-1.85.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     6879 2023-04-03 11:31:58.537659 windmill_api-1.85.0/windmill_api/models/archive_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1314 2023-04-03 11:31:58.461655 windmill_api-1.85.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      259 2023-04-03 11:31:51.993291 windmill_api-1.85.0/windmill_api/models/archive_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      217 2023-04-03 11:31:52.265306 windmill_api-1.85.0/windmill_api/models/archive_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1288 2023-04-03 11:31:58.493657 windmill_api-1.85.0/windmill_api/models/archive_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     3452 2023-04-03 11:31:58.585662 windmill_api-1.85.0/windmill_api/models/audit_log.py
--rw-r--r--   0        0        0      217 2023-04-03 11:31:52.409314 windmill_api-1.85.0/windmill_api/models/audit_log_action_kind.py
--rw-r--r--   0        0        0      620 2023-04-03 11:31:52.565323 windmill_api-1.85.0/windmill_api/models/audit_log_operation.py
--rw-r--r--   0        0        0     1186 2023-04-03 11:31:58.565661 windmill_api-1.85.0/windmill_api/models/audit_log_parameters.py
--rw-r--r--   0        0        0     2933 2023-04-03 11:31:58.613664 windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-04-03 11:31:58.653666 windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-04-03 11:31:51.993291 windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-04-03 11:31:58.645665 windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-04-03 11:31:58.677667 windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-04-03 11:31:58.685668 windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-04-03 11:31:58.725670 windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-04-03 11:31:52.289308 windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-04-03 11:31:58.713669 windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-04-03 11:31:58.765672 windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-04-03 11:31:52.293308 windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-04-03 11:31:58.757671 windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-04-03 11:31:52.225304 windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2377 2023-04-03 11:31:58.805674 windmill_api-1.85.0/windmill_api/models/branch_all.py
--rw-r--r--   0        0        0     2543 2023-04-03 11:31:58.805674 windmill_api-1.85.0/windmill_api/models/branch_all_branches_item.py
--rw-r--r--   0        0        0     6620 2023-04-03 11:31:58.889679 windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-04-03 11:31:58.849677 windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-04-03 11:31:58.877678 windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-03 11:31:58.913680 windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-03 11:31:58.941682 windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-03 11:31:52.133299 windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-03 11:31:58.945682 windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-03 11:31:53.045350 windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-03 11:31:58.973684 windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-03 11:31:59.001685 windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      146 2023-04-03 11:31:52.601325 windmill_api-1.85.0/windmill_api/models/branch_all_type.py
--rw-r--r--   0        0        0     2670 2023-04-03 11:31:59.017686 windmill_api-1.85.0/windmill_api/models/branch_one.py
--rw-r--r--   0        0        0     2372 2023-04-03 11:31:59.041687 windmill_api-1.85.0/windmill_api/models/branch_one_branches_item.py
--rw-r--r--   0        0        0     6620 2023-04-03 11:31:59.105691 windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item.py
--rw-r--r--   0        0        0     3129 2023-04-03 11:31:59.089690 windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     1929 2023-04-03 11:31:59.125692 windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-03 11:31:59.145693 windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-03 11:31:59.161694 windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-03 11:31:52.217304 windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-03 11:31:59.177695 windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-03 11:31:52.889342 windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-03 11:31:59.197696 windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-03 11:31:59.209697 windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6125 2023-04-03 11:31:59.297702 windmill_api-1.85.0/windmill_api/models/branch_one_default_item.py
--rw-r--r--   0        0        0     2906 2023-04-03 11:31:59.249699 windmill_api-1.85.0/windmill_api/models/branch_one_default_item_retry.py
--rw-r--r--   0        0        0     1863 2023-04-03 11:31:59.281701 windmill_api-1.85.0/windmill_api/models/branch_one_default_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-04-03 11:31:59.317703 windmill_api-1.85.0/windmill_api/models/branch_one_default_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-04-03 11:31:59.329703 windmill_api-1.85.0/windmill_api/models/branch_one_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-04-03 11:31:52.061295 windmill_api-1.85.0/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-04-03 11:31:59.365706 windmill_api-1.85.0/windmill_api/models/branch_one_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-04-03 11:31:52.085296 windmill_api-1.85.0/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-04-03 11:31:59.361705 windmill_api-1.85.0/windmill_api/models/branch_one_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-04-03 11:31:59.421709 windmill_api-1.85.0/windmill_api/models/branch_one_default_item_suspend.py
--rw-r--r--   0        0        0      146 2023-04-03 11:31:52.601325 windmill_api-1.85.0/windmill_api/models/branch_one_type.py
--rw-r--r--   0        0        0     1532 2023-04-03 11:31:59.397707 windmill_api-1.85.0/windmill_api/models/cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     1255 2023-04-03 11:31:59.421709 windmill_api-1.85.0/windmill_api/models/cancel_suspended_job_post_json_body.py
--rw-r--r--   0        0        0    10376 2023-04-03 11:31:59.573717 windmill_api-1.85.0/windmill_api/models/completed_job.py
--rw-r--r--   0        0        0     1176 2023-04-03 11:31:59.445710 windmill_api-1.85.0/windmill_api/models/completed_job_args.py
--rw-r--r--   0        0        0     3265 2023-04-03 11:31:59.497713 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status.py
--rw-r--r--   0        0        0     6800 2023-04-03 11:31:59.597719 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1789 2023-04-03 11:31:59.605719 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2136 2023-04-03 11:31:59.633720 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      202 2023-04-03 11:31:52.949345 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1694 2023-04-03 11:31:59.637721 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2230 2023-04-03 11:31:59.673723 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      360 2023-04-03 11:31:51.997291 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6402 2023-04-03 11:31:59.733726 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1779 2023-04-03 11:31:59.705725 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2116 2023-04-03 11:31:59.737726 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      200 2023-04-03 11:31:53.157357 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1684 2023-04-03 11:31:59.765728 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2220 2023-04-03 11:31:59.801730 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      358 2023-04-03 11:31:53.069352 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2040 2023-04-03 11:31:59.801730 windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_retry.py
--rw-r--r--   0        0        0      310 2023-04-03 11:31:53.001348 windmill_api-1.85.0/windmill_api/models/completed_job_job_kind.py
--rw-r--r--   0        0        0      199 2023-04-03 11:31:52.753334 windmill_api-1.85.0/windmill_api/models/completed_job_language.py
--rw-r--r--   0        0        0     3127 2023-04-03 11:31:59.869734 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow.py
--rw-r--r--   0        0        0     6620 2023-04-03 11:31:59.885735 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3129 2023-04-03 11:31:59.913736 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1929 2023-04-03 11:31:59.917736 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2233 2023-04-03 11:31:59.953739 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2079 2023-04-03 11:31:59.949738 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-03 11:31:52.297308 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1946 2023-04-03 11:31:59.981740 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-03 11:31:52.201303 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1922 2023-04-03 11:31:59.989740 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1973 2023-04-03 11:32:00.013742 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6544 2023-04-03 11:32:00.085746 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3095 2023-04-03 11:32:00.061745 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1919 2023-04-03 11:32:00.093746 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2223 2023-04-03 11:32:00.121748 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2050 2023-04-03 11:32:00.125748 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      179 2023-04-03 11:31:52.229304 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1917 2023-04-03 11:32:00.157750 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      179 2023-04-03 11:31:52.105297 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1912 2023-04-03 11:32:00.189752 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1963 2023-04-03 11:32:00.193752 windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1572 2023-04-03 11:32:00.217753 windmill_api-1.85.0/windmill_api/models/connect_callback_json_body.py
--rw-r--r--   0        0        0     2533 2023-04-03 11:32:00.241755 windmill_api-1.85.0/windmill_api/models/connect_callback_response_200.py
--rw-r--r--   0        0        0     1600 2023-04-03 11:32:00.253755 windmill_api-1.85.0/windmill_api/models/connect_slack_callback_json_body.py
--rw-r--r--   0        0        0     1753 2023-04-03 11:32:00.305758 windmill_api-1.85.0/windmill_api/models/contextual_variable.py
--rw-r--r--   0        0        0     2147 2023-04-03 11:32:00.289757 windmill_api-1.85.0/windmill_api/models/create_account_json_body.py
--rw-r--r--   0        0        0     2035 2023-04-03 11:32:00.325759 windmill_api-1.85.0/windmill_api/models/create_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-04-03 11:32:00.361761 windmill_api-1.85.0/windmill_api/models/create_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-04-03 11:31:52.561323 windmill_api-1.85.0/windmill_api/models/create_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-04-03 11:32:00.357761 windmill_api-1.85.0/windmill_api/models/create_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-04-03 11:32:00.381762 windmill_api-1.85.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-04-03 11:32:00.409764 windmill_api-1.85.0/windmill_api/models/create_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-04-03 11:32:00.405764 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-04-03 11:32:00.453766 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-04-03 11:32:00.501769 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-04-03 11:32:00.517770 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-04-03 11:32:00.537771 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-04-03 11:32:00.557772 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-04-03 11:32:00.569773 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-04-03 11:31:52.549322 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-04-03 11:32:00.589774 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-04-03 11:31:52.249305 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-04-03 11:32:00.609775 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-04-03 11:32:00.645777 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-04-03 11:32:00.729782 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-04-03 11:32:00.693780 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-04-03 11:32:00.729782 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-04-03 11:32:00.765784 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-04-03 11:32:00.765784 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-04-03 11:31:52.413315 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-04-03 11:32:00.797786 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-04-03 11:31:52.441316 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-04-03 11:32:00.801786 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-04-03 11:32:00.829787 windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2126 2023-04-03 11:32:00.841788 windmill_api-1.85.0/windmill_api/models/create_folder_json_body.py
--rw-r--r--   0        0        0     1697 2023-04-03 11:32:00.861789 windmill_api-1.85.0/windmill_api/models/create_group_json_body.py
--rw-r--r--   0        0        0     2094 2023-04-03 11:32:00.881790 windmill_api-1.85.0/windmill_api/models/create_resource.py
--rw-r--r--   0        0        0     2140 2023-04-03 11:32:00.897791 windmill_api-1.85.0/windmill_api/models/create_resource_json_body.py
--rw-r--r--   0        0        0     2335 2023-04-03 11:32:00.921793 windmill_api-1.85.0/windmill_api/models/create_resource_type_json_body.py
--rw-r--r--   0        0        0     2843 2023-04-03 11:32:00.945794 windmill_api-1.85.0/windmill_api/models/create_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-04-03 11:32:00.945794 windmill_api-1.85.0/windmill_api/models/create_schedule_json_body_args.py
--rw-r--r--   0        0        0     4616 2023-04-03 11:32:01.029799 windmill_api-1.85.0/windmill_api/models/create_script_json_body.py
--rw-r--r--   0        0        0      249 2023-04-03 11:31:51.965289 windmill_api-1.85.0/windmill_api/models/create_script_json_body_kind.py
--rw-r--r--   0        0        0      207 2023-04-03 11:31:52.753334 windmill_api-1.85.0/windmill_api/models/create_script_json_body_language.py
--rw-r--r--   0        0        0     1232 2023-04-03 11:32:00.977796 windmill_api-1.85.0/windmill_api/models/create_script_json_body_schema.py
--rw-r--r--   0        0        0     2169 2023-04-03 11:32:01.017798 windmill_api-1.85.0/windmill_api/models/create_token_json_body.py
--rw-r--r--   0        0        0     2364 2023-04-03 11:32:01.061800 windmill_api-1.85.0/windmill_api/models/create_user_globally_json_body.py
--rw-r--r--   0        0        0     1771 2023-04-03 11:32:01.061800 windmill_api-1.85.0/windmill_api/models/create_user_json_body.py
--rw-r--r--   0        0        0     2493 2023-04-03 11:32:01.105803 windmill_api-1.85.0/windmill_api/models/create_variable.py
--rw-r--r--   0        0        0     2539 2023-04-03 11:32:01.133804 windmill_api-1.85.0/windmill_api/models/create_variable_json_body.py
--rw-r--r--   0        0        0     1678 2023-04-03 11:32:01.137805 windmill_api-1.85.0/windmill_api/models/create_workspace.py
--rw-r--r--   0        0        0     1724 2023-04-03 11:32:01.169807 windmill_api-1.85.0/windmill_api/models/create_workspace_json_body.py
--rw-r--r--   0        0        0     1490 2023-04-03 11:32:01.197808 windmill_api-1.85.0/windmill_api/models/decline_invite_json_body.py
--rw-r--r--   0        0        0    10978 2023-04-03 11:32:01.321815 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200.py
--rw-r--r--   0        0        0     1270 2023-04-03 11:32:01.221809 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3658 2023-04-03 11:32:01.273812 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7442 2023-04-03 11:32:01.369818 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1883 2023-04-03 11:32:01.353817 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2318 2023-04-03 11:32:01.389819 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      219 2023-04-03 11:31:52.833338 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1788 2023-04-03 11:32:01.401820 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2324 2023-04-03 11:32:01.433821 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      377 2023-04-03 11:31:52.925344 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7053 2023-04-03 11:32:01.497825 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1873 2023-04-03 11:32:01.465823 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2298 2023-04-03 11:32:01.501825 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      217 2023-04-03 11:31:51.941288 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1778 2023-04-03 11:32:01.569829 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2314 2023-04-03 11:32:01.541827 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      375 2023-04-03 11:31:52.241305 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2134 2023-04-03 11:32:01.613831 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      327 2023-04-03 11:31:52.133299 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      216 2023-04-03 11:31:52.801337 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3432 2023-04-03 11:32:01.625832 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7425 2023-04-03 11:32:01.709837 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3442 2023-04-03 11:32:01.669834 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2023 2023-04-03 11:32:01.701836 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2327 2023-04-03 11:32:01.737838 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2261 2023-04-03 11:32:01.741839 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      198 2023-04-03 11:31:51.945288 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-03 11:32:01.769840 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      198 2023-04-03 11:31:52.449317 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2016 2023-04-03 11:32:01.777840 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2067 2023-04-03 11:32:01.801842 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7349 2023-04-03 11:32:01.873846 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3408 2023-04-03 11:32:01.845844 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2013 2023-04-03 11:32:01.881846 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2317 2023-04-03 11:32:01.913848 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2241 2023-04-03 11:32:01.913848 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-04-03 11:31:52.241305 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2108 2023-04-03 11:32:01.945850 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-04-03 11:31:53.049351 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2006 2023-04-03 11:32:01.957851 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2057 2023-04-03 11:32:01.977852 windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1783 2023-04-03 11:32:02.017854 windmill_api-1.85.0/windmill_api/models/delete_invite_json_body.py
--rw-r--r--   0        0        0     6853 2023-04-03 11:32:02.109859 windmill_api-1.85.0/windmill_api/models/delete_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1309 2023-04-03 11:32:02.045856 windmill_api-1.85.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      258 2023-04-03 11:31:52.129299 windmill_api-1.85.0/windmill_api/models/delete_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      216 2023-04-03 11:31:53.073352 windmill_api-1.85.0/windmill_api/models/delete_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1283 2023-04-03 11:32:02.073857 windmill_api-1.85.0/windmill_api/models/delete_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     2933 2023-04-03 11:32:02.121860 windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5556 2023-04-03 11:32:02.177863 windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      326 2023-04-03 11:31:52.293308 windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1608 2023-04-03 11:32:02.149861 windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1673 2023-04-03 11:32:02.181863 windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2171 2023-04-03 11:32:02.209865 windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3293 2023-04-03 11:32:02.229866 windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      344 2023-04-03 11:31:51.957289 windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1641 2023-04-03 11:32:02.237866 windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3161 2023-04-03 11:32:02.281869 windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      335 2023-04-03 11:31:52.101297 windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1590 2023-04-03 11:32:02.265868 windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      180 2023-04-03 11:31:52.965346 windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     1551 2023-04-03 11:32:02.297870 windmill_api-1.85.0/windmill_api/models/edit_auto_invite_json_body.py
--rw-r--r--   0        0        0     1980 2023-04-03 11:32:02.317871 windmill_api-1.85.0/windmill_api/models/edit_resource.py
--rw-r--r--   0        0        0     1791 2023-04-03 11:32:02.325871 windmill_api-1.85.0/windmill_api/models/edit_resource_type.py
--rw-r--r--   0        0        0     1663 2023-04-03 11:32:02.353873 windmill_api-1.85.0/windmill_api/models/edit_schedule.py
--rw-r--r--   0        0        0     1176 2023-04-03 11:32:02.349872 windmill_api-1.85.0/windmill_api/models/edit_schedule_args.py
--rw-r--r--   0        0        0     1691 2023-04-03 11:32:02.377874 windmill_api-1.85.0/windmill_api/models/edit_slack_command_json_body.py
--rw-r--r--   0        0        0     2260 2023-04-03 11:32:02.393875 windmill_api-1.85.0/windmill_api/models/edit_variable.py
--rw-r--r--   0        0        0     1520 2023-04-03 11:32:02.405876 windmill_api-1.85.0/windmill_api/models/edit_webhook_json_body.py
--rw-r--r--   0        0        0     2058 2023-04-03 11:32:02.433877 windmill_api-1.85.0/windmill_api/models/edit_workspace_user.py
--rw-r--r--   0        0        0     3663 2023-04-03 11:32:02.493881 windmill_api-1.85.0/windmill_api/models/execute_component_json_body.py
--rw-r--r--   0        0        0     1346 2023-04-03 11:32:02.485880 windmill_api-1.85.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
--rw-r--r--   0        0        0     1942 2023-04-03 11:32:02.521882 windmill_api-1.85.0/windmill_api/models/execute_component_json_body_raw_code.py
--rw-r--r--   0        0        0     1577 2023-04-03 11:32:02.525882 windmill_api-1.85.0/windmill_api/models/exists_username_json_body.py
--rw-r--r--   0        0        0     1400 2023-04-03 11:32:02.549884 windmill_api-1.85.0/windmill_api/models/exists_workspace_json_body.py
--rw-r--r--   0        0        0     4633 2023-04-03 11:32:02.601887 windmill_api-1.85.0/windmill_api/models/flow.py
--rw-r--r--   0        0        0     1166 2023-04-03 11:32:02.573885 windmill_api-1.85.0/windmill_api/models/flow_extra_perms.py
--rw-r--r--   0        0        0     3416 2023-04-03 11:32:02.625888 windmill_api-1.85.0/windmill_api/models/flow_metadata.py
--rw-r--r--   0        0        0     1209 2023-04-03 11:32:02.625888 windmill_api-1.85.0/windmill_api/models/flow_metadata_extra_perms.py
--rw-r--r--   0        0        0     5729 2023-04-03 11:32:02.713893 windmill_api-1.85.0/windmill_api/models/flow_module.py
--rw-r--r--   0        0        0     2726 2023-04-03 11:32:02.673891 windmill_api-1.85.0/windmill_api/models/flow_module_retry.py
--rw-r--r--   0        0        0     1807 2023-04-03 11:32:02.709893 windmill_api-1.85.0/windmill_api/models/flow_module_retry_constant.py
--rw-r--r--   0        0        0     2111 2023-04-03 11:32:02.745895 windmill_api-1.85.0/windmill_api/models/flow_module_retry_exponential.py
--rw-r--r--   0        0        0     1834 2023-04-03 11:32:02.745895 windmill_api-1.85.0/windmill_api/models/flow_module_sleep_type_0.py
--rw-r--r--   0        0        0      159 2023-04-03 11:31:52.233304 windmill_api-1.85.0/windmill_api/models/flow_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1701 2023-04-03 11:32:02.781897 windmill_api-1.85.0/windmill_api/models/flow_module_sleep_type_1.py
--rw-r--r--   0        0        0      159 2023-04-03 11:31:52.781335 windmill_api-1.85.0/windmill_api/models/flow_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1800 2023-04-03 11:32:02.781897 windmill_api-1.85.0/windmill_api/models/flow_module_stop_after_if.py
--rw-r--r--   0        0        0     1851 2023-04-03 11:32:02.813898 windmill_api-1.85.0/windmill_api/models/flow_module_suspend.py
--rw-r--r--   0        0        0     3080 2023-04-03 11:32:02.829899 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_0.py
--rw-r--r--   0        0        0     3564 2023-04-03 11:32:02.853901 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-03 11:32:02.865901 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-03 11:31:52.805337 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-03 11:32:02.921904 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-03 11:31:52.165301 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      208 2023-04-03 11:31:52.293308 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_0_language.py
--rw-r--r--   0        0        0      158 2023-04-03 11:31:53.057351 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_0_type.py
--rw-r--r--   0        0        0     2477 2023-04-03 11:32:02.913904 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_1.py
--rw-r--r--   0        0        0     3564 2023-04-03 11:32:02.993909 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-03 11:32:02.957907 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-03 11:31:52.025293 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-03 11:32:02.989908 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-03 11:31:52.669329 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      152 2023-04-03 11:31:53.117354 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_1_type.py
--rw-r--r--   0        0        0     2204 2023-04-03 11:32:03.025910 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_2.py
--rw-r--r--   0        0        0     3564 2023-04-03 11:32:03.037911 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
--rw-r--r--   0        0        0     2261 2023-04-03 11:32:03.061912 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      198 2023-04-03 11:31:52.917343 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2128 2023-04-03 11:32:03.073913 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      198 2023-04-03 11:31:52.205303 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      148 2023-04-03 11:31:52.481319 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_2_type.py
--rw-r--r--   0        0        0     4138 2023-04-03 11:32:03.121916 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3.py
--rw-r--r--   0        0        0     1990 2023-04-03 11:32:03.109915 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
--rw-r--r--   0        0        0      173 2023-04-03 11:31:52.929344 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
--rw-r--r--   0        0        0     1857 2023-04-03 11:32:03.145917 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
--rw-r--r--   0        0        0      173 2023-04-03 11:31:52.061295 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
--rw-r--r--   0        0        0     6636 2023-04-03 11:32:03.217921 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py
--rw-r--r--   0        0        0     3148 2023-04-03 11:32:03.197920 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
--rw-r--r--   0        0        0     1935 2023-04-03 11:32:03.233922 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-04-03 11:32:03.257923 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-04-03 11:32:03.269924 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-03 11:31:52.309309 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-04-03 11:32:03.289925 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-03 11:31:52.393314 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-04-03 11:32:03.309926 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-04-03 11:32:03.325927 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
--rw-r--r--   0        0        0      162 2023-04-03 11:31:52.405314 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_type.py
--rw-r--r--   0        0        0     2934 2023-04-03 11:32:03.381930 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4.py
--rw-r--r--   0        0        0     2508 2023-04-03 11:32:03.409932 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py
--rw-r--r--   0        0        0     7243 2023-04-03 11:32:03.481936 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-04-03 11:32:03.453935 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-04-03 11:32:03.489936 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-04-03 11:32:03.525939 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-04-03 11:32:03.525939 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-03 11:31:52.609326 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-04-03 11:32:03.557940 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-03 11:31:53.121355 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-04-03 11:32:03.561941 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-04-03 11:32:03.593942 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0     6636 2023-04-03 11:32:03.661946 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item.py
--rw-r--r--   0        0        0     3148 2023-04-03 11:32:03.649946 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
--rw-r--r--   0        0        0     1935 2023-04-03 11:32:03.685948 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
--rw-r--r--   0        0        0     2239 2023-04-03 11:32:03.701949 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
--rw-r--r--   0        0        0     2087 2023-04-03 11:32:03.729950 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
--rw-r--r--   0        0        0      181 2023-04-03 11:31:52.817338 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1954 2023-04-03 11:32:03.733950 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
--rw-r--r--   0        0        0      181 2023-04-03 11:31:52.281307 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1928 2023-04-03 11:32:03.765952 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
--rw-r--r--   0        0        0     1979 2023-04-03 11:32:03.765952 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
--rw-r--r--   0        0        0      158 2023-04-03 11:31:52.921343 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_type.py
--rw-r--r--   0        0        0     2577 2023-04-03 11:32:03.845957 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5.py
--rw-r--r--   0        0        0     2679 2023-04-03 11:32:03.809955 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py
--rw-r--r--   0        0        0     7243 2023-04-03 11:32:03.953963 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
--rw-r--r--   0        0        0     3362 2023-04-03 11:32:03.893959 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
--rw-r--r--   0        0        0     2001 2023-04-03 11:32:03.929962 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2305 2023-04-03 11:32:03.965963 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2215 2023-04-03 11:32:03.993965 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-03 11:31:52.765335 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2082 2023-04-03 11:32:04.001966 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-03 11:31:51.925287 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1994 2023-04-03 11:32:04.033967 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2045 2023-04-03 11:32:04.037968 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
--rw-r--r--   0        0        0      158 2023-04-03 11:31:52.465318 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_type.py
--rw-r--r--   0        0        0     1839 2023-04-03 11:32:04.073970 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_6.py
--rw-r--r--   0        0        0      156 2023-04-03 11:31:53.069352 windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_6_type.py
--rw-r--r--   0        0        0     2009 2023-04-03 11:32:04.077970 windmill_api-1.85.0/windmill_api/models/flow_preview.py
--rw-r--r--   0        0        0     1171 2023-04-03 11:32:04.097971 windmill_api-1.85.0/windmill_api/models/flow_preview_args.py
--rw-r--r--   0        0        0     3074 2023-04-03 11:32:04.125973 windmill_api-1.85.0/windmill_api/models/flow_preview_value.py
--rw-r--r--   0        0        0     6498 2023-04-03 11:32:04.197977 windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module.py
--rw-r--r--   0        0        0     3064 2023-04-03 11:32:04.173975 windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_retry.py
--rw-r--r--   0        0        0     1911 2023-04-03 11:32:04.209977 windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2215 2023-04-03 11:32:04.237979 windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2036 2023-04-03 11:32:04.241979 windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-03 11:31:52.485319 windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1903 2023-04-03 11:32:04.273981 windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-03 11:31:52.709331 windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1904 2023-04-03 11:32:04.317983 windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1955 2023-04-03 11:32:04.309983 windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6422 2023-04-03 11:32:04.461992 windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item.py
--rw-r--r--   0        0        0     3030 2023-04-03 11:32:04.361986 windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_retry.py
--rw-r--r--   0        0        0     1901 2023-04-03 11:32:04.397988 windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2205 2023-04-03 11:32:04.437990 windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2016 2023-04-03 11:32:04.469992 windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-04-03 11:31:52.985347 windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1883 2023-04-03 11:32:04.497994 windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-04-03 11:31:52.297308 windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1894 2023-04-03 11:32:04.505994 windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1945 2023-04-03 11:32:04.533996 windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1143 2023-04-03 11:32:04.533996 windmill_api-1.85.0/windmill_api/models/flow_schema.py
--rw-r--r--   0        0        0     3001 2023-04-03 11:32:04.585999 windmill_api-1.85.0/windmill_api/models/flow_status.py
--rw-r--r--   0        0        0     6370 2023-04-03 11:32:04.650002 windmill_api-1.85.0/windmill_api/models/flow_status_failure_module.py
--rw-r--r--   0        0        0     1723 2023-04-03 11:32:04.618000 windmill_api-1.85.0/windmill_api/models/flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     1999 2023-04-03 11:32:04.650002 windmill_api-1.85.0/windmill_api/models/flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      190 2023-04-03 11:31:52.977347 windmill_api-1.85.0/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1628 2023-04-03 11:32:04.682004 windmill_api-1.85.0/windmill_api/models/flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2164 2023-04-03 11:32:04.698005 windmill_api-1.85.0/windmill_api/models/flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      348 2023-04-03 11:31:52.493319 windmill_api-1.85.0/windmill_api/models/flow_status_failure_module_type.py
--rw-r--r--   0        0        0     5808 2023-04-03 11:32:04.830012 windmill_api-1.85.0/windmill_api/models/flow_status_module.py
--rw-r--r--   0        0        0     1685 2023-04-03 11:32:04.730007 windmill_api-1.85.0/windmill_api/models/flow_status_module_approvers_item.py
--rw-r--r--   0        0        0     1925 2023-04-03 11:32:04.766009 windmill_api-1.85.0/windmill_api/models/flow_status_module_branch_chosen.py
--rw-r--r--   0        0        0      183 2023-04-03 11:31:52.657328 windmill_api-1.85.0/windmill_api/models/flow_status_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1590 2023-04-03 11:32:04.802011 windmill_api-1.85.0/windmill_api/models/flow_status_module_branchall.py
--rw-r--r--   0        0        0     2126 2023-04-03 11:32:04.914017 windmill_api-1.85.0/windmill_api/models/flow_status_module_iterator.py
--rw-r--r--   0        0        0      341 2023-04-03 11:31:52.401314 windmill_api-1.85.0/windmill_api/models/flow_status_module_type.py
--rw-r--r--   0        0        0     5981 2023-04-03 11:32:04.930018 windmill_api-1.85.0/windmill_api/models/flow_status_modules_item.py
--rw-r--r--   0        0        0     1713 2023-04-03 11:32:04.946019 windmill_api-1.85.0/windmill_api/models/flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     1979 2023-04-03 11:32:04.966020 windmill_api-1.85.0/windmill_api/models/flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      188 2023-04-03 11:31:52.997348 windmill_api-1.85.0/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1618 2023-04-03 11:32:04.978021 windmill_api-1.85.0/windmill_api/models/flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2154 2023-04-03 11:32:05.010023 windmill_api-1.85.0/windmill_api/models/flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      346 2023-04-03 11:31:52.357312 windmill_api-1.85.0/windmill_api/models/flow_status_modules_item_type.py
--rw-r--r--   0        0        0     1974 2023-04-03 11:32:05.022023 windmill_api-1.85.0/windmill_api/models/flow_status_retry.py
--rw-r--r--   0        0        0     2957 2023-04-03 11:32:05.058025 windmill_api-1.85.0/windmill_api/models/flow_value.py
--rw-r--r--   0        0        0     6224 2023-04-03 11:32:05.122029 windmill_api-1.85.0/windmill_api/models/flow_value_failure_module.py
--rw-r--r--   0        0        0     2940 2023-04-03 11:32:05.106028 windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1873 2023-04-03 11:32:05.142030 windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-04-03 11:32:05.162031 windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-04-03 11:32:05.178032 windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-04-03 11:31:52.725332 windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-04-03 11:32:05.202034 windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-04-03 11:31:52.001291 windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-04-03 11:32:05.270038 windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-04-03 11:32:05.238036 windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6125 2023-04-03 11:32:05.410045 windmill_api-1.85.0/windmill_api/models/flow_value_modules_item.py
--rw-r--r--   0        0        0     2906 2023-04-03 11:32:05.318040 windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1863 2023-04-03 11:32:05.354042 windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2167 2023-04-03 11:32:05.390044 windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1942 2023-04-03 11:32:05.426046 windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      169 2023-04-03 11:31:52.701331 windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1809 2023-04-03 11:32:05.442047 windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      169 2023-04-03 11:31:52.429316 windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1856 2023-04-03 11:32:05.462048 windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1907 2023-04-03 11:32:05.482049 windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1858 2023-04-03 11:32:05.498050 windmill_api-1.85.0/windmill_api/models/folder.py
--rw-r--r--   0        0        0     1179 2023-04-03 11:32:05.506051 windmill_api-1.85.0/windmill_api/models/folder_extra_perms.py
--rw-r--r--   0        0        0     1560 2023-04-03 11:32:05.530052 windmill_api-1.85.0/windmill_api/models/force_cancel_queued_job_json_body.py
--rw-r--r--   0        0        0     3807 2023-04-03 11:32:05.570054 windmill_api-1.85.0/windmill_api/models/forloop_flow.py
--rw-r--r--   0        0        0     1874 2023-04-03 11:32:05.562054 windmill_api-1.85.0/windmill_api/models/forloop_flow_iterator_type_0.py
--rw-r--r--   0        0        0      163 2023-04-03 11:31:52.697331 windmill_api-1.85.0/windmill_api/models/forloop_flow_iterator_type_0_type.py
--rw-r--r--   0        0        0     1741 2023-04-03 11:32:05.598056 windmill_api-1.85.0/windmill_api/models/forloop_flow_iterator_type_1.py
--rw-r--r--   0        0        0      163 2023-04-03 11:31:52.693331 windmill_api-1.85.0/windmill_api/models/forloop_flow_iterator_type_1_type.py
--rw-r--r--   0        0        0     6224 2023-04-03 11:32:05.670060 windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item.py
--rw-r--r--   0        0        0     2940 2023-04-03 11:32:05.646059 windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1873 2023-04-03 11:32:05.678061 windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2177 2023-04-03 11:32:05.710062 windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1962 2023-04-03 11:32:05.750065 windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      171 2023-04-03 11:31:53.149356 windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1829 2023-04-03 11:32:05.746064 windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      171 2023-04-03 11:31:52.405314 windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1866 2023-04-03 11:32:05.782066 windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1917 2023-04-03 11:32:05.786067 windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_suspend.py
--rw-r--r--   0        0        0      152 2023-04-03 11:31:52.413315 windmill_api-1.85.0/windmill_api/models/forloop_flow_type.py
--rw-r--r--   0        0        0     4052 2023-04-03 11:32:05.846070 windmill_api-1.85.0/windmill_api/models/get_app_by_path_response_200.py
--rw-r--r--   0        0        0      219 2023-04-03 11:31:52.985347 windmill_api-1.85.0/windmill_api/models/get_app_by_path_response_200_execution_mode.py
--rw-r--r--   0        0        0     1279 2023-04-03 11:32:05.810068 windmill_api-1.85.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     3811 2023-04-03 11:32:05.866071 windmill_api-1.85.0/windmill_api/models/get_app_by_path_response_200_policy.py
--rw-r--r--   0        0        0      225 2023-04-03 11:31:52.557323 windmill_api-1.85.0/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2009 2023-04-03 11:32:05.954076 windmill_api-1.85.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1412 2023-04-03 11:32:05.890072 windmill_api-1.85.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     4112 2023-04-03 11:32:05.950076 windmill_api-1.85.0/windmill_api/models/get_app_by_version_response_200.py
--rw-r--r--   0        0        0      222 2023-04-03 11:31:52.577324 windmill_api-1.85.0/windmill_api/models/get_app_by_version_response_200_execution_mode.py
--rw-r--r--   0        0        0     1294 2023-04-03 11:32:05.978078 windmill_api-1.85.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py
--rw-r--r--   0        0        0     3862 2023-04-03 11:32:06.014080 windmill_api-1.85.0/windmill_api/models/get_app_by_version_response_200_policy.py
--rw-r--r--   0        0        0      228 2023-04-03 11:31:52.973346 windmill_api-1.85.0/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2042 2023-04-03 11:32:06.010079 windmill_api-1.85.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1427 2023-04-03 11:32:06.034081 windmill_api-1.85.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3764 2023-04-03 11:32:06.078083 windmill_api-1.85.0/windmill_api/models/get_audit_log_response_200.py
--rw-r--r--   0        0        0      231 2023-04-03 11:31:52.041293 windmill_api-1.85.0/windmill_api/models/get_audit_log_response_200_action_kind.py
--rw-r--r--   0        0        0      634 2023-04-03 11:31:52.137299 windmill_api-1.85.0/windmill_api/models/get_audit_log_response_200_operation.py
--rw-r--r--   0        0        0     1265 2023-04-03 11:32:06.062082 windmill_api-1.85.0/windmill_api/models/get_audit_log_response_200_parameters.py
--rw-r--r--   0        0        0    10876 2023-04-03 11:32:06.294095 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200.py
--rw-r--r--   0        0        0     1255 2023-04-03 11:32:06.102084 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_args.py
--rw-r--r--   0        0        0     3595 2023-04-03 11:32:06.154087 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status.py
--rw-r--r--   0        0        0     7343 2023-04-03 11:32:06.258093 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
--rw-r--r--   0        0        0     1868 2023-04-03 11:32:06.290095 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2288 2023-04-03 11:32:06.326097 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      216 2023-04-03 11:31:52.161300 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1773 2023-04-03 11:32:06.326097 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2309 2023-04-03 11:32:06.442104 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      374 2023-04-03 11:31:52.997348 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6924 2023-04-03 11:32:06.422103 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
--rw-r--r--   0        0        0     1858 2023-04-03 11:32:06.454105 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-04-03 11:32:06.478106 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-04-03 11:31:52.917343 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-04-03 11:32:06.486106 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2299 2023-04-03 11:32:06.522108 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      372 2023-04-03 11:31:52.501320 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2119 2023-04-03 11:32:06.526109 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
--rw-r--r--   0        0        0      324 2023-04-03 11:31:52.417315 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_job_kind.py
--rw-r--r--   0        0        0      213 2023-04-03 11:31:52.941345 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_language.py
--rw-r--r--   0        0        0     3375 2023-04-03 11:32:06.578112 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow.py
--rw-r--r--   0        0        0     7311 2023-04-03 11:32:06.630114 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3391 2023-04-03 11:32:06.630114 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2008 2023-04-03 11:32:06.666117 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2312 2023-04-03 11:32:06.742121 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2231 2023-04-03 11:32:06.698118 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      195 2023-04-03 11:31:53.181358 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2098 2023-04-03 11:32:06.730120 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      195 2023-04-03 11:31:52.769335 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2001 2023-04-03 11:32:06.766122 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2052 2023-04-03 11:32:06.778123 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7235 2023-04-03 11:32:06.938132 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3357 2023-04-03 11:32:06.826125 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1998 2023-04-03 11:32:06.862128 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-04-03 11:32:06.898130 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-04-03 11:32:06.934132 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-03 11:31:52.645328 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-04-03 11:32:06.970134 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-03 11:31:52.421315 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-04-03 11:32:06.974134 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-04-03 11:32:07.006136 windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     5083 2023-04-03 11:32:07.054139 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200.py
--rw-r--r--   0        0        0     1281 2023-04-03 11:32:07.030137 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0     1258 2023-04-03 11:32:07.054139 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_schema.py
--rw-r--r--   0        0        0     3302 2023-04-03 11:32:07.106141 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value.py
--rw-r--r--   0        0        0     7159 2023-04-03 11:32:07.206147 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
--rw-r--r--   0        0        0     3323 2023-04-03 11:32:07.154144 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
--rw-r--r--   0        0        0     1988 2023-04-03 11:32:07.186146 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-04-03 11:32:07.226148 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-04-03 11:32:07.242149 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-03 11:31:52.261306 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-04-03 11:32:07.262150 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-03 11:31:52.253306 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-04-03 11:32:07.290152 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-04-03 11:32:07.294152 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7066 2023-04-03 11:32:07.394158 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
--rw-r--r--   0        0        0     3289 2023-04-03 11:32:07.342155 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
--rw-r--r--   0        0        0     1978 2023-04-03 11:32:07.378157 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2282 2023-04-03 11:32:07.418159 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2171 2023-04-03 11:32:07.430160 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-03 11:31:53.173358 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2038 2023-04-03 11:32:07.522165 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-03 11:31:52.381313 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1971 2023-04-03 11:32:07.466162 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2022 2023-04-03 11:32:07.502164 windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2010 2023-04-03 11:32:07.538166 windmill_api-1.85.0/windmill_api/models/get_folder_response_200.py
--rw-r--r--   0        0        0     1258 2023-04-03 11:32:07.550167 windmill_api-1.85.0/windmill_api/models/get_folder_response_200_extra_perms.py
--rw-r--r--   0        0        0     2357 2023-04-03 11:32:07.586169 windmill_api-1.85.0/windmill_api/models/get_folder_usage_response_200.py
--rw-r--r--   0        0        0      301 2023-04-03 11:31:53.025349 windmill_api-1.85.0/windmill_api/models/get_granular_acls_kind.py
--rw-r--r--   0        0        0     1235 2023-04-03 11:32:07.574168 windmill_api-1.85.0/windmill_api/models/get_granular_acls_response_200.py
--rw-r--r--   0        0        0     2888 2023-04-03 11:32:07.626171 windmill_api-1.85.0/windmill_api/models/get_group_response_200.py
--rw-r--r--   0        0        0     1253 2023-04-03 11:32:07.610170 windmill_api-1.85.0/windmill_api/models/get_group_response_200_extra_perms.py
--rw-r--r--   0        0        0     1606 2023-04-03 11:32:07.642172 windmill_api-1.85.0/windmill_api/models/get_hub_app_by_id_response_200.py
--rw-r--r--   0        0        0     1634 2023-04-03 11:32:07.658173 windmill_api-1.85.0/windmill_api/models/get_hub_app_by_id_response_200_app.py
--rw-r--r--   0        0        0     1977 2023-04-03 11:32:07.726177 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200.py
--rw-r--r--   0        0        0     2950 2023-04-03 11:32:07.706175 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
--rw-r--r--   0        0        0     1289 2023-04-03 11:32:07.730177 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
--rw-r--r--   0        0        0     3410 2023-04-03 11:32:07.778180 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
--rw-r--r--   0        0        0     7365 2023-04-03 11:32:07.830182 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
--rw-r--r--   0        0        0     3418 2023-04-03 11:32:07.826182 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     2019 2023-04-03 11:32:07.858184 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2323 2023-04-03 11:32:07.870185 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2249 2023-04-03 11:32:07.898186 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      196 2023-04-03 11:31:53.129355 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2116 2023-04-03 11:32:07.906187 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      196 2023-04-03 11:31:52.289308 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2012 2023-04-03 11:32:07.930188 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2063 2023-04-03 11:32:08.018193 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7289 2023-04-03 11:32:08.030194 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
--rw-r--r--   0        0        0     3384 2023-04-03 11:32:08.070196 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     2009 2023-04-03 11:32:08.066196 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2313 2023-04-03 11:32:08.102198 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2229 2023-04-03 11:32:08.106198 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      194 2023-04-03 11:31:52.077296 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2096 2023-04-03 11:32:08.190203 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      194 2023-04-03 11:31:52.401314 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2002 2023-04-03 11:32:08.142200 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2053 2023-04-03 11:32:08.178202 windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2698 2023-04-03 11:32:08.226205 windmill_api-1.85.0/windmill_api/models/get_hub_script_by_path_response_200.py
--rw-r--r--   0        0        0      216 2023-04-03 11:31:52.053294 windmill_api-1.85.0/windmill_api/models/get_hub_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     1852 2023-04-03 11:32:08.230205 windmill_api-1.85.0/windmill_api/models/get_job_response_200.py
--rw-r--r--   0        0        0      188 2023-04-03 11:31:52.181301 windmill_api-1.85.0/windmill_api/models/get_job_response_200_type.py
--rw-r--r--   0        0        0     2364 2023-04-03 11:32:08.274208 windmill_api-1.85.0/windmill_api/models/get_job_updates_response_200.py
--rw-r--r--   0        0        0     1744 2023-04-03 11:32:08.266207 windmill_api-1.85.0/windmill_api/models/get_premium_info_response_200.py
--rw-r--r--   0        0        0     4218 2023-04-03 11:32:08.326211 windmill_api-1.85.0/windmill_api/models/get_public_app_by_secret_response_200.py
--rw-r--r--   0        0        0      227 2023-04-03 11:31:52.273307 windmill_api-1.85.0/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
--rw-r--r--   0        0        0     1322 2023-04-03 11:32:08.298209 windmill_api-1.85.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
--rw-r--r--   0        0        0     3970 2023-04-03 11:32:08.354212 windmill_api-1.85.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py
--rw-r--r--   0        0        0      233 2023-04-03 11:31:52.369312 windmill_api-1.85.0/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
--rw-r--r--   0        0        0     2131 2023-04-03 11:32:08.362213 windmill_api-1.85.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
--rw-r--r--   0        0        0     1455 2023-04-03 11:32:08.378214 windmill_api-1.85.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     3533 2023-04-03 11:32:08.422216 windmill_api-1.85.0/windmill_api/models/get_resource_response_200.py
--rw-r--r--   0        0        0     1268 2023-04-03 11:32:08.402215 windmill_api-1.85.0/windmill_api/models/get_resource_response_200_extra_perms.py
--rw-r--r--   0        0        0     2335 2023-04-03 11:32:08.442217 windmill_api-1.85.0/windmill_api/models/get_resource_type_response_200.py
--rw-r--r--   0        0        0     1840 2023-04-03 11:32:08.454218 windmill_api-1.85.0/windmill_api/models/get_resume_urls_response_200.py
--rw-r--r--   0        0        0     4307 2023-04-03 11:32:08.514221 windmill_api-1.85.0/windmill_api/models/get_schedule_response_200.py
--rw-r--r--   0        0        0     1232 2023-04-03 11:32:08.482220 windmill_api-1.85.0/windmill_api/models/get_schedule_response_200_args.py
--rw-r--r--   0        0        0     1268 2023-04-03 11:32:08.502220 windmill_api-1.85.0/windmill_api/models/get_schedule_response_200_extra_perms.py
--rw-r--r--   0        0        0     6775 2023-04-03 11:32:08.686231 windmill_api-1.85.0/windmill_api/models/get_script_by_hash_response_200.py
--rw-r--r--   0        0        0     1294 2023-04-03 11:32:08.538223 windmill_api-1.85.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-03 11:31:52.901342 windmill_api-1.85.0/windmill_api/models/get_script_by_hash_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-04-03 11:31:52.441316 windmill_api-1.85.0/windmill_api/models/get_script_by_hash_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-04-03 11:32:08.566224 windmill_api-1.85.0/windmill_api/models/get_script_by_hash_response_200_schema.py
--rw-r--r--   0        0        0     6775 2023-04-03 11:32:08.722233 windmill_api-1.85.0/windmill_api/models/get_script_by_path_response_200.py
--rw-r--r--   0        0        0     1294 2023-04-03 11:32:08.710232 windmill_api-1.85.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-03 11:31:53.085353 windmill_api-1.85.0/windmill_api/models/get_script_by_path_response_200_kind.py
--rw-r--r--   0        0        0      213 2023-04-03 11:31:53.129355 windmill_api-1.85.0/windmill_api/models/get_script_by_path_response_200_language.py
--rw-r--r--   0        0        0     1268 2023-04-03 11:32:08.738234 windmill_api-1.85.0/windmill_api/models/get_script_by_path_response_200_schema.py
--rw-r--r--   0        0        0     1922 2023-04-03 11:32:08.758235 windmill_api-1.85.0/windmill_api/models/get_script_deployment_status_response_200.py
--rw-r--r--   0        0        0     4157 2023-04-03 11:32:08.806238 windmill_api-1.85.0/windmill_api/models/get_settings_response_200.py
--rw-r--r--   0        0        0     2428 2023-04-03 11:32:08.794237 windmill_api-1.85.0/windmill_api/models/get_suspended_job_flow_response_200.py
--rw-r--r--   0        0        0     1764 2023-04-03 11:32:08.826239 windmill_api-1.85.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
--rw-r--r--   0        0        0     2040 2023-04-03 11:32:08.846240 windmill_api-1.85.0/windmill_api/models/get_suspended_job_flow_response_200_job.py
--rw-r--r--   0        0        0      204 2023-04-03 11:31:52.965346 windmill_api-1.85.0/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
--rw-r--r--   0        0        0     4554 2023-04-03 11:32:08.898243 windmill_api-1.85.0/windmill_api/models/get_variable_response_200.py
--rw-r--r--   0        0        0     1268 2023-04-03 11:32:08.866241 windmill_api-1.85.0/windmill_api/models/get_variable_response_200_extra_perms.py
--rw-r--r--   0        0        0     2647 2023-04-03 11:32:08.914244 windmill_api-1.85.0/windmill_api/models/global_user_info.py
--rw-r--r--   0        0        0      176 2023-04-03 11:31:52.641327 windmill_api-1.85.0/windmill_api/models/global_user_info_login_type.py
--rw-r--r--   0        0        0     1627 2023-04-03 11:32:08.930245 windmill_api-1.85.0/windmill_api/models/global_user_update_json_body.py
--rw-r--r--   0        0        0     2741 2023-04-03 11:32:08.966247 windmill_api-1.85.0/windmill_api/models/global_whoami_response_200.py
--rw-r--r--   0        0        0      185 2023-04-03 11:31:52.105297 windmill_api-1.85.0/windmill_api/models/global_whoami_response_200_login_type.py
--rw-r--r--   0        0        0     2903 2023-04-03 11:32:08.978248 windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5478 2023-04-03 11:32:09.038251 windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      324 2023-04-03 11:31:53.101354 windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1598 2023-04-03 11:32:09.010249 windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1663 2023-04-03 11:32:09.042251 windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2151 2023-04-03 11:32:09.170258 windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3257 2023-04-03 11:32:09.150257 windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      342 2023-04-03 11:31:52.489319 windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1631 2023-04-03 11:32:09.182259 windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3100 2023-04-03 11:32:09.218261 windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      333 2023-04-03 11:31:52.861340 windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1580 2023-04-03 11:32:09.218261 windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      178 2023-04-03 11:31:51.953289 windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0     2722 2023-04-03 11:32:09.270264 windmill_api-1.85.0/windmill_api/models/group.py
--rw-r--r--   0        0        0     1174 2023-04-03 11:32:09.246263 windmill_api-1.85.0/windmill_api/models/group_extra_perms.py
--rw-r--r--   0        0        0     1689 2023-04-03 11:32:09.282265 windmill_api-1.85.0/windmill_api/models/identity.py
--rw-r--r--   0        0        0      143 2023-04-03 11:31:52.241305 windmill_api-1.85.0/windmill_api/models/identity_type.py
--rw-r--r--   0        0        0     1820 2023-04-03 11:32:09.306266 windmill_api-1.85.0/windmill_api/models/input_transform_type_0.py
--rw-r--r--   0        0        0      158 2023-04-03 11:31:52.685330 windmill_api-1.85.0/windmill_api/models/input_transform_type_0_type.py
--rw-r--r--   0        0        0     1687 2023-04-03 11:32:09.318267 windmill_api-1.85.0/windmill_api/models/input_transform_type_1.py
--rw-r--r--   0        0        0      158 2023-04-03 11:31:52.765335 windmill_api-1.85.0/windmill_api/models/input_transform_type_1_type.py
--rw-r--r--   0        0        0     1773 2023-04-03 11:32:09.342268 windmill_api-1.85.0/windmill_api/models/invite_user_json_body.py
--rw-r--r--   0        0        0     1679 2023-04-03 11:32:09.350269 windmill_api-1.85.0/windmill_api/models/javascript_transform.py
--rw-r--r--   0        0        0      158 2023-04-03 11:31:52.793336 windmill_api-1.85.0/windmill_api/models/javascript_transform_type.py
--rw-r--r--   0        0        0     1686 2023-04-03 11:32:09.382270 windmill_api-1.85.0/windmill_api/models/job.py
--rw-r--r--   0        0        0      174 2023-04-03 11:31:52.853340 windmill_api-1.85.0/windmill_api/models/job_type.py
--rw-r--r--   0        0        0     3583 2023-04-03 11:32:09.406272 windmill_api-1.85.0/windmill_api/models/list_apps_response_200_item.py
--rw-r--r--   0        0        0      219 2023-04-03 11:31:51.917286 windmill_api-1.85.0/windmill_api/models/list_apps_response_200_item_execution_mode.py
--rw-r--r--   0        0        0     1276 2023-04-03 11:32:09.410272 windmill_api-1.85.0/windmill_api/models/list_apps_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      218 2023-04-03 11:31:52.913343 windmill_api-1.85.0/windmill_api/models/list_audit_logs_action_kind.py
--rw-r--r--   0        0        0     3896 2023-04-03 11:32:09.470275 windmill_api-1.85.0/windmill_api/models/list_audit_logs_response_200_item.py
--rw-r--r--   0        0        0      237 2023-04-03 11:31:52.173301 windmill_api-1.85.0/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
--rw-r--r--   0        0        0      640 2023-04-03 11:31:52.409314 windmill_api-1.85.0/windmill_api/models/list_audit_logs_response_200_item_operation.py
--rw-r--r--   0        0        0     1298 2023-04-03 11:32:09.442274 windmill_api-1.85.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py
--rw-r--r--   0        0        0    11088 2023-04-03 11:32:09.686288 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item.py
--rw-r--r--   0        0        0     1288 2023-04-03 11:32:09.494277 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_args.py
--rw-r--r--   0        0        0     3736 2023-04-03 11:32:09.546280 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7579 2023-04-03 11:32:09.706289 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1901 2023-04-03 11:32:09.718289 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2352 2023-04-03 11:32:09.742291 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      222 2023-04-03 11:31:52.545322 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1806 2023-04-03 11:32:09.754292 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2342 2023-04-03 11:32:09.786293 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      380 2023-04-03 11:31:52.209303 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     7160 2023-04-03 11:32:09.854297 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1891 2023-04-03 11:32:09.814295 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2332 2023-04-03 11:32:09.850297 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      220 2023-04-03 11:31:52.733333 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1796 2023-04-03 11:32:09.882299 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2332 2023-04-03 11:32:09.898300 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      378 2023-04-03 11:31:52.597325 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2152 2023-04-03 11:32:09.922301 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      330 2023-04-03 11:31:52.229304 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
--rw-r--r--   0        0        0      219 2023-04-03 11:31:52.405314 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_language.py
--rw-r--r--   0        0        0     3485 2023-04-03 11:32:09.954303 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7593 2023-04-03 11:32:10.022307 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3498 2023-04-03 11:32:10.002306 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     2041 2023-04-03 11:32:10.038308 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2345 2023-04-03 11:32:10.062309 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2295 2023-04-03 11:32:10.078310 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      201 2023-04-03 11:31:52.993348 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2162 2023-04-03 11:32:10.154314 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      201 2023-04-03 11:31:52.649328 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     2034 2023-04-03 11:32:10.206317 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2085 2023-04-03 11:32:10.190316 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7471 2023-04-03 11:32:10.290322 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3464 2023-04-03 11:32:10.254320 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     2031 2023-04-03 11:32:10.290322 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2335 2023-04-03 11:32:10.330324 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2275 2023-04-03 11:32:10.326324 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      199 2023-04-03 11:31:52.233304 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2142 2023-04-03 11:32:10.362326 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      199 2023-04-03 11:31:52.197302 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     2024 2023-04-03 11:32:10.370326 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2075 2023-04-03 11:32:10.398328 windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     1865 2023-04-03 11:32:10.406329 windmill_api-1.85.0/windmill_api/models/list_contextual_variables_response_200_item.py
--rw-r--r--   0        0        0     5077 2023-04-03 11:32:10.474332 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item.py
--rw-r--r--   0        0        0     1278 2023-04-03 11:32:10.430330 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     1255 2023-04-03 11:32:10.454331 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_schema.py
--rw-r--r--   0        0        0     3297 2023-04-03 11:32:10.506334 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value.py
--rw-r--r--   0        0        0     7151 2023-04-03 11:32:10.646342 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py
--rw-r--r--   0        0        0     3318 2023-04-03 11:32:10.554337 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py
--rw-r--r--   0        0        0     1985 2023-04-03 11:32:10.594339 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2289 2023-04-03 11:32:10.630341 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2187 2023-04-03 11:32:10.666343 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-03 11:31:52.549322 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2054 2023-04-03 11:32:10.678344 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-03 11:31:52.613326 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1978 2023-04-03 11:32:10.702345 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2029 2023-04-03 11:32:10.714346 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py
--rw-r--r--   0        0        0     7049 2023-04-03 11:32:10.886356 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py
--rw-r--r--   0        0        0     3284 2023-04-03 11:32:10.762349 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py
--rw-r--r--   0        0        0     1975 2023-04-03 11:32:10.798351 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-04-03 11:32:10.834353 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-04-03 11:32:10.870355 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-03 11:31:52.917343 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-04-03 11:32:10.906357 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-03 11:31:52.629327 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-04-03 11:32:10.926358 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-04-03 11:32:10.942359 windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2074 2023-04-03 11:32:10.966360 windmill_api-1.85.0/windmill_api/models/list_folders_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-04-03 11:32:10.966360 windmill_api-1.85.0/windmill_api/models/list_folders_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2958 2023-04-03 11:32:11.018363 windmill_api-1.85.0/windmill_api/models/list_groups_response_200_item.py
--rw-r--r--   0        0        0     1286 2023-04-03 11:32:10.990362 windmill_api-1.85.0/windmill_api/models/list_groups_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2076 2023-04-03 11:32:11.034364 windmill_api-1.85.0/windmill_api/models/list_hub_apps_response_200.py
--rw-r--r--   0        0        0     2304 2023-04-03 11:32:11.062366 windmill_api-1.85.0/windmill_api/models/list_hub_apps_response_200_apps_item.py
--rw-r--r--   0        0        0     2116 2023-04-03 11:32:11.074366 windmill_api-1.85.0/windmill_api/models/list_hub_flows_response_200.py
--rw-r--r--   0        0        0     2324 2023-04-03 11:32:11.106368 windmill_api-1.85.0/windmill_api/models/list_hub_flows_response_200_flows_item.py
--rw-r--r--   0        0        0     2106 2023-04-03 11:32:11.110368 windmill_api-1.85.0/windmill_api/models/list_hub_scripts_response_200.py
--rw-r--r--   0        0        0     2790 2023-04-03 11:32:11.158371 windmill_api-1.85.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py
--rw-r--r--   0        0        0      262 2023-04-03 11:31:51.997291 windmill_api-1.85.0/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
--rw-r--r--   0        0        0     1922 2023-04-03 11:32:11.210374 windmill_api-1.85.0/windmill_api/models/list_jobs_response_200_item.py
--rw-r--r--   0        0        0      194 2023-04-03 11:31:52.729333 windmill_api-1.85.0/windmill_api/models/list_jobs_response_200_item_type.py
--rw-r--r--   0        0        0     2076 2023-04-03 11:32:11.198373 windmill_api-1.85.0/windmill_api/models/list_pending_invites_response_200_item.py
--rw-r--r--   0        0        0    11982 2023-04-03 11:32:11.494390 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item.py
--rw-r--r--   0        0        0     1245 2023-04-03 11:32:11.238376 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_args.py
--rw-r--r--   0        0        0     3544 2023-04-03 11:32:11.318380 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status.py
--rw-r--r--   0        0        0     7247 2023-04-03 11:32:11.418386 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
--rw-r--r--   0        0        0     1858 2023-04-03 11:32:11.450388 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2268 2023-04-03 11:32:11.486390 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      214 2023-04-03 11:31:52.809337 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1763 2023-04-03 11:32:11.522392 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2299 2023-04-03 11:32:11.538393 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      372 2023-04-03 11:31:52.277307 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6858 2023-04-03 11:32:11.626397 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
--rw-r--r--   0        0        0     1848 2023-04-03 11:32:11.566394 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2248 2023-04-03 11:32:11.602396 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      212 2023-04-03 11:31:52.893342 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1753 2023-04-03 11:32:11.638398 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2289 2023-04-03 11:32:11.742404 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      370 2023-04-03 11:31:53.121355 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2109 2023-04-03 11:32:11.678401 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
--rw-r--r--   0        0        0      322 2023-04-03 11:31:52.133299 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_job_kind.py
--rw-r--r--   0        0        0      211 2023-04-03 11:31:52.981347 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_language.py
--rw-r--r--   0        0        0     3334 2023-04-03 11:32:11.738404 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow.py
--rw-r--r--   0        0        0     7235 2023-04-03 11:32:11.942416 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3357 2023-04-03 11:32:11.790407 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1998 2023-04-03 11:32:11.826409 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2302 2023-04-03 11:32:11.866411 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2211 2023-04-03 11:32:11.898413 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      193 2023-04-03 11:31:52.621327 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2078 2023-04-03 11:32:11.934415 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      193 2023-04-03 11:31:53.081353 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1991 2023-04-03 11:32:11.974417 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2042 2023-04-03 11:32:11.978417 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     7159 2023-04-03 11:32:12.074423 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3323 2023-04-03 11:32:12.026420 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1988 2023-04-03 11:32:12.062422 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2292 2023-04-03 11:32:12.102424 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2191 2023-04-03 11:32:12.110425 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      191 2023-04-03 11:31:53.177358 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2058 2023-04-03 11:32:12.138427 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      191 2023-04-03 11:31:52.005292 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1981 2023-04-03 11:32:12.222431 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2032 2023-04-03 11:32:12.174429 windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     4884 2023-04-03 11:32:12.250433 windmill_api-1.85.0/windmill_api/models/list_resource_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-04-03 11:32:12.246433 windmill_api-1.85.0/windmill_api/models/list_resource_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2363 2023-04-03 11:32:12.290435 windmill_api-1.85.0/windmill_api/models/list_resource_type_response_200_item.py
--rw-r--r--   0        0        0     4408 2023-04-03 11:32:12.322437 windmill_api-1.85.0/windmill_api/models/list_schedules_response_200_item.py
--rw-r--r--   0        0        0     1265 2023-04-03 11:32:12.314437 windmill_api-1.85.0/windmill_api/models/list_schedules_response_200_item_args.py
--rw-r--r--   0        0        0     1301 2023-04-03 11:32:12.342438 windmill_api-1.85.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     6768 2023-04-03 11:32:12.514448 windmill_api-1.85.0/windmill_api/models/list_scripts_response_200_item.py
--rw-r--r--   0        0        0     1291 2023-04-03 11:32:12.366439 windmill_api-1.85.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py
--rw-r--r--   0        0        0      255 2023-04-03 11:31:51.945288 windmill_api-1.85.0/windmill_api/models/list_scripts_response_200_item_kind.py
--rw-r--r--   0        0        0      213 2023-04-03 11:31:52.233304 windmill_api-1.85.0/windmill_api/models/list_scripts_response_200_item_language.py
--rw-r--r--   0        0        0     1265 2023-04-03 11:32:12.394441 windmill_api-1.85.0/windmill_api/models/list_scripts_response_200_item_schema.py
--rw-r--r--   0        0        0     2985 2023-04-03 11:32:12.446444 windmill_api-1.85.0/windmill_api/models/list_tokens_response_200_item.py
--rw-r--r--   0        0        0     2250 2023-04-03 11:32:12.482446 windmill_api-1.85.0/windmill_api/models/list_user_workspaces_response_200.py
--rw-r--r--   0        0        0     1833 2023-04-03 11:32:12.518448 windmill_api-1.85.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
--rw-r--r--   0        0        0     2896 2023-04-03 11:32:12.562451 windmill_api-1.85.0/windmill_api/models/list_users_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0      198 2023-04-03 11:31:52.961346 windmill_api-1.85.0/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
--rw-r--r--   0        0        0     4035 2023-04-03 11:32:12.590452 windmill_api-1.85.0/windmill_api/models/list_users_response_200_item.py
--rw-r--r--   0        0        0     1613 2023-04-03 11:32:12.594452 windmill_api-1.85.0/windmill_api/models/list_users_response_200_item_usage.py
--rw-r--r--   0        0        0     4608 2023-04-03 11:32:12.730460 windmill_api-1.85.0/windmill_api/models/list_variable_response_200_item.py
--rw-r--r--   0        0        0     1296 2023-04-03 11:32:12.618454 windmill_api-1.85.0/windmill_api/models/list_variable_response_200_item_extra_perms.py
--rw-r--r--   0        0        0     2693 2023-04-03 11:32:12.662456 windmill_api-1.85.0/windmill_api/models/list_workers_response_200_item.py
--rw-r--r--   0        0        0     2086 2023-04-03 11:32:12.698458 windmill_api-1.85.0/windmill_api/models/list_workspace_invites_response_200_item.py
--rw-r--r--   0        0        0     2082 2023-04-03 11:32:12.738461 windmill_api-1.85.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
--rw-r--r--   0        0        0     2013 2023-04-03 11:32:12.770462 windmill_api-1.85.0/windmill_api/models/list_workspaces_response_200_item.py
--rw-r--r--   0        0        0     3388 2023-04-03 11:32:12.794464 windmill_api-1.85.0/windmill_api/models/listable_app.py
--rw-r--r--   0        0        0      207 2023-04-03 11:31:52.533321 windmill_api-1.85.0/windmill_api/models/listable_app_execution_mode.py
--rw-r--r--   0        0        0     1207 2023-04-03 11:32:12.794464 windmill_api-1.85.0/windmill_api/models/listable_app_extra_perms.py
--rw-r--r--   0        0        0     4751 2023-04-03 11:32:12.870468 windmill_api-1.85.0/windmill_api/models/listable_resource.py
--rw-r--r--   0        0        0     1232 2023-04-03 11:32:12.818465 windmill_api-1.85.0/windmill_api/models/listable_resource_extra_perms.py
--rw-r--r--   0        0        0     4486 2023-04-03 11:32:12.894469 windmill_api-1.85.0/windmill_api/models/listable_variable.py
--rw-r--r--   0        0        0     1232 2023-04-03 11:32:12.890469 windmill_api-1.85.0/windmill_api/models/listable_variable_extra_perms.py
--rw-r--r--   0        0        0     1513 2023-04-03 11:32:12.922471 windmill_api-1.85.0/windmill_api/models/login.py
--rw-r--r--   0        0        0     1559 2023-04-03 11:32:12.926471 windmill_api-1.85.0/windmill_api/models/login_json_body.py
--rw-r--r--   0        0        0     1739 2023-04-03 11:32:13.050478 windmill_api-1.85.0/windmill_api/models/login_with_oauth_json_body.py
--rw-r--r--   0        0        0     2758 2023-04-03 11:32:12.974474 windmill_api-1.85.0/windmill_api/models/main_arg_signature.py
--rw-r--r--   0        0        0     5099 2023-04-03 11:32:13.046478 windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item.py
--rw-r--r--   0        0        0      315 2023-04-03 11:31:51.969289 windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1547 2023-04-03 11:32:13.078480 windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1612 2023-04-03 11:32:13.082480 windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2044 2023-04-03 11:32:13.110482 windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3049 2023-04-03 11:32:13.126483 windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      333 2023-04-03 11:31:52.681330 windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1580 2023-04-03 11:32:13.142483 windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     2862 2023-04-03 11:32:13.242489 windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
--rw-r--r--   0        0        0      324 2023-04-03 11:31:52.109297 windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1529 2023-04-03 11:32:13.170485 windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      169 2023-04-03 11:31:53.045350 windmill_api-1.85.0/windmill_api/models/main_arg_signature_type.py
--rw-r--r--   0        0        0     2725 2023-04-03 11:32:13.222488 windmill_api-1.85.0/windmill_api/models/new_schedule.py
--rw-r--r--   0        0        0     1171 2023-04-03 11:32:13.246489 windmill_api-1.85.0/windmill_api/models/new_schedule_args.py
--rw-r--r--   0        0        0     2108 2023-04-03 11:32:13.286491 windmill_api-1.85.0/windmill_api/models/new_token.py
--rw-r--r--   0        0        0     1710 2023-04-03 11:32:13.282491 windmill_api-1.85.0/windmill_api/models/new_user.py
--rw-r--r--   0        0        0     2584 2023-04-03 11:32:13.330494 windmill_api-1.85.0/windmill_api/models/open_flow.py
--rw-r--r--   0        0        0     1166 2023-04-03 11:32:13.310493 windmill_api-1.85.0/windmill_api/models/open_flow_schema.py
--rw-r--r--   0        0        0     3026 2023-04-03 11:32:13.362496 windmill_api-1.85.0/windmill_api/models/open_flow_value.py
--rw-r--r--   0        0        0     6384 2023-04-03 11:32:13.426499 windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module.py
--rw-r--r--   0        0        0     3013 2023-04-03 11:32:13.410498 windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_retry.py
--rw-r--r--   0        0        0     1896 2023-04-03 11:32:13.446501 windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2200 2023-04-03 11:32:13.462502 windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2006 2023-04-03 11:32:13.482503 windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      175 2023-04-03 11:31:52.505320 windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1873 2023-04-03 11:32:13.498504 windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      175 2023-04-03 11:31:52.053294 windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1889 2023-04-03 11:32:13.518505 windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1940 2023-04-03 11:32:13.530505 windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6308 2023-04-03 11:32:13.618510 windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item.py
--rw-r--r--   0        0        0     2979 2023-04-03 11:32:13.578508 windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_retry.py
--rw-r--r--   0        0        0     1886 2023-04-03 11:32:13.702515 windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2190 2023-04-03 11:32:13.654513 windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     1986 2023-04-03 11:32:13.766519 windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      173 2023-04-03 11:31:52.797336 windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1853 2023-04-03 11:32:13.742517 windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      173 2023-04-03 11:31:51.977290 windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1879 2023-04-03 11:32:13.774519 windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1930 2023-04-03 11:32:13.802521 windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-04-03 11:32:13.826522 windmill_api-1.85.0/windmill_api/models/open_flow_w_path.py
--rw-r--r--   0        0        0     1197 2023-04-03 11:32:13.830522 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_schema.py
--rw-r--r--   0        0        0     3116 2023-04-03 11:32:13.878525 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value.py
--rw-r--r--   0        0        0     6590 2023-04-03 11:32:13.926528 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module.py
--rw-r--r--   0        0        0     3117 2023-04-03 11:32:13.922528 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
--rw-r--r--   0        0        0     1927 2023-04-03 11:32:13.958530 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2231 2023-04-03 11:32:13.966530 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2073 2023-04-03 11:32:13.994532 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      180 2023-04-03 11:31:52.465318 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1940 2023-04-03 11:32:14.002532 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      180 2023-04-03 11:31:52.185302 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1920 2023-04-03 11:32:14.030534 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1971 2023-04-03 11:32:14.038534 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6514 2023-04-03 11:32:14.122539 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item.py
--rw-r--r--   0        0        0     3074 2023-04-03 11:32:14.086537 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
--rw-r--r--   0        0        0     1917 2023-04-03 11:32:14.118539 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2221 2023-04-03 11:32:14.158541 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2044 2023-04-03 11:32:14.158541 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-03 11:31:52.937344 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1911 2023-04-03 11:32:14.190543 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-03 11:31:52.389313 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1910 2023-04-03 11:32:14.194543 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1961 2023-04-03 11:32:14.306549 windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1989 2023-04-03 11:32:14.230545 windmill_api-1.85.0/windmill_api/models/path_flow.py
--rw-r--r--   0        0        0     3089 2023-04-03 11:32:14.274547 windmill_api-1.85.0/windmill_api/models/path_flow_input_transforms.py
--rw-r--r--   0        0        0     2115 2023-04-03 11:32:14.306549 windmill_api-1.85.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      185 2023-04-03 11:31:52.285308 windmill_api-1.85.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1982 2023-04-03 11:32:14.342551 windmill_api-1.85.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      185 2023-04-03 11:31:52.521321 windmill_api-1.85.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      135 2023-04-03 11:31:52.689330 windmill_api-1.85.0/windmill_api/models/path_flow_type.py
--rw-r--r--   0        0        0     2292 2023-04-03 11:32:14.426556 windmill_api-1.85.0/windmill_api/models/path_script.py
--rw-r--r--   0        0        0     3181 2023-04-03 11:32:14.386554 windmill_api-1.85.0/windmill_api/models/path_script_input_transforms.py
--rw-r--r--   0        0        0     2135 2023-04-03 11:32:14.422556 windmill_api-1.85.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      187 2023-04-03 11:31:52.353311 windmill_api-1.85.0/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     2002 2023-04-03 11:32:14.458558 windmill_api-1.85.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      187 2023-04-03 11:31:52.581324 windmill_api-1.85.0/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      141 2023-04-03 11:31:52.469318 windmill_api-1.85.0/windmill_api/models/path_script_type.py
--rw-r--r--   0        0        0     3390 2023-04-03 11:32:14.486559 windmill_api-1.85.0/windmill_api/models/policy.py
--rw-r--r--   0        0        0      202 2023-04-03 11:31:52.713332 windmill_api-1.85.0/windmill_api/models/policy_execution_mode.py
--rw-r--r--   0        0        0     1709 2023-04-03 11:32:14.490560 windmill_api-1.85.0/windmill_api/models/policy_triggerables.py
--rw-r--r--   0        0        0     1279 2023-04-03 11:32:14.510561 windmill_api-1.85.0/windmill_api/models/policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2147 2023-04-03 11:32:14.530562 windmill_api-1.85.0/windmill_api/models/preview.py
--rw-r--r--   0        0        0     1148 2023-04-03 11:32:14.534562 windmill_api-1.85.0/windmill_api/models/preview_args.py
--rw-r--r--   0        0        0      194 2023-04-03 11:31:53.049351 windmill_api-1.85.0/windmill_api/models/preview_language.py
--rw-r--r--   0        0        0     1746 2023-04-03 11:32:14.570564 windmill_api-1.85.0/windmill_api/models/preview_schedule_json_body.py
--rw-r--r--   0        0        0     2963 2023-04-03 11:32:14.586565 windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200.py
--rw-r--r--   0        0        0     5679 2023-04-03 11:32:14.646569 windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py
--rw-r--r--   0        0        0      328 2023-04-03 11:31:51.949288 windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
--rw-r--r--   0        0        0     1618 2023-04-03 11:32:14.618567 windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
--rw-r--r--   0        0        0     1683 2023-04-03 11:32:14.650569 windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
--rw-r--r--   0        0        0     2191 2023-04-03 11:32:14.682571 windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
--rw-r--r--   0        0        0     3329 2023-04-03 11:32:14.694571 windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
--rw-r--r--   0        0        0      346 2023-04-03 11:31:52.537322 windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
--rw-r--r--   0        0        0     1651 2023-04-03 11:32:14.714572 windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
--rw-r--r--   0        0        0     3214 2023-04-03 11:32:14.742574 windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
--rw-r--r--   0        0        0      337 2023-04-03 11:31:52.169301 windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
--rw-r--r--   0        0        0     1600 2023-04-03 11:32:14.746574 windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
--rw-r--r--   0        0        0      182 2023-04-03 11:31:52.877341 windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_type.py
--rw-r--r--   0        0        0    11448 2023-04-03 11:32:15.006589 windmill_api-1.85.0/windmill_api/models/queued_job.py
--rw-r--r--   0        0        0     1161 2023-04-03 11:32:14.770576 windmill_api-1.85.0/windmill_api/models/queued_job_args.py
--rw-r--r--   0        0        0     3202 2023-04-03 11:32:14.822579 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status.py
--rw-r--r--   0        0        0     6683 2023-04-03 11:32:15.022590 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_failure_module.py
--rw-r--r--   0        0        0     1774 2023-04-03 11:32:15.038591 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
--rw-r--r--   0        0        0     2106 2023-04-03 11:32:15.058592 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
--rw-r--r--   0        0        0      199 2023-04-03 11:31:52.665329 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
--rw-r--r--   0        0        0     1679 2023-04-03 11:32:15.074593 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
--rw-r--r--   0        0        0     2215 2023-04-03 11:32:15.102594 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
--rw-r--r--   0        0        0      357 2023-04-03 11:31:52.369312 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_failure_module_type.py
--rw-r--r--   0        0        0     6294 2023-04-03 11:32:15.170598 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_modules_item.py
--rw-r--r--   0        0        0     1764 2023-04-03 11:32:15.134596 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
--rw-r--r--   0        0        0     2086 2023-04-03 11:32:15.170598 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
--rw-r--r--   0        0        0      197 2023-04-03 11:31:53.049351 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
--rw-r--r--   0        0        0     1669 2023-04-03 11:32:15.202600 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
--rw-r--r--   0        0        0     2205 2023-04-03 11:32:15.214601 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
--rw-r--r--   0        0        0      355 2023-04-03 11:31:52.945345 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_modules_item_type.py
--rw-r--r--   0        0        0     2025 2023-04-03 11:32:15.242602 windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_retry.py
--rw-r--r--   0        0        0      307 2023-04-03 11:31:52.137299 windmill_api-1.85.0/windmill_api/models/queued_job_job_kind.py
--rw-r--r--   0        0        0      196 2023-04-03 11:31:52.425315 windmill_api-1.85.0/windmill_api/models/queued_job_language.py
--rw-r--r--   0        0        0     3079 2023-04-03 11:32:15.274604 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow.py
--rw-r--r--   0        0        0     6506 2023-04-03 11:32:15.442614 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module.py
--rw-r--r--   0        0        0     3069 2023-04-03 11:32:15.322607 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
--rw-r--r--   0        0        0     1914 2023-04-03 11:32:15.354609 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2218 2023-04-03 11:32:15.394611 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2040 2023-04-03 11:32:15.430613 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      178 2023-04-03 11:31:52.969346 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1907 2023-04-03 11:32:15.462615 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      178 2023-04-03 11:31:52.597325 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1907 2023-04-03 11:32:15.478616 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1958 2023-04-03 11:32:15.498617 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
--rw-r--r--   0        0        0     6430 2023-04-03 11:32:15.574621 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item.py
--rw-r--r--   0        0        0     3035 2023-04-03 11:32:15.546620 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
--rw-r--r--   0        0        0     1904 2023-04-03 11:32:15.578621 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2208 2023-04-03 11:32:15.614623 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2020 2023-04-03 11:32:15.614623 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      176 2023-04-03 11:31:52.677330 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1887 2023-04-03 11:32:15.646625 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      176 2023-04-03 11:31:52.541322 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1897 2023-04-03 11:32:15.750631 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1948 2023-04-03 11:32:15.678627 windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
--rw-r--r--   0        0        0     2816 2023-04-03 11:32:15.726630 windmill_api-1.85.0/windmill_api/models/raw_script.py
--rw-r--r--   0        0        0     3139 2023-04-03 11:32:15.770632 windmill_api-1.85.0/windmill_api/models/raw_script_input_transforms.py
--rw-r--r--   0        0        0     2125 2023-04-03 11:32:15.786633 windmill_api-1.85.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
--rw-r--r--   0        0        0      186 2023-04-03 11:31:52.205303 windmill_api-1.85.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
--rw-r--r--   0        0        0     1992 2023-04-03 11:32:15.802634 windmill_api-1.85.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
--rw-r--r--   0        0        0      186 2023-04-03 11:31:52.201303 windmill_api-1.85.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
--rw-r--r--   0        0        0      196 2023-04-03 11:31:52.125298 windmill_api-1.85.0/windmill_api/models/raw_script_language.py
--rw-r--r--   0        0        0      146 2023-04-03 11:31:52.509320 windmill_api-1.85.0/windmill_api/models/raw_script_type.py
--rw-r--r--   0        0        0     1405 2023-04-03 11:32:15.822635 windmill_api-1.85.0/windmill_api/models/refresh_token_json_body.py
--rw-r--r--   0        0        0     1448 2023-04-03 11:32:15.830636 windmill_api-1.85.0/windmill_api/models/remove_granular_acls_json_body.py
--rw-r--r--   0        0        0      304 2023-04-03 11:31:53.005348 windmill_api-1.85.0/windmill_api/models/remove_granular_acls_kind.py
--rw-r--r--   0        0        0     1544 2023-04-03 11:32:15.854637 windmill_api-1.85.0/windmill_api/models/remove_owner_to_folder_json_body.py
--rw-r--r--   0        0        0     1567 2023-04-03 11:32:15.858637 windmill_api-1.85.0/windmill_api/models/remove_user_to_group_json_body.py
--rw-r--r--   0        0        0     3367 2023-04-03 11:32:15.914640 windmill_api-1.85.0/windmill_api/models/resource.py
--rw-r--r--   0        0        0     1189 2023-04-03 11:32:15.886639 windmill_api-1.85.0/windmill_api/models/resource_extra_perms.py
--rw-r--r--   0        0        0     2256 2023-04-03 11:32:15.926641 windmill_api-1.85.0/windmill_api/models/resource_type.py
--rw-r--r--   0        0        0     1278 2023-04-03 11:32:15.942642 windmill_api-1.85.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
--rw-r--r--   0        0        0     1255 2023-04-03 11:32:16.046648 windmill_api-1.85.0/windmill_api/models/resume_suspended_job_post_json_body.py
--rw-r--r--   0        0        0     2546 2023-04-03 11:32:15.990645 windmill_api-1.85.0/windmill_api/models/retry.py
--rw-r--r--   0        0        0     1751 2023-04-03 11:32:16.022647 windmill_api-1.85.0/windmill_api/models/retry_constant.py
--rw-r--r--   0        0        0     2055 2023-04-03 11:32:16.066649 windmill_api-1.85.0/windmill_api/models/retry_exponential.py
--rw-r--r--   0        0        0     1210 2023-04-03 11:32:16.074649 windmill_api-1.85.0/windmill_api/models/run_flow_by_path_json_body.py
--rw-r--r--   0        0        0     2189 2023-04-03 11:32:16.106651 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body.py
--rw-r--r--   0        0        0     1235 2023-04-03 11:32:16.094651 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_args.py
--rw-r--r--   0        0        0     3265 2023-04-03 11:32:16.146654 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value.py
--rw-r--r--   0        0        0     7049 2023-04-03 11:32:16.206657 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3284 2023-04-03 11:32:16.194656 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1975 2023-04-03 11:32:16.230658 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2279 2023-04-03 11:32:16.242659 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2167 2023-04-03 11:32:16.266660 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      189 2023-04-03 11:31:52.205303 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     2034 2023-04-03 11:32:16.278661 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      189 2023-04-03 11:31:52.537322 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1968 2023-04-03 11:32:16.302662 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     2019 2023-04-03 11:32:16.314663 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6939 2023-04-03 11:32:16.398668 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3250 2023-04-03 11:32:16.466672 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1965 2023-04-03 11:32:16.434670 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2269 2023-04-03 11:32:16.470672 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2147 2023-04-03 11:32:16.498673 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      187 2023-04-03 11:31:52.905342 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     2014 2023-04-03 11:32:16.506674 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      187 2023-04-03 11:31:52.617326 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1958 2023-04-03 11:32:16.534675 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     2009 2023-04-03 11:32:16.542676 windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1220 2023-04-03 11:32:16.558677 windmill_api-1.85.0/windmill_api/models/run_script_by_hash_json_body.py
--rw-r--r--   0        0        0     1220 2023-04-03 11:32:16.566677 windmill_api-1.85.0/windmill_api/models/run_script_by_path_json_body.py
--rw-r--r--   0        0        0     2422 2023-04-03 11:32:16.602679 windmill_api-1.85.0/windmill_api/models/run_script_preview_json_body.py
--rw-r--r--   0        0        0     1245 2023-04-03 11:32:16.590679 windmill_api-1.85.0/windmill_api/models/run_script_preview_json_body_args.py
--rw-r--r--   0        0        0      211 2023-04-03 11:31:52.973346 windmill_api-1.85.0/windmill_api/models/run_script_preview_json_body_language.py
--rw-r--r--   0        0        0     1266 2023-04-03 11:32:16.710685 windmill_api-1.85.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py
--rw-r--r--   0        0        0     1276 2023-04-03 11:32:16.626681 windmill_api-1.85.0/windmill_api/models/run_wait_result_script_by_path_json_body.py
--rw-r--r--   0        0        0     4068 2023-04-03 11:32:16.694685 windmill_api-1.85.0/windmill_api/models/schedule.py
--rw-r--r--   0        0        0     1153 2023-04-03 11:32:16.718686 windmill_api-1.85.0/windmill_api/models/schedule_args.py
--rw-r--r--   0        0        0     1189 2023-04-03 11:32:16.734687 windmill_api-1.85.0/windmill_api/models/schedule_extra_perms.py
--rw-r--r--   0        0        0     6220 2023-04-03 11:32:16.814691 windmill_api-1.85.0/windmill_api/models/script.py
--rw-r--r--   0        0        0     1143 2023-04-03 11:32:16.758688 windmill_api-1.85.0/windmill_api/models/script_args.py
--rw-r--r--   0        0        0     1179 2023-04-03 11:32:16.782689 windmill_api-1.85.0/windmill_api/models/script_extra_perms.py
--rw-r--r--   0        0        0      235 2023-04-03 11:31:52.217304 windmill_api-1.85.0/windmill_api/models/script_kind.py
--rw-r--r--   0        0        0      193 2023-04-03 11:31:53.093353 windmill_api-1.85.0/windmill_api/models/script_language.py
--rw-r--r--   0        0        0     1153 2023-04-03 11:32:16.810691 windmill_api-1.85.0/windmill_api/models/script_schema.py
--rw-r--r--   0        0        0     1440 2023-04-03 11:32:16.838693 windmill_api-1.85.0/windmill_api/models/set_password_json_body.py
--rw-r--r--   0        0        0     1470 2023-04-03 11:32:16.842693 windmill_api-1.85.0/windmill_api/models/set_schedule_enabled_json_body.py
--rw-r--r--   0        0        0     2032 2023-04-03 11:32:16.878695 windmill_api-1.85.0/windmill_api/models/slack_token.py
--rw-r--r--   0        0        0     1586 2023-04-03 11:32:16.870694 windmill_api-1.85.0/windmill_api/models/slack_token_bot.py
--rw-r--r--   0        0        0     2227 2023-04-03 11:32:17.014703 windmill_api-1.85.0/windmill_api/models/star_json_body.py
--rw-r--r--   0        0        0      185 2023-04-03 11:31:53.133355 windmill_api-1.85.0/windmill_api/models/star_json_body_favorite_kind.py
--rw-r--r--   0        0        0     1772 2023-04-03 11:32:16.918697 windmill_api-1.85.0/windmill_api/models/static_transform.py
--rw-r--r--   0        0        0      154 2023-04-03 11:31:52.789336 windmill_api-1.85.0/windmill_api/models/static_transform_type.py
--rw-r--r--   0        0        0     2462 2023-04-03 11:32:16.962700 windmill_api-1.85.0/windmill_api/models/token_response.py
--rw-r--r--   0        0        0     2921 2023-04-03 11:32:17.014703 windmill_api-1.85.0/windmill_api/models/truncated_token.py
--rw-r--r--   0        0        0     2249 2023-04-03 11:32:17.054705 windmill_api-1.85.0/windmill_api/models/unstar_json_body.py
--rw-r--r--   0        0        0      187 2023-04-03 11:31:51.929287 windmill_api-1.85.0/windmill_api/models/unstar_json_body_favorite_kind.py
--rw-r--r--   0        0        0     2638 2023-04-03 11:32:17.066706 windmill_api-1.85.0/windmill_api/models/update_app_json_body.py
--rw-r--r--   0        0        0     3699 2023-04-03 11:32:17.110708 windmill_api-1.85.0/windmill_api/models/update_app_json_body_policy.py
--rw-r--r--   0        0        0      219 2023-04-03 11:31:52.285308 windmill_api-1.85.0/windmill_api/models/update_app_json_body_policy_execution_mode.py
--rw-r--r--   0        0        0     1935 2023-04-03 11:32:17.098707 windmill_api-1.85.0/windmill_api/models/update_app_json_body_policy_triggerables.py
--rw-r--r--   0        0        0     1376 2023-04-03 11:32:17.126709 windmill_api-1.85.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
--rw-r--r--   0        0        0     2896 2023-04-03 11:32:17.158711 windmill_api-1.85.0/windmill_api/models/update_flow_json_body.py
--rw-r--r--   0        0        0     1222 2023-04-03 11:32:17.150710 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_schema.py
--rw-r--r--   0        0        0     3196 2023-04-03 11:32:17.202713 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value.py
--rw-r--r--   0        0        0     6855 2023-04-03 11:32:17.254716 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module.py
--rw-r--r--   0        0        0     3211 2023-04-03 11:32:17.250716 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
--rw-r--r--   0        0        0     1952 2023-04-03 11:32:17.282718 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
--rw-r--r--   0        0        0     2256 2023-04-03 11:32:17.394724 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
--rw-r--r--   0        0        0     2123 2023-04-03 11:32:17.318720 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
--rw-r--r--   0        0        0      185 2023-04-03 11:31:52.577324 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
--rw-r--r--   0        0        0     1990 2023-04-03 11:32:17.354722 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
--rw-r--r--   0        0        0      185 2023-04-03 11:31:53.037350 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
--rw-r--r--   0        0        0     1945 2023-04-03 11:32:17.390724 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
--rw-r--r--   0        0        0     1996 2023-04-03 11:32:17.426726 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
--rw-r--r--   0        0        0     6739 2023-04-03 11:32:17.490730 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item.py
--rw-r--r--   0        0        0     3177 2023-04-03 11:32:17.474729 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
--rw-r--r--   0        0        0     1942 2023-04-03 11:32:17.510731 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
--rw-r--r--   0        0        0     2246 2023-04-03 11:32:17.530732 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
--rw-r--r--   0        0        0     2103 2023-04-03 11:32:17.546733 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
--rw-r--r--   0        0        0      183 2023-04-03 11:31:52.477318 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
--rw-r--r--   0        0        0     1970 2023-04-03 11:32:17.566734 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
--rw-r--r--   0        0        0      183 2023-04-03 11:31:52.169301 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
--rw-r--r--   0        0        0     1935 2023-04-03 11:32:17.582735 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
--rw-r--r--   0        0        0     1986 2023-04-03 11:32:17.598736 windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
--rw-r--r--   0        0        0     1949 2023-04-03 11:32:17.622737 windmill_api-1.85.0/windmill_api/models/update_folder_json_body.py
--rw-r--r--   0        0        0     1520 2023-04-03 11:32:17.630737 windmill_api-1.85.0/windmill_api/models/update_group_json_body.py
--rw-r--r--   0        0        0     2036 2023-04-03 11:32:17.662739 windmill_api-1.85.0/windmill_api/models/update_resource_json_body.py
--rw-r--r--   0        0        0     1847 2023-04-03 11:32:17.666740 windmill_api-1.85.0/windmill_api/models/update_resource_type_json_body.py
--rw-r--r--   0        0        0     1541 2023-04-03 11:32:17.694741 windmill_api-1.85.0/windmill_api/models/update_resource_value_json_body.py
--rw-r--r--   0        0        0     1771 2023-04-03 11:32:17.698741 windmill_api-1.85.0/windmill_api/models/update_schedule_json_body.py
--rw-r--r--   0        0        0     1232 2023-04-03 11:32:17.718742 windmill_api-1.85.0/windmill_api/models/update_schedule_json_body_args.py
--rw-r--r--   0        0        0     2066 2023-04-03 11:32:17.738744 windmill_api-1.85.0/windmill_api/models/update_user_json_body.py
--rw-r--r--   0        0        0     2316 2023-04-03 11:32:17.762745 windmill_api-1.85.0/windmill_api/models/update_variable_json_body.py
--rw-r--r--   0        0        0     1478 2023-04-03 11:32:17.766745 windmill_api-1.85.0/windmill_api/models/usage.py
--rw-r--r--   0        0        0     3799 2023-04-03 11:32:17.834749 windmill_api-1.85.0/windmill_api/models/user.py
--rw-r--r--   0        0        0     1501 2023-04-03 11:32:17.798747 windmill_api-1.85.0/windmill_api/models/user_usage.py
--rw-r--r--   0        0        0     2122 2023-04-03 11:32:17.834749 windmill_api-1.85.0/windmill_api/models/user_workspace_list.py
--rw-r--r--   0        0        0     1767 2023-04-03 11:32:17.870751 windmill_api-1.85.0/windmill_api/models/user_workspace_list_workspaces_item.py
--rw-r--r--   0        0        0     3950 2023-04-03 11:32:17.906753 windmill_api-1.85.0/windmill_api/models/whoami_response_200.py
--rw-r--r--   0        0        0     1572 2023-04-03 11:32:17.902753 windmill_api-1.85.0/windmill_api/models/whoami_response_200_usage.py
--rw-r--r--   0        0        0     3939 2023-04-03 11:32:18.078763 windmill_api-1.85.0/windmill_api/models/whois_response_200.py
--rw-r--r--   0        0        0     1567 2023-04-03 11:32:17.934755 windmill_api-1.85.0/windmill_api/models/whois_response_200_usage.py
--rw-r--r--   0        0        0     2604 2023-04-03 11:32:18.094764 windmill_api-1.85.0/windmill_api/models/worker_ping.py
--rw-r--r--   0        0        0     1901 2023-04-03 11:32:18.118765 windmill_api-1.85.0/windmill_api/models/workspace.py
--rw-r--r--   0        0        0     1974 2023-04-03 11:32:18.130766 windmill_api-1.85.0/windmill_api/models/workspace_invite.py
--rw-r--r--   0        0        0       25 2023-04-03 11:31:41.552699 windmill_api-1.85.0/windmill_api/py.typed
--rw-r--r--   0        0        0      939 2023-04-03 11:32:18.138766 windmill_api-1.85.0/windmill_api/types.py
--rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 windmill_api-1.85.0/setup.py
--rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.85.0/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-04-08 20:03:14.828319 windmill_api-1.86.0/LICENSE
+-rw-r--r--   0        0        0     2952 2023-04-08 20:03:14.832320 windmill_api-1.86.0/README.md
+-rw-r--r--   0        0        0      717 2023-04-08 20:03:14.828319 windmill_api-1.86.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-04-08 20:02:44.203774 windmill_api-1.86.0/windmill_api/__init__.py
+-rw-r--r--   0        0        0       47 2023-04-08 20:02:44.679783 windmill_api-1.86.0/windmill_api/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.783784 windmill_api-1.86.0/windmill_api/api/app/__init__.py
+-rw-r--r--   0        0        0     1999 2023-04-08 20:02:54.755963 windmill_api-1.86.0/windmill_api/api/app/create_app.py
+-rw-r--r--   0        0        0     1769 2023-04-08 20:02:54.747963 windmill_api-1.86.0/windmill_api/api/app/delete_app.py
+-rw-r--r--   0        0        0     2214 2023-04-08 20:02:54.779964 windmill_api-1.86.0/windmill_api/api/app/execute_component.py
+-rw-r--r--   0        0        0     2782 2023-04-08 20:02:54.807964 windmill_api-1.86.0/windmill_api/api/app/exists_app.py
+-rw-r--r--   0        0        0     3020 2023-04-08 20:02:54.819965 windmill_api-1.86.0/windmill_api/api/app/get_app_by_path.py
+-rw-r--r--   0        0        0     3031 2023-04-08 20:02:54.847965 windmill_api-1.86.0/windmill_api/api/app/get_app_by_version.py
+-rw-r--r--   0        0        0     2649 2023-04-08 20:02:54.855965 windmill_api-1.86.0/windmill_api/api/app/get_hub_app_by_id.py
+-rw-r--r--   0        0        0     3168 2023-04-08 20:02:54.903966 windmill_api-1.86.0/windmill_api/api/app/get_public_app_by_secret.py
+-rw-r--r--   0        0        0     1797 2023-04-08 20:02:54.891966 windmill_api-1.86.0/windmill_api/api/app/get_public_secret_of_app.py
+-rw-r--r--   0        0        0     7289 2023-04-08 20:02:54.983968 windmill_api-1.86.0/windmill_api/api/app/list_apps.py
+-rw-r--r--   0        0        0     2405 2023-04-08 20:02:54.935967 windmill_api-1.86.0/windmill_api/api/app/list_hub_apps.py
+-rw-r--r--   0        0        0     2140 2023-04-08 20:02:54.963967 windmill_api-1.86.0/windmill_api/api/app/update_app.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.719783 windmill_api-1.86.0/windmill_api/api/audit/__init__.py
+-rw-r--r--   0        0        0     3065 2023-04-08 20:02:55.003968 windmill_api-1.86.0/windmill_api/api/audit/get_audit_log.py
+-rw-r--r--   0        0        0     8723 2023-04-08 20:02:55.095970 windmill_api-1.86.0/windmill_api/api/audit/list_audit_logs.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.835785 windmill_api-1.86.0/windmill_api/api/capture/__init__.py
+-rw-r--r--   0        0        0     1796 2023-04-08 20:02:55.027968 windmill_api-1.86.0/windmill_api/api/capture/create_capture.py
+-rw-r--r--   0        0        0     1790 2023-04-08 20:02:55.055969 windmill_api-1.86.0/windmill_api/api/capture/get_capture.py
+-rw-r--r--   0        0        0     1799 2023-04-08 20:02:55.083969 windmill_api-1.86.0/windmill_api/api/capture/update_capture.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.835785 windmill_api-1.86.0/windmill_api/api/favorite/__init__.py
+-rw-r--r--   0        0        0     1964 2023-04-08 20:02:55.115970 windmill_api-1.86.0/windmill_api/api/favorite/star.py
+-rw-r--r--   0        0        0     1984 2023-04-08 20:02:55.119970 windmill_api-1.86.0/windmill_api/api/favorite/unstar.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.775784 windmill_api-1.86.0/windmill_api/api/flow/__init__.py
+-rw-r--r--   0        0        0     1789 2023-04-08 20:02:55.147971 windmill_api-1.86.0/windmill_api/api/flow/archive_flow_by_path.py
+-rw-r--r--   0        0        0     2009 2023-04-08 20:02:55.147971 windmill_api-1.86.0/windmill_api/api/flow/create_flow.py
+-rw-r--r--   0        0        0     1788 2023-04-08 20:02:55.175971 windmill_api-1.86.0/windmill_api/api/flow/delete_flow_by_path.py
+-rw-r--r--   0        0        0     2755 2023-04-08 20:02:55.183971 windmill_api-1.86.0/windmill_api/api/flow/exists_flow_by_path.py
+-rw-r--r--   0        0        0     3036 2023-04-08 20:02:55.215972 windmill_api-1.86.0/windmill_api/api/flow/get_flow_by_path.py
+-rw-r--r--   0        0        0     2667 2023-04-08 20:02:55.243972 windmill_api-1.86.0/windmill_api/api/flow/get_hub_flow_by_id.py
+-rw-r--r--   0        0        0     1668 2023-04-08 20:02:55.259972 windmill_api-1.86.0/windmill_api/api/flow/list_flow_paths.py
+-rw-r--r--   0        0        0     7969 2023-04-08 20:02:55.335974 windmill_api-1.86.0/windmill_api/api/flow/list_flows.py
+-rw-r--r--   0        0        0     2423 2023-04-08 20:02:55.291973 windmill_api-1.86.0/windmill_api/api/flow/list_hub_flows.py
+-rw-r--r--   0        0        0     2150 2023-04-08 20:02:55.319974 windmill_api-1.86.0/windmill_api/api/flow/update_flow.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.827785 windmill_api-1.86.0/windmill_api/api/folder/__init__.py
+-rw-r--r--   0        0        0     2214 2023-04-08 20:02:55.355974 windmill_api-1.86.0/windmill_api/api/folder/add_owner_to_folder.py
+-rw-r--r--   0        0        0     2029 2023-04-08 20:02:55.359974 windmill_api-1.86.0/windmill_api/api/folder/create_folder.py
+-rw-r--r--   0        0        0     1778 2023-04-08 20:02:55.383975 windmill_api-1.86.0/windmill_api/api/folder/delete_folder.py
+-rw-r--r--   0        0        0     2960 2023-04-08 20:02:55.399975 windmill_api-1.86.0/windmill_api/api/folder/get_folder.py
+-rw-r--r--   0        0        0     3055 2023-04-08 20:02:55.423975 windmill_api-1.86.0/windmill_api/api/folder/get_folder_usage.py
+-rw-r--r--   0        0        0     3405 2023-04-08 20:02:55.443976 windmill_api-1.86.0/windmill_api/api/folder/list_folder_names.py
+-rw-r--r--   0        0        0     4251 2023-04-08 20:02:55.479976 windmill_api-1.86.0/windmill_api/api/folder/list_folders.py
+-rw-r--r--   0        0        0     2244 2023-04-08 20:02:55.471976 windmill_api-1.86.0/windmill_api/api/folder/remove_owner_to_folder.py
+-rw-r--r--   0        0        0     2170 2023-04-08 20:02:55.499977 windmill_api-1.86.0/windmill_api/api/folder/update_folder.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.831786 windmill_api-1.86.0/windmill_api/api/granular_acl/__init__.py
+-rw-r--r--   0        0        0     2480 2023-04-08 20:02:55.527977 windmill_api-1.86.0/windmill_api/api/granular_acl/add_granular_acls.py
+-rw-r--r--   0        0        0     3526 2023-04-08 20:02:55.579978 windmill_api-1.86.0/windmill_api/api/granular_acl/get_granular_acls.py
+-rw-r--r--   0        0        0     2545 2023-04-08 20:02:55.559978 windmill_api-1.86.0/windmill_api/api/granular_acl/remove_granular_acls.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.819785 windmill_api-1.86.0/windmill_api/api/group/__init__.py
+-rw-r--r--   0        0        0     2194 2023-04-08 20:02:55.611979 windmill_api-1.86.0/windmill_api/api/group/add_user_to_group.py
+-rw-r--r--   0        0        0     2019 2023-04-08 20:02:55.607979 windmill_api-1.86.0/windmill_api/api/group/create_group.py
+-rw-r--r--   0        0        0     1775 2023-04-08 20:02:55.631979 windmill_api-1.86.0/windmill_api/api/group/delete_group.py
+-rw-r--r--   0        0        0     2942 2023-04-08 20:02:55.651979 windmill_api-1.86.0/windmill_api/api/group/get_group.py
+-rw-r--r--   0        0        0     3400 2023-04-08 20:02:55.679980 windmill_api-1.86.0/windmill_api/api/group/list_group_names.py
+-rw-r--r--   0        0        0     4233 2023-04-08 20:02:55.707980 windmill_api-1.86.0/windmill_api/api/group/list_groups.py
+-rw-r--r--   0        0        0     2224 2023-04-08 20:02:55.707980 windmill_api-1.86.0/windmill_api/api/group/remove_user_to_group.py
+-rw-r--r--   0        0        0     2160 2023-04-08 20:02:55.735981 windmill_api-1.86.0/windmill_api/api/group/update_group.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.791785 windmill_api-1.86.0/windmill_api/api/job/__init__.py
+-rw-r--r--   0        0        0     2181 2023-04-08 20:02:55.743981 windmill_api-1.86.0/windmill_api/api/job/cancel_queued_job.py
+-rw-r--r--   0        0        0     2687 2023-04-08 20:02:55.775982 windmill_api-1.86.0/windmill_api/api/job/cancel_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-04-08 20:02:55.795982 windmill_api-1.86.0/windmill_api/api/job/cancel_suspended_job_post.py
+-rw-r--r--   0        0        0     2535 2023-04-08 20:02:55.807982 windmill_api-1.86.0/windmill_api/api/job/create_job_signature.py
+-rw-r--r--   0        0        0     3217 2023-04-08 20:02:55.835983 windmill_api-1.86.0/windmill_api/api/job/delete_completed_job.py
+-rw-r--r--   0        0        0     2235 2023-04-08 20:02:55.835983 windmill_api-1.86.0/windmill_api/api/job/force_cancel_queued_job.py
+-rw-r--r--   0        0        0     3034 2023-04-08 20:02:55.875983 windmill_api-1.86.0/windmill_api/api/job/get_completed_job.py
+-rw-r--r--   0        0        0     1784 2023-04-08 20:02:55.863983 windmill_api-1.86.0/windmill_api/api/job/get_completed_job_result.py
+-rw-r--r--   0        0        0     2868 2023-04-08 20:02:55.915984 windmill_api-1.86.0/windmill_api/api/job/get_job.py
+-rw-r--r--   0        0        0     4305 2023-04-08 20:02:55.931984 windmill_api-1.86.0/windmill_api/api/job/get_job_updates.py
+-rw-r--r--   0        0        0     4306 2023-04-08 20:02:55.963985 windmill_api-1.86.0/windmill_api/api/job/get_resume_urls.py
+-rw-r--r--   0        0        0     4601 2023-04-08 20:02:56.007986 windmill_api-1.86.0/windmill_api/api/job/get_suspended_job_flow.py
+-rw-r--r--   0        0        0    12602 2023-04-08 20:02:56.099987 windmill_api-1.86.0/windmill_api/api/job/list_completed_jobs.py
+-rw-r--r--   0        0        0    11829 2023-04-08 20:02:56.139988 windmill_api-1.86.0/windmill_api/api/job/list_jobs.py
+-rw-r--r--   0        0        0    12367 2023-04-08 20:02:56.263990 windmill_api-1.86.0/windmill_api/api/job/list_queue.py
+-rw-r--r--   0        0        0     2067 2023-04-08 20:02:56.171989 windmill_api-1.86.0/windmill_api/api/job/result_by_id.py
+-rw-r--r--   0        0        0     2313 2023-04-08 20:02:56.199989 windmill_api-1.86.0/windmill_api/api/job/resume_suspended_flow_as_owner.py
+-rw-r--r--   0        0        0     2994 2023-04-08 20:02:56.243990 windmill_api-1.86.0/windmill_api/api/job/resume_suspended_job_get.py
+-rw-r--r--   0        0        0     3154 2023-04-08 20:02:56.287991 windmill_api-1.86.0/windmill_api/api/job/resume_suspended_job_post.py
+-rw-r--r--   0        0        0     4566 2023-04-08 20:02:56.319991 windmill_api-1.86.0/windmill_api/api/job/run_flow_by_path.py
+-rw-r--r--   0        0        0     3037 2023-04-08 20:02:56.351992 windmill_api-1.86.0/windmill_api/api/job/run_flow_preview.py
+-rw-r--r--   0        0        0     4594 2023-04-08 20:02:56.371992 windmill_api-1.86.0/windmill_api/api/job/run_script_by_hash.py
+-rw-r--r--   0        0        0     4200 2023-04-08 20:02:56.407993 windmill_api-1.86.0/windmill_api/api/job/run_script_by_path.py
+-rw-r--r--   0        0        0     3050 2023-04-08 20:02:56.407993 windmill_api-1.86.0/windmill_api/api/job/run_script_preview.py
+-rw-r--r--   0        0        0     3215 2023-04-08 20:02:56.447993 windmill_api-1.86.0/windmill_api/api/job/run_wait_result_flow_by_path.py
+-rw-r--r--   0        0        0     3521 2023-04-08 20:02:56.451994 windmill_api-1.86.0/windmill_api/api/job/run_wait_result_script_by_path.py
+-rw-r--r--   0        0        0     3356 2023-04-08 20:02:56.499994 windmill_api-1.86.0/windmill_api/api/job/run_wait_result_script_by_path_get.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.747784 windmill_api-1.86.0/windmill_api/api/oauth/__init__.py
+-rw-r--r--   0        0        0     3506 2023-04-08 20:02:56.491994 windmill_api-1.86.0/windmill_api/api/oauth/connect_callback.py
+-rw-r--r--   0        0        0     2118 2023-04-08 20:02:56.519995 windmill_api-1.86.0/windmill_api/api/oauth/connect_slack_callback.py
+-rw-r--r--   0        0        0     2056 2023-04-08 20:02:56.527995 windmill_api-1.86.0/windmill_api/api/oauth/create_account.py
+-rw-r--r--   0        0        0     1764 2023-04-08 20:02:56.543995 windmill_api-1.86.0/windmill_api/api/oauth/disconnect_account.py
+-rw-r--r--   0        0        0     1649 2023-04-08 20:02:56.555995 windmill_api-1.86.0/windmill_api/api/oauth/disconnect_slack.py
+-rw-r--r--   0        0        0     1426 2023-04-08 20:02:56.567996 windmill_api-1.86.0/windmill_api/api/oauth/list_o_auth_connects.py
+-rw-r--r--   0        0        0     2162 2023-04-08 20:02:56.591996 windmill_api-1.86.0/windmill_api/api/oauth/list_o_auth_logins.py
+-rw-r--r--   0        0        0     2151 2023-04-08 20:02:56.615996 windmill_api-1.86.0/windmill_api/api/oauth/refresh_token.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.755784 windmill_api-1.86.0/windmill_api/api/resource/__init__.py
+-rw-r--r--   0        0        0     2049 2023-04-08 20:02:56.623997 windmill_api-1.86.0/windmill_api/api/resource/create_resource.py
+-rw-r--r--   0        0        0     2093 2023-04-08 20:02:56.639997 windmill_api-1.86.0/windmill_api/api/resource/create_resource_type.py
+-rw-r--r--   0        0        0     1784 2023-04-08 20:02:56.651997 windmill_api-1.86.0/windmill_api/api/resource/delete_resource.py
+-rw-r--r--   0        0        0     1799 2023-04-08 20:02:56.667997 windmill_api-1.86.0/windmill_api/api/resource/delete_resource_type.py
+-rw-r--r--   0        0        0     2763 2023-04-08 20:02:56.707998 windmill_api-1.86.0/windmill_api/api/resource/exists_resource.py
+-rw-r--r--   0        0        0     2788 2023-04-08 20:02:56.707998 windmill_api-1.86.0/windmill_api/api/resource/exists_resource_type.py
+-rw-r--r--   0        0        0     2996 2023-04-08 20:02:56.747999 windmill_api-1.86.0/windmill_api/api/resource/get_resource.py
+-rw-r--r--   0        0        0     3074 2023-04-08 20:02:56.743999 windmill_api-1.86.0/windmill_api/api/resource/get_resource_type.py
+-rw-r--r--   0        0        0     1790 2023-04-08 20:02:56.771999 windmill_api-1.86.0/windmill_api/api/resource/get_resource_value.py
+-rw-r--r--   0        0        0     5732 2023-04-08 20:02:56.816000 windmill_api-1.86.0/windmill_api/api/resource/list_resource.py
+-rw-r--r--   0        0        0     3149 2023-04-08 20:02:56.812000 windmill_api-1.86.0/windmill_api/api/resource/list_resource_type.py
+-rw-r--r--   0        0        0     2600 2023-04-08 20:02:56.848001 windmill_api-1.86.0/windmill_api/api/resource/list_resource_type_names.py
+-rw-r--r--   0        0        0     2190 2023-04-08 20:02:56.848001 windmill_api-1.86.0/windmill_api/api/resource/update_resource.py
+-rw-r--r--   0        0        0     2234 2023-04-08 20:02:56.876001 windmill_api-1.86.0/windmill_api/api/resource/update_resource_type.py
+-rw-r--r--   0        0        0     2244 2023-04-08 20:02:56.880001 windmill_api-1.86.0/windmill_api/api/resource/update_resource_value.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.815785 windmill_api-1.86.0/windmill_api/api/schedule/__init__.py
+-rw-r--r--   0        0        0     2049 2023-04-08 20:02:56.908002 windmill_api-1.86.0/windmill_api/api/schedule/create_schedule.py
+-rw-r--r--   0        0        0     1784 2023-04-08 20:02:56.904002 windmill_api-1.86.0/windmill_api/api/schedule/delete_schedule.py
+-rw-r--r--   0        0        0     2763 2023-04-08 20:02:56.944002 windmill_api-1.86.0/windmill_api/api/schedule/exists_schedule.py
+-rw-r--r--   0        0        0     2996 2023-04-08 20:02:56.964003 windmill_api-1.86.0/windmill_api/api/schedule/get_schedule.py
+-rw-r--r--   0        0        0     4287 2023-04-08 20:02:57.000003 windmill_api-1.86.0/windmill_api/api/schedule/list_schedules.py
+-rw-r--r--   0        0        0     3217 2023-04-08 20:02:57.008003 windmill_api-1.86.0/windmill_api/api/schedule/preview_schedule.py
+-rw-r--r--   0        0        0     2233 2023-04-08 20:02:57.048004 windmill_api-1.86.0/windmill_api/api/schedule/set_schedule_enabled.py
+-rw-r--r--   0        0        0     2190 2023-04-08 20:02:57.036004 windmill_api-1.86.0/windmill_api/api/schedule/update_schedule.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.763784 windmill_api-1.86.0/windmill_api/api/script/__init__.py
+-rw-r--r--   0        0        0     3165 2023-04-08 20:02:57.080005 windmill_api-1.86.0/windmill_api/api/script/archive_script_by_hash.py
+-rw-r--r--   0        0        0     1797 2023-04-08 20:02:57.072005 windmill_api-1.86.0/windmill_api/api/script/archive_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-04-08 20:02:57.112005 windmill_api-1.86.0/windmill_api/api/script/bash_to_jsonschema.py
+-rw-r--r--   0        0        0     2029 2023-04-08 20:02:57.108005 windmill_api-1.86.0/windmill_api/api/script/create_script.py
+-rw-r--r--   0        0        0     3327 2023-04-08 20:02:57.152006 windmill_api-1.86.0/windmill_api/api/script/delete_script_by_hash.py
+-rw-r--r--   0        0        0     2873 2023-04-08 20:02:57.148006 windmill_api-1.86.0/windmill_api/api/script/delete_script_by_path.py
+-rw-r--r--   0        0        0     3003 2023-04-08 20:02:57.184007 windmill_api-1.86.0/windmill_api/api/script/deno_to_jsonschema.py
+-rw-r--r--   0        0        0     2767 2023-04-08 20:02:57.200007 windmill_api-1.86.0/windmill_api/api/script/exists_script_by_path.py
+-rw-r--r--   0        0        0     2802 2023-04-08 20:02:57.224007 windmill_api-1.86.0/windmill_api/api/script/get_hub_script_by_path.py
+-rw-r--r--   0        0        0     1607 2023-04-08 20:02:57.228007 windmill_api-1.86.0/windmill_api/api/script/get_hub_script_content_by_path.py
+-rw-r--r--   0        0        0     3092 2023-04-08 20:02:57.264008 windmill_api-1.86.0/windmill_api/api/script/get_script_by_hash.py
+-rw-r--r--   0        0        0     3074 2023-04-08 20:02:57.288008 windmill_api-1.86.0/windmill_api/api/script/get_script_by_path.py
+-rw-r--r--   0        0        0     3276 2023-04-08 20:02:57.304009 windmill_api-1.86.0/windmill_api/api/script/get_script_deployment_status.py
+-rw-r--r--   0        0        0     2967 2023-04-08 20:02:57.324009 windmill_api-1.86.0/windmill_api/api/script/go_to_jsonschema.py
+-rw-r--r--   0        0        0     2459 2023-04-08 20:02:57.352009 windmill_api-1.86.0/windmill_api/api/script/list_hub_scripts.py
+-rw-r--r--   0        0        0     1676 2023-04-08 20:02:57.348009 windmill_api-1.86.0/windmill_api/api/script/list_script_paths.py
+-rw-r--r--   0        0        0    11165 2023-04-08 20:02:57.476012 windmill_api-1.86.0/windmill_api/api/script/list_scripts.py
+-rw-r--r--   0        0        0     3039 2023-04-08 20:02:57.388010 windmill_api-1.86.0/windmill_api/api/script/python_to_jsonschema.py
+-rw-r--r--   0        0        0     1784 2023-04-08 20:02:57.412011 windmill_api-1.86.0/windmill_api/api/script/raw_script_by_hash.py
+-rw-r--r--   0        0        0     1784 2023-04-08 20:02:57.440011 windmill_api-1.86.0/windmill_api/api/script/raw_script_by_path.py
+-rw-r--r--   0        0        0     2119 2023-04-08 20:02:57.468011 windmill_api-1.86.0/windmill_api/api/script/raw_script_by_path_tokened.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.691783 windmill_api-1.86.0/windmill_api/api/settings/__init__.py
+-rw-r--r--   0        0        0     1414 2023-04-08 20:02:57.492012 windmill_api-1.86.0/windmill_api/api/settings/backend_version.py
+-rw-r--r--   0        0        0     1423 2023-04-08 20:02:57.504012 windmill_api-1.86.0/windmill_api/api/settings/get_open_api_yaml.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.719783 windmill_api-1.86.0/windmill_api/api/user/__init__.py
+-rw-r--r--   0        0        0     1857 2023-04-08 20:02:57.516013 windmill_api-1.86.0/windmill_api/api/user/accept_invite.py
+-rw-r--r--   0        0        0     1822 2023-04-08 20:02:57.532013 windmill_api-1.86.0/windmill_api/api/user/create_token.py
+-rw-r--r--   0        0        0     1991 2023-04-08 20:02:57.544013 windmill_api-1.86.0/windmill_api/api/user/create_token_impersonate.py
+-rw-r--r--   0        0        0     2058 2023-04-08 20:02:57.560013 windmill_api-1.86.0/windmill_api/api/user/create_user.py
+-rw-r--r--   0        0        0     1863 2023-04-08 20:02:57.568013 windmill_api-1.86.0/windmill_api/api/user/create_user_globally.py
+-rw-r--r--   0        0        0     1867 2023-04-08 20:02:57.584014 windmill_api-1.86.0/windmill_api/api/user/decline_invite.py
+-rw-r--r--   0        0        0     1674 2023-04-08 20:02:57.596014 windmill_api-1.86.0/windmill_api/api/user/delete_token.py
+-rw-r--r--   0        0        0     1872 2023-04-08 20:02:57.612014 windmill_api-1.86.0/windmill_api/api/user/delete_user.py
+-rw-r--r--   0        0        0     1454 2023-04-08 20:02:57.616014 windmill_api-1.86.0/windmill_api/api/user/get_current_email.py
+-rw-r--r--   0        0        0     1474 2023-04-08 20:02:57.660015 windmill_api-1.86.0/windmill_api/api/user/get_usage.py
+-rw-r--r--   0        0        0     1639 2023-04-08 20:02:57.644015 windmill_api-1.86.0/windmill_api/api/user/global_user_delete.py
+-rw-r--r--   0        0        0     2060 2023-04-08 20:02:57.684015 windmill_api-1.86.0/windmill_api/api/user/global_user_update.py
+-rw-r--r--   0        0        0     2468 2023-04-08 20:02:57.692016 windmill_api-1.86.0/windmill_api/api/user/global_whoami.py
+-rw-r--r--   0        0        0     2745 2023-04-08 20:02:57.724016 windmill_api-1.86.0/windmill_api/api/user/is_owner_of_path.py
+-rw-r--r--   0        0        0     1646 2023-04-08 20:02:57.720016 windmill_api-1.86.0/windmill_api/api/user/leave_workspace.py
+-rw-r--r--   0        0        0     2633 2023-04-08 20:02:57.764017 windmill_api-1.86.0/windmill_api/api/user/list_tokens.py
+-rw-r--r--   0        0        0     2552 2023-04-08 20:02:57.760017 windmill_api-1.86.0/windmill_api/api/user/list_usernames.py
+-rw-r--r--   0        0        0     3012 2023-04-08 20:02:57.800017 windmill_api-1.86.0/windmill_api/api/user/list_users.py
+-rw-r--r--   0        0        0     4222 2023-04-08 20:02:57.816018 windmill_api-1.86.0/windmill_api/api/user/list_users_as_super_admin.py
+-rw-r--r--   0        0        0     2829 2023-04-08 20:02:57.840018 windmill_api-1.86.0/windmill_api/api/user/list_workspace_invites.py
+-rw-r--r--   0        0        0     1784 2023-04-08 20:02:57.844018 windmill_api-1.86.0/windmill_api/api/user/login.py
+-rw-r--r--   0        0        0     2116 2023-04-08 20:02:57.872019 windmill_api-1.86.0/windmill_api/api/user/login_with_oauth.py
+-rw-r--r--   0        0        0     1393 2023-04-08 20:02:57.864019 windmill_api-1.86.0/windmill_api/api/user/logout.py
+-rw-r--r--   0        0        0     1820 2023-04-08 20:02:57.892019 windmill_api-1.86.0/windmill_api/api/user/set_password.py
+-rw-r--r--   0        0        0     2250 2023-04-08 20:02:57.900019 windmill_api-1.86.0/windmill_api/api/user/update_user.py
+-rw-r--r--   0        0        0     2652 2023-04-08 20:02:57.924020 windmill_api-1.86.0/windmill_api/api/user/whoami.py
+-rw-r--r--   0        0        0     2967 2023-04-08 20:02:57.944020 windmill_api-1.86.0/windmill_api/api/user/whois.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.743784 windmill_api-1.86.0/windmill_api/api/variable/__init__.py
+-rw-r--r--   0        0        0     2634 2023-04-08 20:02:57.960020 windmill_api-1.86.0/windmill_api/api/variable/create_variable.py
+-rw-r--r--   0        0        0     1784 2023-04-08 20:02:57.972020 windmill_api-1.86.0/windmill_api/api/variable/delete_variable.py
+-rw-r--r--   0        0        0     2795 2023-04-08 20:02:58.044022 windmill_api-1.86.0/windmill_api/api/variable/exists_variable.py
+-rw-r--r--   0        0        0     3840 2023-04-08 20:02:58.040022 windmill_api-1.86.0/windmill_api/api/variable/get_variable.py
+-rw-r--r--   0        0        0     3270 2023-04-08 20:02:58.080022 windmill_api-1.86.0/windmill_api/api/variable/list_contextual_variables.py
+-rw-r--r--   0        0        0     3071 2023-04-08 20:02:58.080022 windmill_api-1.86.0/windmill_api/api/variable/list_variable.py
+-rw-r--r--   0        0        0     2775 2023-04-08 20:02:58.116023 windmill_api-1.86.0/windmill_api/api/variable/update_variable.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.831786 windmill_api-1.86.0/windmill_api/api/worker/__init__.py
+-rw-r--r--   0        0        0     3896 2023-04-08 20:02:58.140024 windmill_api-1.86.0/windmill_api/api/worker/list_workers.py
+-rw-r--r--   0        0        0        0 2023-04-08 20:02:44.735784 windmill_api-1.86.0/windmill_api/api/workspace/__init__.py
+-rw-r--r--   0        0        0     2015 2023-04-08 20:02:58.144024 windmill_api-1.86.0/windmill_api/api/workspace/add_user.py
+-rw-r--r--   0        0        0     1647 2023-04-08 20:02:58.164024 windmill_api-1.86.0/windmill_api/api/workspace/archive_workspace.py
+-rw-r--r--   0        0        0     1856 2023-04-08 20:02:58.168024 windmill_api-1.86.0/windmill_api/api/workspace/create_workspace.py
+-rw-r--r--   0        0        0     2049 2023-04-08 20:02:58.196025 windmill_api-1.86.0/windmill_api/api/workspace/delete_invite.py
+-rw-r--r--   0        0        0     1688 2023-04-08 20:02:58.192024 windmill_api-1.86.0/windmill_api/api/workspace/delete_workspace.py
+-rw-r--r--   0        0        0     2063 2023-04-08 20:02:58.220025 windmill_api-1.86.0/windmill_api/api/workspace/edit_auto_invite.py
+-rw-r--r--   0        0        0     2083 2023-04-08 20:02:58.228025 windmill_api-1.86.0/windmill_api/api/workspace/edit_slack_command.py
+-rw-r--r--   0        0        0     2029 2023-04-08 20:02:58.248026 windmill_api-1.86.0/windmill_api/api/workspace/edit_webhook.py
+-rw-r--r--   0        0        0     1856 2023-04-08 20:02:58.256026 windmill_api-1.86.0/windmill_api/api/workspace/exists_username.py
+-rw-r--r--   0        0        0     1856 2023-04-08 20:02:58.276026 windmill_api-1.86.0/windmill_api/api/workspace/exists_workspace.py
+-rw-r--r--   0        0        0     2809 2023-04-08 20:02:58.304026 windmill_api-1.86.0/windmill_api/api/workspace/get_premium_info.py
+-rw-r--r--   0        0        0     2753 2023-04-08 20:02:58.312027 windmill_api-1.86.0/windmill_api/api/workspace/get_settings.py
+-rw-r--r--   0        0        0     2045 2023-04-08 20:02:58.336027 windmill_api-1.86.0/windmill_api/api/workspace/invite_user.py
+-rw-r--r--   0        0        0     2176 2023-04-08 20:02:58.360027 windmill_api-1.86.0/windmill_api/api/workspace/is_domain_allowed.py
+-rw-r--r--   0        0        0     3255 2023-04-08 20:02:58.396028 windmill_api-1.86.0/windmill_api/api/workspace/list_pending_invites.py
+-rw-r--r--   0        0        0     2583 2023-04-08 20:02:58.392028 windmill_api-1.86.0/windmill_api/api/workspace/list_user_workspaces.py
+-rw-r--r--   0        0        0     2775 2023-04-08 20:02:58.428029 windmill_api-1.86.0/windmill_api/api/workspace/list_workspaces.py
+-rw-r--r--   0        0        0     4311 2023-04-08 20:02:58.448029 windmill_api-1.86.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py
+-rw-r--r--   0        0        0     1651 2023-04-08 20:02:58.452029 windmill_api-1.86.0/windmill_api/api/workspace/unarchive_workspace.py
+-rw-r--r--   0        0        0     1821 2023-04-08 20:02:58.476029 windmill_api-1.86.0/windmill_api/client.py
+-rw-r--r--   0        0        0        1 2023-04-08 20:03:14.824319 windmill_api-1.86.0/windmill_api/models/__init__.py
+-rw-r--r--   0        0        0     1667 2023-04-08 20:02:58.504030 windmill_api-1.86.0/windmill_api/models/accept_invite_json_body.py
+-rw-r--r--   0        0        0     1710 2023-04-08 20:02:58.528030 windmill_api-1.86.0/windmill_api/models/add_granular_acls_json_body.py
+-rw-r--r--   0        0        0      301 2023-04-08 20:02:53.875948 windmill_api-1.86.0/windmill_api/models/add_granular_acls_kind.py
+-rw-r--r--   0        0        0     1529 2023-04-08 20:02:58.552031 windmill_api-1.86.0/windmill_api/models/add_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1940 2023-04-08 20:02:58.584031 windmill_api-1.86.0/windmill_api/models/add_user_json_body.py
+-rw-r--r--   0        0        0     1552 2023-04-08 20:02:58.596032 windmill_api-1.86.0/windmill_api/models/add_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3940 2023-04-08 20:02:58.632032 windmill_api-1.86.0/windmill_api/models/app_with_last_version.py
+-rw-r--r--   0        0        0      214 2023-04-08 20:02:53.795946 windmill_api-1.86.0/windmill_api/models/app_with_last_version_execution_mode.py
+-rw-r--r--   0        0        0     1248 2023-04-08 20:02:58.640032 windmill_api-1.86.0/windmill_api/models/app_with_last_version_extra_perms.py
+-rw-r--r--   0        0        0     3716 2023-04-08 20:02:58.680033 windmill_api-1.86.0/windmill_api/models/app_with_last_version_policy.py
+-rw-r--r--   0        0        0      220 2023-04-08 20:02:53.263937 windmill_api-1.86.0/windmill_api/models/app_with_last_version_policy_execution_mode.py
+-rw-r--r--   0        0        0     1946 2023-04-08 20:02:58.664033 windmill_api-1.86.0/windmill_api/models/app_with_last_version_policy_triggerables.py
+-rw-r--r--   0        0        0     1381 2023-04-08 20:02:58.688033 windmill_api-1.86.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     6879 2023-04-08 20:02:58.788035 windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1314 2023-04-08 20:02:58.708034 windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      259 2023-04-08 20:02:53.459940 windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      217 2023-04-08 20:02:53.915948 windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1288 2023-04-08 20:02:58.728034 windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     3452 2023-04-08 20:02:58.772035 windmill_api-1.86.0/windmill_api/models/audit_log.py
+-rw-r--r--   0        0        0      217 2023-04-08 20:02:53.383939 windmill_api-1.86.0/windmill_api/models/audit_log_action_kind.py
+-rw-r--r--   0        0        0      620 2023-04-08 20:02:53.291937 windmill_api-1.86.0/windmill_api/models/audit_log_operation.py
+-rw-r--r--   0        0        0     1186 2023-04-08 20:02:58.796035 windmill_api-1.86.0/windmill_api/models/audit_log_parameters.py
+-rw-r--r--   0        0        0     2933 2023-04-08 20:02:58.828036 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-04-08 20:02:58.852036 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-04-08 20:02:53.355939 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-04-08 20:02:58.856036 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-04-08 20:02:58.876037 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-04-08 20:02:58.888037 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-04-08 20:02:58.912037 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-04-08 20:02:53.151935 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-04-08 20:02:58.916037 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-04-08 20:02:58.944038 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-04-08 20:02:53.831947 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-04-08 20:02:58.940038 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-04-08 20:02:53.119934 windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2377 2023-04-08 20:02:58.976038 windmill_api-1.86.0/windmill_api/models/branch_all.py
+-rw-r--r--   0        0        0     2543 2023-04-08 20:02:58.996039 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-04-08 20:02:59.056040 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-04-08 20:02:59.036039 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-04-08 20:02:59.060040 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-04-08 20:02:59.092040 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-04-08 20:02:59.088040 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-08 20:02:53.467940 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-04-08 20:02:59.116041 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-08 20:02:53.571942 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-04-08 20:02:59.152042 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-04-08 20:02:59.144041 windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-04-08 20:02:54.127952 windmill_api-1.86.0/windmill_api/models/branch_all_type.py
+-rw-r--r--   0        0        0     2670 2023-04-08 20:02:59.180042 windmill_api-1.86.0/windmill_api/models/branch_one.py
+-rw-r--r--   0        0        0     2372 2023-04-08 20:02:59.184042 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item.py
+-rw-r--r--   0        0        0     6620 2023-04-08 20:02:59.256043 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3129 2023-04-08 20:02:59.224043 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     1929 2023-04-08 20:02:59.252043 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-04-08 20:02:59.296044 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-04-08 20:02:59.284044 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-08 20:02:53.383939 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-04-08 20:02:59.312044 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-08 20:02:54.007950 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-04-08 20:02:59.328045 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-04-08 20:02:59.356045 windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6125 2023-04-08 20:02:59.412046 windmill_api-1.86.0/windmill_api/models/branch_one_default_item.py
+-rw-r--r--   0        0        0     2906 2023-04-08 20:02:59.392046 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-04-08 20:02:59.420046 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-04-08 20:02:59.444047 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-04-08 20:02:59.448047 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-04-08 20:02:53.723945 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-04-08 20:02:59.472047 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-04-08 20:02:53.251937 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-04-08 20:02:59.476047 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-04-08 20:02:59.504048 windmill_api-1.86.0/windmill_api/models/branch_one_default_item_suspend.py
+-rw-r--r--   0        0        0      146 2023-04-08 20:02:53.651944 windmill_api-1.86.0/windmill_api/models/branch_one_type.py
+-rw-r--r--   0        0        0     1532 2023-04-08 20:02:59.516048 windmill_api-1.86.0/windmill_api/models/cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     1255 2023-04-08 20:02:59.548048 windmill_api-1.86.0/windmill_api/models/cancel_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0    10376 2023-04-08 20:02:59.640050 windmill_api-1.86.0/windmill_api/models/completed_job.py
+-rw-r--r--   0        0        0     1176 2023-04-08 20:02:59.568049 windmill_api-1.86.0/windmill_api/models/completed_job_args.py
+-rw-r--r--   0        0        0     3265 2023-04-08 20:02:59.608049 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status.py
+-rw-r--r--   0        0        0     6800 2023-04-08 20:02:59.692051 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1789 2023-04-08 20:02:59.668051 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2136 2023-04-08 20:02:59.720051 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      202 2023-04-08 20:02:53.847947 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1694 2023-04-08 20:02:59.720051 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2230 2023-04-08 20:02:59.752052 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      360 2023-04-08 20:02:53.451940 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6402 2023-04-08 20:02:59.804053 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1779 2023-04-08 20:02:59.776053 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2116 2023-04-08 20:02:59.804053 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      200 2023-04-08 20:02:53.895948 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1684 2023-04-08 20:02:59.828053 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2220 2023-04-08 20:02:59.844054 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      358 2023-04-08 20:02:53.463940 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2040 2023-04-08 20:02:59.860054 windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_retry.py
+-rw-r--r--   0        0        0      310 2023-04-08 20:02:53.407940 windmill_api-1.86.0/windmill_api/models/completed_job_job_kind.py
+-rw-r--r--   0        0        0      199 2023-04-08 20:02:53.495941 windmill_api-1.86.0/windmill_api/models/completed_job_language.py
+-rw-r--r--   0        0        0     3127 2023-04-08 20:02:59.916055 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow.py
+-rw-r--r--   0        0        0     6620 2023-04-08 20:02:59.936055 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3129 2023-04-08 20:02:59.956056 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1929 2023-04-08 20:02:59.964056 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2233 2023-04-08 20:02:59.988056 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2079 2023-04-08 20:02:59.992056 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-08 20:02:53.647944 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1946 2023-04-08 20:03:00.020057 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-08 20:02:54.127952 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1922 2023-04-08 20:03:00.020057 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1973 2023-04-08 20:03:00.048057 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6544 2023-04-08 20:03:00.120059 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3095 2023-04-08 20:03:00.088058 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1919 2023-04-08 20:03:00.116058 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2223 2023-04-08 20:03:00.152059 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2050 2023-04-08 20:03:00.148059 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      179 2023-04-08 20:02:54.107952 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1917 2023-04-08 20:03:00.172059 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      179 2023-04-08 20:02:53.287937 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1912 2023-04-08 20:03:00.184060 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1963 2023-04-08 20:03:00.200060 windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1572 2023-04-08 20:03:00.212060 windmill_api-1.86.0/windmill_api/models/connect_callback_json_body.py
+-rw-r--r--   0        0        0     2533 2023-04-08 20:03:00.236061 windmill_api-1.86.0/windmill_api/models/connect_callback_response_200.py
+-rw-r--r--   0        0        0     1600 2023-04-08 20:03:00.236061 windmill_api-1.86.0/windmill_api/models/connect_slack_callback_json_body.py
+-rw-r--r--   0        0        0     1753 2023-04-08 20:03:00.264061 windmill_api-1.86.0/windmill_api/models/contextual_variable.py
+-rw-r--r--   0        0        0     2147 2023-04-08 20:03:00.268061 windmill_api-1.86.0/windmill_api/models/create_account_json_body.py
+-rw-r--r--   0        0        0     2035 2023-04-08 20:03:00.312062 windmill_api-1.86.0/windmill_api/models/create_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-04-08 20:03:00.316062 windmill_api-1.86.0/windmill_api/models/create_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-04-08 20:02:53.551942 windmill_api-1.86.0/windmill_api/models/create_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-04-08 20:03:00.348063 windmill_api-1.86.0/windmill_api/models/create_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-04-08 20:03:00.332062 windmill_api-1.86.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-04-08 20:03:00.376063 windmill_api-1.86.0/windmill_api/models/create_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-04-08 20:03:00.372063 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-04-08 20:03:00.412064 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-04-08 20:03:00.480065 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-04-08 20:03:00.452064 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-04-08 20:03:00.480065 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-04-08 20:03:00.516066 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-04-08 20:03:00.508066 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-04-08 20:02:53.583943 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-04-08 20:03:00.536066 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-04-08 20:02:54.099952 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-04-08 20:03:00.548066 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-04-08 20:03:00.564067 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-04-08 20:03:00.628068 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-04-08 20:03:00.600067 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-04-08 20:03:00.628068 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-04-08 20:03:00.680069 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-04-08 20:03:00.656068 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-04-08 20:02:53.671944 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-04-08 20:03:00.688069 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-04-08 20:02:53.779946 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-04-08 20:03:00.708069 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-04-08 20:03:00.716069 windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2126 2023-04-08 20:03:00.744070 windmill_api-1.86.0/windmill_api/models/create_folder_json_body.py
+-rw-r--r--   0        0        0     1697 2023-04-08 20:03:00.740069 windmill_api-1.86.0/windmill_api/models/create_group_json_body.py
+-rw-r--r--   0        0        0     2094 2023-04-08 20:03:00.772070 windmill_api-1.86.0/windmill_api/models/create_resource.py
+-rw-r--r--   0        0        0     2140 2023-04-08 20:03:00.776070 windmill_api-1.86.0/windmill_api/models/create_resource_json_body.py
+-rw-r--r--   0        0        0     2335 2023-04-08 20:03:00.832071 windmill_api-1.86.0/windmill_api/models/create_resource_type_json_body.py
+-rw-r--r--   0        0        0     2780 2023-04-08 20:03:00.816071 windmill_api-1.86.0/windmill_api/models/create_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-04-08 20:03:00.836071 windmill_api-1.86.0/windmill_api/models/create_schedule_json_body_args.py
+-rw-r--r--   0        0        0     4616 2023-04-08 20:03:00.896072 windmill_api-1.86.0/windmill_api/models/create_script_json_body.py
+-rw-r--r--   0        0        0      249 2023-04-08 20:02:53.647944 windmill_api-1.86.0/windmill_api/models/create_script_json_body_kind.py
+-rw-r--r--   0        0        0      207 2023-04-08 20:02:53.399939 windmill_api-1.86.0/windmill_api/models/create_script_json_body_language.py
+-rw-r--r--   0        0        0     1232 2023-04-08 20:03:00.864072 windmill_api-1.86.0/windmill_api/models/create_script_json_body_schema.py
+-rw-r--r--   0        0        0     2534 2023-04-08 20:03:00.900072 windmill_api-1.86.0/windmill_api/models/create_token_impersonate_json_body.py
+-rw-r--r--   0        0        0     2169 2023-04-08 20:03:00.928073 windmill_api-1.86.0/windmill_api/models/create_token_json_body.py
+-rw-r--r--   0        0        0     2364 2023-04-08 20:03:00.936073 windmill_api-1.86.0/windmill_api/models/create_user_globally_json_body.py
+-rw-r--r--   0        0        0     1771 2023-04-08 20:03:00.952073 windmill_api-1.86.0/windmill_api/models/create_user_json_body.py
+-rw-r--r--   0        0        0     2493 2023-04-08 20:03:00.976074 windmill_api-1.86.0/windmill_api/models/create_variable.py
+-rw-r--r--   0        0        0     2539 2023-04-08 20:03:00.992074 windmill_api-1.86.0/windmill_api/models/create_variable_json_body.py
+-rw-r--r--   0        0        0     1678 2023-04-08 20:03:01.004074 windmill_api-1.86.0/windmill_api/models/create_workspace.py
+-rw-r--r--   0        0        0     1724 2023-04-08 20:03:01.016075 windmill_api-1.86.0/windmill_api/models/create_workspace_json_body.py
+-rw-r--r--   0        0        0     1490 2023-04-08 20:03:01.028075 windmill_api-1.86.0/windmill_api/models/decline_invite_json_body.py
+-rw-r--r--   0        0        0    10978 2023-04-08 20:03:01.184077 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200.py
+-rw-r--r--   0        0        0     1270 2023-04-08 20:03:01.064075 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3658 2023-04-08 20:03:01.108076 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7442 2023-04-08 20:03:01.196078 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1883 2023-04-08 20:03:01.208078 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2318 2023-04-08 20:03:01.224078 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      219 2023-04-08 20:02:53.259937 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1788 2023-04-08 20:03:01.232078 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2324 2023-04-08 20:03:01.264079 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      377 2023-04-08 20:02:53.995950 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7053 2023-04-08 20:03:01.312080 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1873 2023-04-08 20:03:01.288079 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2298 2023-04-08 20:03:01.320080 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      217 2023-04-08 20:02:53.947949 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1778 2023-04-08 20:03:01.340080 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2314 2023-04-08 20:03:01.360081 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      375 2023-04-08 20:02:54.151953 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2134 2023-04-08 20:03:01.372081 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      327 2023-04-08 20:02:54.111952 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      216 2023-04-08 20:02:54.139953 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3432 2023-04-08 20:03:01.408081 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7425 2023-04-08 20:03:01.460082 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3442 2023-04-08 20:03:01.476083 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2023 2023-04-08 20:03:01.492083 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2327 2023-04-08 20:03:01.508083 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2261 2023-04-08 20:03:01.560084 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-08 20:02:53.211936 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-08 20:03:01.540084 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-08 20:02:53.843947 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2016 2023-04-08 20:03:01.572084 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2067 2023-04-08 20:03:01.588085 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7349 2023-04-08 20:03:01.656086 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3408 2023-04-08 20:03:01.624085 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2013 2023-04-08 20:03:01.652086 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2317 2023-04-08 20:03:01.684086 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2241 2023-04-08 20:03:01.684086 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-04-08 20:02:53.291937 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2108 2023-04-08 20:03:01.712087 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-04-08 20:02:53.751946 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2006 2023-04-08 20:03:01.716087 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2057 2023-04-08 20:03:01.736087 windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1783 2023-04-08 20:03:01.752087 windmill_api-1.86.0/windmill_api/models/delete_invite_json_body.py
+-rw-r--r--   0        0        0     6853 2023-04-08 20:03:01.816089 windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1309 2023-04-08 20:03:01.772088 windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      258 2023-04-08 20:02:53.803947 windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      216 2023-04-08 20:02:54.063951 windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1283 2023-04-08 20:03:01.800088 windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     2933 2023-04-08 20:03:01.860089 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5556 2023-04-08 20:03:01.876090 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      326 2023-04-08 20:02:53.531942 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1608 2023-04-08 20:03:01.888090 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1673 2023-04-08 20:03:01.936091 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2171 2023-04-08 20:03:01.916090 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3293 2023-04-08 20:03:01.956091 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      344 2023-04-08 20:02:53.247937 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1641 2023-04-08 20:03:01.960091 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3161 2023-04-08 20:03:01.996092 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      335 2023-04-08 20:02:53.591943 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1590 2023-04-08 20:03:01.984092 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      180 2023-04-08 20:02:53.695945 windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     1551 2023-04-08 20:03:02.008092 windmill_api-1.86.0/windmill_api/models/edit_auto_invite_json_body.py
+-rw-r--r--   0        0        0     1980 2023-04-08 20:03:02.032092 windmill_api-1.86.0/windmill_api/models/edit_resource.py
+-rw-r--r--   0        0        0     1791 2023-04-08 20:03:02.036093 windmill_api-1.86.0/windmill_api/models/edit_resource_type.py
+-rw-r--r--   0        0        0     1845 2023-04-08 20:03:02.060093 windmill_api-1.86.0/windmill_api/models/edit_schedule.py
+-rw-r--r--   0        0        0     1176 2023-04-08 20:03:02.056093 windmill_api-1.86.0/windmill_api/models/edit_schedule_args.py
+-rw-r--r--   0        0        0     1691 2023-04-08 20:03:02.080093 windmill_api-1.86.0/windmill_api/models/edit_slack_command_json_body.py
+-rw-r--r--   0        0        0     2260 2023-04-08 20:03:02.100094 windmill_api-1.86.0/windmill_api/models/edit_variable.py
+-rw-r--r--   0        0        0     1520 2023-04-08 20:03:02.104094 windmill_api-1.86.0/windmill_api/models/edit_webhook_json_body.py
+-rw-r--r--   0        0        0     2058 2023-04-08 20:03:02.132094 windmill_api-1.86.0/windmill_api/models/edit_workspace_user.py
+-rw-r--r--   0        0        0     3663 2023-04-08 20:03:02.148095 windmill_api-1.86.0/windmill_api/models/execute_component_json_body.py
+-rw-r--r--   0        0        0     1346 2023-04-08 20:03:02.152095 windmill_api-1.86.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py
+-rw-r--r--   0        0        0     1942 2023-04-08 20:03:02.180095 windmill_api-1.86.0/windmill_api/models/execute_component_json_body_raw_code.py
+-rw-r--r--   0        0        0     1577 2023-04-08 20:03:02.176095 windmill_api-1.86.0/windmill_api/models/exists_username_json_body.py
+-rw-r--r--   0        0        0     1400 2023-04-08 20:03:02.200096 windmill_api-1.86.0/windmill_api/models/exists_workspace_json_body.py
+-rw-r--r--   0        0        0     4633 2023-04-08 20:03:02.240096 windmill_api-1.86.0/windmill_api/models/flow.py
+-rw-r--r--   0        0        0     1166 2023-04-08 20:03:02.244096 windmill_api-1.86.0/windmill_api/models/flow_extra_perms.py
+-rw-r--r--   0        0        0     3416 2023-04-08 20:03:02.316098 windmill_api-1.86.0/windmill_api/models/flow_metadata.py
+-rw-r--r--   0        0        0     1209 2023-04-08 20:03:02.264097 windmill_api-1.86.0/windmill_api/models/flow_metadata_extra_perms.py
+-rw-r--r--   0        0        0     5729 2023-04-08 20:03:02.344098 windmill_api-1.86.0/windmill_api/models/flow_module.py
+-rw-r--r--   0        0        0     2726 2023-04-08 20:03:02.352098 windmill_api-1.86.0/windmill_api/models/flow_module_retry.py
+-rw-r--r--   0        0        0     1807 2023-04-08 20:03:02.372099 windmill_api-1.86.0/windmill_api/models/flow_module_retry_constant.py
+-rw-r--r--   0        0        0     2111 2023-04-08 20:03:02.384099 windmill_api-1.86.0/windmill_api/models/flow_module_retry_exponential.py
+-rw-r--r--   0        0        0     1834 2023-04-08 20:03:02.404099 windmill_api-1.86.0/windmill_api/models/flow_module_sleep_type_0.py
+-rw-r--r--   0        0        0      159 2023-04-08 20:02:53.303938 windmill_api-1.86.0/windmill_api/models/flow_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1701 2023-04-08 20:03:02.412099 windmill_api-1.86.0/windmill_api/models/flow_module_sleep_type_1.py
+-rw-r--r--   0        0        0      159 2023-04-08 20:02:53.307938 windmill_api-1.86.0/windmill_api/models/flow_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1800 2023-04-08 20:03:02.432100 windmill_api-1.86.0/windmill_api/models/flow_module_stop_after_if.py
+-rw-r--r--   0        0        0     1851 2023-04-08 20:03:02.440100 windmill_api-1.86.0/windmill_api/models/flow_module_suspend.py
+-rw-r--r--   0        0        0     3080 2023-04-08 20:03:02.472100 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0.py
+-rw-r--r--   0        0        0     3564 2023-04-08 20:03:02.476100 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-04-08 20:03:02.504101 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-08 20:02:53.243936 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-08 20:03:02.504101 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-08 20:02:53.255937 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      208 2023-04-08 20:02:53.851947 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_language.py
+-rw-r--r--   0        0        0      158 2023-04-08 20:02:53.551942 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_type.py
+-rw-r--r--   0        0        0     2477 2023-04-08 20:03:02.540101 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1.py
+-rw-r--r--   0        0        0     3564 2023-04-08 20:03:02.544102 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-04-08 20:03:02.564102 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-08 20:02:53.251937 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-08 20:03:02.576102 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-08 20:02:53.551942 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      152 2023-04-08 20:02:53.475941 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_type.py
+-rw-r--r--   0        0        0     2204 2023-04-08 20:03:02.596103 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2.py
+-rw-r--r--   0        0        0     3564 2023-04-08 20:03:02.640103 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py
+-rw-r--r--   0        0        0     2261 2023-04-08 20:03:02.624103 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      198 2023-04-08 20:02:54.043951 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2128 2023-04-08 20:03:02.680104 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      198 2023-04-08 20:02:54.167953 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      148 2023-04-08 20:02:53.791946 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_type.py
+-rw-r--r--   0        0        0     4138 2023-04-08 20:03:02.692104 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3.py
+-rw-r--r--   0        0        0     1990 2023-04-08 20:03:02.708104 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py
+-rw-r--r--   0        0        0      173 2023-04-08 20:02:53.315938 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1857 2023-04-08 20:03:02.720105 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py
+-rw-r--r--   0        0        0      173 2023-04-08 20:02:54.131952 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6636 2023-04-08 20:03:02.792106 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py
+-rw-r--r--   0        0        0     3148 2023-04-08 20:03:02.760105 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-04-08 20:03:02.788106 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-04-08 20:03:02.816106 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-04-08 20:03:02.824107 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-08 20:02:53.459940 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-04-08 20:03:02.844107 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-08 20:02:53.971949 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-04-08 20:03:02.852107 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-04-08 20:03:02.876108 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py
+-rw-r--r--   0        0        0      162 2023-04-08 20:02:53.259937 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_type.py
+-rw-r--r--   0        0        0     2934 2023-04-08 20:03:02.888108 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4.py
+-rw-r--r--   0        0        0     2508 2023-04-08 20:03:02.912108 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-04-08 20:03:02.972109 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-04-08 20:03:02.952109 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-04-08 20:03:03.004110 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-04-08 20:03:03.000110 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-04-08 20:03:03.068111 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-08 20:02:53.591943 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-04-08 20:03:03.032110 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-08 20:02:53.831947 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-04-08 20:03:03.064111 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-04-08 20:03:03.092111 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0     6636 2023-04-08 20:03:03.148112 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item.py
+-rw-r--r--   0        0        0     3148 2023-04-08 20:03:03.132112 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py
+-rw-r--r--   0        0        0     1935 2023-04-08 20:03:03.160112 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py
+-rw-r--r--   0        0        0     2239 2023-04-08 20:03:03.180113 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py
+-rw-r--r--   0        0        0     2087 2023-04-08 20:03:03.192113 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py
+-rw-r--r--   0        0        0      181 2023-04-08 20:02:53.239936 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1954 2023-04-08 20:03:03.204113 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py
+-rw-r--r--   0        0        0      181 2023-04-08 20:02:53.719945 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1928 2023-04-08 20:03:03.220114 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py
+-rw-r--r--   0        0        0     1979 2023-04-08 20:03:03.232114 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-04-08 20:02:53.975950 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_type.py
+-rw-r--r--   0        0        0     2577 2023-04-08 20:03:03.260114 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5.py
+-rw-r--r--   0        0        0     2679 2023-04-08 20:03:03.268114 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py
+-rw-r--r--   0        0        0     7243 2023-04-08 20:03:03.368116 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py
+-rw-r--r--   0        0        0     3362 2023-04-08 20:03:03.308115 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py
+-rw-r--r--   0        0        0     2001 2023-04-08 20:03:03.332116 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2305 2023-04-08 20:03:03.364116 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2215 2023-04-08 20:03:03.392117 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-08 20:02:54.139953 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2082 2023-04-08 20:03:03.400117 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-08 20:02:53.503941 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1994 2023-04-08 20:03:03.456118 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2045 2023-04-08 20:03:03.428117 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py
+-rw-r--r--   0        0        0      158 2023-04-08 20:02:53.879948 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_type.py
+-rw-r--r--   0        0        0     1839 2023-04-08 20:03:03.460118 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_6.py
+-rw-r--r--   0        0        0      156 2023-04-08 20:02:53.723945 windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_6_type.py
+-rw-r--r--   0        0        0     2009 2023-04-08 20:03:03.488119 windmill_api-1.86.0/windmill_api/models/flow_preview.py
+-rw-r--r--   0        0        0     1171 2023-04-08 20:03:03.480118 windmill_api-1.86.0/windmill_api/models/flow_preview_args.py
+-rw-r--r--   0        0        0     3074 2023-04-08 20:03:03.520119 windmill_api-1.86.0/windmill_api/models/flow_preview_value.py
+-rw-r--r--   0        0        0     6498 2023-04-08 20:03:03.564120 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module.py
+-rw-r--r--   0        0        0     3064 2023-04-08 20:03:03.560120 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1911 2023-04-08 20:03:03.588120 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2215 2023-04-08 20:03:03.596120 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2036 2023-04-08 20:03:03.620121 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-04-08 20:02:53.547942 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1903 2023-04-08 20:03:03.624121 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-08 20:02:53.507941 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1904 2023-04-08 20:03:03.652121 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1955 2023-04-08 20:03:03.660122 windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6422 2023-04-08 20:03:03.728123 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item.py
+-rw-r--r--   0        0        0     3030 2023-04-08 20:03:03.696122 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1901 2023-04-08 20:03:03.728123 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2205 2023-04-08 20:03:03.792124 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2016 2023-04-08 20:03:03.760123 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-04-08 20:02:53.975950 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1883 2023-04-08 20:03:03.828125 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-04-08 20:02:53.555942 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1894 2023-04-08 20:03:03.824124 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1945 2023-04-08 20:03:03.856125 windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1143 2023-04-08 20:03:03.848125 windmill_api-1.86.0/windmill_api/models/flow_schema.py
+-rw-r--r--   0        0        0     3001 2023-04-08 20:03:03.888126 windmill_api-1.86.0/windmill_api/models/flow_status.py
+-rw-r--r--   0        0        0     6370 2023-04-08 20:03:03.936127 windmill_api-1.86.0/windmill_api/models/flow_status_failure_module.py
+-rw-r--r--   0        0        0     1723 2023-04-08 20:03:03.912126 windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     1999 2023-04-08 20:03:03.940127 windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      190 2023-04-08 20:02:53.463940 windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1628 2023-04-08 20:03:03.968127 windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2164 2023-04-08 20:03:03.976127 windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      348 2023-04-08 20:02:53.243936 windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     5808 2023-04-08 20:03:04.052129 windmill_api-1.86.0/windmill_api/models/flow_status_module.py
+-rw-r--r--   0        0        0     1685 2023-04-08 20:03:04.000128 windmill_api-1.86.0/windmill_api/models/flow_status_module_approvers_item.py
+-rw-r--r--   0        0        0     1925 2023-04-08 20:03:04.028128 windmill_api-1.86.0/windmill_api/models/flow_status_module_branch_chosen.py
+-rw-r--r--   0        0        0      183 2023-04-08 20:02:53.515941 windmill_api-1.86.0/windmill_api/models/flow_status_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1590 2023-04-08 20:03:04.056129 windmill_api-1.86.0/windmill_api/models/flow_status_module_branchall.py
+-rw-r--r--   0        0        0     2126 2023-04-08 20:03:04.088129 windmill_api-1.86.0/windmill_api/models/flow_status_module_iterator.py
+-rw-r--r--   0        0        0      341 2023-04-08 20:02:53.979950 windmill_api-1.86.0/windmill_api/models/flow_status_module_type.py
+-rw-r--r--   0        0        0     5981 2023-04-08 20:03:04.132130 windmill_api-1.86.0/windmill_api/models/flow_status_modules_item.py
+-rw-r--r--   0        0        0     1713 2023-04-08 20:03:04.112130 windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     1979 2023-04-08 20:03:04.176131 windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      188 2023-04-08 20:02:53.339938 windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1618 2023-04-08 20:03:04.204131 windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2154 2023-04-08 20:03:04.216132 windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      346 2023-04-08 20:02:53.343938 windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     1974 2023-04-08 20:03:04.240132 windmill_api-1.86.0/windmill_api/models/flow_status_retry.py
+-rw-r--r--   0        0        0     2957 2023-04-08 20:03:04.256132 windmill_api-1.86.0/windmill_api/models/flow_value.py
+-rw-r--r--   0        0        0     6224 2023-04-08 20:03:04.316133 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module.py
+-rw-r--r--   0        0        0     2940 2023-04-08 20:03:04.296133 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1873 2023-04-08 20:03:04.328134 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-04-08 20:03:04.348134 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-04-08 20:03:04.356134 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-04-08 20:02:53.351938 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-04-08 20:03:04.376134 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-04-08 20:02:53.495941 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-04-08 20:03:04.388135 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-04-08 20:03:04.404135 windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6125 2023-04-08 20:03:04.464136 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item.py
+-rw-r--r--   0        0        0     2906 2023-04-08 20:03:04.440136 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1863 2023-04-08 20:03:04.468136 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2167 2023-04-08 20:03:04.500137 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1942 2023-04-08 20:03:04.496137 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      169 2023-04-08 20:02:54.171953 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1809 2023-04-08 20:03:04.524137 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      169 2023-04-08 20:02:53.611943 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1856 2023-04-08 20:03:04.560138 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1907 2023-04-08 20:03:04.552138 windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1858 2023-04-08 20:03:04.580138 windmill_api-1.86.0/windmill_api/models/folder.py
+-rw-r--r--   0        0        0     1179 2023-04-08 20:03:04.580138 windmill_api-1.86.0/windmill_api/models/folder_extra_perms.py
+-rw-r--r--   0        0        0     1560 2023-04-08 20:03:04.604138 windmill_api-1.86.0/windmill_api/models/force_cancel_queued_job_json_body.py
+-rw-r--r--   0        0        0     3807 2023-04-08 20:03:04.664140 windmill_api-1.86.0/windmill_api/models/forloop_flow.py
+-rw-r--r--   0        0        0     1874 2023-04-08 20:03:04.632139 windmill_api-1.86.0/windmill_api/models/forloop_flow_iterator_type_0.py
+-rw-r--r--   0        0        0      163 2023-04-08 20:02:53.811947 windmill_api-1.86.0/windmill_api/models/forloop_flow_iterator_type_0_type.py
+-rw-r--r--   0        0        0     1741 2023-04-08 20:03:04.660140 windmill_api-1.86.0/windmill_api/models/forloop_flow_iterator_type_1.py
+-rw-r--r--   0        0        0      163 2023-04-08 20:02:53.439940 windmill_api-1.86.0/windmill_api/models/forloop_flow_iterator_type_1_type.py
+-rw-r--r--   0        0        0     6224 2023-04-08 20:03:04.744141 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item.py
+-rw-r--r--   0        0        0     2940 2023-04-08 20:03:04.704140 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1873 2023-04-08 20:03:04.732141 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2177 2023-04-08 20:03:04.760141 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1962 2023-04-08 20:03:04.772142 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      171 2023-04-08 20:02:53.871948 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1829 2023-04-08 20:03:04.788142 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      171 2023-04-08 20:02:53.255937 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1866 2023-04-08 20:03:04.800142 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1917 2023-04-08 20:03:04.816142 windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0      152 2023-04-08 20:02:53.175935 windmill_api-1.86.0/windmill_api/models/forloop_flow_type.py
+-rw-r--r--   0        0        0     4052 2023-04-08 20:03:04.852143 windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200.py
+-rw-r--r--   0        0        0      219 2023-04-08 20:02:53.719945 windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1279 2023-04-08 20:03:04.836143 windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3811 2023-04-08 20:03:04.884144 windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_policy.py
+-rw-r--r--   0        0        0      225 2023-04-08 20:02:53.471941 windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2009 2023-04-08 20:03:04.876144 windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1412 2023-04-08 20:03:04.896144 windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     4112 2023-04-08 20:03:04.936144 windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200.py
+-rw-r--r--   0        0        0      222 2023-04-08 20:02:54.019950 windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1294 2023-04-08 20:03:04.948145 windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3862 2023-04-08 20:03:04.980145 windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_policy.py
+-rw-r--r--   0        0        0      228 2023-04-08 20:02:53.923949 windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2042 2023-04-08 20:03:04.976145 windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1427 2023-04-08 20:03:04.996146 windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3764 2023-04-08 20:03:05.080147 windmill_api-1.86.0/windmill_api/models/get_audit_log_response_200.py
+-rw-r--r--   0        0        0      231 2023-04-08 20:02:53.499941 windmill_api-1.86.0/windmill_api/models/get_audit_log_response_200_action_kind.py
+-rw-r--r--   0        0        0      634 2023-04-08 20:02:53.395939 windmill_api-1.86.0/windmill_api/models/get_audit_log_response_200_operation.py
+-rw-r--r--   0        0        0     1265 2023-04-08 20:03:05.020146 windmill_api-1.86.0/windmill_api/models/get_audit_log_response_200_parameters.py
+-rw-r--r--   0        0        0    10876 2023-04-08 20:03:05.152148 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200.py
+-rw-r--r--   0        0        0     1255 2023-04-08 20:03:05.100148 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_args.py
+-rw-r--r--   0        0        0     3595 2023-04-08 20:03:05.140148 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status.py
+-rw-r--r--   0        0        0     7343 2023-04-08 20:03:05.224150 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1868 2023-04-08 20:03:05.180149 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2288 2023-04-08 20:03:05.208150 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      216 2023-04-08 20:02:53.763946 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1773 2023-04-08 20:03:05.236150 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2309 2023-04-08 20:03:05.260150 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      374 2023-04-08 20:02:53.535942 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6924 2023-04-08 20:03:05.380153 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1858 2023-04-08 20:03:05.284151 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-04-08 20:03:05.312151 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-04-08 20:02:53.727945 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-04-08 20:03:05.340152 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2299 2023-04-08 20:03:05.376152 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      372 2023-04-08 20:02:53.111934 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2119 2023-04-08 20:03:05.464154 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py
+-rw-r--r--   0        0        0      324 2023-04-08 20:02:54.147953 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_job_kind.py
+-rw-r--r--   0        0        0      213 2023-04-08 20:02:54.011950 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_language.py
+-rw-r--r--   0        0        0     3375 2023-04-08 20:03:05.428153 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow.py
+-rw-r--r--   0        0        0     7311 2023-04-08 20:03:05.512155 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3391 2023-04-08 20:03:05.504155 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2008 2023-04-08 20:03:05.532155 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2312 2023-04-08 20:03:05.544155 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2231 2023-04-08 20:03:05.564156 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      195 2023-04-08 20:02:53.467940 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2098 2023-04-08 20:03:05.576156 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      195 2023-04-08 20:02:54.023950 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2001 2023-04-08 20:03:05.592156 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2052 2023-04-08 20:03:05.608157 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7235 2023-04-08 20:03:05.676158 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3357 2023-04-08 20:03:05.648157 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1998 2023-04-08 20:03:05.680158 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-04-08 20:03:05.708158 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-04-08 20:03:05.748159 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-08 20:02:53.143935 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-04-08 20:03:05.736159 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-08 20:02:53.751946 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-04-08 20:03:05.772160 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-04-08 20:03:05.780160 windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     5083 2023-04-08 20:03:05.896162 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200.py
+-rw-r--r--   0        0        0     1281 2023-04-08 20:03:05.796160 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1258 2023-04-08 20:03:05.816160 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     3302 2023-04-08 20:03:05.860161 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value.py
+-rw-r--r--   0        0        0     7159 2023-04-08 20:03:05.940163 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py
+-rw-r--r--   0        0        0     3323 2023-04-08 20:03:05.936163 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1988 2023-04-08 20:03:05.964163 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-04-08 20:03:05.976163 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-04-08 20:03:05.992164 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-04-08 20:02:53.499941 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-04-08 20:03:06.008164 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-04-08 20:02:53.347938 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-04-08 20:03:06.024164 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-04-08 20:03:06.036164 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7066 2023-04-08 20:03:06.104166 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py
+-rw-r--r--   0        0        0     3289 2023-04-08 20:03:06.076165 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1978 2023-04-08 20:03:06.148166 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2282 2023-04-08 20:03:06.136166 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2171 2023-04-08 20:03:06.164167 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-04-08 20:02:53.547942 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2038 2023-04-08 20:03:06.180167 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-04-08 20:02:53.891948 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1971 2023-04-08 20:03:06.192167 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2022 2023-04-08 20:03:06.208167 windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2010 2023-04-08 20:03:06.288169 windmill_api-1.86.0/windmill_api/models/get_folder_response_200.py
+-rw-r--r--   0        0        0     1258 2023-04-08 20:03:06.228168 windmill_api-1.86.0/windmill_api/models/get_folder_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2357 2023-04-08 20:03:06.264168 windmill_api-1.86.0/windmill_api/models/get_folder_usage_response_200.py
+-rw-r--r--   0        0        0      301 2023-04-08 20:02:53.363939 windmill_api-1.86.0/windmill_api/models/get_granular_acls_kind.py
+-rw-r--r--   0        0        0     1235 2023-04-08 20:03:06.288169 windmill_api-1.86.0/windmill_api/models/get_granular_acls_response_200.py
+-rw-r--r--   0        0        0     2888 2023-04-08 20:03:06.332170 windmill_api-1.86.0/windmill_api/models/get_group_response_200.py
+-rw-r--r--   0        0        0     1253 2023-04-08 20:03:06.308169 windmill_api-1.86.0/windmill_api/models/get_group_response_200_extra_perms.py
+-rw-r--r--   0        0        0     1606 2023-04-08 20:03:06.332170 windmill_api-1.86.0/windmill_api/models/get_hub_app_by_id_response_200.py
+-rw-r--r--   0        0        0     1634 2023-04-08 20:03:06.360170 windmill_api-1.86.0/windmill_api/models/get_hub_app_by_id_response_200_app.py
+-rw-r--r--   0        0        0     1977 2023-04-08 20:03:06.364170 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200.py
+-rw-r--r--   0        0        0     2950 2023-04-08 20:03:06.400171 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py
+-rw-r--r--   0        0        0     1289 2023-04-08 20:03:06.380170 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py
+-rw-r--r--   0        0        0     3410 2023-04-08 20:03:06.424171 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py
+-rw-r--r--   0        0        0     7365 2023-04-08 20:03:06.488172 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3418 2023-04-08 20:03:06.464172 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     2019 2023-04-08 20:03:06.492173 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2323 2023-04-08 20:03:06.572174 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2249 2023-04-08 20:03:06.524173 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      196 2023-04-08 20:02:53.555942 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2116 2023-04-08 20:03:06.552174 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      196 2023-04-08 20:02:53.379939 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2012 2023-04-08 20:03:06.584174 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2063 2023-04-08 20:03:06.600175 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7289 2023-04-08 20:03:06.724177 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py
+-rw-r--r--   0        0        0     3384 2023-04-08 20:03:06.640175 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     2009 2023-04-08 20:03:06.668176 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2313 2023-04-08 20:03:06.700176 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2229 2023-04-08 20:03:06.732177 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      194 2023-04-08 20:02:53.563942 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2096 2023-04-08 20:03:06.752177 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      194 2023-04-08 20:02:53.691944 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2002 2023-04-08 20:03:06.760177 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2053 2023-04-08 20:03:06.784178 windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2698 2023-04-08 20:03:06.800178 windmill_api-1.86.0/windmill_api/models/get_hub_script_by_path_response_200.py
+-rw-r--r--   0        0        0      216 2023-04-08 20:02:53.219936 windmill_api-1.86.0/windmill_api/models/get_hub_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     1852 2023-04-08 20:03:06.816178 windmill_api-1.86.0/windmill_api/models/get_job_response_200.py
+-rw-r--r--   0        0        0      188 2023-04-08 20:02:53.963949 windmill_api-1.86.0/windmill_api/models/get_job_response_200_type.py
+-rw-r--r--   0        0        0     2364 2023-04-08 20:03:06.836179 windmill_api-1.86.0/windmill_api/models/get_job_updates_response_200.py
+-rw-r--r--   0        0        0     1744 2023-04-08 20:03:06.844179 windmill_api-1.86.0/windmill_api/models/get_premium_info_response_200.py
+-rw-r--r--   0        0        0     4218 2023-04-08 20:03:06.888180 windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200.py
+-rw-r--r--   0        0        0      227 2023-04-08 20:02:53.731945 windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_execution_mode.py
+-rw-r--r--   0        0        0     1322 2023-04-08 20:03:06.868179 windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py
+-rw-r--r--   0        0        0     3970 2023-04-08 20:03:06.916180 windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py
+-rw-r--r--   0        0        0      233 2023-04-08 20:02:53.259937 windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_policy_execution_mode.py
+-rw-r--r--   0        0        0     2131 2023-04-08 20:03:06.912180 windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py
+-rw-r--r--   0        0        0     1455 2023-04-08 20:03:06.980181 windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     3533 2023-04-08 20:03:06.964181 windmill_api-1.86.0/windmill_api/models/get_resource_response_200.py
+-rw-r--r--   0        0        0     1268 2023-04-08 20:03:06.984182 windmill_api-1.86.0/windmill_api/models/get_resource_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2335 2023-04-08 20:03:07.016182 windmill_api-1.86.0/windmill_api/models/get_resource_type_response_200.py
+-rw-r--r--   0        0        0     1840 2023-04-08 20:03:07.012182 windmill_api-1.86.0/windmill_api/models/get_resume_urls_response_200.py
+-rw-r--r--   0        0        0     4325 2023-04-08 20:03:07.072183 windmill_api-1.86.0/windmill_api/models/get_schedule_response_200.py
+-rw-r--r--   0        0        0     1232 2023-04-08 20:03:07.036182 windmill_api-1.86.0/windmill_api/models/get_schedule_response_200_args.py
+-rw-r--r--   0        0        0     1268 2023-04-08 20:03:07.056183 windmill_api-1.86.0/windmill_api/models/get_schedule_response_200_extra_perms.py
+-rw-r--r--   0        0        0     6775 2023-04-08 20:03:07.140184 windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200.py
+-rw-r--r--   0        0        0     1294 2023-04-08 20:03:07.092183 windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-04-08 20:02:53.731945 windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-04-08 20:02:53.247937 windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-04-08 20:03:07.116184 windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200_schema.py
+-rw-r--r--   0        0        0     6775 2023-04-08 20:03:07.268187 windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200.py
+-rw-r--r--   0        0        0     1294 2023-04-08 20:03:07.160185 windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-04-08 20:02:53.547942 windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200_kind.py
+-rw-r--r--   0        0        0      213 2023-04-08 20:02:54.027950 windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200_language.py
+-rw-r--r--   0        0        0     1268 2023-04-08 20:03:07.180185 windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200_schema.py
+-rw-r--r--   0        0        0     1922 2023-04-08 20:03:07.212185 windmill_api-1.86.0/windmill_api/models/get_script_deployment_status_response_200.py
+-rw-r--r--   0        0        0     4157 2023-04-08 20:03:07.264186 windmill_api-1.86.0/windmill_api/models/get_settings_response_200.py
+-rw-r--r--   0        0        0     2428 2023-04-08 20:03:07.296187 windmill_api-1.86.0/windmill_api/models/get_suspended_job_flow_response_200.py
+-rw-r--r--   0        0        0     1764 2023-04-08 20:03:07.292187 windmill_api-1.86.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py
+-rw-r--r--   0        0        0     2040 2023-04-08 20:03:07.324188 windmill_api-1.86.0/windmill_api/models/get_suspended_job_flow_response_200_job.py
+-rw-r--r--   0        0        0      204 2023-04-08 20:02:53.247937 windmill_api-1.86.0/windmill_api/models/get_suspended_job_flow_response_200_job_type.py
+-rw-r--r--   0        0        0     4554 2023-04-08 20:03:07.420189 windmill_api-1.86.0/windmill_api/models/get_variable_response_200.py
+-rw-r--r--   0        0        0     1268 2023-04-08 20:03:07.344188 windmill_api-1.86.0/windmill_api/models/get_variable_response_200_extra_perms.py
+-rw-r--r--   0        0        0     2647 2023-04-08 20:03:07.384189 windmill_api-1.86.0/windmill_api/models/global_user_info.py
+-rw-r--r--   0        0        0      176 2023-04-08 20:02:53.275937 windmill_api-1.86.0/windmill_api/models/global_user_info_login_type.py
+-rw-r--r--   0        0        0     1627 2023-04-08 20:03:07.412189 windmill_api-1.86.0/windmill_api/models/global_user_update_json_body.py
+-rw-r--r--   0        0        0     2741 2023-04-08 20:03:07.448190 windmill_api-1.86.0/windmill_api/models/global_whoami_response_200.py
+-rw-r--r--   0        0        0      185 2023-04-08 20:02:53.203936 windmill_api-1.86.0/windmill_api/models/global_whoami_response_200_login_type.py
+-rw-r--r--   0        0        0     2903 2023-04-08 20:03:07.460190 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5478 2023-04-08 20:03:07.512191 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      324 2023-04-08 20:02:53.475941 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1598 2023-04-08 20:03:07.488191 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1663 2023-04-08 20:03:07.512191 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2151 2023-04-08 20:03:07.540192 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3257 2023-04-08 20:03:07.548192 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      342 2023-04-08 20:02:53.843947 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1631 2023-04-08 20:03:07.564192 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3100 2023-04-08 20:03:07.584192 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      333 2023-04-08 20:02:53.851947 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1580 2023-04-08 20:03:07.588192 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-08 20:02:53.187935 windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0     2722 2023-04-08 20:03:07.628193 windmill_api-1.86.0/windmill_api/models/group.py
+-rw-r--r--   0        0        0     1174 2023-04-08 20:03:07.608193 windmill_api-1.86.0/windmill_api/models/group_extra_perms.py
+-rw-r--r--   0        0        0     1689 2023-04-08 20:03:07.640193 windmill_api-1.86.0/windmill_api/models/identity.py
+-rw-r--r--   0        0        0      143 2023-04-08 20:02:53.819947 windmill_api-1.86.0/windmill_api/models/identity_type.py
+-rw-r--r--   0        0        0     1820 2023-04-08 20:03:07.656194 windmill_api-1.86.0/windmill_api/models/input_transform_type_0.py
+-rw-r--r--   0        0        0      158 2023-04-08 20:02:53.707945 windmill_api-1.86.0/windmill_api/models/input_transform_type_0_type.py
+-rw-r--r--   0        0        0     1687 2023-04-08 20:03:07.668194 windmill_api-1.86.0/windmill_api/models/input_transform_type_1.py
+-rw-r--r--   0        0        0      158 2023-04-08 20:02:53.607943 windmill_api-1.86.0/windmill_api/models/input_transform_type_1_type.py
+-rw-r--r--   0        0        0     1773 2023-04-08 20:03:07.684194 windmill_api-1.86.0/windmill_api/models/invite_user_json_body.py
+-rw-r--r--   0        0        0     1679 2023-04-08 20:03:07.696194 windmill_api-1.86.0/windmill_api/models/javascript_transform.py
+-rw-r--r--   0        0        0      158 2023-04-08 20:02:54.167953 windmill_api-1.86.0/windmill_api/models/javascript_transform_type.py
+-rw-r--r--   0        0        0     1686 2023-04-08 20:03:07.716195 windmill_api-1.86.0/windmill_api/models/job.py
+-rw-r--r--   0        0        0      174 2023-04-08 20:02:53.531942 windmill_api-1.86.0/windmill_api/models/job_type.py
+-rw-r--r--   0        0        0     3583 2023-04-08 20:03:07.804196 windmill_api-1.86.0/windmill_api/models/list_apps_response_200_item.py
+-rw-r--r--   0        0        0      219 2023-04-08 20:02:53.315938 windmill_api-1.86.0/windmill_api/models/list_apps_response_200_item_execution_mode.py
+-rw-r--r--   0        0        0     1276 2023-04-08 20:03:07.780196 windmill_api-1.86.0/windmill_api/models/list_apps_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      218 2023-04-08 20:02:53.439940 windmill_api-1.86.0/windmill_api/models/list_audit_logs_action_kind.py
+-rw-r--r--   0        0        0     3896 2023-04-08 20:03:07.832197 windmill_api-1.86.0/windmill_api/models/list_audit_logs_response_200_item.py
+-rw-r--r--   0        0        0      237 2023-04-08 20:02:53.875948 windmill_api-1.86.0/windmill_api/models/list_audit_logs_response_200_item_action_kind.py
+-rw-r--r--   0        0        0      640 2023-04-08 20:02:53.871948 windmill_api-1.86.0/windmill_api/models/list_audit_logs_response_200_item_operation.py
+-rw-r--r--   0        0        0     1298 2023-04-08 20:03:07.828197 windmill_api-1.86.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py
+-rw-r--r--   0        0        0    11088 2023-04-08 20:03:07.956199 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item.py
+-rw-r--r--   0        0        0     1288 2023-04-08 20:03:07.852197 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_args.py
+-rw-r--r--   0        0        0     3736 2023-04-08 20:03:07.896198 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7579 2023-04-08 20:03:07.980199 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1901 2023-04-08 20:03:07.980199 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2352 2023-04-08 20:03:08.008200 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      222 2023-04-08 20:02:53.355939 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1806 2023-04-08 20:03:08.008200 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2342 2023-04-08 20:03:08.044201 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      380 2023-04-08 20:02:53.479941 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     7160 2023-04-08 20:03:08.092201 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1891 2023-04-08 20:03:08.068201 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2332 2023-04-08 20:03:08.092201 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      220 2023-04-08 20:02:53.743945 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1796 2023-04-08 20:03:08.188203 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2332 2023-04-08 20:03:08.188203 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      378 2023-04-08 20:02:54.143952 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2152 2023-04-08 20:03:08.220204 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      330 2023-04-08 20:02:53.203936 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      219 2023-04-08 20:02:53.483941 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_language.py
+-rw-r--r--   0        0        0     3485 2023-04-08 20:03:08.236204 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7593 2023-04-08 20:03:08.300205 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3498 2023-04-08 20:03:08.276205 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     2041 2023-04-08 20:03:08.304205 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2345 2023-04-08 20:03:08.332206 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2295 2023-04-08 20:03:08.336206 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      201 2023-04-08 20:02:54.035951 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2162 2023-04-08 20:03:08.360206 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      201 2023-04-08 20:02:53.559942 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2034 2023-04-08 20:03:08.364206 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2085 2023-04-08 20:03:08.388207 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7471 2023-04-08 20:03:08.444208 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3464 2023-04-08 20:03:08.428207 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     2031 2023-04-08 20:03:08.456208 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2335 2023-04-08 20:03:08.476208 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2275 2023-04-08 20:03:08.484208 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      199 2023-04-08 20:02:53.775946 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2142 2023-04-08 20:03:08.504209 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      199 2023-04-08 20:02:53.863947 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     2024 2023-04-08 20:03:08.516209 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2075 2023-04-08 20:03:08.576210 windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     1865 2023-04-08 20:03:08.540209 windmill_api-1.86.0/windmill_api/models/list_contextual_variables_response_200_item.py
+-rw-r--r--   0        0        0     5077 2023-04-08 20:03:08.656211 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item.py
+-rw-r--r--   0        0        0     1278 2023-04-08 20:03:08.592210 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     1255 2023-04-08 20:03:08.616211 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_schema.py
+-rw-r--r--   0        0        0     3297 2023-04-08 20:03:08.656211 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value.py
+-rw-r--r--   0        0        0     7151 2023-04-08 20:03:08.736213 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py
+-rw-r--r--   0        0        0     3318 2023-04-08 20:03:08.696212 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1985 2023-04-08 20:03:08.724213 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2289 2023-04-08 20:03:08.756213 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2187 2023-04-08 20:03:08.768214 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-04-08 20:02:53.123934 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2054 2023-04-08 20:03:08.780214 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-04-08 20:02:53.403939 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1978 2023-04-08 20:03:08.796214 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2029 2023-04-08 20:03:08.808214 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     7049 2023-04-08 20:03:08.876216 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py
+-rw-r--r--   0        0        0     3284 2023-04-08 20:03:08.844215 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1975 2023-04-08 20:03:08.872215 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-04-08 20:03:08.904216 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-04-08 20:03:08.904216 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-04-08 20:02:53.939949 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-04-08 20:03:08.988217 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-04-08 20:02:54.051951 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-04-08 20:03:08.976217 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-04-08 20:03:09.008218 windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2074 2023-04-08 20:03:09.016218 windmill_api-1.86.0/windmill_api/models/list_folders_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-04-08 20:03:09.028218 windmill_api-1.86.0/windmill_api/models/list_folders_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2958 2023-04-08 20:03:09.056219 windmill_api-1.86.0/windmill_api/models/list_groups_response_200_item.py
+-rw-r--r--   0        0        0     1286 2023-04-08 20:03:09.044219 windmill_api-1.86.0/windmill_api/models/list_groups_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2076 2023-04-08 20:03:09.076219 windmill_api-1.86.0/windmill_api/models/list_hub_apps_response_200.py
+-rw-r--r--   0        0        0     2304 2023-04-08 20:03:09.092219 windmill_api-1.86.0/windmill_api/models/list_hub_apps_response_200_apps_item.py
+-rw-r--r--   0        0        0     2116 2023-04-08 20:03:09.108220 windmill_api-1.86.0/windmill_api/models/list_hub_flows_response_200.py
+-rw-r--r--   0        0        0     2324 2023-04-08 20:03:09.124220 windmill_api-1.86.0/windmill_api/models/list_hub_flows_response_200_flows_item.py
+-rw-r--r--   0        0        0     2106 2023-04-08 20:03:09.140220 windmill_api-1.86.0/windmill_api/models/list_hub_scripts_response_200.py
+-rw-r--r--   0        0        0     2790 2023-04-08 20:03:09.164221 windmill_api-1.86.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py
+-rw-r--r--   0        0        0      262 2023-04-08 20:02:53.691944 windmill_api-1.86.0/windmill_api/models/list_hub_scripts_response_200_asks_item_kind.py
+-rw-r--r--   0        0        0     1922 2023-04-08 20:03:09.176221 windmill_api-1.86.0/windmill_api/models/list_jobs_response_200_item.py
+-rw-r--r--   0        0        0      194 2023-04-08 20:02:53.327938 windmill_api-1.86.0/windmill_api/models/list_jobs_response_200_item_type.py
+-rw-r--r--   0        0        0     2076 2023-04-08 20:03:09.192221 windmill_api-1.86.0/windmill_api/models/list_pending_invites_response_200_item.py
+-rw-r--r--   0        0        0    11982 2023-04-08 20:03:09.368224 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item.py
+-rw-r--r--   0        0        0     1245 2023-04-08 20:03:09.212221 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_args.py
+-rw-r--r--   0        0        0     3544 2023-04-08 20:03:09.256222 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status.py
+-rw-r--r--   0        0        0     7247 2023-04-08 20:03:09.336224 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1858 2023-04-08 20:03:09.420225 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2268 2023-04-08 20:03:09.400225 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      214 2023-04-08 20:02:53.967949 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1763 2023-04-08 20:03:09.428225 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2299 2023-04-08 20:03:09.452226 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      372 2023-04-08 20:02:53.323938 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6858 2023-04-08 20:03:09.512227 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1848 2023-04-08 20:03:09.476226 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2248 2023-04-08 20:03:09.504227 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      212 2023-04-08 20:02:53.327938 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1753 2023-04-08 20:03:09.532227 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2289 2023-04-08 20:03:09.544227 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      370 2023-04-08 20:02:53.975950 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2109 2023-04-08 20:03:09.564228 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py
+-rw-r--r--   0        0        0      322 2023-04-08 20:02:53.115934 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_job_kind.py
+-rw-r--r--   0        0        0      211 2023-04-08 20:02:53.723945 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_language.py
+-rw-r--r--   0        0        0     3334 2023-04-08 20:03:09.588228 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow.py
+-rw-r--r--   0        0        0     7235 2023-04-08 20:03:09.644229 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3357 2023-04-08 20:03:09.624229 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1998 2023-04-08 20:03:09.652229 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2302 2023-04-08 20:03:09.676230 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2211 2023-04-08 20:03:09.680230 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      193 2023-04-08 20:02:53.687945 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2078 2023-04-08 20:03:09.708231 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      193 2023-04-08 20:02:53.911949 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1991 2023-04-08 20:03:09.760231 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2042 2023-04-08 20:03:09.736231 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     7159 2023-04-08 20:03:09.876233 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3323 2023-04-08 20:03:09.796232 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1988 2023-04-08 20:03:09.824233 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2292 2023-04-08 20:03:09.856233 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2191 2023-04-08 20:03:09.888234 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      191 2023-04-08 20:02:53.115934 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2058 2023-04-08 20:03:09.904234 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      191 2023-04-08 20:02:53.527942 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1981 2023-04-08 20:03:09.916234 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2032 2023-04-08 20:03:09.932235 windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     4884 2023-04-08 20:03:09.980235 windmill_api-1.86.0/windmill_api/models/list_resource_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-04-08 20:03:09.952235 windmill_api-1.86.0/windmill_api/models/list_resource_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2363 2023-04-08 20:03:09.984235 windmill_api-1.86.0/windmill_api/models/list_resource_type_response_200_item.py
+-rw-r--r--   0        0        0     4426 2023-04-08 20:03:10.036236 windmill_api-1.86.0/windmill_api/models/list_schedules_response_200_item.py
+-rw-r--r--   0        0        0     1265 2023-04-08 20:03:10.004236 windmill_api-1.86.0/windmill_api/models/list_schedules_response_200_item_args.py
+-rw-r--r--   0        0        0     1301 2023-04-08 20:03:10.020236 windmill_api-1.86.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     6768 2023-04-08 20:03:10.104238 windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item.py
+-rw-r--r--   0        0        0     1291 2023-04-08 20:03:10.056237 windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0      255 2023-04-08 20:02:53.851947 windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item_kind.py
+-rw-r--r--   0        0        0      213 2023-04-08 20:02:53.279937 windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item_language.py
+-rw-r--r--   0        0        0     1265 2023-04-08 20:03:10.080237 windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item_schema.py
+-rw-r--r--   0        0        0     2985 2023-04-08 20:03:10.168239 windmill_api-1.86.0/windmill_api/models/list_tokens_response_200_item.py
+-rw-r--r--   0        0        0     2250 2023-04-08 20:03:10.132238 windmill_api-1.86.0/windmill_api/models/list_user_workspaces_response_200.py
+-rw-r--r--   0        0        0     1833 2023-04-08 20:03:10.160239 windmill_api-1.86.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py
+-rw-r--r--   0        0        0     2896 2023-04-08 20:03:10.196239 windmill_api-1.86.0/windmill_api/models/list_users_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0      198 2023-04-08 20:02:53.583943 windmill_api-1.86.0/windmill_api/models/list_users_as_super_admin_response_200_item_login_type.py
+-rw-r--r--   0        0        0     4035 2023-04-08 20:03:10.228240 windmill_api-1.86.0/windmill_api/models/list_users_response_200_item.py
+-rw-r--r--   0        0        0     1613 2023-04-08 20:03:10.292241 windmill_api-1.86.0/windmill_api/models/list_users_response_200_item_usage.py
+-rw-r--r--   0        0        0     4608 2023-04-08 20:03:10.288241 windmill_api-1.86.0/windmill_api/models/list_variable_response_200_item.py
+-rw-r--r--   0        0        0     1296 2023-04-08 20:03:10.308241 windmill_api-1.86.0/windmill_api/models/list_variable_response_200_item_extra_perms.py
+-rw-r--r--   0        0        0     2693 2023-04-08 20:03:10.328242 windmill_api-1.86.0/windmill_api/models/list_workers_response_200_item.py
+-rw-r--r--   0        0        0     2086 2023-04-08 20:03:10.340242 windmill_api-1.86.0/windmill_api/models/list_workspace_invites_response_200_item.py
+-rw-r--r--   0        0        0     2082 2023-04-08 20:03:10.360242 windmill_api-1.86.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py
+-rw-r--r--   0        0        0     2013 2023-04-08 20:03:10.372243 windmill_api-1.86.0/windmill_api/models/list_workspaces_response_200_item.py
+-rw-r--r--   0        0        0     3388 2023-04-08 20:03:10.404243 windmill_api-1.86.0/windmill_api/models/listable_app.py
+-rw-r--r--   0        0        0      207 2023-04-08 20:02:53.115934 windmill_api-1.86.0/windmill_api/models/listable_app_execution_mode.py
+-rw-r--r--   0        0        0     1207 2023-04-08 20:03:10.392243 windmill_api-1.86.0/windmill_api/models/listable_app_extra_perms.py
+-rw-r--r--   0        0        0     4751 2023-04-08 20:03:10.456244 windmill_api-1.86.0/windmill_api/models/listable_resource.py
+-rw-r--r--   0        0        0     1232 2023-04-08 20:03:10.424243 windmill_api-1.86.0/windmill_api/models/listable_resource_extra_perms.py
+-rw-r--r--   0        0        0     4486 2023-04-08 20:03:10.484244 windmill_api-1.86.0/windmill_api/models/listable_variable.py
+-rw-r--r--   0        0        0     1232 2023-04-08 20:03:10.476244 windmill_api-1.86.0/windmill_api/models/listable_variable_extra_perms.py
+-rw-r--r--   0        0        0     1513 2023-04-08 20:03:10.544246 windmill_api-1.86.0/windmill_api/models/login.py
+-rw-r--r--   0        0        0     1559 2023-04-08 20:03:10.508245 windmill_api-1.86.0/windmill_api/models/login_json_body.py
+-rw-r--r--   0        0        0     1739 2023-04-08 20:03:10.536245 windmill_api-1.86.0/windmill_api/models/login_with_oauth_json_body.py
+-rw-r--r--   0        0        0     2758 2023-04-08 20:03:10.576246 windmill_api-1.86.0/windmill_api/models/main_arg_signature.py
+-rw-r--r--   0        0        0     5099 2023-04-08 20:03:10.604247 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item.py
+-rw-r--r--   0        0        0      315 2023-04-08 20:02:54.071951 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1547 2023-04-08 20:03:10.600247 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1612 2023-04-08 20:03:10.624247 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2044 2023-04-08 20:03:10.628247 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3049 2023-04-08 20:03:10.660248 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      333 2023-04-08 20:02:53.179935 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1580 2023-04-08 20:03:10.652248 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     2862 2023-04-08 20:03:10.688248 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      324 2023-04-08 20:02:53.983950 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1529 2023-04-08 20:03:10.684248 windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      169 2023-04-08 20:02:54.103952 windmill_api-1.86.0/windmill_api/models/main_arg_signature_type.py
+-rw-r--r--   0        0        0     2662 2023-04-08 20:03:10.724249 windmill_api-1.86.0/windmill_api/models/new_schedule.py
+-rw-r--r--   0        0        0     1171 2023-04-08 20:03:10.708248 windmill_api-1.86.0/windmill_api/models/new_schedule_args.py
+-rw-r--r--   0        0        0     2108 2023-04-08 20:03:10.744249 windmill_api-1.86.0/windmill_api/models/new_token.py
+-rw-r--r--   0        0        0     2473 2023-04-08 20:03:10.828251 windmill_api-1.86.0/windmill_api/models/new_token_impersonate.py
+-rw-r--r--   0        0        0     1710 2023-04-08 20:03:10.772250 windmill_api-1.86.0/windmill_api/models/new_user.py
+-rw-r--r--   0        0        0     2584 2023-04-08 20:03:10.808250 windmill_api-1.86.0/windmill_api/models/open_flow.py
+-rw-r--r--   0        0        0     1166 2023-04-08 20:03:10.832251 windmill_api-1.86.0/windmill_api/models/open_flow_schema.py
+-rw-r--r--   0        0        0     3026 2023-04-08 20:03:10.868251 windmill_api-1.86.0/windmill_api/models/open_flow_value.py
+-rw-r--r--   0        0        0     6384 2023-04-08 20:03:10.956253 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module.py
+-rw-r--r--   0        0        0     3013 2023-04-08 20:03:10.904252 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1896 2023-04-08 20:03:10.932253 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2200 2023-04-08 20:03:10.968253 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2006 2023-04-08 20:03:10.984253 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      175 2023-04-08 20:02:53.703945 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1873 2023-04-08 20:03:10.996254 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      175 2023-04-08 20:02:54.003950 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1889 2023-04-08 20:03:11.012254 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1940 2023-04-08 20:03:11.024254 windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6308 2023-04-08 20:03:11.092255 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item.py
+-rw-r--r--   0        0        0     2979 2023-04-08 20:03:11.064255 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1886 2023-04-08 20:03:11.092255 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2190 2023-04-08 20:03:11.124256 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     1986 2023-04-08 20:03:11.120256 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      173 2023-04-08 20:02:53.463940 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1853 2023-04-08 20:03:11.148256 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      173 2023-04-08 20:02:54.139953 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1879 2023-04-08 20:03:11.152256 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1930 2023-04-08 20:03:11.176257 windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     2816 2023-04-08 20:03:11.192257 windmill_api-1.86.0/windmill_api/models/open_flow_w_path.py
+-rw-r--r--   0        0        0     1197 2023-04-08 20:03:11.196257 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_schema.py
+-rw-r--r--   0        0        0     3116 2023-04-08 20:03:11.236258 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value.py
+-rw-r--r--   0        0        0     6590 2023-04-08 20:03:11.276258 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module.py
+-rw-r--r--   0        0        0     3117 2023-04-08 20:03:11.272258 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1927 2023-04-08 20:03:11.376260 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2231 2023-04-08 20:03:11.372260 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2073 2023-04-08 20:03:11.400261 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      180 2023-04-08 20:02:53.743945 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1940 2023-04-08 20:03:11.404260 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      180 2023-04-08 20:02:53.359938 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1920 2023-04-08 20:03:11.432261 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1971 2023-04-08 20:03:11.436261 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6514 2023-04-08 20:03:11.512262 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item.py
+-rw-r--r--   0        0        0     3074 2023-04-08 20:03:11.472262 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1917 2023-04-08 20:03:11.500262 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2221 2023-04-08 20:03:11.532263 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2044 2023-04-08 20:03:11.540263 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-04-08 20:02:54.011950 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1911 2023-04-08 20:03:11.560263 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-08 20:02:53.159935 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1910 2023-04-08 20:03:11.568263 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1961 2023-04-08 20:03:11.588264 windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1989 2023-04-08 20:03:11.596264 windmill_api-1.86.0/windmill_api/models/path_flow.py
+-rw-r--r--   0        0        0     3089 2023-04-08 20:03:11.624264 windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms.py
+-rw-r--r--   0        0        0     2115 2023-04-08 20:03:11.624264 windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      185 2023-04-08 20:02:53.795946 windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1982 2023-04-08 20:03:11.652265 windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      185 2023-04-08 20:02:53.731945 windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      135 2023-04-08 20:02:53.427940 windmill_api-1.86.0/windmill_api/models/path_flow_type.py
+-rw-r--r--   0        0        0     2292 2023-04-08 20:03:11.664265 windmill_api-1.86.0/windmill_api/models/path_script.py
+-rw-r--r--   0        0        0     3181 2023-04-08 20:03:11.688265 windmill_api-1.86.0/windmill_api/models/path_script_input_transforms.py
+-rw-r--r--   0        0        0     2135 2023-04-08 20:03:11.692266 windmill_api-1.86.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      187 2023-04-08 20:02:53.403939 windmill_api-1.86.0/windmill_api/models/path_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     2002 2023-04-08 20:03:11.792267 windmill_api-1.86.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      187 2023-04-08 20:02:53.247937 windmill_api-1.86.0/windmill_api/models/path_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      141 2023-04-08 20:02:53.475941 windmill_api-1.86.0/windmill_api/models/path_script_type.py
+-rw-r--r--   0        0        0     3390 2023-04-08 20:03:11.744266 windmill_api-1.86.0/windmill_api/models/policy.py
+-rw-r--r--   0        0        0      202 2023-04-08 20:02:53.527942 windmill_api-1.86.0/windmill_api/models/policy_execution_mode.py
+-rw-r--r--   0        0        0     1709 2023-04-08 20:03:11.768267 windmill_api-1.86.0/windmill_api/models/policy_triggerables.py
+-rw-r--r--   0        0        0     1279 2023-04-08 20:03:11.788267 windmill_api-1.86.0/windmill_api/models/policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2147 2023-04-08 20:03:11.824268 windmill_api-1.86.0/windmill_api/models/preview.py
+-rw-r--r--   0        0        0     1148 2023-04-08 20:03:11.812268 windmill_api-1.86.0/windmill_api/models/preview_args.py
+-rw-r--r--   0        0        0      194 2023-04-08 20:02:53.339938 windmill_api-1.86.0/windmill_api/models/preview_language.py
+-rw-r--r--   0        0        0     1642 2023-04-08 20:03:11.840268 windmill_api-1.86.0/windmill_api/models/preview_schedule_json_body.py
+-rw-r--r--   0        0        0     2963 2023-04-08 20:03:11.860268 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200.py
+-rw-r--r--   0        0        0     5679 2023-04-08 20:03:11.900269 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py
+-rw-r--r--   0        0        0      328 2023-04-08 20:02:54.015950 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_0.py
+-rw-r--r--   0        0        0     1618 2023-04-08 20:03:11.888269 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py
+-rw-r--r--   0        0        0     1683 2023-04-08 20:03:11.912269 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py
+-rw-r--r--   0        0        0     2191 2023-04-08 20:03:11.928270 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py
+-rw-r--r--   0        0        0     3329 2023-04-08 20:03:11.948270 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py
+-rw-r--r--   0        0        0      346 2023-04-08 20:02:53.391939 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_0.py
+-rw-r--r--   0        0        0     1651 2023-04-08 20:03:11.952270 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py
+-rw-r--r--   0        0        0     3214 2023-04-08 20:03:12.052272 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py
+-rw-r--r--   0        0        0      337 2023-04-08 20:02:53.111934 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_0.py
+-rw-r--r--   0        0        0     1600 2023-04-08 20:03:11.976271 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py
+-rw-r--r--   0        0        0      182 2023-04-08 20:02:53.947949 windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_type.py
+-rw-r--r--   0        0        0    11448 2023-04-08 20:03:12.200274 windmill_api-1.86.0/windmill_api/models/queued_job.py
+-rw-r--r--   0        0        0     1161 2023-04-08 20:03:12.072272 windmill_api-1.86.0/windmill_api/models/queued_job_args.py
+-rw-r--r--   0        0        0     3202 2023-04-08 20:03:12.112273 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status.py
+-rw-r--r--   0        0        0     6683 2023-04-08 20:03:12.196274 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module.py
+-rw-r--r--   0        0        0     1774 2023-04-08 20:03:12.220275 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py
+-rw-r--r--   0        0        0     2106 2023-04-08 20:03:12.228275 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py
+-rw-r--r--   0        0        0      199 2023-04-08 20:02:53.523942 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen_type.py
+-rw-r--r--   0        0        0     1679 2023-04-08 20:03:12.244275 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py
+-rw-r--r--   0        0        0     2215 2023-04-08 20:03:12.264275 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py
+-rw-r--r--   0        0        0      357 2023-04-08 20:02:53.495941 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_type.py
+-rw-r--r--   0        0        0     6294 2023-04-08 20:03:12.324277 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item.py
+-rw-r--r--   0        0        0     1764 2023-04-08 20:03:12.288276 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py
+-rw-r--r--   0        0        0     2086 2023-04-08 20:03:12.316276 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py
+-rw-r--r--   0        0        0      197 2023-04-08 20:02:53.595943 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen_type.py
+-rw-r--r--   0        0        0     1669 2023-04-08 20:03:12.344277 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py
+-rw-r--r--   0        0        0     2205 2023-04-08 20:03:12.356277 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py
+-rw-r--r--   0        0        0      355 2023-04-08 20:02:53.535942 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_type.py
+-rw-r--r--   0        0        0     2025 2023-04-08 20:03:12.380277 windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_retry.py
+-rw-r--r--   0        0        0      307 2023-04-08 20:02:53.107934 windmill_api-1.86.0/windmill_api/models/queued_job_job_kind.py
+-rw-r--r--   0        0        0      196 2023-04-08 20:02:53.999950 windmill_api-1.86.0/windmill_api/models/queued_job_language.py
+-rw-r--r--   0        0        0     3079 2023-04-08 20:03:12.476279 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow.py
+-rw-r--r--   0        0        0     6506 2023-04-08 20:03:12.460279 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module.py
+-rw-r--r--   0        0        0     3069 2023-04-08 20:03:12.500280 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py
+-rw-r--r--   0        0        0     1914 2023-04-08 20:03:12.504279 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2218 2023-04-08 20:03:12.572281 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2040 2023-04-08 20:03:12.532280 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      178 2023-04-08 20:02:53.651944 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1907 2023-04-08 20:03:12.556280 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      178 2023-04-08 20:02:53.667944 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1907 2023-04-08 20:03:12.592281 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1958 2023-04-08 20:03:12.596281 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py
+-rw-r--r--   0        0        0     6430 2023-04-08 20:03:12.668282 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item.py
+-rw-r--r--   0        0        0     3035 2023-04-08 20:03:12.708283 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py
+-rw-r--r--   0        0        0     1904 2023-04-08 20:03:12.696283 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2208 2023-04-08 20:03:12.728284 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2020 2023-04-08 20:03:12.736284 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      176 2023-04-08 20:02:53.599943 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1887 2023-04-08 20:03:12.756284 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      176 2023-04-08 20:02:53.219936 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1897 2023-04-08 20:03:12.764284 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1948 2023-04-08 20:03:12.784284 windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py
+-rw-r--r--   0        0        0     2816 2023-04-08 20:03:12.804285 windmill_api-1.86.0/windmill_api/models/raw_script.py
+-rw-r--r--   0        0        0     3139 2023-04-08 20:03:12.816285 windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms.py
+-rw-r--r--   0        0        0     2125 2023-04-08 20:03:12.832285 windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py
+-rw-r--r--   0        0        0      186 2023-04-08 20:02:53.187935 windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0_type.py
+-rw-r--r--   0        0        0     1992 2023-04-08 20:03:12.844285 windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py
+-rw-r--r--   0        0        0      186 2023-04-08 20:02:54.143952 windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1_type.py
+-rw-r--r--   0        0        0      196 2023-04-08 20:02:53.311938 windmill_api-1.86.0/windmill_api/models/raw_script_language.py
+-rw-r--r--   0        0        0      146 2023-04-08 20:02:53.927949 windmill_api-1.86.0/windmill_api/models/raw_script_type.py
+-rw-r--r--   0        0        0     1405 2023-04-08 20:03:12.860286 windmill_api-1.86.0/windmill_api/models/refresh_token_json_body.py
+-rw-r--r--   0        0        0     1448 2023-04-08 20:03:12.868286 windmill_api-1.86.0/windmill_api/models/remove_granular_acls_json_body.py
+-rw-r--r--   0        0        0      304 2023-04-08 20:02:54.099952 windmill_api-1.86.0/windmill_api/models/remove_granular_acls_kind.py
+-rw-r--r--   0        0        0     1544 2023-04-08 20:03:12.888286 windmill_api-1.86.0/windmill_api/models/remove_owner_to_folder_json_body.py
+-rw-r--r--   0        0        0     1567 2023-04-08 20:03:12.968288 windmill_api-1.86.0/windmill_api/models/remove_user_to_group_json_body.py
+-rw-r--r--   0        0        0     3367 2023-04-08 20:03:12.936287 windmill_api-1.86.0/windmill_api/models/resource.py
+-rw-r--r--   0        0        0     1189 2023-04-08 20:03:12.952287 windmill_api-1.86.0/windmill_api/models/resource_extra_perms.py
+-rw-r--r--   0        0        0     2256 2023-04-08 20:03:12.988288 windmill_api-1.86.0/windmill_api/models/resource_type.py
+-rw-r--r--   0        0        0     1278 2023-04-08 20:03:12.988288 windmill_api-1.86.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py
+-rw-r--r--   0        0        0     1255 2023-04-08 20:03:13.008288 windmill_api-1.86.0/windmill_api/models/resume_suspended_job_post_json_body.py
+-rw-r--r--   0        0        0     2546 2023-04-08 20:03:13.028288 windmill_api-1.86.0/windmill_api/models/retry.py
+-rw-r--r--   0        0        0     1751 2023-04-08 20:03:13.036289 windmill_api-1.86.0/windmill_api/models/retry_constant.py
+-rw-r--r--   0        0        0     2055 2023-04-08 20:03:13.060289 windmill_api-1.86.0/windmill_api/models/retry_exponential.py
+-rw-r--r--   0        0        0     1210 2023-04-08 20:03:13.052289 windmill_api-1.86.0/windmill_api/models/run_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     2189 2023-04-08 20:03:13.084289 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body.py
+-rw-r--r--   0        0        0     1235 2023-04-08 20:03:13.080289 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_args.py
+-rw-r--r--   0        0        0     3265 2023-04-08 20:03:13.120290 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value.py
+-rw-r--r--   0        0        0     7049 2023-04-08 20:03:13.164291 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3284 2023-04-08 20:03:13.160291 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1975 2023-04-08 20:03:13.260293 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2279 2023-04-08 20:03:13.196292 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2167 2023-04-08 20:03:13.224292 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      189 2023-04-08 20:02:53.887948 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2034 2023-04-08 20:03:13.252292 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      189 2023-04-08 20:02:53.607943 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1968 2023-04-08 20:03:13.280293 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     2019 2023-04-08 20:03:13.288293 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6939 2023-04-08 20:03:13.360294 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3250 2023-04-08 20:03:13.328294 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1965 2023-04-08 20:03:13.356294 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2269 2023-04-08 20:03:13.388295 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2147 2023-04-08 20:03:13.388295 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      187 2023-04-08 20:02:53.259937 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     2014 2023-04-08 20:03:13.484296 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      187 2023-04-08 20:02:53.999950 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1958 2023-04-08 20:03:13.416295 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     2009 2023-04-08 20:03:13.444296 windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1220 2023-04-08 20:03:13.464296 windmill_api-1.86.0/windmill_api/models/run_script_by_hash_json_body.py
+-rw-r--r--   0        0        0     1220 2023-04-08 20:03:13.484296 windmill_api-1.86.0/windmill_api/models/run_script_by_path_json_body.py
+-rw-r--r--   0        0        0     2422 2023-04-08 20:03:13.516297 windmill_api-1.86.0/windmill_api/models/run_script_preview_json_body.py
+-rw-r--r--   0        0        0     1245 2023-04-08 20:03:13.504297 windmill_api-1.86.0/windmill_api/models/run_script_preview_json_body_args.py
+-rw-r--r--   0        0        0      211 2023-04-08 20:02:53.475941 windmill_api-1.86.0/windmill_api/models/run_script_preview_json_body_language.py
+-rw-r--r--   0        0        0     1266 2023-04-08 20:03:13.524297 windmill_api-1.86.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py
+-rw-r--r--   0        0        0     1276 2023-04-08 20:03:13.540297 windmill_api-1.86.0/windmill_api/models/run_wait_result_script_by_path_json_body.py
+-rw-r--r--   0        0        0     4086 2023-04-08 20:03:13.584298 windmill_api-1.86.0/windmill_api/models/schedule.py
+-rw-r--r--   0        0        0     1153 2023-04-08 20:03:13.560298 windmill_api-1.86.0/windmill_api/models/schedule_args.py
+-rw-r--r--   0        0        0     1189 2023-04-08 20:03:13.580298 windmill_api-1.86.0/windmill_api/models/schedule_extra_perms.py
+-rw-r--r--   0        0        0     6220 2023-04-08 20:03:13.660299 windmill_api-1.86.0/windmill_api/models/script.py
+-rw-r--r--   0        0        0     1143 2023-04-08 20:03:13.600299 windmill_api-1.86.0/windmill_api/models/script_args.py
+-rw-r--r--   0        0        0     1179 2023-04-08 20:03:13.620299 windmill_api-1.86.0/windmill_api/models/script_extra_perms.py
+-rw-r--r--   0        0        0      235 2023-04-08 20:02:53.255937 windmill_api-1.86.0/windmill_api/models/script_kind.py
+-rw-r--r--   0        0        0      193 2023-04-08 20:02:53.571942 windmill_api-1.86.0/windmill_api/models/script_language.py
+-rw-r--r--   0        0        0     1153 2023-04-08 20:03:13.644299 windmill_api-1.86.0/windmill_api/models/script_schema.py
+-rw-r--r--   0        0        0     1440 2023-04-08 20:03:13.664300 windmill_api-1.86.0/windmill_api/models/set_password_json_body.py
+-rw-r--r--   0        0        0     1470 2023-04-08 20:03:13.680300 windmill_api-1.86.0/windmill_api/models/set_schedule_enabled_json_body.py
+-rw-r--r--   0        0        0     2032 2023-04-08 20:03:13.696300 windmill_api-1.86.0/windmill_api/models/slack_token.py
+-rw-r--r--   0        0        0     1586 2023-04-08 20:03:13.704300 windmill_api-1.86.0/windmill_api/models/slack_token_bot.py
+-rw-r--r--   0        0        0     2227 2023-04-08 20:03:13.728301 windmill_api-1.86.0/windmill_api/models/star_json_body.py
+-rw-r--r--   0        0        0      185 2023-04-08 20:02:53.731945 windmill_api-1.86.0/windmill_api/models/star_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     1772 2023-04-08 20:03:13.736301 windmill_api-1.86.0/windmill_api/models/static_transform.py
+-rw-r--r--   0        0        0      154 2023-04-08 20:02:53.127935 windmill_api-1.86.0/windmill_api/models/static_transform_type.py
+-rw-r--r--   0        0        0     2462 2023-04-08 20:03:13.768301 windmill_api-1.86.0/windmill_api/models/token_response.py
+-rw-r--r--   0        0        0     2921 2023-04-08 20:03:13.776301 windmill_api-1.86.0/windmill_api/models/truncated_token.py
+-rw-r--r--   0        0        0     2249 2023-04-08 20:03:13.800302 windmill_api-1.86.0/windmill_api/models/unstar_json_body.py
+-rw-r--r--   0        0        0      187 2023-04-08 20:02:53.439940 windmill_api-1.86.0/windmill_api/models/unstar_json_body_favorite_kind.py
+-rw-r--r--   0        0        0     2638 2023-04-08 20:03:13.820302 windmill_api-1.86.0/windmill_api/models/update_app_json_body.py
+-rw-r--r--   0        0        0     3699 2023-04-08 20:03:13.904304 windmill_api-1.86.0/windmill_api/models/update_app_json_body_policy.py
+-rw-r--r--   0        0        0      219 2023-04-08 20:02:53.507941 windmill_api-1.86.0/windmill_api/models/update_app_json_body_policy_execution_mode.py
+-rw-r--r--   0        0        0     1935 2023-04-08 20:03:13.844303 windmill_api-1.86.0/windmill_api/models/update_app_json_body_policy_triggerables.py
+-rw-r--r--   0        0        0     1376 2023-04-08 20:03:13.864303 windmill_api-1.86.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py
+-rw-r--r--   0        0        0     2896 2023-04-08 20:03:13.904304 windmill_api-1.86.0/windmill_api/models/update_flow_json_body.py
+-rw-r--r--   0        0        0     1222 2023-04-08 20:03:13.924304 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_schema.py
+-rw-r--r--   0        0        0     3196 2023-04-08 20:03:13.944304 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value.py
+-rw-r--r--   0        0        0     6855 2023-04-08 20:03:14.084307 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module.py
+-rw-r--r--   0        0        0     3211 2023-04-08 20:03:13.984305 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py
+-rw-r--r--   0        0        0     1952 2023-04-08 20:03:14.012306 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py
+-rw-r--r--   0        0        0     2256 2023-04-08 20:03:14.044306 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py
+-rw-r--r--   0        0        0     2123 2023-04-08 20:03:14.072306 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py
+-rw-r--r--   0        0        0      185 2023-04-08 20:02:54.143952 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1990 2023-04-08 20:03:14.100307 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py
+-rw-r--r--   0        0        0      185 2023-04-08 20:02:53.763946 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1945 2023-04-08 20:03:14.112307 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py
+-rw-r--r--   0        0        0     1996 2023-04-08 20:03:14.128307 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py
+-rw-r--r--   0        0        0     6739 2023-04-08 20:03:14.188309 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item.py
+-rw-r--r--   0        0        0     3177 2023-04-08 20:03:14.164308 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py
+-rw-r--r--   0        0        0     1942 2023-04-08 20:03:14.192309 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py
+-rw-r--r--   0        0        0     2246 2023-04-08 20:03:14.220309 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py
+-rw-r--r--   0        0        0     2103 2023-04-08 20:03:14.220309 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py
+-rw-r--r--   0        0        0      183 2023-04-08 20:02:53.579943 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0_type.py
+-rw-r--r--   0        0        0     1970 2023-04-08 20:03:14.248309 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py
+-rw-r--r--   0        0        0      183 2023-04-08 20:02:53.167935 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1_type.py
+-rw-r--r--   0        0        0     1935 2023-04-08 20:03:14.248309 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py
+-rw-r--r--   0        0        0     1986 2023-04-08 20:03:14.276310 windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py
+-rw-r--r--   0        0        0     1949 2023-04-08 20:03:14.280310 windmill_api-1.86.0/windmill_api/models/update_folder_json_body.py
+-rw-r--r--   0        0        0     1520 2023-04-08 20:03:14.300310 windmill_api-1.86.0/windmill_api/models/update_group_json_body.py
+-rw-r--r--   0        0        0     2036 2023-04-08 20:03:14.312311 windmill_api-1.86.0/windmill_api/models/update_resource_json_body.py
+-rw-r--r--   0        0        0     1847 2023-04-08 20:03:14.328311 windmill_api-1.86.0/windmill_api/models/update_resource_type_json_body.py
+-rw-r--r--   0        0        0     1541 2023-04-08 20:03:14.336311 windmill_api-1.86.0/windmill_api/models/update_resource_value_json_body.py
+-rw-r--r--   0        0        0     1953 2023-04-08 20:03:14.356311 windmill_api-1.86.0/windmill_api/models/update_schedule_json_body.py
+-rw-r--r--   0        0        0     1232 2023-04-08 20:03:14.356311 windmill_api-1.86.0/windmill_api/models/update_schedule_json_body_args.py
+-rw-r--r--   0        0        0     2066 2023-04-08 20:03:14.452313 windmill_api-1.86.0/windmill_api/models/update_user_json_body.py
+-rw-r--r--   0        0        0     2316 2023-04-08 20:03:14.392312 windmill_api-1.86.0/windmill_api/models/update_variable_json_body.py
+-rw-r--r--   0        0        0     1478 2023-04-08 20:03:14.412312 windmill_api-1.86.0/windmill_api/models/usage.py
+-rw-r--r--   0        0        0     3799 2023-04-08 20:03:14.556315 windmill_api-1.86.0/windmill_api/models/user.py
+-rw-r--r--   0        0        0     1501 2023-04-08 20:03:14.476313 windmill_api-1.86.0/windmill_api/models/user_usage.py
+-rw-r--r--   0        0        0     2122 2023-04-08 20:03:14.504314 windmill_api-1.86.0/windmill_api/models/user_workspace_list.py
+-rw-r--r--   0        0        0     1767 2023-04-08 20:03:14.532314 windmill_api-1.86.0/windmill_api/models/user_workspace_list_workspaces_item.py
+-rw-r--r--   0        0        0     3950 2023-04-08 20:03:14.588315 windmill_api-1.86.0/windmill_api/models/whoami_response_200.py
+-rw-r--r--   0        0        0     1572 2023-04-08 20:03:14.580315 windmill_api-1.86.0/windmill_api/models/whoami_response_200_usage.py
+-rw-r--r--   0        0        0     3939 2023-04-08 20:03:14.636316 windmill_api-1.86.0/windmill_api/models/whois_response_200.py
+-rw-r--r--   0        0        0     1567 2023-04-08 20:03:14.612316 windmill_api-1.86.0/windmill_api/models/whois_response_200_usage.py
+-rw-r--r--   0        0        0     2604 2023-04-08 20:03:14.648316 windmill_api-1.86.0/windmill_api/models/worker_ping.py
+-rw-r--r--   0        0        0     1901 2023-04-08 20:03:14.668317 windmill_api-1.86.0/windmill_api/models/workspace.py
+-rw-r--r--   0        0        0     1974 2023-04-08 20:03:14.676317 windmill_api-1.86.0/windmill_api/models/workspace_invite.py
+-rw-r--r--   0        0        0       25 2023-04-08 20:02:44.203774 windmill_api-1.86.0/windmill_api/py.typed
+-rw-r--r--   0        0        0      939 2023-04-08 20:03:14.684317 windmill_api-1.86.0/windmill_api/types.py
+-rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 windmill_api-1.86.0/setup.py
+-rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 windmill_api-1.86.0/PKG-INFO
```

### Comparing `windmill_api-1.85.0/LICENSE` & `windmill_api-1.86.0/LICENSE`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/README.md` & `windmill_api-1.86.0/README.md`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/pyproject.toml` & `windmill_api-1.86.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "windmill-api"
-version = "1.85.0"
+version = "1.86.0"
 description = "A client library for accessing Windmill API"
 license = "Apache-2.0"
 
 authors = ["Ruben Fiszel <ruben@windmill.dev>"]
 
 readme = "README.md"
 packages = [
```

### Comparing `windmill_api-1.85.0/windmill_api/api/app/create_app.py` & `windmill_api-1.86.0/windmill_api/api/app/create_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/app/delete_app.py` & `windmill_api-1.86.0/windmill_api/api/app/delete_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/app/execute_component.py` & `windmill_api-1.86.0/windmill_api/api/app/execute_component.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/app/exists_app.py` & `windmill_api-1.86.0/windmill_api/api/app/exists_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/app/get_app_by_path.py` & `windmill_api-1.86.0/windmill_api/api/app/get_app_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/app/get_app_by_version.py` & `windmill_api-1.86.0/windmill_api/api/app/get_app_by_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/app/get_hub_app_by_id.py` & `windmill_api-1.86.0/windmill_api/api/app/get_hub_app_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/app/get_public_app_by_secret.py` & `windmill_api-1.86.0/windmill_api/api/app/get_public_app_by_secret.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/app/get_public_secret_of_app.py` & `windmill_api-1.86.0/windmill_api/api/app/get_public_secret_of_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/app/list_apps.py` & `windmill_api-1.86.0/windmill_api/api/app/list_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/app/list_hub_apps.py` & `windmill_api-1.86.0/windmill_api/api/app/list_hub_apps.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/app/update_app.py` & `windmill_api-1.86.0/windmill_api/api/app/update_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/audit/get_audit_log.py` & `windmill_api-1.86.0/windmill_api/api/audit/get_audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/audit/list_audit_logs.py` & `windmill_api-1.86.0/windmill_api/api/audit/list_audit_logs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/capture/create_capture.py` & `windmill_api-1.86.0/windmill_api/api/capture/create_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/capture/get_capture.py` & `windmill_api-1.86.0/windmill_api/api/capture/get_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/capture/update_capture.py` & `windmill_api-1.86.0/windmill_api/api/capture/update_capture.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/favorite/star.py` & `windmill_api-1.86.0/windmill_api/api/favorite/star.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/favorite/unstar.py` & `windmill_api-1.86.0/windmill_api/api/favorite/unstar.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/flow/archive_flow_by_path.py` & `windmill_api-1.86.0/windmill_api/api/flow/archive_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/flow/create_flow.py` & `windmill_api-1.86.0/windmill_api/api/flow/create_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/flow/delete_flow_by_path.py` & `windmill_api-1.86.0/windmill_api/api/flow/delete_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/flow/exists_flow_by_path.py` & `windmill_api-1.86.0/windmill_api/api/flow/exists_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/flow/get_flow_by_path.py` & `windmill_api-1.86.0/windmill_api/api/flow/get_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/flow/get_hub_flow_by_id.py` & `windmill_api-1.86.0/windmill_api/api/flow/get_hub_flow_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/flow/list_flow_paths.py` & `windmill_api-1.86.0/windmill_api/api/flow/list_flow_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/flow/list_flows.py` & `windmill_api-1.86.0/windmill_api/api/flow/list_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/flow/list_hub_flows.py` & `windmill_api-1.86.0/windmill_api/api/flow/list_hub_flows.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/flow/update_flow.py` & `windmill_api-1.86.0/windmill_api/api/flow/update_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/folder/add_owner_to_folder.py` & `windmill_api-1.86.0/windmill_api/api/folder/add_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/folder/create_folder.py` & `windmill_api-1.86.0/windmill_api/api/folder/create_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/folder/delete_folder.py` & `windmill_api-1.86.0/windmill_api/api/folder/delete_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/folder/get_folder.py` & `windmill_api-1.86.0/windmill_api/api/folder/get_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/folder/get_folder_usage.py` & `windmill_api-1.86.0/windmill_api/api/folder/get_folder_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/folder/list_folder_names.py` & `windmill_api-1.86.0/windmill_api/api/folder/list_folder_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/folder/list_folders.py` & `windmill_api-1.86.0/windmill_api/api/folder/list_folders.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/folder/remove_owner_to_folder.py` & `windmill_api-1.86.0/windmill_api/api/folder/remove_owner_to_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/folder/update_folder.py` & `windmill_api-1.86.0/windmill_api/api/folder/update_folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/granular_acl/add_granular_acls.py` & `windmill_api-1.86.0/windmill_api/api/granular_acl/add_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/granular_acl/get_granular_acls.py` & `windmill_api-1.86.0/windmill_api/api/granular_acl/get_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/granular_acl/remove_granular_acls.py` & `windmill_api-1.86.0/windmill_api/api/granular_acl/remove_granular_acls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/group/add_user_to_group.py` & `windmill_api-1.86.0/windmill_api/api/group/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/group/create_group.py` & `windmill_api-1.86.0/windmill_api/api/group/create_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/group/delete_group.py` & `windmill_api-1.86.0/windmill_api/api/group/delete_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/group/get_group.py` & `windmill_api-1.86.0/windmill_api/api/group/get_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/group/list_group_names.py` & `windmill_api-1.86.0/windmill_api/api/group/list_group_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/group/list_groups.py` & `windmill_api-1.86.0/windmill_api/api/group/list_groups.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/group/remove_user_to_group.py` & `windmill_api-1.86.0/windmill_api/api/group/remove_user_to_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/group/update_group.py` & `windmill_api-1.86.0/windmill_api/api/group/update_group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/cancel_queued_job.py` & `windmill_api-1.86.0/windmill_api/api/job/cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/cancel_suspended_job_get.py` & `windmill_api-1.86.0/windmill_api/api/job/cancel_suspended_job_get.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/cancel_suspended_job_post.py` & `windmill_api-1.86.0/windmill_api/api/job/cancel_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/create_job_signature.py` & `windmill_api-1.86.0/windmill_api/api/job/create_job_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/delete_completed_job.py` & `windmill_api-1.86.0/windmill_api/api/job/delete_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/force_cancel_queued_job.py` & `windmill_api-1.86.0/windmill_api/api/job/force_cancel_queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/get_completed_job.py` & `windmill_api-1.86.0/windmill_api/api/job/get_completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/get_completed_job_result.py` & `windmill_api-1.86.0/windmill_api/api/job/get_completed_job_result.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/get_job.py` & `windmill_api-1.86.0/windmill_api/api/job/get_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/get_job_updates.py` & `windmill_api-1.86.0/windmill_api/api/job/get_job_updates.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/get_resume_urls.py` & `windmill_api-1.86.0/windmill_api/api/job/get_resume_urls.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/get_suspended_job_flow.py` & `windmill_api-1.86.0/windmill_api/api/job/get_suspended_job_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/list_completed_jobs.py` & `windmill_api-1.86.0/windmill_api/api/job/list_completed_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/list_jobs.py` & `windmill_api-1.86.0/windmill_api/api/job/list_jobs.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/list_queue.py` & `windmill_api-1.86.0/windmill_api/api/job/list_queue.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/result_by_id.py` & `windmill_api-1.86.0/windmill_api/api/job/result_by_id.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/resume_suspended_flow_as_owner.py` & `windmill_api-1.86.0/windmill_api/api/job/resume_suspended_flow_as_owner.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/resume_suspended_job_get.py` & `windmill_api-1.86.0/windmill_api/api/job/resume_suspended_job_get.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,24 +9,27 @@
 def _get_kwargs(
     workspace: str,
     id: str,
     resume_id: int,
     signature: str,
     *,
     client: Client,
+    payload: Union[Unset, None, str] = UNSET,
     approver: Union[Unset, None, str] = UNSET,
 ) -> Dict[str, Any]:
     url = "{}/w/{workspace}/jobs_u/resume/{id}/{resume_id}/{signature}".format(
         client.base_url, workspace=workspace, id=id, resume_id=resume_id, signature=signature
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
+    params["payload"] = payload
+
     params["approver"] = approver
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
@@ -49,35 +52,38 @@
 def sync_detailed(
     workspace: str,
     id: str,
     resume_id: int,
     signature: str,
     *,
     client: Client,
+    payload: Union[Unset, None, str] = UNSET,
     approver: Union[Unset, None, str] = UNSET,
 ) -> Response[Any]:
     """resume a job for a suspended flow
 
     Args:
         workspace (str):
         id (str):
         resume_id (int):
         signature (str):
+        payload (Union[Unset, None, str]):
         approver (Union[Unset, None, str]):
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
         workspace=workspace,
         id=id,
         resume_id=resume_id,
         signature=signature,
         client=client,
+        payload=payload,
         approver=approver,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
@@ -88,35 +94,38 @@
 async def asyncio_detailed(
     workspace: str,
     id: str,
     resume_id: int,
     signature: str,
     *,
     client: Client,
+    payload: Union[Unset, None, str] = UNSET,
     approver: Union[Unset, None, str] = UNSET,
 ) -> Response[Any]:
     """resume a job for a suspended flow
 
     Args:
         workspace (str):
         id (str):
         resume_id (int):
         signature (str):
+        payload (Union[Unset, None, str]):
         approver (Union[Unset, None, str]):
 
     Returns:
         Response[Any]
     """
 
     kwargs = _get_kwargs(
         workspace=workspace,
         id=id,
         resume_id=resume_id,
         signature=signature,
         client=client,
+        payload=payload,
         approver=approver,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
```

### Comparing `windmill_api-1.85.0/windmill_api/api/job/resume_suspended_job_post.py` & `windmill_api-1.86.0/windmill_api/api/job/resume_suspended_job_post.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/run_flow_by_path.py` & `windmill_api-1.86.0/windmill_api/api/job/run_flow_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/run_flow_preview.py` & `windmill_api-1.86.0/windmill_api/api/job/run_flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/run_script_by_hash.py` & `windmill_api-1.86.0/windmill_api/api/job/run_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/run_script_by_path.py` & `windmill_api-1.86.0/windmill_api/api/job/run_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/run_script_preview.py` & `windmill_api-1.86.0/windmill_api/api/job/run_script_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/job/run_wait_result_script_by_path.py` & `windmill_api-1.86.0/windmill_api/api/variable/get_variable.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,158 +1,169 @@
-import datetime
-from typing import Any, Dict, Union
+from typing import Any, Dict, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.run_wait_result_script_by_path_json_body import RunWaitResultScriptByPathJsonBody
+from ...models.get_variable_response_200 import GetVariableResponse200
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     workspace: str,
     path: str,
     *,
     client: Client,
-    json_body: RunWaitResultScriptByPathJsonBody,
-    scheduled_for: Union[Unset, None, datetime.datetime] = UNSET,
-    scheduled_in_secs: Union[Unset, None, int] = UNSET,
-    parent_job: Union[Unset, None, str] = UNSET,
-    include_header: Union[Unset, None, str] = UNSET,
-    queue_limit: Union[Unset, None, str] = UNSET,
+    decrypt_secret: Union[Unset, None, bool] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/w/{workspace}/jobs/run_wait_result/p/{path}".format(client.base_url, workspace=workspace, path=path)
+    url = "{}/w/{workspace}/variables/get/{path}".format(client.base_url, workspace=workspace, path=path)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    json_scheduled_for: Union[Unset, None, str] = UNSET
-    if not isinstance(scheduled_for, Unset):
-        json_scheduled_for = scheduled_for.isoformat() if scheduled_for else None
-
-    params["scheduled_for"] = json_scheduled_for
-
-    params["scheduled_in_secs"] = scheduled_in_secs
-
-    params["parent_job"] = parent_job
-
-    params["include_header"] = include_header
-
-    params["queue_limit"] = queue_limit
+    params["decrypt_secret"] = decrypt_secret
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
-        "json": json_json_body,
         "params": params,
     }
 
 
-def _build_response(*, response: httpx.Response) -> Response[Any]:
+def _parse_response(*, response: httpx.Response) -> Optional[GetVariableResponse200]:
+    if response.status_code == 200:
+        response_200 = GetVariableResponse200.from_dict(response.json())
+
+        return response_200
+    return None
+
+
+def _build_response(*, response: httpx.Response) -> Response[GetVariableResponse200]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
-        parsed=None,
+        parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     workspace: str,
     path: str,
     *,
     client: Client,
-    json_body: RunWaitResultScriptByPathJsonBody,
-    scheduled_for: Union[Unset, None, datetime.datetime] = UNSET,
-    scheduled_in_secs: Union[Unset, None, int] = UNSET,
-    parent_job: Union[Unset, None, str] = UNSET,
-    include_header: Union[Unset, None, str] = UNSET,
-    queue_limit: Union[Unset, None, str] = UNSET,
-) -> Response[Any]:
-    """run script by path
+    decrypt_secret: Union[Unset, None, bool] = UNSET,
+) -> Response[GetVariableResponse200]:
+    """get variable
 
     Args:
         workspace (str):
         path (str):
-        scheduled_for (Union[Unset, None, datetime.datetime]):
-        scheduled_in_secs (Union[Unset, None, int]):
-        parent_job (Union[Unset, None, str]):
-        include_header (Union[Unset, None, str]):
-        queue_limit (Union[Unset, None, str]):
-        json_body (RunWaitResultScriptByPathJsonBody):
+        decrypt_secret (Union[Unset, None, bool]):
 
     Returns:
-        Response[Any]
+        Response[GetVariableResponse200]
     """
 
     kwargs = _get_kwargs(
         workspace=workspace,
         path=path,
         client=client,
-        json_body=json_body,
-        scheduled_for=scheduled_for,
-        scheduled_in_secs=scheduled_in_secs,
-        parent_job=parent_job,
-        include_header=include_header,
-        queue_limit=queue_limit,
+        decrypt_secret=decrypt_secret,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
+def sync(
+    workspace: str,
+    path: str,
+    *,
+    client: Client,
+    decrypt_secret: Union[Unset, None, bool] = UNSET,
+) -> Optional[GetVariableResponse200]:
+    """get variable
+
+    Args:
+        workspace (str):
+        path (str):
+        decrypt_secret (Union[Unset, None, bool]):
+
+    Returns:
+        Response[GetVariableResponse200]
+    """
+
+    return sync_detailed(
+        workspace=workspace,
+        path=path,
+        client=client,
+        decrypt_secret=decrypt_secret,
+    ).parsed
+
+
 async def asyncio_detailed(
     workspace: str,
     path: str,
     *,
     client: Client,
-    json_body: RunWaitResultScriptByPathJsonBody,
-    scheduled_for: Union[Unset, None, datetime.datetime] = UNSET,
-    scheduled_in_secs: Union[Unset, None, int] = UNSET,
-    parent_job: Union[Unset, None, str] = UNSET,
-    include_header: Union[Unset, None, str] = UNSET,
-    queue_limit: Union[Unset, None, str] = UNSET,
-) -> Response[Any]:
-    """run script by path
+    decrypt_secret: Union[Unset, None, bool] = UNSET,
+) -> Response[GetVariableResponse200]:
+    """get variable
 
     Args:
         workspace (str):
         path (str):
-        scheduled_for (Union[Unset, None, datetime.datetime]):
-        scheduled_in_secs (Union[Unset, None, int]):
-        parent_job (Union[Unset, None, str]):
-        include_header (Union[Unset, None, str]):
-        queue_limit (Union[Unset, None, str]):
-        json_body (RunWaitResultScriptByPathJsonBody):
+        decrypt_secret (Union[Unset, None, bool]):
 
     Returns:
-        Response[Any]
+        Response[GetVariableResponse200]
     """
 
     kwargs = _get_kwargs(
         workspace=workspace,
         path=path,
         client=client,
-        json_body=json_body,
-        scheduled_for=scheduled_for,
-        scheduled_in_secs=scheduled_in_secs,
-        parent_job=parent_job,
-        include_header=include_header,
-        queue_limit=queue_limit,
+        decrypt_secret=decrypt_secret,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
+
+
+async def asyncio(
+    workspace: str,
+    path: str,
+    *,
+    client: Client,
+    decrypt_secret: Union[Unset, None, bool] = UNSET,
+) -> Optional[GetVariableResponse200]:
+    """get variable
+
+    Args:
+        workspace (str):
+        path (str):
+        decrypt_secret (Union[Unset, None, bool]):
+
+    Returns:
+        Response[GetVariableResponse200]
+    """
+
+    return (
+        await asyncio_detailed(
+            workspace=workspace,
+            path=path,
+            client=client,
+            decrypt_secret=decrypt_secret,
+        )
+    ).parsed
```

### Comparing `windmill_api-1.85.0/windmill_api/api/oauth/connect_callback.py` & `windmill_api-1.86.0/windmill_api/api/oauth/connect_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/oauth/connect_slack_callback.py` & `windmill_api-1.86.0/windmill_api/api/oauth/connect_slack_callback.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/oauth/create_account.py` & `windmill_api-1.86.0/windmill_api/api/oauth/create_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/oauth/disconnect_account.py` & `windmill_api-1.86.0/windmill_api/api/oauth/disconnect_account.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/oauth/disconnect_slack.py` & `windmill_api-1.86.0/windmill_api/api/oauth/disconnect_slack.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/oauth/list_o_auth_connects.py` & `windmill_api-1.86.0/windmill_api/api/oauth/list_o_auth_connects.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/oauth/list_o_auth_logins.py` & `windmill_api-1.86.0/windmill_api/api/oauth/list_o_auth_logins.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/oauth/refresh_token.py` & `windmill_api-1.86.0/windmill_api/api/oauth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/create_resource.py` & `windmill_api-1.86.0/windmill_api/api/resource/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/create_resource_type.py` & `windmill_api-1.86.0/windmill_api/api/resource/create_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/delete_resource.py` & `windmill_api-1.86.0/windmill_api/api/resource/delete_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/delete_resource_type.py` & `windmill_api-1.86.0/windmill_api/api/resource/delete_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/exists_resource.py` & `windmill_api-1.86.0/windmill_api/api/resource/exists_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/exists_resource_type.py` & `windmill_api-1.86.0/windmill_api/api/resource/exists_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/get_resource.py` & `windmill_api-1.86.0/windmill_api/api/resource/get_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/get_resource_type.py` & `windmill_api-1.86.0/windmill_api/api/resource/get_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/get_resource_value.py` & `windmill_api-1.86.0/windmill_api/api/resource/get_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/list_resource.py` & `windmill_api-1.86.0/windmill_api/api/resource/list_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/list_resource_type.py` & `windmill_api-1.86.0/windmill_api/api/resource/list_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/list_resource_type_names.py` & `windmill_api-1.86.0/windmill_api/api/resource/list_resource_type_names.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/update_resource.py` & `windmill_api-1.86.0/windmill_api/api/resource/update_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/update_resource_type.py` & `windmill_api-1.86.0/windmill_api/api/resource/update_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/resource/update_resource_value.py` & `windmill_api-1.86.0/windmill_api/api/resource/update_resource_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/schedule/create_schedule.py` & `windmill_api-1.86.0/windmill_api/api/schedule/create_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/schedule/delete_schedule.py` & `windmill_api-1.86.0/windmill_api/api/schedule/delete_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/schedule/exists_schedule.py` & `windmill_api-1.86.0/windmill_api/api/schedule/exists_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/schedule/get_schedule.py` & `windmill_api-1.86.0/windmill_api/api/schedule/get_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/schedule/list_schedules.py` & `windmill_api-1.86.0/windmill_api/api/schedule/list_schedules.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/schedule/preview_schedule.py` & `windmill_api-1.86.0/windmill_api/api/schedule/preview_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/schedule/set_schedule_enabled.py` & `windmill_api-1.86.0/windmill_api/api/schedule/set_schedule_enabled.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/schedule/update_schedule.py` & `windmill_api-1.86.0/windmill_api/api/schedule/update_schedule.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/archive_script_by_hash.py` & `windmill_api-1.86.0/windmill_api/api/script/archive_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/archive_script_by_path.py` & `windmill_api-1.86.0/windmill_api/api/script/archive_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/bash_to_jsonschema.py` & `windmill_api-1.86.0/windmill_api/api/script/bash_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/create_script.py` & `windmill_api-1.86.0/windmill_api/api/script/create_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/delete_script_by_hash.py` & `windmill_api-1.86.0/windmill_api/api/script/delete_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/delete_script_by_path.py` & `windmill_api-1.86.0/windmill_api/api/script/delete_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/deno_to_jsonschema.py` & `windmill_api-1.86.0/windmill_api/api/script/deno_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/exists_script_by_path.py` & `windmill_api-1.86.0/windmill_api/api/script/exists_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/get_hub_script_by_path.py` & `windmill_api-1.86.0/windmill_api/api/script/get_hub_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/get_hub_script_content_by_path.py` & `windmill_api-1.86.0/windmill_api/api/script/get_hub_script_content_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/get_script_by_hash.py` & `windmill_api-1.86.0/windmill_api/api/script/get_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/get_script_by_path.py` & `windmill_api-1.86.0/windmill_api/api/script/get_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/get_script_deployment_status.py` & `windmill_api-1.86.0/windmill_api/api/script/get_script_deployment_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/go_to_jsonschema.py` & `windmill_api-1.86.0/windmill_api/api/script/go_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/list_hub_scripts.py` & `windmill_api-1.86.0/windmill_api/api/script/list_hub_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/list_script_paths.py` & `windmill_api-1.86.0/windmill_api/api/script/list_script_paths.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/list_scripts.py` & `windmill_api-1.86.0/windmill_api/api/script/list_scripts.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/python_to_jsonschema.py` & `windmill_api-1.86.0/windmill_api/api/script/python_to_jsonschema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/raw_script_by_hash.py` & `windmill_api-1.86.0/windmill_api/api/script/raw_script_by_hash.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/script/raw_script_by_path.py` & `windmill_api-1.86.0/windmill_api/api/script/raw_script_by_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/settings/backend_version.py` & `windmill_api-1.86.0/windmill_api/api/settings/backend_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/settings/get_open_api_yaml.py` & `windmill_api-1.86.0/windmill_api/api/settings/get_open_api_yaml.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/accept_invite.py` & `windmill_api-1.86.0/windmill_api/api/user/accept_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/create_token.py` & `windmill_api-1.86.0/windmill_api/api/user/create_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/create_user.py` & `windmill_api-1.86.0/windmill_api/api/user/create_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/create_user_globally.py` & `windmill_api-1.86.0/windmill_api/api/user/create_user_globally.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/decline_invite.py` & `windmill_api-1.86.0/windmill_api/api/user/decline_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/delete_token.py` & `windmill_api-1.86.0/windmill_api/api/user/delete_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/delete_user.py` & `windmill_api-1.86.0/windmill_api/api/user/delete_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/get_current_email.py` & `windmill_api-1.86.0/windmill_api/api/user/get_current_email.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/get_usage.py` & `windmill_api-1.86.0/windmill_api/api/user/get_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/global_user_delete.py` & `windmill_api-1.86.0/windmill_api/api/user/global_user_delete.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/global_user_update.py` & `windmill_api-1.86.0/windmill_api/api/user/global_user_update.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/global_whoami.py` & `windmill_api-1.86.0/windmill_api/api/user/global_whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/is_owner_of_path.py` & `windmill_api-1.86.0/windmill_api/api/user/is_owner_of_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/leave_workspace.py` & `windmill_api-1.86.0/windmill_api/api/user/leave_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/list_tokens.py` & `windmill_api-1.86.0/windmill_api/api/user/list_tokens.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/list_usernames.py` & `windmill_api-1.86.0/windmill_api/api/user/list_usernames.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/list_users.py` & `windmill_api-1.86.0/windmill_api/api/user/list_users.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/list_users_as_super_admin.py` & `windmill_api-1.86.0/windmill_api/api/user/list_users_as_super_admin.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/list_workspace_invites.py` & `windmill_api-1.86.0/windmill_api/api/user/list_workspace_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/login.py` & `windmill_api-1.86.0/windmill_api/api/user/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/login_with_oauth.py` & `windmill_api-1.86.0/windmill_api/api/user/login_with_oauth.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/logout.py` & `windmill_api-1.86.0/windmill_api/api/user/logout.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/set_password.py` & `windmill_api-1.86.0/windmill_api/api/user/set_password.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/update_user.py` & `windmill_api-1.86.0/windmill_api/api/user/update_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/whoami.py` & `windmill_api-1.86.0/windmill_api/api/user/whoami.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/user/whois.py` & `windmill_api-1.86.0/windmill_api/api/user/whois.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/variable/create_variable.py` & `windmill_api-1.86.0/windmill_api/api/variable/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/variable/delete_variable.py` & `windmill_api-1.86.0/windmill_api/api/variable/delete_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/variable/exists_variable.py` & `windmill_api-1.86.0/windmill_api/api/variable/exists_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/variable/get_variable.py` & `windmill_api-1.86.0/windmill_api/api/worker/list_workers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,169 +1,163 @@
-from typing import Any, Dict, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.get_variable_response_200 import GetVariableResponse200
+from ...models.list_workers_response_200_item import ListWorkersResponse200Item
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
-    workspace: str,
-    path: str,
     *,
     client: Client,
-    decrypt_secret: Union[Unset, None, bool] = UNSET,
+    page: Union[Unset, None, int] = UNSET,
+    per_page: Union[Unset, None, int] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/w/{workspace}/variables/get/{path}".format(client.base_url, workspace=workspace, path=path)
+    url = "{}/workers/list".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
-    params["decrypt_secret"] = decrypt_secret
+    params["page"] = page
+
+    params["per_page"] = per_page
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[GetVariableResponse200]:
+def _parse_response(*, response: httpx.Response) -> Optional[List[ListWorkersResponse200Item]]:
     if response.status_code == 200:
-        response_200 = GetVariableResponse200.from_dict(response.json())
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = ListWorkersResponse200Item.from_dict(response_200_item_data)
+
+            response_200.append(response_200_item)
 
         return response_200
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[GetVariableResponse200]:
+def _build_response(*, response: httpx.Response) -> Response[List[ListWorkersResponse200Item]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
-    workspace: str,
-    path: str,
     *,
     client: Client,
-    decrypt_secret: Union[Unset, None, bool] = UNSET,
-) -> Response[GetVariableResponse200]:
-    """get variable
+    page: Union[Unset, None, int] = UNSET,
+    per_page: Union[Unset, None, int] = UNSET,
+) -> Response[List[ListWorkersResponse200Item]]:
+    """list workers
 
     Args:
-        workspace (str):
-        path (str):
-        decrypt_secret (Union[Unset, None, bool]):
+        page (Union[Unset, None, int]):
+        per_page (Union[Unset, None, int]):
 
     Returns:
-        Response[GetVariableResponse200]
+        Response[List[ListWorkersResponse200Item]]
     """
 
     kwargs = _get_kwargs(
-        workspace=workspace,
-        path=path,
         client=client,
-        decrypt_secret=decrypt_secret,
+        page=page,
+        per_page=per_page,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(response=response)
 
 
 def sync(
-    workspace: str,
-    path: str,
     *,
     client: Client,
-    decrypt_secret: Union[Unset, None, bool] = UNSET,
-) -> Optional[GetVariableResponse200]:
-    """get variable
+    page: Union[Unset, None, int] = UNSET,
+    per_page: Union[Unset, None, int] = UNSET,
+) -> Optional[List[ListWorkersResponse200Item]]:
+    """list workers
 
     Args:
-        workspace (str):
-        path (str):
-        decrypt_secret (Union[Unset, None, bool]):
+        page (Union[Unset, None, int]):
+        per_page (Union[Unset, None, int]):
 
     Returns:
-        Response[GetVariableResponse200]
+        Response[List[ListWorkersResponse200Item]]
     """
 
     return sync_detailed(
-        workspace=workspace,
-        path=path,
         client=client,
-        decrypt_secret=decrypt_secret,
+        page=page,
+        per_page=per_page,
     ).parsed
 
 
 async def asyncio_detailed(
-    workspace: str,
-    path: str,
     *,
     client: Client,
-    decrypt_secret: Union[Unset, None, bool] = UNSET,
-) -> Response[GetVariableResponse200]:
-    """get variable
+    page: Union[Unset, None, int] = UNSET,
+    per_page: Union[Unset, None, int] = UNSET,
+) -> Response[List[ListWorkersResponse200Item]]:
+    """list workers
 
     Args:
-        workspace (str):
-        path (str):
-        decrypt_secret (Union[Unset, None, bool]):
+        page (Union[Unset, None, int]):
+        per_page (Union[Unset, None, int]):
 
     Returns:
-        Response[GetVariableResponse200]
+        Response[List[ListWorkersResponse200Item]]
     """
 
     kwargs = _get_kwargs(
-        workspace=workspace,
-        path=path,
         client=client,
-        decrypt_secret=decrypt_secret,
+        page=page,
+        per_page=per_page,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(response=response)
 
 
 async def asyncio(
-    workspace: str,
-    path: str,
     *,
     client: Client,
-    decrypt_secret: Union[Unset, None, bool] = UNSET,
-) -> Optional[GetVariableResponse200]:
-    """get variable
+    page: Union[Unset, None, int] = UNSET,
+    per_page: Union[Unset, None, int] = UNSET,
+) -> Optional[List[ListWorkersResponse200Item]]:
+    """list workers
 
     Args:
-        workspace (str):
-        path (str):
-        decrypt_secret (Union[Unset, None, bool]):
+        page (Union[Unset, None, int]):
+        per_page (Union[Unset, None, int]):
 
     Returns:
-        Response[GetVariableResponse200]
+        Response[List[ListWorkersResponse200Item]]
     """
 
     return (
         await asyncio_detailed(
-            workspace=workspace,
-            path=path,
             client=client,
-            decrypt_secret=decrypt_secret,
+            page=page,
+            per_page=per_page,
         )
     ).parsed
```

### Comparing `windmill_api-1.85.0/windmill_api/api/variable/list_contextual_variables.py` & `windmill_api-1.86.0/windmill_api/api/variable/list_contextual_variables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/variable/list_variable.py` & `windmill_api-1.86.0/windmill_api/api/variable/list_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/variable/update_variable.py` & `windmill_api-1.86.0/windmill_api/api/variable/update_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/worker/list_workers.py` & `windmill_api-1.86.0/windmill_api/api/workspace/list_workspaces_as_super_admin.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Any, Dict, List, Optional, Union
 
 import httpx
 
 from ...client import Client
-from ...models.list_workers_response_200_item import ListWorkersResponse200Item
+from ...models.list_workspaces_as_super_admin_response_200_item import ListWorkspacesAsSuperAdminResponse200Item
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
     client: Client,
     page: Union[Unset, None, int] = UNSET,
     per_page: Union[Unset, None, int] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/workers/list".format(client.base_url)
+    url = "{}/workspaces/list_as_superadmin".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["page"] = page
 
@@ -31,50 +31,50 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "params": params,
     }
 
 
-def _parse_response(*, response: httpx.Response) -> Optional[List[ListWorkersResponse200Item]]:
+def _parse_response(*, response: httpx.Response) -> Optional[List[ListWorkspacesAsSuperAdminResponse200Item]]:
     if response.status_code == 200:
         response_200 = []
         _response_200 = response.json()
         for response_200_item_data in _response_200:
-            response_200_item = ListWorkersResponse200Item.from_dict(response_200_item_data)
+            response_200_item = ListWorkspacesAsSuperAdminResponse200Item.from_dict(response_200_item_data)
 
             response_200.append(response_200_item)
 
         return response_200
     return None
 
 
-def _build_response(*, response: httpx.Response) -> Response[List[ListWorkersResponse200Item]]:
+def _build_response(*, response: httpx.Response) -> Response[List[ListWorkspacesAsSuperAdminResponse200Item]]:
     return Response(
         status_code=response.status_code,
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
     page: Union[Unset, None, int] = UNSET,
     per_page: Union[Unset, None, int] = UNSET,
-) -> Response[List[ListWorkersResponse200Item]]:
-    """list workers
+) -> Response[List[ListWorkspacesAsSuperAdminResponse200Item]]:
+    """list all workspaces as super admin (require to be super admin)
 
     Args:
         page (Union[Unset, None, int]):
         per_page (Union[Unset, None, int]):
 
     Returns:
-        Response[List[ListWorkersResponse200Item]]
+        Response[List[ListWorkspacesAsSuperAdminResponse200Item]]
     """
 
     kwargs = _get_kwargs(
         client=client,
         page=page,
         per_page=per_page,
     )
@@ -88,46 +88,46 @@
 
 
 def sync(
     *,
     client: Client,
     page: Union[Unset, None, int] = UNSET,
     per_page: Union[Unset, None, int] = UNSET,
-) -> Optional[List[ListWorkersResponse200Item]]:
-    """list workers
+) -> Optional[List[ListWorkspacesAsSuperAdminResponse200Item]]:
+    """list all workspaces as super admin (require to be super admin)
 
     Args:
         page (Union[Unset, None, int]):
         per_page (Union[Unset, None, int]):
 
     Returns:
-        Response[List[ListWorkersResponse200Item]]
+        Response[List[ListWorkspacesAsSuperAdminResponse200Item]]
     """
 
     return sync_detailed(
         client=client,
         page=page,
         per_page=per_page,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
     page: Union[Unset, None, int] = UNSET,
     per_page: Union[Unset, None, int] = UNSET,
-) -> Response[List[ListWorkersResponse200Item]]:
-    """list workers
+) -> Response[List[ListWorkspacesAsSuperAdminResponse200Item]]:
+    """list all workspaces as super admin (require to be super admin)
 
     Args:
         page (Union[Unset, None, int]):
         per_page (Union[Unset, None, int]):
 
     Returns:
-        Response[List[ListWorkersResponse200Item]]
+        Response[List[ListWorkspacesAsSuperAdminResponse200Item]]
     """
 
     kwargs = _get_kwargs(
         client=client,
         page=page,
         per_page=per_page,
     )
@@ -139,23 +139,23 @@
 
 
 async def asyncio(
     *,
     client: Client,
     page: Union[Unset, None, int] = UNSET,
     per_page: Union[Unset, None, int] = UNSET,
-) -> Optional[List[ListWorkersResponse200Item]]:
-    """list workers
+) -> Optional[List[ListWorkspacesAsSuperAdminResponse200Item]]:
+    """list all workspaces as super admin (require to be super admin)
 
     Args:
         page (Union[Unset, None, int]):
         per_page (Union[Unset, None, int]):
 
     Returns:
-        Response[List[ListWorkersResponse200Item]]
+        Response[List[ListWorkspacesAsSuperAdminResponse200Item]]
     """
 
     return (
         await asyncio_detailed(
             client=client,
             page=page,
             per_page=per_page,
```

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/add_user.py` & `windmill_api-1.86.0/windmill_api/api/workspace/add_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/archive_workspace.py` & `windmill_api-1.86.0/windmill_api/api/workspace/archive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/create_workspace.py` & `windmill_api-1.86.0/windmill_api/api/workspace/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/delete_invite.py` & `windmill_api-1.86.0/windmill_api/api/workspace/delete_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/delete_workspace.py` & `windmill_api-1.86.0/windmill_api/api/workspace/delete_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/edit_auto_invite.py` & `windmill_api-1.86.0/windmill_api/api/workspace/edit_auto_invite.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/edit_slack_command.py` & `windmill_api-1.86.0/windmill_api/api/workspace/edit_slack_command.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/edit_webhook.py` & `windmill_api-1.86.0/windmill_api/api/workspace/edit_webhook.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/exists_username.py` & `windmill_api-1.86.0/windmill_api/api/workspace/exists_username.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/exists_workspace.py` & `windmill_api-1.86.0/windmill_api/api/workspace/exists_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/get_premium_info.py` & `windmill_api-1.86.0/windmill_api/api/workspace/get_premium_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/get_settings.py` & `windmill_api-1.86.0/windmill_api/api/workspace/get_settings.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/invite_user.py` & `windmill_api-1.86.0/windmill_api/api/workspace/invite_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/is_domain_allowed.py` & `windmill_api-1.86.0/windmill_api/api/workspace/is_domain_allowed.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/list_pending_invites.py` & `windmill_api-1.86.0/windmill_api/api/workspace/list_pending_invites.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/list_user_workspaces.py` & `windmill_api-1.86.0/windmill_api/api/workspace/list_user_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/list_workspaces.py` & `windmill_api-1.86.0/windmill_api/api/workspace/list_workspaces.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/api/workspace/unarchive_workspace.py` & `windmill_api-1.86.0/windmill_api/api/workspace/unarchive_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/client.py` & `windmill_api-1.86.0/windmill_api/client.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/accept_invite_json_body.py` & `windmill_api-1.86.0/windmill_api/models/accept_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/add_granular_acls_json_body.py` & `windmill_api-1.86.0/windmill_api/models/add_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/add_owner_to_folder_json_body.py` & `windmill_api-1.86.0/windmill_api/models/add_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/add_user_json_body.py` & `windmill_api-1.86.0/windmill_api/models/add_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/add_user_to_group_json_body.py` & `windmill_api-1.86.0/windmill_api/models/add_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/app_with_last_version.py` & `windmill_api-1.86.0/windmill_api/models/app_with_last_version.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/app_with_last_version_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/app_with_last_version_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/app_with_last_version_policy.py` & `windmill_api-1.86.0/windmill_api/models/app_with_last_version_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/app_with_last_version_policy_triggerables.py` & `windmill_api-1.86.0/windmill_api/models/app_with_last_version_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py` & `windmill_api-1.86.0/windmill_api/models/app_with_last_version_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/archive_script_by_hash_response_200.py` & `windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/archive_script_by_hash_response_200_schema.py` & `windmill_api-1.86.0/windmill_api/models/archive_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/audit_log.py` & `windmill_api-1.86.0/windmill_api/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/audit_log_operation.py` & `windmill_api-1.86.0/windmill_api/models/audit_log_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/audit_log_parameters.py` & `windmill_api-1.86.0/windmill_api/models/audit_log_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200.py` & `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py` & `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.86.0/windmill_api/models/bash_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_all.py` & `windmill_api-1.86.0/windmill_api/models/branch_all.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_all_branches_item.py` & `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/branch_all_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one.py` & `windmill_api-1.86.0/windmill_api/models/branch_one.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_branches_item.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_default_item.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_default_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_default_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_default_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_default_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_default_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_default_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/branch_one_default_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/branch_one_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/cancel_queued_job_json_body.py` & `windmill_api-1.86.0/windmill_api/models/cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/cancel_suspended_job_post_json_body.py` & `windmill_api-1.86.0/windmill_api/models/cancel_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job.py` & `windmill_api-1.86.0/windmill_api/models/completed_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_args.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_flow_status.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_flow_status_retry.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/completed_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/connect_callback_json_body.py` & `windmill_api-1.86.0/windmill_api/models/connect_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/connect_callback_response_200.py` & `windmill_api-1.86.0/windmill_api/models/connect_callback_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/connect_slack_callback_json_body.py` & `windmill_api-1.86.0/windmill_api/models/connect_slack_callback_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/contextual_variable.py` & `windmill_api-1.86.0/windmill_api/models/contextual_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_account_json_body.py` & `windmill_api-1.86.0/windmill_api/models/create_account_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_app_json_body.py` & `windmill_api-1.86.0/windmill_api/models/create_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_app_json_body_policy.py` & `windmill_api-1.86.0/windmill_api/models/create_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_app_json_body_policy_triggerables.py` & `windmill_api-1.86.0/windmill_api/models/create_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.86.0/windmill_api/models/create_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_schema.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/create_flow_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_folder_json_body.py` & `windmill_api-1.86.0/windmill_api/models/create_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_group_json_body.py` & `windmill_api-1.86.0/windmill_api/models/create_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_resource.py` & `windmill_api-1.86.0/windmill_api/models/create_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_resource_json_body.py` & `windmill_api-1.86.0/windmill_api/models/create_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_resource_type_json_body.py` & `windmill_api-1.86.0/windmill_api/models/create_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_schedule_json_body.py` & `windmill_api-1.86.0/windmill_api/models/create_schedule_json_body.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,82 +10,81 @@
 
 @attr.s(auto_attribs=True)
 class CreateScheduleJsonBody:
     """
     Attributes:
         path (str):
         schedule (str):
+        timezone (str):
         script_path (str):
         is_flow (bool):
         args (CreateScheduleJsonBodyArgs):
-        offset (Union[Unset, int]):
         enabled (Union[Unset, bool]):
     """
 
     path: str
     schedule: str
+    timezone: str
     script_path: str
     is_flow: bool
     args: CreateScheduleJsonBodyArgs
-    offset: Union[Unset, int] = UNSET
     enabled: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         path = self.path
         schedule = self.schedule
+        timezone = self.timezone
         script_path = self.script_path
         is_flow = self.is_flow
         args = self.args.to_dict()
 
-        offset = self.offset
         enabled = self.enabled
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "path": path,
                 "schedule": schedule,
+                "timezone": timezone,
                 "script_path": script_path,
                 "is_flow": is_flow,
                 "args": args,
             }
         )
-        if offset is not UNSET:
-            field_dict["offset"] = offset
         if enabled is not UNSET:
             field_dict["enabled"] = enabled
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         path = d.pop("path")
 
         schedule = d.pop("schedule")
 
+        timezone = d.pop("timezone")
+
         script_path = d.pop("script_path")
 
         is_flow = d.pop("is_flow")
 
         args = CreateScheduleJsonBodyArgs.from_dict(d.pop("args"))
 
-        offset = d.pop("offset", UNSET)
-
         enabled = d.pop("enabled", UNSET)
 
         create_schedule_json_body = cls(
             path=path,
             schedule=schedule,
+            timezone=timezone,
             script_path=script_path,
             is_flow=is_flow,
             args=args,
-            offset=offset,
             enabled=enabled,
         )
 
         create_schedule_json_body.additional_properties = d
         return create_schedule_json_body
 
     @property
```

### Comparing `windmill_api-1.85.0/windmill_api/models/create_schedule_json_body_args.py` & `windmill_api-1.86.0/windmill_api/models/create_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_script_json_body.py` & `windmill_api-1.86.0/windmill_api/models/create_script_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_script_json_body_schema.py` & `windmill_api-1.86.0/windmill_api/models/create_script_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_token_json_body.py` & `windmill_api-1.86.0/windmill_api/models/create_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_user_globally_json_body.py` & `windmill_api-1.86.0/windmill_api/models/create_user_globally_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_user_json_body.py` & `windmill_api-1.86.0/windmill_api/models/create_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_variable.py` & `windmill_api-1.86.0/windmill_api/models/create_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_variable_json_body.py` & `windmill_api-1.86.0/windmill_api/models/create_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_workspace.py` & `windmill_api-1.86.0/windmill_api/models/create_workspace.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/create_workspace_json_body.py` & `windmill_api-1.86.0/windmill_api/models/create_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/decline_invite_json_body.py` & `windmill_api-1.86.0/windmill_api/models/decline_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_args.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/delete_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_invite_json_body.py` & `windmill_api-1.86.0/windmill_api/models/delete_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_script_by_hash_response_200.py` & `windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/delete_script_by_hash_response_200_schema.py` & `windmill_api-1.86.0/windmill_api/models/delete_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200.py` & `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py` & `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.86.0/windmill_api/models/deno_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/edit_auto_invite_json_body.py` & `windmill_api-1.86.0/windmill_api/models/edit_auto_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/edit_resource.py` & `windmill_api-1.86.0/windmill_api/models/edit_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/edit_resource_type.py` & `windmill_api-1.86.0/windmill_api/models/edit_resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/edit_schedule.py` & `windmill_api-1.86.0/windmill_api/models/edit_schedule.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,45 +8,52 @@
 
 
 @attr.s(auto_attribs=True)
 class EditSchedule:
     """
     Attributes:
         schedule (str):
+        timezone (str):
         args (EditScheduleArgs):
     """
 
     schedule: str
+    timezone: str
     args: EditScheduleArgs
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         schedule = self.schedule
+        timezone = self.timezone
         args = self.args.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "schedule": schedule,
+                "timezone": timezone,
                 "args": args,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         schedule = d.pop("schedule")
 
+        timezone = d.pop("timezone")
+
         args = EditScheduleArgs.from_dict(d.pop("args"))
 
         edit_schedule = cls(
             schedule=schedule,
+            timezone=timezone,
             args=args,
         )
 
         edit_schedule.additional_properties = d
         return edit_schedule
 
     @property
```

### Comparing `windmill_api-1.85.0/windmill_api/models/edit_schedule_args.py` & `windmill_api-1.86.0/windmill_api/models/edit_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/edit_slack_command_json_body.py` & `windmill_api-1.86.0/windmill_api/models/edit_slack_command_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/edit_variable.py` & `windmill_api-1.86.0/windmill_api/models/edit_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/edit_webhook_json_body.py` & `windmill_api-1.86.0/windmill_api/models/edit_webhook_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/edit_workspace_user.py` & `windmill_api-1.86.0/windmill_api/models/edit_workspace_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/execute_component_json_body.py` & `windmill_api-1.86.0/windmill_api/models/execute_component_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py` & `windmill_api-1.86.0/windmill_api/models/execute_component_json_body_force_viewer_static_fields.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/execute_component_json_body_raw_code.py` & `windmill_api-1.86.0/windmill_api/models/execute_component_json_body_raw_code.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/exists_username_json_body.py` & `windmill_api-1.86.0/windmill_api/models/exists_username_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/exists_workspace_json_body.py` & `windmill_api-1.86.0/windmill_api/models/exists_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow.py` & `windmill_api-1.86.0/windmill_api/models/flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/flow_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_metadata.py` & `windmill_api-1.86.0/windmill_api/models/flow_metadata.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_metadata_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/flow_metadata_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module.py` & `windmill_api-1.86.0/windmill_api/models/flow_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_0.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_0_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_1.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_1_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_2.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_2_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_3_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_4_default_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_5_branches_item_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_module_value_2_type_6.py` & `windmill_api-1.86.0/windmill_api/models/flow_module_value_2_type_6.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_args.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_preview_value_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/flow_preview_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_schema.py` & `windmill_api-1.86.0/windmill_api/models/flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status.py` & `windmill_api-1.86.0/windmill_api/models/flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_failure_module_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_failure_module_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_failure_module_branchall.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_failure_module_iterator.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_module.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_module_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_module_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_module_branchall.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_module_iterator.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_modules_item_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_modules_item_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_modules_item_branchall.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_modules_item_iterator.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_status_retry.py` & `windmill_api-1.86.0/windmill_api/models/flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value.py` & `windmill_api-1.86.0/windmill_api/models/flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/flow_value_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/folder.py` & `windmill_api-1.86.0/windmill_api/models/folder.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/folder_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/folder_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/force_cancel_queued_job_json_body.py` & `windmill_api-1.86.0/windmill_api/models/force_cancel_queued_job_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/forloop_flow.py` & `windmill_api-1.86.0/windmill_api/models/forloop_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/forloop_flow_iterator_type_0.py` & `windmill_api-1.86.0/windmill_api/models/forloop_flow_iterator_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/forloop_flow_iterator_type_1.py` & `windmill_api-1.86.0/windmill_api/models/forloop_flow_iterator_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/forloop_flow_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/forloop_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_app_by_path_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_app_by_path_response_200_policy.py` & `windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py` & `windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.86.0/windmill_api/models/get_app_by_path_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_app_by_version_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_app_by_version_response_200_policy.py` & `windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py` & `windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.86.0/windmill_api/models/get_app_by_version_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_audit_log_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_audit_log_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_audit_log_response_200_operation.py` & `windmill_api-1.86.0/windmill_api/models/get_audit_log_response_200_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_audit_log_response_200_parameters.py` & `windmill_api-1.86.0/windmill_api/models/get_audit_log_response_200_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_args.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/get_completed_job_response_200_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_schema.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/get_flow_by_path_response_200_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_folder_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_folder_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_folder_response_200_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/get_folder_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_folder_usage_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_folder_usage_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_granular_acls_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_granular_acls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_group_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_group_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_group_response_200_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/get_group_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_app_by_id_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_app_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_app_by_id_response_200_app.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_app_by_id_response_200_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_flow_by_id_response_200_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_hub_script_by_path_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_hub_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_job_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_job_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_job_updates_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_job_updates_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_premium_info_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_premium_info_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_public_app_by_secret_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py` & `windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py` & `windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py` & `windmill_api-1.86.0/windmill_api/models/get_public_app_by_secret_response_200_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_resource_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_resource_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_resource_response_200_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/get_resource_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_resource_type_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_resource_type_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_resume_urls_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_resume_urls_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_schedule_response_200.py` & `windmill_api-1.86.0/windmill_api/models/schedule.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.get_schedule_response_200_args import GetScheduleResponse200Args
-from ..models.get_schedule_response_200_extra_perms import GetScheduleResponse200ExtraPerms
+from ..models.schedule_args import ScheduleArgs
+from ..models.schedule_extra_perms import ScheduleExtraPerms
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="GetScheduleResponse200")
+T = TypeVar("T", bound="Schedule")
 
 
 @attr.s(auto_attribs=True)
-class GetScheduleResponse200:
+class Schedule:
     """
     Attributes:
         path (str):
         edited_by (str):
         edited_at (datetime.datetime):
         schedule (str):
-        offset (int):
+        timezone (str):
         enabled (bool):
         script_path (str):
         is_flow (bool):
-        extra_perms (GetScheduleResponse200ExtraPerms):
+        extra_perms (ScheduleExtraPerms):
         email (str):
-        args (Union[Unset, GetScheduleResponse200Args]):
+        args (Union[Unset, ScheduleArgs]):
         error (Union[Unset, str]):
     """
 
     path: str
     edited_by: str
     edited_at: datetime.datetime
     schedule: str
-    offset: int
+    timezone: str
     enabled: bool
     script_path: str
     is_flow: bool
-    extra_perms: GetScheduleResponse200ExtraPerms
+    extra_perms: ScheduleExtraPerms
     email: str
-    args: Union[Unset, GetScheduleResponse200Args] = UNSET
+    args: Union[Unset, ScheduleArgs] = UNSET
     error: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         path = self.path
         edited_by = self.edited_by
         edited_at = self.edited_at.isoformat()
 
         schedule = self.schedule
-        offset = self.offset
+        timezone = self.timezone
         enabled = self.enabled
         script_path = self.script_path
         is_flow = self.is_flow
         extra_perms = self.extra_perms.to_dict()
 
         email = self.email
         args: Union[Unset, Dict[str, Any]] = UNSET
@@ -66,15 +66,15 @@
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "path": path,
                 "edited_by": edited_by,
                 "edited_at": edited_at,
                 "schedule": schedule,
-                "offset_": offset,
+                "timezone": timezone,
                 "enabled": enabled,
                 "script_path": script_path,
                 "is_flow": is_flow,
                 "extra_perms": extra_perms,
                 "email": email,
             }
         )
@@ -92,52 +92,52 @@
 
         edited_by = d.pop("edited_by")
 
         edited_at = isoparse(d.pop("edited_at"))
 
         schedule = d.pop("schedule")
 
-        offset = d.pop("offset_")
+        timezone = d.pop("timezone")
 
         enabled = d.pop("enabled")
 
         script_path = d.pop("script_path")
 
         is_flow = d.pop("is_flow")
 
-        extra_perms = GetScheduleResponse200ExtraPerms.from_dict(d.pop("extra_perms"))
+        extra_perms = ScheduleExtraPerms.from_dict(d.pop("extra_perms"))
 
         email = d.pop("email")
 
         _args = d.pop("args", UNSET)
-        args: Union[Unset, GetScheduleResponse200Args]
+        args: Union[Unset, ScheduleArgs]
         if isinstance(_args, Unset):
             args = UNSET
         else:
-            args = GetScheduleResponse200Args.from_dict(_args)
+            args = ScheduleArgs.from_dict(_args)
 
         error = d.pop("error", UNSET)
 
-        get_schedule_response_200 = cls(
+        schedule = cls(
             path=path,
             edited_by=edited_by,
             edited_at=edited_at,
             schedule=schedule,
-            offset=offset,
+            timezone=timezone,
             enabled=enabled,
             script_path=script_path,
             is_flow=is_flow,
             extra_perms=extra_perms,
             email=email,
             args=args,
             error=error,
         )
 
-        get_schedule_response_200.additional_properties = d
-        return get_schedule_response_200
+        schedule.additional_properties = d
+        return schedule
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.85.0/windmill_api/models/get_schedule_response_200_args.py` & `windmill_api-1.86.0/windmill_api/models/get_schedule_response_200_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_schedule_response_200_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/get_schedule_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_script_by_hash_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_script_by_hash_response_200_schema.py` & `windmill_api-1.86.0/windmill_api/models/get_script_by_hash_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_script_by_path_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_script_by_path_response_200_schema.py` & `windmill_api-1.86.0/windmill_api/models/get_script_by_path_response_200_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_script_deployment_status_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_script_deployment_status_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_settings_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_suspended_job_flow_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_suspended_job_flow_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/get_suspended_job_flow_response_200_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_suspended_job_flow_response_200_job.py` & `windmill_api-1.86.0/windmill_api/models/get_suspended_job_flow_response_200_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_variable_response_200.py` & `windmill_api-1.86.0/windmill_api/models/get_variable_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/get_variable_response_200_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/get_variable_response_200_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/global_user_info.py` & `windmill_api-1.86.0/windmill_api/models/global_user_info.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/global_user_update_json_body.py` & `windmill_api-1.86.0/windmill_api/models/global_user_update_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/global_whoami_response_200.py` & `windmill_api-1.86.0/windmill_api/models/global_whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200.py` & `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py` & `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.86.0/windmill_api/models/go_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/group.py` & `windmill_api-1.86.0/windmill_api/models/group.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/group_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/group_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/identity.py` & `windmill_api-1.86.0/windmill_api/models/identity.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/input_transform_type_0.py` & `windmill_api-1.86.0/windmill_api/models/input_transform_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/input_transform_type_1.py` & `windmill_api-1.86.0/windmill_api/models/input_transform_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/invite_user_json_body.py` & `windmill_api-1.86.0/windmill_api/models/invite_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/javascript_transform.py` & `windmill_api-1.86.0/windmill_api/models/javascript_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/job.py` & `windmill_api-1.86.0/windmill_api/models/job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_apps_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_apps_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_apps_response_200_item_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/list_apps_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_audit_logs_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_audit_logs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_audit_logs_response_200_item_operation.py` & `windmill_api-1.86.0/windmill_api/models/list_audit_logs_response_200_item_operation.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py` & `windmill_api-1.86.0/windmill_api/models/list_audit_logs_response_200_item_parameters.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_args.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/list_completed_jobs_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_contextual_variables_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_contextual_variables_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_schema.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/list_flows_response_200_item_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_folders_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_folders_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_folders_response_200_item_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/list_folders_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_groups_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_groups_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_groups_response_200_item_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/list_groups_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_hub_apps_response_200.py` & `windmill_api-1.86.0/windmill_api/models/list_hub_apps_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_hub_apps_response_200_apps_item.py` & `windmill_api-1.86.0/windmill_api/models/list_hub_apps_response_200_apps_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_hub_flows_response_200.py` & `windmill_api-1.86.0/windmill_api/models/list_hub_flows_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_hub_flows_response_200_flows_item.py` & `windmill_api-1.86.0/windmill_api/models/list_hub_flows_response_200_flows_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_hub_scripts_response_200.py` & `windmill_api-1.86.0/windmill_api/models/list_hub_scripts_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py` & `windmill_api-1.86.0/windmill_api/models/list_hub_scripts_response_200_asks_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_jobs_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_jobs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_pending_invites_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_pending_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_args.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/list_queue_response_200_item_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_resource_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_resource_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_resource_response_200_item_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/list_resource_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_resource_type_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_resource_type_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_schedules_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_schedules_response_200_item.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 class ListSchedulesResponse200Item:
     """
     Attributes:
         path (str):
         edited_by (str):
         edited_at (datetime.datetime):
         schedule (str):
-        offset (int):
+        timezone (str):
         enabled (bool):
         script_path (str):
         is_flow (bool):
         extra_perms (ListSchedulesResponse200ItemExtraPerms):
         email (str):
         args (Union[Unset, ListSchedulesResponse200ItemArgs]):
         error (Union[Unset, str]):
     """
 
     path: str
     edited_by: str
     edited_at: datetime.datetime
     schedule: str
-    offset: int
+    timezone: str
     enabled: bool
     script_path: str
     is_flow: bool
     extra_perms: ListSchedulesResponse200ItemExtraPerms
     email: str
     args: Union[Unset, ListSchedulesResponse200ItemArgs] = UNSET
     error: Union[Unset, str] = UNSET
@@ -45,15 +45,15 @@
 
     def to_dict(self) -> Dict[str, Any]:
         path = self.path
         edited_by = self.edited_by
         edited_at = self.edited_at.isoformat()
 
         schedule = self.schedule
-        offset = self.offset
+        timezone = self.timezone
         enabled = self.enabled
         script_path = self.script_path
         is_flow = self.is_flow
         extra_perms = self.extra_perms.to_dict()
 
         email = self.email
         args: Union[Unset, Dict[str, Any]] = UNSET
@@ -66,15 +66,15 @@
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "path": path,
                 "edited_by": edited_by,
                 "edited_at": edited_at,
                 "schedule": schedule,
-                "offset_": offset,
+                "timezone": timezone,
                 "enabled": enabled,
                 "script_path": script_path,
                 "is_flow": is_flow,
                 "extra_perms": extra_perms,
                 "email": email,
             }
         )
@@ -92,15 +92,15 @@
 
         edited_by = d.pop("edited_by")
 
         edited_at = isoparse(d.pop("edited_at"))
 
         schedule = d.pop("schedule")
 
-        offset = d.pop("offset_")
+        timezone = d.pop("timezone")
 
         enabled = d.pop("enabled")
 
         script_path = d.pop("script_path")
 
         is_flow = d.pop("is_flow")
 
@@ -118,15 +118,15 @@
         error = d.pop("error", UNSET)
 
         list_schedules_response_200_item = cls(
             path=path,
             edited_by=edited_by,
             edited_at=edited_at,
             schedule=schedule,
-            offset=offset,
+            timezone=timezone,
             enabled=enabled,
             script_path=script_path,
             is_flow=is_flow,
             extra_perms=extra_perms,
             email=email,
             args=args,
             error=error,
```

### Comparing `windmill_api-1.85.0/windmill_api/models/list_schedules_response_200_item_args.py` & `windmill_api-1.86.0/windmill_api/models/list_schedules_response_200_item_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/list_schedules_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_scripts_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_scripts_response_200_item_schema.py` & `windmill_api-1.86.0/windmill_api/models/list_scripts_response_200_item_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_tokens_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_tokens_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_user_workspaces_response_200.py` & `windmill_api-1.86.0/windmill_api/models/list_user_workspaces_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py` & `windmill_api-1.86.0/windmill_api/models/list_user_workspaces_response_200_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_users_as_super_admin_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_users_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_users_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_users_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_users_response_200_item_usage.py` & `windmill_api-1.86.0/windmill_api/models/list_users_response_200_item_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_variable_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_variable_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_variable_response_200_item_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/list_variable_response_200_item_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_workers_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_workers_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_workspace_invites_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_workspace_invites_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_workspaces_as_super_admin_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/list_workspaces_response_200_item.py` & `windmill_api-1.86.0/windmill_api/models/list_workspaces_response_200_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/listable_app.py` & `windmill_api-1.86.0/windmill_api/models/listable_app.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/listable_app_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/listable_app_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/listable_resource.py` & `windmill_api-1.86.0/windmill_api/models/listable_resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/listable_resource_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/listable_resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/listable_variable.py` & `windmill_api-1.86.0/windmill_api/models/listable_variable.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/listable_variable_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/listable_variable_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/login.py` & `windmill_api-1.86.0/windmill_api/models/login.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/login_json_body.py` & `windmill_api-1.86.0/windmill_api/models/login_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/login_with_oauth_json_body.py` & `windmill_api-1.86.0/windmill_api/models/login_with_oauth_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/main_arg_signature.py` & `windmill_api-1.86.0/windmill_api/models/main_arg_signature.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item.py` & `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py` & `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py` & `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py` & `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py` & `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py` & `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.86.0/windmill_api/models/main_arg_signature_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/new_schedule.py` & `windmill_api-1.86.0/windmill_api/models/new_schedule.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,82 +10,81 @@
 
 @attr.s(auto_attribs=True)
 class NewSchedule:
     """
     Attributes:
         path (str):
         schedule (str):
+        timezone (str):
         script_path (str):
         is_flow (bool):
         args (NewScheduleArgs):
-        offset (Union[Unset, int]):
         enabled (Union[Unset, bool]):
     """
 
     path: str
     schedule: str
+    timezone: str
     script_path: str
     is_flow: bool
     args: NewScheduleArgs
-    offset: Union[Unset, int] = UNSET
     enabled: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         path = self.path
         schedule = self.schedule
+        timezone = self.timezone
         script_path = self.script_path
         is_flow = self.is_flow
         args = self.args.to_dict()
 
-        offset = self.offset
         enabled = self.enabled
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "path": path,
                 "schedule": schedule,
+                "timezone": timezone,
                 "script_path": script_path,
                 "is_flow": is_flow,
                 "args": args,
             }
         )
-        if offset is not UNSET:
-            field_dict["offset"] = offset
         if enabled is not UNSET:
             field_dict["enabled"] = enabled
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         path = d.pop("path")
 
         schedule = d.pop("schedule")
 
+        timezone = d.pop("timezone")
+
         script_path = d.pop("script_path")
 
         is_flow = d.pop("is_flow")
 
         args = NewScheduleArgs.from_dict(d.pop("args"))
 
-        offset = d.pop("offset", UNSET)
-
         enabled = d.pop("enabled", UNSET)
 
         new_schedule = cls(
             path=path,
             schedule=schedule,
+            timezone=timezone,
             script_path=script_path,
             is_flow=is_flow,
             args=args,
-            offset=offset,
             enabled=enabled,
         )
 
         new_schedule.additional_properties = d
         return new_schedule
 
     @property
```

### Comparing `windmill_api-1.85.0/windmill_api/models/new_schedule_args.py` & `windmill_api-1.86.0/windmill_api/models/new_schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/new_token.py` & `windmill_api-1.86.0/windmill_api/models/new_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/new_user.py` & `windmill_api-1.86.0/windmill_api/models/new_user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow.py` & `windmill_api-1.86.0/windmill_api/models/open_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_schema.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_value_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_schema.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/open_flow_w_path_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/path_flow.py` & `windmill_api-1.86.0/windmill_api/models/path_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/path_flow_input_transforms.py` & `windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py` & `windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py` & `windmill_api-1.86.0/windmill_api/models/path_flow_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/path_script.py` & `windmill_api-1.86.0/windmill_api/models/path_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/path_script_input_transforms.py` & `windmill_api-1.86.0/windmill_api/models/path_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.86.0/windmill_api/models/path_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.86.0/windmill_api/models/path_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/policy.py` & `windmill_api-1.86.0/windmill_api/models/policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/policy_triggerables.py` & `windmill_api-1.86.0/windmill_api/models/policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/policy_triggerables_additional_property.py` & `windmill_api-1.86.0/windmill_api/models/policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/preview.py` & `windmill_api-1.86.0/windmill_api/models/preview.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/preview_args.py` & `windmill_api-1.86.0/windmill_api/models/preview_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/preview_schedule_json_body.py` & `windmill_api-1.86.0/windmill_api/models/update_resource_value_json_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,48 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PreviewScheduleJsonBody")
+T = TypeVar("T", bound="UpdateResourceValueJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class PreviewScheduleJsonBody:
+class UpdateResourceValueJsonBody:
     """
     Attributes:
-        schedule (str):
-        offset (Union[Unset, int]):
+        value (Union[Unset, Any]):
     """
 
-    schedule: str
-    offset: Union[Unset, int] = UNSET
+    value: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        schedule = self.schedule
-        offset = self.offset
+        value = self.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "schedule": schedule,
-            }
-        )
-        if offset is not UNSET:
-            field_dict["offset"] = offset
+        field_dict.update({})
+        if value is not UNSET:
+            field_dict["value"] = value
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        schedule = d.pop("schedule")
-
-        offset = d.pop("offset", UNSET)
+        value = d.pop("value", UNSET)
 
-        preview_schedule_json_body = cls(
-            schedule=schedule,
-            offset=offset,
+        update_resource_value_json_body = cls(
+            value=value,
         )
 
-        preview_schedule_json_body.additional_properties = d
-        return preview_schedule_json_body
+        update_resource_value_json_body.additional_properties = d
+        return update_resource_value_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200.py` & `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py` & `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py` & `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py` & `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_2.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py` & `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py` & `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py` & `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_3_object_item_typ_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py` & `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py` & `windmill_api-1.86.0/windmill_api/models/python_to_jsonschema_response_200_args_item_typ_type_4_list_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job.py` & `windmill_api-1.86.0/windmill_api/models/queued_job.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_args.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_flow_status.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_failure_module_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_approvers_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_branch_chosen.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_branchall.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_modules_item_iterator.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_flow_status_retry.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_flow_status_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/queued_job_raw_flow_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/raw_script.py` & `windmill_api-1.86.0/windmill_api/models/raw_script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/raw_script_input_transforms.py` & `windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py` & `windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms_additional_property_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py` & `windmill_api-1.86.0/windmill_api/models/raw_script_input_transforms_additional_property_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/refresh_token_json_body.py` & `windmill_api-1.86.0/windmill_api/models/refresh_token_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/remove_granular_acls_json_body.py` & `windmill_api-1.86.0/windmill_api/models/remove_granular_acls_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/remove_owner_to_folder_json_body.py` & `windmill_api-1.86.0/windmill_api/models/remove_owner_to_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/remove_user_to_group_json_body.py` & `windmill_api-1.86.0/windmill_api/models/remove_user_to_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/resource.py` & `windmill_api-1.86.0/windmill_api/models/resource.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/resource_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/resource_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/resource_type.py` & `windmill_api-1.86.0/windmill_api/models/resource_type.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py` & `windmill_api-1.86.0/windmill_api/models/resume_suspended_flow_as_owner_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/resume_suspended_job_post_json_body.py` & `windmill_api-1.86.0/windmill_api/models/resume_suspended_job_post_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/retry.py` & `windmill_api-1.86.0/windmill_api/models/retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_by_path_json_body.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_args.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/run_flow_preview_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_script_by_hash_json_body.py` & `windmill_api-1.86.0/windmill_api/models/run_script_by_hash_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_script_by_path_json_body.py` & `windmill_api-1.86.0/windmill_api/models/run_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_script_preview_json_body.py` & `windmill_api-1.86.0/windmill_api/models/run_script_preview_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_script_preview_json_body_args.py` & `windmill_api-1.86.0/windmill_api/models/run_script_preview_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py` & `windmill_api-1.86.0/windmill_api/models/run_wait_result_flow_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/run_wait_result_script_by_path_json_body.py` & `windmill_api-1.86.0/windmill_api/models/run_wait_result_script_by_path_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/schedule.py` & `windmill_api-1.86.0/windmill_api/models/get_schedule_response_200.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 import datetime
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.schedule_args import ScheduleArgs
-from ..models.schedule_extra_perms import ScheduleExtraPerms
+from ..models.get_schedule_response_200_args import GetScheduleResponse200Args
+from ..models.get_schedule_response_200_extra_perms import GetScheduleResponse200ExtraPerms
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Schedule")
+T = TypeVar("T", bound="GetScheduleResponse200")
 
 
 @attr.s(auto_attribs=True)
-class Schedule:
+class GetScheduleResponse200:
     """
     Attributes:
         path (str):
         edited_by (str):
         edited_at (datetime.datetime):
         schedule (str):
-        offset (int):
+        timezone (str):
         enabled (bool):
         script_path (str):
         is_flow (bool):
-        extra_perms (ScheduleExtraPerms):
+        extra_perms (GetScheduleResponse200ExtraPerms):
         email (str):
-        args (Union[Unset, ScheduleArgs]):
+        args (Union[Unset, GetScheduleResponse200Args]):
         error (Union[Unset, str]):
     """
 
     path: str
     edited_by: str
     edited_at: datetime.datetime
     schedule: str
-    offset: int
+    timezone: str
     enabled: bool
     script_path: str
     is_flow: bool
-    extra_perms: ScheduleExtraPerms
+    extra_perms: GetScheduleResponse200ExtraPerms
     email: str
-    args: Union[Unset, ScheduleArgs] = UNSET
+    args: Union[Unset, GetScheduleResponse200Args] = UNSET
     error: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         path = self.path
         edited_by = self.edited_by
         edited_at = self.edited_at.isoformat()
 
         schedule = self.schedule
-        offset = self.offset
+        timezone = self.timezone
         enabled = self.enabled
         script_path = self.script_path
         is_flow = self.is_flow
         extra_perms = self.extra_perms.to_dict()
 
         email = self.email
         args: Union[Unset, Dict[str, Any]] = UNSET
@@ -66,15 +66,15 @@
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "path": path,
                 "edited_by": edited_by,
                 "edited_at": edited_at,
                 "schedule": schedule,
-                "offset_": offset,
+                "timezone": timezone,
                 "enabled": enabled,
                 "script_path": script_path,
                 "is_flow": is_flow,
                 "extra_perms": extra_perms,
                 "email": email,
             }
         )
@@ -92,52 +92,52 @@
 
         edited_by = d.pop("edited_by")
 
         edited_at = isoparse(d.pop("edited_at"))
 
         schedule = d.pop("schedule")
 
-        offset = d.pop("offset_")
+        timezone = d.pop("timezone")
 
         enabled = d.pop("enabled")
 
         script_path = d.pop("script_path")
 
         is_flow = d.pop("is_flow")
 
-        extra_perms = ScheduleExtraPerms.from_dict(d.pop("extra_perms"))
+        extra_perms = GetScheduleResponse200ExtraPerms.from_dict(d.pop("extra_perms"))
 
         email = d.pop("email")
 
         _args = d.pop("args", UNSET)
-        args: Union[Unset, ScheduleArgs]
+        args: Union[Unset, GetScheduleResponse200Args]
         if isinstance(_args, Unset):
             args = UNSET
         else:
-            args = ScheduleArgs.from_dict(_args)
+            args = GetScheduleResponse200Args.from_dict(_args)
 
         error = d.pop("error", UNSET)
 
-        schedule = cls(
+        get_schedule_response_200 = cls(
             path=path,
             edited_by=edited_by,
             edited_at=edited_at,
             schedule=schedule,
-            offset=offset,
+            timezone=timezone,
             enabled=enabled,
             script_path=script_path,
             is_flow=is_flow,
             extra_perms=extra_perms,
             email=email,
             args=args,
             error=error,
         )
 
-        schedule.additional_properties = d
-        return schedule
+        get_schedule_response_200.additional_properties = d
+        return get_schedule_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.85.0/windmill_api/models/schedule_args.py` & `windmill_api-1.86.0/windmill_api/models/schedule_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/schedule_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/schedule_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/script.py` & `windmill_api-1.86.0/windmill_api/models/script.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/script_args.py` & `windmill_api-1.86.0/windmill_api/models/script_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/script_extra_perms.py` & `windmill_api-1.86.0/windmill_api/models/script_extra_perms.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/script_schema.py` & `windmill_api-1.86.0/windmill_api/models/script_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/set_password_json_body.py` & `windmill_api-1.86.0/windmill_api/models/set_password_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/set_schedule_enabled_json_body.py` & `windmill_api-1.86.0/windmill_api/models/set_schedule_enabled_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/slack_token.py` & `windmill_api-1.86.0/windmill_api/models/slack_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/slack_token_bot.py` & `windmill_api-1.86.0/windmill_api/models/slack_token_bot.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/star_json_body.py` & `windmill_api-1.86.0/windmill_api/models/star_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/static_transform.py` & `windmill_api-1.86.0/windmill_api/models/static_transform.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/token_response.py` & `windmill_api-1.86.0/windmill_api/models/token_response.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/truncated_token.py` & `windmill_api-1.86.0/windmill_api/models/truncated_token.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/unstar_json_body.py` & `windmill_api-1.86.0/windmill_api/models/unstar_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_app_json_body.py` & `windmill_api-1.86.0/windmill_api/models/update_app_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_app_json_body_policy.py` & `windmill_api-1.86.0/windmill_api/models/update_app_json_body_policy.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_app_json_body_policy_triggerables.py` & `windmill_api-1.86.0/windmill_api/models/update_app_json_body_policy_triggerables.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py` & `windmill_api-1.86.0/windmill_api/models/update_app_json_body_policy_triggerables_additional_property.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_schema.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_schema.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_failure_module_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_retry.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_constant.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_retry_exponential.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_0.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_sleep_type_1.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_stop_after_if.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py` & `windmill_api-1.86.0/windmill_api/models/update_flow_json_body_value_modules_item_suspend.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_folder_json_body.py` & `windmill_api-1.86.0/windmill_api/models/update_folder_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_group_json_body.py` & `windmill_api-1.86.0/windmill_api/models/update_group_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_resource_json_body.py` & `windmill_api-1.86.0/windmill_api/models/update_resource_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_resource_type_json_body.py` & `windmill_api-1.86.0/windmill_api/models/update_resource_type_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_resource_value_json_body.py` & `windmill_api-1.86.0/windmill_api/models/workspace.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,72 @@
 from typing import Any, Dict, List, Type, TypeVar, Union
 
 import attr
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="UpdateResourceValueJsonBody")
+T = TypeVar("T", bound="Workspace")
 
 
 @attr.s(auto_attribs=True)
-class UpdateResourceValueJsonBody:
+class Workspace:
     """
     Attributes:
-        value (Union[Unset, Any]):
+        id (str):
+        name (str):
+        owner (str):
+        domain (Union[Unset, str]):
     """
 
-    value: Union[Unset, Any] = UNSET
+    id: str
+    name: str
+    owner: str
+    domain: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        value = self.value
+        id = self.id
+        name = self.name
+        owner = self.owner
+        domain = self.domain
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if value is not UNSET:
-            field_dict["value"] = value
+        field_dict.update(
+            {
+                "id": id,
+                "name": name,
+                "owner": owner,
+            }
+        )
+        if domain is not UNSET:
+            field_dict["domain"] = domain
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        value = d.pop("value", UNSET)
+        id = d.pop("id")
+
+        name = d.pop("name")
+
+        owner = d.pop("owner")
+
+        domain = d.pop("domain", UNSET)
 
-        update_resource_value_json_body = cls(
-            value=value,
+        workspace = cls(
+            id=id,
+            name=name,
+            owner=owner,
+            domain=domain,
         )
 
-        update_resource_value_json_body.additional_properties = d
-        return update_resource_value_json_body
+        workspace.additional_properties = d
+        return workspace
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.85.0/windmill_api/models/update_schedule_json_body.py` & `windmill_api-1.86.0/windmill_api/models/update_schedule_json_body.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,45 +8,52 @@
 
 
 @attr.s(auto_attribs=True)
 class UpdateScheduleJsonBody:
     """
     Attributes:
         schedule (str):
+        timezone (str):
         args (UpdateScheduleJsonBodyArgs):
     """
 
     schedule: str
+    timezone: str
     args: UpdateScheduleJsonBodyArgs
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         schedule = self.schedule
+        timezone = self.timezone
         args = self.args.to_dict()
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "schedule": schedule,
+                "timezone": timezone,
                 "args": args,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         schedule = d.pop("schedule")
 
+        timezone = d.pop("timezone")
+
         args = UpdateScheduleJsonBodyArgs.from_dict(d.pop("args"))
 
         update_schedule_json_body = cls(
             schedule=schedule,
+            timezone=timezone,
             args=args,
         )
 
         update_schedule_json_body.additional_properties = d
         return update_schedule_json_body
 
     @property
```

### Comparing `windmill_api-1.85.0/windmill_api/models/update_schedule_json_body_args.py` & `windmill_api-1.86.0/windmill_api/models/update_schedule_json_body_args.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_user_json_body.py` & `windmill_api-1.86.0/windmill_api/models/update_user_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/update_variable_json_body.py` & `windmill_api-1.86.0/windmill_api/models/update_variable_json_body.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/usage.py` & `windmill_api-1.86.0/windmill_api/models/usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/user.py` & `windmill_api-1.86.0/windmill_api/models/user.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/user_usage.py` & `windmill_api-1.86.0/windmill_api/models/user_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/user_workspace_list.py` & `windmill_api-1.86.0/windmill_api/models/user_workspace_list.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/user_workspace_list_workspaces_item.py` & `windmill_api-1.86.0/windmill_api/models/user_workspace_list_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/whoami_response_200.py` & `windmill_api-1.86.0/windmill_api/models/whoami_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/whoami_response_200_usage.py` & `windmill_api-1.86.0/windmill_api/models/whoami_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/whois_response_200.py` & `windmill_api-1.86.0/windmill_api/models/whois_response_200.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/whois_response_200_usage.py` & `windmill_api-1.86.0/windmill_api/models/whois_response_200_usage.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/worker_ping.py` & `windmill_api-1.86.0/windmill_api/models/worker_ping.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/windmill_api/models/workspace.py` & `windmill_api-1.86.0/windmill_api/models/workspace_invite.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,69 @@
-from typing import Any, Dict, List, Type, TypeVar, Union
+from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-from ..types import UNSET, Unset
-
-T = TypeVar("T", bound="Workspace")
+T = TypeVar("T", bound="WorkspaceInvite")
 
 
 @attr.s(auto_attribs=True)
-class Workspace:
+class WorkspaceInvite:
     """
     Attributes:
-        id (str):
-        name (str):
-        owner (str):
-        domain (Union[Unset, str]):
+        workspace_id (str):
+        email (str):
+        is_admin (bool):
+        operator (bool):
     """
 
-    id: str
-    name: str
-    owner: str
-    domain: Union[Unset, str] = UNSET
+    workspace_id: str
+    email: str
+    is_admin: bool
+    operator: bool
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-        name = self.name
-        owner = self.owner
-        domain = self.domain
+        workspace_id = self.workspace_id
+        email = self.email
+        is_admin = self.is_admin
+        operator = self.operator
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "id": id,
-                "name": name,
-                "owner": owner,
+                "workspace_id": workspace_id,
+                "email": email,
+                "is_admin": is_admin,
+                "operator": operator,
             }
         )
-        if domain is not UNSET:
-            field_dict["domain"] = domain
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        id = d.pop("id")
+        workspace_id = d.pop("workspace_id")
 
-        name = d.pop("name")
+        email = d.pop("email")
 
-        owner = d.pop("owner")
+        is_admin = d.pop("is_admin")
 
-        domain = d.pop("domain", UNSET)
+        operator = d.pop("operator")
 
-        workspace = cls(
-            id=id,
-            name=name,
-            owner=owner,
-            domain=domain,
+        workspace_invite = cls(
+            workspace_id=workspace_id,
+            email=email,
+            is_admin=is_admin,
+            operator=operator,
         )
 
-        workspace.additional_properties = d
-        return workspace
+        workspace_invite.additional_properties = d
+        return workspace_invite
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `windmill_api-1.85.0/windmill_api/types.py` & `windmill_api-1.86.0/windmill_api/types.py`

 * *Files identical despite different names*

### Comparing `windmill_api-1.85.0/setup.py` & `windmill_api-1.86.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 {'': ['*']}
 
 install_requires = \
 ['attrs>=21.3.0', 'httpx>=0.15.4,<0.24.0', 'python-dateutil>=2.8.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'windmill-api',
-    'version': '1.85.0',
+    'version': '1.86.0',
     'description': 'A client library for accessing Windmill API',
     'long_description': '# Autogenerated Windmill OpenApi Client\nThis is the raw autogenerated api client. You are most likely more interested in [wmill](https://pypi.org/project/wmill/) which leverages this client to offer an user friendly experience. We use [this openapi python client generator](https://github.com/openapi-generators/openapi-python-client/)\n\n# windmill-api\nA client library for accessing Windmill API\n\n## Usage\nFirst, create a client:\n\n```python\nfrom windmill_api import Client\n\nclient = Client(base_url="https://api.example.com")\n```\n\nIf the endpoints you\'re going to hit require authentication, use `AuthenticatedClient` instead:\n\n```python\nfrom windmill_api import AuthenticatedClient\n\nclient = AuthenticatedClient(base_url="https://api.example.com", token="SuperSecretToken")\n```\n\nNow call your endpoint and use your models:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = get_my_data_model.sync(client=client)\n# or if you need more info (e.g. status_code)\nresponse: Response[MyDataModel] = get_my_data_model.sync_detailed(client=client)\n```\n\nOr do the same thing with an async version:\n\n```python\nfrom windmill_api.models import MyDataModel\nfrom windmill_api.api.my_tag import get_my_data_model\nfrom windmill_api.types import Response\n\nmy_data: MyDataModel = await get_my_data_model.asyncio(client=client)\nresponse: Response[MyDataModel] = await get_my_data_model.asyncio_detailed(client=client)\n```\n\nBy default, when you\'re calling an HTTPS API it will attempt to verify that SSL is working correctly. Using certificate verification is highly recommended most of the time, but sometimes you may need to authenticate to a server (especially an internal server) using a custom certificate bundle.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken",\n    verify_ssl="/path/to/certificate_bundle.pem",\n)\n```\n\nYou can also disable certificate validation altogether, but beware that **this is a security risk**.\n\n```python\nclient = AuthenticatedClient(\n    base_url="https://internal_api.example.com", \n    token="SuperSecretToken", \n    verify_ssl=False\n)\n```\n\nThings to know:\n1. Every path/method combo becomes a Python module with four functions:\n    1. `sync`: Blocking request that returns parsed data (if successful) or `None`\n    1. `sync_detailed`: Blocking request that always returns a `Request`, optionally with `parsed` set if the request was successful.\n    1. `asyncio`: Like `sync` but async instead of blocking\n    1. `asyncio_detailed`: Like `sync_detailed` but async instead of blocking\n\n1. All path/query params, and bodies become method arguments.\n1. If your endpoint had any tags on it, the first tag will be used as a module name for the function (my_tag above)\n1. Any endpoint which did not have a tag will be in `windmill_api.api.default`\n\n',
     'author': 'Ruben Fiszel',
     'author_email': 'ruben@windmill.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `windmill_api-1.85.0/PKG-INFO` & `windmill_api-1.86.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windmill-api
-Version: 1.85.0
+Version: 1.86.0
 Summary: A client library for accessing Windmill API
 License: Apache-2.0
 Author: Ruben Fiszel
 Author-email: ruben@windmill.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

