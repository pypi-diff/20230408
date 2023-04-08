# Comparing `tmp/pulumi_consul-3.9.0a1679413309.tar.gz` & `tmp/pulumi_consul-3.9.0a1680908224.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_consul-3.9.0a1679413309.tar", last modified: Tue Mar 21 15:56:36 2023, max compression
+gzip compressed data, was "pulumi_consul-3.9.0a1680908224.tar", last modified: Fri Apr  7 23:04:54 2023, max compression
```

## Comparing `pulumi_consul-3.9.0a1679413309.tar` & `pulumi_consul-3.9.0a1680908224.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:56:36.273754 pulumi_consul-3.9.0a1679413309/
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-03-21 15:56:36.273754 pulumi_consul-3.9.0a1679413309/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:56:36.273754 pulumi_consul-3.9.0a1679413309/pulumi_consul/
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63113 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    32057 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/acl_auth_method.py
--rw-r--r--   0 runner    (1001) docker     (123)    19649 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/acl_binding_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    15617 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/acl_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/acl_role.py
--rw-r--r--   0 runner    (1001) docker     (123)    27926 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/acl_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/acl_token_policy_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/acl_token_role_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/admin_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)    12984 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/agent_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    28074 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/autopilot_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17952 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/catalog_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/certificate_authority.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:56:36.273754 pulumi_consul-3.9.0a1679413309/pulumi_consul/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    26665 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/config_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_acl_auth_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_acl_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_acl_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_acl_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_acl_token_secret_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_agent_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    40338 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_agent_self.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_autopilot_health.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_catalog_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_catalog_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_catalog_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_config_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_key_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_network_area_members.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_network_segments.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_peering.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_peerings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_service_health.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)    25887 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/intention.py
--rw-r--r--   0 runner    (1001) docker     (123)    25562 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/key_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/license.py
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/namespace_policy_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/namespace_role_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    18835 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/network_area.py
--rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    89118 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/peering.py
--rw-r--r--   0 runner    (1001) docker     (123)    14132 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/peering_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    51836 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/prepared_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34646 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul/service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 15:56:36.273754 pulumi_consul-3.9.0a1679413309/pulumi_consul.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/pulumi_consul.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 15:56:36.273754 pulumi_consul-3.9.0a1679413309/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-03-21 15:56:36.000000 pulumi_consul-3.9.0a1679413309/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:04:54.381832 pulumi_consul-3.9.0a1680908224/
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-07 23:04:54.381832 pulumi_consul-3.9.0a1680908224/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:04:54.381832 pulumi_consul-3.9.0a1680908224/pulumi_consul/
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63113 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32057 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/acl_auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19649 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/acl_binding_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15617 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/acl_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20703 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/acl_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27926 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/acl_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/acl_token_policy_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/acl_token_role_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/admin_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12984 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/agent_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28074 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/autopilot_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17952 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/catalog_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/certificate_authority.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:04:54.381832 pulumi_consul-3.9.0a1680908224/pulumi_consul/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26665 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/config_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_acl_auth_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_acl_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_acl_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8984 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_acl_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6833 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_acl_token_secret_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40338 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_agent_self.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_autopilot_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_catalog_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_catalog_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_catalog_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_config_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_key_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_network_area_members.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_network_segments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_peerings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_service_health.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25887 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/intention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25562 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/key_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19688 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/namespace_policy_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8087 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/namespace_role_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18835 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/network_area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89118 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21184 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14132 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/peering_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51836 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/prepared_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15129 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34646 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:04:54.381832 pulumi_consul-3.9.0a1680908224/pulumi_consul.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-04-07 23:04:54.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-07 23:04:54.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:04:54.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:04:54.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 23:04:54.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-07 23:04:54.000000 pulumi_consul-3.9.0a1680908224/pulumi_consul.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 23:04:54.381832 pulumi_consul-3.9.0a1680908224/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-07 23:04:53.000000 pulumi_consul-3.9.0a1680908224/setup.py
```

### Comparing `pulumi_consul-3.9.0a1679413309/PKG-INFO` & `pulumi_consul-3.9.0a1680908224/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_consul
-Version: 3.9.0a1679413309
+Version: 3.9.0a1680908224
 Summary: A Pulumi package for creating and managing consul resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-consul
 Keywords: pulumi consul
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_consul-3.9.0a1679413309/README.md` & `pulumi_consul-3.9.0a1680908224/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/__init__.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/_inputs.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/_utilities.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/acl_auth_method.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/acl_auth_method.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/acl_binding_rule.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/acl_binding_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/acl_policy.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/acl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/acl_role.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/acl_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/acl_token.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/acl_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/acl_token_policy_attachment.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/acl_token_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/acl_token_role_attachment.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/acl_token_role_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/admin_partition.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/admin_partition.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/agent_service.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/agent_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/autopilot_config.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/autopilot_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/catalog_entry.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/catalog_entry.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/certificate_authority.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/certificate_authority.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/config/outputs.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/config/vars.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/config_entry.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/config_entry.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_acl_auth_method.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_acl_auth_method.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_acl_policy.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_acl_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_acl_role.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_acl_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_acl_token.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_acl_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_acl_token_secret_id.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_acl_token_secret_id.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_agent_config.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_agent_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_agent_self.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_agent_self.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_autopilot_health.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_autopilot_health.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_catalog_nodes.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_catalog_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_catalog_service.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_catalog_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_catalog_services.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_catalog_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_config_entry.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_config_entry.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_datacenters.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_key_prefix.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_key_prefix.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_keys.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_network_area_members.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_network_area_members.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_network_segments.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_network_segments.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_nodes.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_peering.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_peerings.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_peerings.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_service.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_service_health.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_service_health.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/get_services.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/intention.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/intention.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/key_prefix.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/key_prefix.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/keys.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/license.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/license.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/namespace.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/namespace.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/namespace_policy_attachment.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/namespace_policy_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/namespace_role_attachment.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/namespace_role_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/network_area.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/network_area.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/node.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/node.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/outputs.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/peering.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/peering_token.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/peering_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/prepared_query.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/prepared_query.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/provider.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul/service.py` & `pulumi_consul-3.9.0a1680908224/pulumi_consul/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul.egg-info/PKG-INFO` & `pulumi_consul-3.9.0a1680908224/pulumi_consul.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-consul
-Version: 3.9.0a1679413309
+Version: 3.9.0a1680908224
 Summary: A Pulumi package for creating and managing consul resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-consul
 Keywords: pulumi consul
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_consul-3.9.0a1679413309/pulumi_consul.egg-info/SOURCES.txt` & `pulumi_consul-3.9.0a1680908224/pulumi_consul.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_consul-3.9.0a1679413309/setup.py` & `pulumi_consul-3.9.0a1680908224/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.9.0a1679413309"
-PLUGIN_VERSION = "3.9.0-alpha.1679413309+18e01cf3"
+VERSION = "3.9.0a1680908224"
+PLUGIN_VERSION = "3.9.0-alpha.1680908224+874a184f"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'consul', PLUGIN_VERSION])
         except OSError as error:
```

