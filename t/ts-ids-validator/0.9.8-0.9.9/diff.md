# Comparing `tmp/ts-ids-validator-0.9.8.tar.gz` & `tmp/ts-ids-validator-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/tarik.setia/tetrascience/ids-validator/dist/tmp_jwuzy99/ts-ids-validator-0.9.8.tar", last modified: Tue Dec 14 09:20:15 2021, max compression
+gzip compressed data, was "/Users/tarik.setia/tetrascience/ids-validator/dist/tmp6bfhjhp9/ts-ids-validator-0.9.9.tar", last modified: Fri Jan  7 04:17:32 2022, max compression
```

## Comparing `ts-ids-validator-0.9.8.tar` & `ts-ids-validator-0.9.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/
--rw-r--r--   0 tarik.setia (472973718) 1138207179    11357 2021-10-25 07:28:08.000000 ts-ids-validator-0.9.8/LICENSE
--rw-r--r--   0 tarik.setia (472973718) 1138207179      111 2021-11-08 11:19:16.000000 ts-ids-validator-0.9.8/MANIFEST.in
--rw-r--r--   0 tarik.setia (472973718) 1138207179     8777 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/PKG-INFO
--rw-r--r--   0 tarik.setia (472973718) 1138207179     8188 2021-12-14 09:19:01.000000 ts-ids-validator-0.9.8/README.md
-drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/ids_validator/
--rw-r--r--   0 tarik.setia (472973718) 1138207179        0 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/__init__.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179      727 2021-11-23 05:48:31.000000 ts-ids-validator-0.9.8/ids_validator/__main__.py
-drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/ids_validator/checks/
--rw-r--r--   0 tarik.setia (472973718) 1138207179     1130 2021-11-23 05:48:31.000000 ts-ids-validator-0.9.8/ids_validator/checks/__init__.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179      232 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/abstract_checker.py
-drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/ids_validator/checks/generic/
--rw-r--r--   0 tarik.setia (472973718) 1138207179      508 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/generic/__init__.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     1029 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/generic/additional_property.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     7569 2021-11-23 05:48:31.000000 ts-ids-validator-0.9.8/ids_validator/checks/generic/athena.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179    11011 2021-12-14 09:19:01.000000 ts-ids-validator-0.9.8/ids_validator/checks/generic/datacubes.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     3337 2021-11-08 11:01:39.000000 ts-ids-validator-0.9.8/ids_validator/checks/generic/elasticsearch.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179      757 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/generic/required_property.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     1456 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/generic/root_node.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179      550 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/generic/type_check.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     4761 2021-12-14 09:19:01.000000 ts-ids-validator-0.9.8/ids_validator/checks/rules_checker.py
-drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/
--rw-r--r--   0 tarik.setia (472973718) 1138207179      489 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/__init__.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179      716 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/child_name.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179      594 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/convention_version_check.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179      467 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/nodes_checker.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     1122 2021-11-08 11:08:34.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/related_files_checker.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     1016 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/root_node.py
-drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/rules/
-drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/rules/samples/
--rw-r--r--   0 tarik.setia (472973718) 1138207179      494 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/rules/samples/__init__.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     2032 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/rules/samples/sample_properties.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     1174 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/rules/samples/samples_labels.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     1110 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/rules/samples/samples_location.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     2730 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/rules/samples/samples_root.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     2516 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/rules/systems.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179      537 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/rules/users.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     1147 2021-11-08 07:58:00.000000 ts-ids-validator-0.9.8/ids_validator/checks/v1/snake_case.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179      427 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/ids_validator/convention_versions.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     6603 2021-12-08 21:04:51.000000 ts-ids-validator-0.9.8/ids_validator/ids_node.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     3498 2021-11-10 14:40:17.000000 ts-ids-validator-0.9.8/ids_validator/ids_validator.py
-drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/ids_validator/templates/
--rw-r--r--   0 tarik.setia (472973718) 1138207179      378 2021-11-23 05:48:31.000000 ts-ids-validator-0.9.8/ids_validator/templates/athena.json
--rw-r--r--   0 tarik.setia (472973718) 1138207179     1816 2021-11-08 11:08:34.000000 ts-ids-validator-0.9.8/ids_validator/templates/related_files.json
--rw-r--r--   0 tarik.setia (472973718) 1138207179      573 2021-11-23 05:48:31.000000 ts-ids-validator-0.9.8/ids_validator/utils.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179     1826 2021-11-10 14:40:17.000000 ts-ids-validator-0.9.8/ids_validator/validator.py
--rw-r--r--   0 tarik.setia (472973718) 1138207179      103 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.8/pyproject.toml
--rw-r--r--   0 tarik.setia (472973718) 1138207179      758 2021-11-23 05:48:31.000000 ts-ids-validator-0.9.8/requirements.txt
--rw-r--r--   0 tarik.setia (472973718) 1138207179       38 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/setup.cfg
--rw-r--r--   0 tarik.setia (472973718) 1138207179     1207 2021-12-14 09:19:01.000000 ts-ids-validator-0.9.8/setup.py
-drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/ts_ids_validator.egg-info/
--rw-r--r--   0 tarik.setia (472973718) 1138207179     8777 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/ts_ids_validator.egg-info/PKG-INFO
--rw-r--r--   0 tarik.setia (472973718) 1138207179     1659 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/ts_ids_validator.egg-info/SOURCES.txt
--rw-r--r--   0 tarik.setia (472973718) 1138207179        1 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/ts_ids_validator.egg-info/dependency_links.txt
--rw-r--r--   0 tarik.setia (472973718) 1138207179      537 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/ts_ids_validator.egg-info/requires.txt
--rw-r--r--   0 tarik.setia (472973718) 1138207179       14 2021-12-14 09:20:15.000000 ts-ids-validator-0.9.8/ts_ids_validator.egg-info/top_level.txt
+drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2022-01-07 04:17:32.000000 ts-ids-validator-0.9.9/
+-rw-r--r--   0 tarik.setia (472973718) 1138207179    11357 2021-10-25 07:28:08.000000 ts-ids-validator-0.9.9/LICENSE
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      111 2021-11-08 11:19:16.000000 ts-ids-validator-0.9.9/MANIFEST.in
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     8837 2022-01-07 04:17:32.000000 ts-ids-validator-0.9.9/PKG-INFO
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     8248 2022-01-07 04:14:44.000000 ts-ids-validator-0.9.9/README.md
+drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2022-01-07 04:17:32.000000 ts-ids-validator-0.9.9/ids_validator/
+-rw-r--r--   0 tarik.setia (472973718) 1138207179        0 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.9/ids_validator/__init__.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      783 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/__main__.py
+drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2022-01-07 04:17:32.000000 ts-ids-validator-0.9.9/ids_validator/checks/
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     1131 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/__init__.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      232 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.9/ids_validator/checks/abstract_checker.py
+drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2022-01-07 04:17:32.000000 ts-ids-validator-0.9.9/ids_validator/checks/generic/
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      509 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/generic/__init__.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     1111 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/generic/additional_property.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     7664 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/generic/athena.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179    11134 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/generic/datacubes.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     3242 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/generic/elasticsearch.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      828 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/generic/required_property.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     1492 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/generic/root_node.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      550 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.9/ids_validator/checks/generic/type_check.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     4478 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/rules_checker.py
+drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2022-01-07 04:17:32.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      491 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/__init__.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      747 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/child_name.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      665 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/convention_version_check.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      467 2021-11-05 12:58:59.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/nodes_checker.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     1225 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/related_files_checker.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     1088 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/root_node.py
+drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2022-01-07 04:17:32.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/rules/
+drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2022-01-07 04:17:32.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/rules/samples/
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      513 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/rules/samples/__init__.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     1843 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/rules/samples/sample_properties.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      983 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/rules/samples/samples_labels.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      903 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/rules/samples/samples_location.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     2345 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/rules/samples/samples_root.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     2248 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/rules/systems.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      428 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/rules/users.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     1032 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/checks/v1/snake_case.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      393 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/convention_versions.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     5997 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/ids_node.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     3465 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/ids_validator.py
+drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2022-01-07 04:17:32.000000 ts-ids-validator-0.9.9/ids_validator/templates/
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      378 2021-11-23 05:48:31.000000 ts-ids-validator-0.9.9/ids_validator/templates/athena.json
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     1816 2021-11-08 11:08:34.000000 ts-ids-validator-0.9.9/ids_validator/templates/related_files.json
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      515 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/utils.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     1797 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/ids_validator/validator.py
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      226 2022-01-06 06:55:04.000000 ts-ids-validator-0.9.9/pyproject.toml
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      787 2022-01-07 04:14:44.000000 ts-ids-validator-0.9.9/requirements.txt
+-rw-r--r--   0 tarik.setia (472973718) 1138207179       38 2022-01-07 04:17:32.000000 ts-ids-validator-0.9.9/setup.cfg
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     1178 2022-01-07 04:14:44.000000 ts-ids-validator-0.9.9/setup.py
+drwxr-xr-x   0 tarik.setia (472973718) 1138207179        0 2022-01-07 04:17:32.000000 ts-ids-validator-0.9.9/ts_ids_validator.egg-info/
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     8837 2022-01-07 04:17:31.000000 ts-ids-validator-0.9.9/ts_ids_validator.egg-info/PKG-INFO
+-rw-r--r--   0 tarik.setia (472973718) 1138207179     1659 2022-01-07 04:17:31.000000 ts-ids-validator-0.9.9/ts_ids_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 tarik.setia (472973718) 1138207179        1 2022-01-07 04:17:31.000000 ts-ids-validator-0.9.9/ts_ids_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 tarik.setia (472973718) 1138207179      538 2022-01-07 04:17:31.000000 ts-ids-validator-0.9.9/ts_ids_validator.egg-info/requires.txt
+-rw-r--r--   0 tarik.setia (472973718) 1138207179       14 2022-01-07 04:17:31.000000 ts-ids-validator-0.9.9/ts_ids_validator.egg-info/top_level.txt
```

### Comparing `ts-ids-validator-0.9.8/LICENSE` & `ts-ids-validator-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ts-ids-validator-0.9.8/PKG-INFO` & `ts-ids-validator-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-ids-validator
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python utility for validating IDS
 Home-page: https://github.com/tetrascience/ts-ids-validator
 Author: tetrascience
 Author-email: developers@tetrascience.com
 License: Apache License 2.0
 Project-URL: Tetra Developer Site, https://developers.tetrascience.com
 Platform: UNKNOWN
@@ -207,14 +207,18 @@
 ### List of Checks for Validator
 
 - `checks_dict`, defined [here](src/checks/__init__.py), maps the `type of validation` that we want to perform to the `list the of checks` needed to be run for the validation
 - The list off checks is actually a list of instantiated checker objects
 
 ## Changelog
 
+## v0.9.9
+
+- Lock `jsonschema` version in requirements.txt
+
 ## v0.9.8
 
 - Modify `RulesChecker` to log missing and extra properties
 
 ## v0.9.7
 
 - Allow properties with `const` values to have non-nullable `type`
```

### Comparing `ts-ids-validator-0.9.8/README.md` & `ts-ids-validator-0.9.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -190,14 +190,18 @@
 ### List of Checks for Validator
 
 - `checks_dict`, defined [here](src/checks/__init__.py), maps the `type of validation` that we want to perform to the `list the of checks` needed to be run for the validation
 - The list off checks is actually a list of instantiated checker objects
 
 ## Changelog
 
+## v0.9.9
+
+- Lock `jsonschema` version in requirements.txt
+
 ## v0.9.8
 
 - Modify `RulesChecker` to log missing and extra properties
 
 ## v0.9.7
 
 - Allow properties with `const` values to have non-nullable `type`
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/__init__.py` & `ts-ids-validator-0.9.9/ids_validator/checks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,25 @@
     V1ChildNameChecker,
     V1ConventionVersionChecker,
     V1RootNodeChecker,
     V1SnakeCaseChecker,
     V1SampleNodeChecker,
     V1SystemNodeChecker,
     V1UserNodeChecker,
-    V1RelatedFilesChecker
+    V1RelatedFilesChecker,
 )
 
 generic_checks = [
     AdditionalPropertyChecker(),
     DatacubesChecker(),
     RequiredPropertiesChecker(),
     RootNodeChecker(),
     TypeChecker(),
     ElasticsearchChecker(),
-    AthenaChecker()
+    AthenaChecker(),
 ]
 
 v1_checks = generic_checks + [
     V1ChildNameChecker(),
     V1ConventionVersionChecker(),
     V1RootNodeChecker(),
     V1SnakeCaseChecker(),
@@ -40,9 +40,9 @@
     V1UserNodeChecker(),
     V1RelatedFilesChecker(),
 ]
 
 
 checks_dict = {
     Conventions.GENERIC: generic_checks,
-    Conventions.V1_0_0 : v1_checks,
+    Conventions.V1_0_0: v1_checks,
 }
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/generic/additional_property.py` & `ts-ids-validator-0.9.9/ids_validator/checks/generic/additional_property.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,24 +10,27 @@
     If type is not object or is not defined, additionalProperties
     must not exist.
     """
 
     def run(self, node: Node, context: dict = None):
         logs = []
 
-        if (
-            node.get("type") != 'object'
-            and "additionalProperties" in node
-        ):
+        if node.get("type") != "object" and "additionalProperties" in node:
             logs.append(
-                ("'additionalProperties' can only be defined for 'type = object'", Log.CRITICAL.value)
+                (
+                    "'additionalProperties' can only be defined for 'type = object'",
+                    Log.CRITICAL.value,
+                )
             )
 
         if (
-            node.get("type") == 'object'
+            node.get("type") == "object"
             and node.get("additionalProperties") is not False
         ):
             logs.append(
-                ("'additionalProperties' must be present and set to 'false' for 'object' types", Log.CRITICAL.value)
+                (
+                    "'additionalProperties' must be present and set to 'false' for 'object' types",
+                    Log.CRITICAL.value,
+                )
             )
 
         return logs
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/generic/athena.py` & `ts-ids-validator-0.9.9/ids_validator/checks/generic/athena.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,69 +20,68 @@
     - Ancestor of any `partition.path` is not an array
     """
 
     def run(self, node: Node, context: dict = None):
         logs = []
         if node.name == "root":
             if not context.get("athena.json"):
-                logs += [("Make sure athena.js exist in IDS folder and has correct structure.", Log.CRITICAL.value)]
+                logs += [
+                    (
+                        "Make sure athena.js exist in IDS folder and has correct structure.",
+                        Log.CRITICAL.value,
+                    )
+                ]
 
             athena = context.get("athena.json")
             ids = context.get("schema.json")
             ids_node = Node(ids)
 
             logs += self._validate_schema(athena)
             if logs:
                 return logs
 
             partition_paths = self.get_athena_partitions_path(athena)
             logs += self.check_all_paths_exist(partition_paths, ids_node)
-            logs += self.check_paths_nested_inside_array(
-                partition_paths, ids_node)
+            logs += self.check_paths_nested_inside_array(partition_paths, ids_node)
             logs += self.check_path_and_name_conflicts(athena)
-            logs += self.check_athena_path_and_root_properties_conflict(
-                ids, athena)
+            logs += self.check_athena_path_and_root_properties_conflict(ids, athena)
 
         return logs
 
     @classmethod
     def check_all_paths_exist(cls, partition_paths: list, ids: Node):
         logs = []
-        missing = [
-            path
-            for path in partition_paths
-            if not cls.path_exists(path, ids)
-        ]
+        missing = [path for path in partition_paths if not cls.path_exists(path, ids)]
         if missing:
             logs.append(
                 (
                     f"Athena.js: Cannot find following properties in IDS: {sorted(missing)}",
-                    Log.CRITICAL.value
+                    Log.CRITICAL.value,
                 )
             )
         return logs
 
     @classmethod
     def check_paths_nested_inside_array(cls, partition_paths: list, ids: Node):
         logs = []
         existing_partition_paths = [
-            path
-            for path in partition_paths
-            if cls.path_exists(path, ids)
+            path for path in partition_paths if cls.path_exists(path, ids)
         ]
-        paths_nested_inside_array = sorted([
-            path
-            for path in existing_partition_paths
-            if cls.path_nested_in_array(path, ids)
-        ])
+        paths_nested_inside_array = sorted(
+            [
+                path
+                for path in existing_partition_paths
+                if cls.path_nested_in_array(path, ids)
+            ]
+        )
         if paths_nested_inside_array:
             logs.append(
                 (
                     f"Athena.js: Following paths are either array type or nested in array types: {paths_nested_inside_array}",
-                    Log.CRITICAL.value
+                    Log.CRITICAL.value,
                 )
             )
         return logs
 
     @classmethod
     def check_path_and_name_conflicts(cls, athena_dict: dict):
         """Check and log if there is a conflict in `partition.path`
@@ -94,44 +93,52 @@
         Normalized path is obtained by replacing "." with "_" in `partiions[*].path`
 
         Args:
             athena_dict (Node): athena.json loaded as a python dict
         """
         logs = []
         partitions_name = set(cls.get_athena_partitions_name(athena_dict))
-        normalized_paths = set([
-            cls.normalize_path_name(path)
-            for path in cls.get_athena_partitions_path(athena_dict)
-        ])
+        normalized_paths = set(
+            [
+                cls.normalize_path_name(path)
+                for path in cls.get_athena_partitions_path(athena_dict)
+            ]
+        )
         intersection = partitions_name.intersection(normalized_paths)
         if intersection:
             logs.append(
-                (f"Athena.js: Following names are conflicting with path: {', '.join(intersection)}", Log.CRITICAL.value)
+                (
+                    f"Athena.js: Following names are conflicting with path: {', '.join(intersection)}",
+                    Log.CRITICAL.value,
+                )
             )
         return logs
 
     @classmethod
     def check_athena_path_and_root_properties_conflict(cls, ids_dict, athena_dict):
         """Normalized partition path must not be a root level
         ids property."""
         logs = []
 
         ids_top_level_props = set(ids_dict.get("properties", {}).keys())
-        athena_normalized_paths = set([
-            cls.normalize_path_name(path)
-            for path in cls.get_athena_partitions_path(athena_dict)
-        ])
-
-        intersection = ids_top_level_props.intersection(
-            athena_normalized_paths
+        athena_normalized_paths = set(
+            [
+                cls.normalize_path_name(path)
+                for path in cls.get_athena_partitions_path(athena_dict)
+            ]
         )
+
+        intersection = ids_top_level_props.intersection(athena_normalized_paths)
         intersection = sorted(list(intersection))
         if intersection:
             logs.append(
-                (f"Athena.js: Following athena paths are in conflict with top level properties in IDS schema: {intersection}", Log.CRITICAL.value)
+                (
+                    f"Athena.js: Following athena paths are in conflict with top level properties in IDS schema: {intersection}",
+                    Log.CRITICAL.value,
+                )
             )
 
         return logs
 
     @classmethod
     def path_nested_in_array(cls, path: str, ids: Node):
         """Traverse on node's path and return True if any
@@ -139,17 +146,16 @@
         IDS property.
         """
         nodes = path.split(".")
         parent = ids
         for idx, node in enumerate(nodes):
             children = parent.properties_dict
             child = children.get(node)
-            if (
-                (parent["type"] == 'array' and idx > 1)
-                or (child["type"] == "array" and idx > 0)
+            if (parent["type"] == "array" and idx > 1) or (
+                child["type"] == "array" and idx > 0
             ):
                 return True
 
             parent = Node(child, path=None)
         return False
 
     @classmethod
@@ -174,27 +180,21 @@
                 return False
             parent = Node(child, path=None)
         return True
 
     @classmethod
     def get_athena_partitions_path(cls, athena_schema) -> list:
         partitions = athena_schema.get("partitions", {})
-        paths = [
-            partition.get("path")
-            for partition in partitions
-        ]
+        paths = [partition.get("path") for partition in partitions]
         return paths
 
     @classmethod
     def get_athena_partitions_name(cls, athena_schema) -> list:
         partitions = athena_schema.get("partitions", {})
-        names = [
-            partition.get("name")
-            for partition in partitions
-        ]
+        names = [partition.get("name") for partition in partitions]
         return names
 
     @classmethod
     def normalize_path_name(cls, path_name):
         """
         Weird-partition!@name -> weird_partition_name
         @fileId -> fileid
@@ -205,21 +205,19 @@
         normalized_path = normalized_path.lstrip("_")
         normalized_path = normalized_path.lower()
         return normalized_path
 
     def _validate_schema(self, athena_schema):
         logs = []
         if not ATHENA_TEMPLATE.exists():
-            logs += [(
-                f"Could not find athena template : {ATHENA_TEMPLATE}", Log.CRITICAL
-            )]
+            logs += [
+                (f"Could not find athena template : {ATHENA_TEMPLATE}", Log.CRITICAL)
+            ]
             return logs
 
         template_schema = read_schema(ATHENA_TEMPLATE)
         try:
-            validate(athena_schema,template_schema)
+            validate(athena_schema, template_schema)
         except Exception as e:
             msg = str(e).split("\n")[0]
-            logs += [(
-                f"JSON schema validation failed : {msg}", Log.CRITICAL
-            )]
-        return logs
+            logs += [(f"JSON schema validation failed : {msg}", Log.CRITICAL)]
+        return logs
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/generic/datacubes.py` & `ts-ids-validator-0.9.9/ids_validator/checks/generic/datacubes.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,41 @@
 VALUE_NODE = "items.properties.measures.items.properties.value"
 DIMENSION_NODE = "items.properties.dimensions"
 SCALES_NODE = "items.properties.dimensions.items.properties.scale"
 
 
 class Message(Enum):
     TYPE_CHECK = "'type' must be an array"
-    REQUIRED_CHECK = "'required' must exist and contain at least ['name','measures','dimensions']"
+    REQUIRED_CHECK = (
+        "'required' must exist and contain at least ['name','measures','dimensions']"
+    )
     PROPERTY_CHECK = "'properties' must exist and contain all the required properties"
     MEASURES_UNDEFINED = "'measures' must be defined and 'measures.type' must be array"
     MEASURE_MIN_MAX_CHECK = "measures.minItems must be equal to measures.maxItems"
-    MEASURE_MIN_MAX_MISSING = "'measures' must have both 'minItems' and 'maxItems' defined"
-    DIMENSIONS_MIN_MAX_MISSING = "'dimension' must have both 'minItems' and 'maxItems' defined"
-    DIMENSIONS_UNDEFINED = "'dimensions' must be defined and 'dimension.type' must be array"
-    DIMENSIONS_MIN_MAX_CHECK = "dimensions.minItems must be equal to dimensions.maxItems"
+    MEASURE_MIN_MAX_MISSING = (
+        "'measures' must have both 'minItems' and 'maxItems' defined"
+    )
+    DIMENSIONS_MIN_MAX_MISSING = (
+        "'dimension' must have both 'minItems' and 'maxItems' defined"
+    )
+    DIMENSIONS_UNDEFINED = (
+        "'dimensions' must be defined and 'dimension.type' must be array"
+    )
+    DIMENSIONS_MIN_MAX_CHECK = (
+        "dimensions.minItems must be equal to dimensions.maxItems"
+    )
     MEASURES_VALUES_DIMENSIONALITY_ERROR = "'measures.value': Dimensionality of data stored in `measures.value` must be equal to `dimensions.minItems` or `dimensions.maxItems`"
     MEASURES_VALUES_TYPE_ERROR = "'measures.value': Type Error. Type must be either be `number` or `string`. It can be nullable"
-    MEASURES_VALUES_NESTED_ARRAY_TYPE_ERROR = "'measures.value': Type Error. Nested objects/dicts must be `array` types"
+    MEASURES_VALUES_NESTED_ARRAY_TYPE_ERROR = (
+        "'measures.value': Type Error. Nested objects/dicts must be `array` types"
+    )
     DIMENSIONS_SCALE_TYPE_ERROR = "'dimensions.scale': Type Error. Type must be 'array'"
-    DIMENSIONS_SCALE_ITEMS_TYPE_ERROR = "'dimensions.scale.items': Type Error. Type must be 'number'"
+    DIMENSIONS_SCALE_ITEMS_TYPE_ERROR = (
+        "'dimensions.scale.items': Type Error. Type must be 'number'"
+    )
 
     def __str__(self):
         return self.value
 
 
 class DatacubesChecker(AbstractChecker):
     """It run only when `node.path == "root.properties.datacubes"` and
@@ -78,20 +92,20 @@
         """
         logs = []
         items = datacubes.get("items")
 
         if not items or (type(items) != dict):
             logs += [
                 (Message.REQUIRED_CHECK.value, Log.CRITICAL.value),
-                (Message.PROPERTY_CHECK.value, Log.CRITICAL.value)
+                (Message.PROPERTY_CHECK.value, Log.CRITICAL.value),
             ]
             return logs
 
         items = Node(items)
-        minimum_required = {'name', 'dimensions', 'measures'}
+        minimum_required = {"name", "dimensions", "measures"}
 
         if not items.required_contains_values(minimum_required):
             logs += [(Message.REQUIRED_CHECK.value, Log.CRITICAL.value)]
 
         if not items.has_properties(list(minimum_required)):
             logs += [(Message.PROPERTY_CHECK.value, Log.CRITICAL.value)]
 
@@ -114,19 +128,19 @@
         """
         logs = []
         measures = get(datacubes, "items.properties.measures")
         if not measures:
             logs += [(Message.MEASURES_UNDEFINED.value, Log.CRITICAL.value)]
             return logs
 
-        if measures.get("type") != 'array':
+        if measures.get("type") != "array":
             logs += [(Message.MEASURES_UNDEFINED.value, Log.CRITICAL.value)]
 
-        minItems = get(measures, 'minItems')
-        maxItems = get(measures, 'maxItems')
+        minItems = get(measures, "minItems")
+        maxItems = get(measures, "maxItems")
 
         if all([minItems, maxItems]):
             if minItems != maxItems:
                 logs += [(Message.MEASURE_MIN_MAX_CHECK.value, Log.CRITICAL.value)]
         else:
             logs += [(Message.MEASURE_MIN_MAX_MISSING.value, Log.CRITICAL.value)]
         return list(set(logs))
@@ -148,19 +162,19 @@
         """
         logs = []
         dimensions = get(datacubes, "items.properties.dimensions")
         if not dimensions:
             logs += [(Message.DIMENSIONS_UNDEFINED.value, Log.CRITICAL.value)]
             return logs
 
-        if dimensions.get('type') != 'array':
+        if dimensions.get("type") != "array":
             logs += [(Message.DIMENSIONS_UNDEFINED.value, Log.CRITICAL.value)]
 
-        minItems = get(dimensions, 'minItems')
-        maxItems = get(dimensions, 'maxItems')
+        minItems = get(dimensions, "minItems")
+        maxItems = get(dimensions, "maxItems")
 
         if all([minItems, maxItems]):
             if minItems != maxItems:
                 logs += [(Message.DIMENSIONS_MIN_MAX_CHECK.value, Log.CRITICAL.value)]
         else:
             logs += [(Message.DIMENSIONS_MIN_MAX_MISSING.value, Log.CRITICAL.value)]
 
@@ -176,30 +190,31 @@
         Returns:
             list: list of failed check
         """
         logs = []
         values = get(datacubes, VALUE_NODE)
         dimensions = get(datacubes, DIMENSION_NODE)
 
-        num_dimensions = (
-            get(dimensions, "minItems")
-            or get(dimensions, "maxItems")
-        )
+        num_dimensions = get(dimensions, "minItems") or get(dimensions, "maxItems")
         if not (
             (values and type(values) == dict)
             and (dimensions and type(dimensions) == dict)
             and num_dimensions
         ):
-            logs += [(Message.MEASURES_VALUES_DIMENSIONALITY_ERROR.value, Log.CRITICAL.value)]
+            logs += [
+                (Message.MEASURES_VALUES_DIMENSIONALITY_ERROR.value, Log.CRITICAL.value)
+            ]
             return logs
 
         value_dimensions = cls.get_value_dimensions(values)
 
         if num_dimensions != value_dimensions:
-            logs += [(Message.MEASURES_VALUES_DIMENSIONALITY_ERROR.value, Log.CRITICAL.value)]
+            logs += [
+                (Message.MEASURES_VALUES_DIMENSIONALITY_ERROR.value, Log.CRITICAL.value)
+            ]
 
         return list(set(logs))
 
     @classmethod
     def check_measures_values_type(cls, datacubes: Node) -> list:
         """It makes sure that `measures.values` is a nested `dicts` of `array`,
         with innermost `dict` being a `number` or `string` type, nullable or not.
@@ -232,21 +247,19 @@
         scale = get(datacubes, SCALES_NODE, {})
         if not scale:
             logs += [(Message.DIMENSIONS_SCALE_TYPE_ERROR.value, Log.CRITICAL.value)]
 
         if get(scale, "type") != "array":
             logs += [(Message.DIMENSIONS_SCALE_TYPE_ERROR.value, Log.CRITICAL.value)]
 
-        valid_items_type =[
-            "number",
-            ["null", "number"],
-            ["number", "null"]
-        ]
+        valid_items_type = ["number", ["null", "number"], ["number", "null"]]
         if get(scale, "items.type") not in valid_items_type:
-            logs += [(Message.DIMENSIONS_SCALE_ITEMS_TYPE_ERROR.value, Log.CRITICAL.value)]
+            logs += [
+                (Message.DIMENSIONS_SCALE_ITEMS_TYPE_ERROR.value, Log.CRITICAL.value)
+            ]
 
         return list(set(logs))
 
     @classmethod
     def get_value_dimensions(cls, node) -> int:
         """Calculate Depth of nesting only for `measures.value`.
 
@@ -280,16 +293,16 @@
         node_type = get(node, "type")
         if node_items:
             if node_type != "array":
                 return True, Message.MEASURES_VALUES_NESTED_ARRAY_TYPE_ERROR
             return cls._check_measures_value_for_type_error(node_items)
         else:
             if type(node_type) == list:
-                if not(sorted(node_type) in [
-                    sorted(["null", "string"]),
-                    sorted(["null", "number"])
-                ]):
+                if not (
+                    sorted(node_type)
+                    in [sorted(["null", "string"]), sorted(["null", "number"])]
+                ):
                     return True, Message.MEASURES_VALUES_TYPE_ERROR
             elif node_type not in ["string", "number"]:
                 return True, Message.MEASURES_VALUES_TYPE_ERROR
 
         return False, None
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/generic/elasticsearch.py` & `ts-ids-validator-0.9.9/ids_validator/checks/generic/elasticsearch.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,87 +16,79 @@
     """
     - copy schema.json to temp folder
     - create elasticsearch.json in tmp folder
     - compare tmp/elasticsearch.json and ids/elasticsearch.json
     """
 
     def run(self, node: Node, context: dict = None):
-        if node.path != 'root':
+        if node.path != "root":
             return []
 
         logs = []
         ids_dir: Path = context["ids_folder_path"]
         elasticsearch_json = ids_dir / "elasticsearch.json"
         convention_version = context.get("convention_version", "generic")
 
         criticality = (
-            Log.WARNING.value
-            if convention_version == "generic"
-            else Log.CRITICAL.value
+            Log.WARNING.value if convention_version == "generic" else Log.CRITICAL.value
         )
 
         # Make sure elasticsearch.json exist
         if not elasticsearch_json.exists():
-            logs += [(
-                f"Make sure elasticsearch.json exist at {elasticsearch_json}",
-                criticality
-            )]
+            logs += [
+                (
+                    f"Make sure elasticsearch.json exist at {elasticsearch_json}",
+                    criticality,
+                )
+            ]
             return logs
 
         # Create a temp folder, copy ids/schema.json in it.
         # Generate a new elasticsearch.json in it
         try:
             with tempfile.TemporaryDirectory() as temp_ids_dir:
-                shutil.copy(
-                    ids_dir / "schema.json",
-                    temp_ids_dir
-                )
+                shutil.copy(ids_dir / "schema.json", temp_ids_dir)
                 self._create_new_elasticsearch_json(Path(temp_ids_dir))
                 tmp_es_json = Path(temp_ids_dir) / "elasticsearch.json"
                 original_es_schema = read_schema(elasticsearch_json)
                 generated_es_schema = read_schema(tmp_es_json)
         except Exception as e:
             msg = f"ElasticsearchChecker: Internal Error: {repr(e)}"
             logs += [(msg, criticality)]
             return logs
 
         # Get ES mappings
         original_mapping = json.dumps(
-            original_es_schema.get("mapping", {}),
-            indent=2
+            original_es_schema.get("mapping", {}), indent=2
         ).split("\n")
         generated_mapping = json.dumps(
-            generated_es_schema.get("mapping", {}),
-            indent=2
+            generated_es_schema.get("mapping", {}), indent=2
         ).split("\n")
 
         # Compare ES mappings
         diff_lines = difflib.unified_diff(
             original_mapping,
             generated_mapping,
             fromfile=str(elasticsearch_json),
-            tofile=str(tmp_es_json)
+            tofile=str(tmp_es_json),
         )
         diff_lines = list(diff_lines)
         if diff_lines:
             diff_lines = self._format_diffs(diff_lines)
             logs += [(diff_lines, criticality)]
         return logs
 
     def _create_new_elasticsearch_json(self, tmp: Path):
         es_gen_process = subprocess.run(
             ["python", "-m", "ids_es_json_generator", str(tmp)],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
-            check=True
+            check=True,
         )
         tmp_es_json = tmp / "elasticsearch.json"
         if not tmp_es_json.exists():
             raise FileNotFoundError(f"Could not find generated elasticsearch.json")
 
     def _format_diffs(self, diffs):
-        lines = [
-            f"    {line}\n"
-            for line in diffs
-        ]
+        lines = [f"    {line}\n" for line in diffs]
         lines = ["Elasticsearch diff \n"] + lines
-        return ''.join(lines)
+        return "".join(lines)
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/generic/required_property.py` & `ts-ids-validator-0.9.9/ids_validator/checks/generic/required_property.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,11 +13,14 @@
 
     def run(self, node: Node, context: dict = None):
         logs = []
         if node.has_required_list:
             missing_properties = node.missing_properties
             if missing_properties:
                 logs.append(
-                    (f"Required Properties are missing: {missing_properties}", Log.CRITICAL.value)
+                    (
+                        f"Required Properties are missing: {missing_properties}",
+                        Log.CRITICAL.value,
+                    )
                 )
 
         return logs
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/generic/root_node.py` & `ts-ids-validator-0.9.9/ids_validator/checks/generic/root_node.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 from pydash import get
 
 from ids_validator.ids_node import Node
 from ids_validator.checks import AbstractChecker
 from ids_validator.utils import Log
 
-root_minimum_required = [
-    "@idsType",
-    "@idsVersion",
-    "@idsNamespace"
-]
+root_minimum_required = ["@idsType", "@idsVersion", "@idsNamespace"]
 
 
 class RootNodeChecker(AbstractChecker):
-
     def run(self, node: Node, context=None):
         logs = []
-        if node.path == 'root':
+        if node.path == "root":
             logs += RootNodeChecker._check_min_required_props(node)
 
-            meta_paths = [
-                f"properties.{name}"
-                for name in root_minimum_required
-            ]
+            meta_paths = [f"properties.{name}" for name in root_minimum_required]
             for path in meta_paths:
                 prop = get(node, path)
-                meta_checks = [
-                    get(prop, "type") == 'string',
-                    get(prop, "const")
-                ]
+                meta_checks = [get(prop, "type") == "string", get(prop, "const")]
                 if not prop or not all(meta_checks):
                     logs.append(
-                        (f"'{path}' must be present with type 'string' with non-empty 'const'", Log.CRITICAL.value)
+                        (
+                            f"'{path}' must be present with type 'string' with non-empty 'const'",
+                            Log.CRITICAL.value,
+                        )
                     )
         return logs
 
     @staticmethod
     def _check_min_required_props(node: Node):
         logs = []
         if not node.has_required_list:
             logs.append(("'root.required' must be a list", Log.CRITICAL.value))
 
         if not node.required_contains_values(root_minimum_required):
             logs.append(
-                (f"'required' must contain: {', '.join(sorted(root_minimum_required))}", Log.CRITICAL.value))
+                (
+                    f"'required' must contain: {', '.join(sorted(root_minimum_required))}",
+                    Log.CRITICAL.value,
+                )
+            )
 
         return logs
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/generic/type_check.py` & `ts-ids-validator-0.9.9/ids_validator/checks/generic/type_check.py`

 * *Files identical despite different names*

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/rules_checker.py` & `ts-ids-validator-0.9.9/ids_validator/checks/rules_checker.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,32 +19,21 @@
 
     @classmethod
     def enforce_checks(cls, node: Node, checks: dict):
         logs = []
         if "type" in checks:
             logs += cls.enforce_type(node, checks.get("type"))
         if "required" in checks:
-            logs += cls.enforce_required(
-                node,
-                checks.get("required")
-            )
+            logs += cls.enforce_required(node, checks.get("required"))
         if "properties" in checks:
-            logs += cls.enforce_properties(
-                node,
-                checks.get("properties")
-            )
+            logs += cls.enforce_properties(node, checks.get("properties"))
         if "min_properties" in checks:
-            logs += cls.enforce_min_properties(
-                node,
-                checks.get("min_properties")
-            )
+            logs += cls.enforce_min_properties(node, checks.get("min_properties"))
         if "min_required" in checks:
-            logs += cls.enforce_min_required(
-                node, checks.get("min_required")
-            )
+            logs += cls.enforce_min_required(node, checks.get("min_required"))
         return logs
 
     @classmethod
     def enforce_type(cls, node: Node, type_: Union[List, str]):
         logs = []
 
         # DE-2922
@@ -57,23 +46,17 @@
                 logs += [(msg, Log.CRITICAL.value)]
                 return logs
             return logs
 
         if type(node.type_) != type(type_):
             logs += [(f"'type' must be {type_}", Log.CRITICAL.value)]
             return logs
-        elif (
-            (type(type_) == list)
-            and (sorted(node.type_) != sorted(type_))
-        ):
+        elif (type(type_) == list) and (sorted(node.type_) != sorted(type_)):
             logs += [(f"'type' must be {type_}", Log.CRITICAL.value)]
-        elif (
-            (type(type_) != list)
-            and (node.type_ != type_)
-        ):
+        elif (type(type_) != list) and (node.type_ != type_):
             logs += [(f"'type' must be {type_}", Log.CRITICAL.value)]
 
         return logs
 
     @classmethod
     def enforce_required(cls, node: Node, required: list):
         logs = []
@@ -86,72 +69,64 @@
 
     @classmethod
     def enforce_min_required(cls, node: Node, required: list):
         logs = []
         min_required = set(required)
         node_required = node.get("required", [])
         if type(node_required) != list:
-            logs += [(
-                f"'required' must contain {min_required}",
-                Log.CRITICAL.value
-            )]
+            logs += [(f"'required' must contain {min_required}", Log.CRITICAL.value)]
             return logs
 
         node_required = set(node_required)
         missing = min_required - node_required
         if missing:
-            logs += [(
-                f"'required' must contain {missing}",
-                Log.CRITICAL.value
-            )]
+            logs += [(f"'required' must contain {missing}", Log.CRITICAL.value)]
 
         return logs
 
     @classmethod
     def enforce_properties(cls, node: Node, properties: list):
         logs = []
-        node_properties = (
-            get(node, "properties")
-            or get(node, "items.properties")
-            or {}
-        )
+        node_properties = get(node, "properties") or get(node, "items.properties") or {}
         node_properties = node_properties.keys()
         properties = set(properties)
 
         extra_properties = node_properties - properties
         missing_properties = properties - node_properties
         if extra_properties:
-            logs += [(
+            logs += [
                 (
-                    f"'properties' must only contain {sorted(properties)}. Extra properties found: {extra_properties}"
-                ),
-                Log.CRITICAL.value
-            )]
+                    (
+                        f"'properties' must only contain {sorted(properties)}. Extra properties found: {extra_properties}"
+                    ),
+                    Log.CRITICAL.value,
+                )
+            ]
 
         if missing_properties:
-            logs += [(
+            logs += [
                 (
-                    f"'properties' must only contain {sorted(properties)}. Missing properties: {missing_properties}"
-                ),
-                Log.CRITICAL.value
-            )]
+                    (
+                        f"'properties' must only contain {sorted(properties)}. Missing properties: {missing_properties}"
+                    ),
+                    Log.CRITICAL.value,
+                )
+            ]
 
         return logs
 
     @classmethod
     def enforce_min_properties(cls, node: Node, properties: list):
         logs = []
-        node_properties = (
-            get(node, "properties")
-            or get(node, "items.properties")
-            or {}
-        )
+        node_properties = get(node, "properties") or get(node, "items.properties") or {}
         node_properties = set(node_properties.keys())
         min_props = set(properties)
 
         missing = min_props - node_properties
         if missing:
-            logs += [(
-                f"'properties' must contain {sorted(list(missing))}",
-                Log.CRITICAL.value
-            )]
+            logs += [
+                (
+                    f"'properties' must contain {sorted(list(missing))}",
+                    Log.CRITICAL.value,
+                )
+            ]
         return logs
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/v1/child_name.py` & `ts-ids-validator-0.9.9/ids_validator/checks/v1/child_name.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 class V1ChildNameChecker(AbstractChecker):
     """Checks if child name starts with parent's name"""
 
     def run(self, node: Node, context=None):
         logs = []
         properties = node.properties_list or []
         child_start_with_parent_name = [
-            prop.lower().startswith(node.name.lower())
-            for prop in properties
+            prop.lower().startswith(node.name.lower()) for prop in properties
         ]
         if any(child_start_with_parent_name):
-            logs += [(
-                f"Child property prefix uses the same name as the parent property '{node.name}'",
-                Log.WARNING.value
-            )]
+            logs += [
+                (
+                    f"Child property prefix uses the same name as the parent property '{node.name}'",
+                    Log.WARNING.value,
+                )
+            ]
         return logs
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/v1/convention_version_check.py` & `ts-ids-validator-0.9.9/ids_validator/checks/v1/convention_version_check.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from ids_validator.checks import AbstractChecker
 from ids_validator.utils import Log
 
 
 class V1ConventionVersionChecker(AbstractChecker):
     def run(self, node: Node, context: dict):
         logs = []
-        if node.path == 'root.properties.@idsConventionVersion':
+        if node.path == "root.properties.@idsConventionVersion":
             convention_version = context.get("convention_version")
-            if node.get('const') != convention_version:
+            if node.get("const") != convention_version:
                 logs.append(
-                    (f"'@idsConventionVersion must be {convention_version}", Log.CRITICAL.value)
+                    (
+                        f"'@idsConventionVersion must be {convention_version}",
+                        Log.CRITICAL.value,
+                    )
                 )
         return logs
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/v1/related_files_checker.py` & `ts-ids-validator-0.9.9/ids_validator/checks/v1/related_files_checker.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,26 +6,31 @@
 from ids_validator.utils import Log, read_schema
 
 
 TEMPLATES_DIR = (Path(__file__) / "../../../templates").resolve()
 RELATED_FILES_TEMPLATE = TEMPLATES_DIR / "related_files.json"
 RELATED_FILES = "root.properties.related_files"
 
+
 class V1RelatedFilesChecker(AbstractChecker):
     def run(self, node: Node, context: dict):
         logs = []
         if node.path == RELATED_FILES:
             if not RELATED_FILES_TEMPLATE.exists():
-                logs += [(
-                    f"Could not find template: {RELATED_FILES_TEMPLATE}",
-                    Log.CRITICAL.value
-                )]
+                logs += [
+                    (
+                        f"Could not find template: {RELATED_FILES_TEMPLATE}",
+                        Log.CRITICAL.value,
+                    )
+                ]
                 return logs
 
             related_files_template = read_schema(RELATED_FILES_TEMPLATE)
             if related_files_template["related_files"] != node.data:
-                logs += [(
-                    "'related_files' isn't an exact match of the template. Please refer to confluence docs.",
-                    Log.CRITICAL.value
-                )]
+                logs += [
+                    (
+                        "'related_files' isn't an exact match of the template. Please refer to confluence docs.",
+                        Log.CRITICAL.value,
+                    )
+                ]
 
         return logs
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/v1/root_node.py` & `ts-ids-validator-0.9.9/ids_validator/checks/v1/root_node.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,16 +14,19 @@
     """
 
     def run(self, node: Node, context: dict):
         logs = []
         if node.path == "roots":
             convention_version = get(node, CONVENTION_VERSION_PATH)
             checks = [
-                get(convention_version, "type") == 'string',
-                get(convention_version, "const")
+                get(convention_version, "type") == "string",
+                get(convention_version, "const"),
             ]
             if not convention_version or not all(checks):
                 logs.append(
-                    (f"'{CONVENTION_VERSION_PATH}' must be of type 'string' with none-empty 'const'", Log.CRITICAL.value)
+                    (
+                        f"'{CONVENTION_VERSION_PATH}' must be of type 'string' with none-empty 'const'",
+                        Log.CRITICAL.value,
+                    )
                 )
 
         return logs
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/v1/rules/samples/sample_properties.py` & `ts-ids-validator-0.9.9/ids_validator/checks/v1/rules/samples/sample_properties.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,55 +21,29 @@
             "name",
             "value",
             "value_data_type",
             "string_value",
             "numerical_value",
             "numerical_value_unit",
             "boolean_value",
-            "time"
+            "time",
         ],
     },
     SOURCE: {
         "type": "object",
-        "required": [
-            "name",
-            "type"
-        ],
-        "min_properties": ["name", "type"]
-    },
-    SOURCE_NAME: {
-        "type": ["string", "null"]
-    },
-    SOURCE_TYPE: {
-        "type":  ["string", "null"]
-    },
-    NAME: {
-        "type": "string"
-    },
-    VALUE: {
-        "type": "string"
-    },
-    VALUE_DATA_TYPE: {
-        "type": "string"
-    },
-    STRING_VALUE: {
-        "type": ["string", "null"]
-    },
-    NUMERICAL_VALUE: {
-        "type": ["number", "null"]
+        "required": ["name", "type"],
+        "min_properties": ["name", "type"],
     },
+    SOURCE_NAME: {"type": ["string", "null"]},
+    SOURCE_TYPE: {"type": ["string", "null"]},
+    NAME: {"type": "string"},
+    VALUE: {"type": "string"},
+    VALUE_DATA_TYPE: {"type": "string"},
+    STRING_VALUE: {"type": ["string", "null"]},
+    NUMERICAL_VALUE: {"type": ["number", "null"]},
     NUMERICAL_VALUE_UNIT: {
         "type": ["string", "null"],
     },
-    BOOLEAN_VALUE: {
-        "type": ["boolean", "null"]
-    },
-    TIME: {
-        "type": "object",
-        "required": ["lookup"],
-        "min_properties": ["lookup"]
-    },
-    TIME_LOOKUP: {
-        "type": ["string", "null"]
-    }
+    BOOLEAN_VALUE: {"type": ["boolean", "null"]},
+    TIME: {"type": "object", "required": ["lookup"], "min_properties": ["lookup"]},
+    TIME_LOOKUP: {"type": ["string", "null"]},
 }
-
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/v1/rules/samples/samples_labels.py` & `ts-ids-validator-0.9.9/ids_validator/checks/v1/rules/samples/samples_labels.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,44 +7,21 @@
 VALUE = f"{LABELS}.items.properties.value"
 TIME = f"{LABELS}.items.properties.time"
 TIME_LOOKUP = f"{LABELS}.items.properties.time.properties.lookup"
 
 path_to_checks = {
     ITEMS: {
         "type": "object",
-        "required": [
-            "source",
-            "name",
-            "value",
-            "time"
-        ],
+        "required": ["source", "name", "value", "time"],
     },
     SOURCE: {
         "type": "object",
-        "required": [
-            "name",
-            "type"
-        ],
-        "min_properties": ["name", "type"]
+        "required": ["name", "type"],
+        "min_properties": ["name", "type"],
     },
-    SOURCE_NAME: {
-        "type": "string"
-    },
-    SOURCE_TYPE: {
-        "type":  ["string", "null"]
-
-    },
-    NAME: {
-        "type": "string"
-    },
-    VALUE: {
-        "type": "string"
-    },
-    TIME: {
-        "type": "object",
-        "required": ["lookup"],
-        "min_properties": ["lookup"]
-    },
-    TIME_LOOKUP: {
-        "type": ["string", "null"]
-    }
-}
+    SOURCE_NAME: {"type": "string"},
+    SOURCE_TYPE: {"type": ["string", "null"]},
+    NAME: {"type": "string"},
+    VALUE: {"type": "string"},
+    TIME: {"type": "object", "required": ["lookup"], "min_properties": ["lookup"]},
+    TIME_LOOKUP: {"type": ["string", "null"]},
+}
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/v1/rules/samples/samples_root.py` & `ts-ids-validator-0.9.9/ids_validator/checks/v1/rules/samples/samples_root.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 SAMPLES = "root.properties.samples"
-ITEMS =  f"{SAMPLES}.items"
+ITEMS = f"{SAMPLES}.items"
 ID = f"{SAMPLES}.items.properties.id"
 BARCODE = f"{SAMPLES}.items.properties.barcode"
 NAME = f"{SAMPLES}.items.properties.name"
 BATCH = f"{SAMPLES}.items.properties.batch"
 BATCH_ID = f"{SAMPLES}.items.properties.batch.properties.id"
 BATCH_NAME = f"{SAMPLES}.items.properties.batch.properties.name"
 BATCH_BARCODE = f"{SAMPLES}.items.properties.batch.properties.barcode"
@@ -15,103 +15,57 @@
 LOT_NAME = f"{SAMPLES}.items.properties.lot.properties.name"
 LOCATION = f"{SAMPLES}.items.properties.location"
 PROPERTIES = f"{SAMPLES}.items.properties.properties"
 LABELS = f"{SAMPLES}.items.properties.labels"
 
 
 path_to_checks = {
-    SAMPLES:{
+    SAMPLES: {
         "type": "array",
     },
-    ITEMS:{
+    ITEMS: {
         "type": "object",
-        "properties":[
+        "properties": [
             "id",
             "barcode",
             "name",
             "batch",
             "set",
             "lot",
             "location",
             "properties",
-            "labels"
-        ]
-    },
-    ID: {
-        "type": ["string", "null"]
-    },
-    BARCODE: {
-        "type": ["string", "null"]
-    },
-    NAME: {
-        "type": ["string", "null"]
-    },
-    BATCH: {
-        "type": "object",
-        "min_properties":[
-            "id",
-            "name",
-            "barcode"
-        ]
-    },
-    BATCH_ID:{
-        "type": ["string", "null"]
-    },
-    BATCH_NAME: {
-        "type": ["string", "null"]
-    },
-    BATCH_BARCODE: {
-        "type": ["string", "null"]
-    },
-    SET: {
-        "type": "object",
-        "min_properties": [
-            "id",
-            "name"
-        ]
-    },
-    SET_ID:{
-        "type": ["string", "null"]
-    },
-    SET_NAME: {
-        "type": ["string", "null"]
-    },
-    LOT: {
-        "type": "object",
-        "min_properties": [
-            "id",
-            "name"
-        ]
-    },
-    LOT_ID: {
-        "type": ["string", "null"]
-    },
-    LOT_NAME: {
-        "type": ["string", "null"]
-    },
-    LOCATION: {
-        "type" : "object"
+            "labels",
+        ],
     },
+    ID: {"type": ["string", "null"]},
+    BARCODE: {"type": ["string", "null"]},
+    NAME: {"type": ["string", "null"]},
+    BATCH: {"type": "object", "min_properties": ["id", "name", "barcode"]},
+    BATCH_ID: {"type": ["string", "null"]},
+    BATCH_NAME: {"type": ["string", "null"]},
+    BATCH_BARCODE: {"type": ["string", "null"]},
+    SET: {"type": "object", "min_properties": ["id", "name"]},
+    SET_ID: {"type": ["string", "null"]},
+    SET_NAME: {"type": ["string", "null"]},
+    LOT: {"type": "object", "min_properties": ["id", "name"]},
+    LOT_ID: {"type": ["string", "null"]},
+    LOT_NAME: {"type": ["string", "null"]},
+    LOCATION: {"type": "object"},
     PROPERTIES: {
-        "type" : "array",
-        "min_properties":[
+        "type": "array",
+        "min_properties": [
             "source",
             "name",
             "value",
             "value_data_type",
             "string_value",
             "numerical_value",
             "numerical_value_unit",
             "boolean_value",
-            "time"
+            "time",
         ],
     },
     LABELS: {
-        "type" : "array",
-        "min_properties": [
-            "source",
-            "name",
-            "value",
-            "time"
-        ],
+        "type": "array",
+        "min_properties": ["source", "name", "value", "time"],
     },
-}
+}
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/v1/rules/systems.py` & `ts-ids-validator-0.9.9/ids_validator/checks/v1/rules/systems.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,83 +23,48 @@
 systems_rules = {
     SYSTEMS: {
         "type": "array",
         "min_properties": [
             "vendor",
             "model",
             "type",
-        ]
+        ],
     },
     ITEMS: {
         "type": "object",
-        "min_required": [
-            "vendor",
-            "model",
-            "type"
-        ],
-
-    },
-    ID: {
-        "type": ["string", "null"]
-    },
-    NAME: {
-        "type": ["string", "null"]
-    },
-    VENDOR: {
-        "type": ["string", "null"]
-    },
-    MODEL: {
-        "type": ["string", "null"]
-    },
-    TYPE: {
-        "type": ["string", "null"]
+        "min_required": ["vendor", "model", "type"],
     },
+    ID: {"type": ["string", "null"]},
+    NAME: {"type": ["string", "null"]},
+    VENDOR: {"type": ["string", "null"]},
+    MODEL: {"type": ["string", "null"]},
+    TYPE: {"type": ["string", "null"]},
     SERIAL_NUMBER: {"type": ["string", "null"]},
-
     FIRMWARE: {
         "type": "array",
         "min_properties": [
             "name",
             "version",
-        ]
+        ],
     },
     FIRMWARE_ITEMS: {
         "type": "object",
-        "min_required": [
-            "name",
-            "version"
-        ],
-    },
-    FIRMWARE_NAME: {
-        "type": ["string", "null"]
-    },
-    FIRMWARE_VERSION: {
-        "type": ["string", "null"]
+        "min_required": ["name", "version"],
     },
-    FIRMWARE_LAST_UPDATE: {
-        "type": ["string", "null"]
-    },
-
+    FIRMWARE_NAME: {"type": ["string", "null"]},
+    FIRMWARE_VERSION: {"type": ["string", "null"]},
+    FIRMWARE_LAST_UPDATE: {"type": ["string", "null"]},
     SOFTWARE: {
         "type": "array",
         "min_properties": [
             "name",
             "version",
-        ]
+        ],
     },
     SOFTWARE_ITEMS: {
         "type": "object",
-        "min_required": [
-            "name",
-            "version"
-        ],
-    },
-    SOFTWARE_NAME: {
-        "type": ["string", "null"]
-    },
-    SOFTWARE_VERSION: {
-        "type": ["null", "string"]
-    },
-    SOFTWARE_LAST_UPDATE: {
-        "type": ["string", "null"]
+        "min_required": ["name", "version"],
     },
+    SOFTWARE_NAME: {"type": ["string", "null"]},
+    SOFTWARE_VERSION: {"type": ["null", "string"]},
+    SOFTWARE_LAST_UPDATE: {"type": ["string", "null"]},
 }
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/checks/v1/snake_case.py` & `ts-ids-validator-0.9.9/ids_validator/checks/v1/snake_case.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,42 +2,34 @@
 from ids_validator.ids_node import Node
 from ids_validator.checks import AbstractChecker
 from ids_validator.utils import Log
 
 
 ignored_paths = [
     "root.properties.related_files.items.properties.pointer.properties.fileId",
-    "root.properties.related_files.items.properties.pointer.properties.fileKey"
+    "root.properties.related_files.items.properties.pointer.properties.fileKey",
 ]
+
+
 class V1SnakeCaseChecker(AbstractChecker):
     def run(self, node: Node, context: dict = None):
         logs = []
 
         if node.path in ignored_paths:
             return logs
 
         name: str = node.name
         checks = [
             name.islower() or name.isdigit(),
             len(name.split()) == 1,
-            all(
-                [
-                    x.isalnum()
-                    for x in _filter_empty_string(name.split('_'))
-                ]
-            )
-
+            all([x.isalnum() for x in _filter_empty_string(name.split("_"))]),
         ]
         if not name.startswith("@") and not all(checks):
             logs.append(
                 (f"'{node.name}' should be named as snake_case.", Log.CRITICAL.value)
             )
 
         return logs
 
 
 def _filter_empty_string(str_list):
-    return [
-        str_val
-        for str_val in str_list
-        if str_val != ''
-    ]
+    return [str_val for str_val in str_list if str_val != ""]
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/ids_node.py` & `ts-ids-validator-0.9.9/ids_validator/ids_node.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,70 @@
 from collections import UserDict
 from pydash import get
 
 
 class Node(UserDict):
-
     def __init__(self, ids_dict, path="", name="root"):
         self.data = ids_dict
         self.name = name
         self.path = path
 
     @property
     def properties_dict(self):
         ids = self.data
-        if ids.get('type') == 'object' and ids.get('properties') is not None:
-            return ids.get('properties')
-        elif ids.get('type') == 'array' and get(ids, 'items.properties') is not None:
-            return get(ids, 'items.properties')
+        if ids.get("type") == "object" and ids.get("properties") is not None:
+            return ids.get("properties")
+        elif ids.get("type") == "array" and get(ids, "items.properties") is not None:
+            return get(ids, "items.properties")
         else:
             return None
 
     @property
     def properties_list(self):
         prop_dict = self.properties_dict
         if prop_dict:
             return prop_dict.keys()
 
     @property
     def type_(self):
-        type = self.data.get('type')
+        type = self.data.get("type")
         return type
 
     @property
     def has_required_list(self):
-        required = self.get('required')
+        required = self.get("required")
         required_exist = required and type(required) == list
         return True if required_exist else False
 
     def required_contains_values(self, min_required_values: list):
         if self.has_required_list:
-            required = set(self.get('required'))
+            required = set(self.get("required"))
             min_required = set(min_required_values)
-            return (
-                False if min_required - required
-                else True
-            )
+            return False if min_required - required else True
         return False
 
     def has_properties(self, prop_list: list):
         properties = self.properties_list or []
         properties = set(properties)
 
         req_prop = set(prop_list)
 
-        return (
-            False
-            if req_prop - properties
-            else True
-        )
+        return False if req_prop - properties else True
 
     @property
     def missing_properties(self):
         required = set(self.get("required"))
         properties = self.get("properties", {}).keys()
         return required - properties
 
     @property
     def has_valid_type(self):
         if "const" in self.data:
             return self._check_const_type()
-        if self.type_ == 'object':
+        if self.type_ == "object":
             return self._check_object_type()
         elif self.type_ == "array":
             return self._check_array_type()
         elif type(self.type_) == list:
             return self._check_list_type()
         elif type(self.type_) == str:
             return self._check_unit_type()
@@ -80,62 +72,57 @@
             return True, None
 
     def _check_const_type(self):
         """If const is defined, then type must
         not be a list
         """
         valid_const_type = [
-            'number',
-            'string',
-            'boolean',
-            'integer',
+            "number",
+            "string",
+            "boolean",
+            "integer",
         ]
-        if self.type_ not in  valid_const_type:
+        if self.type_ not in valid_const_type:
             return (
                 False,
-                f"'type' must be one of {valid_const_type} when 'const' is defined"
+                f"'type' must be one of {valid_const_type} when 'const' is defined",
             )
         return True, None
 
     def _check_object_type(self):
         """Checks if `object` type contains properties
 
         Returns:
             tuple: A `tuple` with `boolean` that tells whether
             node a valid `object` type or not and a `string` message
             if its invalid `object` type
         """
         return (
-            (True, None) if self.properties_list
-            else (
-                False,
-                "'object' type must  contains non-empty 'properties'"
-            )
+            (True, None)
+            if self.properties_list
+            else (False, "'object' type must  contains non-empty 'properties'")
         )
 
     def _check_array_type(self):
         """Checks if node is valid `array` type that contains
         child `properties`
 
         Returns:
             tuple: A `tuple` with `boolean` that tells whether
             node a valid `array` type or not and a `string` message
             if its invalid `array` type
         """
         # Arrays inside datacubes measures and dimensions
         # doesn't need to have children. So, ignore them.
         ignored_paths = [
-            'datacubes.items.properties.measures',
-            'datacubes.items.properties.dimensions',
+            "datacubes.items.properties.measures",
+            "datacubes.items.properties.dimensions",
         ]
 
-        if (
-            ignored_paths[0] in self.path
-            or ignored_paths[1] in self.path
-        ):
+        if ignored_paths[0] in self.path or ignored_paths[1] in self.path:
             return (True, None)
 
         # Array must contain items: dict
         if "items" not in self:
             return (False, "'array' type must contain 'items: dict'")
 
         items = get(self, "items")
@@ -149,82 +136,45 @@
         if "type" not in items:
             return (False, "'array' type must contain items.type")
 
         # All Good, it a valid array time
         return True, None
 
     def _check_list_type(self):
-        valid_nullable_types = {
-            'number',
-            'string',
-            'boolean',
-            'integer',
-            'null'
-        }
+        valid_nullable_types = {"number", "string", "boolean", "integer", "null"}
 
         checks = [
             # Length of list type must 2.
             (0 < len(self.type_) <= 2),
-
             # list must not contain same value
             len(set(self.type_)) == len(self.type_),
-
             # List must only contain values from
             # valid_nullable types
             ((set(self.type_) - valid_nullable_types) == set()),
-
             # If list contains two data types
             # make sure one of them is null
-            (
-                ("null" in self.type_)
-                if len(self.type_) == 2
-                else True
-            ),
-
+            (("null" in self.type_) if len(self.type_) == 2 else True),
             # If list contains one datatypes
             # make sure its not null
-            (
-                ("null" not in self.type_)
-                if len(self.type_) == 1
-                else True
-            )
-
+            (("null" not in self.type_) if len(self.type_) == 1 else True),
         ]
-        result = (
-            (True, None) if all(checks)
-            else (False, None)
-        )
+        result = (True, None) if all(checks) else (False, None)
         return result
 
     def _check_unit_type(self):
-        valid_types = {
-            'number',
-            'string',
-            'boolean',
-            'array',
-            'object',
-            'integer'
-        }
-        return (
-            (True, None) if self.type_ in valid_types
-            else (False, None)
-        )
+        valid_types = {"number", "string", "boolean", "array", "object", "integer"}
+        return (True, None) if self.type_ in valid_types else (False, None)
 
     def _is_numeric_type(self):
         if type(self.type_) == list:
             type_ = sorted(self.type_)
-            if not (
-                type_ in [
-                    sorted(["null", "integer"]),
-                    sorted(["null", "number"])
-                ]
-            ):
+            if not (type_ in [sorted(["null", "integer"]), sorted(["null", "number"])]):
                 return False
 
-        elif not(self.type_ in ["number", "integer"]):
+        elif not (self.type_ in ["number", "integer"]):
             return False
 
         return True
 
     def get_missing_paths(self, paths: list):
         result = []
         for path in paths:
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/ids_validator.py` & `ts-ids-validator-0.9.9/ids_validator/ids_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,24 +25,21 @@
     Returns:
         Convention: Enum value for the convention version or generic type
     """
     if version is not None:
         result = Conventions.get_by_value(version)
         if result not in checks_dict:
             print(
-                f"* Invalid Version passed. Supported Version: {Conventions.values()}")
+                f"* Invalid Version passed. Supported Version: {Conventions.values()}"
+            )
             sys.exit(1)
         return result
     else:
         print(f"* Reading @idsConventionVersion from schema.json")
-        convention = get(
-            ids,
-            "properties.@idsConventionVersion.const",
-            None
-        )
+        convention = get(ids, "properties.@idsConventionVersion.const", None)
         if convention is None:
             print("* @idsConvention not specified in schema.json.")
             print("* Using Generic Validator")
             return Conventions.get_by_value("generic")
 
         if convention:
             convention_enum_value = Conventions.get_by_value(convention)
```

### Comparing `ts-ids-validator-0.9.8/ids_validator/templates/related_files.json` & `ts-ids-validator-0.9.9/ids_validator/templates/related_files.json`

 * *Files identical despite different names*

### Comparing `ts-ids-validator-0.9.8/ids_validator/validator.py` & `ts-ids-validator-0.9.9/ids_validator/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.ids = ids
         self.athena = athena
         self.checks_list = checks_list
         self.context = {
             "athena.json": self.athena,
             "schema.json": self.ids,
             "convention_version": convention_version,
-            "ids_folder_path": ids_folder_path
+            "ids_folder_path": ids_folder_path,
         }
         self.console = Console()
         self.property_failures = {}
         self.has_critical_failures = False
 
     def _traverse(self, schema, name="root", path="root"):
         node = Node(ids_dict=schema, name=name, path=path)
@@ -42,17 +42,15 @@
             if type(v) == dict:
                 self._traverse(v, name=k, path=f"{path}.{k}")
 
     def validate_ids(self):
         self._traverse(schema=self.ids)
 
     def log(self, messages, property_name, prop_color="red"):
-        self.console.print(
-            f"[b u  {prop_color}]{property_name}[/b u {prop_color}]:")
+        self.console.print(f"[b u  {prop_color}]{property_name}[/b u {prop_color}]:")
 
         for msg, log_level in sorted(messages, key=lambda x: str(x[0])):
             if log_level == Log.CRITICAL.value:
                 self.has_critical_failures = True
 
             msg_color = "yellow" if log_level == Log.CRITICAL.value else "white"
-            self.console.print(
-                f"[italic {msg_color}]   * {msg}[italic {msg_color}]")
+            self.console.print(f"[italic {msg_color}]   * {msg}[italic {msg_color}]")
```

### Comparing `ts-ids-validator-0.9.8/requirements.txt` & `ts-ids-validator-0.9.9/requirements.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 # These requirements were autogenerated by pipenv
 # To regenerate from the project's Pipfile, run:
 #
 #    pipenv lock --requirements
 #
 
 -i https://pypi.org/simple
-attrs>=21.2.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
-colorama>=0.4.4; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
-commonmark>=0.9.1
-importlib-metadata>=4.8.2; python_version < '3.8'
-importlib-resources>=5.4.0; python_version < '3.9'
-jsonref>=0.2
-jsonschema>=4.2.1
-pydash>=5.1.0
-pygments>=2.10.0; python_version >= '3.5'
-pyrsistent>=0.18.0; python_version >= '3.6'
-rich>=10.14.0
-ts-ids-es-json-generator>=1.0.1
-typing-extensions>=4.0.0; python_version < '3.8' and python_version < '3.8'
-zipp>=3.6.0; python_version < '3.10'
+attrs==21.2.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
+colorama==0.4.4; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
+commonmark==0.9.1
+importlib-metadata==4.10.0; python_version < '3.8'
+jsonref==0.2
+jsonschema==3.2.0
+pydash==5.1.0
+pygments==2.10.0; python_version >= '3.5'
+pyrsistent==0.18.0; python_version >= '3.6'
+rich==10.16.1
+six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2'
+ts-ids-es-json-generator==1.0.1
+typing-extensions==4.0.1; python_version < '3.8' and python_version < '3.8'
+zipp==3.6.0; python_version >= '3.6'
```

### Comparing `ts-ids-validator-0.9.8/setup.py` & `ts-ids-validator-0.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 # coding: utf-8
 
 from setuptools import setup, find_packages
 
 NAME = "ts-ids-validator"
-VERSION = "0.9.8"
+VERSION = "0.9.9"
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 # Read Requirements
 with open("./requirements.txt", "r") as req_file:
     requirements = req_file.read()
     requirements = requirements.splitlines()
-    requirements = [
-        req
-        for req in requirements
-        if req and req[0].isalpha()
-    ]
+    requirements = [req for req in requirements if req and req[0].isalpha()]
 
 setup(
     name=NAME,
     version=VERSION,
     description="Python utility for validating IDS",
     author="tetrascience",
     author_email="developers@tetrascience.com",
@@ -30,15 +26,15 @@
     },
     keywords=[],
     install_requires=requirements,
     packages=find_packages(),
     include_package_data=True,
     long_description=readme,
     long_description_content_type="text/markdown",
-    python_requires='>=3.7',
-    license='Apache License 2.0',
+    python_requires=">=3.7",
+    license="Apache License 2.0",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
-)
+)
```

### Comparing `ts-ids-validator-0.9.8/ts_ids_validator.egg-info/PKG-INFO` & `ts-ids-validator-0.9.9/ts_ids_validator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts-ids-validator
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python utility for validating IDS
 Home-page: https://github.com/tetrascience/ts-ids-validator
 Author: tetrascience
 Author-email: developers@tetrascience.com
 License: Apache License 2.0
 Project-URL: Tetra Developer Site, https://developers.tetrascience.com
 Platform: UNKNOWN
@@ -207,14 +207,18 @@
 ### List of Checks for Validator
 
 - `checks_dict`, defined [here](src/checks/__init__.py), maps the `type of validation` that we want to perform to the `list the of checks` needed to be run for the validation
 - The list off checks is actually a list of instantiated checker objects
 
 ## Changelog
 
+## v0.9.9
+
+- Lock `jsonschema` version in requirements.txt
+
 ## v0.9.8
 
 - Modify `RulesChecker` to log missing and extra properties
 
 ## v0.9.7
 
 - Allow properties with `const` values to have non-nullable `type`
```

### Comparing `ts-ids-validator-0.9.8/ts_ids_validator.egg-info/SOURCES.txt` & `ts-ids-validator-0.9.9/ts_ids_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ts-ids-validator-0.9.8/ts_ids_validator.egg-info/requires.txt` & `ts-ids-validator-0.9.9/ts_ids_validator.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-commonmark>=0.9.1
-jsonref>=0.2
-jsonschema>=4.2.1
-pydash>=5.1.0
-rich>=10.14.0
-ts-ids-es-json-generator>=1.0.1
-
-[:python_version < "3.10"]
-zipp>=3.6.0
+commonmark==0.9.1
+jsonref==0.2
+jsonschema==3.2.0
+pydash==5.1.0
+rich==10.16.1
+ts-ids-es-json-generator==1.0.1
 
 [:python_version < "3.8"]
-importlib-metadata>=4.8.2
+importlib-metadata==4.10.0
 
 [:python_version < "3.8" and python_version < "3.8"]
-typing-extensions>=4.0.0
+typing-extensions==4.0.1
 
-[:python_version < "3.9"]
-importlib-resources>=5.4.0
+[:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2"]
+six==1.16.0
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"]
-attrs>=21.2.0
-colorama>=0.4.4
+attrs==21.2.0
+colorama==0.4.4
 
 [:python_version >= "3.5"]
-pygments>=2.10.0
+pygments==2.10.0
 
 [:python_version >= "3.6"]
-pyrsistent>=0.18.0
+pyrsistent==0.18.0
+zipp==3.6.0
```

