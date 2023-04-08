# Comparing `tmp/pulumi_auth0-2.9.0a1651588791.tar.gz` & `tmp/pulumi_auth0-2.9.0a1653604814.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_auth0-2.9.0a1651588791.tar", last modified: Tue May  3 14:42:53 2022, max compression
+gzip compressed data, was "dist/pulumi_auth0-2.9.0a1653604814.tar", last modified: Thu May 26 22:43:53 2022, max compression
```

## Comparing `pulumi_auth0-2.9.0a1651588791.tar` & `pulumi_auth0-2.9.0a1653604814.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 14:42:53.000000 pulumi_auth0-2.9.0a1651588791/
--rw-r--r--   0 runner    (1001) docker     (121)     3084 2022-05-03 14:42:53.000000 pulumi_auth0-2.9.0a1651588791/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 14:42:53.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/
--rw-r--r--   0 runner    (1001) docker     (121)     5038 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   220616 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7667 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    25961 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/action.py
--rw-r--r--   0 runner    (1001) docker     (121)    18333 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/attack_protection.py
--rw-r--r--   0 runner    (1001) docker     (121)    17115 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/branding.py
--rw-r--r--   0 runner    (1001) docker     (121)   102443 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    12549 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/client_grant.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 14:42:53.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)    35011 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    17267 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (121)     7278 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/custom_domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (121)    15547 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/email.py
--rw-r--r--   0 runner    (1001) docker     (121)    26567 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/email_template.py
--rw-r--r--   0 runner    (1001) docker     (121)    19494 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/get_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    19692 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/get_global_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/get_tenant.py
--rw-r--r--   0 runner    (1001) docker     (121)    61234 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/global_client.py
--rw-r--r--   0 runner    (1001) docker     (121)    14571 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/guardian.py
--rw-r--r--   0 runner    (1001) docker     (121)    18354 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/hook.py
--rw-r--r--   0 runner    (1001) docker     (121)    12998 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/log_stream.py
--rw-r--r--   0 runner    (1001) docker     (121)    18237 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/organization.py
--rw-r--r--   0 runner    (1001) docker     (121)   228508 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    10281 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/prompt.py
--rw-r--r--   0 runner    (1001) docker     (121)    18785 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/prompt_custom_text.py
--rw-r--r--   0 runner    (1001) docker     (121)     7379 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    39073 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/resource_server.py
--rw-r--r--   0 runner    (1001) docker     (121)    13599 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/role.py
--rw-r--r--   0 runner    (1001) docker     (121)    13475 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/rule.py
--rw-r--r--   0 runner    (1001) docker     (121)     9227 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/rule_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    52289 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/tenant.py
--rw-r--r--   0 runner    (1001) docker     (121)    11878 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/trigger_binding.py
--rw-r--r--   0 runner    (1001) docker     (121)    41564 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0/user.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-03 14:42:53.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3084 2022-05-03 14:42:53.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-05-03 14:42:53.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 14:42:53.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-03 14:42:53.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-03 14:42:53.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-03 14:42:53.000000 pulumi_auth0-2.9.0a1651588791/pulumi_auth0.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-03 14:42:53.000000 pulumi_auth0-2.9.0a1651588791/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-05-03 14:42:52.000000 pulumi_auth0-2.9.0a1651588791/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/
+-rw-r--r--   0 runner    (1001) docker     (121)     3084 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/
+-rw-r--r--   0 runner    (1001) docker     (121)     5038 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)   220728 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7667 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25961 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/action.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18333 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/attack_protection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17115 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/branding.py
+-rw-r--r--   0 runner    (1001) docker     (121)   102443 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12549 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/client_grant.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35001 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/connection.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14576 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9515 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/custom_domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15547 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/email.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26567 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/email_template.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19494 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/get_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19692 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/get_global_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2991 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/get_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    61234 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/global_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14571 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/guardian.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18354 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/hook.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16260 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/log_stream.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18237 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/organization.py
+-rw-r--r--   0 runner    (1001) docker     (121)   228550 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10281 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18785 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/prompt_custom_text.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7379 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    39073 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/resource_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13599 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/role.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13475 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/rule.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9227 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/rule_config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    52289 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11878 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/trigger_binding.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41564 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0/user.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3084 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1214 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/pulumi_auth0.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2115 2022-05-26 22:43:53.000000 pulumi_auth0-2.9.0a1653604814/setup.py
```

### Comparing `pulumi_auth0-2.9.0a1651588791/PKG-INFO` & `pulumi_auth0-2.9.0a1653604814/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_auth0
-Version: 2.9.0a1651588791
+Version: 2.9.0a1653604814
 Summary: A Pulumi package for creating and managing auth0 cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-auth0
 Description: [![Actions Status](https://github.com/pulumi/pulumi-auth0/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-auth0/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fauth0.svg)](https://www.npmjs.com/package/@pulumi/auth0)
```

### Comparing `pulumi_auth0-2.9.0a1651588791/README.md` & `pulumi_auth0-2.9.0a1653604814/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/__init__.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/_inputs.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -4485,15 +4485,15 @@
                  azure_resource_group: Optional[pulumi.Input[str]] = None,
                  azure_subscription_id: Optional[pulumi.Input[str]] = None,
                  datadog_api_key: Optional[pulumi.Input[str]] = None,
                  datadog_region: Optional[pulumi.Input[str]] = None,
                  http_authorization: Optional[pulumi.Input[str]] = None,
                  http_content_format: Optional[pulumi.Input[str]] = None,
                  http_content_type: Optional[pulumi.Input[str]] = None,
-                 http_custom_headers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 http_custom_headers: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]] = None,
                  http_endpoint: Optional[pulumi.Input[str]] = None,
                  splunk_domain: Optional[pulumi.Input[str]] = None,
                  splunk_port: Optional[pulumi.Input[str]] = None,
                  splunk_secure: Optional[pulumi.Input[bool]] = None,
                  splunk_token: Optional[pulumi.Input[str]] = None,
                  sumo_source_address: Optional[pulumi.Input[str]] = None):
         """
@@ -4505,15 +4505,15 @@
         :param pulumi.Input[str] azure_resource_group: The Azure EventGrid resource group which allows you to manage all Azure assets within one subscription
         :param pulumi.Input[str] azure_subscription_id: The unique alphanumeric string that identifies your Azure subscription
         :param pulumi.Input[str] datadog_api_key: The Datadog API key
         :param pulumi.Input[str] datadog_region: The Datadog region
         :param pulumi.Input[str] http_authorization: Sent in the HTTP "Authorization" header with each request
         :param pulumi.Input[str] http_content_format: The format of data sent over HTTP. Options are "JSONLINES", "JSONARRAY" or "JSONOBJECT"
         :param pulumi.Input[str] http_content_type: The ContentType header to send over HTTP.  Common value is "application/json"
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] http_custom_headers: Additional HTTP headers to be included as part of the HTTP request
+        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]] http_custom_headers: Additional HTTP headers to be included as part of the HTTP request
         :param pulumi.Input[str] http_endpoint: The HTTP endpoint to send streaming logs
         :param pulumi.Input[str] splunk_domain: The Splunk domain name
         :param pulumi.Input[bool] splunk_secure: This toggle should be turned off when using self-signed certificates
         :param pulumi.Input[str] splunk_token: The Splunk access token
         :param pulumi.Input[str] sumo_source_address: Generated URL for your defined HTTP source in Sumo Logic for collecting streaming data from Auth0
         """
         if aws_account_id is not None:
@@ -4697,22 +4697,22 @@
 
     @http_content_type.setter
     def http_content_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "http_content_type", value)
 
     @property
     @pulumi.getter(name="httpCustomHeaders")
-    def http_custom_headers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+    def http_custom_headers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]]:
         """
         Additional HTTP headers to be included as part of the HTTP request
         """
         return pulumi.get(self, "http_custom_headers")
 
     @http_custom_headers.setter
-    def http_custom_headers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+    def http_custom_headers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]]):
         pulumi.set(self, "http_custom_headers", value)
 
     @property
     @pulumi.getter(name="httpEndpoint")
     def http_endpoint(self) -> Optional[pulumi.Input[str]]:
         """
         The HTTP endpoint to send streaming logs
```

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/_utilities.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/action.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/action.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/attack_protection.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/attack_protection.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/branding.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/branding.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/client.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/client.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/client_grant.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/client_grant.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/config/vars.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/connection.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -607,15 +607,15 @@
         """
         Name of the connection.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
-    def options(self) -> pulumi.Output[Optional['outputs.ConnectionOptions']]:
+    def options(self) -> pulumi.Output['outputs.ConnectionOptions']:
         """
         Configuration settings for connection options. For details, see Options.
         """
         return pulumi.get(self, "options")
 
     @property
     @pulumi.getter
```

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/custom_domain.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/custom_domain.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,30 +12,22 @@
 
 __all__ = ['CustomDomainArgs', 'CustomDomain']
 
 @pulumi.input_type
 class CustomDomainArgs:
     def __init__(__self__, *,
                  domain: pulumi.Input[str],
-                 type: pulumi.Input[str],
-                 verification_method: Optional[pulumi.Input[str]] = None):
+                 type: pulumi.Input[str]):
         """
         The set of arguments for constructing a CustomDomain resource.
         :param pulumi.Input[str] domain: String. Name of the custom domain.
         :param pulumi.Input[str] type: String. Provisioning type for the custom domain. Options include `auth0_managed_certs` and `self_managed_certs`.
-        :param pulumi.Input[str] verification_method: String. Domain verification method. The method is chosen according to the type of
-               the custom domain. `CNAME` for `auth0_managed_certs`, `TXT` for `self_managed_certs`.
         """
         pulumi.set(__self__, "domain", domain)
         pulumi.set(__self__, "type", type)
-        if verification_method is not None:
-            warnings.warn("""The method is chosen according to the type of the custom domain. CNAME for auth0_managed_certs, TXT for self_managed_certs""", DeprecationWarning)
-            pulumi.log.warn("""verification_method is deprecated: The method is chosen according to the type of the custom domain. CNAME for auth0_managed_certs, TXT for self_managed_certs""")
-        if verification_method is not None:
-            pulumi.set(__self__, "verification_method", verification_method)
 
     @property
     @pulumi.getter
     def domain(self) -> pulumi.Input[str]:
         """
         String. Name of the custom domain.
         """
@@ -53,76 +45,71 @@
         """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
-    @property
-    @pulumi.getter(name="verificationMethod")
-    def verification_method(self) -> Optional[pulumi.Input[str]]:
-        """
-        String. Domain verification method. The method is chosen according to the type of
-        the custom domain. `CNAME` for `auth0_managed_certs`, `TXT` for `self_managed_certs`.
-        """
-        return pulumi.get(self, "verification_method")
-
-    @verification_method.setter
-    def verification_method(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "verification_method", value)
-
 
 @pulumi.input_type
 class _CustomDomainState:
     def __init__(__self__, *,
                  domain: Optional[pulumi.Input[str]] = None,
+                 origin_domain_name: Optional[pulumi.Input[str]] = None,
                  primary: Optional[pulumi.Input[bool]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 verification: Optional[pulumi.Input['CustomDomainVerificationArgs']] = None,
-                 verification_method: Optional[pulumi.Input[str]] = None):
+                 verifications: Optional[pulumi.Input[Sequence[pulumi.Input['CustomDomainVerificationArgs']]]] = None):
         """
         Input properties used for looking up and filtering CustomDomain resources.
         :param pulumi.Input[str] domain: String. Name of the custom domain.
+        :param pulumi.Input[str] origin_domain_name: String. Once the configuration status is `ready`, the DNS name of the Auth0 origin server that handles traffic for the custom domain.
         :param pulumi.Input[bool] primary: Boolean. Indicates whether this is a primary domain.
         :param pulumi.Input[str] status: String. Configuration status for the custom domain. Options include `disabled`, `pending`, `pending_verification`, and `ready`.
         :param pulumi.Input[str] type: String. Provisioning type for the custom domain. Options include `auth0_managed_certs` and `self_managed_certs`.
-        :param pulumi.Input['CustomDomainVerificationArgs'] verification: List(Resource). Configuration settings for verification. For details, see Verification.
-        :param pulumi.Input[str] verification_method: String. Domain verification method. The method is chosen according to the type of
-               the custom domain. `CNAME` for `auth0_managed_certs`, `TXT` for `self_managed_certs`.
+        :param pulumi.Input[Sequence[pulumi.Input['CustomDomainVerificationArgs']]] verifications: List(Resource). Configuration settings for verification. For details, see Verification.
         """
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
+        if origin_domain_name is not None:
+            pulumi.set(__self__, "origin_domain_name", origin_domain_name)
         if primary is not None:
             pulumi.set(__self__, "primary", primary)
         if status is not None:
             pulumi.set(__self__, "status", status)
         if type is not None:
             pulumi.set(__self__, "type", type)
-        if verification is not None:
-            pulumi.set(__self__, "verification", verification)
-        if verification_method is not None:
-            warnings.warn("""The method is chosen according to the type of the custom domain. CNAME for auth0_managed_certs, TXT for self_managed_certs""", DeprecationWarning)
-            pulumi.log.warn("""verification_method is deprecated: The method is chosen according to the type of the custom domain. CNAME for auth0_managed_certs, TXT for self_managed_certs""")
-        if verification_method is not None:
-            pulumi.set(__self__, "verification_method", verification_method)
+        if verifications is not None:
+            pulumi.set(__self__, "verifications", verifications)
 
     @property
     @pulumi.getter
     def domain(self) -> Optional[pulumi.Input[str]]:
         """
         String. Name of the custom domain.
         """
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain", value)
 
     @property
+    @pulumi.getter(name="originDomainName")
+    def origin_domain_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        String. Once the configuration status is `ready`, the DNS name of the Auth0 origin server that handles traffic for the custom domain.
+        """
+        return pulumi.get(self, "origin_domain_name")
+
+    @origin_domain_name.setter
+    def origin_domain_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "origin_domain_name", value)
+
+    @property
     @pulumi.getter
     def primary(self) -> Optional[pulumi.Input[bool]]:
         """
         Boolean. Indicates whether this is a primary domain.
         """
         return pulumi.get(self, "primary")
 
@@ -152,46 +139,32 @@
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
-    def verification(self) -> Optional[pulumi.Input['CustomDomainVerificationArgs']]:
+    def verifications(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['CustomDomainVerificationArgs']]]]:
         """
         List(Resource). Configuration settings for verification. For details, see Verification.
         """
-        return pulumi.get(self, "verification")
+        return pulumi.get(self, "verifications")
 
-    @verification.setter
-    def verification(self, value: Optional[pulumi.Input['CustomDomainVerificationArgs']]):
-        pulumi.set(self, "verification", value)
-
-    @property
-    @pulumi.getter(name="verificationMethod")
-    def verification_method(self) -> Optional[pulumi.Input[str]]:
-        """
-        String. Domain verification method. The method is chosen according to the type of
-        the custom domain. `CNAME` for `auth0_managed_certs`, `TXT` for `self_managed_certs`.
-        """
-        return pulumi.get(self, "verification_method")
-
-    @verification_method.setter
-    def verification_method(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "verification_method", value)
+    @verifications.setter
+    def verifications(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['CustomDomainVerificationArgs']]]]):
+        pulumi.set(self, "verifications", value)
 
 
 class CustomDomain(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  domain: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 verification_method: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         With Auth0, you can use a custom domain to maintain a consistent user experience. This resource allows you to create and
         manage a custom domain within your Auth0 tenant.
 
         ## Example Usage
 
@@ -212,16 +185,14 @@
          $ pulumi import auth0:index/customDomain:CustomDomain my_custom_domain cd_XXXXXXXXXXXXXXXX
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] domain: String. Name of the custom domain.
         :param pulumi.Input[str] type: String. Provisioning type for the custom domain. Options include `auth0_managed_certs` and `self_managed_certs`.
-        :param pulumi.Input[str] verification_method: String. Domain verification method. The method is chosen according to the type of
-               the custom domain. `CNAME` for `auth0_managed_certs`, `TXT` for `self_managed_certs`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: CustomDomainArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -261,15 +232,14 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  domain: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
-                 verification_method: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.version is None:
             opts.version = _utilities.get_version()
@@ -280,73 +250,77 @@
 
             if domain is None and not opts.urn:
                 raise TypeError("Missing required property 'domain'")
             __props__.__dict__["domain"] = domain
             if type is None and not opts.urn:
                 raise TypeError("Missing required property 'type'")
             __props__.__dict__["type"] = type
-            if verification_method is not None and not opts.urn:
-                warnings.warn("""The method is chosen according to the type of the custom domain. CNAME for auth0_managed_certs, TXT for self_managed_certs""", DeprecationWarning)
-                pulumi.log.warn("""verification_method is deprecated: The method is chosen according to the type of the custom domain. CNAME for auth0_managed_certs, TXT for self_managed_certs""")
-            __props__.__dict__["verification_method"] = verification_method
+            __props__.__dict__["origin_domain_name"] = None
             __props__.__dict__["primary"] = None
             __props__.__dict__["status"] = None
-            __props__.__dict__["verification"] = None
+            __props__.__dict__["verifications"] = None
         super(CustomDomain, __self__).__init__(
             'auth0:index/customDomain:CustomDomain',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             domain: Optional[pulumi.Input[str]] = None,
+            origin_domain_name: Optional[pulumi.Input[str]] = None,
             primary: Optional[pulumi.Input[bool]] = None,
             status: Optional[pulumi.Input[str]] = None,
             type: Optional[pulumi.Input[str]] = None,
-            verification: Optional[pulumi.Input[pulumi.InputType['CustomDomainVerificationArgs']]] = None,
-            verification_method: Optional[pulumi.Input[str]] = None) -> 'CustomDomain':
+            verifications: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CustomDomainVerificationArgs']]]]] = None) -> 'CustomDomain':
         """
         Get an existing CustomDomain resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] domain: String. Name of the custom domain.
+        :param pulumi.Input[str] origin_domain_name: String. Once the configuration status is `ready`, the DNS name of the Auth0 origin server that handles traffic for the custom domain.
         :param pulumi.Input[bool] primary: Boolean. Indicates whether this is a primary domain.
         :param pulumi.Input[str] status: String. Configuration status for the custom domain. Options include `disabled`, `pending`, `pending_verification`, and `ready`.
         :param pulumi.Input[str] type: String. Provisioning type for the custom domain. Options include `auth0_managed_certs` and `self_managed_certs`.
-        :param pulumi.Input[pulumi.InputType['CustomDomainVerificationArgs']] verification: List(Resource). Configuration settings for verification. For details, see Verification.
-        :param pulumi.Input[str] verification_method: String. Domain verification method. The method is chosen according to the type of
-               the custom domain. `CNAME` for `auth0_managed_certs`, `TXT` for `self_managed_certs`.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['CustomDomainVerificationArgs']]]] verifications: List(Resource). Configuration settings for verification. For details, see Verification.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _CustomDomainState.__new__(_CustomDomainState)
 
         __props__.__dict__["domain"] = domain
+        __props__.__dict__["origin_domain_name"] = origin_domain_name
         __props__.__dict__["primary"] = primary
         __props__.__dict__["status"] = status
         __props__.__dict__["type"] = type
-        __props__.__dict__["verification"] = verification
-        __props__.__dict__["verification_method"] = verification_method
+        __props__.__dict__["verifications"] = verifications
         return CustomDomain(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def domain(self) -> pulumi.Output[str]:
         """
         String. Name of the custom domain.
         """
         return pulumi.get(self, "domain")
 
     @property
+    @pulumi.getter(name="originDomainName")
+    def origin_domain_name(self) -> pulumi.Output[str]:
+        """
+        String. Once the configuration status is `ready`, the DNS name of the Auth0 origin server that handles traffic for the custom domain.
+        """
+        return pulumi.get(self, "origin_domain_name")
+
+    @property
     @pulumi.getter
     def primary(self) -> pulumi.Output[bool]:
         """
         Boolean. Indicates whether this is a primary domain.
         """
         return pulumi.get(self, "primary")
 
@@ -364,22 +338,13 @@
         """
         String. Provisioning type for the custom domain. Options include `auth0_managed_certs` and `self_managed_certs`.
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
-    def verification(self) -> pulumi.Output['outputs.CustomDomainVerification']:
+    def verifications(self) -> pulumi.Output[Sequence['outputs.CustomDomainVerification']]:
         """
         List(Resource). Configuration settings for verification. For details, see Verification.
         """
-        return pulumi.get(self, "verification")
-
-    @property
-    @pulumi.getter(name="verificationMethod")
-    def verification_method(self) -> pulumi.Output[Optional[str]]:
-        """
-        String. Domain verification method. The method is chosen according to the type of
-        the custom domain. `CNAME` for `auth0_managed_certs`, `TXT` for `self_managed_certs`.
-        """
-        return pulumi.get(self, "verification_method")
+        return pulumi.get(self, "verifications")
```

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/custom_domain_verification.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/custom_domain_verification.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,34 +32,62 @@
     def custom_domain_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "custom_domain_id", value)
 
 
 @pulumi.input_type
 class _CustomDomainVerificationState:
     def __init__(__self__, *,
-                 custom_domain_id: Optional[pulumi.Input[str]] = None):
+                 cname_api_key: Optional[pulumi.Input[str]] = None,
+                 custom_domain_id: Optional[pulumi.Input[str]] = None,
+                 origin_domain_name: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering CustomDomainVerification resources.
         :param pulumi.Input[str] custom_domain_id: String. ID of the custom domain resource.
+        :param pulumi.Input[str] origin_domain_name: String. The DNS name of the Auth0 origin server that handles traffic for the custom domain.
         """
+        if cname_api_key is not None:
+            pulumi.set(__self__, "cname_api_key", cname_api_key)
         if custom_domain_id is not None:
             pulumi.set(__self__, "custom_domain_id", custom_domain_id)
+        if origin_domain_name is not None:
+            pulumi.set(__self__, "origin_domain_name", origin_domain_name)
+
+    @property
+    @pulumi.getter(name="cnameApiKey")
+    def cname_api_key(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "cname_api_key")
+
+    @cname_api_key.setter
+    def cname_api_key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cname_api_key", value)
 
     @property
     @pulumi.getter(name="customDomainId")
     def custom_domain_id(self) -> Optional[pulumi.Input[str]]:
         """
         String. ID of the custom domain resource.
         """
         return pulumi.get(self, "custom_domain_id")
 
     @custom_domain_id.setter
     def custom_domain_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_domain_id", value)
 
+    @property
+    @pulumi.getter(name="originDomainName")
+    def origin_domain_name(self) -> Optional[pulumi.Input[str]]:
+        """
+        String. The DNS name of the Auth0 origin server that handles traffic for the custom domain.
+        """
+        return pulumi.get(self, "origin_domain_name")
+
+    @origin_domain_name.setter
+    def origin_domain_name(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "origin_domain_name", value)
+
 
 class CustomDomainVerification(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  custom_domain_id: Optional[pulumi.Input[str]] = None,
@@ -127,42 +155,62 @@
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = CustomDomainVerificationInitArgs.__new__(CustomDomainVerificationInitArgs)
 
             if custom_domain_id is None and not opts.urn:
                 raise TypeError("Missing required property 'custom_domain_id'")
             __props__.__dict__["custom_domain_id"] = custom_domain_id
+            __props__.__dict__["cname_api_key"] = None
+            __props__.__dict__["origin_domain_name"] = None
         super(CustomDomainVerification, __self__).__init__(
             'auth0:index/customDomainVerification:CustomDomainVerification',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            custom_domain_id: Optional[pulumi.Input[str]] = None) -> 'CustomDomainVerification':
+            cname_api_key: Optional[pulumi.Input[str]] = None,
+            custom_domain_id: Optional[pulumi.Input[str]] = None,
+            origin_domain_name: Optional[pulumi.Input[str]] = None) -> 'CustomDomainVerification':
         """
         Get an existing CustomDomainVerification resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] custom_domain_id: String. ID of the custom domain resource.
+        :param pulumi.Input[str] origin_domain_name: String. The DNS name of the Auth0 origin server that handles traffic for the custom domain.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _CustomDomainVerificationState.__new__(_CustomDomainVerificationState)
 
+        __props__.__dict__["cname_api_key"] = cname_api_key
         __props__.__dict__["custom_domain_id"] = custom_domain_id
+        __props__.__dict__["origin_domain_name"] = origin_domain_name
         return CustomDomainVerification(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="cnameApiKey")
+    def cname_api_key(self) -> pulumi.Output[str]:
+        return pulumi.get(self, "cname_api_key")
+
+    @property
     @pulumi.getter(name="customDomainId")
     def custom_domain_id(self) -> pulumi.Output[str]:
         """
         String. ID of the custom domain resource.
         """
         return pulumi.get(self, "custom_domain_id")
 
+    @property
+    @pulumi.getter(name="originDomainName")
+    def origin_domain_name(self) -> pulumi.Output[str]:
+        """
+        String. The DNS name of the Auth0 origin server that handles traffic for the custom domain.
+        """
+        return pulumi.get(self, "origin_domain_name")
+
```

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/email.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/email.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/email_template.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/email_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/get_client.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/get_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/get_global_client.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/get_global_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/get_tenant.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/get_tenant.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/global_client.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/global_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/guardian.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/guardian.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/hook.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/log_stream.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/log_stream.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,25 +13,29 @@
 __all__ = ['LogStreamArgs', 'LogStream']
 
 @pulumi.input_type
 class LogStreamArgs:
     def __init__(__self__, *,
                  sink: pulumi.Input['LogStreamSinkArgs'],
                  type: pulumi.Input[str],
+                 filters: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  status: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a LogStream resource.
         :param pulumi.Input['LogStreamSinkArgs'] sink: List(Resource) The sink configuration for the log stream. For details, see Sink Configuration.
         :param pulumi.Input[str] type: The type of log stream. Options are "eventbridge", "eventgrid", "http", "datadog", "splunk", "sumo"
+        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]] filters: Only logs events matching these filters will be delivered by the stream.
         :param pulumi.Input[str] name: Name of the log stream
         :param pulumi.Input[str] status: The current status of the log stream. Options are "active", "paused", "suspended"
         """
         pulumi.set(__self__, "sink", sink)
         pulumi.set(__self__, "type", type)
+        if filters is not None:
+            pulumi.set(__self__, "filters", filters)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if status is not None:
             pulumi.set(__self__, "status", status)
 
     @property
     @pulumi.getter
@@ -55,14 +59,26 @@
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter
+    def filters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]]:
+        """
+        Only logs events matching these filters will be delivered by the stream.
+        """
+        return pulumi.get(self, "filters")
+
+    @filters.setter
+    def filters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]]):
+        pulumi.set(self, "filters", value)
+
+    @property
+    @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Name of the log stream
         """
         return pulumi.get(self, "name")
 
     @name.setter
@@ -81,36 +97,52 @@
     def status(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "status", value)
 
 
 @pulumi.input_type
 class _LogStreamState:
     def __init__(__self__, *,
+                 filters: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  sink: Optional[pulumi.Input['LogStreamSinkArgs']] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering LogStream resources.
+        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]] filters: Only logs events matching these filters will be delivered by the stream.
         :param pulumi.Input[str] name: Name of the log stream
         :param pulumi.Input['LogStreamSinkArgs'] sink: List(Resource) The sink configuration for the log stream. For details, see Sink Configuration.
         :param pulumi.Input[str] status: The current status of the log stream. Options are "active", "paused", "suspended"
         :param pulumi.Input[str] type: The type of log stream. Options are "eventbridge", "eventgrid", "http", "datadog", "splunk", "sumo"
         """
+        if filters is not None:
+            pulumi.set(__self__, "filters", filters)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if sink is not None:
             pulumi.set(__self__, "sink", sink)
         if status is not None:
             pulumi.set(__self__, "status", status)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
+    def filters(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]]:
+        """
+        Only logs events matching these filters will be delivered by the stream.
+        """
+        return pulumi.get(self, "filters")
+
+    @filters.setter
+    def filters(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]]):
+        pulumi.set(self, "filters", value)
+
+    @property
+    @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         Name of the log stream
         """
         return pulumi.get(self, "name")
 
     @name.setter
@@ -155,14 +187,15 @@
 
 
 class LogStream(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 filters: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  sink: Optional[pulumi.Input[pulumi.InputType['LogStreamSinkArgs']]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         With this resource, you can manage your Auth0 log streams.
@@ -170,14 +203,24 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_auth0 as auth0
 
         example = auth0.LogStream("example",
+            filters=[
+                {
+                    "name": "auth.login.fail",
+                    "type": "category",
+                },
+                {
+                    "name": "auth.signup.fail",
+                    "type": "category",
+                },
+            ],
             sink=auth0.LogStreamSinkArgs(
                 aws_account_id="my_account_id",
                 aws_region="us-east-2",
             ),
             status="active",
             type="eventbridge")
         ```
@@ -188,14 +231,15 @@
 
         ```sh
          $ pulumi import auth0:index/logStream:LogStream example lst_XXXXXXXXXXXXXXXX
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]] filters: Only logs events matching these filters will be delivered by the stream.
         :param pulumi.Input[str] name: Name of the log stream
         :param pulumi.Input[pulumi.InputType['LogStreamSinkArgs']] sink: List(Resource) The sink configuration for the log stream. For details, see Sink Configuration.
         :param pulumi.Input[str] status: The current status of the log stream. Options are "active", "paused", "suspended"
         :param pulumi.Input[str] type: The type of log stream. Options are "eventbridge", "eventgrid", "http", "datadog", "splunk", "sumo"
         """
         ...
     @overload
@@ -209,14 +253,24 @@
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_auth0 as auth0
 
         example = auth0.LogStream("example",
+            filters=[
+                {
+                    "name": "auth.login.fail",
+                    "type": "category",
+                },
+                {
+                    "name": "auth.signup.fail",
+                    "type": "category",
+                },
+            ],
             sink=auth0.LogStreamSinkArgs(
                 aws_account_id="my_account_id",
                 aws_region="us-east-2",
             ),
             status="active",
             type="eventbridge")
         ```
@@ -240,14 +294,15 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 filters: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  sink: Optional[pulumi.Input[pulumi.InputType['LogStreamSinkArgs']]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         if opts is None:
             opts = pulumi.ResourceOptions()
@@ -256,14 +311,15 @@
         if opts.version is None:
             opts.version = _utilities.get_version()
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = LogStreamArgs.__new__(LogStreamArgs)
 
+            __props__.__dict__["filters"] = filters
             __props__.__dict__["name"] = name
             if sink is None and not opts.urn:
                 raise TypeError("Missing required property 'sink'")
             __props__.__dict__["sink"] = sink
             __props__.__dict__["status"] = status
             if type is None and not opts.urn:
                 raise TypeError("Missing required property 'type'")
@@ -274,42 +330,53 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            filters: Optional[pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]]] = None,
             name: Optional[pulumi.Input[str]] = None,
             sink: Optional[pulumi.Input[pulumi.InputType['LogStreamSinkArgs']]] = None,
             status: Optional[pulumi.Input[str]] = None,
             type: Optional[pulumi.Input[str]] = None) -> 'LogStream':
         """
         Get an existing LogStream resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[Mapping[str, pulumi.Input[str]]]]] filters: Only logs events matching these filters will be delivered by the stream.
         :param pulumi.Input[str] name: Name of the log stream
         :param pulumi.Input[pulumi.InputType['LogStreamSinkArgs']] sink: List(Resource) The sink configuration for the log stream. For details, see Sink Configuration.
         :param pulumi.Input[str] status: The current status of the log stream. Options are "active", "paused", "suspended"
         :param pulumi.Input[str] type: The type of log stream. Options are "eventbridge", "eventgrid", "http", "datadog", "splunk", "sumo"
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _LogStreamState.__new__(_LogStreamState)
 
+        __props__.__dict__["filters"] = filters
         __props__.__dict__["name"] = name
         __props__.__dict__["sink"] = sink
         __props__.__dict__["status"] = status
         __props__.__dict__["type"] = type
         return LogStream(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
+    def filters(self) -> pulumi.Output[Optional[Sequence[Mapping[str, str]]]]:
+        """
+        Only logs events matching these filters will be delivered by the stream.
+        """
+        return pulumi.get(self, "filters")
+
+    @property
+    @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
         Name of the log stream
         """
         return pulumi.get(self, "name")
 
     @property
```

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/organization.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/outputs.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4129,15 +4129,15 @@
                  azure_resource_group: Optional[str] = None,
                  azure_subscription_id: Optional[str] = None,
                  datadog_api_key: Optional[str] = None,
                  datadog_region: Optional[str] = None,
                  http_authorization: Optional[str] = None,
                  http_content_format: Optional[str] = None,
                  http_content_type: Optional[str] = None,
-                 http_custom_headers: Optional[Sequence[str]] = None,
+                 http_custom_headers: Optional[Sequence[Mapping[str, str]]] = None,
                  http_endpoint: Optional[str] = None,
                  splunk_domain: Optional[str] = None,
                  splunk_port: Optional[str] = None,
                  splunk_secure: Optional[bool] = None,
                  splunk_token: Optional[str] = None,
                  sumo_source_address: Optional[str] = None):
         """
@@ -4149,15 +4149,15 @@
         :param str azure_resource_group: The Azure EventGrid resource group which allows you to manage all Azure assets within one subscription
         :param str azure_subscription_id: The unique alphanumeric string that identifies your Azure subscription
         :param str datadog_api_key: The Datadog API key
         :param str datadog_region: The Datadog region
         :param str http_authorization: Sent in the HTTP "Authorization" header with each request
         :param str http_content_format: The format of data sent over HTTP. Options are "JSONLINES", "JSONARRAY" or "JSONOBJECT"
         :param str http_content_type: The ContentType header to send over HTTP.  Common value is "application/json"
-        :param Sequence[str] http_custom_headers: Additional HTTP headers to be included as part of the HTTP request
+        :param Sequence[Mapping[str, str]] http_custom_headers: Additional HTTP headers to be included as part of the HTTP request
         :param str http_endpoint: The HTTP endpoint to send streaming logs
         :param str splunk_domain: The Splunk domain name
         :param bool splunk_secure: This toggle should be turned off when using self-signed certificates
         :param str splunk_token: The Splunk access token
         :param str sumo_source_address: Generated URL for your defined HTTP source in Sumo Logic for collecting streaming data from Auth0
         """
         if aws_account_id is not None:
@@ -4293,15 +4293,15 @@
         """
         The ContentType header to send over HTTP.  Common value is "application/json"
         """
         return pulumi.get(self, "http_content_type")
 
     @property
     @pulumi.getter(name="httpCustomHeaders")
-    def http_custom_headers(self) -> Optional[Sequence[str]]:
+    def http_custom_headers(self) -> Optional[Sequence[Mapping[str, str]]]:
         """
         Additional HTTP headers to be included as part of the HTTP request
         """
         return pulumi.get(self, "http_custom_headers")
 
     @property
     @pulumi.getter(name="httpEndpoint")
```

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/prompt.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/prompt.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/prompt_custom_text.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/prompt_custom_text.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/provider.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/resource_server.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/resource_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/role.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/rule.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/rule_config.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/rule_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/tenant.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/tenant.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/trigger_binding.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/trigger_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0/user.py` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0.egg-info/PKG-INFO` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-auth0
-Version: 2.9.0a1651588791
+Version: 2.9.0a1653604814
 Summary: A Pulumi package for creating and managing auth0 cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-auth0
 Description: [![Actions Status](https://github.com/pulumi/pulumi-auth0/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-auth0/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fauth0.svg)](https://www.npmjs.com/package/@pulumi/auth0)
```

### Comparing `pulumi_auth0-2.9.0a1651588791/pulumi_auth0.egg-info/SOURCES.txt` & `pulumi_auth0-2.9.0a1653604814/pulumi_auth0.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_auth0-2.9.0a1651588791/setup.py` & `pulumi_auth0-2.9.0a1653604814/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.9.0a1651588791"
-PLUGIN_VERSION = "2.9.0-alpha.1651588791+122e05bb"
+VERSION = "2.9.0a1653604814"
+PLUGIN_VERSION = "2.9.0-alpha.1653604814+4d1ac1e6"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'auth0', PLUGIN_VERSION])
         except OSError as error:
```

