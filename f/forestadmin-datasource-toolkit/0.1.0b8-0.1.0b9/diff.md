# Comparing `tmp/forestadmin_datasource_toolkit-0.1.0b8.tar.gz` & `tmp/forestadmin_datasource_toolkit-0.1.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_datasource_toolkit-0.1.0b8.tar", max compression
+gzip compressed data, was "forestadmin_datasource_toolkit-0.1.0b9.tar", max compression
```

## Comparing `forestadmin_datasource_toolkit-0.1.0b8.tar` & `forestadmin_datasource_toolkit-0.1.0b9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/README.md
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/__init__.py
--rw-r--r--   0        0        0     2219 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/collections.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/context/__init__.py
--rw-r--r--   0        0        0      716 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/context/agent_context.py
--rw-r--r--   0        0        0      768 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/context/collection_context.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/context/relaxed_wrappers/__init__.py
--rw-r--r--   0        0        0     6533 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py
--rw-r--r--   0        0        0     1195 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/datasources.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/__init__.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/__init__.py
--rw-r--r--   0        0        0     4910 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/collections.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/context/__init__.py
--rw-r--r--   0        0        0     1944 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/context/base.py
--rw-r--r--   0        0        0      799 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/context/bulk.py
--rw-r--r--   0        0        0      776 2022-12-07 16:04:48.561013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/context/single.py
--rw-r--r--   0        0        0     1984 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/result_builder.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/types/__init__.py
--rw-r--r--   0        0        0     1656 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/types/actions.py
--rw-r--r--   0        0        0    12320 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/types/fields.py
--rw-r--r--   0        0        0     1530 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/collections.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/computed/__init__.py
--rw-r--r--   0        0        0     4537 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/computed/collections.py
--rw-r--r--   0        0        0      150 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/computed/exceptions.py
--rw-r--r--   0        0        0     5113 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/computed/helpers.py
--rw-r--r--   0        0        0      535 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/computed/types.py
--rw-r--r--   0        0        0     2814 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/computed/utils.py
--rw-r--r--   0        0        0      595 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/datasource.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/operators_replace/__init__.py
--rw-r--r--   0        0        0     3279 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/operators_replace/collections.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/proxy/__init__.py
--rw-r--r--   0        0        0     3362 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/proxy/collection.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/publication/__init__.py
--rw-r--r--   0        0        0     2689 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/publication/collections.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/rename/__init__.py
--rw-r--r--   0        0        0     9765 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/rename/collections.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/search/__init__.py
--rw-r--r--   0        0        0     5247 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/search/collections.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/segments/__init__.py
--rw-r--r--   0        0        0     2432 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/segments/collections.py
--rw-r--r--   0        0        0       54 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/exceptions.py
--rw-r--r--   0        0        0     6148 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/__init__.py
--rw-r--r--   0        0        0     1881 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/actions.py
--rw-r--r--   0        0        0     1781 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/collections.py
--rw-r--r--   0        0        0     5139 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/fields.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/models/__init__.py
--rw-r--r--   0        0        0     1400 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/models/collections.py
--rw-r--r--   0        0        0     6148 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/__init__.py
--rw-r--r--   0        0        0     7811 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/aggregation.py
--rw-r--r--   0        0        0     6148 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/__init__.py
--rw-r--r--   0        0        0     4663 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py
--rw-r--r--   0        0        0     5323 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/__init__.py
--rw-r--r--   0        0        0     2124 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py
--rw-r--r--   0        0        0     4370 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py
--rw-r--r--   0        0        0     9674 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py
--rw-r--r--   0        0        0     1270 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/__init__.py
--rw-r--r--   0        0        0     3937 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py
--rw-r--r--   0        0        0     1579 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py
--rw-r--r--   0        0        0     7661 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/filter/__init__.py
--rw-r--r--   0        0        0     6662 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py
--rw-r--r--   0        0        0     2877 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py
--rw-r--r--   0        0        0     3213 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py
--rw-r--r--   0        0        0      875 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/page.py
--rw-r--r--   0        0        0     4482 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py
--rw-r--r--   0        0        0      901 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py
--rw-r--r--   0        0        0     2619 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py
--rw-r--r--   0        0        0      574 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py
--rw-r--r--   0        0        0      118 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/records.py
--rw-r--r--   0        0        0       73 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     7007 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/utils/collections.py
--rw-r--r--   0        0        0     1165 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/utils/records.py
--rw-r--r--   0        0        0     1658 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/utils/schema.py
--rw-r--r--   0        0        0        0 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/validations/__init__.py
--rw-r--r--   0        0        0     4756 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/validations/condition_tree.py
--rw-r--r--   0        0        0     3577 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/validations/field.py
--rw-r--r--   0        0        0      393 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/validations/projection.py
--rw-r--r--   0        0        0     1542 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/validations/records.py
--rw-r--r--   0        0        0     4536 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/validations/rules.py
--rw-r--r--   0        0        0      469 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/validations/sort.py
--rw-r--r--   0        0        0     4348 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/validations/type_getter.py
--rw-r--r--   0        0        0      372 2022-12-07 16:04:48.565013 forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/validations/types.py
--rw-r--r--   0        0        0     1622 2022-12-07 16:05:09.209204 forestadmin_datasource_toolkit-0.1.0b8/pyproject.toml
--rw-r--r--   0        0        0     2365 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-0.1.0b8/setup.py
--rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-0.1.0b8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/README.md
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/__init__.py
+-rw-r--r--   0        0        0     2219 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/collections.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/context/__init__.py
+-rw-r--r--   0        0        0      716 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/context/agent_context.py
+-rw-r--r--   0        0        0      768 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/context/collection_context.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/context/relaxed_wrappers/__init__.py
+-rw-r--r--   0        0        0     6533 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py
+-rw-r--r--   0        0        0     1195 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/datasources.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/__init__.py
+-rw-r--r--   0        0        0     4910 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/collections.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/context/__init__.py
+-rw-r--r--   0        0        0     1944 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/context/base.py
+-rw-r--r--   0        0        0      799 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/context/bulk.py
+-rw-r--r--   0        0        0      776 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/context/single.py
+-rw-r--r--   0        0        0     1984 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/result_builder.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/types/__init__.py
+-rw-r--r--   0        0        0     1656 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/types/actions.py
+-rw-r--r--   0        0        0    12320 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/types/fields.py
+-rw-r--r--   0        0        0     1530 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/collections.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/__init__.py
+-rw-r--r--   0        0        0     4537 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/collections.py
+-rw-r--r--   0        0        0      150 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/exceptions.py
+-rw-r--r--   0        0        0     5113 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/helpers.py
+-rw-r--r--   0        0        0      535 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/types.py
+-rw-r--r--   0        0        0     2814 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/utils.py
+-rw-r--r--   0        0        0      595 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/datasource.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/operators_replace/__init__.py
+-rw-r--r--   0        0        0     3279 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/operators_replace/collections.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/proxy/__init__.py
+-rw-r--r--   0        0        0     3362 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/proxy/collection.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/publication/__init__.py
+-rw-r--r--   0        0        0     2689 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/publication/collections.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/rename/__init__.py
+-rw-r--r--   0        0        0     9765 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/rename/collections.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/search/__init__.py
+-rw-r--r--   0        0        0     5247 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/search/collections.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/segments/__init__.py
+-rw-r--r--   0        0        0     2432 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/segments/collections.py
+-rw-r--r--   0        0        0       54 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/exceptions.py
+-rw-r--r--   0        0        0     6148 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/.DS_Store
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/__init__.py
+-rw-r--r--   0        0        0     1881 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/actions.py
+-rw-r--r--   0        0        0     1781 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/collections.py
+-rw-r--r--   0        0        0     5139 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/fields.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/models/__init__.py
+-rw-r--r--   0        0        0     1400 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/models/collections.py
+-rw-r--r--   0        0        0     6148 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/.DS_Store
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/__init__.py
+-rw-r--r--   0        0        0     7811 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/aggregation.py
+-rw-r--r--   0        0        0     6148 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/__init__.py
+-rw-r--r--   0        0        0     4663 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py
+-rw-r--r--   0        0        0     5323 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/__init__.py
+-rw-r--r--   0        0        0     2124 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py
+-rw-r--r--   0        0        0     4370 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py
+-rw-r--r--   0        0        0     9674 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py
+-rw-r--r--   0        0        0     1270 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/__init__.py
+-rw-r--r--   0        0        0     3937 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py
+-rw-r--r--   0        0        0     1579 2022-12-07 16:20:36.784438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py
+-rw-r--r--   0        0        0     7661 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/filter/__init__.py
+-rw-r--r--   0        0        0     6662 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py
+-rw-r--r--   0        0        0     2877 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py
+-rw-r--r--   0        0        0     3213 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py
+-rw-r--r--   0        0        0      875 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/page.py
+-rw-r--r--   0        0        0     4482 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py
+-rw-r--r--   0        0        0      901 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py
+-rw-r--r--   0        0        0     2619 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py
+-rw-r--r--   0        0        0      574 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py
+-rw-r--r--   0        0        0      118 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/records.py
+-rw-r--r--   0        0        0       73 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     7007 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/utils/collections.py
+-rw-r--r--   0        0        0     1165 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/utils/records.py
+-rw-r--r--   0        0        0     1658 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/utils/schema.py
+-rw-r--r--   0        0        0        0 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/__init__.py
+-rw-r--r--   0        0        0     4756 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/condition_tree.py
+-rw-r--r--   0        0        0     3577 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/field.py
+-rw-r--r--   0        0        0      393 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/projection.py
+-rw-r--r--   0        0        0     1542 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/records.py
+-rw-r--r--   0        0        0     4536 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/rules.py
+-rw-r--r--   0        0        0      469 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/sort.py
+-rw-r--r--   0        0        0     4348 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/type_getter.py
+-rw-r--r--   0        0        0      372 2022-12-07 16:20:36.788438 forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/types.py
+-rw-r--r--   0        0        0     1622 2022-12-07 16:20:54.420138 forestadmin_datasource_toolkit-0.1.0b9/pyproject.toml
+-rw-r--r--   0        0        0     2365 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-0.1.0b9/setup.py
+-rw-r--r--   0        0        0      908 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-0.1.0b9/PKG-INFO
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/collections.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/context/agent_context.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/context/agent_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/context/collection_context.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/context/collection_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/datasources.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/datasources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/collections.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/context/base.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/context/base.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/context/bulk.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/context/bulk.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/context/single.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/context/single.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/result_builder.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/result_builder.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/types/actions.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/types/actions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/action/types/fields.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/action/types/fields.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/collections.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/computed/collections.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/computed/helpers.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/helpers.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/computed/types.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/types.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/computed/utils.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/computed/utils.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/datasource.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/operators_replace/collections.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/operators_replace/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/proxy/collection.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/proxy/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/publication/collections.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/publication/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/rename/collections.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/rename/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/search/collections.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/search/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/decorators/segments/collections.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/decorators/segments/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/.DS_Store` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/actions.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/actions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/collections.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/fields.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/fields.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/models/collections.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/models/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/.DS_Store` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/aggregation.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/aggregation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/page.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/page.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/utils/collections.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/utils/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/utils/records.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/utils/records.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/utils/schema.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/utils/schema.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/validations/condition_tree.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/condition_tree.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/validations/field.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/validations/records.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/records.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/validations/rules.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/rules.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/forestadmin/datasource_toolkit/validations/type_getter.py` & `forestadmin_datasource_toolkit-0.1.0b9/forestadmin/datasource_toolkit/validations/type_getter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/pyproject.toml` & `forestadmin_datasource_toolkit-0.1.0b9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-datasource-toolkit"
-version = "0.1.0-beta.8"
+version = "0.1.0-beta.9"
 description = ""
 authors = [ "Valentin Monté <valentinm@forestadmin.com>",]
 readme = "README.md"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.semantic_release]
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/setup.py` & `forestadmin_datasource_toolkit-0.1.0b9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 {':python_full_version < "3.7.1"': ['pandas==1.1.5'],
  ':python_full_version >= "3.7.1" and python_version < "3.8"': ['pandas==1.3.5'],
  ':python_version < "3.9"': ['backports.zoneinfo[tzdata]>=0.2.1,<0.3.0'],
  ':python_version >= "3.8"': ['pandas>=1.4.2,<1.5.0']}
 
 setup_kwargs = {
     'name': 'forestadmin-datasource-toolkit',
-    'version': '0.1.0b8',
+    'version': '0.1.0b9',
     'description': '',
     'long_description': '',
     'author': 'Valentin Monté',
     'author_email': 'valentinm@forestadmin.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `forestadmin_datasource_toolkit-0.1.0b8/PKG-INFO` & `forestadmin_datasource_toolkit-0.1.0b9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forestadmin-datasource-toolkit
-Version: 0.1.0b8
+Version: 0.1.0b9
 Summary: 
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

