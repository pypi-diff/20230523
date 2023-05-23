# Comparing `tmp/cqlpy-0.2.2.tar.gz` & `tmp/cqlpy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cqlpy-0.2.2.tar", max compression
+gzip compressed data, was "cqlpy-0.2.4.tar", max compression
```

## Comparing `cqlpy-0.2.2.tar` & `cqlpy-0.2.4.tar`

### file list

```diff
@@ -1,86 +1,92 @@
--rw-r--r--   0        0        0     1070 2023-04-21 17:09:29.459947 cqlpy-0.2.2/LICENSE
--rw-r--r--   0        0        0        8 2023-04-21 17:09:29.459947 cqlpy-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/__init__.py
--rw-r--r--   0        0        0     5078 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/context/context.py
--rw-r--r--   0        0        0      748 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/context/cql_value_set_provider.py
--rw-r--r--   0        0        0    17487 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/context/fhir_r4_data_model.py
--rw-r--r--   0        0        0      689 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/context/parameter_provider.py
--rw-r--r--   0        0        0     2319 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/context/resource_query.py
--rw-r--r--   0        0        0     1696 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/context/type_factory.py
--rw-r--r--   0        0        0       92 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/exceptions.py
--rw-r--r--   0        0        0      123 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/operators/aggregate/count.py
--rw-r--r--   0        0        0      339 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/operators/arithmetic/max_value.py
--rw-r--r--   0        0        0      320 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/operators/arithmetic/min_value.py
--rw-r--r--   0        0        0      691 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/operators/clinical/any_in_valueset.py
--rw-r--r--   0        0        0     1052 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/operators/clinical/in_valueset.py
--rw-r--r--   0        0        0      120 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/operators/comparison/equal.py
--rw-r--r--   0        0        0      511 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/operators/comparison/equivalent.py
--rw-r--r--   0        0        0      735 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/operators/comparison/greater.py
--rw-r--r--   0        0        0      763 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/operators/comparison/greater_or_equal.py
--rw-r--r--   0        0        0      507 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/operators/comparison/in_list.py
--rw-r--r--   0        0        0      726 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/operators/comparison/less.py
--rw-r--r--   0        0        0      753 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/operators/comparison/less_or_equal.py
--rw-r--r--   0        0        0      741 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/operators/comparison/not_equal.py
--rw-r--r--   0        0        0      671 2023-04-21 17:09:29.459947 cqlpy-0.2.2/cqlpy/_internal/operators/cql_in.py
--rw-r--r--   0        0        0     1165 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/date_time/add.py
--rw-r--r--   0        0        0      541 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/date_time/after.py
--rw-r--r--   0        0        0      558 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/date_time/before.py
--rw-r--r--   0        0        0      588 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/date_time/calculate_age_at.py
--rw-r--r--   0        0        0      157 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/date_time/date_time_precision.py
--rw-r--r--   0        0        0      898 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/date_time/difference_between.py
--rw-r--r--   0        0        0      890 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/date_time/duration_between.py
--rw-r--r--   0        0        0      378 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/date_time/same_or_before.py
--rw-r--r--   0        0        0     1181 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/date_time/subtract.py
--rw-r--r--   0        0        0     3800 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/interval/collapse.py
--rw-r--r--   0        0        0      381 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/interval/end.py
--rw-r--r--   0        0        0     1411 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/interval/in_interval.py
--rw-r--r--   0        0        0     1546 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/interval/included_in.py
--rw-r--r--   0        0        0      587 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/interval/overlaps.py
--rw-r--r--   0        0        0      976 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/interval/start.py
--rw-r--r--   0        0        0      348 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/list/distinct.py
--rw-r--r--   0        0        0      230 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/list/exists.py
--rw-r--r--   0        0        0      324 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/list/first.py
--rw-r--r--   0        0        0      291 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/list/flatten.py
--rw-r--r--   0        0        0     2195 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/list/intersect.py
--rw-r--r--   0        0        0      306 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/list/last.py
--rw-r--r--   0        0        0      404 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/list/singleton_from.py
--rw-r--r--   0        0        0      236 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/list/union.py
--rw-r--r--   0        0        0      409 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/nullological/coalesce.py
--rw-r--r--   0        0        0      212 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/nullological/is_false.py
--rw-r--r--   0        0        0      358 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/nullological/is_null.py
--rw-r--r--   0        0        0      193 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/nullological/is_true.py
--rw-r--r--   0        0        0      254 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/sort/sort_by_column.py
--rw-r--r--   0        0        0      134 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/sort/sort_by_direction.py
--rw-r--r--   0        0        0      173 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/sort/sort_by_expression.py
--rw-r--r--   0        0        0       51 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/sort/tuple_sort.py
--rw-r--r--   0        0        0      166 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/string/ends_with.py
--rw-r--r--   0        0        0      170 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/string/split.py
--rw-r--r--   0        0        0      149 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/to_list.py
--rw-r--r--   0        0        0      162 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/type/to_concept.py
--rw-r--r--   0        0        0      280 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/operators/type/to_datetime.py
--rw-r--r--   0        0        0      509 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/parameter.py
--rw-r--r--   0        0        0        0 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/__init__.py
--rw-r--r--   0        0        0     2901 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/any.py
--rw-r--r--   0        0        0      988 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/boolean.py
--rw-r--r--   0        0        0     1700 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/code.py
--rw-r--r--   0        0        0      851 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/code_system.py
--rw-r--r--   0        0        0     2459 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/concept.py
--rw-r--r--   0        0        0     1001 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/date.py
--rw-r--r--   0        0        0     2986 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/datetime.py
--rw-r--r--   0        0        0     1128 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/decimal.py
--rw-r--r--   0        0        0      756 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/integer.py
--rw-r--r--   0        0        0     3674 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/interval.py
--rw-r--r--   0        0        0     1605 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/list.py
--rw-r--r--   0        0        0       81 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/long.py
--rw-r--r--   0        0        0      416 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/null.py
--rw-r--r--   0        0        0      887 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/quantity.py
--rw-r--r--   0        0        0      989 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/string.py
--rw-r--r--   0        0        0     2003 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/types/value_set.py
--rw-r--r--   0        0        0      170 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/_internal/valueset_provider.py
--rw-r--r--   0        0        0      456 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/context.py
--rw-r--r--   0        0        0     4289 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/operators.py
--rw-r--r--   0        0        0        0 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/py.typed
--rw-r--r--   0        0        0     1988 2023-04-21 17:09:29.463947 cqlpy-0.2.2/cqlpy/types.py
--rw-r--r--   0        0        0      586 2023-04-21 17:09:52.136317 cqlpy-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 cqlpy-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-23 01:02:56.408660 cqlpy-0.2.4/LICENSE
+-rw-r--r--   0        0        0        8 2023-05-23 01:02:56.408660 cqlpy-0.2.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-23 01:02:56.408660 cqlpy-0.2.4/cqlpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 01:02:56.408660 cqlpy-0.2.4/cqlpy/_internal/__init__.py
+-rw-r--r--   0        0        0     5073 2023-05-23 01:02:56.408660 cqlpy-0.2.4/cqlpy/_internal/context/context.py
+-rw-r--r--   0        0        0      748 2023-05-23 01:02:56.408660 cqlpy-0.2.4/cqlpy/_internal/context/cql_value_set_provider.py
+-rw-r--r--   0        0        0   335719 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/context/fhir/r4/map.py
+-rw-r--r--   0        0        0    16313 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/context/fhir/r4/model.py
+-rw-r--r--   0        0        0      689 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/context/parameter_provider.py
+-rw-r--r--   0        0        0     2319 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/context/resource_query.py
+-rw-r--r--   0        0        0     1696 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/context/type_factory.py
+-rw-r--r--   0        0        0       92 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/exceptions.py
+-rw-r--r--   0        0        0      123 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/aggregate/count.py
+-rw-r--r--   0        0        0      339 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/arithmetic/max_value.py
+-rw-r--r--   0        0        0      320 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/arithmetic/min_value.py
+-rw-r--r--   0        0        0      691 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/clinical/any_in_valueset.py
+-rw-r--r--   0        0        0     1052 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/clinical/in_valueset.py
+-rw-r--r--   0        0        0      120 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/equal.py
+-rw-r--r--   0        0        0      511 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/equivalent.py
+-rw-r--r--   0        0        0      735 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/greater.py
+-rw-r--r--   0        0        0      763 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/greater_or_equal.py
+-rw-r--r--   0        0        0      507 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/in_list.py
+-rw-r--r--   0        0        0      726 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/less.py
+-rw-r--r--   0        0        0      753 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/less_or_equal.py
+-rw-r--r--   0        0        0      741 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/comparison/not_equal.py
+-rw-r--r--   0        0        0      671 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/cql_in.py
+-rw-r--r--   0        0        0     1165 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/add.py
+-rw-r--r--   0        0        0      541 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/after.py
+-rw-r--r--   0        0        0      558 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/before.py
+-rw-r--r--   0        0        0      588 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/calculate_age_at.py
+-rw-r--r--   0        0        0      157 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/date_time_precision.py
+-rw-r--r--   0        0        0      898 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/difference_between.py
+-rw-r--r--   0        0        0      890 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/duration_between.py
+-rw-r--r--   0        0        0      378 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/same_or_before.py
+-rw-r--r--   0        0        0     1181 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/date_time/subtract.py
+-rw-r--r--   0        0        0     3800 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/interval/collapse.py
+-rw-r--r--   0        0        0      381 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/interval/end.py
+-rw-r--r--   0        0        0     1411 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/interval/in_interval.py
+-rw-r--r--   0        0        0     1546 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/interval/included_in.py
+-rw-r--r--   0        0        0      587 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/interval/overlaps.py
+-rw-r--r--   0        0        0      976 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/interval/start.py
+-rw-r--r--   0        0        0      348 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/distinct.py
+-rw-r--r--   0        0        0      230 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/exists.py
+-rw-r--r--   0        0        0      324 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/first.py
+-rw-r--r--   0        0        0      291 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/flatten.py
+-rw-r--r--   0        0        0     2195 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/intersect.py
+-rw-r--r--   0        0        0      306 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/last.py
+-rw-r--r--   0        0        0      404 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/singleton_from.py
+-rw-r--r--   0        0        0      236 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/list/union.py
+-rw-r--r--   0        0        0      409 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/nullological/coalesce.py
+-rw-r--r--   0        0        0      212 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/nullological/is_false.py
+-rw-r--r--   0        0        0      358 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/nullological/is_null.py
+-rw-r--r--   0        0        0      193 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/nullological/is_true.py
+-rw-r--r--   0        0        0      254 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/sort/sort_by_column.py
+-rw-r--r--   0        0        0      134 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/sort/sort_by_direction.py
+-rw-r--r--   0        0        0      173 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/sort/sort_by_expression.py
+-rw-r--r--   0        0        0       51 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/sort/tuple_sort.py
+-rw-r--r--   0        0        0      166 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/string/ends_with.py
+-rw-r--r--   0        0        0      170 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/string/split.py
+-rw-r--r--   0        0        0      149 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/to_list.py
+-rw-r--r--   0        0        0      162 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/type/to_concept.py
+-rw-r--r--   0        0        0      280 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/operators/type/to_datetime.py
+-rw-r--r--   0        0        0      509 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/parameter.py
+-rw-r--r--   0        0        0     9366 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/scripts/fhir_map_generator.py
+-rw-r--r--   0        0        0        0 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/__init__.py
+-rw-r--r--   0        0        0     2901 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/any.py
+-rw-r--r--   0        0        0      988 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/boolean.py
+-rw-r--r--   0        0        0     1700 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/code.py
+-rw-r--r--   0        0        0      851 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/code_system.py
+-rw-r--r--   0        0        0     2459 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/concept.py
+-rw-r--r--   0        0        0     1001 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/date.py
+-rw-r--r--   0        0        0     2986 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/datetime.py
+-rw-r--r--   0        0        0     1128 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/decimal.py
+-rw-r--r--   0        0        0      756 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/integer.py
+-rw-r--r--   0        0        0     3674 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/interval.py
+-rw-r--r--   0        0        0     1605 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/list.py
+-rw-r--r--   0        0        0       81 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/long.py
+-rw-r--r--   0        0        0      416 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/null.py
+-rw-r--r--   0        0        0      887 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/quantity.py
+-rw-r--r--   0        0        0     1053 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/string.py
+-rw-r--r--   0        0        0     2003 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/types/value_set.py
+-rw-r--r--   0        0        0      170 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/_internal/valueset_provider.py
+-rw-r--r--   0        0        0      451 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/context.py
+-rw-r--r--   0        0        0     4227 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/operators.py
+-rw-r--r--   0        0        0        0 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/providers/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/providers/logger.py
+-rw-r--r--   0        0        0       15 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/providers/requirements.txt
+-rw-r--r--   0        0        0     4871 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/providers/rosetta_valueset_provider.py
+-rw-r--r--   0        0        0        0 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/py.typed
+-rw-r--r--   0        0        0     1089 2023-05-23 01:02:56.412660 cqlpy-0.2.4/cqlpy/types.py
+-rw-r--r--   0        0        0      636 2023-05-23 01:03:18.340855 cqlpy-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 cqlpy-0.2.4/PKG-INFO
```

### Comparing `cqlpy-0.2.2/LICENSE` & `cqlpy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/context/context.py` & `cqlpy-0.2.4/cqlpy/_internal/context/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from typing import Optional, Union
 from cqlpy._internal.context.cql_value_set_provider import CqlValueSetProvider
 
-from cqlpy._internal.context.fhir_r4_data_model import FhirR4DataModel
+from cqlpy._internal.context.fhir.r4.model import FhirR4DataModel
 from cqlpy._internal.context.parameter_provider import ParameterProvider
 from cqlpy._internal.parameter import Parameter
 from cqlpy._internal.types.code import Code
 from cqlpy._internal.types.value_set import ValueSet
 from cqlpy._internal.valueset_provider import ValueSetProvider
```

### Comparing `cqlpy-0.2.2/cqlpy/_internal/context/cql_value_set_provider.py` & `cqlpy-0.2.4/cqlpy/_internal/context/cql_value_set_provider.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/context/fhir_r4_data_model.py` & `cqlpy-0.2.4/cqlpy/_internal/context/fhir/r4/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 import json
-from typing import Iterator, Mapping, Optional, Protocol, Sequence, Union
+from typing import Iterator, Optional, Protocol, Sequence, Union
 
 from cqlpy._internal.context.parameter_provider import ParameterProvider
 from cqlpy._internal.context.resource_query import ResourceQuery
 from cqlpy._internal.context.type_factory import TypeFactory
 from cqlpy._internal.operators.comparison.in_list import in_list
 from cqlpy._internal.operators.list.exists import exists
 from cqlpy._internal.operators.list.intersect import intersect
@@ -13,125 +13,76 @@
 from cqlpy._internal.types.any import CqlAny
 from cqlpy._internal.types.code import Code
 from cqlpy._internal.types.concept import Concept
 from cqlpy._internal.types.datetime import DateTime
 from cqlpy._internal.types.interval import Interval
 from cqlpy._internal.types.null import Null
 from cqlpy._internal.types.value_set import ValueSet
-from cqlpy._internal.valueset_provider import ValueSetProvider
-
-
-FHIR_TO_CQL_TYPE_MAP = {
-    "Condition": {
-        "id": "String",
-        "clinicalStatus": "Concept",
-        "category": "List<Concept>",
-        "code": "Concept",
-        "encounter": "Reference",
-        "claim": "Reference",
-        "onset": "Choice:Interval<DateTime>",
-        "bodySite": "List<Concept>",
-    },
-    "Encounter": {
-        "id": "String",
-        "class": "Code",
-        "type": "List<Concept>",
-        "period": "Interval<DateTime>",
-        "status": "String",
-        "diagnosis": "List<BackboneElement:Diagnosis>",
-        "location": "List<BackboneElement:Location>",
-        "hospitalization": "BackboneElement:EncounterHospitalization",
-    },
-    "Diagnosis": {
-        "condition": "Reference",
-    },
-    "Location": {"location": "String"},
-    "EncounterHospitalization": {
-        "dischargeDisposition": "Concept",
-    },
-    "Extension": {"url": "String", "valueCoding": "Code"},
-    "Reference": {"reference": "String"},
-    "Patient": {
-        "id": "String",
-        "birthDate": "Date",
-        "gender": "String",
-    },
-    "Observation": {
-        "encounter": "Reference",
-        "code": "Concept",
-        "effective": "Choice:Interval<DateTime>",
-    },
-    "Procedure": {
-        "encounter": "Reference",
-        "claim": "Reference",
-        "code": "Concept",
-        "performed": "Choice:Interval<DateTime>",
-        "status": "String",
-    },
-    "DiagnosticReport": {
-        "code": "Concept",
-        "effective": "Choice:Interval<DateTime>",
-        "status": "String",
-    },
-}
+from cqlpy._internal.types.string import String
+from cqlpy._internal.context.fhir.r4.map import FHIR_TO_CQL_MAP
 
 
 class FhirBase:
     def __init__(self, fhir_json: dict, base_type: str):
         self._fhir_json = fhir_json
         self._base_type = base_type
 
     def __str__(self) -> str:
         return json.dumps(self._fhir_json)
 
     def __getitem__(self, property_name: str):
-        if property_name == "extension":
-            if "extension" in self._fhir_json:
-                return [Element(ex, "Extension") for ex in self._fhir_json["extension"]]
-            else:
-                return []
-
-        elif property_name in ["resourceType", "derivedFromResourceType"]:
+        if property_name in ["resourceType", "derivedFromResourceType"]:
             if property_name in self._fhir_json:
                 return self._fhir_json[property_name]
             else:
                 return None
 
-        elif (self._base_type in FHIR_TO_CQL_TYPE_MAP) and (
-            property_name in FHIR_TO_CQL_TYPE_MAP[self._base_type]
+        elif (self._base_type in FHIR_TO_CQL_MAP) and (
+            property_name in FHIR_TO_CQL_MAP[self._base_type]
         ):
-            cql_type_name = FHIR_TO_CQL_TYPE_MAP[self._base_type][property_name]
+            cql_type_name = FHIR_TO_CQL_MAP[self._base_type][property_name]
 
             if cql_type_name == "Choice:Interval<DateTime>":
                 if f"{property_name}DateTime" in self._fhir_json:
                     cql_type, _ = TypeFactory.get_type("DateTime")
                     value = cql_type.parse_fhir_json(
                         self._fhir_json[f"{property_name}DateTime"]
                     )
                     assert isinstance(value, DateTime)
                     return Interval(value, True, value, True)
 
-            elif cql_type_name == "Reference":
-                if property_name in self._fhir_json:
-                    return Element(self._fhir_json[property_name], "Reference")
-                else:
-                    return Element({}, "Reference")
+            elif cql_type_name == "Choice:String":
+                if any(prop.startswith(property_name) for prop in self._fhir_json):
+                    cql_type, _ = TypeFactory.get_type("String")
+                    value = cql_type.parse_fhir_json(self._fhir_json[property_name])
+                    assert isinstance(value, str)
+                    return String(value)
 
             elif "List<BackboneElement:" in cql_type_name:
                 element_name = cql_type_name.split(":")[1].replace(">", "")
 
                 if property_name in self._fhir_json:
                     return [
                         BackboneElement(item, element_name)
                         for item in self._fhir_json[property_name]
                     ]
                 else:
                     return []
 
-            elif "BackboneElement:" in cql_type_name:
+            elif cql_type_name.startswith("List<"):
+                element_name = cql_type_name.split("<")[1].replace(">", "")
+
+                if property_name in self._fhir_json:
+                    cql_type, subtype = TypeFactory.get_type(element_name)
+                    return [
+                        cql_type.parse_fhir_json(item, subtype)
+                        for item in self._fhir_json[property_name]
+                    ]
+
+            elif cql_type_name.startswith("BackboneElement:"):
                 element_name = cql_type_name.split(":")[1]
 
                 if property_name in self._fhir_json:
                     return BackboneElement(self._fhir_json[property_name], element_name)
                 else:
                     return BackboneElement({}, element_name)
```

### Comparing `cqlpy-0.2.2/cqlpy/_internal/context/parameter_provider.py` & `cqlpy-0.2.4/cqlpy/_internal/context/parameter_provider.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/context/resource_query.py` & `cqlpy-0.2.4/cqlpy/_internal/context/resource_query.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/context/type_factory.py` & `cqlpy-0.2.4/cqlpy/_internal/context/type_factory.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/clinical/any_in_valueset.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/clinical/any_in_valueset.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/clinical/in_valueset.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/clinical/in_valueset.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/comparison/greater.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/comparison/greater.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/comparison/greater_or_equal.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/comparison/greater_or_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/comparison/less.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/comparison/less.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/comparison/less_or_equal.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/comparison/less_or_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/comparison/not_equal.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/comparison/not_equal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/cql_in.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/cql_in.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/date_time/add.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/date_time/add.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/date_time/after.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/date_time/after.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/date_time/before.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/date_time/before.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/date_time/calculate_age_at.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/date_time/calculate_age_at.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/date_time/difference_between.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/date_time/difference_between.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/date_time/duration_between.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/date_time/duration_between.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/date_time/subtract.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/date_time/subtract.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/interval/collapse.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/interval/collapse.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/interval/in_interval.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/interval/in_interval.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/interval/included_in.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/interval/included_in.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/interval/overlaps.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/interval/overlaps.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/interval/start.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/interval/start.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/operators/list/intersect.py` & `cqlpy-0.2.4/cqlpy/_internal/operators/list/intersect.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/types/any.py` & `cqlpy-0.2.4/cqlpy/_internal/types/any.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/types/boolean.py` & `cqlpy-0.2.4/cqlpy/_internal/types/boolean.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/types/code.py` & `cqlpy-0.2.4/cqlpy/_internal/types/code.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/types/code_system.py` & `cqlpy-0.2.4/cqlpy/_internal/types/code_system.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/types/concept.py` & `cqlpy-0.2.4/cqlpy/_internal/types/concept.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/types/date.py` & `cqlpy-0.2.4/cqlpy/_internal/types/date.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/types/datetime.py` & `cqlpy-0.2.4/cqlpy/_internal/types/datetime.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/types/decimal.py` & `cqlpy-0.2.4/cqlpy/_internal/types/decimal.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/types/integer.py` & `cqlpy-0.2.4/cqlpy/_internal/types/integer.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/types/interval.py` & `cqlpy-0.2.4/cqlpy/_internal/types/interval.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/types/list.py` & `cqlpy-0.2.4/cqlpy/_internal/types/list.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/types/quantity.py` & `cqlpy-0.2.4/cqlpy/_internal/types/quantity.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/_internal/types/string.py` & `cqlpy-0.2.4/cqlpy/_internal/types/string.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from cqlpy._internal.types.any import CqlAny
 
 
 class String(CqlAny[str, str], str):
     def __init__(self, value: str):
         self.__value = value
 
+    def __hash__(self) -> int:
+        return hash(self.value)
+
     def __new__(cls, value: str):
         return str.__new__(cls, value)
 
     def __repr__(self) -> str:
         return f"String({self.value})"
 
     def __str__(self) -> str:
```

### Comparing `cqlpy-0.2.2/cqlpy/_internal/types/value_set.py` & `cqlpy-0.2.4/cqlpy/_internal/types/value_set.py`

 * *Files identical despite different names*

### Comparing `cqlpy-0.2.2/cqlpy/operators.py` & `cqlpy-0.2.4/cqlpy/operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# For reference
-# https://cql.hl7.org/09-b-cqlreference.html
-
 from cqlpy._internal.operators.aggregate.count import count
 from cqlpy._internal.operators.arithmetic.max_value import max_value
 from cqlpy._internal.operators.arithmetic.min_value import min_value
 from cqlpy._internal.operators.clinical.any_in_valueset import any_in_valueset
 from cqlpy._internal.operators.clinical.in_valueset import in_valueset
 from cqlpy._internal.operators.comparison.equal import equal
 from cqlpy._internal.operators.comparison.equivalent import equivalent
```

### Comparing `cqlpy-0.2.2/cqlpy/types.py` & `cqlpy-0.2.4/cqlpy/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,37 +12,14 @@
 from cqlpy._internal.types.boolean import Boolean
 from cqlpy._internal.types.string import String
 from cqlpy._internal.types.decimal import Decimal
 from cqlpy._internal.types.long import Long
 from cqlpy._internal.types.integer import Integer
 from cqlpy._internal.types.list import List
 
-# For reference
-# https://cql.hl7.org/09-b-cqlreference.html
-# https://rszalski.github.io/magicmethods/
-
-# CQL Structured types implemented as Python classes:
-# 1.1 CqlAny
-# 1.2 Boolean
-# 1.3 Code
-# 1.4 CodeSystem
-# 1.5 Concept
-# 1.6 Date (technically a CQL simple type, but CQL uncertainty and date precision concepts require class implementation)
-# 1.7 DateTime (technically a CQL simple type, but CQL uncertainty and date precision concepts require class implementation)
-# 1.8 Decimal (float)
-# 1.9 Long (int)
-# 1.10 Integer (int)
-# 1.11 Quantity
-# 1.12 Ratio (not yet implemented)
-# 1.13 String
-# 1.14 Time (not yet implemented, technically a CQL simple type, but CQL uncertainty and time precision concepts require class implementation)
-# 1.15 ValueSet (extended to include a codes property)
-# 1.16 Vocabulary (not yet implemented)
-# Parameter (technically not a type, but implemented as one)
-
 __all__ = [
     "Null",
     "CqlAny",
     "CodeSystem",
     "Code",
     "Concept",
     "Date",
```

### Comparing `cqlpy-0.2.2/pyproject.toml` & `cqlpy-0.2.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -3,24 +3,26 @@
   "John Wyderko <john@careevolution.com>",
   "Jeremy Fortune <jeremy@careevolution.com>",
 ]
 description = "Tooling to execute CQL-like Python against FHIR resources."
 license = "MIT"
 name = "cqlpy"
 readme = "README.md"
-version = "0.2.2"
+version = "0.2.4"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
+requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 mypy = "^1.1.1"
 notebook = "^6.5.3"
 types-python-dateutil = "^2.8.19.11"
+types-requests = "^2.30.0.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.4.0"]
```

### Comparing `cqlpy-0.2.2/PKG-INFO` & `cqlpy-0.2.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: cqlpy
-Version: 0.2.2
+Version: 0.2.4
 Summary: Tooling to execute CQL-like Python against FHIR resources.
 License: MIT
 Author: John Wyderko
 Author-email: john@careevolution.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # CQLpy
```

