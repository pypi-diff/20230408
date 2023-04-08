# Comparing `tmp/pulumi_gitlab-4.9.0.tar.gz` & `tmp/pulumi_gitlab-4.9.0a1666628674.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_gitlab-4.9.0.tar", last modified: Tue Oct 25 16:53:57 2022, max compression
+gzip compressed data, was "pulumi_gitlab-4.9.0a1666628674.tar", last modified: Mon Oct 24 16:29:17 2022, max compression
```

## Comparing `pulumi_gitlab-4.9.0.tar` & `pulumi_gitlab-4.9.0a1666628674.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 16:53:57.509333 pulumi_gitlab-4.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-10-25 16:53:57.509333 pulumi_gitlab-4.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 16:53:57.509333 pulumi_gitlab-4.9.0/pulumi_gitlab/
--rw-r--r--   0 runner    (1001) docker     (121)    15068 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    41789 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)   690957 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/application_settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    19660 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/branch.py
--rw-r--r--   0 runner    (1001) docker     (121)    30500 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/branch_protection.py
--rw-r--r--   0 runner    (1001) docker     (121)    13955 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/cluster_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)    19017 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/cluster_agent_token.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 16:53:57.509333 pulumi_gitlab-4.9.0/pulumi_gitlab/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3088 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)    12989 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/deploy_key.py
--rw-r--r--   0 runner    (1001) docker     (121)    15428 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/deploy_key_enable.py
--rw-r--r--   0 runner    (1001) docker     (121)    18697 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/deploy_token.py
--rw-r--r--   0 runner    (1001) docker     (121)     7828 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_branch.py
--rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_cluster_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     4050 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_cluster_agents.py
--rw-r--r--   0 runner    (1001) docker     (121)     5799 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_current_user.py
--rw-r--r--   0 runner    (1001) docker     (121)    10244 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    13528 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_group_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_group_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)     5806 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_group_membership.py
--rw-r--r--   0 runner    (1001) docker     (121)     7546 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_group_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)     5058 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_group_variables.py
--rw-r--r--   0 runner    (1001) docker     (121)     4193 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_instance_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_instance_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_instance_variables.py
--rw-r--r--   0 runner    (1001) docker     (121)    37320 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_project.py
--rw-r--r--   0 runner    (1001) docker     (121)    13666 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)     3810 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)    24426 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_issue.py
--rw-r--r--   0 runner    (1001) docker     (121)    30589 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_issues.py
--rw-r--r--   0 runner    (1001) docker     (121)     6569 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_membership.py
--rw-r--r--   0 runner    (1001) docker     (121)     9546 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_milestone.py
--rw-r--r--   0 runner    (1001) docker     (121)     8568 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_milestones.py
--rw-r--r--   0 runner    (1001) docker     (121)     7308 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_protected_branch.py
--rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_protected_branches.py
--rw-r--r--   0 runner    (1001) docker     (121)     6221 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)     6653 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_tags.py
--rw-r--r--   0 runner    (1001) docker     (121)     7672 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)     5182 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_variables.py
--rw-r--r--   0 runner    (1001) docker     (121)    24027 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (121)     7918 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_release_link.py
--rw-r--r--   0 runner    (1001) docker     (121)     4588 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_release_links.py
--rw-r--r--   0 runner    (1001) docker     (121)     9387 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_repository_tree.py
--rw-r--r--   0 runner    (1001) docker     (121)    16997 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_user.py
--rw-r--r--   0 runner    (1001) docker     (121)    11124 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/get_users.py
--rw-r--r--   0 runner    (1001) docker     (121)    50120 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/group.py
--rw-r--r--   0 runner    (1001) docker     (121)    23419 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/group_access_token.py
--rw-r--r--   0 runner    (1001) docker     (121)    13282 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/group_badge.py
--rw-r--r--   0 runner    (1001) docker     (121)    33679 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/group_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    10032 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/group_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)    46605 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/group_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)    12990 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/group_label.py
--rw-r--r--   0 runner    (1001) docker     (121)    21224 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/group_ldap_link.py
--rw-r--r--   0 runner    (1001) docker     (121)    20006 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/group_membership.py
--rw-r--r--   0 runner    (1001) docker     (121)    11204 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/group_project_file_template.py
--rw-r--r--   0 runner    (1001) docker     (121)    11025 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/group_saml_link.py
--rw-r--r--   0 runner    (1001) docker     (121)    14114 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/group_share_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    21008 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/group_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)    34419 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/instance_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    16259 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/instance_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)    13356 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/label.py
--rw-r--r--   0 runner    (1001) docker     (121)    13496 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/managed_license.py
--rw-r--r--   0 runner    (1001) docker     (121)   143765 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    20048 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/personal_access_token.py
--rw-r--r--   0 runner    (1001) docker     (121)    16323 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (121)    13430 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/pipeline_schedule_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)     9919 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/pipeline_trigger.py
--rw-r--r--   0 runner    (1001) docker     (121)   207341 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project.py
--rw-r--r--   0 runner    (1001) docker     (121)    22325 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_access_token.py
--rw-r--r--   0 runner    (1001) docker     (121)    21004 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_approval_rule.py
--rw-r--r--   0 runner    (1001) docker     (121)    14991 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_badge.py
--rw-r--r--   0 runner    (1001) docker     (121)    36176 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_cluster.py
--rw-r--r--   0 runner    (1001) docker     (121)    10174 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)    18418 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)    13439 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_freeze_period.py
--rw-r--r--   0 runner    (1001) docker     (121)    43374 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)    74557 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_issue.py
--rw-r--r--   0 runner    (1001) docker     (121)    23095 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_issue_board.py
--rw-r--r--   0 runner    (1001) docker     (121)    24116 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_level_mr_approvals.py
--rw-r--r--   0 runner    (1001) docker     (121)    14008 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_membership.py
--rw-r--r--   0 runner    (1001) docker     (121)    25238 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_milestone.py
--rw-r--r--   0 runner    (1001) docker     (121)    17018 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_mirror.py
--rw-r--r--   0 runner    (1001) docker     (121)    19969 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_protected_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     9163 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_runner_enablement.py
--rw-r--r--   0 runner    (1001) docker     (121)    15179 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_share_group.py
--rw-r--r--   0 runner    (1001) docker     (121)    17670 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_tag.py
--rw-r--r--   0 runner    (1001) docker     (121)    21758 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/project_variable.py
--rw-r--r--   0 runner    (1001) docker     (121)    16195 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    21523 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/release_link.py
--rw-r--r--   0 runner    (1001) docker     (121)    30915 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/repository_file.py
--rw-r--r--   0 runner    (1001) docker     (121)    24337 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/runner.py
--rw-r--r--   0 runner    (1001) docker     (121)    15306 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/service_external_wiki.py
--rw-r--r--   0 runner    (1001) docker     (121)    18963 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/service_github.py
--rw-r--r--   0 runner    (1001) docker     (121)    45107 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/service_jira.py
--rw-r--r--   0 runner    (1001) docker     (121)    37739 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/service_microsoft_teams.py
--rw-r--r--   0 runner    (1001) docker     (121)    15484 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/service_pipelines_email.py
--rw-r--r--   0 runner    (1001) docker     (121)    59413 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/service_slack.py
--rw-r--r--   0 runner    (1001) docker     (121)    21890 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/system_hook.py
--rw-r--r--   0 runner    (1001) docker     (121)    10971 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/tag_protection.py
--rw-r--r--   0 runner    (1001) docker     (121)    20056 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/topic.py
--rw-r--r--   0 runner    (1001) docker     (121)    32444 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     9949 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/user_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (121)    13260 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/user_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (121)    15378 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab/user_ssh_key.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-25 16:53:57.509333 pulumi_gitlab-4.9.0/pulumi_gitlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3261 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/pulumi_gitlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-25 16:53:57.509333 pulumi_gitlab-4.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2081 2022-10-25 16:53:57.000000 pulumi_gitlab-4.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 16:29:17.455358 pulumi_gitlab-4.9.0a1666628674/
+-rw-r--r--   0 runner    (1001) docker     (121)     3272 2022-10-24 16:29:17.455358 pulumi_gitlab-4.9.0a1666628674/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2935 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 16:29:17.455358 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/
+-rw-r--r--   0 runner    (1001) docker     (121)    15068 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41789 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)   690957 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19660 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/branch.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30500 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/branch_protection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13955 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/cluster_agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19017 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/cluster_agent_token.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 16:29:17.455358 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3088 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12989 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/deploy_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15428 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/deploy_key_enable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18697 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/deploy_token.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7828 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_branch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_cluster_agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4050 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_cluster_agents.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5799 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_current_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10244 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13528 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3305 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5806 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7546 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_variable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5058 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4193 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_instance_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5347 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_instance_variable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2426 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_instance_variables.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37320 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13666 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3810 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24426 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_issue.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30589 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_issues.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6569 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_membership.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9546 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8568 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_milestones.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7308 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_protected_branch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4484 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_protected_branches.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6221 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6653 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7672 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_variable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5182 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_variables.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24027 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7918 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_release_link.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4588 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_release_links.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9387 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6384 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_repository_tree.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16997 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11124 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50120 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23419 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13282 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_badge.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33679 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10032 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46605 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12990 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_label.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21224 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_ldap_link.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20006 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11204 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_project_file_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11025 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_saml_link.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14114 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_share_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21008 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_variable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34419 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/instance_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16259 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/instance_variable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13356 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/label.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13496 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/managed_license.py
+-rw-r--r--   0 runner    (1001) docker     (121)   143765 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20048 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/personal_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16323 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13430 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/pipeline_schedule_variable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9919 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/pipeline_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (121)   207341 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22325 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21004 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_approval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14991 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_badge.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36176 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10174 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18418 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13439 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_freeze_period.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43374 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)    74557 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_issue.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23095 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_issue_board.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24116 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_level_mr_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14008 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_membership.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25238 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17018 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19969 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_protected_environment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9163 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_runner_enablement.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15179 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_share_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17670 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_tag.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21758 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_variable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16195 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    21523 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/release_link.py
+-rw-r--r--   0 runner    (1001) docker     (121)    30915 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24337 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/runner.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15306 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_external_wiki.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18963 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_github.py
+-rw-r--r--   0 runner    (1001) docker     (121)    45107 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_jira.py
+-rw-r--r--   0 runner    (1001) docker     (121)    37739 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_microsoft_teams.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15484 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_pipelines_email.py
+-rw-r--r--   0 runner    (1001) docker     (121)    59413 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_slack.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21890 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/system_hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10971 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/tag_protection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20056 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/topic.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32444 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9949 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13260 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15378 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user_ssh_key.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 16:29:17.455358 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3272 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-24 16:29:17.455358 pulumi_gitlab-4.9.0a1666628674/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2118 2022-10-24 16:29:17.000000 pulumi_gitlab-4.9.0a1666628674/setup.py
```

### Comparing `pulumi_gitlab-4.9.0/PKG-INFO` & `pulumi_gitlab-4.9.0a1666628674/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_gitlab
-Version: 4.9.0
+Version: 4.9.0a1666628674
 Summary: A Pulumi package for creating and managing GitLab resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-gitlab
 Keywords: pulumi gitlab
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_gitlab-4.9.0/README.md` & `pulumi_gitlab-4.9.0a1666628674/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/__init__.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/_inputs.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/_utilities.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/application_settings.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/application_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/branch.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/branch_protection.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/branch_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/cluster_agent.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/cluster_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/cluster_agent_token.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/cluster_agent_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/config/vars.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/deploy_key.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/deploy_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/deploy_key_enable.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/deploy_key_enable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/deploy_token.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/deploy_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_branch.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_cluster_agent.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_cluster_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_cluster_agents.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_cluster_agents.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_current_user.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_current_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_group.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_group_hook.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_group_hooks.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_hooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_group_membership.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_group_variable.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_group_variables.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_group_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_instance_deploy_keys.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_instance_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_instance_variable.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_instance_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_instance_variables.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_instance_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_project.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_hook.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_hooks.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_hooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_issue.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_issue.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_issues.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_issues.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_membership.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_milestone.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_milestones.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_milestones.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_protected_branch.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_protected_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_protected_branches.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_protected_branches.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_tag.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_tags.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_tags.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_variable.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_project_variables.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_project_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_projects.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_projects.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_release_link.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_release_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_release_links.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_release_links.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_repository_file.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_repository_tree.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_repository_tree.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_user.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/get_users.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/group.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/group_access_token.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/group_badge.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_badge.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/group_cluster.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/group_custom_attribute.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/group_hook.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/group_label.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_label.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/group_ldap_link.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_ldap_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/group_membership.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/group_project_file_template.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_project_file_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/group_saml_link.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_saml_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/group_share_group.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_share_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/group_variable.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/group_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/instance_cluster.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/instance_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/instance_variable.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/instance_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/label.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/label.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/managed_license.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/managed_license.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/outputs.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/personal_access_token.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/personal_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/pipeline_schedule.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/pipeline_schedule_variable.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/pipeline_schedule_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/pipeline_trigger.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/pipeline_trigger.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_access_token.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_approval_rule.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_approval_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_badge.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_badge.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_cluster.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_custom_attribute.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_environment.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_freeze_period.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_freeze_period.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_hook.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_issue.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_issue.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_issue_board.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_issue_board.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_level_mr_approvals.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_level_mr_approvals.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_membership.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_milestone.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_mirror.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_mirror.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_protected_environment.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_protected_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_runner_enablement.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_runner_enablement.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_share_group.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_share_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_tag.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/project_variable.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/project_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/provider.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/release_link.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/release_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/repository_file.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/runner.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/runner.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/service_external_wiki.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_external_wiki.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/service_github.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/service_jira.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_jira.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/service_microsoft_teams.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_microsoft_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/service_pipelines_email.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_pipelines_email.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/service_slack.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/service_slack.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/system_hook.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/system_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/tag_protection.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/tag_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/topic.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/user.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/user_custom_attribute.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/user_gpg_key.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user_gpg_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab/user_ssh_key.py` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab/user_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab.egg-info/PKG-INFO` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-gitlab
-Version: 4.9.0
+Version: 4.9.0a1666628674
 Summary: A Pulumi package for creating and managing GitLab resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-gitlab
 Keywords: pulumi gitlab
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_gitlab-4.9.0/pulumi_gitlab.egg-info/SOURCES.txt` & `pulumi_gitlab-4.9.0a1666628674/pulumi_gitlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-4.9.0/setup.py` & `pulumi_gitlab-4.9.0a1666628674/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.9.0"
-PLUGIN_VERSION = "4.9.0"
+VERSION = "4.9.0a1666628674"
+PLUGIN_VERSION = "4.9.0-alpha.1666628674+a29b05ea"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'gitlab', PLUGIN_VERSION])
         except OSError as error:
```

