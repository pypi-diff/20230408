# Comparing `tmp/pulumi_hcloud-1.9.0a1654086467.tar.gz` & `tmp/pulumi_hcloud-1.9.0a1657117726.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_hcloud-1.9.0a1654086467.tar", last modified: Wed Jun  1 12:34:20 2022, max compression
+gzip compressed data, was "dist/pulumi_hcloud-1.9.0a1657117726.tar", last modified: Wed Jul  6 14:32:20 2022, max compression
```

## Comparing `pulumi_hcloud-1.9.0a1654086467.tar` & `pulumi_hcloud-1.9.0a1657117726.tar`

### file list

```diff
@@ -1,71 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:34:20.000000 pulumi_hcloud-1.9.0a1654086467/
--rw-r--r--   0 runner    (1001) docker     (121)     2347 2022-06-01 12:34:20.000000 pulumi_hcloud-1.9.0a1654086467/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:34:20.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/
--rw-r--r--   0 runner    (1001) docker     (121)     5760 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27515 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     7667 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    13710 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:34:20.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/config/
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (121)    14300 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/firewall.py
--rw-r--r--   0 runner    (1001) docker     (121)    13565 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/firewall_attachment.py
--rw-r--r--   0 runner    (1001) docker     (121)    20617 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (121)     9500 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/floating_ip_assignment.py
--rw-r--r--   0 runner    (1001) docker     (121)     8103 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (121)     3815 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_certificates.py
--rw-r--r--   0 runner    (1001) docker     (121)     5661 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (121)     5290 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (121)     7595 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (121)     4406 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_firewalls.py
--rw-r--r--   0 runner    (1001) docker     (121)    10178 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (121)     3788 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_floating_ips.py
--rw-r--r--   0 runner    (1001) docker     (121)    10336 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_image.py
--rw-r--r--   0 runner    (1001) docker     (121)     5254 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_images.py
--rw-r--r--   0 runner    (1001) docker     (121)     9322 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3946 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_load_balancers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5940 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_location.py
--rw-r--r--   0 runner    (1001) docker     (121)     5146 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_locations.py
--rw-r--r--   0 runner    (1001) docker     (121)     6595 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_network.py
--rw-r--r--   0 runner    (1001) docker     (121)     3703 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_networks.py
--rw-r--r--   0 runner    (1001) docker     (121)     6953 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_placement_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     4845 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_placement_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)    14584 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_server.py
--rw-r--r--   0 runner    (1001) docker     (121)     5923 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_server_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     4722 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_server_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     4721 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_servers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6749 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (121)     3779 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)     9246 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (121)     4591 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_volumes.py
--rw-r--r--   0 runner    (1001) docker     (121)    25859 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (121)    21999 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/load_balancer_network.py
--rw-r--r--   0 runner    (1001) docker     (121)    21667 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/load_balancer_service.py
--rw-r--r--   0 runner    (1001) docker     (121)    18774 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/load_balancer_target.py
--rw-r--r--   0 runner    (1001) docker     (121)    17235 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/managed_certificate.py
--rw-r--r--   0 runner    (1001) docker     (121)    13033 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/network.py
--rw-r--r--   0 runner    (1001) docker     (121)    13297 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/network_route.py
--rw-r--r--   0 runner    (1001) docker     (121)    16092 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/network_subnet.py
--rw-r--r--   0 runner    (1001) docker     (121)    72034 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/outputs.py
--rw-r--r--   0 runner    (1001) docker     (121)    11247 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/placement_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     6039 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/provider.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    19402 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/rdns.py
--rw-r--r--   0 runner    (1001) docker     (121)    52756 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/server.py
--rw-r--r--   0 runner    (1001) docker     (121)    21558 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/server_network.py
--rw-r--r--   0 runner    (1001) docker     (121)    10698 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (121)    11508 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (121)    19004 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/uploaded_certificate.py
--rw-r--r--   0 runner    (1001) docker     (121)    21394 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/volume.py
--rw-r--r--   0 runner    (1001) docker     (121)    10917 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/volume_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-01 12:34:20.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2347 2022-06-01 12:34:20.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1999 2022-06-01 12:34:20.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 12:34:20.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-01 12:34:20.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-01 12:34:20.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-01 12:34:20.000000 pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-01 12:34:20.000000 pulumi_hcloud-1.9.0a1654086467/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-06-01 12:34:19.000000 pulumi_hcloud-1.9.0a1654086467/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/
+-rw-r--r--   0 runner    (1001) docker     (121)     2347 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1601 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/
+-rw-r--r--   0 runner    (1001) docker     (121)     5997 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    29307 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7667 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13710 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/config/
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      801 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14300 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13565 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/firewall_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20617 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9500 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/floating_ip_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8103 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3815 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5661 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5290 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7595 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4406 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_firewalls.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10178 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3788 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_floating_ips.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10336 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_image.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5254 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_images.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9322 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3946 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_load_balancers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5940 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5146 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_locations.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6595 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3703 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_networks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6953 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_placement_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4845 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_placement_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10859 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_primary_ip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3747 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_primary_ips.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14584 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5923 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_server_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4722 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_server_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4721 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_servers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6749 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3779 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9246 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4591 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25859 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21999 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/load_balancer_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21667 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/load_balancer_service.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18774 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/load_balancer_target.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17235 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/managed_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13033 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/network.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13297 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/network_route.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16092 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/network_subnet.py
+-rw-r--r--   0 runner    (1001) docker     (121)    76351 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11247 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/placement_group.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22220 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/primary_ip.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6039 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)    19402 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/rdns.py
+-rw-r--r--   0 runner    (1001) docker     (121)    55327 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/server.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21558 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/server_network.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10698 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11508 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19004 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/uploaded_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21394 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/volume.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10917 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/volume_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2347 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2092 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-07-06 14:32:20.000000 pulumi_hcloud-1.9.0a1657117726/setup.py
```

### Comparing `pulumi_hcloud-1.9.0a1654086467/PKG-INFO` & `pulumi_hcloud-1.9.0a1657117726/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_hcloud
-Version: 1.9.0a1654086467
+Version: 1.9.0a1657117726
 Summary: A Pulumi package for creating and managing hcloud cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-hcloud
 Description: # HCloud provider
         
         The HCloud resource provider for Pulumi lets you use Hetzner Cloud resources in your infrastructure
```

### Comparing `pulumi_hcloud-1.9.0a1654086467/README.md` & `pulumi_hcloud-1.9.0a1657117726/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/__init__.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 from .get_load_balancers import *
 from .get_location import *
 from .get_locations import *
 from .get_network import *
 from .get_networks import *
 from .get_placement_group import *
 from .get_placement_groups import *
+from .get_primary_ip import *
+from .get_primary_ips import *
 from .get_server import *
 from .get_server_type import *
 from .get_server_types import *
 from .get_servers import *
 from .get_ssh_key import *
 from .get_ssh_keys import *
 from .get_volume import *
@@ -41,14 +43,15 @@
 from .load_balancer_service import *
 from .load_balancer_target import *
 from .managed_certificate import *
 from .network import *
 from .network_route import *
 from .network_subnet import *
 from .placement_group import *
+from .primary_ip import *
 from .provider import *
 from .rdns import *
 from .server import *
 from .server_network import *
 from .snapshot import *
 from .ssh_key import *
 from .uploaded_certificate import *
@@ -177,14 +180,22 @@
   "fqn": "pulumi_hcloud",
   "classes": {
    "hcloud:index/placementGroup:PlacementGroup": "PlacementGroup"
   }
  },
  {
   "pkg": "hcloud",
+  "mod": "index/primaryIp",
+  "fqn": "pulumi_hcloud",
+  "classes": {
+   "hcloud:index/primaryIp:PrimaryIp": "PrimaryIp"
+  }
+ },
+ {
+  "pkg": "hcloud",
   "mod": "index/rdns",
   "fqn": "pulumi_hcloud",
   "classes": {
    "hcloud:index/rdns:Rdns": "Rdns"
   }
  },
  {
```

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/_inputs.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     'FirewallRuleArgs',
     'LoadBalancerAlgorithmArgs',
     'LoadBalancerServiceHealthCheckArgs',
     'LoadBalancerServiceHealthCheckHttpArgs',
     'LoadBalancerServiceHttpArgs',
     'LoadBalancerTargetArgs',
     'ServerNetworkArgs',
+    'ServerPublicNetArgs',
     'GetFirewallApplyToArgs',
     'GetFirewallRuleArgs',
 ]
 
 @pulumi.input_type
 class FirewallApplyToArgs:
     def __init__(__self__, *,
@@ -583,14 +584,67 @@
 
     @mac_address.setter
     def mac_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "mac_address", value)
 
 
 @pulumi.input_type
+class ServerPublicNetArgs:
+    def __init__(__self__, *,
+                 ipv4: Optional[pulumi.Input[int]] = None,
+                 ipv4_enabled: Optional[pulumi.Input[bool]] = None,
+                 ipv6: Optional[pulumi.Input[int]] = None,
+                 ipv6_enabled: Optional[pulumi.Input[bool]] = None):
+        if ipv4 is not None:
+            pulumi.set(__self__, "ipv4", ipv4)
+        if ipv4_enabled is not None:
+            pulumi.set(__self__, "ipv4_enabled", ipv4_enabled)
+        if ipv6 is not None:
+            pulumi.set(__self__, "ipv6", ipv6)
+        if ipv6_enabled is not None:
+            pulumi.set(__self__, "ipv6_enabled", ipv6_enabled)
+
+    @property
+    @pulumi.getter
+    def ipv4(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "ipv4")
+
+    @ipv4.setter
+    def ipv4(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "ipv4", value)
+
+    @property
+    @pulumi.getter(name="ipv4Enabled")
+    def ipv4_enabled(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "ipv4_enabled")
+
+    @ipv4_enabled.setter
+    def ipv4_enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "ipv4_enabled", value)
+
+    @property
+    @pulumi.getter
+    def ipv6(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "ipv6")
+
+    @ipv6.setter
+    def ipv6(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "ipv6", value)
+
+    @property
+    @pulumi.getter(name="ipv6Enabled")
+    def ipv6_enabled(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "ipv6_enabled")
+
+    @ipv6_enabled.setter
+    def ipv6_enabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "ipv6_enabled", value)
+
+
+@pulumi.input_type
 class GetFirewallApplyToArgs:
     def __init__(__self__, *,
                  label_selector: str,
                  server: int):
         """
         :param str label_selector: (string) Label Selector to select servers the firewall is applied to. Empty if a server is directly
                referenced
```

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/_utilities.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/certificate.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/config/vars.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/firewall.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/firewall_attachment.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/firewall_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/floating_ip.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/floating_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/floating_ip_assignment.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/floating_ip_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_certificate.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_certificates.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_certificates.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_datacenter.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_datacenters.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_firewall.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_firewalls.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_firewalls.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_floating_ip.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_floating_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_floating_ips.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_floating_ips.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_image.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_images.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_images.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_load_balancer.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_load_balancers.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_load_balancers.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_location.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_location.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_locations.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_locations.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_network.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_networks.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_placement_group.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_placement_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_placement_groups.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_placement_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_server.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_server_type.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_server_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_server_types.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_server_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_servers.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_ssh_key.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_ssh_keys.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_volume.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/get_volumes.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/get_volumes.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/load_balancer.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/load_balancer_network.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/load_balancer_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/load_balancer_service.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/load_balancer_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/load_balancer_target.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/load_balancer_target.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/managed_certificate.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/managed_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/network.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/network_route.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/network_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/network_subnet.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/network_subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/outputs.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     'FirewallRule',
     'LoadBalancerAlgorithm',
     'LoadBalancerServiceHealthCheck',
     'LoadBalancerServiceHealthCheckHttp',
     'LoadBalancerServiceHttp',
     'LoadBalancerTarget',
     'ServerNetwork',
+    'ServerPublicNet',
     'GetCertificatesCertificateResult',
     'GetDatacentersDatacenterResult',
     'GetFirewallApplyToResult',
     'GetFirewallRuleResult',
     'GetFirewallsFirewallResult',
     'GetFirewallsFirewallApplyToResult',
     'GetFirewallsFirewallRuleResult',
@@ -39,14 +40,15 @@
     'GetLoadBalancersLoadBalancerServiceHealthCheckResult',
     'GetLoadBalancersLoadBalancerServiceHealthCheckHttpResult',
     'GetLoadBalancersLoadBalancerServiceHttpResult',
     'GetLoadBalancersLoadBalancerTargetResult',
     'GetLocationsLocationResult',
     'GetNetworksNetworkResult',
     'GetPlacementGroupsPlacementGroupResult',
+    'GetPrimaryIpsPrimaryIpResult',
     'GetServerTypesServerTypeResult',
     'GetServersServerResult',
     'GetSshKeysSshKeyResult',
     'GetVolumesVolumeResult',
 ]
 
 @pulumi.output_type
@@ -596,14 +598,70 @@
         """
         (Optional, string) The MAC address the private interface of the server has
         """
         return pulumi.get(self, "mac_address")
 
 
 @pulumi.output_type
+class ServerPublicNet(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "ipv4Enabled":
+            suggest = "ipv4_enabled"
+        elif key == "ipv6Enabled":
+            suggest = "ipv6_enabled"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in ServerPublicNet. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        ServerPublicNet.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        ServerPublicNet.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 ipv4: Optional[int] = None,
+                 ipv4_enabled: Optional[bool] = None,
+                 ipv6: Optional[int] = None,
+                 ipv6_enabled: Optional[bool] = None):
+        if ipv4 is not None:
+            pulumi.set(__self__, "ipv4", ipv4)
+        if ipv4_enabled is not None:
+            pulumi.set(__self__, "ipv4_enabled", ipv4_enabled)
+        if ipv6 is not None:
+            pulumi.set(__self__, "ipv6", ipv6)
+        if ipv6_enabled is not None:
+            pulumi.set(__self__, "ipv6_enabled", ipv6_enabled)
+
+    @property
+    @pulumi.getter
+    def ipv4(self) -> Optional[int]:
+        return pulumi.get(self, "ipv4")
+
+    @property
+    @pulumi.getter(name="ipv4Enabled")
+    def ipv4_enabled(self) -> Optional[bool]:
+        return pulumi.get(self, "ipv4_enabled")
+
+    @property
+    @pulumi.getter
+    def ipv6(self) -> Optional[int]:
+        return pulumi.get(self, "ipv6")
+
+    @property
+    @pulumi.getter(name="ipv6Enabled")
+    def ipv6_enabled(self) -> Optional[bool]:
+        return pulumi.get(self, "ipv6_enabled")
+
+
+@pulumi.output_type
 class GetCertificatesCertificateResult(dict):
     def __init__(__self__, *,
                  certificate: str,
                  created: str,
                  domain_names: Sequence[str],
                  fingerprint: str,
                  id: int,
@@ -1879,14 +1937,97 @@
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
+class GetPrimaryIpsPrimaryIpResult(dict):
+    def __init__(__self__, *,
+                 assignee_id: int,
+                 assignee_type: str,
+                 auto_delete: bool,
+                 datacenter: str,
+                 delete_protection: bool,
+                 id: int,
+                 ip_address: str,
+                 ip_network: str,
+                 labels: Mapping[str, Any],
+                 type: str,
+                 name: Optional[str] = None):
+        pulumi.set(__self__, "assignee_id", assignee_id)
+        pulumi.set(__self__, "assignee_type", assignee_type)
+        pulumi.set(__self__, "auto_delete", auto_delete)
+        pulumi.set(__self__, "datacenter", datacenter)
+        pulumi.set(__self__, "delete_protection", delete_protection)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "ip_address", ip_address)
+        pulumi.set(__self__, "ip_network", ip_network)
+        pulumi.set(__self__, "labels", labels)
+        pulumi.set(__self__, "type", type)
+        if name is not None:
+            pulumi.set(__self__, "name", name)
+
+    @property
+    @pulumi.getter(name="assigneeId")
+    def assignee_id(self) -> int:
+        return pulumi.get(self, "assignee_id")
+
+    @property
+    @pulumi.getter(name="assigneeType")
+    def assignee_type(self) -> str:
+        return pulumi.get(self, "assignee_type")
+
+    @property
+    @pulumi.getter(name="autoDelete")
+    def auto_delete(self) -> bool:
+        return pulumi.get(self, "auto_delete")
+
+    @property
+    @pulumi.getter
+    def datacenter(self) -> str:
+        return pulumi.get(self, "datacenter")
+
+    @property
+    @pulumi.getter(name="deleteProtection")
+    def delete_protection(self) -> bool:
+        return pulumi.get(self, "delete_protection")
+
+    @property
+    @pulumi.getter
+    def id(self) -> int:
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="ipAddress")
+    def ip_address(self) -> str:
+        return pulumi.get(self, "ip_address")
+
+    @property
+    @pulumi.getter(name="ipNetwork")
+    def ip_network(self) -> str:
+        return pulumi.get(self, "ip_network")
+
+    @property
+    @pulumi.getter
+    def labels(self) -> Mapping[str, Any]:
+        return pulumi.get(self, "labels")
+
+    @property
+    @pulumi.getter
+    def type(self) -> str:
+        return pulumi.get(self, "type")
+
+    @property
+    @pulumi.getter
+    def name(self) -> Optional[str]:
+        return pulumi.get(self, "name")
+
+
+@pulumi.output_type
 class GetServerTypesServerTypeResult(dict):
     def __init__(__self__, *,
                  cores: int,
                  cpu_type: str,
                  description: str,
                  disk: int,
                  id: int,
```

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/placement_group.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/placement_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/provider.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/rdns.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/rdns.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/server.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
                  iso: Optional[pulumi.Input[str]] = None,
                  keep_disk: Optional[pulumi.Input[bool]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  location: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  networks: Optional[pulumi.Input[Sequence[pulumi.Input['ServerNetworkArgs']]]] = None,
                  placement_group_id: Optional[pulumi.Input[int]] = None,
+                 public_nets: Optional[pulumi.Input[Sequence[pulumi.Input['ServerPublicNetArgs']]]] = None,
                  rebuild_protection: Optional[pulumi.Input[bool]] = None,
                  rescue: Optional[pulumi.Input[str]] = None,
                  ssh_keys: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  user_data: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a Server resource.
         :param pulumi.Input[str] server_type: Name of the server type this server should be created with.
@@ -49,14 +50,15 @@
         :param pulumi.Input[str] iso: ID or Name of an ISO image to mount.
         :param pulumi.Input[bool] keep_disk: If true, do not upgrade the disk. This allows downgrading the server type later.
         :param pulumi.Input[Mapping[str, Any]] labels: User-defined labels (key-value pairs) should be created with.
         :param pulumi.Input[str] location: The location name to create the server in. `nbg1`, `fsn1`, `hel1` or `ash`
         :param pulumi.Input[str] name: Name of the server to create (must be unique per project and a valid hostname as per RFC 1123).
         :param pulumi.Input[Sequence[pulumi.Input['ServerNetworkArgs']]] networks: Network the server should be attached to on creation. (Can be specified multiple times)
         :param pulumi.Input[int] placement_group_id: Placement Group ID the server added to on creation.
+        :param pulumi.Input[Sequence[pulumi.Input['ServerPublicNetArgs']]] public_nets: In this block you can either enable / disable ipv4 and ipv6 or link existing primary IPs (checkout the examples)
         :param pulumi.Input[bool] rebuild_protection: Enable or disable rebuild protection (Needs to be the same as `delete_protection`).
         :param pulumi.Input[str] rescue: Enable and boot in to the specified rescue system. This enables simple installation of custom operating systems. `linux64` `linux32` or `freebsd64`
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ssh_keys: SSH key IDs or names which should be injected into the server at creation time
         :param pulumi.Input[str] user_data: Cloud-Init user data to use during server creation
         """
         pulumi.set(__self__, "server_type", server_type)
         if backups is not None:
@@ -81,14 +83,16 @@
             pulumi.set(__self__, "location", location)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if networks is not None:
             pulumi.set(__self__, "networks", networks)
         if placement_group_id is not None:
             pulumi.set(__self__, "placement_group_id", placement_group_id)
+        if public_nets is not None:
+            pulumi.set(__self__, "public_nets", public_nets)
         if rebuild_protection is not None:
             pulumi.set(__self__, "rebuild_protection", rebuild_protection)
         if rescue is not None:
             pulumi.set(__self__, "rescue", rescue)
         if ssh_keys is not None:
             pulumi.set(__self__, "ssh_keys", ssh_keys)
         if user_data is not None:
@@ -263,14 +267,26 @@
         return pulumi.get(self, "placement_group_id")
 
     @placement_group_id.setter
     def placement_group_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "placement_group_id", value)
 
     @property
+    @pulumi.getter(name="publicNets")
+    def public_nets(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServerPublicNetArgs']]]]:
+        """
+        In this block you can either enable / disable ipv4 and ipv6 or link existing primary IPs (checkout the examples)
+        """
+        return pulumi.get(self, "public_nets")
+
+    @public_nets.setter
+    def public_nets(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServerPublicNetArgs']]]]):
+        pulumi.set(self, "public_nets", value)
+
+    @property
     @pulumi.getter(name="rebuildProtection")
     def rebuild_protection(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable or disable rebuild protection (Needs to be the same as `delete_protection`).
         """
         return pulumi.get(self, "rebuild_protection")
 
@@ -331,14 +347,15 @@
                  iso: Optional[pulumi.Input[str]] = None,
                  keep_disk: Optional[pulumi.Input[bool]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  location: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  networks: Optional[pulumi.Input[Sequence[pulumi.Input['ServerNetworkArgs']]]] = None,
                  placement_group_id: Optional[pulumi.Input[int]] = None,
+                 public_nets: Optional[pulumi.Input[Sequence[pulumi.Input['ServerPublicNetArgs']]]] = None,
                  rebuild_protection: Optional[pulumi.Input[bool]] = None,
                  rescue: Optional[pulumi.Input[str]] = None,
                  server_type: Optional[pulumi.Input[str]] = None,
                  ssh_keys: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  status: Optional[pulumi.Input[str]] = None,
                  user_data: Optional[pulumi.Input[str]] = None):
         """
@@ -360,14 +377,15 @@
         :param pulumi.Input[str] iso: ID or Name of an ISO image to mount.
         :param pulumi.Input[bool] keep_disk: If true, do not upgrade the disk. This allows downgrading the server type later.
         :param pulumi.Input[Mapping[str, Any]] labels: User-defined labels (key-value pairs) should be created with.
         :param pulumi.Input[str] location: The location name to create the server in. `nbg1`, `fsn1`, `hel1` or `ash`
         :param pulumi.Input[str] name: Name of the server to create (must be unique per project and a valid hostname as per RFC 1123).
         :param pulumi.Input[Sequence[pulumi.Input['ServerNetworkArgs']]] networks: Network the server should be attached to on creation. (Can be specified multiple times)
         :param pulumi.Input[int] placement_group_id: Placement Group ID the server added to on creation.
+        :param pulumi.Input[Sequence[pulumi.Input['ServerPublicNetArgs']]] public_nets: In this block you can either enable / disable ipv4 and ipv6 or link existing primary IPs (checkout the examples)
         :param pulumi.Input[bool] rebuild_protection: Enable or disable rebuild protection (Needs to be the same as `delete_protection`).
         :param pulumi.Input[str] rescue: Enable and boot in to the specified rescue system. This enables simple installation of custom operating systems. `linux64` `linux32` or `freebsd64`
         :param pulumi.Input[str] server_type: Name of the server type this server should be created with.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ssh_keys: SSH key IDs or names which should be injected into the server at creation time
         :param pulumi.Input[str] status: (string) The status of the server.
         :param pulumi.Input[str] user_data: Cloud-Init user data to use during server creation
         """
@@ -404,14 +422,16 @@
             pulumi.set(__self__, "location", location)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if networks is not None:
             pulumi.set(__self__, "networks", networks)
         if placement_group_id is not None:
             pulumi.set(__self__, "placement_group_id", placement_group_id)
+        if public_nets is not None:
+            pulumi.set(__self__, "public_nets", public_nets)
         if rebuild_protection is not None:
             pulumi.set(__self__, "rebuild_protection", rebuild_protection)
         if rescue is not None:
             pulumi.set(__self__, "rescue", rescue)
         if server_type is not None:
             pulumi.set(__self__, "server_type", server_type)
         if ssh_keys is not None:
@@ -626,14 +646,26 @@
         return pulumi.get(self, "placement_group_id")
 
     @placement_group_id.setter
     def placement_group_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "placement_group_id", value)
 
     @property
+    @pulumi.getter(name="publicNets")
+    def public_nets(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ServerPublicNetArgs']]]]:
+        """
+        In this block you can either enable / disable ipv4 and ipv6 or link existing primary IPs (checkout the examples)
+        """
+        return pulumi.get(self, "public_nets")
+
+    @public_nets.setter
+    def public_nets(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ServerPublicNetArgs']]]]):
+        pulumi.set(self, "public_nets", value)
+
+    @property
     @pulumi.getter(name="rebuildProtection")
     def rebuild_protection(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable or disable rebuild protection (Needs to be the same as `delete_protection`).
         """
         return pulumi.get(self, "rebuild_protection")
 
@@ -716,35 +748,24 @@
                  iso: Optional[pulumi.Input[str]] = None,
                  keep_disk: Optional[pulumi.Input[bool]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  location: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  networks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerNetworkArgs']]]]] = None,
                  placement_group_id: Optional[pulumi.Input[int]] = None,
+                 public_nets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerPublicNetArgs']]]]] = None,
                  rebuild_protection: Optional[pulumi.Input[bool]] = None,
                  rescue: Optional[pulumi.Input[str]] = None,
                  server_type: Optional[pulumi.Input[str]] = None,
                  ssh_keys: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         ## Example Usage
-        ### Basic server creation
-
-        ```python
-        import pulumi
-        import pulumi_hcloud as hcloud
-
-        # Create a new server running debian
-        node1 = hcloud.Server("node1",
-            image="debian-9",
-            server_type="cx11")
-        ```
         ### Server creation with network
-
         ```python
         import pulumi
         import pulumi_hcloud as hcloud
 
         network = hcloud.Network("network", ip_range="10.0.0.0/16")
         network_subnet = hcloud.NetworkSubnet("network-subnet",
             type="cloud",
@@ -789,41 +810,30 @@
         :param pulumi.Input[str] iso: ID or Name of an ISO image to mount.
         :param pulumi.Input[bool] keep_disk: If true, do not upgrade the disk. This allows downgrading the server type later.
         :param pulumi.Input[Mapping[str, Any]] labels: User-defined labels (key-value pairs) should be created with.
         :param pulumi.Input[str] location: The location name to create the server in. `nbg1`, `fsn1`, `hel1` or `ash`
         :param pulumi.Input[str] name: Name of the server to create (must be unique per project and a valid hostname as per RFC 1123).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerNetworkArgs']]]] networks: Network the server should be attached to on creation. (Can be specified multiple times)
         :param pulumi.Input[int] placement_group_id: Placement Group ID the server added to on creation.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerPublicNetArgs']]]] public_nets: In this block you can either enable / disable ipv4 and ipv6 or link existing primary IPs (checkout the examples)
         :param pulumi.Input[bool] rebuild_protection: Enable or disable rebuild protection (Needs to be the same as `delete_protection`).
         :param pulumi.Input[str] rescue: Enable and boot in to the specified rescue system. This enables simple installation of custom operating systems. `linux64` `linux32` or `freebsd64`
         :param pulumi.Input[str] server_type: Name of the server type this server should be created with.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ssh_keys: SSH key IDs or names which should be injected into the server at creation time
         :param pulumi.Input[str] user_data: Cloud-Init user data to use during server creation
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: ServerArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         ## Example Usage
-        ### Basic server creation
-
-        ```python
-        import pulumi
-        import pulumi_hcloud as hcloud
-
-        # Create a new server running debian
-        node1 = hcloud.Server("node1",
-            image="debian-9",
-            server_type="cx11")
-        ```
         ### Server creation with network
-
         ```python
         import pulumi
         import pulumi_hcloud as hcloud
 
         network = hcloud.Network("network", ip_range="10.0.0.0/16")
         network_subnet = hcloud.NetworkSubnet("network-subnet",
             type="cloud",
@@ -877,14 +887,15 @@
                  iso: Optional[pulumi.Input[str]] = None,
                  keep_disk: Optional[pulumi.Input[bool]] = None,
                  labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  location: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  networks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerNetworkArgs']]]]] = None,
                  placement_group_id: Optional[pulumi.Input[int]] = None,
+                 public_nets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerPublicNetArgs']]]]] = None,
                  rebuild_protection: Optional[pulumi.Input[bool]] = None,
                  rescue: Optional[pulumi.Input[str]] = None,
                  server_type: Optional[pulumi.Input[str]] = None,
                  ssh_keys: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  user_data: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         if opts is None:
@@ -907,14 +918,15 @@
             __props__.__dict__["iso"] = iso
             __props__.__dict__["keep_disk"] = keep_disk
             __props__.__dict__["labels"] = labels
             __props__.__dict__["location"] = location
             __props__.__dict__["name"] = name
             __props__.__dict__["networks"] = networks
             __props__.__dict__["placement_group_id"] = placement_group_id
+            __props__.__dict__["public_nets"] = public_nets
             __props__.__dict__["rebuild_protection"] = rebuild_protection
             __props__.__dict__["rescue"] = rescue
             if server_type is None and not opts.urn:
                 raise TypeError("Missing required property 'server_type'")
             __props__.__dict__["server_type"] = server_type
             __props__.__dict__["ssh_keys"] = ssh_keys
             __props__.__dict__["user_data"] = user_data
@@ -946,14 +958,15 @@
             iso: Optional[pulumi.Input[str]] = None,
             keep_disk: Optional[pulumi.Input[bool]] = None,
             labels: Optional[pulumi.Input[Mapping[str, Any]]] = None,
             location: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             networks: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerNetworkArgs']]]]] = None,
             placement_group_id: Optional[pulumi.Input[int]] = None,
+            public_nets: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerPublicNetArgs']]]]] = None,
             rebuild_protection: Optional[pulumi.Input[bool]] = None,
             rescue: Optional[pulumi.Input[str]] = None,
             server_type: Optional[pulumi.Input[str]] = None,
             ssh_keys: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             status: Optional[pulumi.Input[str]] = None,
             user_data: Optional[pulumi.Input[str]] = None) -> 'Server':
         """
@@ -980,14 +993,15 @@
         :param pulumi.Input[str] iso: ID or Name of an ISO image to mount.
         :param pulumi.Input[bool] keep_disk: If true, do not upgrade the disk. This allows downgrading the server type later.
         :param pulumi.Input[Mapping[str, Any]] labels: User-defined labels (key-value pairs) should be created with.
         :param pulumi.Input[str] location: The location name to create the server in. `nbg1`, `fsn1`, `hel1` or `ash`
         :param pulumi.Input[str] name: Name of the server to create (must be unique per project and a valid hostname as per RFC 1123).
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerNetworkArgs']]]] networks: Network the server should be attached to on creation. (Can be specified multiple times)
         :param pulumi.Input[int] placement_group_id: Placement Group ID the server added to on creation.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ServerPublicNetArgs']]]] public_nets: In this block you can either enable / disable ipv4 and ipv6 or link existing primary IPs (checkout the examples)
         :param pulumi.Input[bool] rebuild_protection: Enable or disable rebuild protection (Needs to be the same as `delete_protection`).
         :param pulumi.Input[str] rescue: Enable and boot in to the specified rescue system. This enables simple installation of custom operating systems. `linux64` `linux32` or `freebsd64`
         :param pulumi.Input[str] server_type: Name of the server type this server should be created with.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ssh_keys: SSH key IDs or names which should be injected into the server at creation time
         :param pulumi.Input[str] status: (string) The status of the server.
         :param pulumi.Input[str] user_data: Cloud-Init user data to use during server creation
         """
@@ -1008,14 +1022,15 @@
         __props__.__dict__["iso"] = iso
         __props__.__dict__["keep_disk"] = keep_disk
         __props__.__dict__["labels"] = labels
         __props__.__dict__["location"] = location
         __props__.__dict__["name"] = name
         __props__.__dict__["networks"] = networks
         __props__.__dict__["placement_group_id"] = placement_group_id
+        __props__.__dict__["public_nets"] = public_nets
         __props__.__dict__["rebuild_protection"] = rebuild_protection
         __props__.__dict__["rescue"] = rescue
         __props__.__dict__["server_type"] = server_type
         __props__.__dict__["ssh_keys"] = ssh_keys
         __props__.__dict__["status"] = status
         __props__.__dict__["user_data"] = user_data
         return Server(resource_name, opts=opts, __props__=__props__)
@@ -1157,14 +1172,22 @@
     def placement_group_id(self) -> pulumi.Output[Optional[int]]:
         """
         Placement Group ID the server added to on creation.
         """
         return pulumi.get(self, "placement_group_id")
 
     @property
+    @pulumi.getter(name="publicNets")
+    def public_nets(self) -> pulumi.Output[Optional[Sequence['outputs.ServerPublicNet']]]:
+        """
+        In this block you can either enable / disable ipv4 and ipv6 or link existing primary IPs (checkout the examples)
+        """
+        return pulumi.get(self, "public_nets")
+
+    @property
     @pulumi.getter(name="rebuildProtection")
     def rebuild_protection(self) -> pulumi.Output[Optional[bool]]:
         """
         Enable or disable rebuild protection (Needs to be the same as `delete_protection`).
         """
         return pulumi.get(self, "rebuild_protection")
```

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/server_network.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/server_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/snapshot.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/ssh_key.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/uploaded_certificate.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/uploaded_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/volume.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud/volume_attachment.py` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud/volume_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud.egg-info/PKG-INFO` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-hcloud
-Version: 1.9.0a1654086467
+Version: 1.9.0a1657117726
 Summary: A Pulumi package for creating and managing hcloud cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-hcloud
 Description: # HCloud provider
         
         The HCloud resource provider for Pulumi lets you use Hetzner Cloud resources in your infrastructure
```

### Comparing `pulumi_hcloud-1.9.0a1654086467/pulumi_hcloud.egg-info/SOURCES.txt` & `pulumi_hcloud-1.9.0a1657117726/pulumi_hcloud.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 pulumi_hcloud/get_load_balancers.py
 pulumi_hcloud/get_location.py
 pulumi_hcloud/get_locations.py
 pulumi_hcloud/get_network.py
 pulumi_hcloud/get_networks.py
 pulumi_hcloud/get_placement_group.py
 pulumi_hcloud/get_placement_groups.py
+pulumi_hcloud/get_primary_ip.py
+pulumi_hcloud/get_primary_ips.py
 pulumi_hcloud/get_server.py
 pulumi_hcloud/get_server_type.py
 pulumi_hcloud/get_server_types.py
 pulumi_hcloud/get_servers.py
 pulumi_hcloud/get_ssh_key.py
 pulumi_hcloud/get_ssh_keys.py
 pulumi_hcloud/get_volume.py
@@ -40,14 +42,15 @@
 pulumi_hcloud/load_balancer_target.py
 pulumi_hcloud/managed_certificate.py
 pulumi_hcloud/network.py
 pulumi_hcloud/network_route.py
 pulumi_hcloud/network_subnet.py
 pulumi_hcloud/outputs.py
 pulumi_hcloud/placement_group.py
+pulumi_hcloud/primary_ip.py
 pulumi_hcloud/provider.py
 pulumi_hcloud/pulumi-plugin.json
 pulumi_hcloud/py.typed
 pulumi_hcloud/rdns.py
 pulumi_hcloud/server.py
 pulumi_hcloud/server_network.py
 pulumi_hcloud/snapshot.py
```

### Comparing `pulumi_hcloud-1.9.0a1654086467/setup.py` & `pulumi_hcloud-1.9.0a1657117726/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.9.0a1654086467"
-PLUGIN_VERSION = "1.9.0-alpha.1654086467+434a3aef"
+VERSION = "1.9.0a1657117726"
+PLUGIN_VERSION = "1.9.0-alpha.1657117726+18f6e4c3"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'hcloud', PLUGIN_VERSION])
         except OSError as error:
```

