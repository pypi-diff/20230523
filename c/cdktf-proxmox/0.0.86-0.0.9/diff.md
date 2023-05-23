# Comparing `tmp/cdktf-proxmox-0.0.86.tar.gz` & `tmp/cdktf-proxmox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-proxmox-0.0.86.tar", last modified: Tue May 23 00:30:21 2023, max compression
+gzip compressed data, was "cdktf-proxmox-0.0.9.tar", last modified: Fri Mar 10 04:16:02 2023, max compression
```

## Comparing `cdktf-proxmox-0.0.86.tar` & `cdktf-proxmox-0.0.9.tar`

### file list

```diff
@@ -1,81 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.552355 cdktf-proxmox-0.0.86/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-23 00:30:21.552355 cdktf-proxmox-0.0.86/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 00:30:21.552355 cdktf-proxmox-0.0.86/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.536355 cdktf-proxmox-0.0.86/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.540355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.544355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   472465 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/_jsii/cdktf-proxmox@0.0.86.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.544355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_lvm_storage_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    40294 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_lvm_storage_classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.544355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_lvm_thinpool_storage_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    41352 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_lvm_thinpool_storage_classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.544355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_lvm_thinpools/
--rw-r--r--   0 runner    (1001) docker     (123)    40164 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_lvm_thinpools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.544355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_lvms/
--rw-r--r--   0 runner    (1001) docker     (123)    38851 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_lvms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.544355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_network_bonds/
--rw-r--r--   0 runner    (1001) docker     (123)    53915 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_network_bonds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.544355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_network_bridges/
--rw-r--r--   0 runner    (1001) docker     (123)    55637 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_network_bridges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.544355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_nfs_storage_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    40607 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_nfs_storage_classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.544355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_node_storage_lvm_thinpools/
--rw-r--r--   0 runner    (1001) docker     (123)    41455 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_node_storage_lvm_thinpools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.544355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_node_storage_lvms/
--rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_node_storage_lvms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.544355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_node_storage_nfs/
--rw-r--r--   0 runner    (1001) docker     (123)    40594 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_node_storage_nfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.544355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_node_storage_zfs/
--rw-r--r--   0 runner    (1001) docker     (123)    40422 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_node_storage_zfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.548354 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)    49186 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.548354 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_resource_pools/
--rw-r--r--   0 runner    (1001) docker     (123)    48933 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_resource_pools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.548354 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_template/
--rw-r--r--   0 runner    (1001) docker     (123)    95525 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.548354 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_templates/
--rw-r--r--   0 runner    (1001) docker     (123)   117070 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.548354 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_virtual_machines/
--rw-r--r--   0 runner    (1001) docker     (123)   120407 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_virtual_machines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.548354 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_zfs_pools/
--rw-r--r--   0 runner    (1001) docker     (123)    39686 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_zfs_pools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.548354 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_zfs_storage_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    40435 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_zfs_storage_classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.548354 cdktf-proxmox-0.0.86/src/cdktf_proxmox/lvm/
--rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/lvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.548354 cdktf-proxmox-0.0.86/src/cdktf_proxmox/lvm_storage_class/
--rw-r--r--   0 runner    (1001) docker     (123)    22542 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/lvm_storage_class/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.548354 cdktf-proxmox-0.0.86/src/cdktf_proxmox/lvm_thinpool/
--rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/lvm_thinpool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.548354 cdktf-proxmox-0.0.86/src/cdktf_proxmox/lvm_thinpool_storage_class/
--rw-r--r--   0 runner    (1001) docker     (123)    25096 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/lvm_thinpool_storage_class/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.548354 cdktf-proxmox-0.0.86/src/cdktf_proxmox/network_bond/
--rw-r--r--   0 runner    (1001) docker     (123)    56269 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/network_bond/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.548354 cdktf-proxmox-0.0.86/src/cdktf_proxmox/network_bridge/
--rw-r--r--   0 runner    (1001) docker     (123)    52889 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/network_bridge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.552355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/nfs_storage_class/
--rw-r--r--   0 runner    (1001) docker     (123)    24594 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/nfs_storage_class/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.552355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.552355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/resource_pool/
--rw-r--r--   0 runner    (1001) docker     (123)    34782 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/resource_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.552355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/virtual_machine/
--rw-r--r--   0 runner    (1001) docker     (123)   413855 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/virtual_machine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.552355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/zfs_pool/
--rw-r--r--   0 runner    (1001) docker     (123)    20911 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/zfs_pool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.552355 cdktf-proxmox-0.0.86/src/cdktf_proxmox/zfs_storage_class/
--rw-r--r--   0 runner    (1001) docker     (123)    22435 2023-05-23 00:30:03.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox/zfs_storage_class/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 00:30:21.540355 cdktf-proxmox-0.0.86/src/cdktf_proxmox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-23 00:30:21.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-23 00:30:21.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 00:30:21.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-23 00:30:21.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 00:30:21.000000 cdktf-proxmox-0.0.86/src/cdktf_proxmox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.336244 cdktf-proxmox-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-03-10 04:16:02.336244 cdktf-proxmox-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-10 04:16:02.336244 cdktf-proxmox-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.324244 cdktf-proxmox-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.328244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.328244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   441553 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/_jsii/cdktf-proxmox@0.0.9.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.328244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_lvm_storage_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    40294 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_lvm_storage_classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.328244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_lvm_thinpool_storage_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    41352 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_lvm_thinpool_storage_classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.328244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_lvm_thinpools/
+-rw-r--r--   0 runner    (1001) docker     (123)    40164 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_lvm_thinpools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.328244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_lvms/
+-rw-r--r--   0 runner    (1001) docker     (123)    38851 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_lvms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.328244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_network_bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)    53915 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_network_bonds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.328244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_network_bridges/
+-rw-r--r--   0 runner    (1001) docker     (123)    55637 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_network_bridges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.328244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_nfs_storage_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    40607 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_nfs_storage_classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.328244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_node_storage_lvm_thinpools/
+-rw-r--r--   0 runner    (1001) docker     (123)    41455 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_node_storage_lvm_thinpools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.328244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_node_storage_lvms/
+-rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_node_storage_lvms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_node_storage_nfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    40594 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_node_storage_nfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_node_storage_zfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    40422 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_node_storage_zfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)    49186 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_resource_pools/
+-rw-r--r--   0 runner    (1001) docker     (123)    48933 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_resource_pools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)   116910 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_virtual_machines/
+-rw-r--r--   0 runner    (1001) docker     (123)   120247 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_virtual_machines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_zfs_pools/
+-rw-r--r--   0 runner    (1001) docker     (123)    39686 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_zfs_pools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_zfs_storage_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    40435 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_zfs_storage_classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/lvm/
+-rw-r--r--   0 runner    (1001) docker     (123)    18285 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/lvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/lvm_storage_class/
+-rw-r--r--   0 runner    (1001) docker     (123)    22542 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/lvm_storage_class/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/lvm_thinpool/
+-rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/lvm_thinpool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/lvm_thinpool_storage_class/
+-rw-r--r--   0 runner    (1001) docker     (123)    25096 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/lvm_thinpool_storage_class/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/network_bond/
+-rw-r--r--   0 runner    (1001) docker     (123)    56269 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/network_bond/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/network_bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)    52889 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/network_bridge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/nfs_storage_class/
+-rw-r--r--   0 runner    (1001) docker     (123)    24594 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/nfs_storage_class/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    17553 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/resource_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)    34782 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/resource_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/virtual_machine/
+-rw-r--r--   0 runner    (1001) docker     (123)   413535 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/virtual_machine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.332244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/zfs_pool/
+-rw-r--r--   0 runner    (1001) docker     (123)    20911 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/zfs_pool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.336244 cdktf-proxmox-0.0.9/src/cdktf_proxmox/zfs_storage_class/
+-rw-r--r--   0 runner    (1001) docker     (123)    22435 2023-03-10 04:15:49.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox/zfs_storage_class/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 04:16:02.328244 cdktf-proxmox-0.0.9/src/cdktf_proxmox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-03-10 04:16:02.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-03-10 04:16:02.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 04:16:02.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-10 04:16:02.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-10 04:16:02.000000 cdktf-proxmox-0.0.9/src/cdktf_proxmox.egg-info/top_level.txt
```

### Comparing `cdktf-proxmox-0.0.86/LICENSE` & `cdktf-proxmox-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/PKG-INFO` & `cdktf-proxmox-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-proxmox
-Version: 0.0.86
+Version: 0.0.9
 Summary: A package that vends generated constructs from the Proxmox Terraform provider
 Home-page: https://github.com/awlsring/cdktf-proxmox.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-proxmox.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-proxmox-0.0.86/README.md` & `cdktf-proxmox-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/setup.py` & `cdktf-proxmox-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-proxmox",
-    "version": "0.0.86",
+    "version": "0.0.9",
     "description": "A package that vends generated constructs from the Proxmox Terraform provider",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdktf-proxmox.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -32,15 +32,14 @@
         "cdktf_proxmox.data_proxmox_nfs_storage_classes",
         "cdktf_proxmox.data_proxmox_node_storage_lvm_thinpools",
         "cdktf_proxmox.data_proxmox_node_storage_lvms",
         "cdktf_proxmox.data_proxmox_node_storage_nfs",
         "cdktf_proxmox.data_proxmox_node_storage_zfs",
         "cdktf_proxmox.data_proxmox_nodes",
         "cdktf_proxmox.data_proxmox_resource_pools",
-        "cdktf_proxmox.data_proxmox_template",
         "cdktf_proxmox.data_proxmox_templates",
         "cdktf_proxmox.data_proxmox_virtual_machines",
         "cdktf_proxmox.data_proxmox_zfs_pools",
         "cdktf_proxmox.data_proxmox_zfs_storage_classes",
         "cdktf_proxmox.lvm",
         "cdktf_proxmox.lvm_storage_class",
         "cdktf_proxmox.lvm_thinpool",
@@ -52,25 +51,25 @@
         "cdktf_proxmox.resource_pool",
         "cdktf_proxmox.virtual_machine",
         "cdktf_proxmox.zfs_pool",
         "cdktf_proxmox.zfs_storage_class"
     ],
     "package_data": {
         "cdktf_proxmox._jsii": [
-            "cdktf-proxmox@0.0.86.jsii.tgz"
+            "cdktf-proxmox@0.0.9.jsii.tgz"
         ],
         "cdktf_proxmox": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdktf>=0.14.3, <0.15.0",
         "constructs>=10.1.52, <11.0.0",
-        "jsii>=1.82.0, <2.0.0",
+        "jsii>=1.77.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_lvm_storage_classes/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_lvm_storage_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_lvm_thinpool_storage_classes/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_lvm_thinpool_storage_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_lvm_thinpools/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_lvm_thinpools/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_lvms/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_lvms/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_network_bonds/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_network_bonds/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_network_bridges/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_network_bridges/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_nfs_storage_classes/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_nfs_storage_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_node_storage_lvm_thinpools/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_node_storage_lvm_thinpools/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_node_storage_lvms/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_node_storage_lvms/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_node_storage_nfs/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_node_storage_nfs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_node_storage_zfs/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_node_storage_zfs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_nodes/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_resource_pools/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_resource_pools/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_template/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_templates/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `data_proxmox_template`
+# `data_proxmox_templates`
 
-Refer to the Terraform Registory for docs: [`data_proxmox_template`](https://www.terraform.io/docs/providers/proxmox/d/template).
+Refer to the Terraform Registory for docs: [`data_proxmox_templates`](https://www.terraform.io/docs/providers/proxmox/d/templates).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,257 +17,541 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class DataProxmoxTemplate(
+class DataProxmoxTemplates(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplate",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplates",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/proxmox/d/template proxmox_template}.'''
+    '''Represents a {@link https://www.terraform.io/docs/providers/proxmox/d/templates proxmox_templates}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        id_: builtins.str,
+        id: builtins.str,
         *,
-        node_attribute: builtins.str,
-        id: typing.Optional[jsii.Number] = None,
-        name: typing.Optional[builtins.str] = None,
+        filters: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataProxmoxTemplatesFilters", typing.Dict[builtins.str, typing.Any]]]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[jsii.Number] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/proxmox/d/template proxmox_template} Data Source.
+        '''Create a new {@link https://www.terraform.io/docs/providers/proxmox/d/templates proxmox_templates} Data Source.
 
         :param scope: The scope in which to define this construct.
-        :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param node_attribute: The node to create the template on. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/template#node DataProxmoxTemplate#node}
-        :param id: The identifier of the template. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/template#id DataProxmoxTemplate#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: The name of the template. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/template#name DataProxmoxTemplate#name}
+        :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
+        :param filters: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/templates#filters DataProxmoxTemplates#filters}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e4ef2cd22cf433a6e1971b184320047824643e5aace46960ef74bf9cbf53982a)
+            type_hints = typing.get_type_hints(_typecheckingstub__9c8f43a8ed4d9862bb2dfda7c754989b1621c88e999f35c8aa0300d8f6ba0675)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
-            check_type(argname="argument id_", value=id_, expected_type=type_hints["id_"])
-        config = DataProxmoxTemplateConfig(
-            node_attribute=node_attribute,
-            id=id,
-            name=name,
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        config = DataProxmoxTemplatesConfig(
+            filters=filters,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
             provisioners=provisioners,
         )
 
-        jsii.create(self.__class__, self, [scope, id_, config])
+        jsii.create(self.__class__, self, [scope, id, config])
 
-    @jsii.member(jsii_name="resetId")
-    def reset_id(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetId", []))
-
-    @jsii.member(jsii_name="resetName")
-    def reset_name(self) -> None:
-        return typing.cast(None, jsii.invoke(self, "resetName", []))
+    @jsii.member(jsii_name="putFilters")
+    def put_filters(
+        self,
+        value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataProxmoxTemplatesFilters", typing.Dict[builtins.str, typing.Any]]]],
+    ) -> None:
+        '''
+        :param value: -
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__233a1989690e82037c4c9dc0c040be824ca0bc7ab5562170fe8918e4876b29f9)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        return typing.cast(None, jsii.invoke(self, "putFilters", [value]))
+
+    @jsii.member(jsii_name="resetFilters")
+    def reset_filters(self) -> None:
+        return typing.cast(None, jsii.invoke(self, "resetFilters", []))
 
     @jsii.member(jsii_name="synthesizeAttributes")
     def _synthesize_attributes(self) -> typing.Mapping[builtins.str, typing.Any]:
         return typing.cast(typing.Mapping[builtins.str, typing.Any], jsii.invoke(self, "synthesizeAttributes", []))
 
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
-    @jsii.member(jsii_name="agent")
-    def agent(self) -> "DataProxmoxTemplateAgentOutputReference":
-        return typing.cast("DataProxmoxTemplateAgentOutputReference", jsii.get(self, "agent"))
+    @jsii.member(jsii_name="filters")
+    def filters(self) -> "DataProxmoxTemplatesFiltersList":
+        return typing.cast("DataProxmoxTemplatesFiltersList", jsii.get(self, "filters"))
 
     @builtins.property
-    @jsii.member(jsii_name="bios")
-    def bios(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "bios"))
+    @jsii.member(jsii_name="templates")
+    def templates(self) -> "DataProxmoxTemplatesTemplatesList":
+        return typing.cast("DataProxmoxTemplatesTemplatesList", jsii.get(self, "templates"))
 
     @builtins.property
-    @jsii.member(jsii_name="cloudInit")
-    def cloud_init(self) -> "DataProxmoxTemplateCloudInitOutputReference":
-        return typing.cast("DataProxmoxTemplateCloudInitOutputReference", jsii.get(self, "cloudInit"))
+    @jsii.member(jsii_name="filtersInput")
+    def filters_input(
+        self,
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataProxmoxTemplatesFilters"]]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataProxmoxTemplatesFilters"]]], jsii.get(self, "filtersInput"))
+
+
+@jsii.data_type(
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesConfig",
+    jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
+    name_mapping={
+        "connection": "connection",
+        "count": "count",
+        "depends_on": "dependsOn",
+        "for_each": "forEach",
+        "lifecycle": "lifecycle",
+        "provider": "provider",
+        "provisioners": "provisioners",
+        "filters": "filters",
+    },
+)
+class DataProxmoxTemplatesConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+    def __init__(
+        self,
+        *,
+        connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
+        count: typing.Optional[jsii.Number] = None,
+        depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
+        for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
+        lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
+        provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
+        provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
+        filters: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataProxmoxTemplatesFilters", typing.Dict[builtins.str, typing.Any]]]]] = None,
+    ) -> None:
+        '''
+        :param connection: 
+        :param count: 
+        :param depends_on: 
+        :param for_each: 
+        :param lifecycle: 
+        :param provider: 
+        :param provisioners: 
+        :param filters: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/templates#filters DataProxmoxTemplates#filters}.
+        '''
+        if isinstance(lifecycle, dict):
+            lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__4b9b87d43a9822a28f232fcb57074d7978bca6aa140657b9397ad2bf3cabac68)
+            check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
+            check_type(argname="argument count", value=count, expected_type=type_hints["count"])
+            check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
+            check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
+            check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
+            check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
+            check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
+            check_type(argname="argument filters", value=filters, expected_type=type_hints["filters"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if connection is not None:
+            self._values["connection"] = connection
+        if count is not None:
+            self._values["count"] = count
+        if depends_on is not None:
+            self._values["depends_on"] = depends_on
+        if for_each is not None:
+            self._values["for_each"] = for_each
+        if lifecycle is not None:
+            self._values["lifecycle"] = lifecycle
+        if provider is not None:
+            self._values["provider"] = provider
+        if provisioners is not None:
+            self._values["provisioners"] = provisioners
+        if filters is not None:
+            self._values["filters"] = filters
 
     @builtins.property
-    @jsii.member(jsii_name="cpu")
-    def cpu(self) -> "DataProxmoxTemplateCpuOutputReference":
-        return typing.cast("DataProxmoxTemplateCpuOutputReference", jsii.get(self, "cpu"))
+    def connection(
+        self,
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("connection")
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
 
     @builtins.property
-    @jsii.member(jsii_name="description")
-    def description(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "description"))
+    def count(self) -> typing.Optional[jsii.Number]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("count")
+        return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    @jsii.member(jsii_name="disks")
-    def disks(self) -> "DataProxmoxTemplateDisksList":
-        return typing.cast("DataProxmoxTemplateDisksList", jsii.get(self, "disks"))
+    def depends_on(
+        self,
+    ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("depends_on")
+        return typing.cast(typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]], result)
 
     @builtins.property
-    @jsii.member(jsii_name="keyboardLayout")
-    def keyboard_layout(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "keyboardLayout"))
+    def for_each(self) -> typing.Optional[_cdktf_9a9027ec.ITerraformIterator]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("for_each")
+        return typing.cast(typing.Optional[_cdktf_9a9027ec.ITerraformIterator], result)
 
     @builtins.property
-    @jsii.member(jsii_name="kvmArguments")
-    def kvm_arguments(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "kvmArguments"))
+    def lifecycle(self) -> typing.Optional[_cdktf_9a9027ec.TerraformResourceLifecycle]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("lifecycle")
+        return typing.cast(typing.Optional[_cdktf_9a9027ec.TerraformResourceLifecycle], result)
 
     @builtins.property
-    @jsii.member(jsii_name="machineType")
-    def machine_type(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "machineType"))
+    def provider(self) -> typing.Optional[_cdktf_9a9027ec.TerraformProvider]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("provider")
+        return typing.cast(typing.Optional[_cdktf_9a9027ec.TerraformProvider], result)
 
     @builtins.property
-    @jsii.member(jsii_name="memory")
-    def memory(self) -> "DataProxmoxTemplateMemoryOutputReference":
-        return typing.cast("DataProxmoxTemplateMemoryOutputReference", jsii.get(self, "memory"))
+    def provisioners(
+        self,
+    ) -> typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("provisioners")
+        return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
-    @jsii.member(jsii_name="networkInterfaces")
-    def network_interfaces(self) -> "DataProxmoxTemplateNetworkInterfacesList":
-        return typing.cast("DataProxmoxTemplateNetworkInterfacesList", jsii.get(self, "networkInterfaces"))
+    def filters(
+        self,
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataProxmoxTemplatesFilters"]]]:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/templates#filters DataProxmoxTemplates#filters}.'''
+        result = self._values.get("filters")
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataProxmoxTemplatesFilters"]]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "DataProxmoxTemplatesConfig(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesFilters",
+    jsii_struct_bases=[],
+    name_mapping={"name": "name", "values": "values"},
+)
+class DataProxmoxTemplatesFilters:
+    def __init__(
+        self,
+        *,
+        name: builtins.str,
+        values: typing.Sequence[builtins.str],
+    ) -> None:
+        '''
+        :param name: The name of the attribute to filter on. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/templates#name DataProxmoxTemplates#name}
+        :param values: The value(s) to be used in the filter. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/templates#values DataProxmoxTemplates#values}
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__7b5a2e2e69a8b272223cae04497ef0e50f1388bd002ce5d48b07318623fc0fd0)
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument values", value=values, expected_type=type_hints["values"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "name": name,
+            "values": values,
+        }
 
     @builtins.property
-    @jsii.member(jsii_name="pciDevices")
-    def pci_devices(self) -> "DataProxmoxTemplatePciDevicesList":
-        return typing.cast("DataProxmoxTemplatePciDevicesList", jsii.get(self, "pciDevices"))
+    def name(self) -> builtins.str:
+        '''The name of the attribute to filter on.
+
+        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/templates#name DataProxmoxTemplates#name}
+        '''
+        result = self._values.get("name")
+        assert result is not None, "Required property 'name' is missing"
+        return typing.cast(builtins.str, result)
 
     @builtins.property
-    @jsii.member(jsii_name="resourcePool")
-    def resource_pool(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "resourcePool"))
+    def values(self) -> typing.List[builtins.str]:
+        '''The value(s) to be used in the filter.
+
+        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/templates#values DataProxmoxTemplates#values}
+        '''
+        result = self._values.get("values")
+        assert result is not None, "Required property 'values' is missing"
+        return typing.cast(typing.List[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "DataProxmoxTemplatesFilters(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+class DataProxmoxTemplatesFiltersList(
+    _cdktf_9a9027ec.ComplexList,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesFiltersList",
+):
+    def __init__(
+        self,
+        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+        terraform_attribute: builtins.str,
+        wraps_set: builtins.bool,
+    ) -> None:
+        '''
+        :param terraform_resource: The parent resource.
+        :param terraform_attribute: The attribute on the parent resource this class is referencing.
+        :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__7185592ee5df14f6502caf1b02c1c8f7f1a998c262a921b4059ae73ed17d01f7)
+            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
+            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
+            check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
+        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
+
+    @jsii.member(jsii_name="get")
+    def get(self, index: jsii.Number) -> "DataProxmoxTemplatesFiltersOutputReference":
+        '''
+        :param index: the index of the item to return.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b3e0e2fef1c0a4b8e2a1b64ae525d2b0ac767a60597d7eb6476cf5a4b328eb58)
+            check_type(argname="argument index", value=index, expected_type=type_hints["index"])
+        return typing.cast("DataProxmoxTemplatesFiltersOutputReference", jsii.invoke(self, "get", [index]))
 
     @builtins.property
-    @jsii.member(jsii_name="startOnNodeBoot")
-    def start_on_node_boot(self) -> _cdktf_9a9027ec.IResolvable:
-        return typing.cast(_cdktf_9a9027ec.IResolvable, jsii.get(self, "startOnNodeBoot"))
+    @jsii.member(jsii_name="terraformAttribute")
+    def _terraform_attribute(self) -> builtins.str:
+        '''The attribute on the parent resource this class is referencing.'''
+        return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
+
+    @_terraform_attribute.setter
+    def _terraform_attribute(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__12203107c9a9b5812061df83af59f971166e12e0dd3c53822898b587c4a13a1a)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "terraformAttribute", value)
 
     @builtins.property
-    @jsii.member(jsii_name="tags")
-    def tags(self) -> typing.List[builtins.str]:
-        return typing.cast(typing.List[builtins.str], jsii.get(self, "tags"))
+    @jsii.member(jsii_name="terraformResource")
+    def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
+        '''The parent resource.'''
+        return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
+
+    @_terraform_resource.setter
+    def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__7c18c8f27f5b5749f0930032ce59cf9aa9dd8c3fe11454a21edfacfb39110484)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "terraformResource", value)
 
     @builtins.property
-    @jsii.member(jsii_name="type")
-    def type(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "type"))
+    @jsii.member(jsii_name="wrapsSet")
+    def _wraps_set(self) -> builtins.bool:
+        '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
+        return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
+
+    @_wraps_set.setter
+    def _wraps_set(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__1de467d3e8e92a1d8d17a81042c85e45ddb8a5f8a574026c01b38410619c435e)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "wrapsSet", value)
 
     @builtins.property
-    @jsii.member(jsii_name="idInput")
-    def id_input(self) -> typing.Optional[jsii.Number]:
-        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "idInput"))
+    @jsii.member(jsii_name="internalValue")
+    def internal_value(
+        self,
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataProxmoxTemplatesFilters]]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataProxmoxTemplatesFilters]]], jsii.get(self, "internalValue"))
+
+    @internal_value.setter
+    def internal_value(
+        self,
+        value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataProxmoxTemplatesFilters]]],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__4eeb8042fe9f97bb3b08f79bdd3f5544c61ad333e13f34069ee25b3925b85f8c)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "internalValue", value)
+
+
+class DataProxmoxTemplatesFiltersOutputReference(
+    _cdktf_9a9027ec.ComplexObject,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesFiltersOutputReference",
+):
+    def __init__(
+        self,
+        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+        terraform_attribute: builtins.str,
+        complex_object_index: jsii.Number,
+        complex_object_is_from_set: builtins.bool,
+    ) -> None:
+        '''
+        :param terraform_resource: The parent resource.
+        :param terraform_attribute: The attribute on the parent resource this class is referencing.
+        :param complex_object_index: the index of this item in the list.
+        :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8327cf5bac96b9877733ed3b92c5e728be3a17f989a4bdbaf2900a291c81f07d)
+            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
+            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
+            check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
+            check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
+        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
     @jsii.member(jsii_name="nameInput")
     def name_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nameInput"))
 
     @builtins.property
-    @jsii.member(jsii_name="nodeAttributeInput")
-    def node_attribute_input(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "nodeAttributeInput"))
-
-    @builtins.property
-    @jsii.member(jsii_name="id")
-    def id(self) -> jsii.Number:
-        return typing.cast(jsii.Number, jsii.get(self, "id"))
-
-    @id.setter
-    def id(self, value: jsii.Number) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a4eeeeba3c39a0f8fd661594829813f3b5a08a9acc56fe1852ca4f52acbb54e1)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "id", value)
+    @jsii.member(jsii_name="valuesInput")
+    def values_input(self) -> typing.Optional[typing.List[builtins.str]]:
+        return typing.cast(typing.Optional[typing.List[builtins.str]], jsii.get(self, "valuesInput"))
 
     @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2ceebbba99c0db4bd5489cb0e441408679e0230c816b563d9bfed0277fb7d9c8)
+            type_hints = typing.get_type_hints(_typecheckingstub__16f3ef7637865b9efbe01d5d61b463f735bae38264ad57354abdbce513208aef)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
     @builtins.property
-    @jsii.member(jsii_name="nodeAttribute")
-    def node_attribute(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "nodeAttribute"))
+    @jsii.member(jsii_name="values")
+    def values(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "values"))
+
+    @values.setter
+    def values(self, value: typing.List[builtins.str]) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8a7dc4004f107546dc9c621fa798620b5001c0fd8917d4c9140a0ad48064ed70)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "values", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="internalValue")
+    def internal_value(
+        self,
+    ) -> typing.Optional[typing.Union[DataProxmoxTemplatesFilters, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[DataProxmoxTemplatesFilters, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
 
-    @node_attribute.setter
-    def node_attribute(self, value: builtins.str) -> None:
+    @internal_value.setter
+    def internal_value(
+        self,
+        value: typing.Optional[typing.Union[DataProxmoxTemplatesFilters, _cdktf_9a9027ec.IResolvable]],
+    ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__cb31b96735bf37ac81d559ab0ce9a0af448e344b0dbcaa737213f4ce4ddaf6c3)
+            type_hints = typing.get_type_hints(_typecheckingstub__dec6db530ef281b602f64ed73e330e24906e6e0c6b954683c5ba96b7ad21dcbf)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "nodeAttribute", value)
+        jsii.set(self, "internalValue", value)
+
+
+@jsii.data_type(
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplates",
+    jsii_struct_bases=[],
+    name_mapping={},
+)
+class DataProxmoxTemplatesTemplates:
+    def __init__(self) -> None:
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "DataProxmoxTemplatesTemplates(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateAgent",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesAgent",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplateAgent:
+class DataProxmoxTemplatesTemplatesAgent:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplateAgent(%s)" % ", ".join(
+        return "DataProxmoxTemplatesTemplatesAgent(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplateAgentOutputReference(
+class DataProxmoxTemplatesTemplatesAgentOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateAgentOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesAgentOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1bb6e3882eca230c304fbf04eb486d51f93c5b3cec722cf92e5d311e526f7c11)
+            type_hints = typing.get_type_hints(_typecheckingstub__673e66db611a5fbc4e59ce825f6e4416fa82cbf66904ba65202f13a93beb37d2)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="enabled")
     def enabled(self) -> _cdktf_9a9027ec.IResolvable:
@@ -281,83 +565,86 @@
     @builtins.property
     @jsii.member(jsii_name="useFstrim")
     def use_fstrim(self) -> _cdktf_9a9027ec.IResolvable:
         return typing.cast(_cdktf_9a9027ec.IResolvable, jsii.get(self, "useFstrim"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplateAgent]:
-        return typing.cast(typing.Optional[DataProxmoxTemplateAgent], jsii.get(self, "internalValue"))
+    def internal_value(self) -> typing.Optional[DataProxmoxTemplatesTemplatesAgent]:
+        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesAgent], jsii.get(self, "internalValue"))
 
     @internal_value.setter
-    def internal_value(self, value: typing.Optional[DataProxmoxTemplateAgent]) -> None:
+    def internal_value(
+        self,
+        value: typing.Optional[DataProxmoxTemplatesTemplatesAgent],
+    ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b6bb09a4e0bd03a04ee862ea7232014b12fe4ae50859f376a3d90f318942f2c5)
+            type_hints = typing.get_type_hints(_typecheckingstub__11571a58fd163ae522f420d6c0dff17873e68251c637a1ebc2f4261d40a0908e)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCloudInit",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInit",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplateCloudInit:
+class DataProxmoxTemplatesTemplatesCloudInit:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplateCloudInit(%s)" % ", ".join(
+        return "DataProxmoxTemplatesTemplatesCloudInit(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCloudInitDns",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitDns",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplateCloudInitDns:
+class DataProxmoxTemplatesTemplatesCloudInitDns:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplateCloudInitDns(%s)" % ", ".join(
+        return "DataProxmoxTemplatesTemplatesCloudInitDns(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplateCloudInitDnsOutputReference(
+class DataProxmoxTemplatesTemplatesCloudInitDnsOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCloudInitDnsOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitDnsOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b85bfac621b455ab5a57c0b8c4693493aac54564221c9c9a9519403ea8e69700)
+            type_hints = typing.get_type_hints(_typecheckingstub__e067c9db4e634da658b56ee80ca7edfde446f1a440b47d1f6eb546e326a67b26)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="domain")
     def domain(self) -> builtins.str:
@@ -366,129 +653,131 @@
     @builtins.property
     @jsii.member(jsii_name="nameserver")
     def nameserver(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "nameserver"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplateCloudInitDns]:
-        return typing.cast(typing.Optional[DataProxmoxTemplateCloudInitDns], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataProxmoxTemplatesTemplatesCloudInitDns]:
+        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesCloudInitDns], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplateCloudInitDns],
+        value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitDns],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ad3a996ef8508c2e45f8c89cbe97b055c8049b37dfc00c7c621d91ecb1658772)
+            type_hints = typing.get_type_hints(_typecheckingstub__0782611e20910ed665dc0d5e84a3f71452ba5bade5ae664490668cd11d64b023)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCloudInitIp",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitIp",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplateCloudInitIp:
+class DataProxmoxTemplatesTemplatesCloudInitIp:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplateCloudInitIp(%s)" % ", ".join(
+        return "DataProxmoxTemplatesTemplatesCloudInitIp(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplateCloudInitIpList(
+class DataProxmoxTemplatesTemplatesCloudInitIpList(
     _cdktf_9a9027ec.ComplexList,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCloudInitIpList",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitIpList",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         wraps_set: builtins.bool,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4a7c2c37c375e4ab986f9089b062a7e192800caf657d5ec277feea581473b4d0)
+            type_hints = typing.get_type_hints(_typecheckingstub__99f203b02f9592f1a1fb7a64a5635c720b9dd6c7f992bc56e8edb0bab0e63ae7)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
 
     @jsii.member(jsii_name="get")
     def get(
         self,
         index: jsii.Number,
-    ) -> "DataProxmoxTemplateCloudInitIpOutputReference":
+    ) -> "DataProxmoxTemplatesTemplatesCloudInitIpOutputReference":
         '''
         :param index: the index of the item to return.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3e009569d142ff7aba80375d28185467544bd3f2873a65544d9839015570431d)
+            type_hints = typing.get_type_hints(_typecheckingstub__17abca3a5e9277181468d701c2550bed8e6e1d101cde67b7c64c5bf22a976a80)
             check_type(argname="argument index", value=index, expected_type=type_hints["index"])
-        return typing.cast("DataProxmoxTemplateCloudInitIpOutputReference", jsii.invoke(self, "get", [index]))
+        return typing.cast("DataProxmoxTemplatesTemplatesCloudInitIpOutputReference", jsii.invoke(self, "get", [index]))
 
     @builtins.property
     @jsii.member(jsii_name="terraformAttribute")
     def _terraform_attribute(self) -> builtins.str:
         '''The attribute on the parent resource this class is referencing.'''
         return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
 
     @_terraform_attribute.setter
     def _terraform_attribute(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6fb11e8926625e3516c5ba5e7e6c66632c96345b59c27a2a58b803fe0c08c28d)
+            type_hints = typing.get_type_hints(_typecheckingstub__8f5acfd27a377920da103fd958e5f6b4dbf0ed9b81ad89a5f0293c850734683d)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformAttribute", value)
 
     @builtins.property
     @jsii.member(jsii_name="terraformResource")
     def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
         '''The parent resource.'''
         return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
 
     @_terraform_resource.setter
     def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2bb8b6c66ae22b277647f9c432e158f1b082f79d274ca0d23fb83aea02ee6a1c)
+            type_hints = typing.get_type_hints(_typecheckingstub__4ab6c78fc6f14f4f992d620cd01deffae673cfc19cb90a2b3a92306efc35ecdc)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformResource", value)
 
     @builtins.property
     @jsii.member(jsii_name="wrapsSet")
     def _wraps_set(self) -> builtins.bool:
         '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
         return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
 
     @_wraps_set.setter
     def _wraps_set(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a639524ed9315ed9d91aac6b0127189faa76eab66ea489a3238da2624df80de2)
+            type_hints = typing.get_type_hints(_typecheckingstub__d95d53ee35c350fc80dac6a96148f86fabee41b7110a6853b4b1a4f0a5d8f0c7)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wrapsSet", value)
 
 
-class DataProxmoxTemplateCloudInitIpOutputReference(
+class DataProxmoxTemplatesTemplatesCloudInitIpOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCloudInitIpOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitIpOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         complex_object_index: jsii.Number,
         complex_object_is_from_set: builtins.bool,
@@ -496,89 +785,91 @@
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param complex_object_index: the index of this item in the list.
         :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fdcfaca0f364368bd1226da91c9f2d31f057343ce49525cef66f18d3335f6bf3)
+            type_hints = typing.get_type_hints(_typecheckingstub__bd10d7eba8b193e54bbf14d276b04c99e46b2cdd97d9ee8c3b3b5574420a6e07)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
     @jsii.member(jsii_name="position")
     def position(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "position"))
 
     @builtins.property
     @jsii.member(jsii_name="v4")
-    def v4(self) -> "DataProxmoxTemplateCloudInitIpV4OutputReference":
-        return typing.cast("DataProxmoxTemplateCloudInitIpV4OutputReference", jsii.get(self, "v4"))
+    def v4(self) -> "DataProxmoxTemplatesTemplatesCloudInitIpV4OutputReference":
+        return typing.cast("DataProxmoxTemplatesTemplatesCloudInitIpV4OutputReference", jsii.get(self, "v4"))
 
     @builtins.property
     @jsii.member(jsii_name="v6")
-    def v6(self) -> "DataProxmoxTemplateCloudInitIpV6OutputReference":
-        return typing.cast("DataProxmoxTemplateCloudInitIpV6OutputReference", jsii.get(self, "v6"))
+    def v6(self) -> "DataProxmoxTemplatesTemplatesCloudInitIpV6OutputReference":
+        return typing.cast("DataProxmoxTemplatesTemplatesCloudInitIpV6OutputReference", jsii.get(self, "v6"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplateCloudInitIp]:
-        return typing.cast(typing.Optional[DataProxmoxTemplateCloudInitIp], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIp]:
+        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIp], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplateCloudInitIp],
+        value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIp],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5858909d52662a9c24ec5106d2d6d35860d6e5b7b7a90223e537459f59ef3e8a)
+            type_hints = typing.get_type_hints(_typecheckingstub__c6edec7bf9da7fc858d6f00b1a2bca916dd1537601759f0547eecdabfc5fd9dd)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCloudInitIpV4",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitIpV4",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplateCloudInitIpV4:
+class DataProxmoxTemplatesTemplatesCloudInitIpV4:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplateCloudInitIpV4(%s)" % ", ".join(
+        return "DataProxmoxTemplatesTemplatesCloudInitIpV4(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplateCloudInitIpV4OutputReference(
+class DataProxmoxTemplatesTemplatesCloudInitIpV4OutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCloudInitIpV4OutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitIpV4OutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e32298d56745ecd36ed7b6548c083eb701114b2286988e4df1114a91553df9b1)
+            type_hints = typing.get_type_hints(_typecheckingstub__489e948956a30a57fae7529bdc147f4aca6ac2e350685a9c13f1011adf371d56)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="address")
     def address(self) -> builtins.str:
@@ -597,65 +888,67 @@
     @builtins.property
     @jsii.member(jsii_name="netmask")
     def netmask(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "netmask"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplateCloudInitIpV4]:
-        return typing.cast(typing.Optional[DataProxmoxTemplateCloudInitIpV4], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV4]:
+        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV4], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplateCloudInitIpV4],
+        value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV4],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__670200d0b80cb4065467e6269dd79835fd42ac8127c3c7d7c9f2751e483f397d)
+            type_hints = typing.get_type_hints(_typecheckingstub__316b4ac8b088bec9d0a20b18732922b3c4f2ec34c73423ab7110590748dc5151)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCloudInitIpV6",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitIpV6",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplateCloudInitIpV6:
+class DataProxmoxTemplatesTemplatesCloudInitIpV6:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplateCloudInitIpV6(%s)" % ", ".join(
+        return "DataProxmoxTemplatesTemplatesCloudInitIpV6(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplateCloudInitIpV6OutputReference(
+class DataProxmoxTemplatesTemplatesCloudInitIpV6OutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCloudInitIpV6OutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitIpV6OutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__cb436ea63218b40afd9e84ad661df0a509f0b7792946dc474097d2aa7ff70a38)
+            type_hints = typing.get_type_hints(_typecheckingstub__794b5f9374ea15e16167c1ac262a044629688c6c6d472d93a73026f2902c9054)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="address")
     def address(self) -> builtins.str:
@@ -674,116 +967,118 @@
     @builtins.property
     @jsii.member(jsii_name="netmask")
     def netmask(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "netmask"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplateCloudInitIpV6]:
-        return typing.cast(typing.Optional[DataProxmoxTemplateCloudInitIpV6], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV6]:
+        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV6], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplateCloudInitIpV6],
+        value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV6],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8c16f92bb88ae79e2bab8492da3727d022ba2c6d6b640706db6a5175e313ce0e)
+            type_hints = typing.get_type_hints(_typecheckingstub__ff35973d8191c68c6e6ff6f7e9a4b46f7fb17e1b8800426dcf85ae2efb76e925)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
-class DataProxmoxTemplateCloudInitOutputReference(
+class DataProxmoxTemplatesTemplatesCloudInitOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCloudInitOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__74586077d05c7122a866ed8368cf9935d56d7f258f9b2fc7b44c3f4da1783caf)
+            type_hints = typing.get_type_hints(_typecheckingstub__29f4c65f37a567f10935f4c966639f7bdf80838af210c4911049934a056a8f50)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="dns")
-    def dns(self) -> DataProxmoxTemplateCloudInitDnsOutputReference:
-        return typing.cast(DataProxmoxTemplateCloudInitDnsOutputReference, jsii.get(self, "dns"))
+    def dns(self) -> DataProxmoxTemplatesTemplatesCloudInitDnsOutputReference:
+        return typing.cast(DataProxmoxTemplatesTemplatesCloudInitDnsOutputReference, jsii.get(self, "dns"))
 
     @builtins.property
     @jsii.member(jsii_name="ip")
-    def ip(self) -> DataProxmoxTemplateCloudInitIpList:
-        return typing.cast(DataProxmoxTemplateCloudInitIpList, jsii.get(self, "ip"))
+    def ip(self) -> DataProxmoxTemplatesTemplatesCloudInitIpList:
+        return typing.cast(DataProxmoxTemplatesTemplatesCloudInitIpList, jsii.get(self, "ip"))
 
     @builtins.property
     @jsii.member(jsii_name="user")
-    def user(self) -> "DataProxmoxTemplateCloudInitUserOutputReference":
-        return typing.cast("DataProxmoxTemplateCloudInitUserOutputReference", jsii.get(self, "user"))
+    def user(self) -> "DataProxmoxTemplatesTemplatesCloudInitUserOutputReference":
+        return typing.cast("DataProxmoxTemplatesTemplatesCloudInitUserOutputReference", jsii.get(self, "user"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplateCloudInit]:
-        return typing.cast(typing.Optional[DataProxmoxTemplateCloudInit], jsii.get(self, "internalValue"))
+    def internal_value(self) -> typing.Optional[DataProxmoxTemplatesTemplatesCloudInit]:
+        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesCloudInit], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplateCloudInit],
+        value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInit],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__bc0ac97475cef00e9aa4edc3efa28ac0964267904611b4de2656597c6942a42c)
+            type_hints = typing.get_type_hints(_typecheckingstub__4aef00a6fe7514158fcad983bbd4c46da783c27bccbf0aeeb7e342ba5ce802b8)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCloudInitUser",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitUser",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplateCloudInitUser:
+class DataProxmoxTemplatesTemplatesCloudInitUser:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplateCloudInitUser(%s)" % ", ".join(
+        return "DataProxmoxTemplatesTemplatesCloudInitUser(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplateCloudInitUserOutputReference(
+class DataProxmoxTemplatesTemplatesCloudInitUserOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCloudInitUserOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitUserOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8017c03ba728226e2f25beddf82fa8ee69a810b0b125e4dc85315d6ece9b4e10)
+            type_hints = typing.get_type_hints(_typecheckingstub__ab97a5c9497e31ad13315c518709649341b3f92644baa1db3ad03d0e7724a704)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
@@ -797,249 +1092,67 @@
     @builtins.property
     @jsii.member(jsii_name="publicKeys")
     def public_keys(self) -> typing.List[builtins.str]:
         return typing.cast(typing.List[builtins.str], jsii.get(self, "publicKeys"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplateCloudInitUser]:
-        return typing.cast(typing.Optional[DataProxmoxTemplateCloudInitUser], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataProxmoxTemplatesTemplatesCloudInitUser]:
+        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesCloudInitUser], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplateCloudInitUser],
+        value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitUser],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4be2a926a83166553f3a011cbac11b1ef06e15f8235607146756e8d6dd148467)
+            type_hints = typing.get_type_hints(_typecheckingstub__40a73c62c87638712e722cd3fd3f967956c8dabb50c0d76987263c31322adf9f)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateConfig",
-    jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
-    name_mapping={
-        "connection": "connection",
-        "count": "count",
-        "depends_on": "dependsOn",
-        "for_each": "forEach",
-        "lifecycle": "lifecycle",
-        "provider": "provider",
-        "provisioners": "provisioners",
-        "node_attribute": "nodeAttribute",
-        "id": "id",
-        "name": "name",
-    },
-)
-class DataProxmoxTemplateConfig(_cdktf_9a9027ec.TerraformMetaArguments):
-    def __init__(
-        self,
-        *,
-        connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
-        depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
-        for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
-        lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
-        provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
-        provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-        node_attribute: builtins.str,
-        id: typing.Optional[jsii.Number] = None,
-        name: typing.Optional[builtins.str] = None,
-    ) -> None:
-        '''
-        :param connection: 
-        :param count: 
-        :param depends_on: 
-        :param for_each: 
-        :param lifecycle: 
-        :param provider: 
-        :param provisioners: 
-        :param node_attribute: The node to create the template on. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/template#node DataProxmoxTemplate#node}
-        :param id: The identifier of the template. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/template#id DataProxmoxTemplate#id} Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param name: The name of the template. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/template#name DataProxmoxTemplate#name}
-        '''
-        if isinstance(lifecycle, dict):
-            lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c66e962d7da1b59d6779dc17def3371d1ed9503b8bbce879d246c36c31a8338e)
-            check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
-            check_type(argname="argument count", value=count, expected_type=type_hints["count"])
-            check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
-            check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
-            check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
-            check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
-            check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
-            check_type(argname="argument node_attribute", value=node_attribute, expected_type=type_hints["node_attribute"])
-            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
-            "node_attribute": node_attribute,
-        }
-        if connection is not None:
-            self._values["connection"] = connection
-        if count is not None:
-            self._values["count"] = count
-        if depends_on is not None:
-            self._values["depends_on"] = depends_on
-        if for_each is not None:
-            self._values["for_each"] = for_each
-        if lifecycle is not None:
-            self._values["lifecycle"] = lifecycle
-        if provider is not None:
-            self._values["provider"] = provider
-        if provisioners is not None:
-            self._values["provisioners"] = provisioners
-        if id is not None:
-            self._values["id"] = id
-        if name is not None:
-            self._values["name"] = name
-
-    @builtins.property
-    def connection(
-        self,
-    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]]:
-        '''
-        :stability: experimental
-        '''
-        result = self._values.get("connection")
-        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, _cdktf_9a9027ec.WinrmProvisionerConnection]], result)
-
-    @builtins.property
-    def count(self) -> typing.Optional[jsii.Number]:
-        '''
-        :stability: experimental
-        '''
-        result = self._values.get("count")
-        return typing.cast(typing.Optional[jsii.Number], result)
-
-    @builtins.property
-    def depends_on(
-        self,
-    ) -> typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]]:
-        '''
-        :stability: experimental
-        '''
-        result = self._values.get("depends_on")
-        return typing.cast(typing.Optional[typing.List[_cdktf_9a9027ec.ITerraformDependable]], result)
-
-    @builtins.property
-    def for_each(self) -> typing.Optional[_cdktf_9a9027ec.ITerraformIterator]:
-        '''
-        :stability: experimental
-        '''
-        result = self._values.get("for_each")
-        return typing.cast(typing.Optional[_cdktf_9a9027ec.ITerraformIterator], result)
-
-    @builtins.property
-    def lifecycle(self) -> typing.Optional[_cdktf_9a9027ec.TerraformResourceLifecycle]:
-        '''
-        :stability: experimental
-        '''
-        result = self._values.get("lifecycle")
-        return typing.cast(typing.Optional[_cdktf_9a9027ec.TerraformResourceLifecycle], result)
-
-    @builtins.property
-    def provider(self) -> typing.Optional[_cdktf_9a9027ec.TerraformProvider]:
-        '''
-        :stability: experimental
-        '''
-        result = self._values.get("provider")
-        return typing.cast(typing.Optional[_cdktf_9a9027ec.TerraformProvider], result)
-
-    @builtins.property
-    def provisioners(
-        self,
-    ) -> typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]]:
-        '''
-        :stability: experimental
-        '''
-        result = self._values.get("provisioners")
-        return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
-
-    @builtins.property
-    def node_attribute(self) -> builtins.str:
-        '''The node to create the template on.
-
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/template#node DataProxmoxTemplate#node}
-        '''
-        result = self._values.get("node_attribute")
-        assert result is not None, "Required property 'node_attribute' is missing"
-        return typing.cast(builtins.str, result)
-
-    @builtins.property
-    def id(self) -> typing.Optional[jsii.Number]:
-        '''The identifier of the template.
-
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/template#id DataProxmoxTemplate#id}
-
-        Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
-        If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        '''
-        result = self._values.get("id")
-        return typing.cast(typing.Optional[jsii.Number], result)
-
-    @builtins.property
-    def name(self) -> typing.Optional[builtins.str]:
-        '''The name of the template.
-
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/template#name DataProxmoxTemplate#name}
-        '''
-        result = self._values.get("name")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "DataProxmoxTemplateConfig(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
-@jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCpu",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCpu",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplateCpu:
+class DataProxmoxTemplatesTemplatesCpu:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplateCpu(%s)" % ", ".join(
+        return "DataProxmoxTemplatesTemplatesCpu(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplateCpuOutputReference(
+class DataProxmoxTemplatesTemplatesCpuOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateCpuOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCpuOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d5ad694d0a6e676f3c07528ea9a73c5686c43202cfdc0ce51031d36235394059)
+            type_hints = typing.get_type_hints(_typecheckingstub__a5a42158ebc03e71f8f9bdc4ad6b1258c5fe9acbd56ba299f3e2fdabdf3cd633)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="architecture")
     def architecture(self) -> builtins.str:
@@ -1063,123 +1176,129 @@
     @builtins.property
     @jsii.member(jsii_name="sockets")
     def sockets(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "sockets"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplateCpu]:
-        return typing.cast(typing.Optional[DataProxmoxTemplateCpu], jsii.get(self, "internalValue"))
+    def internal_value(self) -> typing.Optional[DataProxmoxTemplatesTemplatesCpu]:
+        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesCpu], jsii.get(self, "internalValue"))
 
     @internal_value.setter
-    def internal_value(self, value: typing.Optional[DataProxmoxTemplateCpu]) -> None:
+    def internal_value(
+        self,
+        value: typing.Optional[DataProxmoxTemplatesTemplatesCpu],
+    ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d095c71cb9063b6288ccd4bc5c948ed8d7afd0a4f3765b3e394841c2f0627709)
+            type_hints = typing.get_type_hints(_typecheckingstub__fb0f4d2eadaa9e4d99b7a9686d56e4d9532194127cf03192619771e2ef651831)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateDisks",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesDisks",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplateDisks:
+class DataProxmoxTemplatesTemplatesDisks:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplateDisks(%s)" % ", ".join(
+        return "DataProxmoxTemplatesTemplatesDisks(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplateDisksList(
+class DataProxmoxTemplatesTemplatesDisksList(
     _cdktf_9a9027ec.ComplexList,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateDisksList",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesDisksList",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         wraps_set: builtins.bool,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d934cb067bd5bad71e194ed1eb04a11fe78f08d94d62a2cb8fa2b0d3663fabd9)
+            type_hints = typing.get_type_hints(_typecheckingstub__d5f5bf449c9309a6b5d5c6b7f49c07b04a79a2c1c99b5c48638d61eb31622e7c)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
 
     @jsii.member(jsii_name="get")
-    def get(self, index: jsii.Number) -> "DataProxmoxTemplateDisksOutputReference":
+    def get(
+        self,
+        index: jsii.Number,
+    ) -> "DataProxmoxTemplatesTemplatesDisksOutputReference":
         '''
         :param index: the index of the item to return.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e7b959904dd442874bef4f77d8a6285a0748a317d9bda68d07251affa49ae9a4)
+            type_hints = typing.get_type_hints(_typecheckingstub__8b683a39926cfaa60ef131b3061711541f522c4102ea45f5688bdc06bf9edb19)
             check_type(argname="argument index", value=index, expected_type=type_hints["index"])
-        return typing.cast("DataProxmoxTemplateDisksOutputReference", jsii.invoke(self, "get", [index]))
+        return typing.cast("DataProxmoxTemplatesTemplatesDisksOutputReference", jsii.invoke(self, "get", [index]))
 
     @builtins.property
     @jsii.member(jsii_name="terraformAttribute")
     def _terraform_attribute(self) -> builtins.str:
         '''The attribute on the parent resource this class is referencing.'''
         return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
 
     @_terraform_attribute.setter
     def _terraform_attribute(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__915daeb3c7ec7fb66a6de61c486e42f145eb3b999745d71617cb91c1513163e6)
+            type_hints = typing.get_type_hints(_typecheckingstub__1ceab6297650a2d7fe87e70d5e2c1bc0179b8edd69ebcbea2d28f2d3254a7cf9)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformAttribute", value)
 
     @builtins.property
     @jsii.member(jsii_name="terraformResource")
     def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
         '''The parent resource.'''
         return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
 
     @_terraform_resource.setter
     def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5efb9af77ae5902a9606413f60a3d5ad9027fa7b69ba8131ec1763fe14bf6230)
+            type_hints = typing.get_type_hints(_typecheckingstub__0ac4b2edba5a1f5d58b921e4fd12222646c78eac69326d2f9d9cb8cfdf5293f0)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformResource", value)
 
     @builtins.property
     @jsii.member(jsii_name="wrapsSet")
     def _wraps_set(self) -> builtins.bool:
         '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
         return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
 
     @_wraps_set.setter
     def _wraps_set(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6b870c8e0091075e349b5deddd043676ab0a5962e037d5fdb202d4fee6a2b292)
+            type_hints = typing.get_type_hints(_typecheckingstub__3681c1aed5886b3362ddc27a0c8a45545916b1eea3d5c5525293ae002562a24a)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wrapsSet", value)
 
 
-class DataProxmoxTemplateDisksOutputReference(
+class DataProxmoxTemplatesTemplatesDisksOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateDisksOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesDisksOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         complex_object_index: jsii.Number,
         complex_object_is_from_set: builtins.bool,
@@ -1187,15 +1306,15 @@
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param complex_object_index: the index of this item in the list.
         :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__2b0e17869ddb25a41c76d3a5ac519160a7067a68e37d292a5f1ed31059d8467c)
+            type_hints = typing.get_type_hints(_typecheckingstub__e36693344440afa8e05cd759d3059d6580174e1078ac7d475b89fa21b4348697)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
@@ -1210,32 +1329,29 @@
 
     @builtins.property
     @jsii.member(jsii_name="interfaceType")
     def interface_type(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "interfaceType"))
 
     @builtins.property
-    @jsii.member(jsii_name="name")
-    def name(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "name"))
-
-    @builtins.property
     @jsii.member(jsii_name="position")
     def position(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "position"))
 
     @builtins.property
     @jsii.member(jsii_name="size")
     def size(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "size"))
 
     @builtins.property
     @jsii.member(jsii_name="speedLimits")
-    def speed_limits(self) -> "DataProxmoxTemplateDisksSpeedLimitsOutputReference":
-        return typing.cast("DataProxmoxTemplateDisksSpeedLimitsOutputReference", jsii.get(self, "speedLimits"))
+    def speed_limits(
+        self,
+    ) -> "DataProxmoxTemplatesTemplatesDisksSpeedLimitsOutputReference":
+        return typing.cast("DataProxmoxTemplatesTemplatesDisksSpeedLimitsOutputReference", jsii.get(self, "speedLimits"))
 
     @builtins.property
     @jsii.member(jsii_name="ssdEmulation")
     def ssd_emulation(self) -> _cdktf_9a9027ec.IResolvable:
         return typing.cast(_cdktf_9a9027ec.IResolvable, jsii.get(self, "ssdEmulation"))
 
     @builtins.property
@@ -1246,62 +1362,65 @@
     @builtins.property
     @jsii.member(jsii_name="useIothread")
     def use_iothread(self) -> _cdktf_9a9027ec.IResolvable:
         return typing.cast(_cdktf_9a9027ec.IResolvable, jsii.get(self, "useIothread"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplateDisks]:
-        return typing.cast(typing.Optional[DataProxmoxTemplateDisks], jsii.get(self, "internalValue"))
+    def internal_value(self) -> typing.Optional[DataProxmoxTemplatesTemplatesDisks]:
+        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesDisks], jsii.get(self, "internalValue"))
 
     @internal_value.setter
-    def internal_value(self, value: typing.Optional[DataProxmoxTemplateDisks]) -> None:
+    def internal_value(
+        self,
+        value: typing.Optional[DataProxmoxTemplatesTemplatesDisks],
+    ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d76136e96def88404c7f514d9f5ae578934c3d26236f196df47b2b0171bf4c05)
+            type_hints = typing.get_type_hints(_typecheckingstub__3411d4f953ea91029177b1db6c9690297978a4c8aa4f1a064ccb2be6d9a0219e)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateDisksSpeedLimits",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesDisksSpeedLimits",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplateDisksSpeedLimits:
+class DataProxmoxTemplatesTemplatesDisksSpeedLimits:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplateDisksSpeedLimits(%s)" % ", ".join(
+        return "DataProxmoxTemplatesTemplatesDisksSpeedLimits(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplateDisksSpeedLimitsOutputReference(
+class DataProxmoxTemplatesTemplatesDisksSpeedLimitsOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateDisksSpeedLimitsOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesDisksSpeedLimitsOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d3812467d6dd06534e2a77a87fc511b99edf72a5a9e2e7787178ac76b2f37c24)
+            type_hints = typing.get_type_hints(_typecheckingstub__6507fc59ef695082c0ae01339c5f249d975700e498b4e18908c1eafa158d19f8)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="read")
     def read(self) -> jsii.Number:
@@ -1320,65 +1439,140 @@
     @builtins.property
     @jsii.member(jsii_name="writeBurstable")
     def write_burstable(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "writeBurstable"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplateDisksSpeedLimits]:
-        return typing.cast(typing.Optional[DataProxmoxTemplateDisksSpeedLimits], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataProxmoxTemplatesTemplatesDisksSpeedLimits]:
+        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesDisksSpeedLimits], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplateDisksSpeedLimits],
+        value: typing.Optional[DataProxmoxTemplatesTemplatesDisksSpeedLimits],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6bec67f47786894c96c43bc9bf3a90df6221515612bf3b94a4861ea0ed60cc9c)
+            type_hints = typing.get_type_hints(_typecheckingstub__c18f8c7ed8d24d2b06774c7cd39f86063e0c0dd2b09ba5b07796c7ebbfa6b319)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
+class DataProxmoxTemplatesTemplatesList(
+    _cdktf_9a9027ec.ComplexList,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesList",
+):
+    def __init__(
+        self,
+        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+        terraform_attribute: builtins.str,
+        wraps_set: builtins.bool,
+    ) -> None:
+        '''
+        :param terraform_resource: The parent resource.
+        :param terraform_attribute: The attribute on the parent resource this class is referencing.
+        :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__0f08ad26095875cedb140ea7fee38d064da3ca7274d935b385b43bee3f8e0224)
+            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
+            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
+            check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
+        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
+
+    @jsii.member(jsii_name="get")
+    def get(self, index: jsii.Number) -> "DataProxmoxTemplatesTemplatesOutputReference":
+        '''
+        :param index: the index of the item to return.
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__a73b9f8ad3ee64bf1330033bbb94eda72651474ebf3cc08f02fdb5164474837f)
+            check_type(argname="argument index", value=index, expected_type=type_hints["index"])
+        return typing.cast("DataProxmoxTemplatesTemplatesOutputReference", jsii.invoke(self, "get", [index]))
+
+    @builtins.property
+    @jsii.member(jsii_name="terraformAttribute")
+    def _terraform_attribute(self) -> builtins.str:
+        '''The attribute on the parent resource this class is referencing.'''
+        return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
+
+    @_terraform_attribute.setter
+    def _terraform_attribute(self, value: builtins.str) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__848480b079fffd0ff9a7f3a525600012d4afc4dee5881b91ae5e7167dbb59566)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "terraformAttribute", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="terraformResource")
+    def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
+        '''The parent resource.'''
+        return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
+
+    @_terraform_resource.setter
+    def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__fa2c9ff301f9aee5b2b11bbfc41fe82846b8379b5d0938c0623854abf252aa3c)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "terraformResource", value)
+
+    @builtins.property
+    @jsii.member(jsii_name="wrapsSet")
+    def _wraps_set(self) -> builtins.bool:
+        '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
+        return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
+
+    @_wraps_set.setter
+    def _wraps_set(self, value: builtins.bool) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__abebb6092537f032ac958ea0c960b43351ae38dc63f45c0caf96a643d0c578a2)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "wrapsSet", value)
+
+
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateMemory",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesMemory",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplateMemory:
+class DataProxmoxTemplatesTemplatesMemory:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplateMemory(%s)" % ", ".join(
+        return "DataProxmoxTemplatesTemplatesMemory(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplateMemoryOutputReference(
+class DataProxmoxTemplatesTemplatesMemoryOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateMemoryOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesMemoryOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7c7902293e25759c34bd47d693e7b5a145bba9a8c4108581eeba30ad984b2615)
+            type_hints = typing.get_type_hints(_typecheckingstub__85086878bd5559f9bcb76f72ef7d39713a5dfe1a67404088b22a948985c5628d)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="dedicated")
     def dedicated(self) -> jsii.Number:
@@ -1392,126 +1586,129 @@
     @builtins.property
     @jsii.member(jsii_name="shared")
     def shared(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "shared"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplateMemory]:
-        return typing.cast(typing.Optional[DataProxmoxTemplateMemory], jsii.get(self, "internalValue"))
+    def internal_value(self) -> typing.Optional[DataProxmoxTemplatesTemplatesMemory]:
+        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesMemory], jsii.get(self, "internalValue"))
 
     @internal_value.setter
-    def internal_value(self, value: typing.Optional[DataProxmoxTemplateMemory]) -> None:
+    def internal_value(
+        self,
+        value: typing.Optional[DataProxmoxTemplatesTemplatesMemory],
+    ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__816a4adb150a0a61973935b50fe3ad4cf68c614e4184b3ae204ed20a4f2768ee)
+            type_hints = typing.get_type_hints(_typecheckingstub__37ed7ef44a558b41c24319f430bd9d5e8e061f43edd93c6b14328bd6a508557c)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateNetworkInterfaces",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesNetworkInterfaces",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplateNetworkInterfaces:
+class DataProxmoxTemplatesTemplatesNetworkInterfaces:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplateNetworkInterfaces(%s)" % ", ".join(
+        return "DataProxmoxTemplatesTemplatesNetworkInterfaces(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplateNetworkInterfacesList(
+class DataProxmoxTemplatesTemplatesNetworkInterfacesList(
     _cdktf_9a9027ec.ComplexList,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateNetworkInterfacesList",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesNetworkInterfacesList",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         wraps_set: builtins.bool,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d4affaf046aecdcd0850cb64d1fd3be684aeaad4d6ea012096dfdf00dd5d890a)
+            type_hints = typing.get_type_hints(_typecheckingstub__936967cce1c15f47cc61cad0804576959a9d43335f92de11fff9576904e2c633)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
 
     @jsii.member(jsii_name="get")
     def get(
         self,
         index: jsii.Number,
-    ) -> "DataProxmoxTemplateNetworkInterfacesOutputReference":
+    ) -> "DataProxmoxTemplatesTemplatesNetworkInterfacesOutputReference":
         '''
         :param index: the index of the item to return.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__286d6638f911e42cf08d10d1df09bb89c7b9e5ae901d0120eb2aa840c31c4a0c)
+            type_hints = typing.get_type_hints(_typecheckingstub__737e30ba026c9167075fe33c1c2bd27a25ebda2df3ada8476ea562276b30e283)
             check_type(argname="argument index", value=index, expected_type=type_hints["index"])
-        return typing.cast("DataProxmoxTemplateNetworkInterfacesOutputReference", jsii.invoke(self, "get", [index]))
+        return typing.cast("DataProxmoxTemplatesTemplatesNetworkInterfacesOutputReference", jsii.invoke(self, "get", [index]))
 
     @builtins.property
     @jsii.member(jsii_name="terraformAttribute")
     def _terraform_attribute(self) -> builtins.str:
         '''The attribute on the parent resource this class is referencing.'''
         return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
 
     @_terraform_attribute.setter
     def _terraform_attribute(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b98dd353b7d0a794e3df6c5bfa14a1c81e0b8ced4efa40dbaf0c54cb44a76205)
+            type_hints = typing.get_type_hints(_typecheckingstub__48cef1cb379832d204d05e71200269648461a5d9b90d6210fd7323d5d5683d49)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformAttribute", value)
 
     @builtins.property
     @jsii.member(jsii_name="terraformResource")
     def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
         '''The parent resource.'''
         return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
 
     @_terraform_resource.setter
     def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3072c672c8f942bc66a66b6147b2f01463e3f9fdb58332469031b4b76452899c)
+            type_hints = typing.get_type_hints(_typecheckingstub__7a78040dc29e020dddb0be94997801ef14e00270db063f5d34e30354fa694ed1)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformResource", value)
 
     @builtins.property
     @jsii.member(jsii_name="wrapsSet")
     def _wraps_set(self) -> builtins.bool:
         '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
         return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
 
     @_wraps_set.setter
     def _wraps_set(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__bd90e6a0216187386fcd8bc7edfdaa6fcca12336f19fcfc1d7cf6e583092e563)
+            type_hints = typing.get_type_hints(_typecheckingstub__83fa36cc540531a6aa1ce8e8e244ee7b9cd0d2e5314e607e6bdb917be2c4cd9c)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wrapsSet", value)
 
 
-class DataProxmoxTemplateNetworkInterfacesOutputReference(
+class DataProxmoxTemplatesTemplatesNetworkInterfacesOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplateNetworkInterfacesOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesNetworkInterfacesOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         complex_object_index: jsii.Number,
         complex_object_is_from_set: builtins.bool,
@@ -1519,15 +1716,15 @@
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param complex_object_index: the index of this item in the list.
         :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__bf24f3e52ac1ee2a2154a45e764132f705e7e629195695ae9ee0ea2eaecd394c)
+            type_hints = typing.get_type_hints(_typecheckingstub__ca79e6840c22cc22b6a35edff39fed27bec20ff0729d3864153eda76572b6639)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
@@ -1573,126 +1770,268 @@
     @builtins.property
     @jsii.member(jsii_name="vlan")
     def vlan(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "vlan"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplateNetworkInterfaces]:
-        return typing.cast(typing.Optional[DataProxmoxTemplateNetworkInterfaces], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataProxmoxTemplatesTemplatesNetworkInterfaces]:
+        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesNetworkInterfaces], jsii.get(self, "internalValue"))
+
+    @internal_value.setter
+    def internal_value(
+        self,
+        value: typing.Optional[DataProxmoxTemplatesTemplatesNetworkInterfaces],
+    ) -> None:
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__1c58d8361d95c8785388c651a8bef3bdef6a00dcdb17739df96e92e48f2667ca)
+            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
+        jsii.set(self, "internalValue", value)
+
+
+class DataProxmoxTemplatesTemplatesOutputReference(
+    _cdktf_9a9027ec.ComplexObject,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesOutputReference",
+):
+    def __init__(
+        self,
+        terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+        terraform_attribute: builtins.str,
+        complex_object_index: jsii.Number,
+        complex_object_is_from_set: builtins.bool,
+    ) -> None:
+        '''
+        :param terraform_resource: The parent resource.
+        :param terraform_attribute: The attribute on the parent resource this class is referencing.
+        :param complex_object_index: the index of this item in the list.
+        :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__b202d7279af3d9819fdce569a9167c00ce44a03a626378a9a38f76286414bc81)
+            check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
+            check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
+            check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
+            check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
+        jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
+
+    @builtins.property
+    @jsii.member(jsii_name="agent")
+    def agent(self) -> DataProxmoxTemplatesTemplatesAgentOutputReference:
+        return typing.cast(DataProxmoxTemplatesTemplatesAgentOutputReference, jsii.get(self, "agent"))
+
+    @builtins.property
+    @jsii.member(jsii_name="bios")
+    def bios(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "bios"))
+
+    @builtins.property
+    @jsii.member(jsii_name="cloudInit")
+    def cloud_init(self) -> DataProxmoxTemplatesTemplatesCloudInitOutputReference:
+        return typing.cast(DataProxmoxTemplatesTemplatesCloudInitOutputReference, jsii.get(self, "cloudInit"))
+
+    @builtins.property
+    @jsii.member(jsii_name="cpu")
+    def cpu(self) -> DataProxmoxTemplatesTemplatesCpuOutputReference:
+        return typing.cast(DataProxmoxTemplatesTemplatesCpuOutputReference, jsii.get(self, "cpu"))
+
+    @builtins.property
+    @jsii.member(jsii_name="description")
+    def description(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "description"))
+
+    @builtins.property
+    @jsii.member(jsii_name="disks")
+    def disks(self) -> DataProxmoxTemplatesTemplatesDisksList:
+        return typing.cast(DataProxmoxTemplatesTemplatesDisksList, jsii.get(self, "disks"))
+
+    @builtins.property
+    @jsii.member(jsii_name="id")
+    def id(self) -> jsii.Number:
+        return typing.cast(jsii.Number, jsii.get(self, "id"))
+
+    @builtins.property
+    @jsii.member(jsii_name="keyboardLayout")
+    def keyboard_layout(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "keyboardLayout"))
+
+    @builtins.property
+    @jsii.member(jsii_name="kvmArguments")
+    def kvm_arguments(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "kvmArguments"))
+
+    @builtins.property
+    @jsii.member(jsii_name="machineType")
+    def machine_type(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "machineType"))
+
+    @builtins.property
+    @jsii.member(jsii_name="memory")
+    def memory(self) -> DataProxmoxTemplatesTemplatesMemoryOutputReference:
+        return typing.cast(DataProxmoxTemplatesTemplatesMemoryOutputReference, jsii.get(self, "memory"))
+
+    @builtins.property
+    @jsii.member(jsii_name="name")
+    def name(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "name"))
+
+    @builtins.property
+    @jsii.member(jsii_name="networkInterfaces")
+    def network_interfaces(self) -> DataProxmoxTemplatesTemplatesNetworkInterfacesList:
+        return typing.cast(DataProxmoxTemplatesTemplatesNetworkInterfacesList, jsii.get(self, "networkInterfaces"))
+
+    @builtins.property
+    @jsii.member(jsii_name="nodeAttribute")
+    def node_attribute(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "nodeAttribute"))
+
+    @builtins.property
+    @jsii.member(jsii_name="pciDevices")
+    def pci_devices(self) -> "DataProxmoxTemplatesTemplatesPciDevicesList":
+        return typing.cast("DataProxmoxTemplatesTemplatesPciDevicesList", jsii.get(self, "pciDevices"))
+
+    @builtins.property
+    @jsii.member(jsii_name="resourcePool")
+    def resource_pool(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "resourcePool"))
+
+    @builtins.property
+    @jsii.member(jsii_name="startOnNodeBoot")
+    def start_on_node_boot(self) -> _cdktf_9a9027ec.IResolvable:
+        return typing.cast(_cdktf_9a9027ec.IResolvable, jsii.get(self, "startOnNodeBoot"))
+
+    @builtins.property
+    @jsii.member(jsii_name="tags")
+    def tags(self) -> typing.List[builtins.str]:
+        return typing.cast(typing.List[builtins.str], jsii.get(self, "tags"))
+
+    @builtins.property
+    @jsii.member(jsii_name="type")
+    def type(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "type"))
+
+    @builtins.property
+    @jsii.member(jsii_name="internalValue")
+    def internal_value(self) -> typing.Optional[DataProxmoxTemplatesTemplates]:
+        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplates], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplateNetworkInterfaces],
+        value: typing.Optional[DataProxmoxTemplatesTemplates],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8033212282867c593cf20f46be56c12ceb93404971dab446236dee4b3c4289b1)
+            type_hints = typing.get_type_hints(_typecheckingstub__6e3dc4c5d3942ba601d2415386e2de0a087c80913e1cfdafc5a86ecb25ca0683)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplatePciDevices",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesPciDevices",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatePciDevices:
+class DataProxmoxTemplatesTemplatesPciDevices:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatePciDevices(%s)" % ", ".join(
+        return "DataProxmoxTemplatesTemplatesPciDevices(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplatePciDevicesList(
+class DataProxmoxTemplatesTemplatesPciDevicesList(
     _cdktf_9a9027ec.ComplexList,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplatePciDevicesList",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesPciDevicesList",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         wraps_set: builtins.bool,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8f84e607ba3ff415d65f603a56a2c31c2cd3095793b7815bb964d56c8fdb2196)
+            type_hints = typing.get_type_hints(_typecheckingstub__55717d97f120003fb6031ddd71985e3f4c5eab0344a8c0befa42a9c89633667d)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
 
     @jsii.member(jsii_name="get")
-    def get(self, index: jsii.Number) -> "DataProxmoxTemplatePciDevicesOutputReference":
+    def get(
+        self,
+        index: jsii.Number,
+    ) -> "DataProxmoxTemplatesTemplatesPciDevicesOutputReference":
         '''
         :param index: the index of the item to return.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ec52f08bd041e7443d774e9d2822ad213552c49b0a731462f640bb960ccaafdf)
+            type_hints = typing.get_type_hints(_typecheckingstub__569cf596a9a1d3ba8639edd9a452162acdb7b653adf57ee077a1dbb1de70be96)
             check_type(argname="argument index", value=index, expected_type=type_hints["index"])
-        return typing.cast("DataProxmoxTemplatePciDevicesOutputReference", jsii.invoke(self, "get", [index]))
+        return typing.cast("DataProxmoxTemplatesTemplatesPciDevicesOutputReference", jsii.invoke(self, "get", [index]))
 
     @builtins.property
     @jsii.member(jsii_name="terraformAttribute")
     def _terraform_attribute(self) -> builtins.str:
         '''The attribute on the parent resource this class is referencing.'''
         return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
 
     @_terraform_attribute.setter
     def _terraform_attribute(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d51157ff75882eb0c613abc4a7539579579f805674b7ba75f747166cfa6aa982)
+            type_hints = typing.get_type_hints(_typecheckingstub__714ca5189a7e8b8efcba574865cb9541d6bb35e576329c8f5cbd05bfacafcd09)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformAttribute", value)
 
     @builtins.property
     @jsii.member(jsii_name="terraformResource")
     def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
         '''The parent resource.'''
         return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
 
     @_terraform_resource.setter
     def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a339abc46978c87a76cd443abebf11fe00e403b38389989b7934e8a7f8f24d43)
+            type_hints = typing.get_type_hints(_typecheckingstub__400324fc47b84d680a8d6d870b00bcf22a76e01f2693f58a18e7bb03636c6f54)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformResource", value)
 
     @builtins.property
     @jsii.member(jsii_name="wrapsSet")
     def _wraps_set(self) -> builtins.bool:
         '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
         return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
 
     @_wraps_set.setter
     def _wraps_set(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9e56c0d9053713ded7ea08ca036217098c9a9846691b786af6f67e63338ed713)
+            type_hints = typing.get_type_hints(_typecheckingstub__a314b4987d3ace06086de87977325702d27f5bba1ee500f931eb8285c6098fd2)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wrapsSet", value)
 
 
-class DataProxmoxTemplatePciDevicesOutputReference(
+class DataProxmoxTemplatesTemplatesPciDevicesOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplate.DataProxmoxTemplatePciDevicesOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesPciDevicesOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         complex_object_index: jsii.Number,
         complex_object_is_from_set: builtins.bool,
@@ -1700,15 +2039,15 @@
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param complex_object_index: the index of this item in the list.
         :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0a5b183d4c57837e9e4a9da4194da401e1fa320644c940b74d7c8d95ff4a54c3)
+            type_hints = typing.get_type_hints(_typecheckingstub__42f0553ee26f760ca9dbe015a65d976a474040e167c3eb17a393b33cc0ce92c1)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
@@ -1744,414 +2083,526 @@
     @builtins.property
     @jsii.member(jsii_name="romFile")
     def rom_file(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "romFile"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplatePciDevices]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatePciDevices], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataProxmoxTemplatesTemplatesPciDevices]:
+        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesPciDevices], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatePciDevices],
+        value: typing.Optional[DataProxmoxTemplatesTemplatesPciDevices],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e9726e8994ee71310eff26984027fd5d3eeeb95bdc529a0e97af5772d4d21709)
+            type_hints = typing.get_type_hints(_typecheckingstub__1bb2963547ad5083d7060c4cf5df44ddaf83851eefd9ab93fb720702b84cc7ad)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 __all__ = [
-    "DataProxmoxTemplate",
-    "DataProxmoxTemplateAgent",
-    "DataProxmoxTemplateAgentOutputReference",
-    "DataProxmoxTemplateCloudInit",
-    "DataProxmoxTemplateCloudInitDns",
-    "DataProxmoxTemplateCloudInitDnsOutputReference",
-    "DataProxmoxTemplateCloudInitIp",
-    "DataProxmoxTemplateCloudInitIpList",
-    "DataProxmoxTemplateCloudInitIpOutputReference",
-    "DataProxmoxTemplateCloudInitIpV4",
-    "DataProxmoxTemplateCloudInitIpV4OutputReference",
-    "DataProxmoxTemplateCloudInitIpV6",
-    "DataProxmoxTemplateCloudInitIpV6OutputReference",
-    "DataProxmoxTemplateCloudInitOutputReference",
-    "DataProxmoxTemplateCloudInitUser",
-    "DataProxmoxTemplateCloudInitUserOutputReference",
-    "DataProxmoxTemplateConfig",
-    "DataProxmoxTemplateCpu",
-    "DataProxmoxTemplateCpuOutputReference",
-    "DataProxmoxTemplateDisks",
-    "DataProxmoxTemplateDisksList",
-    "DataProxmoxTemplateDisksOutputReference",
-    "DataProxmoxTemplateDisksSpeedLimits",
-    "DataProxmoxTemplateDisksSpeedLimitsOutputReference",
-    "DataProxmoxTemplateMemory",
-    "DataProxmoxTemplateMemoryOutputReference",
-    "DataProxmoxTemplateNetworkInterfaces",
-    "DataProxmoxTemplateNetworkInterfacesList",
-    "DataProxmoxTemplateNetworkInterfacesOutputReference",
-    "DataProxmoxTemplatePciDevices",
-    "DataProxmoxTemplatePciDevicesList",
-    "DataProxmoxTemplatePciDevicesOutputReference",
+    "DataProxmoxTemplates",
+    "DataProxmoxTemplatesConfig",
+    "DataProxmoxTemplatesFilters",
+    "DataProxmoxTemplatesFiltersList",
+    "DataProxmoxTemplatesFiltersOutputReference",
+    "DataProxmoxTemplatesTemplates",
+    "DataProxmoxTemplatesTemplatesAgent",
+    "DataProxmoxTemplatesTemplatesAgentOutputReference",
+    "DataProxmoxTemplatesTemplatesCloudInit",
+    "DataProxmoxTemplatesTemplatesCloudInitDns",
+    "DataProxmoxTemplatesTemplatesCloudInitDnsOutputReference",
+    "DataProxmoxTemplatesTemplatesCloudInitIp",
+    "DataProxmoxTemplatesTemplatesCloudInitIpList",
+    "DataProxmoxTemplatesTemplatesCloudInitIpOutputReference",
+    "DataProxmoxTemplatesTemplatesCloudInitIpV4",
+    "DataProxmoxTemplatesTemplatesCloudInitIpV4OutputReference",
+    "DataProxmoxTemplatesTemplatesCloudInitIpV6",
+    "DataProxmoxTemplatesTemplatesCloudInitIpV6OutputReference",
+    "DataProxmoxTemplatesTemplatesCloudInitOutputReference",
+    "DataProxmoxTemplatesTemplatesCloudInitUser",
+    "DataProxmoxTemplatesTemplatesCloudInitUserOutputReference",
+    "DataProxmoxTemplatesTemplatesCpu",
+    "DataProxmoxTemplatesTemplatesCpuOutputReference",
+    "DataProxmoxTemplatesTemplatesDisks",
+    "DataProxmoxTemplatesTemplatesDisksList",
+    "DataProxmoxTemplatesTemplatesDisksOutputReference",
+    "DataProxmoxTemplatesTemplatesDisksSpeedLimits",
+    "DataProxmoxTemplatesTemplatesDisksSpeedLimitsOutputReference",
+    "DataProxmoxTemplatesTemplatesList",
+    "DataProxmoxTemplatesTemplatesMemory",
+    "DataProxmoxTemplatesTemplatesMemoryOutputReference",
+    "DataProxmoxTemplatesTemplatesNetworkInterfaces",
+    "DataProxmoxTemplatesTemplatesNetworkInterfacesList",
+    "DataProxmoxTemplatesTemplatesNetworkInterfacesOutputReference",
+    "DataProxmoxTemplatesTemplatesOutputReference",
+    "DataProxmoxTemplatesTemplatesPciDevices",
+    "DataProxmoxTemplatesTemplatesPciDevicesList",
+    "DataProxmoxTemplatesTemplatesPciDevicesOutputReference",
 ]
 
 publication.publish()
 
-def _typecheckingstub__e4ef2cd22cf433a6e1971b184320047824643e5aace46960ef74bf9cbf53982a(
+def _typecheckingstub__9c8f43a8ed4d9862bb2dfda7c754989b1621c88e999f35c8aa0300d8f6ba0675(
     scope: _constructs_77d1e7e8.Construct,
-    id_: builtins.str,
+    id: builtins.str,
+    *,
+    filters: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataProxmoxTemplatesFilters, typing.Dict[builtins.str, typing.Any]]]]] = None,
+    connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
+    count: typing.Optional[jsii.Number] = None,
+    depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
+    for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
+    lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
+    provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
+    provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__233a1989690e82037c4c9dc0c040be824ca0bc7ab5562170fe8918e4876b29f9(
+    value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataProxmoxTemplatesFilters, typing.Dict[builtins.str, typing.Any]]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4b9b87d43a9822a28f232fcb57074d7978bca6aa140657b9397ad2bf3cabac68(
     *,
-    node_attribute: builtins.str,
-    id: typing.Optional[jsii.Number] = None,
-    name: typing.Optional[builtins.str] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[jsii.Number] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
+    filters: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataProxmoxTemplatesFilters, typing.Dict[builtins.str, typing.Any]]]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7b5a2e2e69a8b272223cae04497ef0e50f1388bd002ce5d48b07318623fc0fd0(
+    *,
+    name: builtins.str,
+    values: typing.Sequence[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__7185592ee5df14f6502caf1b02c1c8f7f1a998c262a921b4059ae73ed17d01f7(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
+    wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a4eeeeba3c39a0f8fd661594829813f3b5a08a9acc56fe1852ca4f52acbb54e1(
-    value: jsii.Number,
+def _typecheckingstub__b3e0e2fef1c0a4b8e2a1b64ae525d2b0ac767a60597d7eb6476cf5a4b328eb58(
+    index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__2ceebbba99c0db4bd5489cb0e441408679e0230c816b563d9bfed0277fb7d9c8(
+def _typecheckingstub__12203107c9a9b5812061df83af59f971166e12e0dd3c53822898b587c4a13a1a(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__cb31b96735bf37ac81d559ab0ce9a0af448e344b0dbcaa737213f4ce4ddaf6c3(
+def _typecheckingstub__7c18c8f27f5b5749f0930032ce59cf9aa9dd8c3fe11454a21edfacfb39110484(
+    value: _cdktf_9a9027ec.IInterpolatingParent,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1de467d3e8e92a1d8d17a81042c85e45ddb8a5f8a574026c01b38410619c435e(
+    value: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__4eeb8042fe9f97bb3b08f79bdd3f5544c61ad333e13f34069ee25b3925b85f8c(
+    value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataProxmoxTemplatesFilters]]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8327cf5bac96b9877733ed3b92c5e728be3a17f989a4bdbaf2900a291c81f07d(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
+    complex_object_index: jsii.Number,
+    complex_object_is_from_set: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__16f3ef7637865b9efbe01d5d61b463f735bae38264ad57354abdbce513208aef(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1bb6e3882eca230c304fbf04eb486d51f93c5b3cec722cf92e5d311e526f7c11(
+def _typecheckingstub__8a7dc4004f107546dc9c621fa798620b5001c0fd8917d4c9140a0ad48064ed70(
+    value: typing.List[builtins.str],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__dec6db530ef281b602f64ed73e330e24906e6e0c6b954683c5ba96b7ad21dcbf(
+    value: typing.Optional[typing.Union[DataProxmoxTemplatesFilters, _cdktf_9a9027ec.IResolvable]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__673e66db611a5fbc4e59ce825f6e4416fa82cbf66904ba65202f13a93beb37d2(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b6bb09a4e0bd03a04ee862ea7232014b12fe4ae50859f376a3d90f318942f2c5(
-    value: typing.Optional[DataProxmoxTemplateAgent],
+def _typecheckingstub__11571a58fd163ae522f420d6c0dff17873e68251c637a1ebc2f4261d40a0908e(
+    value: typing.Optional[DataProxmoxTemplatesTemplatesAgent],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b85bfac621b455ab5a57c0b8c4693493aac54564221c9c9a9519403ea8e69700(
+def _typecheckingstub__e067c9db4e634da658b56ee80ca7edfde446f1a440b47d1f6eb546e326a67b26(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ad3a996ef8508c2e45f8c89cbe97b055c8049b37dfc00c7c621d91ecb1658772(
-    value: typing.Optional[DataProxmoxTemplateCloudInitDns],
+def _typecheckingstub__0782611e20910ed665dc0d5e84a3f71452ba5bade5ae664490668cd11d64b023(
+    value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitDns],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__4a7c2c37c375e4ab986f9089b062a7e192800caf657d5ec277feea581473b4d0(
+def _typecheckingstub__99f203b02f9592f1a1fb7a64a5635c720b9dd6c7f992bc56e8edb0bab0e63ae7(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__3e009569d142ff7aba80375d28185467544bd3f2873a65544d9839015570431d(
+def _typecheckingstub__17abca3a5e9277181468d701c2550bed8e6e1d101cde67b7c64c5bf22a976a80(
     index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__6fb11e8926625e3516c5ba5e7e6c66632c96345b59c27a2a58b803fe0c08c28d(
+def _typecheckingstub__8f5acfd27a377920da103fd958e5f6b4dbf0ed9b81ad89a5f0293c850734683d(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__2bb8b6c66ae22b277647f9c432e158f1b082f79d274ca0d23fb83aea02ee6a1c(
+def _typecheckingstub__4ab6c78fc6f14f4f992d620cd01deffae673cfc19cb90a2b3a92306efc35ecdc(
     value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a639524ed9315ed9d91aac6b0127189faa76eab66ea489a3238da2624df80de2(
+def _typecheckingstub__d95d53ee35c350fc80dac6a96148f86fabee41b7110a6853b4b1a4f0a5d8f0c7(
     value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__fdcfaca0f364368bd1226da91c9f2d31f057343ce49525cef66f18d3335f6bf3(
+def _typecheckingstub__bd10d7eba8b193e54bbf14d276b04c99e46b2cdd97d9ee8c3b3b5574420a6e07(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__5858909d52662a9c24ec5106d2d6d35860d6e5b7b7a90223e537459f59ef3e8a(
-    value: typing.Optional[DataProxmoxTemplateCloudInitIp],
+def _typecheckingstub__c6edec7bf9da7fc858d6f00b1a2bca916dd1537601759f0547eecdabfc5fd9dd(
+    value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIp],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__e32298d56745ecd36ed7b6548c083eb701114b2286988e4df1114a91553df9b1(
+def _typecheckingstub__489e948956a30a57fae7529bdc147f4aca6ac2e350685a9c13f1011adf371d56(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__670200d0b80cb4065467e6269dd79835fd42ac8127c3c7d7c9f2751e483f397d(
-    value: typing.Optional[DataProxmoxTemplateCloudInitIpV4],
+def _typecheckingstub__316b4ac8b088bec9d0a20b18732922b3c4f2ec34c73423ab7110590748dc5151(
+    value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV4],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__cb436ea63218b40afd9e84ad661df0a509f0b7792946dc474097d2aa7ff70a38(
+def _typecheckingstub__794b5f9374ea15e16167c1ac262a044629688c6c6d472d93a73026f2902c9054(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__8c16f92bb88ae79e2bab8492da3727d022ba2c6d6b640706db6a5175e313ce0e(
-    value: typing.Optional[DataProxmoxTemplateCloudInitIpV6],
+def _typecheckingstub__ff35973d8191c68c6e6ff6f7e9a4b46f7fb17e1b8800426dcf85ae2efb76e925(
+    value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV6],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__74586077d05c7122a866ed8368cf9935d56d7f258f9b2fc7b44c3f4da1783caf(
+def _typecheckingstub__29f4c65f37a567f10935f4c966639f7bdf80838af210c4911049934a056a8f50(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__bc0ac97475cef00e9aa4edc3efa28ac0964267904611b4de2656597c6942a42c(
-    value: typing.Optional[DataProxmoxTemplateCloudInit],
+def _typecheckingstub__4aef00a6fe7514158fcad983bbd4c46da783c27bccbf0aeeb7e342ba5ce802b8(
+    value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInit],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__8017c03ba728226e2f25beddf82fa8ee69a810b0b125e4dc85315d6ece9b4e10(
+def _typecheckingstub__ab97a5c9497e31ad13315c518709649341b3f92644baa1db3ad03d0e7724a704(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__4be2a926a83166553f3a011cbac11b1ef06e15f8235607146756e8d6dd148467(
-    value: typing.Optional[DataProxmoxTemplateCloudInitUser],
+def _typecheckingstub__40a73c62c87638712e722cd3fd3f967956c8dabb50c0d76987263c31322adf9f(
+    value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitUser],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__c66e962d7da1b59d6779dc17def3371d1ed9503b8bbce879d246c36c31a8338e(
-    *,
-    connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
-    depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
-    for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
-    lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
-    provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
-    provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    node_attribute: builtins.str,
-    id: typing.Optional[jsii.Number] = None,
-    name: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__d5ad694d0a6e676f3c07528ea9a73c5686c43202cfdc0ce51031d36235394059(
+def _typecheckingstub__a5a42158ebc03e71f8f9bdc4ad6b1258c5fe9acbd56ba299f3e2fdabdf3cd633(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__d095c71cb9063b6288ccd4bc5c948ed8d7afd0a4f3765b3e394841c2f0627709(
-    value: typing.Optional[DataProxmoxTemplateCpu],
+def _typecheckingstub__fb0f4d2eadaa9e4d99b7a9686d56e4d9532194127cf03192619771e2ef651831(
+    value: typing.Optional[DataProxmoxTemplatesTemplatesCpu],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__d934cb067bd5bad71e194ed1eb04a11fe78f08d94d62a2cb8fa2b0d3663fabd9(
+def _typecheckingstub__d5f5bf449c9309a6b5d5c6b7f49c07b04a79a2c1c99b5c48638d61eb31622e7c(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__e7b959904dd442874bef4f77d8a6285a0748a317d9bda68d07251affa49ae9a4(
+def _typecheckingstub__8b683a39926cfaa60ef131b3061711541f522c4102ea45f5688bdc06bf9edb19(
     index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__915daeb3c7ec7fb66a6de61c486e42f145eb3b999745d71617cb91c1513163e6(
+def _typecheckingstub__1ceab6297650a2d7fe87e70d5e2c1bc0179b8edd69ebcbea2d28f2d3254a7cf9(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__5efb9af77ae5902a9606413f60a3d5ad9027fa7b69ba8131ec1763fe14bf6230(
+def _typecheckingstub__0ac4b2edba5a1f5d58b921e4fd12222646c78eac69326d2f9d9cb8cfdf5293f0(
     value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__6b870c8e0091075e349b5deddd043676ab0a5962e037d5fdb202d4fee6a2b292(
+def _typecheckingstub__3681c1aed5886b3362ddc27a0c8a45545916b1eea3d5c5525293ae002562a24a(
     value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__2b0e17869ddb25a41c76d3a5ac519160a7067a68e37d292a5f1ed31059d8467c(
+def _typecheckingstub__e36693344440afa8e05cd759d3059d6580174e1078ac7d475b89fa21b4348697(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__d76136e96def88404c7f514d9f5ae578934c3d26236f196df47b2b0171bf4c05(
-    value: typing.Optional[DataProxmoxTemplateDisks],
+def _typecheckingstub__3411d4f953ea91029177b1db6c9690297978a4c8aa4f1a064ccb2be6d9a0219e(
+    value: typing.Optional[DataProxmoxTemplatesTemplatesDisks],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__d3812467d6dd06534e2a77a87fc511b99edf72a5a9e2e7787178ac76b2f37c24(
+def _typecheckingstub__6507fc59ef695082c0ae01339c5f249d975700e498b4e18908c1eafa158d19f8(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__6bec67f47786894c96c43bc9bf3a90df6221515612bf3b94a4861ea0ed60cc9c(
-    value: typing.Optional[DataProxmoxTemplateDisksSpeedLimits],
+def _typecheckingstub__c18f8c7ed8d24d2b06774c7cd39f86063e0c0dd2b09ba5b07796c7ebbfa6b319(
+    value: typing.Optional[DataProxmoxTemplatesTemplatesDisksSpeedLimits],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0f08ad26095875cedb140ea7fee38d064da3ca7274d935b385b43bee3f8e0224(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
+    wraps_set: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__a73b9f8ad3ee64bf1330033bbb94eda72651474ebf3cc08f02fdb5164474837f(
+    index: jsii.Number,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__848480b079fffd0ff9a7f3a525600012d4afc4dee5881b91ae5e7167dbb59566(
+    value: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__fa2c9ff301f9aee5b2b11bbfc41fe82846b8379b5d0938c0623854abf252aa3c(
+    value: _cdktf_9a9027ec.IInterpolatingParent,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__abebb6092537f032ac958ea0c960b43351ae38dc63f45c0caf96a643d0c578a2(
+    value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7c7902293e25759c34bd47d693e7b5a145bba9a8c4108581eeba30ad984b2615(
+def _typecheckingstub__85086878bd5559f9bcb76f72ef7d39713a5dfe1a67404088b22a948985c5628d(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__816a4adb150a0a61973935b50fe3ad4cf68c614e4184b3ae204ed20a4f2768ee(
-    value: typing.Optional[DataProxmoxTemplateMemory],
+def _typecheckingstub__37ed7ef44a558b41c24319f430bd9d5e8e061f43edd93c6b14328bd6a508557c(
+    value: typing.Optional[DataProxmoxTemplatesTemplatesMemory],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__d4affaf046aecdcd0850cb64d1fd3be684aeaad4d6ea012096dfdf00dd5d890a(
+def _typecheckingstub__936967cce1c15f47cc61cad0804576959a9d43335f92de11fff9576904e2c633(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__286d6638f911e42cf08d10d1df09bb89c7b9e5ae901d0120eb2aa840c31c4a0c(
+def _typecheckingstub__737e30ba026c9167075fe33c1c2bd27a25ebda2df3ada8476ea562276b30e283(
     index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b98dd353b7d0a794e3df6c5bfa14a1c81e0b8ced4efa40dbaf0c54cb44a76205(
+def _typecheckingstub__48cef1cb379832d204d05e71200269648461a5d9b90d6210fd7323d5d5683d49(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__3072c672c8f942bc66a66b6147b2f01463e3f9fdb58332469031b4b76452899c(
+def _typecheckingstub__7a78040dc29e020dddb0be94997801ef14e00270db063f5d34e30354fa694ed1(
     value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__bd90e6a0216187386fcd8bc7edfdaa6fcca12336f19fcfc1d7cf6e583092e563(
+def _typecheckingstub__83fa36cc540531a6aa1ce8e8e244ee7b9cd0d2e5314e607e6bdb917be2c4cd9c(
     value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__bf24f3e52ac1ee2a2154a45e764132f705e7e629195695ae9ee0ea2eaecd394c(
+def _typecheckingstub__ca79e6840c22cc22b6a35edff39fed27bec20ff0729d3864153eda76572b6639(
+    terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
+    terraform_attribute: builtins.str,
+    complex_object_index: jsii.Number,
+    complex_object_is_from_set: builtins.bool,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__1c58d8361d95c8785388c651a8bef3bdef6a00dcdb17739df96e92e48f2667ca(
+    value: typing.Optional[DataProxmoxTemplatesTemplatesNetworkInterfaces],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__b202d7279af3d9819fdce569a9167c00ce44a03a626378a9a38f76286414bc81(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__8033212282867c593cf20f46be56c12ceb93404971dab446236dee4b3c4289b1(
-    value: typing.Optional[DataProxmoxTemplateNetworkInterfaces],
+def _typecheckingstub__6e3dc4c5d3942ba601d2415386e2de0a087c80913e1cfdafc5a86ecb25ca0683(
+    value: typing.Optional[DataProxmoxTemplatesTemplates],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__8f84e607ba3ff415d65f603a56a2c31c2cd3095793b7815bb964d56c8fdb2196(
+def _typecheckingstub__55717d97f120003fb6031ddd71985e3f4c5eab0344a8c0befa42a9c89633667d(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ec52f08bd041e7443d774e9d2822ad213552c49b0a731462f640bb960ccaafdf(
+def _typecheckingstub__569cf596a9a1d3ba8639edd9a452162acdb7b653adf57ee077a1dbb1de70be96(
     index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__d51157ff75882eb0c613abc4a7539579579f805674b7ba75f747166cfa6aa982(
+def _typecheckingstub__714ca5189a7e8b8efcba574865cb9541d6bb35e576329c8f5cbd05bfacafcd09(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a339abc46978c87a76cd443abebf11fe00e403b38389989b7934e8a7f8f24d43(
+def _typecheckingstub__400324fc47b84d680a8d6d870b00bcf22a76e01f2693f58a18e7bb03636c6f54(
     value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__9e56c0d9053713ded7ea08ca036217098c9a9846691b786af6f67e63338ed713(
+def _typecheckingstub__a314b4987d3ace06086de87977325702d27f5bba1ee500f931eb8285c6098fd2(
     value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__0a5b183d4c57837e9e4a9da4194da401e1fa320644c940b74d7c8d95ff4a54c3(
+def _typecheckingstub__42f0553ee26f760ca9dbe015a65d976a474040e167c3eb17a393b33cc0ce92c1(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__e9726e8994ee71310eff26984027fd5d3eeeb95bdc529a0e97af5772d4d21709(
-    value: typing.Optional[DataProxmoxTemplatePciDevices],
+def _typecheckingstub__1bb2963547ad5083d7060c4cf5df44ddaf83851eefd9ab93fb720702b84cc7ad(
+    value: typing.Optional[DataProxmoxTemplatesTemplatesPciDevices],
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_templates/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_virtual_machines/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `data_proxmox_templates`
+# `data_proxmox_virtual_machines`
 
-Refer to the Terraform Registory for docs: [`data_proxmox_templates`](https://www.terraform.io/docs/providers/proxmox/d/templates).
+Refer to the Terraform Registory for docs: [`data_proxmox_virtual_machines`](https://www.terraform.io/docs/providers/proxmox/d/virtual_machines).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,53 +17,53 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class DataProxmoxTemplates(
+class DataProxmoxVirtualMachines(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplates",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachines",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/proxmox/d/templates proxmox_templates}.'''
+    '''Represents a {@link https://www.terraform.io/docs/providers/proxmox/d/virtual_machines proxmox_virtual_machines}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        filters: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataProxmoxTemplatesFilters", typing.Dict[builtins.str, typing.Any]]]]] = None,
+        filters: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataProxmoxVirtualMachinesFilters", typing.Dict[builtins.str, typing.Any]]]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[jsii.Number] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/proxmox/d/templates proxmox_templates} Data Source.
+        '''Create a new {@link https://www.terraform.io/docs/providers/proxmox/d/virtual_machines proxmox_virtual_machines} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param filters: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/templates#filters DataProxmoxTemplates#filters}.
+        :param filters: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/virtual_machines#filters DataProxmoxVirtualMachines#filters}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__9c8f43a8ed4d9862bb2dfda7c754989b1621c88e999f35c8aa0300d8f6ba0675)
+            type_hints = typing.get_type_hints(_typecheckingstub__8964a502bdd6837bb34f855f2792c0696572ed85c989e789cc2e5b4121a36e07)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        config = DataProxmoxTemplatesConfig(
+        config = DataProxmoxVirtualMachinesConfig(
             filters=filters,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
@@ -71,21 +71,21 @@
         )
 
         jsii.create(self.__class__, self, [scope, id, config])
 
     @jsii.member(jsii_name="putFilters")
     def put_filters(
         self,
-        value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataProxmoxTemplatesFilters", typing.Dict[builtins.str, typing.Any]]]],
+        value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataProxmoxVirtualMachinesFilters", typing.Dict[builtins.str, typing.Any]]]],
     ) -> None:
         '''
         :param value: -
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__233a1989690e82037c4c9dc0c040be824ca0bc7ab5562170fe8918e4876b29f9)
+            type_hints = typing.get_type_hints(_typecheckingstub__234cf70c85efdb576bc5aeff6ef01db102e6418ab29585d697ac0a250b06fd30)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         return typing.cast(None, jsii.invoke(self, "putFilters", [value]))
 
     @jsii.member(jsii_name="resetFilters")
     def reset_filters(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetFilters", []))
 
@@ -96,71 +96,71 @@
     @jsii.python.classproperty
     @jsii.member(jsii_name="tfResourceType")
     def TF_RESOURCE_TYPE(cls) -> builtins.str:
         return typing.cast(builtins.str, jsii.sget(cls, "tfResourceType"))
 
     @builtins.property
     @jsii.member(jsii_name="filters")
-    def filters(self) -> "DataProxmoxTemplatesFiltersList":
-        return typing.cast("DataProxmoxTemplatesFiltersList", jsii.get(self, "filters"))
+    def filters(self) -> "DataProxmoxVirtualMachinesFiltersList":
+        return typing.cast("DataProxmoxVirtualMachinesFiltersList", jsii.get(self, "filters"))
 
     @builtins.property
-    @jsii.member(jsii_name="templates")
-    def templates(self) -> "DataProxmoxTemplatesTemplatesList":
-        return typing.cast("DataProxmoxTemplatesTemplatesList", jsii.get(self, "templates"))
+    @jsii.member(jsii_name="virtualMachines")
+    def virtual_machines(self) -> "DataProxmoxVirtualMachinesVirtualMachinesList":
+        return typing.cast("DataProxmoxVirtualMachinesVirtualMachinesList", jsii.get(self, "virtualMachines"))
 
     @builtins.property
     @jsii.member(jsii_name="filtersInput")
     def filters_input(
         self,
-    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataProxmoxTemplatesFilters"]]]:
-        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataProxmoxTemplatesFilters"]]], jsii.get(self, "filtersInput"))
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataProxmoxVirtualMachinesFilters"]]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataProxmoxVirtualMachinesFilters"]]], jsii.get(self, "filtersInput"))
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesConfig",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "filters": "filters",
     },
 )
-class DataProxmoxTemplatesConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class DataProxmoxVirtualMachinesConfig(_cdktf_9a9027ec.TerraformMetaArguments):
     def __init__(
         self,
         *,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
         count: typing.Optional[jsii.Number] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-        filters: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataProxmoxTemplatesFilters", typing.Dict[builtins.str, typing.Any]]]]] = None,
+        filters: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataProxmoxVirtualMachinesFilters", typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
         '''
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param filters: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/templates#filters DataProxmoxTemplates#filters}.
+        :param filters: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/virtual_machines#filters DataProxmoxVirtualMachines#filters}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4b9b87d43a9822a28f232fcb57074d7978bca6aa140657b9397ad2bf3cabac68)
+            type_hints = typing.get_type_hints(_typecheckingstub__0c1f1b06e874d1f8d6204299e031aa4b0e420c44cbc8804b2a401a388c11d270)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
@@ -244,182 +244,185 @@
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def filters(
         self,
-    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataProxmoxTemplatesFilters"]]]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/templates#filters DataProxmoxTemplates#filters}.'''
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataProxmoxVirtualMachinesFilters"]]]:
+        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/virtual_machines#filters DataProxmoxVirtualMachines#filters}.'''
         result = self._values.get("filters")
-        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataProxmoxTemplatesFilters"]]], result)
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataProxmoxVirtualMachinesFilters"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesConfig(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesFilters",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesFilters",
     jsii_struct_bases=[],
     name_mapping={"name": "name", "values": "values"},
 )
-class DataProxmoxTemplatesFilters:
+class DataProxmoxVirtualMachinesFilters:
     def __init__(
         self,
         *,
         name: builtins.str,
         values: typing.Sequence[builtins.str],
     ) -> None:
         '''
-        :param name: The name of the attribute to filter on. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/templates#name DataProxmoxTemplates#name}
-        :param values: The value(s) to be used in the filter. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/templates#values DataProxmoxTemplates#values}
+        :param name: The name of the attribute to filter on. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/virtual_machines#name DataProxmoxVirtualMachines#name}
+        :param values: The value(s) to be used in the filter. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/virtual_machines#values DataProxmoxVirtualMachines#values}
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7b5a2e2e69a8b272223cae04497ef0e50f1388bd002ce5d48b07318623fc0fd0)
+            type_hints = typing.get_type_hints(_typecheckingstub__859c03e5becb1d85fc603cba6f0b2225308fdef7e7962a6a5c17fd27c6ae0c64)
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument values", value=values, expected_type=type_hints["values"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "name": name,
             "values": values,
         }
 
     @builtins.property
     def name(self) -> builtins.str:
         '''The name of the attribute to filter on.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/templates#name DataProxmoxTemplates#name}
+        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/virtual_machines#name DataProxmoxVirtualMachines#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def values(self) -> typing.List[builtins.str]:
         '''The value(s) to be used in the filter.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/templates#values DataProxmoxTemplates#values}
+        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/proxmox/d/virtual_machines#values DataProxmoxVirtualMachines#values}
         '''
         result = self._values.get("values")
         assert result is not None, "Required property 'values' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesFilters(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesFilters(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplatesFiltersList(
+class DataProxmoxVirtualMachinesFiltersList(
     _cdktf_9a9027ec.ComplexList,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesFiltersList",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesFiltersList",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         wraps_set: builtins.bool,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7185592ee5df14f6502caf1b02c1c8f7f1a998c262a921b4059ae73ed17d01f7)
+            type_hints = typing.get_type_hints(_typecheckingstub__3355cff5bd7377db4300269580da8f8240b6d258eabd8dcdf80d03d8088f28b6)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
 
     @jsii.member(jsii_name="get")
-    def get(self, index: jsii.Number) -> "DataProxmoxTemplatesFiltersOutputReference":
+    def get(
+        self,
+        index: jsii.Number,
+    ) -> "DataProxmoxVirtualMachinesFiltersOutputReference":
         '''
         :param index: the index of the item to return.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b3e0e2fef1c0a4b8e2a1b64ae525d2b0ac767a60597d7eb6476cf5a4b328eb58)
+            type_hints = typing.get_type_hints(_typecheckingstub__073eda288224fca974ec6f12f1acfceb54b74c646aa6900e74c182cdd68d85fc)
             check_type(argname="argument index", value=index, expected_type=type_hints["index"])
-        return typing.cast("DataProxmoxTemplatesFiltersOutputReference", jsii.invoke(self, "get", [index]))
+        return typing.cast("DataProxmoxVirtualMachinesFiltersOutputReference", jsii.invoke(self, "get", [index]))
 
     @builtins.property
     @jsii.member(jsii_name="terraformAttribute")
     def _terraform_attribute(self) -> builtins.str:
         '''The attribute on the parent resource this class is referencing.'''
         return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
 
     @_terraform_attribute.setter
     def _terraform_attribute(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__12203107c9a9b5812061df83af59f971166e12e0dd3c53822898b587c4a13a1a)
+            type_hints = typing.get_type_hints(_typecheckingstub__faf20181ed0e23ef3f5bc1692ab7494a10eaa85c8edab3ac4f4a93d7e57140b3)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformAttribute", value)
 
     @builtins.property
     @jsii.member(jsii_name="terraformResource")
     def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
         '''The parent resource.'''
         return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
 
     @_terraform_resource.setter
     def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7c18c8f27f5b5749f0930032ce59cf9aa9dd8c3fe11454a21edfacfb39110484)
+            type_hints = typing.get_type_hints(_typecheckingstub__c25a6c623b61b177f9bf2f54fae6101d56d21e9edcf027abe9691b547bab6791)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformResource", value)
 
     @builtins.property
     @jsii.member(jsii_name="wrapsSet")
     def _wraps_set(self) -> builtins.bool:
         '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
         return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
 
     @_wraps_set.setter
     def _wraps_set(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1de467d3e8e92a1d8d17a81042c85e45ddb8a5f8a574026c01b38410619c435e)
+            type_hints = typing.get_type_hints(_typecheckingstub__1b039d1c7ee0a20c37735d707128147ad27c3b2066a142a8245801abfab54760)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wrapsSet", value)
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataProxmoxTemplatesFilters]]]:
-        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataProxmoxTemplatesFilters]]], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataProxmoxVirtualMachinesFilters]]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataProxmoxVirtualMachinesFilters]]], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataProxmoxTemplatesFilters]]],
+        value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataProxmoxVirtualMachinesFilters]]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4eeb8042fe9f97bb3b08f79bdd3f5544c61ad333e13f34069ee25b3925b85f8c)
+            type_hints = typing.get_type_hints(_typecheckingstub__de90626d8d6cb4f51e48e76cc780e64af3308dcb4a9387bacd68d9acaefcd3d9)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
-class DataProxmoxTemplatesFiltersOutputReference(
+class DataProxmoxVirtualMachinesFiltersOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesFiltersOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesFiltersOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         complex_object_index: jsii.Number,
         complex_object_is_from_set: builtins.bool,
@@ -427,15 +430,15 @@
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param complex_object_index: the index of this item in the list.
         :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8327cf5bac96b9877733ed3b92c5e728be3a17f989a4bdbaf2900a291c81f07d)
+            type_hints = typing.get_type_hints(_typecheckingstub__e17bdc6aba401b91212b88e17b905a71eb22c22d50f7b0ed5fce967f8502ff54)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
@@ -452,106 +455,106 @@
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
     @name.setter
     def name(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__16f3ef7637865b9efbe01d5d61b463f735bae38264ad57354abdbce513208aef)
+            type_hints = typing.get_type_hints(_typecheckingstub__d16c453aabbc842f9d9270513abd49f9d0512710bfe08e8f3ec0aa4580a67f7e)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "name", value)
 
     @builtins.property
     @jsii.member(jsii_name="values")
     def values(self) -> typing.List[builtins.str]:
         return typing.cast(typing.List[builtins.str], jsii.get(self, "values"))
 
     @values.setter
     def values(self, value: typing.List[builtins.str]) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8a7dc4004f107546dc9c621fa798620b5001c0fd8917d4c9140a0ad48064ed70)
+            type_hints = typing.get_type_hints(_typecheckingstub__d0f24eea4504bd90493c0ddea1d0a515f1b6835969b6e9ef6601c0e4f4b91c1e)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "values", value)
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[typing.Union[DataProxmoxTemplatesFilters, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[DataProxmoxTemplatesFilters, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[typing.Union[DataProxmoxVirtualMachinesFilters, _cdktf_9a9027ec.IResolvable]]:
+        return typing.cast(typing.Optional[typing.Union[DataProxmoxVirtualMachinesFilters, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[typing.Union[DataProxmoxTemplatesFilters, _cdktf_9a9027ec.IResolvable]],
+        value: typing.Optional[typing.Union[DataProxmoxVirtualMachinesFilters, _cdktf_9a9027ec.IResolvable]],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__dec6db530ef281b602f64ed73e330e24906e6e0c6b954683c5ba96b7ad21dcbf)
+            type_hints = typing.get_type_hints(_typecheckingstub__111b39294ca1a0f53214e63c1951305a9a858d7c6b49427b8f31cc150dea7cfc)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplates",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachines",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatesTemplates:
+class DataProxmoxVirtualMachinesVirtualMachines:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesTemplates(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesVirtualMachines(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesAgent",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesAgent",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatesTemplatesAgent:
+class DataProxmoxVirtualMachinesVirtualMachinesAgent:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesTemplatesAgent(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesVirtualMachinesAgent(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplatesTemplatesAgentOutputReference(
+class DataProxmoxVirtualMachinesVirtualMachinesAgentOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesAgentOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesAgentOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__673e66db611a5fbc4e59ce825f6e4416fa82cbf66904ba65202f13a93beb37d2)
+            type_hints = typing.get_type_hints(_typecheckingstub__07d113599c3ded151ad319677ae0805061bedb2e53dc395f36e38892a1732956)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="enabled")
     def enabled(self) -> _cdktf_9a9027ec.IResolvable:
@@ -565,86 +568,88 @@
     @builtins.property
     @jsii.member(jsii_name="useFstrim")
     def use_fstrim(self) -> _cdktf_9a9027ec.IResolvable:
         return typing.cast(_cdktf_9a9027ec.IResolvable, jsii.get(self, "useFstrim"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplatesTemplatesAgent]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesAgent], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesAgent]:
+        return typing.cast(typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesAgent], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatesTemplatesAgent],
+        value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesAgent],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__11571a58fd163ae522f420d6c0dff17873e68251c637a1ebc2f4261d40a0908e)
+            type_hints = typing.get_type_hints(_typecheckingstub__8c6a7e94ae13a6fe6d8277fee1493d5adf31562cf476d3edea88cdb28b4b5f09)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInit",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCloudInit",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatesTemplatesCloudInit:
+class DataProxmoxVirtualMachinesVirtualMachinesCloudInit:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesTemplatesCloudInit(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesVirtualMachinesCloudInit(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitDns",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCloudInitDns",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatesTemplatesCloudInitDns:
+class DataProxmoxVirtualMachinesVirtualMachinesCloudInitDns:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesTemplatesCloudInitDns(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesVirtualMachinesCloudInitDns(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplatesTemplatesCloudInitDnsOutputReference(
+class DataProxmoxVirtualMachinesVirtualMachinesCloudInitDnsOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitDnsOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCloudInitDnsOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e067c9db4e634da658b56ee80ca7edfde446f1a440b47d1f6eb546e326a67b26)
+            type_hints = typing.get_type_hints(_typecheckingstub__2290f2bcf49b3f5380318f104b1ae2747c259487d97ca061b5a305da54bfe390)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="domain")
     def domain(self) -> builtins.str:
@@ -655,129 +660,129 @@
     def nameserver(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "nameserver"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[DataProxmoxTemplatesTemplatesCloudInitDns]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesCloudInitDns], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitDns]:
+        return typing.cast(typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitDns], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitDns],
+        value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitDns],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0782611e20910ed665dc0d5e84a3f71452ba5bade5ae664490668cd11d64b023)
+            type_hints = typing.get_type_hints(_typecheckingstub__0c58e16081384a2f723727787e4cc8068349196e637a1f457896308290b1557f)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitIp",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCloudInitIp",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatesTemplatesCloudInitIp:
+class DataProxmoxVirtualMachinesVirtualMachinesCloudInitIp:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesTemplatesCloudInitIp(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesVirtualMachinesCloudInitIp(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplatesTemplatesCloudInitIpList(
+class DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpList(
     _cdktf_9a9027ec.ComplexList,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitIpList",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpList",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         wraps_set: builtins.bool,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__99f203b02f9592f1a1fb7a64a5635c720b9dd6c7f992bc56e8edb0bab0e63ae7)
+            type_hints = typing.get_type_hints(_typecheckingstub__670bc4d8280f028c77ea09b2abed573c41ec7f36c2783c71af8f86efb9c064b3)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
 
     @jsii.member(jsii_name="get")
     def get(
         self,
         index: jsii.Number,
-    ) -> "DataProxmoxTemplatesTemplatesCloudInitIpOutputReference":
+    ) -> "DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpOutputReference":
         '''
         :param index: the index of the item to return.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__17abca3a5e9277181468d701c2550bed8e6e1d101cde67b7c64c5bf22a976a80)
+            type_hints = typing.get_type_hints(_typecheckingstub__4f2cb10553da29016ece8d9bd3802ddfc4ad73c134c0b0390ff9883c5d145d3c)
             check_type(argname="argument index", value=index, expected_type=type_hints["index"])
-        return typing.cast("DataProxmoxTemplatesTemplatesCloudInitIpOutputReference", jsii.invoke(self, "get", [index]))
+        return typing.cast("DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpOutputReference", jsii.invoke(self, "get", [index]))
 
     @builtins.property
     @jsii.member(jsii_name="terraformAttribute")
     def _terraform_attribute(self) -> builtins.str:
         '''The attribute on the parent resource this class is referencing.'''
         return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
 
     @_terraform_attribute.setter
     def _terraform_attribute(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8f5acfd27a377920da103fd958e5f6b4dbf0ed9b81ad89a5f0293c850734683d)
+            type_hints = typing.get_type_hints(_typecheckingstub__65ae18e026db7c863074d3aec87b67584f61d4014aff3434aa5bc2ea8c97a9bf)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformAttribute", value)
 
     @builtins.property
     @jsii.member(jsii_name="terraformResource")
     def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
         '''The parent resource.'''
         return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
 
     @_terraform_resource.setter
     def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4ab6c78fc6f14f4f992d620cd01deffae673cfc19cb90a2b3a92306efc35ecdc)
+            type_hints = typing.get_type_hints(_typecheckingstub__b951ce6319261e9a74ca61b8cb0c6e32dc7a56176d2ffe94e46f6e9de731b12f)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformResource", value)
 
     @builtins.property
     @jsii.member(jsii_name="wrapsSet")
     def _wraps_set(self) -> builtins.bool:
         '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
         return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
 
     @_wraps_set.setter
     def _wraps_set(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d95d53ee35c350fc80dac6a96148f86fabee41b7110a6853b4b1a4f0a5d8f0c7)
+            type_hints = typing.get_type_hints(_typecheckingstub__224b885742822d9f056ed325941e555baa7b112c1ba45bbda98fb61767292b1e)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wrapsSet", value)
 
 
-class DataProxmoxTemplatesTemplatesCloudInitIpOutputReference(
+class DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitIpOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         complex_object_index: jsii.Number,
         complex_object_is_from_set: builtins.bool,
@@ -785,91 +790,95 @@
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param complex_object_index: the index of this item in the list.
         :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__bd10d7eba8b193e54bbf14d276b04c99e46b2cdd97d9ee8c3b3b5574420a6e07)
+            type_hints = typing.get_type_hints(_typecheckingstub__b3415898b0a5f21c0e71a645d890d0f7d0b5d0671b8c1365c8f61e3eb7110c73)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
     @jsii.member(jsii_name="position")
     def position(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "position"))
 
     @builtins.property
     @jsii.member(jsii_name="v4")
-    def v4(self) -> "DataProxmoxTemplatesTemplatesCloudInitIpV4OutputReference":
-        return typing.cast("DataProxmoxTemplatesTemplatesCloudInitIpV4OutputReference", jsii.get(self, "v4"))
+    def v4(
+        self,
+    ) -> "DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV4OutputReference":
+        return typing.cast("DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV4OutputReference", jsii.get(self, "v4"))
 
     @builtins.property
     @jsii.member(jsii_name="v6")
-    def v6(self) -> "DataProxmoxTemplatesTemplatesCloudInitIpV6OutputReference":
-        return typing.cast("DataProxmoxTemplatesTemplatesCloudInitIpV6OutputReference", jsii.get(self, "v6"))
+    def v6(
+        self,
+    ) -> "DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV6OutputReference":
+        return typing.cast("DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV6OutputReference", jsii.get(self, "v6"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIp]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIp], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitIp]:
+        return typing.cast(typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitIp], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIp],
+        value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitIp],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c6edec7bf9da7fc858d6f00b1a2bca916dd1537601759f0547eecdabfc5fd9dd)
+            type_hints = typing.get_type_hints(_typecheckingstub__34bffe777ebd3bc403935e1b2d49c4491a3aae7a692ba76e9ff55d600a37d857)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitIpV4",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV4",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatesTemplatesCloudInitIpV4:
+class DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV4:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesTemplatesCloudInitIpV4(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV4(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplatesTemplatesCloudInitIpV4OutputReference(
+class DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV4OutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitIpV4OutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV4OutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__489e948956a30a57fae7529bdc147f4aca6ac2e350685a9c13f1011adf371d56)
+            type_hints = typing.get_type_hints(_typecheckingstub__08d9485cead65b2fbe96f1195e36008437795435c6e8f41337038c24d0a97560)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="address")
     def address(self) -> builtins.str:
@@ -890,65 +899,65 @@
     def netmask(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "netmask"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV4]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV4], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV4]:
+        return typing.cast(typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV4], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV4],
+        value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV4],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__316b4ac8b088bec9d0a20b18732922b3c4f2ec34c73423ab7110590748dc5151)
+            type_hints = typing.get_type_hints(_typecheckingstub__b35dc38c3cc9bb23db7099cb8254112e1dcbf68252cf23cbd4b42e4fec6db0c3)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitIpV6",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV6",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatesTemplatesCloudInitIpV6:
+class DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV6:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesTemplatesCloudInitIpV6(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV6(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplatesTemplatesCloudInitIpV6OutputReference(
+class DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV6OutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitIpV6OutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV6OutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__794b5f9374ea15e16167c1ac262a044629688c6c6d472d93a73026f2902c9054)
+            type_hints = typing.get_type_hints(_typecheckingstub__e09b2a2eade5c5be811c9310d90f28a5cbe6719ef4799f52c57bd93061aa88e2)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="address")
     def address(self) -> builtins.str:
@@ -969,116 +978,122 @@
     def netmask(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "netmask"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV6]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV6], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV6]:
+        return typing.cast(typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV6], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV6],
+        value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV6],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ff35973d8191c68c6e6ff6f7e9a4b46f7fb17e1b8800426dcf85ae2efb76e925)
+            type_hints = typing.get_type_hints(_typecheckingstub__055bb09a1452519595b570d7f5ed45e2c0e738e1f38219d8581999a79946e921)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
-class DataProxmoxTemplatesTemplatesCloudInitOutputReference(
+class DataProxmoxVirtualMachinesVirtualMachinesCloudInitOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCloudInitOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__29f4c65f37a567f10935f4c966639f7bdf80838af210c4911049934a056a8f50)
+            type_hints = typing.get_type_hints(_typecheckingstub__81b259dda29c3f040d46b4f55c59e9cc7915255bbc6f8bd9fe0e8c46fa9dc447)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="dns")
-    def dns(self) -> DataProxmoxTemplatesTemplatesCloudInitDnsOutputReference:
-        return typing.cast(DataProxmoxTemplatesTemplatesCloudInitDnsOutputReference, jsii.get(self, "dns"))
+    def dns(
+        self,
+    ) -> DataProxmoxVirtualMachinesVirtualMachinesCloudInitDnsOutputReference:
+        return typing.cast(DataProxmoxVirtualMachinesVirtualMachinesCloudInitDnsOutputReference, jsii.get(self, "dns"))
 
     @builtins.property
     @jsii.member(jsii_name="ip")
-    def ip(self) -> DataProxmoxTemplatesTemplatesCloudInitIpList:
-        return typing.cast(DataProxmoxTemplatesTemplatesCloudInitIpList, jsii.get(self, "ip"))
+    def ip(self) -> DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpList:
+        return typing.cast(DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpList, jsii.get(self, "ip"))
 
     @builtins.property
     @jsii.member(jsii_name="user")
-    def user(self) -> "DataProxmoxTemplatesTemplatesCloudInitUserOutputReference":
-        return typing.cast("DataProxmoxTemplatesTemplatesCloudInitUserOutputReference", jsii.get(self, "user"))
+    def user(
+        self,
+    ) -> "DataProxmoxVirtualMachinesVirtualMachinesCloudInitUserOutputReference":
+        return typing.cast("DataProxmoxVirtualMachinesVirtualMachinesCloudInitUserOutputReference", jsii.get(self, "user"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplatesTemplatesCloudInit]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesCloudInit], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInit]:
+        return typing.cast(typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInit], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInit],
+        value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInit],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4aef00a6fe7514158fcad983bbd4c46da783c27bccbf0aeeb7e342ba5ce802b8)
+            type_hints = typing.get_type_hints(_typecheckingstub__6d252ed48a14f6a7171a01ba9bcaddfdfe37577ad4a546c42f2f20f96b94cb34)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitUser",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCloudInitUser",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatesTemplatesCloudInitUser:
+class DataProxmoxVirtualMachinesVirtualMachinesCloudInitUser:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesTemplatesCloudInitUser(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesVirtualMachinesCloudInitUser(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplatesTemplatesCloudInitUserOutputReference(
+class DataProxmoxVirtualMachinesVirtualMachinesCloudInitUserOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCloudInitUserOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCloudInitUserOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ab97a5c9497e31ad13315c518709649341b3f92644baa1db3ad03d0e7724a704)
+            type_hints = typing.get_type_hints(_typecheckingstub__63293903413c405b49ccc38a464d0226844a76004821eea7f5ca5ee351482ea9)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
@@ -1094,65 +1109,65 @@
     def public_keys(self) -> typing.List[builtins.str]:
         return typing.cast(typing.List[builtins.str], jsii.get(self, "publicKeys"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[DataProxmoxTemplatesTemplatesCloudInitUser]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesCloudInitUser], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitUser]:
+        return typing.cast(typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitUser], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitUser],
+        value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitUser],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__40a73c62c87638712e722cd3fd3f967956c8dabb50c0d76987263c31322adf9f)
+            type_hints = typing.get_type_hints(_typecheckingstub__f8544ddcf0efba56064233ae8312df8b7a7fe49ce90b4652f9783fb89b84da08)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCpu",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCpu",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatesTemplatesCpu:
+class DataProxmoxVirtualMachinesVirtualMachinesCpu:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesTemplatesCpu(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesVirtualMachinesCpu(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplatesTemplatesCpuOutputReference(
+class DataProxmoxVirtualMachinesVirtualMachinesCpuOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesCpuOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesCpuOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a5a42158ebc03e71f8f9bdc4ad6b1258c5fe9acbd56ba299f3e2fdabdf3cd633)
+            type_hints = typing.get_type_hints(_typecheckingstub__1958f45b6ab064186f301d8386335e8c83f22a4ccdcbca2e6ae54f2f6ef983eb)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="architecture")
     def architecture(self) -> builtins.str:
@@ -1176,129 +1191,131 @@
     @builtins.property
     @jsii.member(jsii_name="sockets")
     def sockets(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "sockets"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplatesTemplatesCpu]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesCpu], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCpu]:
+        return typing.cast(typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCpu], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatesTemplatesCpu],
+        value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCpu],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fb0f4d2eadaa9e4d99b7a9686d56e4d9532194127cf03192619771e2ef651831)
+            type_hints = typing.get_type_hints(_typecheckingstub__e9b7f41bb0798211787e68a31b1c7daf4153c5dbfd489800215834eff544b1e8)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesDisks",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesDisks",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatesTemplatesDisks:
+class DataProxmoxVirtualMachinesVirtualMachinesDisks:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesTemplatesDisks(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesVirtualMachinesDisks(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplatesTemplatesDisksList(
+class DataProxmoxVirtualMachinesVirtualMachinesDisksList(
     _cdktf_9a9027ec.ComplexList,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesDisksList",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesDisksList",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         wraps_set: builtins.bool,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__d5f5bf449c9309a6b5d5c6b7f49c07b04a79a2c1c99b5c48638d61eb31622e7c)
+            type_hints = typing.get_type_hints(_typecheckingstub__0c98fbaa0b49269b0c90284fe1740e24d2e9379e844cce804635729047fb09ec)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
 
     @jsii.member(jsii_name="get")
     def get(
         self,
         index: jsii.Number,
-    ) -> "DataProxmoxTemplatesTemplatesDisksOutputReference":
+    ) -> "DataProxmoxVirtualMachinesVirtualMachinesDisksOutputReference":
         '''
         :param index: the index of the item to return.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__8b683a39926cfaa60ef131b3061711541f522c4102ea45f5688bdc06bf9edb19)
+            type_hints = typing.get_type_hints(_typecheckingstub__621e7f7977ebf33a08e0572e42b38746107f67ad9f7e30180350b831a74ba3b8)
             check_type(argname="argument index", value=index, expected_type=type_hints["index"])
-        return typing.cast("DataProxmoxTemplatesTemplatesDisksOutputReference", jsii.invoke(self, "get", [index]))
+        return typing.cast("DataProxmoxVirtualMachinesVirtualMachinesDisksOutputReference", jsii.invoke(self, "get", [index]))
 
     @builtins.property
     @jsii.member(jsii_name="terraformAttribute")
     def _terraform_attribute(self) -> builtins.str:
         '''The attribute on the parent resource this class is referencing.'''
         return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
 
     @_terraform_attribute.setter
     def _terraform_attribute(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1ceab6297650a2d7fe87e70d5e2c1bc0179b8edd69ebcbea2d28f2d3254a7cf9)
+            type_hints = typing.get_type_hints(_typecheckingstub__d460fd02ce4f7b52c6f03034fbdaed0dacf058481f77c05e66bfac805177d900)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformAttribute", value)
 
     @builtins.property
     @jsii.member(jsii_name="terraformResource")
     def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
         '''The parent resource.'''
         return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
 
     @_terraform_resource.setter
     def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0ac4b2edba5a1f5d58b921e4fd12222646c78eac69326d2f9d9cb8cfdf5293f0)
+            type_hints = typing.get_type_hints(_typecheckingstub__cba26de2b6e3232d042a73ac8f07e30ad776b9843de6d2b3f287e4ae2105ca6c)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformResource", value)
 
     @builtins.property
     @jsii.member(jsii_name="wrapsSet")
     def _wraps_set(self) -> builtins.bool:
         '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
         return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
 
     @_wraps_set.setter
     def _wraps_set(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3681c1aed5886b3362ddc27a0c8a45545916b1eea3d5c5525293ae002562a24a)
+            type_hints = typing.get_type_hints(_typecheckingstub__566d4ee1321afb3df335ecaedb5bfd22d08474ad70cc1ed97b042a2cefbceb5a)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wrapsSet", value)
 
 
-class DataProxmoxTemplatesTemplatesDisksOutputReference(
+class DataProxmoxVirtualMachinesVirtualMachinesDisksOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesDisksOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesDisksOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         complex_object_index: jsii.Number,
         complex_object_is_from_set: builtins.bool,
@@ -1306,15 +1323,15 @@
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param complex_object_index: the index of this item in the list.
         :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e36693344440afa8e05cd759d3059d6580174e1078ac7d475b89fa21b4348697)
+            type_hints = typing.get_type_hints(_typecheckingstub__b32e086fb26b23e3a898946ad7abc208af97ba9cc58ae594736dce1bf2550777)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
@@ -1329,34 +1346,29 @@
 
     @builtins.property
     @jsii.member(jsii_name="interfaceType")
     def interface_type(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "interfaceType"))
 
     @builtins.property
-    @jsii.member(jsii_name="name")
-    def name(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "name"))
-
-    @builtins.property
     @jsii.member(jsii_name="position")
     def position(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "position"))
 
     @builtins.property
     @jsii.member(jsii_name="size")
     def size(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "size"))
 
     @builtins.property
     @jsii.member(jsii_name="speedLimits")
     def speed_limits(
         self,
-    ) -> "DataProxmoxTemplatesTemplatesDisksSpeedLimitsOutputReference":
-        return typing.cast("DataProxmoxTemplatesTemplatesDisksSpeedLimitsOutputReference", jsii.get(self, "speedLimits"))
+    ) -> "DataProxmoxVirtualMachinesVirtualMachinesDisksSpeedLimitsOutputReference":
+        return typing.cast("DataProxmoxVirtualMachinesVirtualMachinesDisksSpeedLimitsOutputReference", jsii.get(self, "speedLimits"))
 
     @builtins.property
     @jsii.member(jsii_name="ssdEmulation")
     def ssd_emulation(self) -> _cdktf_9a9027ec.IResolvable:
         return typing.cast(_cdktf_9a9027ec.IResolvable, jsii.get(self, "ssdEmulation"))
 
     @builtins.property
@@ -1367,65 +1379,67 @@
     @builtins.property
     @jsii.member(jsii_name="useIothread")
     def use_iothread(self) -> _cdktf_9a9027ec.IResolvable:
         return typing.cast(_cdktf_9a9027ec.IResolvable, jsii.get(self, "useIothread"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplatesTemplatesDisks]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesDisks], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesDisks]:
+        return typing.cast(typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesDisks], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatesTemplatesDisks],
+        value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesDisks],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__3411d4f953ea91029177b1db6c9690297978a4c8aa4f1a064ccb2be6d9a0219e)
+            type_hints = typing.get_type_hints(_typecheckingstub__2cbd5d298cdb62f85ba547df49f0fd65bc3f4591d25afc720b2ef4224ddb1abb)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesDisksSpeedLimits",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesDisksSpeedLimits",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatesTemplatesDisksSpeedLimits:
+class DataProxmoxVirtualMachinesVirtualMachinesDisksSpeedLimits:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesTemplatesDisksSpeedLimits(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesVirtualMachinesDisksSpeedLimits(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplatesTemplatesDisksSpeedLimitsOutputReference(
+class DataProxmoxVirtualMachinesVirtualMachinesDisksSpeedLimitsOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesDisksSpeedLimitsOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesDisksSpeedLimitsOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6507fc59ef695082c0ae01339c5f249d975700e498b4e18908c1eafa158d19f8)
+            type_hints = typing.get_type_hints(_typecheckingstub__46c7a5b1e39db160d2904fcfa03bd458875cd05b01a4c0852fe8b0a2db0d471c)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="read")
     def read(self) -> jsii.Number:
@@ -1446,138 +1460,141 @@
     def write_burstable(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "writeBurstable"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[DataProxmoxTemplatesTemplatesDisksSpeedLimits]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesDisksSpeedLimits], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesDisksSpeedLimits]:
+        return typing.cast(typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesDisksSpeedLimits], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatesTemplatesDisksSpeedLimits],
+        value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesDisksSpeedLimits],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c18f8c7ed8d24d2b06774c7cd39f86063e0c0dd2b09ba5b07796c7ebbfa6b319)
+            type_hints = typing.get_type_hints(_typecheckingstub__131284fb30fe862c25a9c2aa553cf871875637fbe865e221adeec2521470c8c9)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
-class DataProxmoxTemplatesTemplatesList(
+class DataProxmoxVirtualMachinesVirtualMachinesList(
     _cdktf_9a9027ec.ComplexList,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesList",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesList",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         wraps_set: builtins.bool,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0f08ad26095875cedb140ea7fee38d064da3ca7274d935b385b43bee3f8e0224)
+            type_hints = typing.get_type_hints(_typecheckingstub__980cd4eb86098e6866bb8dc40d7238744a84f546e0824b3fc6c6e3c6a5237fd1)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
 
     @jsii.member(jsii_name="get")
-    def get(self, index: jsii.Number) -> "DataProxmoxTemplatesTemplatesOutputReference":
+    def get(
+        self,
+        index: jsii.Number,
+    ) -> "DataProxmoxVirtualMachinesVirtualMachinesOutputReference":
         '''
         :param index: the index of the item to return.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a73b9f8ad3ee64bf1330033bbb94eda72651474ebf3cc08f02fdb5164474837f)
+            type_hints = typing.get_type_hints(_typecheckingstub__0cfd1aa70ee72623f0979da97640b25f0737a55548794f1f93d0ff21ae2b1e0c)
             check_type(argname="argument index", value=index, expected_type=type_hints["index"])
-        return typing.cast("DataProxmoxTemplatesTemplatesOutputReference", jsii.invoke(self, "get", [index]))
+        return typing.cast("DataProxmoxVirtualMachinesVirtualMachinesOutputReference", jsii.invoke(self, "get", [index]))
 
     @builtins.property
     @jsii.member(jsii_name="terraformAttribute")
     def _terraform_attribute(self) -> builtins.str:
         '''The attribute on the parent resource this class is referencing.'''
         return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
 
     @_terraform_attribute.setter
     def _terraform_attribute(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__848480b079fffd0ff9a7f3a525600012d4afc4dee5881b91ae5e7167dbb59566)
+            type_hints = typing.get_type_hints(_typecheckingstub__40e6af369bd325ebd038a49265102cdb8b5c4cb027266754f3d7cb2130d214bf)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformAttribute", value)
 
     @builtins.property
     @jsii.member(jsii_name="terraformResource")
     def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
         '''The parent resource.'''
         return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
 
     @_terraform_resource.setter
     def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__fa2c9ff301f9aee5b2b11bbfc41fe82846b8379b5d0938c0623854abf252aa3c)
+            type_hints = typing.get_type_hints(_typecheckingstub__6f5f8973a8d38e1ea26c40da9379f115f36db1c2cab24f96811a0809c52ec2b2)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformResource", value)
 
     @builtins.property
     @jsii.member(jsii_name="wrapsSet")
     def _wraps_set(self) -> builtins.bool:
         '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
         return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
 
     @_wraps_set.setter
     def _wraps_set(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__abebb6092537f032ac958ea0c960b43351ae38dc63f45c0caf96a643d0c578a2)
+            type_hints = typing.get_type_hints(_typecheckingstub__0a68d92988fcfdfa3ffdab3821127b4709402e1f83e08ba3e721786afcffa9cf)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wrapsSet", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesMemory",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesMemory",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatesTemplatesMemory:
+class DataProxmoxVirtualMachinesVirtualMachinesMemory:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesTemplatesMemory(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesVirtualMachinesMemory(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplatesTemplatesMemoryOutputReference(
+class DataProxmoxVirtualMachinesVirtualMachinesMemoryOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesMemoryOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesMemoryOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__85086878bd5559f9bcb76f72ef7d39713a5dfe1a67404088b22a948985c5628d)
+            type_hints = typing.get_type_hints(_typecheckingstub__5a1e71e78d36120a049bc9b4d3809b891cd651b04445ad5e19fcb5debcfb94b2)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute])
 
     @builtins.property
     @jsii.member(jsii_name="dedicated")
     def dedicated(self) -> jsii.Number:
@@ -1591,129 +1608,131 @@
     @builtins.property
     @jsii.member(jsii_name="shared")
     def shared(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "shared"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplatesTemplatesMemory]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesMemory], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesMemory]:
+        return typing.cast(typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesMemory], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatesTemplatesMemory],
+        value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesMemory],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__37ed7ef44a558b41c24319f430bd9d5e8e061f43edd93c6b14328bd6a508557c)
+            type_hints = typing.get_type_hints(_typecheckingstub__bda3dbfa79f54ba4a1f9943f6b812bd81885f1c2aae1e6268c893b56b1e5d676)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesNetworkInterfaces",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfaces",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatesTemplatesNetworkInterfaces:
+class DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfaces:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesTemplatesNetworkInterfaces(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfaces(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplatesTemplatesNetworkInterfacesList(
+class DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfacesList(
     _cdktf_9a9027ec.ComplexList,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesNetworkInterfacesList",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfacesList",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         wraps_set: builtins.bool,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__936967cce1c15f47cc61cad0804576959a9d43335f92de11fff9576904e2c633)
+            type_hints = typing.get_type_hints(_typecheckingstub__795a0e16e037136dc5720eda98344143c0c93fe5e7a9a9f58519e0b4c41505c2)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
 
     @jsii.member(jsii_name="get")
     def get(
         self,
         index: jsii.Number,
-    ) -> "DataProxmoxTemplatesTemplatesNetworkInterfacesOutputReference":
+    ) -> "DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfacesOutputReference":
         '''
         :param index: the index of the item to return.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__737e30ba026c9167075fe33c1c2bd27a25ebda2df3ada8476ea562276b30e283)
+            type_hints = typing.get_type_hints(_typecheckingstub__d05a397d7edbf4a67ada5f47bc2c66f1d64e6817f1556ed12442afd20a299cf3)
             check_type(argname="argument index", value=index, expected_type=type_hints["index"])
-        return typing.cast("DataProxmoxTemplatesTemplatesNetworkInterfacesOutputReference", jsii.invoke(self, "get", [index]))
+        return typing.cast("DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfacesOutputReference", jsii.invoke(self, "get", [index]))
 
     @builtins.property
     @jsii.member(jsii_name="terraformAttribute")
     def _terraform_attribute(self) -> builtins.str:
         '''The attribute on the parent resource this class is referencing.'''
         return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
 
     @_terraform_attribute.setter
     def _terraform_attribute(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__48cef1cb379832d204d05e71200269648461a5d9b90d6210fd7323d5d5683d49)
+            type_hints = typing.get_type_hints(_typecheckingstub__29047c3a363ab0a8e7d3a137bd9ace754fc7b9344b7014198ba6e1d7d065f560)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformAttribute", value)
 
     @builtins.property
     @jsii.member(jsii_name="terraformResource")
     def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
         '''The parent resource.'''
         return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
 
     @_terraform_resource.setter
     def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7a78040dc29e020dddb0be94997801ef14e00270db063f5d34e30354fa694ed1)
+            type_hints = typing.get_type_hints(_typecheckingstub__f65753d9b5a1ab71e7119e2e8432894ff681b20a2115ee63f68fb2e5522580b7)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformResource", value)
 
     @builtins.property
     @jsii.member(jsii_name="wrapsSet")
     def _wraps_set(self) -> builtins.bool:
         '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
         return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
 
     @_wraps_set.setter
     def _wraps_set(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__83fa36cc540531a6aa1ce8e8e244ee7b9cd0d2e5314e607e6bdb917be2c4cd9c)
+            type_hints = typing.get_type_hints(_typecheckingstub__64ec7ff087cd1fc3263b767eab2e7e6071219592c30052a84a6ddc7cf7521df3)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wrapsSet", value)
 
 
-class DataProxmoxTemplatesTemplatesNetworkInterfacesOutputReference(
+class DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfacesOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesNetworkInterfacesOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfacesOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         complex_object_index: jsii.Number,
         complex_object_is_from_set: builtins.bool,
@@ -1721,15 +1740,15 @@
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param complex_object_index: the index of this item in the list.
         :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__ca79e6840c22cc22b6a35edff39fed27bec20ff0729d3864153eda76572b6639)
+            type_hints = typing.get_type_hints(_typecheckingstub__d8ff437f72f080f73250f5d43143146351d691b612a516ecfc9d37877773f9e3)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
@@ -1777,32 +1796,32 @@
     def vlan(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "vlan"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[DataProxmoxTemplatesTemplatesNetworkInterfaces]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesNetworkInterfaces], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfaces]:
+        return typing.cast(typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfaces], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatesTemplatesNetworkInterfaces],
+        value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfaces],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1c58d8361d95c8785388c651a8bef3bdef6a00dcdb17739df96e92e48f2667ca)
+            type_hints = typing.get_type_hints(_typecheckingstub__83dd909b57952aafb9dcffd3c9fe30948f38ad3a8e5709ad0da7da1c5dd76af7)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
-class DataProxmoxTemplatesTemplatesOutputReference(
+class DataProxmoxVirtualMachinesVirtualMachinesOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         complex_object_index: jsii.Number,
         complex_object_is_from_set: builtins.bool,
@@ -1810,50 +1829,52 @@
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param complex_object_index: the index of this item in the list.
         :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__b202d7279af3d9819fdce569a9167c00ce44a03a626378a9a38f76286414bc81)
+            type_hints = typing.get_type_hints(_typecheckingstub__7cd50db486f570508ad7adbd3f8bc4cb14cf74955e66e5ab8f06900e833a234b)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
     @jsii.member(jsii_name="agent")
-    def agent(self) -> DataProxmoxTemplatesTemplatesAgentOutputReference:
-        return typing.cast(DataProxmoxTemplatesTemplatesAgentOutputReference, jsii.get(self, "agent"))
+    def agent(self) -> DataProxmoxVirtualMachinesVirtualMachinesAgentOutputReference:
+        return typing.cast(DataProxmoxVirtualMachinesVirtualMachinesAgentOutputReference, jsii.get(self, "agent"))
 
     @builtins.property
     @jsii.member(jsii_name="bios")
     def bios(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "bios"))
 
     @builtins.property
     @jsii.member(jsii_name="cloudInit")
-    def cloud_init(self) -> DataProxmoxTemplatesTemplatesCloudInitOutputReference:
-        return typing.cast(DataProxmoxTemplatesTemplatesCloudInitOutputReference, jsii.get(self, "cloudInit"))
+    def cloud_init(
+        self,
+    ) -> DataProxmoxVirtualMachinesVirtualMachinesCloudInitOutputReference:
+        return typing.cast(DataProxmoxVirtualMachinesVirtualMachinesCloudInitOutputReference, jsii.get(self, "cloudInit"))
 
     @builtins.property
     @jsii.member(jsii_name="cpu")
-    def cpu(self) -> DataProxmoxTemplatesTemplatesCpuOutputReference:
-        return typing.cast(DataProxmoxTemplatesTemplatesCpuOutputReference, jsii.get(self, "cpu"))
+    def cpu(self) -> DataProxmoxVirtualMachinesVirtualMachinesCpuOutputReference:
+        return typing.cast(DataProxmoxVirtualMachinesVirtualMachinesCpuOutputReference, jsii.get(self, "cpu"))
 
     @builtins.property
     @jsii.member(jsii_name="description")
     def description(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "description"))
 
     @builtins.property
     @jsii.member(jsii_name="disks")
-    def disks(self) -> DataProxmoxTemplatesTemplatesDisksList:
-        return typing.cast(DataProxmoxTemplatesTemplatesDisksList, jsii.get(self, "disks"))
+    def disks(self) -> DataProxmoxVirtualMachinesVirtualMachinesDisksList:
+        return typing.cast(DataProxmoxVirtualMachinesVirtualMachinesDisksList, jsii.get(self, "disks"))
 
     @builtins.property
     @jsii.member(jsii_name="id")
     def id(self) -> jsii.Number:
         return typing.cast(jsii.Number, jsii.get(self, "id"))
 
     @builtins.property
@@ -1869,36 +1890,38 @@
     @builtins.property
     @jsii.member(jsii_name="machineType")
     def machine_type(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "machineType"))
 
     @builtins.property
     @jsii.member(jsii_name="memory")
-    def memory(self) -> DataProxmoxTemplatesTemplatesMemoryOutputReference:
-        return typing.cast(DataProxmoxTemplatesTemplatesMemoryOutputReference, jsii.get(self, "memory"))
+    def memory(self) -> DataProxmoxVirtualMachinesVirtualMachinesMemoryOutputReference:
+        return typing.cast(DataProxmoxVirtualMachinesVirtualMachinesMemoryOutputReference, jsii.get(self, "memory"))
 
     @builtins.property
     @jsii.member(jsii_name="name")
     def name(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "name"))
 
     @builtins.property
     @jsii.member(jsii_name="networkInterfaces")
-    def network_interfaces(self) -> DataProxmoxTemplatesTemplatesNetworkInterfacesList:
-        return typing.cast(DataProxmoxTemplatesTemplatesNetworkInterfacesList, jsii.get(self, "networkInterfaces"))
+    def network_interfaces(
+        self,
+    ) -> DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfacesList:
+        return typing.cast(DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfacesList, jsii.get(self, "networkInterfaces"))
 
     @builtins.property
     @jsii.member(jsii_name="nodeAttribute")
     def node_attribute(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "nodeAttribute"))
 
     @builtins.property
     @jsii.member(jsii_name="pciDevices")
-    def pci_devices(self) -> "DataProxmoxTemplatesTemplatesPciDevicesList":
-        return typing.cast("DataProxmoxTemplatesTemplatesPciDevicesList", jsii.get(self, "pciDevices"))
+    def pci_devices(self) -> "DataProxmoxVirtualMachinesVirtualMachinesPciDevicesList":
+        return typing.cast("DataProxmoxVirtualMachinesVirtualMachinesPciDevicesList", jsii.get(self, "pciDevices"))
 
     @builtins.property
     @jsii.member(jsii_name="resourcePool")
     def resource_pool(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "resourcePool"))
 
     @builtins.property
@@ -1914,129 +1937,131 @@
     @builtins.property
     @jsii.member(jsii_name="type")
     def type(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "type"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
-    def internal_value(self) -> typing.Optional[DataProxmoxTemplatesTemplates]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplates], jsii.get(self, "internalValue"))
+    def internal_value(
+        self,
+    ) -> typing.Optional[DataProxmoxVirtualMachinesVirtualMachines]:
+        return typing.cast(typing.Optional[DataProxmoxVirtualMachinesVirtualMachines], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatesTemplates],
+        value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachines],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6e3dc4c5d3942ba601d2415386e2de0a087c80913e1cfdafc5a86ecb25ca0683)
+            type_hints = typing.get_type_hints(_typecheckingstub__bec20785c6139ce71c1b10c6b06068851ac112093f4c6f19ee264ee5f503e04b)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 @jsii.data_type(
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesPciDevices",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesPciDevices",
     jsii_struct_bases=[],
     name_mapping={},
 )
-class DataProxmoxTemplatesTemplatesPciDevices:
+class DataProxmoxVirtualMachinesVirtualMachinesPciDevices:
     def __init__(self) -> None:
         self._values: typing.Dict[builtins.str, typing.Any] = {}
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataProxmoxTemplatesTemplatesPciDevices(%s)" % ", ".join(
+        return "DataProxmoxVirtualMachinesVirtualMachinesPciDevices(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
-class DataProxmoxTemplatesTemplatesPciDevicesList(
+class DataProxmoxVirtualMachinesVirtualMachinesPciDevicesList(
     _cdktf_9a9027ec.ComplexList,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesPciDevicesList",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesPciDevicesList",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         wraps_set: builtins.bool,
     ) -> None:
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param wraps_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__55717d97f120003fb6031ddd71985e3f4c5eab0344a8c0befa42a9c89633667d)
+            type_hints = typing.get_type_hints(_typecheckingstub__d2fac40c30510c7e191317a1f2994186cfa269af0277ffcf6b4f0d73bdc22c16)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument wraps_set", value=wraps_set, expected_type=type_hints["wraps_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, wraps_set])
 
     @jsii.member(jsii_name="get")
     def get(
         self,
         index: jsii.Number,
-    ) -> "DataProxmoxTemplatesTemplatesPciDevicesOutputReference":
+    ) -> "DataProxmoxVirtualMachinesVirtualMachinesPciDevicesOutputReference":
         '''
         :param index: the index of the item to return.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__569cf596a9a1d3ba8639edd9a452162acdb7b653adf57ee077a1dbb1de70be96)
+            type_hints = typing.get_type_hints(_typecheckingstub__4d2ff1734bdea1ad614accd60c4bbdb530e32105b239e7f9d4954462554c30ae)
             check_type(argname="argument index", value=index, expected_type=type_hints["index"])
-        return typing.cast("DataProxmoxTemplatesTemplatesPciDevicesOutputReference", jsii.invoke(self, "get", [index]))
+        return typing.cast("DataProxmoxVirtualMachinesVirtualMachinesPciDevicesOutputReference", jsii.invoke(self, "get", [index]))
 
     @builtins.property
     @jsii.member(jsii_name="terraformAttribute")
     def _terraform_attribute(self) -> builtins.str:
         '''The attribute on the parent resource this class is referencing.'''
         return typing.cast(builtins.str, jsii.get(self, "terraformAttribute"))
 
     @_terraform_attribute.setter
     def _terraform_attribute(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__714ca5189a7e8b8efcba574865cb9541d6bb35e576329c8f5cbd05bfacafcd09)
+            type_hints = typing.get_type_hints(_typecheckingstub__93eb0455bc64ded278a82253e8dca76dc6cea038827502d424b3539ddfe8d39e)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformAttribute", value)
 
     @builtins.property
     @jsii.member(jsii_name="terraformResource")
     def _terraform_resource(self) -> _cdktf_9a9027ec.IInterpolatingParent:
         '''The parent resource.'''
         return typing.cast(_cdktf_9a9027ec.IInterpolatingParent, jsii.get(self, "terraformResource"))
 
     @_terraform_resource.setter
     def _terraform_resource(self, value: _cdktf_9a9027ec.IInterpolatingParent) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__400324fc47b84d680a8d6d870b00bcf22a76e01f2693f58a18e7bb03636c6f54)
+            type_hints = typing.get_type_hints(_typecheckingstub__1f44abc2b711cff13498f2fe7f2c2d3d599d62460e2b7337644b8529a1071635)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "terraformResource", value)
 
     @builtins.property
     @jsii.member(jsii_name="wrapsSet")
     def _wraps_set(self) -> builtins.bool:
         '''whether the list is wrapping a set (will add tolist() to be able to access an item via an index).'''
         return typing.cast(builtins.bool, jsii.get(self, "wrapsSet"))
 
     @_wraps_set.setter
     def _wraps_set(self, value: builtins.bool) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a314b4987d3ace06086de87977325702d27f5bba1ee500f931eb8285c6098fd2)
+            type_hints = typing.get_type_hints(_typecheckingstub__a80882ceed8fef31039313dbca5b1d33a65402a614decd92b48fa92ca5a42898)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "wrapsSet", value)
 
 
-class DataProxmoxTemplatesTemplatesPciDevicesOutputReference(
+class DataProxmoxVirtualMachinesVirtualMachinesPciDevicesOutputReference(
     _cdktf_9a9027ec.ComplexObject,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxTemplates.DataProxmoxTemplatesTemplatesPciDevicesOutputReference",
+    jsii_type="@awlsring/cdktf-proxmox.dataProxmoxVirtualMachines.DataProxmoxVirtualMachinesVirtualMachinesPciDevicesOutputReference",
 ):
     def __init__(
         self,
         terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
         terraform_attribute: builtins.str,
         complex_object_index: jsii.Number,
         complex_object_is_from_set: builtins.bool,
@@ -2044,15 +2069,15 @@
         '''
         :param terraform_resource: The parent resource.
         :param terraform_attribute: The attribute on the parent resource this class is referencing.
         :param complex_object_index: the index of this item in the list.
         :param complex_object_is_from_set: whether the list is wrapping a set (will add tolist() to be able to access an item via an index).
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__42f0553ee26f760ca9dbe015a65d976a474040e167c3eb17a393b33cc0ce92c1)
+            type_hints = typing.get_type_hints(_typecheckingstub__d6ae42fd620058d11c2ed00bfd6815f23450adf4beff345be6239efe7107ecf7)
             check_type(argname="argument terraform_resource", value=terraform_resource, expected_type=type_hints["terraform_resource"])
             check_type(argname="argument terraform_attribute", value=terraform_attribute, expected_type=type_hints["terraform_attribute"])
             check_type(argname="argument complex_object_index", value=complex_object_index, expected_type=type_hints["complex_object_index"])
             check_type(argname="argument complex_object_is_from_set", value=complex_object_is_from_set, expected_type=type_hints["complex_object_is_from_set"])
         jsii.create(self.__class__, self, [terraform_resource, terraform_attribute, complex_object_index, complex_object_is_from_set])
 
     @builtins.property
@@ -2090,524 +2115,524 @@
     def rom_file(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "romFile"))
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[DataProxmoxTemplatesTemplatesPciDevices]:
-        return typing.cast(typing.Optional[DataProxmoxTemplatesTemplatesPciDevices], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesPciDevices]:
+        return typing.cast(typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesPciDevices], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[DataProxmoxTemplatesTemplatesPciDevices],
+        value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesPciDevices],
     ) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__1bb2963547ad5083d7060c4cf5df44ddaf83851eefd9ab93fb720702b84cc7ad)
+            type_hints = typing.get_type_hints(_typecheckingstub__8bc94e70b1696543adfce726f492d86a42d111b809e06d2c63668d472bf25b1d)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
 __all__ = [
-    "DataProxmoxTemplates",
-    "DataProxmoxTemplatesConfig",
-    "DataProxmoxTemplatesFilters",
-    "DataProxmoxTemplatesFiltersList",
-    "DataProxmoxTemplatesFiltersOutputReference",
-    "DataProxmoxTemplatesTemplates",
-    "DataProxmoxTemplatesTemplatesAgent",
-    "DataProxmoxTemplatesTemplatesAgentOutputReference",
-    "DataProxmoxTemplatesTemplatesCloudInit",
-    "DataProxmoxTemplatesTemplatesCloudInitDns",
-    "DataProxmoxTemplatesTemplatesCloudInitDnsOutputReference",
-    "DataProxmoxTemplatesTemplatesCloudInitIp",
-    "DataProxmoxTemplatesTemplatesCloudInitIpList",
-    "DataProxmoxTemplatesTemplatesCloudInitIpOutputReference",
-    "DataProxmoxTemplatesTemplatesCloudInitIpV4",
-    "DataProxmoxTemplatesTemplatesCloudInitIpV4OutputReference",
-    "DataProxmoxTemplatesTemplatesCloudInitIpV6",
-    "DataProxmoxTemplatesTemplatesCloudInitIpV6OutputReference",
-    "DataProxmoxTemplatesTemplatesCloudInitOutputReference",
-    "DataProxmoxTemplatesTemplatesCloudInitUser",
-    "DataProxmoxTemplatesTemplatesCloudInitUserOutputReference",
-    "DataProxmoxTemplatesTemplatesCpu",
-    "DataProxmoxTemplatesTemplatesCpuOutputReference",
-    "DataProxmoxTemplatesTemplatesDisks",
-    "DataProxmoxTemplatesTemplatesDisksList",
-    "DataProxmoxTemplatesTemplatesDisksOutputReference",
-    "DataProxmoxTemplatesTemplatesDisksSpeedLimits",
-    "DataProxmoxTemplatesTemplatesDisksSpeedLimitsOutputReference",
-    "DataProxmoxTemplatesTemplatesList",
-    "DataProxmoxTemplatesTemplatesMemory",
-    "DataProxmoxTemplatesTemplatesMemoryOutputReference",
-    "DataProxmoxTemplatesTemplatesNetworkInterfaces",
-    "DataProxmoxTemplatesTemplatesNetworkInterfacesList",
-    "DataProxmoxTemplatesTemplatesNetworkInterfacesOutputReference",
-    "DataProxmoxTemplatesTemplatesOutputReference",
-    "DataProxmoxTemplatesTemplatesPciDevices",
-    "DataProxmoxTemplatesTemplatesPciDevicesList",
-    "DataProxmoxTemplatesTemplatesPciDevicesOutputReference",
+    "DataProxmoxVirtualMachines",
+    "DataProxmoxVirtualMachinesConfig",
+    "DataProxmoxVirtualMachinesFilters",
+    "DataProxmoxVirtualMachinesFiltersList",
+    "DataProxmoxVirtualMachinesFiltersOutputReference",
+    "DataProxmoxVirtualMachinesVirtualMachines",
+    "DataProxmoxVirtualMachinesVirtualMachinesAgent",
+    "DataProxmoxVirtualMachinesVirtualMachinesAgentOutputReference",
+    "DataProxmoxVirtualMachinesVirtualMachinesCloudInit",
+    "DataProxmoxVirtualMachinesVirtualMachinesCloudInitDns",
+    "DataProxmoxVirtualMachinesVirtualMachinesCloudInitDnsOutputReference",
+    "DataProxmoxVirtualMachinesVirtualMachinesCloudInitIp",
+    "DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpList",
+    "DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpOutputReference",
+    "DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV4",
+    "DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV4OutputReference",
+    "DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV6",
+    "DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV6OutputReference",
+    "DataProxmoxVirtualMachinesVirtualMachinesCloudInitOutputReference",
+    "DataProxmoxVirtualMachinesVirtualMachinesCloudInitUser",
+    "DataProxmoxVirtualMachinesVirtualMachinesCloudInitUserOutputReference",
+    "DataProxmoxVirtualMachinesVirtualMachinesCpu",
+    "DataProxmoxVirtualMachinesVirtualMachinesCpuOutputReference",
+    "DataProxmoxVirtualMachinesVirtualMachinesDisks",
+    "DataProxmoxVirtualMachinesVirtualMachinesDisksList",
+    "DataProxmoxVirtualMachinesVirtualMachinesDisksOutputReference",
+    "DataProxmoxVirtualMachinesVirtualMachinesDisksSpeedLimits",
+    "DataProxmoxVirtualMachinesVirtualMachinesDisksSpeedLimitsOutputReference",
+    "DataProxmoxVirtualMachinesVirtualMachinesList",
+    "DataProxmoxVirtualMachinesVirtualMachinesMemory",
+    "DataProxmoxVirtualMachinesVirtualMachinesMemoryOutputReference",
+    "DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfaces",
+    "DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfacesList",
+    "DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfacesOutputReference",
+    "DataProxmoxVirtualMachinesVirtualMachinesOutputReference",
+    "DataProxmoxVirtualMachinesVirtualMachinesPciDevices",
+    "DataProxmoxVirtualMachinesVirtualMachinesPciDevicesList",
+    "DataProxmoxVirtualMachinesVirtualMachinesPciDevicesOutputReference",
 ]
 
 publication.publish()
 
-def _typecheckingstub__9c8f43a8ed4d9862bb2dfda7c754989b1621c88e999f35c8aa0300d8f6ba0675(
+def _typecheckingstub__8964a502bdd6837bb34f855f2792c0696572ed85c989e789cc2e5b4121a36e07(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
-    filters: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataProxmoxTemplatesFilters, typing.Dict[builtins.str, typing.Any]]]]] = None,
+    filters: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataProxmoxVirtualMachinesFilters, typing.Dict[builtins.str, typing.Any]]]]] = None,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[jsii.Number] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__233a1989690e82037c4c9dc0c040be824ca0bc7ab5562170fe8918e4876b29f9(
-    value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataProxmoxTemplatesFilters, typing.Dict[builtins.str, typing.Any]]]],
+def _typecheckingstub__234cf70c85efdb576bc5aeff6ef01db102e6418ab29585d697ac0a250b06fd30(
+    value: typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataProxmoxVirtualMachinesFilters, typing.Dict[builtins.str, typing.Any]]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__4b9b87d43a9822a28f232fcb57074d7978bca6aa140657b9397ad2bf3cabac68(
+def _typecheckingstub__0c1f1b06e874d1f8d6204299e031aa4b0e420c44cbc8804b2a401a388c11d270(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
     count: typing.Optional[jsii.Number] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
-    filters: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataProxmoxTemplatesFilters, typing.Dict[builtins.str, typing.Any]]]]] = None,
+    filters: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataProxmoxVirtualMachinesFilters, typing.Dict[builtins.str, typing.Any]]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7b5a2e2e69a8b272223cae04497ef0e50f1388bd002ce5d48b07318623fc0fd0(
+def _typecheckingstub__859c03e5becb1d85fc603cba6f0b2225308fdef7e7962a6a5c17fd27c6ae0c64(
     *,
     name: builtins.str,
     values: typing.Sequence[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7185592ee5df14f6502caf1b02c1c8f7f1a998c262a921b4059ae73ed17d01f7(
+def _typecheckingstub__3355cff5bd7377db4300269580da8f8240b6d258eabd8dcdf80d03d8088f28b6(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b3e0e2fef1c0a4b8e2a1b64ae525d2b0ac767a60597d7eb6476cf5a4b328eb58(
+def _typecheckingstub__073eda288224fca974ec6f12f1acfceb54b74c646aa6900e74c182cdd68d85fc(
     index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__12203107c9a9b5812061df83af59f971166e12e0dd3c53822898b587c4a13a1a(
+def _typecheckingstub__faf20181ed0e23ef3f5bc1692ab7494a10eaa85c8edab3ac4f4a93d7e57140b3(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7c18c8f27f5b5749f0930032ce59cf9aa9dd8c3fe11454a21edfacfb39110484(
+def _typecheckingstub__c25a6c623b61b177f9bf2f54fae6101d56d21e9edcf027abe9691b547bab6791(
     value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1de467d3e8e92a1d8d17a81042c85e45ddb8a5f8a574026c01b38410619c435e(
+def _typecheckingstub__1b039d1c7ee0a20c37735d707128147ad27c3b2066a142a8245801abfab54760(
     value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__4eeb8042fe9f97bb3b08f79bdd3f5544c61ad333e13f34069ee25b3925b85f8c(
-    value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataProxmoxTemplatesFilters]]],
+def _typecheckingstub__de90626d8d6cb4f51e48e76cc780e64af3308dcb4a9387bacd68d9acaefcd3d9(
+    value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List[DataProxmoxVirtualMachinesFilters]]],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__8327cf5bac96b9877733ed3b92c5e728be3a17f989a4bdbaf2900a291c81f07d(
+def _typecheckingstub__e17bdc6aba401b91212b88e17b905a71eb22c22d50f7b0ed5fce967f8502ff54(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__16f3ef7637865b9efbe01d5d61b463f735bae38264ad57354abdbce513208aef(
+def _typecheckingstub__d16c453aabbc842f9d9270513abd49f9d0512710bfe08e8f3ec0aa4580a67f7e(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__8a7dc4004f107546dc9c621fa798620b5001c0fd8917d4c9140a0ad48064ed70(
+def _typecheckingstub__d0f24eea4504bd90493c0ddea1d0a515f1b6835969b6e9ef6601c0e4f4b91c1e(
     value: typing.List[builtins.str],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__dec6db530ef281b602f64ed73e330e24906e6e0c6b954683c5ba96b7ad21dcbf(
-    value: typing.Optional[typing.Union[DataProxmoxTemplatesFilters, _cdktf_9a9027ec.IResolvable]],
+def _typecheckingstub__111b39294ca1a0f53214e63c1951305a9a858d7c6b49427b8f31cc150dea7cfc(
+    value: typing.Optional[typing.Union[DataProxmoxVirtualMachinesFilters, _cdktf_9a9027ec.IResolvable]],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__673e66db611a5fbc4e59ce825f6e4416fa82cbf66904ba65202f13a93beb37d2(
+def _typecheckingstub__07d113599c3ded151ad319677ae0805061bedb2e53dc395f36e38892a1732956(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__11571a58fd163ae522f420d6c0dff17873e68251c637a1ebc2f4261d40a0908e(
-    value: typing.Optional[DataProxmoxTemplatesTemplatesAgent],
+def _typecheckingstub__8c6a7e94ae13a6fe6d8277fee1493d5adf31562cf476d3edea88cdb28b4b5f09(
+    value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesAgent],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__e067c9db4e634da658b56ee80ca7edfde446f1a440b47d1f6eb546e326a67b26(
+def _typecheckingstub__2290f2bcf49b3f5380318f104b1ae2747c259487d97ca061b5a305da54bfe390(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__0782611e20910ed665dc0d5e84a3f71452ba5bade5ae664490668cd11d64b023(
-    value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitDns],
+def _typecheckingstub__0c58e16081384a2f723727787e4cc8068349196e637a1f457896308290b1557f(
+    value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitDns],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__99f203b02f9592f1a1fb7a64a5635c720b9dd6c7f992bc56e8edb0bab0e63ae7(
+def _typecheckingstub__670bc4d8280f028c77ea09b2abed573c41ec7f36c2783c71af8f86efb9c064b3(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__17abca3a5e9277181468d701c2550bed8e6e1d101cde67b7c64c5bf22a976a80(
+def _typecheckingstub__4f2cb10553da29016ece8d9bd3802ddfc4ad73c134c0b0390ff9883c5d145d3c(
     index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__8f5acfd27a377920da103fd958e5f6b4dbf0ed9b81ad89a5f0293c850734683d(
+def _typecheckingstub__65ae18e026db7c863074d3aec87b67584f61d4014aff3434aa5bc2ea8c97a9bf(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__4ab6c78fc6f14f4f992d620cd01deffae673cfc19cb90a2b3a92306efc35ecdc(
+def _typecheckingstub__b951ce6319261e9a74ca61b8cb0c6e32dc7a56176d2ffe94e46f6e9de731b12f(
     value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__d95d53ee35c350fc80dac6a96148f86fabee41b7110a6853b4b1a4f0a5d8f0c7(
+def _typecheckingstub__224b885742822d9f056ed325941e555baa7b112c1ba45bbda98fb61767292b1e(
     value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__bd10d7eba8b193e54bbf14d276b04c99e46b2cdd97d9ee8c3b3b5574420a6e07(
+def _typecheckingstub__b3415898b0a5f21c0e71a645d890d0f7d0b5d0671b8c1365c8f61e3eb7110c73(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__c6edec7bf9da7fc858d6f00b1a2bca916dd1537601759f0547eecdabfc5fd9dd(
-    value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIp],
+def _typecheckingstub__34bffe777ebd3bc403935e1b2d49c4491a3aae7a692ba76e9ff55d600a37d857(
+    value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitIp],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__489e948956a30a57fae7529bdc147f4aca6ac2e350685a9c13f1011adf371d56(
+def _typecheckingstub__08d9485cead65b2fbe96f1195e36008437795435c6e8f41337038c24d0a97560(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__316b4ac8b088bec9d0a20b18732922b3c4f2ec34c73423ab7110590748dc5151(
-    value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV4],
+def _typecheckingstub__b35dc38c3cc9bb23db7099cb8254112e1dcbf68252cf23cbd4b42e4fec6db0c3(
+    value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV4],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__794b5f9374ea15e16167c1ac262a044629688c6c6d472d93a73026f2902c9054(
+def _typecheckingstub__e09b2a2eade5c5be811c9310d90f28a5cbe6719ef4799f52c57bd93061aa88e2(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ff35973d8191c68c6e6ff6f7e9a4b46f7fb17e1b8800426dcf85ae2efb76e925(
-    value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitIpV6],
+def _typecheckingstub__055bb09a1452519595b570d7f5ed45e2c0e738e1f38219d8581999a79946e921(
+    value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitIpV6],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__29f4c65f37a567f10935f4c966639f7bdf80838af210c4911049934a056a8f50(
+def _typecheckingstub__81b259dda29c3f040d46b4f55c59e9cc7915255bbc6f8bd9fe0e8c46fa9dc447(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__4aef00a6fe7514158fcad983bbd4c46da783c27bccbf0aeeb7e342ba5ce802b8(
-    value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInit],
+def _typecheckingstub__6d252ed48a14f6a7171a01ba9bcaddfdfe37577ad4a546c42f2f20f96b94cb34(
+    value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInit],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ab97a5c9497e31ad13315c518709649341b3f92644baa1db3ad03d0e7724a704(
+def _typecheckingstub__63293903413c405b49ccc38a464d0226844a76004821eea7f5ca5ee351482ea9(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__40a73c62c87638712e722cd3fd3f967956c8dabb50c0d76987263c31322adf9f(
-    value: typing.Optional[DataProxmoxTemplatesTemplatesCloudInitUser],
+def _typecheckingstub__f8544ddcf0efba56064233ae8312df8b7a7fe49ce90b4652f9783fb89b84da08(
+    value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCloudInitUser],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a5a42158ebc03e71f8f9bdc4ad6b1258c5fe9acbd56ba299f3e2fdabdf3cd633(
+def _typecheckingstub__1958f45b6ab064186f301d8386335e8c83f22a4ccdcbca2e6ae54f2f6ef983eb(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__fb0f4d2eadaa9e4d99b7a9686d56e4d9532194127cf03192619771e2ef651831(
-    value: typing.Optional[DataProxmoxTemplatesTemplatesCpu],
+def _typecheckingstub__e9b7f41bb0798211787e68a31b1c7daf4153c5dbfd489800215834eff544b1e8(
+    value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesCpu],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__d5f5bf449c9309a6b5d5c6b7f49c07b04a79a2c1c99b5c48638d61eb31622e7c(
+def _typecheckingstub__0c98fbaa0b49269b0c90284fe1740e24d2e9379e844cce804635729047fb09ec(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__8b683a39926cfaa60ef131b3061711541f522c4102ea45f5688bdc06bf9edb19(
+def _typecheckingstub__621e7f7977ebf33a08e0572e42b38746107f67ad9f7e30180350b831a74ba3b8(
     index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1ceab6297650a2d7fe87e70d5e2c1bc0179b8edd69ebcbea2d28f2d3254a7cf9(
+def _typecheckingstub__d460fd02ce4f7b52c6f03034fbdaed0dacf058481f77c05e66bfac805177d900(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__0ac4b2edba5a1f5d58b921e4fd12222646c78eac69326d2f9d9cb8cfdf5293f0(
+def _typecheckingstub__cba26de2b6e3232d042a73ac8f07e30ad776b9843de6d2b3f287e4ae2105ca6c(
     value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__3681c1aed5886b3362ddc27a0c8a45545916b1eea3d5c5525293ae002562a24a(
+def _typecheckingstub__566d4ee1321afb3df335ecaedb5bfd22d08474ad70cc1ed97b042a2cefbceb5a(
     value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__e36693344440afa8e05cd759d3059d6580174e1078ac7d475b89fa21b4348697(
+def _typecheckingstub__b32e086fb26b23e3a898946ad7abc208af97ba9cc58ae594736dce1bf2550777(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__3411d4f953ea91029177b1db6c9690297978a4c8aa4f1a064ccb2be6d9a0219e(
-    value: typing.Optional[DataProxmoxTemplatesTemplatesDisks],
+def _typecheckingstub__2cbd5d298cdb62f85ba547df49f0fd65bc3f4591d25afc720b2ef4224ddb1abb(
+    value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesDisks],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__6507fc59ef695082c0ae01339c5f249d975700e498b4e18908c1eafa158d19f8(
+def _typecheckingstub__46c7a5b1e39db160d2904fcfa03bd458875cd05b01a4c0852fe8b0a2db0d471c(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__c18f8c7ed8d24d2b06774c7cd39f86063e0c0dd2b09ba5b07796c7ebbfa6b319(
-    value: typing.Optional[DataProxmoxTemplatesTemplatesDisksSpeedLimits],
+def _typecheckingstub__131284fb30fe862c25a9c2aa553cf871875637fbe865e221adeec2521470c8c9(
+    value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesDisksSpeedLimits],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__0f08ad26095875cedb140ea7fee38d064da3ca7274d935b385b43bee3f8e0224(
+def _typecheckingstub__980cd4eb86098e6866bb8dc40d7238744a84f546e0824b3fc6c6e3c6a5237fd1(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a73b9f8ad3ee64bf1330033bbb94eda72651474ebf3cc08f02fdb5164474837f(
+def _typecheckingstub__0cfd1aa70ee72623f0979da97640b25f0737a55548794f1f93d0ff21ae2b1e0c(
     index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__848480b079fffd0ff9a7f3a525600012d4afc4dee5881b91ae5e7167dbb59566(
+def _typecheckingstub__40e6af369bd325ebd038a49265102cdb8b5c4cb027266754f3d7cb2130d214bf(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__fa2c9ff301f9aee5b2b11bbfc41fe82846b8379b5d0938c0623854abf252aa3c(
+def _typecheckingstub__6f5f8973a8d38e1ea26c40da9379f115f36db1c2cab24f96811a0809c52ec2b2(
     value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__abebb6092537f032ac958ea0c960b43351ae38dc63f45c0caf96a643d0c578a2(
+def _typecheckingstub__0a68d92988fcfdfa3ffdab3821127b4709402e1f83e08ba3e721786afcffa9cf(
     value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__85086878bd5559f9bcb76f72ef7d39713a5dfe1a67404088b22a948985c5628d(
+def _typecheckingstub__5a1e71e78d36120a049bc9b4d3809b891cd651b04445ad5e19fcb5debcfb94b2(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__37ed7ef44a558b41c24319f430bd9d5e8e061f43edd93c6b14328bd6a508557c(
-    value: typing.Optional[DataProxmoxTemplatesTemplatesMemory],
+def _typecheckingstub__bda3dbfa79f54ba4a1f9943f6b812bd81885f1c2aae1e6268c893b56b1e5d676(
+    value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesMemory],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__936967cce1c15f47cc61cad0804576959a9d43335f92de11fff9576904e2c633(
+def _typecheckingstub__795a0e16e037136dc5720eda98344143c0c93fe5e7a9a9f58519e0b4c41505c2(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__737e30ba026c9167075fe33c1c2bd27a25ebda2df3ada8476ea562276b30e283(
+def _typecheckingstub__d05a397d7edbf4a67ada5f47bc2c66f1d64e6817f1556ed12442afd20a299cf3(
     index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__48cef1cb379832d204d05e71200269648461a5d9b90d6210fd7323d5d5683d49(
+def _typecheckingstub__29047c3a363ab0a8e7d3a137bd9ace754fc7b9344b7014198ba6e1d7d065f560(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7a78040dc29e020dddb0be94997801ef14e00270db063f5d34e30354fa694ed1(
+def _typecheckingstub__f65753d9b5a1ab71e7119e2e8432894ff681b20a2115ee63f68fb2e5522580b7(
     value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__83fa36cc540531a6aa1ce8e8e244ee7b9cd0d2e5314e607e6bdb917be2c4cd9c(
+def _typecheckingstub__64ec7ff087cd1fc3263b767eab2e7e6071219592c30052a84a6ddc7cf7521df3(
     value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__ca79e6840c22cc22b6a35edff39fed27bec20ff0729d3864153eda76572b6639(
+def _typecheckingstub__d8ff437f72f080f73250f5d43143146351d691b612a516ecfc9d37877773f9e3(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1c58d8361d95c8785388c651a8bef3bdef6a00dcdb17739df96e92e48f2667ca(
-    value: typing.Optional[DataProxmoxTemplatesTemplatesNetworkInterfaces],
+def _typecheckingstub__83dd909b57952aafb9dcffd3c9fe30948f38ad3a8e5709ad0da7da1c5dd76af7(
+    value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesNetworkInterfaces],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__b202d7279af3d9819fdce569a9167c00ce44a03a626378a9a38f76286414bc81(
+def _typecheckingstub__7cd50db486f570508ad7adbd3f8bc4cb14cf74955e66e5ab8f06900e833a234b(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__6e3dc4c5d3942ba601d2415386e2de0a087c80913e1cfdafc5a86ecb25ca0683(
-    value: typing.Optional[DataProxmoxTemplatesTemplates],
+def _typecheckingstub__bec20785c6139ce71c1b10c6b06068851ac112093f4c6f19ee264ee5f503e04b(
+    value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachines],
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__55717d97f120003fb6031ddd71985e3f4c5eab0344a8c0befa42a9c89633667d(
+def _typecheckingstub__d2fac40c30510c7e191317a1f2994186cfa269af0277ffcf6b4f0d73bdc22c16(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     wraps_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__569cf596a9a1d3ba8639edd9a452162acdb7b653adf57ee077a1dbb1de70be96(
+def _typecheckingstub__4d2ff1734bdea1ad614accd60c4bbdb530e32105b239e7f9d4954462554c30ae(
     index: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__714ca5189a7e8b8efcba574865cb9541d6bb35e576329c8f5cbd05bfacafcd09(
+def _typecheckingstub__93eb0455bc64ded278a82253e8dca76dc6cea038827502d424b3539ddfe8d39e(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__400324fc47b84d680a8d6d870b00bcf22a76e01f2693f58a18e7bb03636c6f54(
+def _typecheckingstub__1f44abc2b711cff13498f2fe7f2c2d3d599d62460e2b7337644b8529a1071635(
     value: _cdktf_9a9027ec.IInterpolatingParent,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__a314b4987d3ace06086de87977325702d27f5bba1ee500f931eb8285c6098fd2(
+def _typecheckingstub__a80882ceed8fef31039313dbca5b1d33a65402a614decd92b48fa92ca5a42898(
     value: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__42f0553ee26f760ca9dbe015a65d976a474040e167c3eb17a393b33cc0ce92c1(
+def _typecheckingstub__d6ae42fd620058d11c2ed00bfd6815f23450adf4beff345be6239efe7107ecf7(
     terraform_resource: _cdktf_9a9027ec.IInterpolatingParent,
     terraform_attribute: builtins.str,
     complex_object_index: jsii.Number,
     complex_object_is_from_set: builtins.bool,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__1bb2963547ad5083d7060c4cf5df44ddaf83851eefd9ab93fb720702b84cc7ad(
-    value: typing.Optional[DataProxmoxTemplatesTemplatesPciDevices],
+def _typecheckingstub__8bc94e70b1696543adfce726f492d86a42d111b809e06d2c63668d472bf25b1d(
+    value: typing.Optional[DataProxmoxVirtualMachinesVirtualMachinesPciDevices],
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_zfs_pools/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_zfs_pools/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/data_proxmox_zfs_storage_classes/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/data_proxmox_zfs_storage_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/lvm/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/lvm/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/lvm_storage_class/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/lvm_storage_class/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/lvm_thinpool/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/lvm_thinpool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/lvm_thinpool_storage_class/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/lvm_thinpool_storage_class/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/network_bond/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/network_bond/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/network_bridge/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/network_bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/nfs_storage_class/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/nfs_storage_class/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/provider/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/resource_pool/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/resource_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/virtual_machine/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/virtual_machine/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2631,19 +2631,14 @@
         return typing.cast(None, jsii.invoke(self, "resetSsdEmulation", []))
 
     @jsii.member(jsii_name="resetUseIothread")
     def reset_use_iothread(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetUseIothread", []))
 
     @builtins.property
-    @jsii.member(jsii_name="name")
-    def name(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "name"))
-
-    @builtins.property
     @jsii.member(jsii_name="speedLimits")
     def speed_limits(self) -> "VirtualMachineComputedDisksSpeedLimitsOutputReference":
         return typing.cast("VirtualMachineComputedDisksSpeedLimitsOutputReference", jsii.get(self, "speedLimits"))
 
     @builtins.property
     @jsii.member(jsii_name="discardInput")
     def discard_input(
@@ -5022,19 +5017,14 @@
         return typing.cast(None, jsii.invoke(self, "resetSsdEmulation", []))
 
     @jsii.member(jsii_name="resetUseIothread")
     def reset_use_iothread(self) -> None:
         return typing.cast(None, jsii.invoke(self, "resetUseIothread", []))
 
     @builtins.property
-    @jsii.member(jsii_name="name")
-    def name(self) -> builtins.str:
-        return typing.cast(builtins.str, jsii.get(self, "name"))
-
-    @builtins.property
     @jsii.member(jsii_name="speedLimits")
     def speed_limits(self) -> "VirtualMachineDisksSpeedLimitsOutputReference":
         return typing.cast("VirtualMachineDisksSpeedLimitsOutputReference", jsii.get(self, "speedLimits"))
 
     @builtins.property
     @jsii.member(jsii_name="discardInput")
     def discard_input(
```

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/zfs_pool/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/zfs_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox/zfs_storage_class/__init__.py` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox/zfs_storage_class/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox.egg-info/PKG-INFO` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-proxmox
-Version: 0.0.86
+Version: 0.0.9
 Summary: A package that vends generated constructs from the Proxmox Terraform provider
 Home-page: https://github.com/awlsring/cdktf-proxmox.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-proxmox.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-proxmox-0.0.86/src/cdktf_proxmox.egg-info/SOURCES.txt` & `cdktf-proxmox-0.0.9/src/cdktf_proxmox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,28 @@
 src/cdktf_proxmox/py.typed
 src/cdktf_proxmox.egg-info/PKG-INFO
 src/cdktf_proxmox.egg-info/SOURCES.txt
 src/cdktf_proxmox.egg-info/dependency_links.txt
 src/cdktf_proxmox.egg-info/requires.txt
 src/cdktf_proxmox.egg-info/top_level.txt
 src/cdktf_proxmox/_jsii/__init__.py
-src/cdktf_proxmox/_jsii/cdktf-proxmox@0.0.86.jsii.tgz
+src/cdktf_proxmox/_jsii/cdktf-proxmox@0.0.9.jsii.tgz
 src/cdktf_proxmox/data_proxmox_lvm_storage_classes/__init__.py
 src/cdktf_proxmox/data_proxmox_lvm_thinpool_storage_classes/__init__.py
 src/cdktf_proxmox/data_proxmox_lvm_thinpools/__init__.py
 src/cdktf_proxmox/data_proxmox_lvms/__init__.py
 src/cdktf_proxmox/data_proxmox_network_bonds/__init__.py
 src/cdktf_proxmox/data_proxmox_network_bridges/__init__.py
 src/cdktf_proxmox/data_proxmox_nfs_storage_classes/__init__.py
 src/cdktf_proxmox/data_proxmox_node_storage_lvm_thinpools/__init__.py
 src/cdktf_proxmox/data_proxmox_node_storage_lvms/__init__.py
 src/cdktf_proxmox/data_proxmox_node_storage_nfs/__init__.py
 src/cdktf_proxmox/data_proxmox_node_storage_zfs/__init__.py
 src/cdktf_proxmox/data_proxmox_nodes/__init__.py
 src/cdktf_proxmox/data_proxmox_resource_pools/__init__.py
-src/cdktf_proxmox/data_proxmox_template/__init__.py
 src/cdktf_proxmox/data_proxmox_templates/__init__.py
 src/cdktf_proxmox/data_proxmox_virtual_machines/__init__.py
 src/cdktf_proxmox/data_proxmox_zfs_pools/__init__.py
 src/cdktf_proxmox/data_proxmox_zfs_storage_classes/__init__.py
 src/cdktf_proxmox/lvm/__init__.py
 src/cdktf_proxmox/lvm_storage_class/__init__.py
 src/cdktf_proxmox/lvm_thinpool/__init__.py
```

