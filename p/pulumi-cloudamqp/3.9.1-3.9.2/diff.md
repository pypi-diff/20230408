# Comparing `tmp/pulumi_cloudamqp-3.9.1.tar.gz` & `tmp/pulumi_cloudamqp-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_cloudamqp-3.9.1.tar", last modified: Fri Aug 26 18:31:56 2022, max compression
+gzip compressed data, was "pulumi_cloudamqp-3.9.2.tar", last modified: Tue Sep 27 04:19:55 2022, max compression
```

## Comparing `pulumi_cloudamqp-3.9.1.tar` & `pulumi_cloudamqp-3.9.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 18:31:56.676849 pulumi_cloudamqp-3.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-08-26 18:31:56.676849 pulumi_cloudamqp-3.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2293 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 18:31:56.676849 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/
--rw-r--r--   0 runner    (1001) docker     (121)     4461 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2843 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    33808 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/alarm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 18:31:56.676849 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)    10021 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/custom_domain.py
--rw-r--r--   0 runner    (1001) docker     (121)    10019 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/extra_disk_size.py
--rw-r--r--   0 runner    (1001) docker     (121)     2882 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_account.py
--rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_account_vpcs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11439 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_alarm.py
--rw-r--r--   0 runner    (1001) docker     (121)     4839 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)    11122 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (121)     5039 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     6204 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_notification.py
--rw-r--r--   0 runner    (1001) docker     (121)     5299 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     5431 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_plugins_community.py
--rw-r--r--   0 runner    (1001) docker     (121)     5044 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_upgradable_versions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6931 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_vpc_gcp_info.py
--rw-r--r--   0 runner    (1001) docker     (121)     7629 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_vpc_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    34311 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/instance.py
--rw-r--r--   0 runner    (1001) docker     (121)    41813 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/integration_log.py
--rw-r--r--   0 runner    (1001) docker     (121)    36116 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/integration_metric.py
--rw-r--r--   0 runner    (1001) docker     (121)    18537 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/node_actions.py
--rw-r--r--   0 runner    (1001) docker     (121)    13483 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/notification.py
--rw-r--r--   0 runner    (1001) docker     (121)     8020 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    12819 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)    11543 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/plugin_community.py
--rw-r--r--   0 runner    (1001) docker     (121)     5519 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    27791 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/rabbit_configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     9100 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/security_firewall.py
--rw-r--r--   0 runner    (1001) docker     (121)     9871 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/upgrade_rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (121)    14364 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/vpc.py
--rw-r--r--   0 runner    (1001) docker     (121)    12785 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/vpc_gcp_peering.py
--rw-r--r--   0 runner    (1001) docker     (121)    14593 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/vpc_peering.py
--rw-r--r--   0 runner    (1001) docker     (121)    17261 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 18:31:56.676849 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/pulumi_cloudamqp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 18:31:56.676849 pulumi_cloudamqp-3.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-08-26 18:31:56.000000 pulumi_cloudamqp-3.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 04:19:55.863301 pulumi_cloudamqp-3.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-09-27 04:19:55.863301 pulumi_cloudamqp-3.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2293 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 04:19:55.863301 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/
+-rw-r--r--   0 runner    (1001) docker     (121)     4461 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2859 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8081 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33808 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/alarm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 04:19:55.863301 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      794 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10021 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/custom_domain.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10019 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/extra_disk_size.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2882 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2899 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_account_vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11439 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4839 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11122 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5039 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6204 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_notification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5299 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5431 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_plugins_community.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5044 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_upgradable_versions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6931 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_vpc_gcp_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7629 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_vpc_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)    34311 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41813 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/integration_log.py
+-rw-r--r--   0 runner    (1001) docker     (121)    36116 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/integration_metric.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18537 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/node_actions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13483 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/notification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8036 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9441 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11977 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/plugin_community.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5519 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    27711 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/rabbit_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9100 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/security_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9871 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/upgrade_rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14364 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/vpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12785 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/vpc_gcp_peering.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14593 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/vpc_peering.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17261 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 04:19:55.863301 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2631 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1520 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/pulumi_cloudamqp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 04:19:55.863301 pulumi_cloudamqp-3.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-09-27 04:19:55.000000 pulumi_cloudamqp-3.9.2/setup.py
```

### Comparing `pulumi_cloudamqp-3.9.1/PKG-INFO` & `pulumi_cloudamqp-3.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_cloudamqp
-Version: 3.9.1
+Version: 3.9.2
 Summary: A Pulumi package for creating and managing CloudAMQP resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudamqp
 Keywords: pulumi cloudamqp
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_cloudamqp-3.9.1/README.md` & `pulumi_cloudamqp-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/__init__.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/_inputs.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/_inputs.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class SecurityFirewallRuleArgs:
     def __init__(__self__, *,
                  ip: pulumi.Input[str],
                  description: Optional[pulumi.Input[str]] = None,
                  ports: Optional[pulumi.Input[Sequence[pulumi.Input[int]]]] = None,
                  services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        :param pulumi.Input[str] ip: Source ip and netmask for the rule. (e.g. 10.56.72.0/24)
+        :param pulumi.Input[str] ip: CIDR address: IP address with CIDR notation (e.g. 10.56.72.0/24)
         :param pulumi.Input[str] description: Description name of the rule. e.g. Default.
         :param pulumi.Input[Sequence[pulumi.Input[int]]] ports: Custom ports to be opened
         :param pulumi.Input[Sequence[pulumi.Input[str]]] services: Pre-defined service ports, see table below
         """
         pulumi.set(__self__, "ip", ip)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -34,15 +34,15 @@
         if services is not None:
             pulumi.set(__self__, "services", services)
 
     @property
     @pulumi.getter
     def ip(self) -> pulumi.Input[str]:
         """
-        Source ip and netmask for the rule. (e.g. 10.56.72.0/24)
+        CIDR address: IP address with CIDR notation (e.g. 10.56.72.0/24)
         """
         return pulumi.get(self, "ip")
 
     @ip.setter
     def ip(self, value: pulumi.Input[str]):
         pulumi.set(self, "ip", value)
```

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/_utilities.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/alarm.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/alarm.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/config/vars.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/custom_domain.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/custom_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/extra_disk_size.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/extra_disk_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_account.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_account_vpcs.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_account_vpcs.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_alarm.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_alarm.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_credentials.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_instance.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_nodes.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_notification.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_plugins.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_plugins.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_plugins_community.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_plugins_community.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_upgradable_versions.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_upgradable_versions.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_vpc_gcp_info.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_vpc_gcp_info.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/get_vpc_info.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/get_vpc_info.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/instance.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/integration_log.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/integration_log.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/integration_metric.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/integration_metric.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/node_actions.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/node_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/notification.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/notification.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/outputs.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class SecurityFirewallRule(dict):
     def __init__(__self__, *,
                  ip: str,
                  description: Optional[str] = None,
                  ports: Optional[Sequence[int]] = None,
                  services: Optional[Sequence[str]] = None):
         """
-        :param str ip: Source ip and netmask for the rule. (e.g. 10.56.72.0/24)
+        :param str ip: CIDR address: IP address with CIDR notation (e.g. 10.56.72.0/24)
         :param str description: Description name of the rule. e.g. Default.
         :param Sequence[int] ports: Custom ports to be opened
         :param Sequence[str] services: Pre-defined service ports, see table below
         """
         pulumi.set(__self__, "ip", ip)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -39,15 +39,15 @@
         if services is not None:
             pulumi.set(__self__, "services", services)
 
     @property
     @pulumi.getter
     def ip(self) -> str:
         """
-        Source ip and netmask for the rule. (e.g. 10.56.72.0/24)
+        CIDR address: IP address with CIDR notation (e.g. 10.56.72.0/24)
         """
         return pulumi.get(self, "ip")
 
     @property
     @pulumi.getter
     def description(self) -> Optional[str]:
         """
```

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/plugin.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/plugin_community.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['PluginArgs', 'Plugin']
+__all__ = ['PluginCommunityArgs', 'PluginCommunity']
 
 @pulumi.input_type
-class PluginArgs:
+class PluginCommunityArgs:
     def __init__(__self__, *,
                  enabled: pulumi.Input[bool],
                  instance_id: pulumi.Input[int],
                  name: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a Plugin resource.
+        The set of arguments for constructing a PluginCommunity resource.
         :param pulumi.Input[bool] enabled: Enable or disable the plugins.
         :param pulumi.Input[int] instance_id: The CloudAMQP instance ID.
-        :param pulumi.Input[str] name: The name of the Rabbit MQ plugin.
+        :param pulumi.Input[str] name: The name of the Rabbit MQ community plugin.
         """
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "instance_id", instance_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
@@ -52,34 +52,34 @@
     def instance_id(self, value: pulumi.Input[int]):
         pulumi.set(self, "instance_id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the Rabbit MQ plugin.
+        The name of the Rabbit MQ community plugin.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
-class _PluginState:
+class _PluginCommunityState:
     def __init__(__self__, *,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  instance_id: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering Plugin resources.
+        Input properties used for looking up and filtering PluginCommunity resources.
         :param pulumi.Input[bool] enabled: Enable or disable the plugins.
         :param pulumi.Input[int] instance_id: The CloudAMQP instance ID.
-        :param pulumi.Input[str] name: The name of the Rabbit MQ plugin.
+        :param pulumi.Input[str] name: The name of the Rabbit MQ community plugin.
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if instance_id is not None:
             pulumi.set(__self__, "instance_id", instance_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -108,147 +108,113 @@
     def instance_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "instance_id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the Rabbit MQ plugin.
+        The name of the Rabbit MQ community plugin.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
-class Plugin(pulumi.CustomResource):
+class PluginCommunity(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  instance_id: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        This resource allows you to enable or disable Rabbit MQ plugins.
+        This resource allows you to install or uninstall community plugins. Once installed the plugin will be available in `Plugin`.
 
         Only available for dedicated subscription plans.
 
-        ⚠️  From our go API wrapper [v1.4.0](https://github.com/84codes/go-api/releases/tag/v1.4.0) there is support for multiple retries when requesting information about plugins. This was introduced to avoid `ReadPlugin error 400: Timeout talking to backend`.
+        > From our go API wrapper [v1.5.0](https://github.com/84codes/go-api/releases/tag/v1.5.0) there is support for multiple retries when requesting information about community plugins. This was introduced to avoid `ReadPluginCommunity error 400: Timeout talking to backend`.
 
-        **Enable multiple plugins:** Rabbit MQ can only change one plugin at a time. It will fail if multiple plugins resources are used, unless by creating dependencies with `depend_on` between the resources. Once one plugin has been enabled, the other will continue. See example below.
+        > From our go API wrapper [v1.9.1](https://github.com/84codes/go-api/releases/tag/v1.9.1) there is support for asynchronous request for plugin/community actions. Solve issues reported when enable multiple plugins.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_cloudamqp as cloudamqp
 
-        rabbitmq_top = cloudamqp.Plugin("rabbitmqTop",
-            instance_id=cloudamqp_instance["instance"]["id"],
+        rabbitmq_delayed_message_exchange = cloudamqp.PluginCommunity("rabbitmqDelayedMessageExchange",
+            instance_id=cloudamqp_instance["instance_01"]["id"],
             enabled=True)
         ```
-
-        **Enable multiple plugins**
-
-        ```python
-        import pulumi
-        import pulumi_cloudamqp as cloudamqp
-
-        rabbitmq_top = cloudamqp.Plugin("rabbitmqTop",
-            instance_id=cloudamqp_instance["instance"]["id"],
-            enabled=True)
-        rabbitmq_amqp10 = cloudamqp.Plugin("rabbitmqAmqp10",
-            instance_id=cloudamqp_instance["instance"]["id"],
-            enabled=True,
-            opts=pulumi.ResourceOptions(depends_on=[rabbitmq_top]))
-        ```
-        ## Dependency
+        ## Depedency
 
         This resource depends on CloudAMQP instance identifier, `cloudamqp_instance.instance.id`.
 
-        If multiple plugins should be enable, create dependencies between the plugin resources. See example above.
-
         ## Import
 
         `cloudamqp_plugin` can be imported using the name argument of the resource together with CloudAMQP instance identifier. The name and identifier are CSV separated, see example below.
 
         ```sh
-         $ pulumi import cloudamqp:index/plugin:Plugin rabbitmq_management rabbitmq_management,<instance_id>`
+         $ pulumi import cloudamqp:index/pluginCommunity:PluginCommunity <resource_name> <plugin_name>,<instance_id>`
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] enabled: Enable or disable the plugins.
         :param pulumi.Input[int] instance_id: The CloudAMQP instance ID.
-        :param pulumi.Input[str] name: The name of the Rabbit MQ plugin.
+        :param pulumi.Input[str] name: The name of the Rabbit MQ community plugin.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: PluginArgs,
+                 args: PluginCommunityArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        This resource allows you to enable or disable Rabbit MQ plugins.
+        This resource allows you to install or uninstall community plugins. Once installed the plugin will be available in `Plugin`.
 
         Only available for dedicated subscription plans.
 
-        ⚠️  From our go API wrapper [v1.4.0](https://github.com/84codes/go-api/releases/tag/v1.4.0) there is support for multiple retries when requesting information about plugins. This was introduced to avoid `ReadPlugin error 400: Timeout talking to backend`.
+        > From our go API wrapper [v1.5.0](https://github.com/84codes/go-api/releases/tag/v1.5.0) there is support for multiple retries when requesting information about community plugins. This was introduced to avoid `ReadPluginCommunity error 400: Timeout talking to backend`.
 
-        **Enable multiple plugins:** Rabbit MQ can only change one plugin at a time. It will fail if multiple plugins resources are used, unless by creating dependencies with `depend_on` between the resources. Once one plugin has been enabled, the other will continue. See example below.
+        > From our go API wrapper [v1.9.1](https://github.com/84codes/go-api/releases/tag/v1.9.1) there is support for asynchronous request for plugin/community actions. Solve issues reported when enable multiple plugins.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_cloudamqp as cloudamqp
 
-        rabbitmq_top = cloudamqp.Plugin("rabbitmqTop",
-            instance_id=cloudamqp_instance["instance"]["id"],
+        rabbitmq_delayed_message_exchange = cloudamqp.PluginCommunity("rabbitmqDelayedMessageExchange",
+            instance_id=cloudamqp_instance["instance_01"]["id"],
             enabled=True)
         ```
-
-        **Enable multiple plugins**
-
-        ```python
-        import pulumi
-        import pulumi_cloudamqp as cloudamqp
-
-        rabbitmq_top = cloudamqp.Plugin("rabbitmqTop",
-            instance_id=cloudamqp_instance["instance"]["id"],
-            enabled=True)
-        rabbitmq_amqp10 = cloudamqp.Plugin("rabbitmqAmqp10",
-            instance_id=cloudamqp_instance["instance"]["id"],
-            enabled=True,
-            opts=pulumi.ResourceOptions(depends_on=[rabbitmq_top]))
-        ```
-        ## Dependency
+        ## Depedency
 
         This resource depends on CloudAMQP instance identifier, `cloudamqp_instance.instance.id`.
 
-        If multiple plugins should be enable, create dependencies between the plugin resources. See example above.
-
         ## Import
 
         `cloudamqp_plugin` can be imported using the name argument of the resource together with CloudAMQP instance identifier. The name and identifier are CSV separated, see example below.
 
         ```sh
-         $ pulumi import cloudamqp:index/plugin:Plugin rabbitmq_management rabbitmq_management,<instance_id>`
+         $ pulumi import cloudamqp:index/pluginCommunity:PluginCommunity <resource_name> <plugin_name>,<instance_id>`
         ```
 
         :param str resource_name: The name of the resource.
-        :param PluginArgs args: The arguments to use to populate this resource's properties.
+        :param PluginCommunityArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(PluginArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(PluginCommunityArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -259,55 +225,55 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = PluginArgs.__new__(PluginArgs)
+            __props__ = PluginCommunityArgs.__new__(PluginCommunityArgs)
 
             if enabled is None and not opts.urn:
                 raise TypeError("Missing required property 'enabled'")
             __props__.__dict__["enabled"] = enabled
             if instance_id is None and not opts.urn:
                 raise TypeError("Missing required property 'instance_id'")
             __props__.__dict__["instance_id"] = instance_id
             __props__.__dict__["name"] = name
-        super(Plugin, __self__).__init__(
-            'cloudamqp:index/plugin:Plugin',
+        super(PluginCommunity, __self__).__init__(
+            'cloudamqp:index/pluginCommunity:PluginCommunity',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             enabled: Optional[pulumi.Input[bool]] = None,
             instance_id: Optional[pulumi.Input[int]] = None,
-            name: Optional[pulumi.Input[str]] = None) -> 'Plugin':
+            name: Optional[pulumi.Input[str]] = None) -> 'PluginCommunity':
         """
-        Get an existing Plugin resource's state with the given name, id, and optional extra
+        Get an existing PluginCommunity resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] enabled: Enable or disable the plugins.
         :param pulumi.Input[int] instance_id: The CloudAMQP instance ID.
-        :param pulumi.Input[str] name: The name of the Rabbit MQ plugin.
+        :param pulumi.Input[str] name: The name of the Rabbit MQ community plugin.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _PluginState.__new__(_PluginState)
+        __props__ = _PluginCommunityState.__new__(_PluginCommunityState)
 
         __props__.__dict__["enabled"] = enabled
         __props__.__dict__["instance_id"] = instance_id
         __props__.__dict__["name"] = name
-        return Plugin(resource_name, opts=opts, __props__=__props__)
+        return PluginCommunity(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def enabled(self) -> pulumi.Output[bool]:
         """
         Enable or disable the plugins.
         """
@@ -321,11 +287,11 @@
         """
         return pulumi.get(self, "instance_id")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The name of the Rabbit MQ plugin.
+        The name of the Rabbit MQ community plugin.
         """
         return pulumi.get(self, "name")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/plugin_community.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/plugin.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
-__all__ = ['PluginCommunityArgs', 'PluginCommunity']
+__all__ = ['PluginArgs', 'Plugin']
 
 @pulumi.input_type
-class PluginCommunityArgs:
+class PluginArgs:
     def __init__(__self__, *,
                  enabled: pulumi.Input[bool],
                  instance_id: pulumi.Input[int],
                  name: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a PluginCommunity resource.
+        The set of arguments for constructing a Plugin resource.
         :param pulumi.Input[bool] enabled: Enable or disable the plugins.
         :param pulumi.Input[int] instance_id: The CloudAMQP instance ID.
-        :param pulumi.Input[str] name: The name of the Rabbit MQ community plugin.
+        :param pulumi.Input[str] name: The name of the Rabbit MQ plugin.
         """
         pulumi.set(__self__, "enabled", enabled)
         pulumi.set(__self__, "instance_id", instance_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
@@ -52,34 +52,34 @@
     def instance_id(self, value: pulumi.Input[int]):
         pulumi.set(self, "instance_id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the Rabbit MQ community plugin.
+        The name of the Rabbit MQ plugin.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
-class _PluginCommunityState:
+class _PluginState:
     def __init__(__self__, *,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  instance_id: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
-        Input properties used for looking up and filtering PluginCommunity resources.
+        Input properties used for looking up and filtering Plugin resources.
         :param pulumi.Input[bool] enabled: Enable or disable the plugins.
         :param pulumi.Input[int] instance_id: The CloudAMQP instance ID.
-        :param pulumi.Input[str] name: The name of the Rabbit MQ community plugin.
+        :param pulumi.Input[str] name: The name of the Rabbit MQ plugin.
         """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if instance_id is not None:
             pulumi.set(__self__, "instance_id", instance_id)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -108,109 +108,69 @@
     def instance_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "instance_id", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the Rabbit MQ community plugin.
+        The name of the Rabbit MQ plugin.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
-class PluginCommunity(pulumi.CustomResource):
+class Plugin(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  instance_id: Optional[pulumi.Input[int]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        This resource allows you to install or uninstall community plugins. Once installed the plugin will be available in `Plugin`.
-
-        Only available for dedicated subscription plans.
-
-        ⚠️  From our go API wrapper [v1.5.0](https://github.com/84codes/go-api/releases/tag/v1.5.0) there is support for multiple retries when requesting information about community plugins. This was introduced to avoid `ReadPluginCommunity error 400: Timeout talking to backend`.
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_cloudamqp as cloudamqp
-
-        rabbitmq_delayed_message_exchange = cloudamqp.PluginCommunity("rabbitmqDelayedMessageExchange",
-            instance_id=cloudamqp_instance["instance_01"]["id"],
-            enabled=True)
-        ```
-        ## Depedency
-
-        This resource depends on CloudAMQP instance identifier, `cloudamqp_instance.instance.id`.
-
         ## Import
 
         `cloudamqp_plugin` can be imported using the name argument of the resource together with CloudAMQP instance identifier. The name and identifier are CSV separated, see example below.
 
         ```sh
-         $ pulumi import cloudamqp:index/pluginCommunity:PluginCommunity <resource_name> <plugin_name>,<instance_id>`
+         $ pulumi import cloudamqp:index/plugin:Plugin rabbitmq_management rabbitmq_management,<instance_id>`
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] enabled: Enable or disable the plugins.
         :param pulumi.Input[int] instance_id: The CloudAMQP instance ID.
-        :param pulumi.Input[str] name: The name of the Rabbit MQ community plugin.
+        :param pulumi.Input[str] name: The name of the Rabbit MQ plugin.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: PluginCommunityArgs,
+                 args: PluginArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        This resource allows you to install or uninstall community plugins. Once installed the plugin will be available in `Plugin`.
-
-        Only available for dedicated subscription plans.
-
-        ⚠️  From our go API wrapper [v1.5.0](https://github.com/84codes/go-api/releases/tag/v1.5.0) there is support for multiple retries when requesting information about community plugins. This was introduced to avoid `ReadPluginCommunity error 400: Timeout talking to backend`.
-
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_cloudamqp as cloudamqp
-
-        rabbitmq_delayed_message_exchange = cloudamqp.PluginCommunity("rabbitmqDelayedMessageExchange",
-            instance_id=cloudamqp_instance["instance_01"]["id"],
-            enabled=True)
-        ```
-        ## Depedency
-
-        This resource depends on CloudAMQP instance identifier, `cloudamqp_instance.instance.id`.
-
         ## Import
 
         `cloudamqp_plugin` can be imported using the name argument of the resource together with CloudAMQP instance identifier. The name and identifier are CSV separated, see example below.
 
         ```sh
-         $ pulumi import cloudamqp:index/pluginCommunity:PluginCommunity <resource_name> <plugin_name>,<instance_id>`
+         $ pulumi import cloudamqp:index/plugin:Plugin rabbitmq_management rabbitmq_management,<instance_id>`
         ```
 
         :param str resource_name: The name of the resource.
-        :param PluginCommunityArgs args: The arguments to use to populate this resource's properties.
+        :param PluginArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(PluginCommunityArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(PluginArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
@@ -221,55 +181,55 @@
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = PluginCommunityArgs.__new__(PluginCommunityArgs)
+            __props__ = PluginArgs.__new__(PluginArgs)
 
             if enabled is None and not opts.urn:
                 raise TypeError("Missing required property 'enabled'")
             __props__.__dict__["enabled"] = enabled
             if instance_id is None and not opts.urn:
                 raise TypeError("Missing required property 'instance_id'")
             __props__.__dict__["instance_id"] = instance_id
             __props__.__dict__["name"] = name
-        super(PluginCommunity, __self__).__init__(
-            'cloudamqp:index/pluginCommunity:PluginCommunity',
+        super(Plugin, __self__).__init__(
+            'cloudamqp:index/plugin:Plugin',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             enabled: Optional[pulumi.Input[bool]] = None,
             instance_id: Optional[pulumi.Input[int]] = None,
-            name: Optional[pulumi.Input[str]] = None) -> 'PluginCommunity':
+            name: Optional[pulumi.Input[str]] = None) -> 'Plugin':
         """
-        Get an existing PluginCommunity resource's state with the given name, id, and optional extra
+        Get an existing Plugin resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] enabled: Enable or disable the plugins.
         :param pulumi.Input[int] instance_id: The CloudAMQP instance ID.
-        :param pulumi.Input[str] name: The name of the Rabbit MQ community plugin.
+        :param pulumi.Input[str] name: The name of the Rabbit MQ plugin.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _PluginCommunityState.__new__(_PluginCommunityState)
+        __props__ = _PluginState.__new__(_PluginState)
 
         __props__.__dict__["enabled"] = enabled
         __props__.__dict__["instance_id"] = instance_id
         __props__.__dict__["name"] = name
-        return PluginCommunity(resource_name, opts=opts, __props__=__props__)
+        return Plugin(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def enabled(self) -> pulumi.Output[bool]:
         """
         Enable or disable the plugins.
         """
@@ -283,11 +243,11 @@
         """
         return pulumi.get(self, "instance_id")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The name of the Rabbit MQ community plugin.
+        The name of the Rabbit MQ plugin.
         """
         return pulumi.get(self, "name")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/provider.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/rabbit_configuration.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/rabbit_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -500,39 +500,39 @@
         __props__.__dict__["max_message_size"] = max_message_size
         __props__.__dict__["queue_index_embed_msgs_below"] = queue_index_embed_msgs_below
         __props__.__dict__["vm_memory_high_watermark"] = vm_memory_high_watermark
         return RabbitConfiguration(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="channelMax")
-    def channel_max(self) -> pulumi.Output[Optional[int]]:
+    def channel_max(self) -> pulumi.Output[int]:
         """
         Set the maximum permissible number of channels per connection.
         """
         return pulumi.get(self, "channel_max")
 
     @property
     @pulumi.getter(name="connectionMax")
-    def connection_max(self) -> pulumi.Output[Optional[int]]:
+    def connection_max(self) -> pulumi.Output[int]:
         """
         Set the maximum permissible number of connection.
         """
         return pulumi.get(self, "connection_max")
 
     @property
     @pulumi.getter(name="consumerTimeout")
-    def consumer_timeout(self) -> pulumi.Output[Optional[int]]:
+    def consumer_timeout(self) -> pulumi.Output[int]:
         """
         A consumer that has recevied a message and does not acknowledge that message within the timeout in milliseconds
         """
         return pulumi.get(self, "consumer_timeout")
 
     @property
     @pulumi.getter
-    def heartbeat(self) -> pulumi.Output[Optional[int]]:
+    def heartbeat(self) -> pulumi.Output[int]:
         """
         Set the server AMQP 0-9-1 heartbeat timeout in seconds.
         """
         return pulumi.get(self, "heartbeat")
 
     @property
     @pulumi.getter(name="instanceId")
@@ -540,37 +540,37 @@
         """
         The CloudAMQP instance ID.
         """
         return pulumi.get(self, "instance_id")
 
     @property
     @pulumi.getter(name="logExchangeLevel")
-    def log_exchange_level(self) -> pulumi.Output[Optional[str]]:
+    def log_exchange_level(self) -> pulumi.Output[str]:
         """
         Log level for the logger used for log integrations and the CloudAMQP Console log view.
         """
         return pulumi.get(self, "log_exchange_level")
 
     @property
     @pulumi.getter(name="maxMessageSize")
-    def max_message_size(self) -> pulumi.Output[Optional[int]]:
+    def max_message_size(self) -> pulumi.Output[int]:
         """
         The largest allowed message payload size in bytes.
         """
         return pulumi.get(self, "max_message_size")
 
     @property
     @pulumi.getter(name="queueIndexEmbedMsgsBelow")
-    def queue_index_embed_msgs_below(self) -> pulumi.Output[Optional[int]]:
+    def queue_index_embed_msgs_below(self) -> pulumi.Output[int]:
         """
         Size in bytes below which to embed messages in the queue index.
         """
         return pulumi.get(self, "queue_index_embed_msgs_below")
 
     @property
     @pulumi.getter(name="vmMemoryHighWatermark")
-    def vm_memory_high_watermark(self) -> pulumi.Output[Optional[float]]:
+    def vm_memory_high_watermark(self) -> pulumi.Output[float]:
         """
         When the server will enter memory based flow-control as relative to the maximum available memory.
         """
         return pulumi.get(self, "vm_memory_high_watermark")
```

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/security_firewall.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/security_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/upgrade_rabbitmq.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/upgrade_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/vpc.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/vpc_gcp_peering.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/vpc_gcp_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/vpc_peering.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/vpc_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp/webhook.py` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp.egg-info/PKG-INFO` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-cloudamqp
-Version: 3.9.1
+Version: 3.9.2
 Summary: A Pulumi package for creating and managing CloudAMQP resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-cloudamqp
 Keywords: pulumi cloudamqp
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_cloudamqp-3.9.1/pulumi_cloudamqp.egg-info/SOURCES.txt` & `pulumi_cloudamqp-3.9.2/pulumi_cloudamqp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_cloudamqp-3.9.1/setup.py` & `pulumi_cloudamqp-3.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.9.1"
-PLUGIN_VERSION = "3.9.1"
+VERSION = "3.9.2"
+PLUGIN_VERSION = "3.9.2"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'cloudamqp', PLUGIN_VERSION])
         except OSError as error:
```

