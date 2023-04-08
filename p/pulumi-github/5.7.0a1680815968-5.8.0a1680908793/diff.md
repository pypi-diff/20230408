# Comparing `tmp/pulumi_github-5.7.0a1680815968.tar.gz` & `tmp/pulumi_github-5.8.0a1680908793.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_github-5.7.0a1680815968.tar", last modified: Thu Apr  6 21:24:05 2023, max compression
+gzip compressed data, was "pulumi_github-5.8.0a1680908793.tar", last modified: Fri Apr  7 23:18:34 2023, max compression
```

## Comparing `pulumi_github-5.7.0a1680815968.tar` & `pulumi_github-5.8.0a1680908793.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:24:05.080604 pulumi_github-5.7.0a1680815968/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-06 21:24:05.080604 pulumi_github-5.7.0a1680815968/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:24:05.080604 pulumi_github-5.7.0a1680815968/pulumi_github/
--rw-r--r--   0 runner    (1001) docker     (123)    15450 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63092 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19178 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/actions_environment_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/actions_environment_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/actions_organization_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/actions_organization_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/actions_organization_secret_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/actions_organization_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/actions_repository_access_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/actions_repository_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25998 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/actions_runner_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/actions_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/actions_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/app_installation_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/app_installation_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/branch_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    44058 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/branch_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    31972 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/branch_protection_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:24:05.080604 pulumi_github-5.7.0a1680815968/pulumi_github/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/dependabot_organization_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/dependabot_organization_secret_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/dependabot_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/emu_group_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    14476 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/enterprise_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_environment_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_organization_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_organization_registration_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_organization_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_organization_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_registration_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_collaborators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_dependabot_organization_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_dependabot_organization_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_dependabot_public_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_dependabot_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_external_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_github_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_organization_ip_allow_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_organization_team_sync_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_organization_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_organization_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_release.py
--rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)    20234 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_pull_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_pull_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_team.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/issue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/issue_label.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/organization_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/organization_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/organization_security_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    79808 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/organization_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    15058 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/organization_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)   102405 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15743 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/project_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/project_column.py
--rw-r--r--   0 runner    (1001) docker     (123)    14143 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28755 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/release.py
--rw-r--r--   0 runner    (1001) docker     (123)   107291 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/repository_autolink_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    21061 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/repository_collaborator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/repository_collaborators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/repository_deploy_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/repository_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    27314 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/repository_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/repository_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/repository_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    28682 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/repository_pull_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/repository_tag_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/repository_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/team_members.py
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/team_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/team_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/team_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/team_sync_group_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/user_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/user_invitation_accepter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/pulumi_github/user_ssh_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 21:24:05.080604 pulumi_github-5.7.0a1680815968/pulumi_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-06 21:24:05.000000 pulumi_github-5.7.0a1680815968/pulumi_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-04-06 21:24:05.000000 pulumi_github-5.7.0a1680815968/pulumi_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 21:24:05.000000 pulumi_github-5.7.0a1680815968/pulumi_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 21:24:05.000000 pulumi_github-5.7.0a1680815968/pulumi_github.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-06 21:24:05.000000 pulumi_github-5.7.0a1680815968/pulumi_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-06 21:24:05.000000 pulumi_github-5.7.0a1680815968/pulumi_github.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 21:24:05.080604 pulumi_github-5.7.0a1680815968/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-06 21:24:04.000000 pulumi_github-5.7.0a1680815968/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:18:34.158939 pulumi_github-5.8.0a1680908793/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-07 23:18:34.158939 pulumi_github-5.8.0a1680908793/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:18:34.158939 pulumi_github-5.8.0a1680908793/pulumi_github/
+-rw-r--r--   0 runner    (1001) docker     (123)    15450 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63092 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19178 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/actions_environment_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16013 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/actions_environment_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9151 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20745 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/actions_organization_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22394 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/actions_organization_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/actions_organization_secret_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/actions_organization_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/actions_repository_access_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14803 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/actions_repository_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25998 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/actions_runner_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15530 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/actions_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/actions_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/app_installation_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/app_installation_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/branch_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44058 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/branch_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31972 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/branch_protection_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:18:34.158939 pulumi_github-5.8.0a1680908793/pulumi_github/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/dependabot_organization_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/dependabot_organization_secret_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14359 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/dependabot_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/emu_group_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14476 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/enterprise_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_environment_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_organization_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_organization_registration_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_organization_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_organization_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_registration_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_collaborators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_dependabot_organization_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_dependabot_organization_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_dependabot_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_dependabot_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_external_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_github_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_organization_ip_allow_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_organization_team_sync_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_organization_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_organization_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_release.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7590 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20234 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_pull_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9795 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_pull_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13277 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/issue_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6674 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/organization_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8955 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/organization_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/organization_security_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79808 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/organization_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15058 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/organization_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102405 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15743 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/project_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/project_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14143 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28755 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/release.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107291 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/repository_autolink_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21061 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/repository_collaborator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17395 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/repository_collaborators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/repository_deploy_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/repository_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27314 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17109 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/repository_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/repository_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28682 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/repository_pull_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/repository_tag_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/repository_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22137 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11019 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/team_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/team_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/team_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16613 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/team_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10810 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/team_sync_group_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/user_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8960 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/user_invitation_accepter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/pulumi_github/user_ssh_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:18:34.158939 pulumi_github-5.8.0a1680908793/pulumi_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-07 23:18:34.000000 pulumi_github-5.8.0a1680908793/pulumi_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-04-07 23:18:34.000000 pulumi_github-5.8.0a1680908793/pulumi_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:18:34.000000 pulumi_github-5.8.0a1680908793/pulumi_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:18:34.000000 pulumi_github-5.8.0a1680908793/pulumi_github.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 23:18:34.000000 pulumi_github-5.8.0a1680908793/pulumi_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 23:18:34.000000 pulumi_github-5.8.0a1680908793/pulumi_github.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 23:18:34.158939 pulumi_github-5.8.0a1680908793/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-07 23:18:33.000000 pulumi_github-5.8.0a1680908793/setup.py
```

### Comparing `pulumi_github-5.7.0a1680815968/PKG-INFO` & `pulumi_github-5.8.0a1680908793/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_github
-Version: 5.7.0a1680815968
+Version: 5.8.0a1680908793
 Summary: A Pulumi package for creating and managing github cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-github
 Keywords: pulumi github
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_github-5.7.0a1680815968/README.md` & `pulumi_github-5.8.0a1680908793/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/__init__.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/_inputs.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/_utilities.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/actions_environment_secret.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/actions_environment_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/actions_environment_variable.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/actions_environment_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/actions_organization_oidc_subject_claim_customization_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/actions_organization_permissions.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/actions_organization_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/actions_organization_secret.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/actions_organization_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/actions_organization_secret_repositories.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/actions_organization_secret_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/actions_organization_variable.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/actions_organization_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/actions_repository_access_level.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/actions_repository_access_level.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/actions_repository_oidc_subject_claim_customization_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/actions_repository_permissions.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/actions_repository_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/actions_runner_group.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/actions_runner_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/actions_secret.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/actions_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/actions_variable.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/actions_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/app_installation_repositories.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/app_installation_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/app_installation_repository.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/app_installation_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/branch.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/branch_default.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/branch_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/branch_protection.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/branch_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/branch_protection_v3.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/branch_protection_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/config/outputs.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/config/vars.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/dependabot_organization_secret.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/dependabot_organization_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/dependabot_organization_secret_repositories.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/dependabot_organization_secret_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/dependabot_secret.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/dependabot_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/emu_group_mapping.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/emu_group_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/enterprise_organization.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/enterprise_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_environment_secrets.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_environment_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_environment_variables.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_environment_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_organization_oidc_subject_claim_customization_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_organization_public_key.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_organization_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_organization_registration_token.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_organization_registration_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_organization_secrets.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_organization_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_organization_variables.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_organization_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_public_key.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_registration_token.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_registration_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_repository_oidc_subject_claim_customization_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_secrets.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_actions_variables.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_actions_variables.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_branch.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_collaborators.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_collaborators.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_dependabot_organization_public_key.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_dependabot_organization_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_dependabot_organization_secrets.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_dependabot_organization_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_dependabot_public_key.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_dependabot_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_dependabot_secrets.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_dependabot_secrets.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_enterprise.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_enterprise.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_external_groups.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_external_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_github_app.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_github_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_ip_ranges.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_membership.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_organization.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_organization_ip_allow_list.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_organization_ip_allow_list.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_organization_team_sync_groups.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_organization_team_sync_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_organization_teams.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_organization_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_organization_webhooks.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_organization_webhooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_ref.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_ref.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_release.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_release.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_repositories.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_repository.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_branches.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_branches.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_deploy_keys.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_file.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_milestone.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_pull_request.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_pull_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_pull_requests.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_teams.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_repository_webhooks.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_repository_webhooks.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_ssh_keys.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_team.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_tree.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_tree.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_user.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/get_users.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/issue.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/issue.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/issue_label.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/issue_label.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/membership.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/organization_block.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/organization_block.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/organization_project.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/organization_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/organization_security_manager.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/organization_security_manager.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/organization_settings.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/organization_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/organization_webhook.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/organization_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/outputs.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/project_card.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/project_card.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/project_column.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/project_column.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/provider.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/release.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/release.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/repository.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/repository_autolink_reference.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/repository_autolink_reference.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/repository_collaborator.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/repository_collaborator.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/repository_collaborators.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/repository_collaborators.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/repository_deploy_key.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/repository_deploy_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/repository_environment.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/repository_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/repository_file.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/repository_milestone.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/repository_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/repository_project.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/repository_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/repository_pull_request.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/repository_pull_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/repository_tag_protection.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/repository_tag_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/repository_webhook.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/repository_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/team.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/team_members.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/team_members.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/team_membership.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/team_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/team_repository.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/team_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/team_settings.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/team_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/team_sync_group_mapping.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/team_sync_group_mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/user_gpg_key.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/user_gpg_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/user_invitation_accepter.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/user_invitation_accepter.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github/user_ssh_key.py` & `pulumi_github-5.8.0a1680908793/pulumi_github/user_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github.egg-info/PKG-INFO` & `pulumi_github-5.8.0a1680908793/pulumi_github.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-github
-Version: 5.7.0a1680815968
+Version: 5.8.0a1680908793
 Summary: A Pulumi package for creating and managing github cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-github
 Keywords: pulumi github
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_github-5.7.0a1680815968/pulumi_github.egg-info/SOURCES.txt` & `pulumi_github-5.8.0a1680908793/pulumi_github.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_github-5.7.0a1680815968/setup.py` & `pulumi_github-5.8.0a1680908793/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "5.7.0a1680815968"
-PLUGIN_VERSION = "5.7.0-alpha.1680815968+cd8957eb"
+VERSION = "5.8.0a1680908793"
+PLUGIN_VERSION = "5.8.0-alpha.1680908793+a30b6472"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'github', PLUGIN_VERSION])
         except OSError as error:
```

