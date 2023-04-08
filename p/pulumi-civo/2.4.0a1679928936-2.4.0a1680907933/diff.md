# Comparing `tmp/pulumi_civo-2.4.0a1679928936.tar.gz` & `tmp/pulumi_civo-2.4.0a1680907933.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_civo-2.4.0a1679928936.tar", last modified: Mon Mar 27 15:00:31 2023, max compression
+gzip compressed data, was "pulumi_civo-2.4.0a1680907933.tar", last modified: Fri Apr  7 23:00:34 2023, max compression
```

## Comparing `pulumi_civo-2.4.0a1679928936.tar` & `pulumi_civo-2.4.0a1680907933.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:00:31.751623 pulumi_civo-2.4.0a1679928936/
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-03-27 15:00:31.751623 pulumi_civo-2.4.0a1679928936/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:00:31.751623 pulumi_civo-2.4.0a1679928936/pulumi_civo/
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39145 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:00:31.751623 pulumi_civo-2.4.0a1679928936/pulumi_civo/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    22605 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    24236 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_disk_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_instances_size.py
--rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_kubernetes_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    47045 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/instance_reserved_ip_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    42980 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22159 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/kubernetes_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    47516 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo/volume_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:00:31.751623 pulumi_civo-2.4.0a1679928936/pulumi_civo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/pulumi_civo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 15:00:31.751623 pulumi_civo-2.4.0a1679928936/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-03-27 15:00:31.000000 pulumi_civo-2.4.0a1679928936/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:00:34.453971 pulumi_civo-2.4.0a1680907933/
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-07 23:00:34.453971 pulumi_civo-2.4.0a1680907933/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:00:34.449971 pulumi_civo-2.4.0a1680907933/pulumi_civo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39145 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:00:34.453971 pulumi_civo-2.4.0a1680907933/pulumi_civo/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17497 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22605 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24236 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7249 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_disk_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_instances_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12458 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_kubernetes_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4230 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47045 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/instance_reserved_ip_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42980 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22159 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/kubernetes_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47516 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo/volume_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 23:00:34.453971 pulumi_civo-2.4.0a1680907933/pulumi_civo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/pulumi_civo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 23:00:34.453971 pulumi_civo-2.4.0a1680907933/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-07 23:00:34.000000 pulumi_civo-2.4.0a1680907933/setup.py
```

### Comparing `pulumi_civo-2.4.0a1679928936/PKG-INFO` & `pulumi_civo-2.4.0a1680907933/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_civo
-Version: 2.4.0a1679928936
+Version: 2.4.0a1680907933
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi civo
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_civo-2.4.0a1679928936/README.md` & `pulumi_civo-2.4.0a1680907933/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/__init__.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/_inputs.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/_utilities.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/config/vars.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/database.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/dns_domain_name.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/dns_domain_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/dns_domain_record.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/firewall.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/firewall_rule.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_database.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_disk_image.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_disk_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_dns_domain_name.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_dns_domain_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_dns_domain_record.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_firewall.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_instance.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_instances.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_instances.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_instances_size.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_instances_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_kubernetes_cluster.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_kubernetes_version.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_kubernetes_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_load_balancer.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_network.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_object_store.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_object_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_object_store_credential.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_object_store_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_region.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_reserved_ip.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_reserved_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_size.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_ssh_key.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/get_volume.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/get_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/instance.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/instance_reserved_ip_assignment.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/instance_reserved_ip_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/kubernetes_cluster.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/kubernetes_node_pool.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/kubernetes_node_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/network.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/object_store.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/object_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/object_store_credential.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/object_store_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/outputs.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/provider.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/reserved_ip.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/reserved_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/ssh_key.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/volume.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo/volume_attachment.py` & `pulumi_civo-2.4.0a1680907933/pulumi_civo/volume_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo.egg-info/PKG-INFO` & `pulumi_civo-2.4.0a1680907933/pulumi_civo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-civo
-Version: 2.4.0a1679928936
+Version: 2.4.0a1680907933
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi civo
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_civo-2.4.0a1679928936/pulumi_civo.egg-info/SOURCES.txt` & `pulumi_civo-2.4.0a1680907933/pulumi_civo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1679928936/setup.py` & `pulumi_civo-2.4.0a1680907933/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.4.0a1679928936"
-PLUGIN_VERSION = "2.4.0-alpha.1679928936+e7ebcbe6"
+VERSION = "2.4.0a1680907933"
+PLUGIN_VERSION = "2.4.0-alpha.1680907933+c169dea2"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'civo', PLUGIN_VERSION])
         except OSError as error:
```

