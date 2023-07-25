# Comparing `tmp/pulumi_civo-2.4.0a1690262333.tar.gz` & `tmp/pulumi_civo-2.4.0a1690301883.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_civo-2.4.0a1690262333.tar", last modified: Tue Jul 25 05:24:08 2023, max compression
+gzip compressed data, was "pulumi_civo-2.4.0a1690301883.tar", last modified: Tue Jul 25 16:22:11 2023, max compression
```

## Comparing `pulumi_civo-2.4.0a1690262333.tar` & `pulumi_civo-2.4.0a1690301883.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:24:08.556493 pulumi_civo-2.4.0a1690262333/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-25 05:24:08.556493 pulumi_civo-2.4.0a1690262333/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:24:08.552493 pulumi_civo-2.4.0a1690262333/pulumi_civo/
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39031 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:24:08.556493 pulumi_civo-2.4.0a1690262333/pulumi_civo/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    22605 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    24236 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_database_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_disk_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_dns_domain_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_dns_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_kubernetes_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    47906 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/instance_reserved_ip_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)    44789 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/kubernetes_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    23500 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/kubernetes_node_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/object_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/object_store_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)    46709 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo/volume_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 05:24:08.556493 pulumi_civo-2.4.0a1690262333/pulumi_civo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/pulumi_civo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 05:24:08.556493 pulumi_civo-2.4.0a1690262333/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-25 05:24:08.000000 pulumi_civo-2.4.0a1690262333/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:22:11.268502 pulumi_civo-2.4.0a1690301883/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-25 16:22:11.268502 pulumi_civo-2.4.0a1690301883/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:22:11.268502 pulumi_civo-2.4.0a1690301883/pulumi_civo/
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39745 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:22:11.268502 pulumi_civo-2.4.0a1690301883/pulumi_civo/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22605 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24236 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9625 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_database_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_disk_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_dns_domain_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_dns_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13408 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_kubernetes_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5164 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47906 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/instance_reserved_ip_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44789 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/kubernetes_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25745 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/kubernetes_node_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15501 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/object_store_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47579 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7299 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9414 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo/volume_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 16:22:11.268502 pulumi_civo-2.4.0a1690301883/pulumi_civo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2423 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/pulumi_civo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 16:22:11.268502 pulumi_civo-2.4.0a1690301883/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-25 16:22:11.000000 pulumi_civo-2.4.0a1690301883/setup.py
```

### Comparing `pulumi_civo-2.4.0a1690262333/PKG-INFO` & `pulumi_civo-2.4.0a1690301883/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_civo
-Version: 2.4.0a1690262333
+Version: 2.4.0a1690301883
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi civo
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_civo-2.4.0a1690262333/README.md` & `pulumi_civo-2.4.0a1690301883/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/__init__.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/_inputs.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/_inputs.py`

 * *Files 4% similar despite different names*

```diff
@@ -285,27 +285,31 @@
 
 @pulumi.input_type
 class KubernetesClusterPoolsArgs:
     def __init__(__self__, *,
                  node_count: pulumi.Input[int],
                  size: pulumi.Input[str],
                  instance_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 label: Optional[pulumi.Input[str]] = None):
+                 label: Optional[pulumi.Input[str]] = None,
+                 public_ip_node_pool: Optional[pulumi.Input[bool]] = None):
         """
         :param pulumi.Input[int] node_count: Number of nodes in the nodepool
         :param pulumi.Input[str] size: Size of the nodes in the nodepool
         :param pulumi.Input[Sequence[pulumi.Input[str]]] instance_names: Instance names in the nodepool
         :param pulumi.Input[str] label: Node pool label, if you don't provide one, we will generate one for you
+        :param pulumi.Input[bool] public_ip_node_pool: Node pool belongs to the public ip node pool
         """
         pulumi.set(__self__, "node_count", node_count)
         pulumi.set(__self__, "size", size)
         if instance_names is not None:
             pulumi.set(__self__, "instance_names", instance_names)
         if label is not None:
             pulumi.set(__self__, "label", label)
+        if public_ip_node_pool is not None:
+            pulumi.set(__self__, "public_ip_node_pool", public_ip_node_pool)
 
     @property
     @pulumi.getter(name="nodeCount")
     def node_count(self) -> pulumi.Input[int]:
         """
         Number of nodes in the nodepool
         """
@@ -347,14 +351,26 @@
         """
         return pulumi.get(self, "label")
 
     @label.setter
     def label(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "label", value)
 
+    @property
+    @pulumi.getter(name="publicIpNodePool")
+    def public_ip_node_pool(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Node pool belongs to the public ip node pool
+        """
+        return pulumi.get(self, "public_ip_node_pool")
+
+    @public_ip_node_pool.setter
+    def public_ip_node_pool(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "public_ip_node_pool", value)
+
 
 @pulumi.input_type
 class GetDatabaseVersionFilterArgs:
     def __init__(__self__, *,
                  key: str,
                  values: Sequence[str],
                  all: Optional[bool] = None,
```

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/_utilities.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/config/vars.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/database.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/dns_domain_name.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/dns_domain_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/dns_domain_record.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/firewall.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/firewall_rule.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_database.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_database.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_database_version.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_database_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_disk_image.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_disk_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_dns_domain_name.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_dns_domain_name.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_dns_domain_record.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_dns_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_firewall.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_instance.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_instances.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_instances.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_kubernetes_cluster.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_kubernetes_version.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_kubernetes_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_load_balancer.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_network.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_object_store.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_object_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_object_store_credential.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_object_store_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_region.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_reserved_ip.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_reserved_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_size.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_ssh_key.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/get_volume.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/get_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/instance.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/instance_reserved_ip_assignment.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/instance_reserved_ip_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/kubernetes_cluster.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/kubernetes_node_pool.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/kubernetes_node_pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,37 +15,41 @@
 class KubernetesNodePoolArgs:
     def __init__(__self__, *,
                  cluster_id: pulumi.Input[str],
                  region: pulumi.Input[str],
                  label: Optional[pulumi.Input[str]] = None,
                  node_count: Optional[pulumi.Input[int]] = None,
                  num_target_nodes: Optional[pulumi.Input[int]] = None,
+                 public_ip_node_pool: Optional[pulumi.Input[bool]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  target_nodes_size: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a KubernetesNodePool resource.
         :param pulumi.Input[str] cluster_id: The ID of your cluster
         :param pulumi.Input[str] region: The region of the node pool, has to match that of the cluster
         :param pulumi.Input[str] label: Node pool label, if you don't provide one, we will generate one for you
         :param pulumi.Input[int] node_count: the number of instances to create (optional, the default at the time of writing is 3)
         :param pulumi.Input[int] num_target_nodes: the number of instances to create (optional, the default at the time of writing is 3)
+        :param pulumi.Input[bool] public_ip_node_pool: Node pool belongs to the public ip node pool
         :param pulumi.Input[str] size: the size of each node (optional, the default is currently g4s.kube.medium)
         :param pulumi.Input[str] target_nodes_size: the size of each node (optional, the default is currently g4s.kube.medium)
         """
         pulumi.set(__self__, "cluster_id", cluster_id)
         pulumi.set(__self__, "region", region)
         if label is not None:
             pulumi.set(__self__, "label", label)
         if node_count is not None:
             pulumi.set(__self__, "node_count", node_count)
         if num_target_nodes is not None:
             warnings.warn("""This field is deprecated, please use `node_count` instead""", DeprecationWarning)
             pulumi.log.warn("""num_target_nodes is deprecated: This field is deprecated, please use `node_count` instead""")
         if num_target_nodes is not None:
             pulumi.set(__self__, "num_target_nodes", num_target_nodes)
+        if public_ip_node_pool is not None:
+            pulumi.set(__self__, "public_ip_node_pool", public_ip_node_pool)
         if size is not None:
             pulumi.set(__self__, "size", size)
         if target_nodes_size is not None:
             warnings.warn("""This field is deprecated, please use `size` instead""", DeprecationWarning)
             pulumi.log.warn("""target_nodes_size is deprecated: This field is deprecated, please use `size` instead""")
         if target_nodes_size is not None:
             pulumi.set(__self__, "target_nodes_size", target_nodes_size)
@@ -110,14 +114,26 @@
         return pulumi.get(self, "num_target_nodes")
 
     @num_target_nodes.setter
     def num_target_nodes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "num_target_nodes", value)
 
     @property
+    @pulumi.getter(name="publicIpNodePool")
+    def public_ip_node_pool(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Node pool belongs to the public ip node pool
+        """
+        return pulumi.get(self, "public_ip_node_pool")
+
+    @public_ip_node_pool.setter
+    def public_ip_node_pool(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "public_ip_node_pool", value)
+
+    @property
     @pulumi.getter
     def size(self) -> Optional[pulumi.Input[str]]:
         """
         the size of each node (optional, the default is currently g4s.kube.medium)
         """
         return pulumi.get(self, "size")
 
@@ -145,24 +161,26 @@
 class _KubernetesNodePoolState:
     def __init__(__self__, *,
                  cluster_id: Optional[pulumi.Input[str]] = None,
                  instance_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  node_count: Optional[pulumi.Input[int]] = None,
                  num_target_nodes: Optional[pulumi.Input[int]] = None,
+                 public_ip_node_pool: Optional[pulumi.Input[bool]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  target_nodes_size: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering KubernetesNodePool resources.
         :param pulumi.Input[str] cluster_id: The ID of your cluster
         :param pulumi.Input[Sequence[pulumi.Input[str]]] instance_names: Instance names in the nodepool
         :param pulumi.Input[str] label: Node pool label, if you don't provide one, we will generate one for you
         :param pulumi.Input[int] node_count: the number of instances to create (optional, the default at the time of writing is 3)
         :param pulumi.Input[int] num_target_nodes: the number of instances to create (optional, the default at the time of writing is 3)
+        :param pulumi.Input[bool] public_ip_node_pool: Node pool belongs to the public ip node pool
         :param pulumi.Input[str] region: The region of the node pool, has to match that of the cluster
         :param pulumi.Input[str] size: the size of each node (optional, the default is currently g4s.kube.medium)
         :param pulumi.Input[str] target_nodes_size: the size of each node (optional, the default is currently g4s.kube.medium)
         """
         if cluster_id is not None:
             pulumi.set(__self__, "cluster_id", cluster_id)
         if instance_names is not None:
@@ -172,14 +190,16 @@
         if node_count is not None:
             pulumi.set(__self__, "node_count", node_count)
         if num_target_nodes is not None:
             warnings.warn("""This field is deprecated, please use `node_count` instead""", DeprecationWarning)
             pulumi.log.warn("""num_target_nodes is deprecated: This field is deprecated, please use `node_count` instead""")
         if num_target_nodes is not None:
             pulumi.set(__self__, "num_target_nodes", num_target_nodes)
+        if public_ip_node_pool is not None:
+            pulumi.set(__self__, "public_ip_node_pool", public_ip_node_pool)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if size is not None:
             pulumi.set(__self__, "size", size)
         if target_nodes_size is not None:
             warnings.warn("""This field is deprecated, please use `size` instead""", DeprecationWarning)
             pulumi.log.warn("""target_nodes_size is deprecated: This field is deprecated, please use `size` instead""")
@@ -246,14 +266,26 @@
         return pulumi.get(self, "num_target_nodes")
 
     @num_target_nodes.setter
     def num_target_nodes(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "num_target_nodes", value)
 
     @property
+    @pulumi.getter(name="publicIpNodePool")
+    def public_ip_node_pool(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Node pool belongs to the public ip node pool
+        """
+        return pulumi.get(self, "public_ip_node_pool")
+
+    @public_ip_node_pool.setter
+    def public_ip_node_pool(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "public_ip_node_pool", value)
+
+    @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
         """
         The region of the node pool, has to match that of the cluster
         """
         return pulumi.get(self, "region")
 
@@ -294,14 +326,15 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cluster_id: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  node_count: Optional[pulumi.Input[int]] = None,
                  num_target_nodes: Optional[pulumi.Input[int]] = None,
+                 public_ip_node_pool: Optional[pulumi.Input[bool]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  target_nodes_size: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a Civo Kubernetes node pool resource. While the default node pool must be defined in the `KubernetesCluster` resource, this resource can be used to add additional ones to a cluster.
 
@@ -315,14 +348,15 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: The ID of your cluster
         :param pulumi.Input[str] label: Node pool label, if you don't provide one, we will generate one for you
         :param pulumi.Input[int] node_count: the number of instances to create (optional, the default at the time of writing is 3)
         :param pulumi.Input[int] num_target_nodes: the number of instances to create (optional, the default at the time of writing is 3)
+        :param pulumi.Input[bool] public_ip_node_pool: Node pool belongs to the public ip node pool
         :param pulumi.Input[str] region: The region of the node pool, has to match that of the cluster
         :param pulumi.Input[str] size: the size of each node (optional, the default is currently g4s.kube.medium)
         :param pulumi.Input[str] target_nodes_size: the size of each node (optional, the default is currently g4s.kube.medium)
         """
         ...
     @overload
     def __init__(__self__,
@@ -355,14 +389,15 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  cluster_id: Optional[pulumi.Input[str]] = None,
                  label: Optional[pulumi.Input[str]] = None,
                  node_count: Optional[pulumi.Input[int]] = None,
                  num_target_nodes: Optional[pulumi.Input[int]] = None,
+                 public_ip_node_pool: Optional[pulumi.Input[bool]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[str]] = None,
                  target_nodes_size: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
@@ -376,14 +411,15 @@
             __props__.__dict__["cluster_id"] = cluster_id
             __props__.__dict__["label"] = label
             __props__.__dict__["node_count"] = node_count
             if num_target_nodes is not None and not opts.urn:
                 warnings.warn("""This field is deprecated, please use `node_count` instead""", DeprecationWarning)
                 pulumi.log.warn("""num_target_nodes is deprecated: This field is deprecated, please use `node_count` instead""")
             __props__.__dict__["num_target_nodes"] = num_target_nodes
+            __props__.__dict__["public_ip_node_pool"] = public_ip_node_pool
             if region is None and not opts.urn:
                 raise TypeError("Missing required property 'region'")
             __props__.__dict__["region"] = region
             __props__.__dict__["size"] = size
             if target_nodes_size is not None and not opts.urn:
                 warnings.warn("""This field is deprecated, please use `size` instead""", DeprecationWarning)
                 pulumi.log.warn("""target_nodes_size is deprecated: This field is deprecated, please use `size` instead""")
@@ -400,14 +436,15 @@
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             cluster_id: Optional[pulumi.Input[str]] = None,
             instance_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             label: Optional[pulumi.Input[str]] = None,
             node_count: Optional[pulumi.Input[int]] = None,
             num_target_nodes: Optional[pulumi.Input[int]] = None,
+            public_ip_node_pool: Optional[pulumi.Input[bool]] = None,
             region: Optional[pulumi.Input[str]] = None,
             size: Optional[pulumi.Input[str]] = None,
             target_nodes_size: Optional[pulumi.Input[str]] = None) -> 'KubernetesNodePool':
         """
         Get an existing KubernetesNodePool resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
@@ -415,27 +452,29 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] cluster_id: The ID of your cluster
         :param pulumi.Input[Sequence[pulumi.Input[str]]] instance_names: Instance names in the nodepool
         :param pulumi.Input[str] label: Node pool label, if you don't provide one, we will generate one for you
         :param pulumi.Input[int] node_count: the number of instances to create (optional, the default at the time of writing is 3)
         :param pulumi.Input[int] num_target_nodes: the number of instances to create (optional, the default at the time of writing is 3)
+        :param pulumi.Input[bool] public_ip_node_pool: Node pool belongs to the public ip node pool
         :param pulumi.Input[str] region: The region of the node pool, has to match that of the cluster
         :param pulumi.Input[str] size: the size of each node (optional, the default is currently g4s.kube.medium)
         :param pulumi.Input[str] target_nodes_size: the size of each node (optional, the default is currently g4s.kube.medium)
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _KubernetesNodePoolState.__new__(_KubernetesNodePoolState)
 
         __props__.__dict__["cluster_id"] = cluster_id
         __props__.__dict__["instance_names"] = instance_names
         __props__.__dict__["label"] = label
         __props__.__dict__["node_count"] = node_count
         __props__.__dict__["num_target_nodes"] = num_target_nodes
+        __props__.__dict__["public_ip_node_pool"] = public_ip_node_pool
         __props__.__dict__["region"] = region
         __props__.__dict__["size"] = size
         __props__.__dict__["target_nodes_size"] = target_nodes_size
         return KubernetesNodePool(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="clusterId")
@@ -477,14 +516,22 @@
         """
         warnings.warn("""This field is deprecated, please use `node_count` instead""", DeprecationWarning)
         pulumi.log.warn("""num_target_nodes is deprecated: This field is deprecated, please use `node_count` instead""")
 
         return pulumi.get(self, "num_target_nodes")
 
     @property
+    @pulumi.getter(name="publicIpNodePool")
+    def public_ip_node_pool(self) -> pulumi.Output[bool]:
+        """
+        Node pool belongs to the public ip node pool
+        """
+        return pulumi.get(self, "public_ip_node_pool")
+
+    @property
     @pulumi.getter
     def region(self) -> pulumi.Output[str]:
         """
         The region of the node pool, has to match that of the cluster
         """
         return pulumi.get(self, "region")
```

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/network.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/object_store.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/object_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/object_store_credential.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/object_store_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/outputs.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,14 +267,16 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "nodeCount":
             suggest = "node_count"
         elif key == "instanceNames":
             suggest = "instance_names"
+        elif key == "publicIpNodePool":
+            suggest = "public_ip_node_pool"
 
         if suggest:
             pulumi.log.warn(f"Key '{key}' not found in KubernetesClusterPools. Access the value via the '{suggest}' property getter instead.")
 
     def __getitem__(self, key: str) -> Any:
         KubernetesClusterPools.__key_warning(key)
         return super().__getitem__(key)
@@ -283,27 +285,31 @@
         KubernetesClusterPools.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  node_count: int,
                  size: str,
                  instance_names: Optional[Sequence[str]] = None,
-                 label: Optional[str] = None):
+                 label: Optional[str] = None,
+                 public_ip_node_pool: Optional[bool] = None):
         """
         :param int node_count: Number of nodes in the nodepool
         :param str size: Size of the nodes in the nodepool
         :param Sequence[str] instance_names: Instance names in the nodepool
         :param str label: Node pool label, if you don't provide one, we will generate one for you
+        :param bool public_ip_node_pool: Node pool belongs to the public ip node pool
         """
         pulumi.set(__self__, "node_count", node_count)
         pulumi.set(__self__, "size", size)
         if instance_names is not None:
             pulumi.set(__self__, "instance_names", instance_names)
         if label is not None:
             pulumi.set(__self__, "label", label)
+        if public_ip_node_pool is not None:
+            pulumi.set(__self__, "public_ip_node_pool", public_ip_node_pool)
 
     @property
     @pulumi.getter(name="nodeCount")
     def node_count(self) -> int:
         """
         Number of nodes in the nodepool
         """
@@ -329,14 +335,22 @@
     @pulumi.getter
     def label(self) -> Optional[str]:
         """
         Node pool label, if you don't provide one, we will generate one for you
         """
         return pulumi.get(self, "label")
 
+    @property
+    @pulumi.getter(name="publicIpNodePool")
+    def public_ip_node_pool(self) -> Optional[bool]:
+        """
+        Node pool belongs to the public ip node pool
+        """
+        return pulumi.get(self, "public_ip_node_pool")
+
 
 @pulumi.output_type
 class GetDatabaseVersionFilterResult(dict):
     def __init__(__self__, *,
                  key: str,
                  values: Sequence[str],
                  all: Optional[bool] = None,
@@ -852,18 +866,20 @@
 
 @pulumi.output_type
 class GetKubernetesClusterPoolResult(dict):
     def __init__(__self__, *,
                  instance_names: Sequence[str],
                  label: str,
                  node_count: int,
+                 public_ip_node_pool: bool,
                  size: str):
         pulumi.set(__self__, "instance_names", instance_names)
         pulumi.set(__self__, "label", label)
         pulumi.set(__self__, "node_count", node_count)
+        pulumi.set(__self__, "public_ip_node_pool", public_ip_node_pool)
         pulumi.set(__self__, "size", size)
 
     @property
     @pulumi.getter(name="instanceNames")
     def instance_names(self) -> Sequence[str]:
         return pulumi.get(self, "instance_names")
 
@@ -874,14 +890,19 @@
 
     @property
     @pulumi.getter(name="nodeCount")
     def node_count(self) -> int:
         return pulumi.get(self, "node_count")
 
     @property
+    @pulumi.getter(name="publicIpNodePool")
+    def public_ip_node_pool(self) -> bool:
+        return pulumi.get(self, "public_ip_node_pool")
+
+    @property
     @pulumi.getter
     def size(self) -> str:
         return pulumi.get(self, "size")
 
 
 @pulumi.output_type
 class GetKubernetesVersionFilterResult(dict):
```

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/provider.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/reserved_ip.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/reserved_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/ssh_key.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/volume.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo/volume_attachment.py` & `pulumi_civo-2.4.0a1690301883/pulumi_civo/volume_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo.egg-info/PKG-INFO` & `pulumi_civo-2.4.0a1690301883/pulumi_civo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-civo
-Version: 2.4.0a1690262333
+Version: 2.4.0a1690301883
 Summary: A Pulumi package for creating and managing Civo cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-civo
 Keywords: pulumi civo
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_civo-2.4.0a1690262333/pulumi_civo.egg-info/SOURCES.txt` & `pulumi_civo-2.4.0a1690301883/pulumi_civo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_civo-2.4.0a1690262333/setup.py` & `pulumi_civo-2.4.0a1690301883/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.4.0a1690262333"
-PLUGIN_VERSION = "2.4.0-alpha.1690262333+fdb816d6"
+VERSION = "2.4.0a1690301883"
+PLUGIN_VERSION = "2.4.0-alpha.1690301883+7a0d1a48"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'civo', PLUGIN_VERSION])
         except OSError as error:
```

