# Comparing `tmp/MGP_SDK-1.1.0.tar.gz` & `tmp/MGP_SDK-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\ty027972\Desktop\marianas-team\marianas-team\SDKs\Python\MGP\dist\.tmp-mnaqdabj\MGP_SDK-1.1.0.tar", last modified: Thu May 18 21:11:38 2023, max compression
+gzip compressed data, was "C:\Users\ty027972\Desktop\marianas-team\marianas-team\SDKs\Python\MGP\dist\.tmp-xz5bmuyq\MGP_SDK-1.1.1.tar", last modified: Tue May 23 17:31:02 2023, max compression
```

## Comparing `MGP_SDK-1.1.0.tar` & `MGP_SDK-1.1.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/
--rw-rw-rw-   0        0        0     2600 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1752 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1845 2023-05-18 21:10:35.000000 MGP_SDK-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/__init__.py
--rw-rw-rw-   0        0        0    43398 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/interface.py
--rw-rw-rw-   0        0        0     5567 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/wfs.py
--rw-rw-rw-   0        0        0     4208 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/wms.py
--rw-rw-rw-   0        0        0     7607 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/wmts.py
--rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/__init__.py
--rw-rw-rw-   0        0        0     3911 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/accounts.py
--rw-rw-rw-   0        0        0     3885 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/activations.py
--rw-rw-rw-   0        0        0     5512 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/addresses.py
--rw-rw-rw-   0        0        0     5759 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/interface.py
--rw-rw-rw-   0        0        0     2823 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/products.py
--rw-rw-rw-   0        0        0     3480 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/rate_tables.py
--rw-rw-rw-   0        0        0     1172 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/roles.py
--rw-rw-rw-   0        0        0     8249 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/usage.py
--rw-rw-rw-   0        0        0     9173 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/account_service/users.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/analytics_service/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/analytics_service/__init__.py
--rw-rw-rw-   0        0        0     6650 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/analytics_service/analytics.py
--rw-rw-rw-   0        0        0     4900 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/analytics_service/interface.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/auth/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/auth/__init__.py
--rw-rw-rw-   0        0        0     6387 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/auth/auth.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/basemap_service/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/basemap_service/__init__.py
--rw-rw-rw-   0        0        0     1271 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/basemap_service/basemaps.py
--rw-rw-rw-   0        0        0     7889 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/basemap_service/interface.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/__init__.py
--rw-rw-rw-   0        0        0     7871 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/catalogs.py
--rw-rw-rw-   0        0        0     7974 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/collections.py
--rw-rw-rw-   0        0        0     6707 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/interface.py
--rw-rw-rw-   0        0        0     3140 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/search.py
--rw-rw-rw-   0        0        0     1241 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/server_checks.py
--rw-rw-rw-   0        0        0     1913 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/interface.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/monitor_service/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/monitor_service/__init__.py
--rw-rw-rw-   0        0        0     3980 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/monitor_service/interface.py
--rw-rw-rw-   0        0        0     7133 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/monitor_service/monitoring.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/__init__.py
--rw-rw-rw-   0        0        0     6264 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/interface.py
--rw-rw-rw-   0        0        0     5932 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/orders.py
--rw-rw-rw-   0        0        0     3353 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/pipelines.py
--rw-rw-rw-   0        0        0    16857 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/process.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/streaming/
--rw-rw-rw-   0        0        0        2 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/streaming/__init__.py
--rw-rw-rw-   0        0        0     6571 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/streaming/cli_commands.py
--rw-rw-rw-   0        0        0    10859 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/streaming/interface.py
--rw-rw-rw-   0        0        0     3866 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/streaming/wcs_archive.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/tasking_service/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/tasking_service/__init__.py
--rw-rw-rw-   0        0        0     3588 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/tasking_service/interface.py
--rw-rw-rw-   0        0        0     5203 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/tasking_service/tasking.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/three_d/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/three_d/__init__.py
--rw-rw-rw-   0        0        0     2183 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/three_d/interface.py
--rw-rw-rw-   0        0        0     3460 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/three_d/three_d.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/token_service/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/token_service/__init__.py
--rw-rw-rw-   0        0        0     3211 2023-05-18 21:09:42.000000 MGP_SDK-1.1.0/src/MGP_SDK/token_service/cli_commands.py
--rw-rw-rw-   0        0        0     2929 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/token_service/token.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK/usage_service/
--rw-rw-rw-   0        0        0        0 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/usage_service/__init__.py
--rw-rw-rw-   0        0        0      702 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/usage_service/interface.py
--rw-rw-rw-   0        0        0     1563 2023-05-17 21:10:26.000000 MGP_SDK-1.1.0/src/MGP_SDK/usage_service/usage.py
-drwxrwxrwx   0        0        0        0 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK.egg-info/
--rw-rw-rw-   0        0        0     2600 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2289 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      461 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       65 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-18 21:11:38.000000 MGP_SDK-1.1.0/src/MGP_SDK.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/
+-rw-rw-rw-   0        0        0     2600 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1752 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1845 2023-05-23 17:30:13.000000 MGP_SDK-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:01.000000 MGP_SDK-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:01.000000 MGP_SDK-1.1.1/src/MGP_SDK/
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/src/MGP_SDK/OGC_Spec/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/OGC_Spec/__init__.py
+-rw-rw-rw-   0        0        0    43398 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/OGC_Spec/interface.py
+-rw-rw-rw-   0        0        0     5567 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/OGC_Spec/wfs.py
+-rw-rw-rw-   0        0        0     4208 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/OGC_Spec/wms.py
+-rw-rw-rw-   0        0        0     7607 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/OGC_Spec/wmts.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/src/MGP_SDK/account_service/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/account_service/__init__.py
+-rw-rw-rw-   0        0        0     3911 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/account_service/accounts.py
+-rw-rw-rw-   0        0        0     3885 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/account_service/activations.py
+-rw-rw-rw-   0        0        0     5512 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/account_service/addresses.py
+-rw-rw-rw-   0        0        0     5759 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/account_service/interface.py
+-rw-rw-rw-   0        0        0     2823 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/account_service/products.py
+-rw-rw-rw-   0        0        0     3480 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/account_service/rate_tables.py
+-rw-rw-rw-   0        0        0     1172 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/account_service/roles.py
+-rw-rw-rw-   0        0        0     8249 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/account_service/usage.py
+-rw-rw-rw-   0        0        0     9173 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/account_service/users.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/src/MGP_SDK/analytics_service/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/analytics_service/__init__.py
+-rw-rw-rw-   0        0        0     6650 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/analytics_service/analytics.py
+-rw-rw-rw-   0        0        0     4900 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/analytics_service/interface.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/src/MGP_SDK/auth/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/auth/__init__.py
+-rw-rw-rw-   0        0        0     6387 2023-05-23 17:30:13.000000 MGP_SDK-1.1.1/src/MGP_SDK/auth/auth.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/src/MGP_SDK/basemap_service/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/basemap_service/__init__.py
+-rw-rw-rw-   0        0        0     1271 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/basemap_service/basemaps.py
+-rw-rw-rw-   0        0        0     7889 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/basemap_service/interface.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/src/MGP_SDK/discovery_service/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/discovery_service/__init__.py
+-rw-rw-rw-   0        0        0     7871 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/discovery_service/catalogs.py
+-rw-rw-rw-   0        0        0     7974 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/discovery_service/collections.py
+-rw-rw-rw-   0        0        0     6707 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/discovery_service/interface.py
+-rw-rw-rw-   0        0        0     3140 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/discovery_service/search.py
+-rw-rw-rw-   0        0        0     1241 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/discovery_service/server_checks.py
+-rw-rw-rw-   0        0        0     1913 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/interface.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/src/MGP_SDK/monitor_service/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/monitor_service/__init__.py
+-rw-rw-rw-   0        0        0     4098 2023-05-23 17:30:13.000000 MGP_SDK-1.1.1/src/MGP_SDK/monitor_service/interface.py
+-rw-rw-rw-   0        0        0     7352 2023-05-23 17:30:13.000000 MGP_SDK-1.1.1/src/MGP_SDK/monitor_service/monitoring.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/src/MGP_SDK/ordering_service/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/ordering_service/__init__.py
+-rw-rw-rw-   0        0        0     6264 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/ordering_service/interface.py
+-rw-rw-rw-   0        0        0     5932 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/ordering_service/orders.py
+-rw-rw-rw-   0        0        0     3353 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/ordering_service/pipelines.py
+-rw-rw-rw-   0        0        0    16857 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/process.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/src/MGP_SDK/streaming/
+-rw-rw-rw-   0        0        0        2 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/streaming/__init__.py
+-rw-rw-rw-   0        0        0     6571 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/streaming/cli_commands.py
+-rw-rw-rw-   0        0        0    10859 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/streaming/interface.py
+-rw-rw-rw-   0        0        0     3866 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/streaming/wcs_archive.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/src/MGP_SDK/tasking_service/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/tasking_service/__init__.py
+-rw-rw-rw-   0        0        0     3588 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/tasking_service/interface.py
+-rw-rw-rw-   0        0        0     5203 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/tasking_service/tasking.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/src/MGP_SDK/three_d/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/three_d/__init__.py
+-rw-rw-rw-   0        0        0     2183 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/three_d/interface.py
+-rw-rw-rw-   0        0        0     3460 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/three_d/three_d.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/src/MGP_SDK/token_service/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/token_service/__init__.py
+-rw-rw-rw-   0        0        0     3211 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/token_service/cli_commands.py
+-rw-rw-rw-   0        0        0     2929 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/token_service/token.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:02.000000 MGP_SDK-1.1.1/src/MGP_SDK/usage_service/
+-rw-rw-rw-   0        0        0        0 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/usage_service/__init__.py
+-rw-rw-rw-   0        0        0      702 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/usage_service/interface.py
+-rw-rw-rw-   0        0        0     1563 2023-05-23 16:45:45.000000 MGP_SDK-1.1.1/src/MGP_SDK/usage_service/usage.py
+drwxrwxrwx   0        0        0        0 2023-05-23 17:31:01.000000 MGP_SDK-1.1.1/src/MGP_SDK.egg-info/
+-rw-rw-rw-   0        0        0     2600 2023-05-23 17:31:01.000000 MGP_SDK-1.1.1/src/MGP_SDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2289 2023-05-23 17:31:01.000000 MGP_SDK-1.1.1/src/MGP_SDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 17:31:01.000000 MGP_SDK-1.1.1/src/MGP_SDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      461 2023-05-23 17:31:01.000000 MGP_SDK-1.1.1/src/MGP_SDK.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       65 2023-05-23 17:31:01.000000 MGP_SDK-1.1.1/src/MGP_SDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 17:31:01.000000 MGP_SDK-1.1.1/src/MGP_SDK.egg-info/top_level.txt
```

### Comparing `MGP_SDK-1.1.0/PKG-INFO` & `MGP_SDK-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGP_SDK
-Version: 1.1.0
+Version: 1.1.1
 Summary: SDK for interacting with Maxar Geospatial Platform
 Author: MDS Marianas Team
 Author-email: DL-GCS-Marianas@maxar.com
 License: MIT
 Project-URL: Documentation, https://maxar-geospatial-platform.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Maxar-Corp/maxar-geospatial-platform
 Keywords: OGC,WMS,WFS,WMTS,WCS,MAXAR,IMAGERY,GIS
```

### Comparing `MGP_SDK-1.1.0/README.md` & `MGP_SDK-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/setup.py` & `MGP_SDK-1.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent.resolve()
 
 README = (HERE / "README.md").read_text()
 
 setup(
   name = 'MGP_SDK',
-  version = '1.1.0',
+  version = '1.1.1',
   license='MIT',
   description = 'SDK for interacting with Maxar Geospatial Platform',
   long_description=README,
   long_description_content_type="text/markdown",
   author = 'MDS Marianas Team',
   author_email = 'DL-GCS-Marianas@maxar.com',
   project_urls = {
```

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/interface.py` & `MGP_SDK-1.1.1/src/MGP_SDK/OGC_Spec/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/wfs.py` & `MGP_SDK-1.1.1/src/MGP_SDK/OGC_Spec/wfs.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/wms.py` & `MGP_SDK-1.1.1/src/MGP_SDK/OGC_Spec/wms.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/OGC_Spec/wmts.py` & `MGP_SDK-1.1.1/src/MGP_SDK/OGC_Spec/wmts.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/account_service/accounts.py` & `MGP_SDK-1.1.1/src/MGP_SDK/account_service/accounts.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/account_service/activations.py` & `MGP_SDK-1.1.1/src/MGP_SDK/account_service/activations.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/account_service/addresses.py` & `MGP_SDK-1.1.1/src/MGP_SDK/account_service/addresses.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/account_service/interface.py` & `MGP_SDK-1.1.1/src/MGP_SDK/account_service/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/account_service/products.py` & `MGP_SDK-1.1.1/src/MGP_SDK/account_service/products.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/account_service/rate_tables.py` & `MGP_SDK-1.1.1/src/MGP_SDK/account_service/rate_tables.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/account_service/roles.py` & `MGP_SDK-1.1.1/src/MGP_SDK/account_service/roles.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/account_service/usage.py` & `MGP_SDK-1.1.1/src/MGP_SDK/account_service/usage.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/account_service/users.py` & `MGP_SDK-1.1.1/src/MGP_SDK/account_service/users.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/analytics_service/analytics.py` & `MGP_SDK-1.1.1/src/MGP_SDK/analytics_service/analytics.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/analytics_service/interface.py` & `MGP_SDK-1.1.1/src/MGP_SDK/analytics_service/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/auth/auth.py` & `MGP_SDK-1.1.1/src/MGP_SDK/auth/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.base_url = "https://account.maxar.com"
         self.api_base_url = "https://api.maxar.com"
         self.username = username
         self.password = password
         self.client_id = client_id
         self.access = None
         self.refresh = None
-        self.version = "Python1.1.0"
+        self.version = "Python1.1.1"
         self.api_version = 'v1'
         self.SSL = True
 
         if not self.username: #checks if username is provided as argument to class. If not, look for .MGP-config
             dir_path = os.path.expanduser('~')
             file = '.MGP-config'
             full_path = os.path.join(dir_path, file)
```

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/basemap_service/basemaps.py` & `MGP_SDK-1.1.1/src/MGP_SDK/basemap_service/basemaps.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/basemap_service/interface.py` & `MGP_SDK-1.1.1/src/MGP_SDK/basemap_service/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/catalogs.py` & `MGP_SDK-1.1.1/src/MGP_SDK/discovery_service/catalogs.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/collections.py` & `MGP_SDK-1.1.1/src/MGP_SDK/discovery_service/collections.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/interface.py` & `MGP_SDK-1.1.1/src/MGP_SDK/discovery_service/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/search.py` & `MGP_SDK-1.1.1/src/MGP_SDK/discovery_service/search.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/discovery_service/server_checks.py` & `MGP_SDK-1.1.1/src/MGP_SDK/discovery_service/server_checks.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/interface.py` & `MGP_SDK-1.1.1/src/MGP_SDK/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/monitor_service/interface.py` & `MGP_SDK-1.1.1/src/MGP_SDK/monitor_service/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,32 +10,33 @@
         client_id (string) = The client id associated with your user
     """
 
     def __init__(self, auth):
         self.auth = auth
         self.monitoring = Monitoring(self.auth)
 
-    def new_monitor(self, source: str, **kwargs):
+    def new_monitor(self, source: str, validate=False, **kwargs):
         """
         Creates a new monitor
         Args:
             source (string) = the ID of the event source to listen to
+            validate (bool) = Binary whether to validate tasking request. Defaults to False
         Kwargs:
             start_datetime (string) = ISO-8601-formatted datetime string indicating when the monitor should start
             end_datetime (string) = ISO-8601-formatted datetime string indicating when the monitor should end
             description (string) = A human-friendly description of the monitor
             intersects (dict) = A GeoJSON geometry indicating the area of interest for the monitor
             match_criteria (dict) = The fields and values to match against; criteria are specified using a JSON object
             monitor_notifications (list) = Destination(s) where notifications should be sent
             order_templates (list) = Orders to be placed automatically when an event matches the monitor's criteria
         Returns:
             JSON response
         """
 
-        return self.monitoring.create_new_monitor(source, **kwargs)
+        return self.monitoring.create_new_monitor(source, validate, **kwargs)
 
     def toggle_monitor_status(self, monitor_id: str, status: str):
         """
         Toggles the 'enabled' status of a monitor
         Args:
             monitor_id (string) = the ID of the monitor
             status (string) = enable or disable
@@ -43,15 +44,15 @@
             Whether the status change has been accepted
         Throws:
             Exception: If the status provided is already applied to the monitor
         """
 
         current_status = self.get_monitor(monitor_id)['data']['enabled']
         if (status == 'enable' and current_status is True) or (status == 'disable' and current_status is False):
-            raise Exception(f'Monitor {monitor_id} is already {status}ed.')
+            raise Exception(f'Monitor {monitor_id} is already {status}d.')
         return self.monitoring.toggle_monitor(monitor_id, status)
 
     def get_monitor(self, monitor_id: str):
         """
         Retrieves a monitor configuration
         Args:
             monitor_id (string) = the ID of the monitor
```

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/monitor_service/monitoring.py` & `MGP_SDK-1.1.1/src/MGP_SDK/monitor_service/monitoring.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,20 @@
     def __init__(self, auth: Auth):
         self.auth = auth
         self.api_version = self.auth.api_version
         self.base_url = f'{self.auth.api_base_url}/monitoring/{self.api_version}/monitors'
         self.token = self.auth.refresh_token()
         self.authorization = {"Authorization": f"Bearer {self.token}"}
 
-    def create_new_monitor(self, source: str, **kwargs):
+    def create_new_monitor(self, source: str, validate=False, **kwargs):
         """
         Creates a new monitor
         Args:
             source (string) = The ID of the event source to listen to
+            validate (bool) = Binary whether to validate tasking request. Defaults to False
         Kwargs:
             start_datetime (string) = ISO-8601-formatted datetime string indicating when the monitor should start
             end_datetime (string) = ISO-8601-formatted datetime string indicating when the monitor should end
             description (string) = A human-friendly description of the monitor
             intersects (dict) = A GeoJSON geometry indicating the area of interest for the monitor
             match_criteria (dict) = the fields and values to match against; criteria are specified using a JSON object
             monitor_notifications (list) = Destination(s) where notifications should be sent
@@ -42,15 +43,19 @@
         if 'end_date' in kwargs.keys():
             try:
                 datetime_string = datetime.fromisoformat(kwargs['end_date'])
             except:
                 raise Exception('Date is not properly formatted. eg: 2023-03-03T10:30:00.000Z')
         data = {**{k: v for k, v in kwargs.items() if k in parameter_list}}
         data.update({"source": source})
-        response = requests.post(self.base_url, data=json.dumps(data), headers=self.authorization, verify=self.auth.SSL)
+        if validate:
+            url = self.base_url + "?validation_only=true"
+        else:
+            url = self.base_url
+        response = requests.post(url, data=json.dumps(data), headers=self.authorization, verify=self.auth.SSL)
         process._response_handler(response)
         return response.json()
 
     def get_monitor_by_id(self, monitor_id: str):
         """
         Retrieve a monitor configuration for a desired monitor
         Args:
@@ -73,15 +78,15 @@
         Returns:
             Dictionary of the desired monitor's status
         """
 
         url = f'{self.base_url}/{monitor_id}/{status}'
         response = requests.post(url, headers=self.authorization, verify=self.auth.SSL)
         process._response_handler(response)
-        if response.status_code == '200':
+        if response.status_code == 200:
             return 'Status change accepted'
 
     def monitor_list(self, **kwargs):
         """
         Retrieves a list of monitor configurations
         Kwargs:
             limit (int) = Number of monitors to return, defaults to 10
@@ -104,15 +109,15 @@
         if 'filter' in kwargs.keys():
             for filter in kwargs['filter']:
                 try:
                     k, v = filter.split(":")
                 except:
                     raise Exception("Filter must be a key value pair separated by a colon (:) " + filter)
         if 'sort' in kwargs.keys():
-            if kwargs['sort'] is not 'asc' or kwargs['sort'] is not 'desc':
+            if kwargs['sort'] != 'asc' and kwargs['sort'] != 'desc':
                 raise Exception('sort must be either asc or desc. ' + kwargs['sort'])
         params = {}
         kwarg_list = ["limit", "filter", "sort"]
         for k, v in kwargs.items():
             if k in kwarg_list:
                 params[k] = v
         response = requests.get(self.base_url, params=params, headers=self.authorization, verify=self.auth.SSL)
```

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/interface.py` & `MGP_SDK-1.1.1/src/MGP_SDK/ordering_service/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/orders.py` & `MGP_SDK-1.1.1/src/MGP_SDK/ordering_service/orders.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/ordering_service/pipelines.py` & `MGP_SDK-1.1.1/src/MGP_SDK/ordering_service/pipelines.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/process.py` & `MGP_SDK-1.1.1/src/MGP_SDK/process.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/streaming/cli_commands.py` & `MGP_SDK-1.1.1/src/MGP_SDK/streaming/cli_commands.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/streaming/interface.py` & `MGP_SDK-1.1.1/src/MGP_SDK/streaming/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/streaming/wcs_archive.py` & `MGP_SDK-1.1.1/src/MGP_SDK/streaming/wcs_archive.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/tasking_service/interface.py` & `MGP_SDK-1.1.1/src/MGP_SDK/tasking_service/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/tasking_service/tasking.py` & `MGP_SDK-1.1.1/src/MGP_SDK/tasking_service/tasking.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/three_d/interface.py` & `MGP_SDK-1.1.1/src/MGP_SDK/three_d/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/three_d/three_d.py` & `MGP_SDK-1.1.1/src/MGP_SDK/three_d/three_d.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/token_service/cli_commands.py` & `MGP_SDK-1.1.1/src/MGP_SDK/token_service/cli_commands.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/token_service/token.py` & `MGP_SDK-1.1.1/src/MGP_SDK/token_service/token.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/usage_service/interface.py` & `MGP_SDK-1.1.1/src/MGP_SDK/usage_service/interface.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK/usage_service/usage.py` & `MGP_SDK-1.1.1/src/MGP_SDK/usage_service/usage.py`

 * *Files identical despite different names*

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK.egg-info/PKG-INFO` & `MGP_SDK-1.1.1/src/MGP_SDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MGP-SDK
-Version: 1.1.0
+Version: 1.1.1
 Summary: SDK for interacting with Maxar Geospatial Platform
 Author: MDS Marianas Team
 Author-email: DL-GCS-Marianas@maxar.com
 License: MIT
 Project-URL: Documentation, https://maxar-geospatial-platform.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/Maxar-Corp/maxar-geospatial-platform
 Keywords: OGC,WMS,WFS,WMTS,WCS,MAXAR,IMAGERY,GIS
```

### Comparing `MGP_SDK-1.1.0/src/MGP_SDK.egg-info/SOURCES.txt` & `MGP_SDK-1.1.1/src/MGP_SDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

